# Comparing `tmp/python-nomad-1.5.0.tar.gz` & `tmp/python-nomad-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/python-nomad/python-nomad/dist/.tmp-up1js129/python-nomad-1.5.0.tar", last modified: Tue Dec  6 12:23:12 2022, max compression
+gzip compressed data, was "python-nomad-2.0.0.tar", last modified: Fri May 26 15:49:42 2023, max compression
```

## Comparing `python-nomad-1.5.0.tar` & `python-nomad-2.0.0.tar`

### file list

```diff
@@ -1,45 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 12:23:12.000000 python-nomad-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2022-12-06 12:22:19.000000 python-nomad-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2022-12-06 12:23:12.000000 python-nomad-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2022-12-06 12:22:19.000000 python-nomad-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 12:23:12.000000 python-nomad-1.5.0/nomad/
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 12:23:12.000000 python-nomad-1.5.0/nomad/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/allocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/allocations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11250 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/evaluations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10229 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2022-12-06 12:22:19.000000 python-nomad-1.5.0/nomad/api/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 12:23:12.000000 python-nomad-1.5.0/python_nomad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2022-12-06 12:23:12.000000 python-nomad-1.5.0/python_nomad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      862 2022-12-06 12:23:12.000000 python-nomad-1.5.0/python_nomad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 12:23:12.000000 python-nomad-1.5.0/python_nomad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-06 12:23:12.000000 python-nomad-1.5.0/python_nomad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-06 12:23:12.000000 python-nomad-1.5.0/python_nomad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-06 12:23:12.000000 python-nomad-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2022-12-06 12:22:19.000000 python-nomad-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:49:42.474536 python-nomad-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 15:49:31.000000 python-nomad-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-05-26 15:49:42.474536 python-nomad-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-26 15:49:31.000000 python-nomad-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:49:42.466536 python-nomad-2.0.0/nomad/
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:49:42.470536 python-nomad-2.0.0/nomad/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/allocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/allocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:49:42.470536 python-nomad-2.0.0/python_nomad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-05-26 15:49:42.000000 python-nomad-2.0.0/python_nomad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-26 15:49:42.000000 python-nomad-2.0.0/python_nomad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:49:42.000000 python-nomad-2.0.0/python_nomad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 15:49:42.000000 python-nomad-2.0.0/python_nomad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 15:49:42.000000 python-nomad-2.0.0/python_nomad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:49:42.474536 python-nomad-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-26 15:49:31.000000 python-nomad-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:49:42.474536 python-nomad-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_allocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_variables.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-nomad-1.5.0/LICENSE` & `python-nomad-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-nomad-1.5.0/PKG-INFO` & `python-nomad-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: python-nomad
-Version: 1.5.0
+Version: 2.0.0
 Summary: Client library for Hashicorp Nomad
 Home-page: http://github.com/jrxfive/python-nomad
 Author: jrxfive
 Author-email: jrxfive@gmail.com
 License: MIT
 Keywords: nomad hashicorp client
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-nomad-1.5.0/README.md` & `python-nomad-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `python-nomad-1.5.0/nomad/__init__.py` & `python-nomad-2.0.0/nomad/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,85 @@
-import nomad.api as api
+"""Nomad Python library"""
 import os
+from typing import Optional
 
+import requests
 
-class Nomad(object):
+from nomad import api
 
-    def __init__(self,
-                 host='127.0.0.1',
-                 secure=False,
-                 port=4646,
-                 address=os.getenv('NOMAD_ADDR', None),
-                 namespace=os.getenv('NOMAD_NAMESPACE', None),
-                 token=os.getenv('NOMAD_TOKEN', None),
-                 timeout=5,
-                 region=os.getenv('NOMAD_REGION', None),
-                 version='v1',
-                 verify=False,
-                 cert=(os.getenv('NOMAD_CLIENT_CERT', None),
-                       os.getenv('NOMAD_CLIENT_KEY', None)),
-                 session=None):
-        """ Nomad api client
-
-          https://github.com/jrxFive/python-nomad/
-
-           optional arguments:
-            - host (defaults 127.0.0.1), string ip or name of the nomad api server/agent that will be used.
-            - port (defaults 4646), integer port that will be used to connect.
-            - secure (defaults False), define if the protocol is secured or not (https or http)
-            - version (defaults v1), vesion of the api of nomad.
-            - verify (defaults False), verify the certificate when tls/ssl is enabled
-                                at nomad.
-            - cert (defaults empty), cert, or key and cert file to validate the certificate
-                                configured at nomad.
-            - region (defaults None), version of the region to use. It will be used then
-                                regions of the current agent of the connection.
-            - namespace (defaults to None), Specifies the enterpise namespace that will
-                                be use to deploy or to ask info to nomad.
-            - token (defaults to None), Specifies to append ACL token to the headers to
-                                make authentication on secured based nomad environemnts.
-            - session (defaults to None), allows for injecting a prepared requests.Session object that
-                                all requests to Nomad should use.
-           returns: Nomad api client object
-
-           raises:
-             - nomad.api.exceptions.BaseNomadException
-             - nomad.api.exceptions.URLNotFoundNomadException
-             - nomad.api.exceptions.URLNotAuthorizedNomadException
+
+class Nomad:  # pylint: disable=too-many-public-methods,too-many-instance-attributes
+    """
+    Nomad API
+    """
+
+    def __init__(  # pylint: disable=too-many-arguments
+        self,
+        host: str = "127.0.0.1",
+        secure: bool = False,
+        port: int = 4646,
+        address: Optional[str] = os.getenv("NOMAD_ADDR", None),
+        user_agent: Optional[str] = None,
+        namespace: Optional[str] = os.getenv("NOMAD_NAMESPACE", None),
+        token: Optional[str] = os.getenv("NOMAD_TOKEN", None),
+        timeout: int = 5,
+        region: Optional[str] = os.getenv("NOMAD_REGION", None),
+        version: str = "v1",
+        verify: bool = False,
+        cert: tuple = (os.getenv("NOMAD_CLIENT_CERT", None), os.getenv("NOMAD_CLIENT_KEY", None)),
+        session: requests.Session = None,
+    ):
+        """Nomad api client
+
+        https://github.com/jrxFive/python-nomad/
+
+         optional arguments:
+          - host (defaults 127.0.0.1), string ip or name of the nomad api server/agent that will be used.
+          - port (defaults 4646), integer port that will be used to connect.
+          - user_agent (defaults None), custom user agent for requests to Nomad.
+          - secure (defaults False), define if the protocol is secured or not (https or http)
+          - version (defaults v1), version of the api of nomad.
+          - verify (defaults False), verify the certificate when tls/ssl is enabled
+                              at nomad.
+          - cert (defaults empty), cert, or key and cert file to validate the certificate
+                              configured at nomad.
+          - region (defaults None), version of the region to use. It will be used then
+                              regions of the current agent of the connection.
+          - namespace (defaults to None), Specifies the enterprise namespace that will
+                              be use to deploy or to ask info to nomad.
+          - token (defaults to None), Specifies to append ACL token to the headers to
+                              make authentication on secured based nomad environments.
+          - session (defaults to None), allows for injecting a prepared requests.Session object that
+                              all requests to Nomad should use.
+         returns: Nomad api client object
+
+         raises:
+           - nomad.api.exceptions.BaseNomadException
+           - nomad.api.exceptions.URLNotFoundNomadException
+           - nomad.api.exceptions.URLNotAuthorizedNomadException
         """
         self.host = host
         self.secure = secure
         self.port = port
         self.address = address
+        self.user_agent = user_agent
         self.region = region
         self.timeout = timeout
         self.version = version
         self.token = token
         self.verify = verify
         self.cert = cert if all(cert) else ()
         self.session = session
         self.__namespace = namespace
 
         self.requester_settings = {
             "address": self.address,
             "uri": self.get_uri(),
             "port": self.port,
+            "user_agent": self.user_agent,
             "namespace": self.__namespace,
             "token": self.token,
             "timeout": self.timeout,
             "version": self.version,
             "verify": self.verify,
             "cert": self.cert,
             "region": self.region,
@@ -98,126 +111,216 @@
         self._status = api.Status(**self.requester_settings)
         self._system = api.System(**self.requester_settings)
         self._validate = api.Validate(**self.requester_settings)
         self._variable = api.Variable(**self.requester_settings)
         self._variables = api.Variables(**self.requester_settings)
 
     def get_uri(self):
+        """
+        Get Nomad host
+        """
         if self.secure:
             protocol = "https"
         else:
             protocol = "http"
-        return "{protocol}://{host}".format(protocol=protocol, host=self.host)
+        return f"{protocol}://{self.host}"
 
     def get_namespace(self):
+        """
+        Get Nomad namaspace
+        """
         return self.__namespace
 
     def get_token(self):
+        """
+        Get Nomad token
+        """
         return self.token
 
     @property
     def jobs(self):
+        """
+        Jobs API
+        """
         return self._jobs
 
     @property
     def job(self):
+        """
+        Job API
+        """
         return self._job
 
     @property
     def nodes(self):
+        """
+        Nodes API
+        """
         return self._nodes
 
     @property
     def node(self):
+        """
+        Node API
+        """
         return self._node
 
     @property
     def allocations(self):
+        """
+        Allocations API
+        """
         return self._allocations
 
     @property
     def allocation(self):
+        """
+        Allocation API
+        """
         return self._allocation
 
     @property
     def evaluations(self):
+        """
+        Evaluations API
+        """
         return self._evaluations
 
     @property
     def evaluation(self):
+        """
+        Evaluation API
+        """
         return self._evaluation
 
     @property
     def event(self):
+        """
+        Event API
+        """
         return self._event
 
     @property
     def agent(self):
+        """
+        Agent API
+        """
         return self._agent
 
     @property
     def client(self):
+        """
+        Client API
+        """
         return self._client
 
     @property
     def deployments(self):
+        """
+        Deployments API
+        """
         return self._deployments
 
     @property
     def deployment(self):
+        """
+        Deployment API
+        """
         return self._deployment
 
     @property
     def regions(self):
+        """
+        Regions API
+        """
         return self._regions
 
     @property
     def scaling(self):
+        """
+        Scaling API
+        """
         return self._scaling
 
     @property
     def status(self):
+        """
+        Status API
+        """
         return self._status
 
     @property
     def system(self):
+        """
+        System API
+        """
         return self._system
 
     @property
     def operator(self):
+        """
+        Operator API
+        """
         return self._operator
 
     @property
     def validate(self):
+        """
+        Validate API
+        """
         return self._validate
 
     @property
     def namespaces(self):
+        """
+        Namespaces API
+        """
         return self._namespaces
 
     @property
     def namespace(self):
+        """
+        Namespace API
+        """
         return self._namespace
 
     @property
     def acl(self):
+        """
+        ACL API
+        """
         return self._acl
 
     @property
     def sentinel(self):
+        """
+        Sentinel API
+        """
         return self._sentinel
 
     @property
     def search(self):
+        """
+        Search API
+        """
         return self._search
 
     @property
     def metrics(self):
+        """
+        Metrics API
+        """
         return self._metrics
 
     @property
     def variable(self):
+        """
+        Variable API
+        """
         return self._variable
 
     @property
     def variables(self):
-        return self._variables
+        """
+        Variables API
+        """
+        return self._variables
```

### Comparing `python-nomad-1.5.0/nomad/api/__init__.py` & `python-nomad-2.0.0/nomad/api/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Nomad Python library"""
 import nomad.api.exceptions
 from nomad.api.acl import Acl
 from nomad.api.agent import Agent
 from nomad.api.allocation import Allocation
 from nomad.api.allocations import Allocations
 from nomad.api.base import Requester
 from nomad.api.client import Client
@@ -22,8 +23,8 @@
 from nomad.api.scaling import Scaling
 from nomad.api.sentinel import Sentinel
 from nomad.api.search import Search
 from nomad.api.status import Status
 from nomad.api.system import System
 from nomad.api.validate import Validate
 from nomad.api.variable import Variable
-from nomad.api.variables import Variables
+from nomad.api.variables import Variables
```

### Comparing `python-nomad-1.5.0/nomad/api/acl.py` & `python-nomad-2.0.0/nomad/api/acl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,194 +1,194 @@
-import nomad.api.exceptions
+"""Nomad ACL: https://developer.hashicorp.com/nomad/api-docs/acl"""
 
 from nomad.api.base import Requester
 
 
 class Acl(Requester):
     """
     The endpoint manage security ACL and tokens
 
     https://www.nomadproject.io/api/acl-tokens.html
     """
 
     ENDPOINT = "acl"
 
     def __init__(self, **kwargs):
-        super(Acl, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
         raise AttributeError
 
     def generate_bootstrap(self):
-        """ Activate bootstrap token.
+        """Activate bootstrap token.
 
-            https://www.nomadproject.io/api/acl-tokens.html
+        https://www.nomadproject.io/api/acl-tokens.html
 
-            returns: dict
+        returns: dict
 
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request("bootstrap", method="post").json()
 
     def get_tokens(self):
-        """ Get a list of tokens.
+        """Get a list of tokens.
 
-            https://www.nomadproject.io/api/acl-tokens.html
+        https://www.nomadproject.io/api/acl-tokens.html
 
-            returns: list
+        returns: list
 
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
 
         return self.request("tokens", method="get").json()
 
-    def get_token(self, id):
-        """ Retrieve specific token.
+    def get_token(self, id_):
+        """Retrieve specific token.
 
-            https://www.nomadproject.io/api/acl-tokens.html
+        https://www.nomadproject.io/api/acl-tokens.html
 
-            returns: dict
+        returns: dict
 
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request("token", id, method="get").json()
+        return self.request("token", id_, method="get").json()
 
     def get_self_token(self):
-        """ Retrieve self token used for auth.
+        """Retrieve self token used for auth.
 
-            https://www.nomadproject.io/api/acl-tokens.html
+        https://www.nomadproject.io/api/acl-tokens.html
 
-            returns: dict
+        returns: dict
 
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request("token", "self", method="get").json()
 
     def create_token(self, token):
-        """ Create token.
+        """Create token.
 
-            https://www.nomadproject.io/api/acl-tokens.html
+        https://www.nomadproject.io/api/acl-tokens.html
 
-            arguments:
-                token
-            returns: dict
+        arguments:
+            token
+        returns: dict
 
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request("token", json=token, method="post").json()
 
-    def delete_token(self, id):
-        """ Delete specific token.
+    def delete_token(self, id_):
+        """Delete specific token.
 
-            https://www.nomadproject.io/api/acl-tokens.html
+        https://www.nomadproject.io/api/acl-tokens.html
 
-            returns: Boolean
+        returns: Boolean
 
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request("token", id, method="delete").ok
+        return self.request("token", id_, method="delete").ok
 
-    def update_token(self, id, token):
-        """ Update token.
+    def update_token(self, id_, token):
+        """Update token.
 
-            https://www.nomadproject.io/api/acl-tokens.html
+        https://www.nomadproject.io/api/acl-tokens.html
 
-            arguments:
-                - AccdesorID
-                - token
-            returns: dict
+        arguments:
+            - AccdesorID
+            - token
+        returns: dict
 
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request("token", id, json=token, method="post").json()
+        return self.request("token", id_, json=token, method="post").json()
 
     def get_policies(self):
-        """ Get a list of policies.
+        """Get a list of policies.
 
-            https://www.nomadproject.io/api/acl-policies.html
+        https://www.nomadproject.io/api/acl-policies.html
 
-            returns: list
+        returns: list
 
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request("policies", method="get").json()
 
-    def create_policy(self, id, policy):
-        """ Create policy.
+    def create_policy(self, id_, policy):
+        """Create policy.
 
-            https://www.nomadproject.io/api/acl-policies.html
+        https://www.nomadproject.io/api/acl-policies.html
 
-            arguments:
-                - policy
-            returns: request.Response
+        arguments:
+            - policy
+        returns: request.Response
 
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request("policy", id, json=policy, method="post")
+        return self.request("policy", id_, json=policy, method="post")
 
-    def get_policy(self, id):
-        """ Get a spacific.
+    def get_policy(self, id_):
+        """Get a spacific.
 
-            https://www.nomadproject.io/api/acl-policies.html
+        https://www.nomadproject.io/api/acl-policies.html
 
-            returns: dict
+        returns: dict
 
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request("policy", id, method="get").json()
+        return self.request("policy", id_, method="get").json()
 
-    def update_policy(self, id, policy):
-        """ Create policy.
+    def update_policy(self, id_, policy):
+        """Create policy.
 
-            https://www.nomadproject.io/api/acl-policies.html
+        https://www.nomadproject.io/api/acl-policies.html
 
-            arguments:
-                - name
-                - policy
-            returns: request.Response
+        arguments:
+            - name
+            - policy
+        returns: request.Response
 
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request("policy", id, json=policy, method="post")
+        return self.request("policy", id_, json=policy, method="post")
 
-    def delete_policy(self, id):
-        """ Delete specific policy.
+    def delete_policy(self, id_):
+        """Delete specific policy.
 
-            https://www.nomadproject.io/api/acl-policies.html
+        https://www.nomadproject.io/api/acl-policies.html
 
-            arguments:
-                - id
-            returns: Boolean
+        arguments:
+            - id
+        returns: Boolean
 
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request("policy", id, method="delete").ok
+        return self.request("policy", id_, method="delete").ok
```

### Comparing `python-nomad-1.5.0/nomad/api/agent.py` & `python-nomad-2.0.0/nomad/api/agent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,98 +1,97 @@
-import nomad.api.exceptions
-
+"""Nomad Agent: https://developer.hashicorp.com/nomad/api-docs/agent"""
 from nomad.api.base import Requester
 
 
 class Agent(Requester):
-
     """The self endpoint is used to query the state of the target agent."""
+
     ENDPOINT = "agent"
 
     def __init__(self, **kwargs):
-        super(Agent, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        msg = "{0} does not exist".format(item)
+        msg = f"{item} does not exist"
         raise AttributeError(msg)
 
     def get_agent(self):
-        """ Query the state of the target agent.
+        """Query the state of the target agent.
 
-            https://www.nomadproject.io/docs/http/agent-self.html
+        https://www.nomadproject.io/docs/http/agent-self.html
 
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request("self", method="get").json()
 
     def get_members(self):
         """Lists the known members of the gossip pool.
 
-           https://www.nomadproject.io/docs/http/agent-members.html
+        https://www.nomadproject.io/docs/http/agent-members.html
 
-            returns: list
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: list
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request("members", method="get").json()
 
     def get_servers(self):
-        """ Lists the known members of the gossip pool.
+        """Lists the known members of the gossip pool.
 
-            https://www.nomadproject.io/docs/http/agent-servers.html
+        https://www.nomadproject.io/docs/http/agent-servers.html
 
-            returns: list
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: list
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request("servers", method="get").json()
 
     def join_agent(self, addresses):
         """Initiate a join between the agent and target peers.
 
-           https://www.nomadproject.io/docs/http/agent-join.html
+        https://www.nomadproject.io/docs/http/agent-join.html
 
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         params = {"address": addresses}
         return self.request("join", params=params, method="post").json()
 
     def update_servers(self, addresses):
         """Updates the list of known servers to the provided list.
-           Replaces all previous server addresses with the new list.
+        Replaces all previous server addresses with the new list.
 
-           https://www.nomadproject.io/docs/http/agent-servers.html
+        https://www.nomadproject.io/docs/http/agent-servers.html
 
-            returns: 200 status code
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: 200 status code
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         params = {"address": addresses}
         return self.request("servers", params=params, method="post").status_code
 
     def force_leave(self, node):
         """Force a failed gossip member into the left state.
 
-            https://www.nomadproject.io/docs/http/agent-force-leave.html
+        https://www.nomadproject.io/docs/http/agent-force-leave.html
 
-            returns: 200 status code
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: 200 status code
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         params = {"node": node}
         return self.request("force-leave", params=params, method="post").status_code
```

### Comparing `python-nomad-1.5.0/nomad/api/allocation.py` & `python-nomad-2.0.0/nomad/api/allocation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Nomad allocation: https://developer.hashicorp.com/nomad/api-docs/allocations"""
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Allocation(Requester):
     """
@@ -11,59 +12,61 @@
 
     https://www.nomadproject.io/docs/http/alloc.html
     """
 
     ENDPOINT = "allocation"
 
     def __init__(self, **kwargs):
-        super(Allocation, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
         raise AttributeError
 
     def __contains__(self, item):
         try:
             response = self.get_allocation(item)
 
             if response["ID"] == item:
                 return True
+            return False
         except nomad.api.exceptions.URLNotFoundNomadException:
             return False
 
     def __getitem__(self, item):
         try:
             response = self.get_allocation(item)
 
             if response["ID"] == item:
                 return response
-        except nomad.api.exceptions.URLNotFoundNomadException:
             raise KeyError
+        except nomad.api.exceptions.URLNotFoundNomadException as exc:
+            raise KeyError from exc
 
-    def get_allocation(self, id):
-        """ Query a specific allocation.
+    def get_allocation(self, id_: str):
+        """Query a specific allocation.
 
-           https://www.nomadproject.io/docs/http/alloc.html
+        https://www.nomadproject.io/docs/http/alloc.html
 
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, method="get").json()
+        return self.request(id_, method="get").json()
 
-    def stop_allocation(self, id):
-        """ Stop a specific allocation.
+    def stop_allocation(self, id_: str):
+        """Stop a specific allocation.
 
-           https://www.nomadproject.io/api-docs/allocations/#stop-allocation
+        https://www.nomadproject.io/api-docs/allocations/#stop-allocation
 
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, "stop", method="post").json()
+        return self.request(id_, "stop", method="post").json()
```

### Comparing `python-nomad-1.5.0/nomad/api/allocations.py` & `python-nomad-2.0.0/nomad/api/system.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,51 @@
+"""Nomad System API: https://developer.hashicorp.com/nomad/api-docs/system"""
 from nomad.api.base import Requester
 
 
-class Allocations(Requester):
-
+class System(Requester):
     """
-    The allocations endpoint is used to query the status of allocations.
-    By default, the agent's local region is used; another region can be
-    specified using the ?region= query parameter.
+    The system endpoint is used to for system maintenance
+    and should not be necessary for most users.
+    By default, the agent's local region is used.
 
-    https://www.nomadproject.io/docs/http/allocs.html
+    https://www.nomadproject.io/docs/http/system.html
     """
-    ENDPOINT = "allocations"
+
+    ENDPOINT = "system"
 
     def __init__(self, **kwargs):
-        super(Allocations, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        raise AttributeError
+        msg = f"{item} does not exist"
+        raise AttributeError(msg)
+
+    def initiate_garbage_collection(self):
+        """Initiate garbage collection of jobs, evals, allocations and nodes.
+
+        https://www.nomadproject.io/docs/http/system.html
 
-    def __len__(self):
-        response = self.get_allocations()
-        return len(response)
-
-    def __iter__(self):
-        response = self.get_allocations()
-        return iter(response)
-
-    def get_allocations(self, prefix=None, namespace=None):
-        """ Lists all the allocations.
-
-           https://www.nomadproject.io/docs/http/allocs.html
-            arguments:
-              - prefix :(str) optional, specifies a string to filter allocations on based on an prefix.
-                        This is specified as a querystring parameter.
-              - namespace :(str) optional, specifies the target namespace. Specifying * would return all jobs.
-                        This is specified as a querystring parameter.
-            returns: list
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: Boolean
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        params = {"prefix": prefix}
-        if namespace:
-            params["namespace"] = namespace
+        return self.request("gc", method="put").ok
 
-        return self.request(method="get", params=params).json()
+    def reconcile_summaries(self):
+        """This endpoint reconciles the summaries of all registered jobs.
+
+        https://www.nomadproject.io/docs/http/system.html
+
+        returns: Boolean
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
+        """
+        return self.request("reconcile", "summaries", method="put").ok
```

### Comparing `python-nomad-1.5.0/nomad/api/base.py` & `python-nomad-2.0.0/nomad/api/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,114 +1,156 @@
+"""Requester"""
+from typing import Optional
+
 import requests
-import nomad.api.exceptions
 
-from requests.packages.urllib3.exceptions import InsecureRequestWarning
-requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
+import nomad.api.exceptions
 
 
-class Requester(object):
+class Requester:  # pylint: disable=too-many-instance-attributes,too-few-public-methods
+    """
+    Base object for endpoints
+    """
 
     ENDPOINT = ""
 
-    def __init__(self, address=None, uri='http://127.0.0.1', port=4646, namespace=None, token=None, timeout=5, version='v1', verify=False, cert=(), region=None, session=None, **kwargs):
+    def __init__(  # pylint: disable=too-many-arguments
+        self,
+        address: Optional[str] = None,
+        uri: Optional[str] = "http://127.0.0.1",
+        port: int = 4646,
+        user_agent: Optional[str] = None,
+        namespace: Optional[str] = None,
+        token: Optional[str] = None,
+        timeout: int = 5,
+        version: str = "v1",
+        verify: bool = False,
+        cert: tuple = (),
+        region: Optional[str] = None,
+        session: requests.Session = None,
+    ):
         self.uri = uri
         self.port = port
+        self.user_agent = user_agent
         self.namespace = namespace
         self.token = token
         self.timeout = timeout
         self.version = version
         self.verify = verify
         self.cert = cert
         self.address = address
         self.session = session or requests.Session()
         self.region = region
 
     def _endpoint_builder(self, *args):
         if args:
-            u = "/".join(args)
-            return "{v}/".format(v=self.version) + u
+            args_str = "/".join(args)
+            return f"{self.version}/" + args_str
+
+        return "/"
 
     def _required_namespace(self, endpoint):
         required_namespace = [
-                                "job",
-                                "jobs",
-                                "allocation",
-                                "allocations",
-                                "deployment",
-                                "deployments",
-                                "acl",
-                                "client",
-                                "node"
-                             ]
+            "job",
+            "jobs",
+            "allocation",
+            "allocations",
+            "deployment",
+            "deployments",
+            "acl",
+            "client",
+            "node",
+            "variable",
+            "variables",
+        ]
         # split 0 -> Api Version
         # split 1 -> Working Endpoint
-        ENDPOINT_NAME = 1
         endpoint_split = endpoint.split("/")
         try:
-            required = endpoint_split[ENDPOINT_NAME] in required_namespace
-        except:
+            endpoint_name = 1
+            required = endpoint_split[endpoint_name] in required_namespace
+        except IndexError:
             required = False
 
         return required
 
     def _url_builder(self, endpoint):
         url = self.address
 
         if self.address is None:
-            url = "{uri}:{port}".format(uri=self.uri, port=self.port)
-
-        url = "{url}/{endpoint}".format(url=url, endpoint=endpoint)
+            url = f"{self.uri}:{self.port}"
+        url = f"{url}/{endpoint}"
 
         return url
 
     def _query_string_builder(self, endpoint, params=None):
-        qs = {}
+        query_string = {}
 
         if not isinstance(params, dict):
             params = {}
 
+        # Remove parameters that are None
+        params = {key: val for key, val in params.items() if val is not None}
+
         if ("namespace" not in params) and (self.namespace and self._required_namespace(endpoint)):
-            qs["namespace"] = self.namespace
+            query_string["namespace"] = self.namespace
 
         if "region" not in params and self.region:
-            qs["region"] = self.region
+            query_string["region"] = self.region
 
-        return qs
+        return query_string
 
     def request(self, *args, **kwargs):
+        """
+        Send HTTP Request (wrapper around requests)
+        """
         endpoint = self._endpoint_builder(self.ENDPOINT, *args)
         response = self._request(
             endpoint=endpoint,
             method=kwargs.get("method"),
             params=kwargs.get("params", None),
             data=kwargs.get("data", None),
             json=kwargs.get("json", None),
             headers=kwargs.get("headers", None),
             allow_redirects=kwargs.get("allow_redirects", False),
             timeout=kwargs.get("timeout", self.timeout),
-            stream=kwargs.get("stream", False)
+            stream=kwargs.get("stream", False),
         )
 
         return response
 
-    def _request(self, method, endpoint, params=None, data=None, json=None, headers=None, allow_redirects=None, timeout=None, stream=False):
+    def _request(  # pylint: disable=too-many-arguments, too-many-branches
+        self,
+        method,
+        endpoint,
+        params=None,
+        data=None,
+        json=None,
+        headers=None,
+        allow_redirects=None,
+        timeout=None,
+        stream=False,
+    ):
         url = self._url_builder(endpoint)
-        qs = self._query_string_builder(endpoint=endpoint, params=params)
+        query_string = self._query_string_builder(endpoint=endpoint, params=params)
 
         if params:
-            params.update(qs)
+            params.update(query_string)
         else:
-            params = qs
+            params = query_string
 
         if self.token:
-            try:
+            if headers is not None:
                 headers["X-Nomad-Token"] = self.token
-            except TypeError:
+            else:
                 headers = {"X-Nomad-Token": self.token}
 
+        if self.user_agent:
+            headers["User-Agent"] = self.user_agent
+
         response = None
 
         try:
             method = method.lower()
             if method == "get":
                 response = self.session.get(
                     allow_redirects=allow_redirects,
@@ -152,24 +194,24 @@
                     timeout=timeout,
                     url=url,
                     verify=self.verify,
                 )
 
             if response.ok:
                 return response
-            elif response.status_code == 400:
+            if response.status_code == 400:
                 raise nomad.api.exceptions.BadRequestNomadException(response)
-            elif response.status_code == 403:
+            if response.status_code == 403:
                 raise nomad.api.exceptions.URLNotAuthorizedNomadException(response)
-            elif response.status_code == 404:
+            if response.status_code == 404:
                 raise nomad.api.exceptions.URLNotFoundNomadException(response)
-            elif response.status_code == 409:
+            if response.status_code == 409:
                 raise nomad.api.exceptions.VariableConflict(response)
-            else:
-                raise nomad.api.exceptions.BaseNomadException(response)
+
+            raise nomad.api.exceptions.BaseNomadException(response)
 
         except requests.exceptions.ConnectionError as error:
             if all([stream, timeout]):
                 raise nomad.api.exceptions.TimeoutNomadException(error)
 
             raise nomad.api.exceptions.BaseNomadException(error)
```

### Comparing `python-nomad-1.5.0/nomad/api/client.py` & `python-nomad-2.0.0/nomad/api/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,39 @@
+# we want to have backward compatibility here
+# pylint: disable=invalid-name,too-many-instance-attributes,too-many-arguments
+"""Nomad Client: https://developer.hashicorp.com/nomad/api-docs/client"""
 from nomad.api.base import Requester
 
 
-class Client(object):
+class Client:
+    """
+    The /client endpoints are used to interact with the Nomad clients.
+    """
 
     def __init__(self, **kwargs):
         self.ls = ls(**kwargs)
         self.cat = cat(**kwargs)
         self.stat = stat(**kwargs)
         self.stats = stats(**kwargs)
         self.allocation = allocation(**kwargs)
         self.read_at = read_at(**kwargs)
         self.stream_file = stream_file(**kwargs)
         self.stream_logs = stream_logs(**kwargs)
         self.gc_allocation = gc_allocation(**kwargs)
         self.gc_all_allocations = gc_all_allocations(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        raise AttributeError
+        msg = f"{item} does not exist"
+        raise AttributeError(msg)
 
 
 class ls(Requester):
 
     """
     The /fs/ls endpoint is used to list files in an allocation directory.
     This API endpoint is hosted by the Nomad client and requests have to be
@@ -34,33 +41,33 @@
 
     https://www.nomadproject.io/docs/http/client-fs-ls.html
     """
 
     ENDPOINT = "client/fs/ls"
 
     def __init__(self, **kwargs):
-        super(ls, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
-    def list_files(self, id=None, path="/"):
-        """ List files in an allocation directory.
+    def list_files(self, id_=None, path="/"):
+        """List files in an allocation directory.
 
-           https://www.nomadproject.io/docs/http/client-fs-ls.html
+        https://www.nomadproject.io/docs/http/client-fs-ls.html
+
+         arguments:
+           - id_
+           - path
+         returns: list
+         raises:
+           - nomad.api.exceptions.BaseNomadException
+           - nomad.api.exceptions.URLNotFoundNomadException
+        """
+        if id_:
+            return self.request(id_, params={"path": path}, method="get").json()
 
-            arguments:
-              - id
-              - path          
-            returns: list
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
-        """
-        if id:
-            return self.request(id, params={"path": path}, method="get").json()
-        else:
-            return self.request(params={"path": path}, method="get").json()
+        return self.request(params={"path": path}, method="get").json()
 
 
 class cat(Requester):
 
     """
     The /fs/cat endpoint is used to read the contents of a file in an
     allocation directory. This API endpoint is hosted by the Nomad
@@ -69,298 +76,280 @@
 
     https://www.nomadproject.io/docs/http/client-fs-cat.html
     """
 
     ENDPOINT = "client/fs/cat"
 
     def __init__(self, **kwargs):
-        super(cat, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
-    def read_file(self, id=None, path="/"):
-        """ Read contents of a file in an allocation directory.
+    def read_file(self, id_=None, path="/"):
+        """Read contents of a file in an allocation directory.
 
-           https://www.nomadproject.io/docs/http/client-fs-cat.html
+        https://www.nomadproject.io/docs/http/client-fs-cat.html
 
-            arguments:
-              - id
-              - path
-            returns: (str) text
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
-        """
-        if id:
-            return self.request(id, params={"path": path}, method="get").text
-        else:
-            return self.request(params={"path": path}, method="get").text
+         arguments:
+           - id_
+           - path
+         returns: (str) text
+         raises:
+           - nomad.api.exceptions.BaseNomadException
+           - nomad.api.exceptions.URLNotFoundNomadException
+        """
+        if id_:
+            return self.request(id_, params={"path": path}, method="get").text
+
+        return self.request(params={"path": path}, method="get").text
 
 
 class read_at(Requester):
 
     """
     This endpoint reads the contents of a file in an allocation directory at a particular offset and limit.
 
     https://www.nomadproject.io/api/client.html#read-file-at-offset
     """
 
     ENDPOINT = "client/fs/readat"
 
     def __init__(self, **kwargs):
-        super(read_at, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
-    def read_file_offset(self, id, offset, limit, path="/"):
-        """ Read contents of a file in an allocation directory.
+    def read_file_offset(self, id_, offset, limit, path="/"):
+        """Read contents of a file in an allocation directory.
 
-           https://www.nomadproject.io/docs/http/client-fs-cat.html
+        https://www.nomadproject.io/docs/http/client-fs-cat.html
 
-            arguments:
-              - id: (str) allocation_id required
-              - offset: (int) required
-              - limit: (int) required
-              - path: (str) optional
-            returns: (str) text
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.BadRequestNomadException
-        """
-        params = {
-            "path": path,
-            "offset": offset,
-            "limit": limit
-        }
-        return self.request(id, params=params, method="get").text
+         arguments:
+           - id_: (str) allocation_id required
+           - offset: (int) required
+           - limit: (int) required
+           - path: (str) optional
+         returns: (str) text
+         raises:
+           - nomad.api.exceptions.BaseNomadException
+           - nomad.api.exceptions.BadRequestNomadException
+        """
+        params = {"path": path, "offset": offset, "limit": limit}
+        return self.request(id_, params=params, method="get").text
 
 
 class stream_file(Requester):
 
     """
     This endpoint streams the contents of a file in an allocation directory.
 
     https://www.nomadproject.io/api/client.html#stream-file
     """
 
     ENDPOINT = "client/fs/stream"
 
     def __init__(self, **kwargs):
-        super(stream_file, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
-    def stream(self, id, offset, origin, path="/"):
-        """ This endpoint streams the contents of a file in an allocation directory.
+    def stream(self, id_, offset, origin, path="/"):
+        """This endpoint streams the contents of a file in an allocation directory.
 
-            https://www.nomadproject.io/api/client.html#stream-file
+        https://www.nomadproject.io/api/client.html#stream-file
 
-            arguments:
-              - id: (str) allocation_id required
-              - offset: (int) required
-              - origin: (str) either start|end
-              - path: (str) optional
-            returns: (str) text
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.BadRequestNomadException
-        """
-        params = {
-            "path": path,
-            "offset": offset,
-            "origin": origin
-        }
-        return self.request(id, params=params, method="get").text
+        arguments:
+          - id_: (str) allocation_id required
+          - offset: (int) required
+          - origin: (str) either start|end
+          - path: (str) optional
+        returns: (str) text
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.BadRequestNomadException
+        """
+        params = {"path": path, "offset": offset, "origin": origin}
+        return self.request(id_, params=params, method="get").text
 
 
 class stream_logs(Requester):
 
     """
     This endpoint streams a task's stderr/stdout logs.
 
     https://www.nomadproject.io/api/client.html#stream-logs
     """
 
     ENDPOINT = "client/fs/logs"
 
     def __init__(self, **kwargs):
-        super(stream_logs, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
-    def stream(self, id, task, type, follow=False, offset=0, origin="start", plain=False):
-        """ This endpoint streams a task's stderr/stdout logs.
+    def stream(self, id_, task, type_, follow=False, offset=0, origin="start", plain=False):
+        """This endpoint streams a task's stderr/stdout logs.
 
-            https://www.nomadproject.io/api/client.html#stream-logs
+        https://www.nomadproject.io/api/client.html#stream-logs
 
-            arguments:
-              - id: (str) allocation_id required
-              - task: (str) name of the task inside the allocation to stream logs from
-              - type: (str) Specifies the stream to stream. Either "stderr|stdout"
-              - follow: (bool) default false
-              - offset: (int) default 0
-              - origin: (str) either start|end, default "start"
-              - plain: (bool) Return just the plain text without framing. default False
-            returns: (str) text
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.BadRequestNomadException
-        """
-        params = {
-            "task": task,
-            "type": type,
-            "follow": follow,
-            "offset": offset,
-            "origin": origin,
-            "plain": plain
-        }
-        return self.request(id, params=params, method="get").text
+        arguments:
+          - id_: (str) allocation_id required
+          - task: (str) name of the task inside the allocation to stream logs from
+          - type_: (str) Specifies the stream to stream. Either "stderr|stdout"
+          - follow: (bool) default false
+          - offset: (int) default 0
+          - origin: (str) either start|end, default "start"
+          - plain: (bool) Return just the plain text without framing. default False
+        returns: (str) text
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.BadRequestNomadException
+        """
+        params = {"task": task, "type": type_, "follow": follow, "offset": offset, "origin": origin, "plain": plain}
+        return self.request(id_, params=params, method="get").text
 
 
 class stat(Requester):
-
     """
-    The /fs/stat endpoint is used to show stat information 
+    The /fs/stat endpoint is used to show stat information
     This API endpoint is hosted by the Nomad client and requests have to be
     made to the Nomad client where the particular allocation was placed.
 
     https://www.nomadproject.io/docs/http/client-fs-stat.html
     """
 
     ENDPOINT = "client/fs/stat"
 
     def __init__(self, **kwargs):
-        super(stat, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
-    def stat_file(self, id=None, path="/"):
-        """ Stat a file in an allocation directory.
+    def stat_file(self, id_=None, path="/"):
+        """Stat a file in an allocation directory.
 
-           https://www.nomadproject.io/docs/http/client-fs-stat.html
+        https://www.nomadproject.io/docs/http/client-fs-stat.html
 
-            arguments:
-              - id
-              - path
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
-        """
-        if id:
-            return self.request(id, params={"path": path}, method="get").json()
-        else:
-            return self.request(params={"path": path}, method="get").json()
+         arguments:
+           - id_
+           - path
+         returns: dict
+         raises:
+           - nomad.api.exceptions.BaseNomadException
+           - nomad.api.exceptions.URLNotFoundNomadException
+        """
+        if id_:
+            return self.request(id_, params={"path": path}, method="get").json()
 
+        return self.request(params={"path": path}, method="get").json()
 
-class stats(Requester):
 
+class stats(Requester):
     """
     The /stats endpoint queries the actual resources consumed on a node.
     The API endpoint is hosted by the Nomad client and requests have to
     be made to the nomad client whose resource usage metrics are of interest.
 
     https://www.nomadproject.io/api/client.html#read-stats
     """
 
     ENDPOINT = "client/stats"
 
     def __init__(self, **kwargs):
-        super(stats, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def read_stats(self, node_id=None):
-        """ Query the actual resources consumed on a node.
+        """
+        Query the actual resources consumed on a node.
 
-            https://www.nomadproject.io/api/client.html#read-stats
+        https://www.nomadproject.io/api/client.html#read-stats
 
-            arguments:
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request(params={"node_id": node_id}, method="get").json()
 
 
 class allocation(Requester):
-
     """
     The allocation/:alloc_id/stats endpoint is used to query the actual
-    resources consumed by an allocation. The API endpoint is hosted by the 
-    Nomad client and requests have to be made to the nomad client whose 
+    resources consumed by an allocation. The API endpoint is hosted by the
+    Nomad client and requests have to be made to the nomad client whose
     resource usage metrics are of interest.
 
     https://www.nomadproject.io/api/client.html#read-allocation
     """
 
     ENDPOINT = "client/allocation"
 
     def __init__(self, **kwargs):
-        super(allocation, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
-    def read_allocation_stats(self, id):
-        """ Query the actual resources consumed by an allocation.
+    def read_allocation_stats(self, id_):
+        """Query the actual resources consumed by an allocation.
 
-            https://www.nomadproject.io/api/client.html#read-allocation
+        https://www.nomadproject.io/api/client.html#read-allocation
 
-            arguments:
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, "stats", method="get").json()
+        return self.request(id_, "stats", method="get").json()
 
-    def restart_allocation(self, id):
-        """ Restart a specific allocation.
+    def restart_allocation(self, id_):
+        """Restart a specific allocation.
 
-           https://www.nomadproject.io/api-docs/allocations/#restart-allocation
+        https://www.nomadproject.io/api-docs/allocations/#restart-allocation
 
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+         returns: dict
+         raises:
+           - nomad.api.exceptions.BaseNomadException
+           - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, "restart", method="post").json()
+        return self.request(id_, "restart", method="post").json()
 
 
 class gc_allocation(Requester):
 
     """
     This endpoint forces a garbage collection of a particular, stopped allocation on a node.
 
     https://www.nomadproject.io/api/client.html#gc-allocation
     """
 
     ENDPOINT = "client/allocation"
 
     def __init__(self, **kwargs):
-        super(gc_allocation, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
-    def garbage_collect(self, id):
-        """ This endpoint forces a garbage collection of a particular, stopped allocation on a node.
+    def garbage_collect(self, id_):
+        """This endpoint forces a garbage collection of a particular, stopped allocation on a node.
 
-            https://www.nomadproject.io/api/client.html#gc-allocation
+        https://www.nomadproject.io/api/client.html#gc-allocation
 
-            arguments:
-              - id: (str) full allocation_id
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id_: (str) full allocation_id
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        self.request(id, "gc", method="get")
+        self.request(id_, "gc", method="get")
 
 
 class gc_all_allocations(Requester):
-
     """
     This endpoint forces a garbage collection of all stopped allocations on a node.
 
     https://www.nomadproject.io/api/client.html#gc-all-allocation
     """
 
     ENDPOINT = "client/gc"
 
     def __init__(self, **kwargs):
-        super(gc_all_allocations, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def garbage_collect(self, node_id=None):
-        """ This endpoint forces a garbage collection of all stopped allocations on a node.
+        """This endpoint forces a garbage collection of all stopped allocations on a node.
 
-            https://www.nomadproject.io/api/client.html#gc-all-allocation
+        https://www.nomadproject.io/api/client.html#gc-all-allocation
 
-            arguments:
-              - node_id: (str) full allocation_id
-            raises:
-              - nomad.api.exceptions.BaseNomadException
+        arguments:
+          - node_id: (str) full allocation_id
+        raises:
+          - nomad.api.exceptions.BaseNomadException
         """
         self.request(params={"node_id": node_id}, method="get")
```

### Comparing `python-nomad-1.5.0/nomad/api/deployment.py` & `python-nomad-2.0.0/nomad/api/deployment.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,165 +1,172 @@
+"""Nomad Deployment: https://developer.hashicorp.com/nomad/api-docs/deployments"""
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Deployment(Requester):
 
     """
     The /deployment endpoints are used to query for and interact with deployments.
 
     https://www.nomadproject.io/docs/http/deployments.html
     """
+
     ENDPOINT = "deployment"
 
     def __init__(self, **kwargs):
-        super(Deployment, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        msg = "{0} does not exist".format(item)
+        msg = f"{item} does not exist"
         raise AttributeError(msg)
 
     def __contains__(self, item):
-
         try:
-            d = self.get_deployment(item)
+            self.get_deployment(item)
             return True
         except nomad.api.exceptions.URLNotFoundNomadException:
             return False
 
     def __getitem__(self, item):
-
         try:
-            d = self.get_deployment(item)
-
-            if d["ID"] == item:
-                return d
-        except nomad.api.exceptions.URLNotFoundNomadException:
+            deployment = self.get_deployment(item)
+            if deployment["ID"] == item:
+                return deployment
             raise KeyError
+        except nomad.api.exceptions.URLNotFoundNomadException as exp:
+            raise KeyError from exp
 
-    def get_deployment(self, id):
-        """ This endpoint reads information about a specific deployment by ID.
+    def get_deployment(self, id_):
+        """This endpoint reads information about a specific deployment by ID.
 
-           https://www.nomadproject.io/docs/http/deployments.html
+        https://www.nomadproject.io/docs/http/deployments.html
 
-            arguments:
-              - id
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
-        """
-        return self.request(id, method="get").json()
-
-    def get_deployment_allocations(self, id):
-        """ This endpoint lists the allocations created or modified for the given deployment.
-
-           https://www.nomadproject.io/docs/http/deployments.html
-
-            arguments:
-              - id
-            returns: list of dicts
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
-        """
-        return self.request("allocations", id, method="get").json()
-
-    def fail_deployment(self, id):
-        """ This endpoint is used to mark a deployment as failed. This should be done to force the scheduler to stop
-            creating allocations as part of the deployment or to cause a rollback to a previous job version.
-
-           https://www.nomadproject.io/docs/http/deployments.html
-
-            arguments:
-              - id
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
-        """
-        fail_json = {"DeploymentID": id}
-        return self.request("fail", id, json=fail_json, method="post").json()
-
-    def pause_deployment(self, id, pause):
-        """ This endpoint is used to pause or unpause a deployment.
-            This is done to pause a rolling upgrade or resume it.
-
-           https://www.nomadproject.io/docs/http/deployments.html
-
-            arguments:
-              - id
-              - pause, Specifies whether to pause or resume the deployment.
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
-        """
-        pause_json = {"Pause": pause,
-                      "DeploymentID": id}
-        return self.request("pause", id, json=pause_json, method="post").json()
-
-    def promote_deployment_all(self, id, all=True):
-        """ This endpoint is used to promote task groups that have canaries for a deployment. This should be done when
-            the placed canaries are healthy and the rolling upgrade of the remaining allocations should begin.
-
-           https://www.nomadproject.io/docs/http/deployments.html
-
-            arguments:
-              - id
-              - all, Specifies whether all task groups should be promoted.
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
-        """
-        promote_all_json = {"All": all,
-                            "DeploymentID": id}
-        return self.request("promote", id, json=promote_all_json, method="post").json()
-
-    def promote_deployment_groups(self, id, groups=list()):
-        """ This endpoint is used to promote task groups that have canaries for a deployment. This should be done when
-            the placed canaries are healthy and the rolling upgrade of the remaining allocations should begin.
-
-           https://www.nomadproject.io/docs/http/deployments.html
-
-            arguments:
-              - id
-              - groups, (list) Specifies a particular set of task groups that should be promoted
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
-        """
-        promote_groups_json = {"Groups": groups,
-                               "DeploymentID": id}
-        return self.request("promote", id, json=promote_groups_json, method="post").json()
-
-    def deployment_allocation_health(self, id, healthy_allocations=list(), unhealthy_allocations=list()):
-        """ This endpoint is used to set the health of an allocation that is in the deployment manually. In some use
-            cases, automatic detection of allocation health may not be desired. As such those task groups can be marked
-            with an upgrade policy that uses health_check = "manual". Those allocations must have their health marked
-            manually using this endpoint. Marking an allocation as healthy will allow the rolling upgrade to proceed.
-            Marking it as failed will cause the deployment to fail.
-
-           https://www.nomadproject.io/docs/http/deployments.html
-
-            arguments:
-              - id
-              - healthy_allocations, Specifies the set of allocation that should be marked as healthy.
-              - unhealthy_allocations,  Specifies the set of allocation that should be marked as unhealthy.
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
-        """
-        allocations = {"HealthyAllocationIDs": healthy_allocations,
-                       "UnHealthyAllocationIDs": unhealthy_allocations,
-                       "DeploymentID": id}
-        return self.request("allocation-health", id, json=allocations, method="post").json()
+        arguments:
+          - id_
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
+        """
+        return self.request(id_, method="get").json()
+
+    def get_deployment_allocations(self, id_):
+        """This endpoint lists the allocations created or modified for the given deployment.
+
+        https://www.nomadproject.io/docs/http/deployments.html
+
+        arguments:
+          - id_
+        returns: list of dicts
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
+        """
+        return self.request("allocations", id_, method="get").json()
+
+    def fail_deployment(self, id_):
+        """This endpoint is used to mark a deployment as failed. This should be done to force the scheduler to stop
+         creating allocations as part of the deployment or to cause a rollback to a previous job version.
+
+        https://www.nomadproject.io/docs/http/deployments.html
+
+         arguments:
+           - id_
+         returns: dict
+         raises:
+           - nomad.api.exceptions.BaseNomadException
+           - nomad.api.exceptions.URLNotFoundNomadException
+        """
+        fail_json = {"DeploymentID": id_}
+        return self.request("fail", id_, json=fail_json, method="post").json()
+
+    def pause_deployment(self, id_, pause):
+        """This endpoint is used to pause or unpause a deployment.
+         This is done to pause a rolling upgrade or resume it.
+
+        https://www.nomadproject.io/docs/http/deployments.html
+
+        arguments:
+          - id_
+          - pause, Specifies whether to pause or resume the deployment.
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
+        """
+        pause_json = {"Pause": pause, "DeploymentID": id_}
+        return self.request("pause", id_, json=pause_json, method="post").json()
+
+    def promote_deployment_all(self, id_, _all=True):
+        """This endpoint is used to promote task groups that have canaries for a deployment. This should be done when
+         the placed canaries are healthy and the rolling upgrade of the remaining allocations should begin.
+
+        https://www.nomadproject.io/docs/http/deployments.html
+
+        arguments:
+          - id_
+          - _all, Specifies whether all task groups should be promoted.
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
+        """
+        promote_all_json = {"All": _all, "DeploymentID": id_}
+        return self.request("promote", id_, json=promote_all_json, method="post").json()
+
+    def promote_deployment_groups(self, id_, groups=None):
+        """This endpoint is used to promote task groups that have canaries for a deployment. This should be done when
+        the placed canaries are healthy and the rolling upgrade of the remaining allocations should begin.
+
+        https://www.nomadproject.io/docs/http/deployments.html
+
+        arguments:
+          - id_
+          - groups, (list) Specifies a particular set of task groups that should be promoted
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
+        """
+        if groups is None:
+            groups = []
+        promote_groups_json = {"Groups": groups, "DeploymentID": id_}
+        return self.request("promote", id_, json=promote_groups_json, method="post").json()
+
+    def deployment_allocation_health(self, id_, healthy_allocations=None, unhealthy_allocations=None):
+        """This endpoint is used to set the health of an allocation that is in the deployment manually. In some use
+        cases, automatic detection of allocation health may not be desired. As such those task groups can be marked
+        with an upgrade policy that uses health_check = "manual". Those allocations must have their health marked
+        manually using this endpoint. Marking an allocation as healthy will allow the rolling upgrade to proceed.
+        Marking it as failed will cause the deployment to fail.
+
+        https://www.nomadproject.io/docs/http/deployments.html
+
+        arguments:
+          - id_
+          - healthy_allocations, Specifies the set of allocation that should be marked as healthy.
+          - unhealthy_allocations,  Specifies the set of allocation that should be marked as unhealthy.
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
+        """
+        if healthy_allocations is None:
+            healthy_allocations = []
+
+        if unhealthy_allocations is None:
+            unhealthy_allocations = []
+
+        allocations = {
+            "HealthyAllocationIDs": healthy_allocations,
+            "UnHealthyAllocationIDs": unhealthy_allocations,
+            "DeploymentID": id_,
+        }
+        return self.request("allocation-health", id_, json=allocations, method="post").json()
```

### Comparing `python-nomad-1.5.0/nomad/api/deployments.py` & `python-nomad-2.0.0/nomad/api/deployments.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+"""Nomad Deployment: https://developer.hashicorp.com/nomad/api-docs/deployments"""
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Deployments(Requester):
-
     """
     The /deployment endpoints are used to query for and interact with deployments.
 
     https://www.nomadproject.io/docs/http/deployments.html
     """
+
     ENDPOINT = "deployments"
 
     def __init__(self, **kwargs):
-        super(Deployments, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
         raise AttributeError
 
     def __len__(self):
         response = self.get_deployments()
         return len(response)
@@ -31,49 +32,46 @@
     def __iter__(self):
         response = self.get_deployments()
         return iter(response)
 
     def __contains__(self, item):
         try:
             deployments = self.get_deployments()
-
-            for d in deployments:
-                if d["ID"] == item:
+            for deployment in deployments:
+                if deployment["ID"] == item:
                     return True
-            else:
-                return False
+
+            return False
         except nomad.api.exceptions.URLNotFoundNomadException:
             return False
 
     def __getitem__(self, item):
         try:
             deployments = self.get_deployments()
-
-            for d in deployments:
-                if d["ID"] == item:
-                    return d
-            else:
-                raise KeyError
-        except nomad.api.exceptions.URLNotFoundNomadException:
+            for deployment in deployments:
+                if deployment["ID"] == item:
+                    return deployment
             raise KeyError
+        except nomad.api.exceptions.URLNotFoundNomadException as exc:
+            raise KeyError from exc
 
     def get_deployments(self, prefix="", namespace=None):
-        """ This endpoint lists all deployments.
+        """This endpoint lists all deployments.
 
-           https://www.nomadproject.io/docs/http/deployments.html
+        https://www.nomadproject.io/docs/http/deployments.html
 
-            optional_arguments:
-              - prefix, (default "") Specifies a string to filter deployments on based on an index prefix.
-                        This is specified as a querystring parameter.
-              - namespace :(str) optional, specifies the target namespace. Specifying * would return all jobs.
-                        This is specified as a querystring parameter.
-
-            returns: list of dicts
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        optional_arguments:
+          - prefix, (default "") Specifies a string to filter deployments on based on an index prefix.
+                This is specified as a querystring parameter.
+          - namespace :(str) optional, specifies the target namespace. Specifying * would return all jobs.
+                This is specified as a querystring parameter.
+
+        returns: list of dicts
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         params = {"prefix": prefix}
         if namespace:
             params["namespace"] = namespace
 
         return self.request(params=params, method="get").json()
```

### Comparing `python-nomad-1.5.0/nomad/api/evaluation.py` & `python-nomad-2.0.0/nomad/api/evaluation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,73 @@
+"""Nomad Evaluation: https://developer.hashicorp.com/nomad/api-docs/evaluations"""
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Evaluation(Requester):
-
     """
     The evaluation endpoint is used to query a specific evaluations.
     By default, the agent's local region is used; another region can
     be specified using the ?region= query parameter.
 
     https://www.nomadproject.io/docs/http/eval.html
     """
+
     ENDPOINT = "evaluation"
 
     def __init__(self, **kwargs):
-        super(Evaluation, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        msg = "{0} does not exist".format(item)
+        msg = f"{item} does not exist"
         raise AttributeError(msg)
 
     def __contains__(self, item):
-
         try:
-            e = self.get_evaluation(item)
+            self.get_evaluation(item)
             return True
         except nomad.api.exceptions.URLNotFoundNomadException:
             return False
 
     def __getitem__(self, item):
-
         try:
-            e = self.get_evaluation(item)
-
-            if e["ID"] == item:
-                return e
-        except nomad.api.exceptions.URLNotFoundNomadException:
+            evaluation = self.get_evaluation(item)
+            if evaluation["ID"] == item:
+                return evaluation
             raise KeyError
+        except nomad.api.exceptions.URLNotFoundNomadException as exc:
+            raise KeyError from exc
 
-    def get_evaluation(self, id):
-        """ Query a specific evaluation.
+    def get_evaluation(self, id_):
+        """Query a specific evaluation.
 
-           https://www.nomadproject.io/docs/http/eval.html
+        https://www.nomadproject.io/docs/http/eval.html
 
-            arguments:
-              - id
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+         arguments:
+           - id_
+         returns: dict
+         raises:
+           - nomad.api.exceptions.BaseNomadException
+           - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, method="get").json()
+        return self.request(id_, method="get").json()
 
-    def get_allocations(self, id):
-        """ Query the allocations created or modified by an evaluation.
+    def get_allocations(self, id_):
+        """Query the allocations created or modified by an evaluation.
 
-           https://www.nomadproject.io/docs/http/eval.html
+        https://www.nomadproject.io/docs/http/eval.html
 
-            arguments:
-              - id
-            returns: list
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+         arguments:
+           - id_
+         returns: list
+         raises:
+           - nomad.api.exceptions.BaseNomadException
+           - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, "allocations", method="get").json()
+        return self.request(id_, "allocations", method="get").json()
```

### Comparing `python-nomad-1.5.0/nomad/api/evaluations.py` & `python-nomad-2.0.0/nomad/api/evaluations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,74 @@
+"""Nomad Evaluations: https://developer.hashicorp.com/nomad/api-docs/evaluations"""
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
-class Evaluations(Requester):
 
+class Evaluations(Requester):
     """
     The evaluations endpoint is used to query the status of evaluations.
     By default, the agent's local region is used; another region can
     be specified using the ?region= query parameter.
 
     https://www.nomadproject.io/docs/http/evals.html
     """
+
     ENDPOINT = "evaluations"
 
     def __init__(self, **kwargs):
-        super(Evaluations, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
         raise AttributeError
 
     def __contains__(self, item):
         try:
             evaluations = self.get_evaluations()
 
-            for e in evaluations:
-                if e["ID"] == item:
+            for evaluation in evaluations:
+                if evaluation["ID"] == item:
                     return True
-            else:
-                return False
+
+            return False
         except nomad.api.exceptions.URLNotFoundNomadException:
             return False
 
     def __len__(self):
         evaluations = self.get_evaluations()
         return len(evaluations)
 
     def __getitem__(self, item):
         try:
             evaluations = self.get_evaluations()
 
-            for e in evaluations:
-                if e["ID"] == item:
-                    return e
-            else:
-                raise KeyError
-        except nomad.api.exceptions.URLNotFoundNomadException:
+            for evaluation in evaluations:
+                if evaluation["ID"] == item:
+                    return evaluation
             raise KeyError
+        except nomad.api.exceptions.URLNotFoundNomadException as exc:
+            raise KeyError from exc
 
     def __iter__(self):
         evaluations = self.get_evaluations()
         return iter(evaluations)
 
     def get_evaluations(self, prefix=None):
-        """ Lists all the evaluations.
+        """Lists all the evaluations.
 
-           https://www.nomadproject.io/docs/http/evals.html
-            arguments:
-              - prefix :(str) optional, specifies a string to filter evaluations on based on an prefix.
-                        This is specified as a querystring parameter.
-            returns: list
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        https://www.nomadproject.io/docs/http/evals.html
+        arguments:
+          - prefix :(str) optional, specifies a string to filter evaluations on based on an prefix.
+                    This is specified as a querystring parameter.
+        returns: list
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         params = {"prefix": prefix}
         return self.request(method="get", params=params).json()
```

### Comparing `python-nomad-1.5.0/nomad/api/event.py` & `python-nomad-2.0.0/nomad/api/event.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,49 @@
+"""Nomad Events: https://developer.hashicorp.com/nomad/api-docs/events"""
 import json
 import threading
+import queue
 
 import requests
 
 from nomad.api.base import Requester
-from nomad.api.exceptions import TimeoutNomadException
 
-try:
-    import queue
-except ImportError:
-    import Queue as queue
 
-
-class Event(object):
+class Event:
+    """
+    Nomad Event
+    """
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
         raise AttributeError
 
     def __init__(self, **kwargs):
         self.stream = stream(**kwargs)
 
 
-class stream(Requester):
+# backward compatibility
+class stream(Requester):  # pylint: disable=invalid-name
     """
     The /event/stream endpoint is used to stream events generated by Nomad.
 
     https://www.nomadproject.io/api-docs/events
     """
 
     ENDPOINT = "event/stream"
 
     def __init__(self, **kwargs):
-        super(stream, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
-    def _get_stream(self, method, params, timeout, event_queue, exit_event):
+    def _get_stream(self, method, params, timeout, event_queue, exit_event):  # pylint: disable=too-many-arguments
         """
         Used as threading target, to obtain json() value
         Args:
             method:
             params:
             timeout:
             event_queue:
@@ -62,30 +62,33 @@
 
                         if exit_event.is_set():
                             return
 
             except requests.exceptions.ConnectionError:
                 continue
 
-    def get_stream(self, index=0, topic=None, namespace=None, event_queue=None, timeout=None):
+    def get_stream(
+        self, index=0, topic=None, namespace=None, event_queue=None, timeout=None
+    ):  # pylint: disable=too-many-arguments
         """
         Usage:
             stream, stream_exit_event, events = n.event.stream.get_stream()
             stream.start()
 
             while True:
                 event = events.get()
                 print(event)
                 events.task_done()
 
         Args:
             index: (int),  Specifies the index to start streaming events from. If the requested index is no longer
                 in the buffer the stream will start at the next available index.
 
-            topic: (None or dict), Specifies a topic to subscribe to and filter on. The default is to subscribe to all topics.
+            topic: (None or dict), Specifies a topic to subscribe to and filter on.
+                The default is to subscribe to all topics.
                 Multiple topics may be specified by passing multiple topic parameters.
                 A valid topic parameter includes a topic type and an optional filter_key separated by a colon :.
                 As an example ?topic=Deployment:redis would subscribe to all Deployment events for a job redis.
                 an additional topic &topic=Deployment:web would include deployment events for redis and web.
                 To only subscribe to Node events a topic parameter of ?topic=Node without a separator value
                 would be used. ?topic=Node:* is also valid.
 
@@ -118,12 +121,12 @@
             name="python-nomad-event-stream",
             target=self._get_stream,
             kwargs={
                 "method": "get",
                 "params": params,
                 "timeout": timeout,
                 "event_queue": event_queue,
-                "exit_event": stream_exit_event
-            }
+                "exit_event": stream_exit_event,
+            },
         )
 
         return _stream, stream_exit_event, event_queue
```

### Comparing `python-nomad-1.5.0/nomad/api/exceptions.py` & `python-nomad-2.0.0/nomad/api/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+"""Internal library exceptions"""
 import requests
 
 
 class BaseNomadException(Exception):
     """General Error occurred when interacting with nomad API"""
+
     def __init__(self, nomad_resp):
         self.nomad_resp = nomad_resp
 
     def __str__(self):
         if isinstance(self.nomad_resp, requests.Response) and hasattr(self.nomad_resp, "text"):
-            return 'The {0} was raised with following response: {1}.'.format(self.__class__.__name__, self.nomad_resp.text)
-        else:
-            return 'The {0} was raised due to the following error: {1}'.format(self.__class__.__name__,  str(self.nomad_resp))
+            return f"The {self.__class__.__name__} was raised with following response: {self.nomad_resp.text}."
+
+        return f"The {self.__class__.__name__} was raised due to the following error: {self.nomad_resp}"
 
 
 class URLNotFoundNomadException(BaseNomadException):
     """The requeted URL given does not exist"""
 
 
 class URLNotAuthorizedNomadException(BaseNomadException):
```

### Comparing `python-nomad-1.5.0/nomad/api/job.py` & `python-nomad-2.0.0/nomad/api/job.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,304 +1,299 @@
+"""Nomad job: https://developer.hashicorp.com/nomad/api-docs/jobs"""
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Job(Requester):
-
     """
     The job endpoint is used for CRUD on a single job.
     By default, the agent's local region is used.
 
     https://www.nomadproject.io/docs/http/job.html
     """
+
     ENDPOINT = "job"
 
     def __init__(self, **kwargs):
-        super(Job, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        msg = "{0} does not exist".format(item)
+        msg = f"{item} does not exist"
         raise AttributeError(msg)
 
     def __contains__(self, item):
-
         try:
-            j = self.get_job(item)
+            self.get_job(item)
             return True
         except nomad.api.exceptions.URLNotFoundNomadException:
             return False
 
     def __getitem__(self, item):
-
         try:
-            j = self.get_job(item)
+            job = self.get_job(item)
+            if job["ID"] == item:
+                return job
+            if job["Name"] == item:
+                return job
 
-            if j["ID"] == item:
-                return j
-            if j["Name"] == item:
-                return j
-            else:
-                raise KeyError
-        except nomad.api.exceptions.URLNotFoundNomadException:
             raise KeyError
+        except nomad.api.exceptions.URLNotFoundNomadException as exc:
+            raise KeyError from exc
 
-    def get_job(self, id, namespace=None):
-        """ Query a single job for its specification and status.
+    def get_job(self, id_, namespace=None):
+        """Query a single job for its specification and status.
 
-           https://www.nomadproject.io/docs/http/job.html
+        https://www.nomadproject.io/docs/http/job.html
 
-            arguments:
-              - id
-              - namespace :(str) optional, specifies the target namespace. Specifying * would return all jobs.
-                        This is specified as a querystring parameter.
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id_
+          - namespace :(str) optional, specifies the target namespace. Specifying * would return all jobs.
+                    This is specified as a querystring parameter.
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         params = {}
 
         if namespace:
             params["namespace"] = namespace
 
-        return self.request(id, method="get", params=params).json()
+        return self.request(id_, method="get", params=params).json()
 
-    def get_versions(self, id):
-        """ This endpoint reads information about all versions of a job.
+    def get_versions(self, id_):
+        """This endpoint reads information about all versions of a job.
 
-           https://www.nomadproject.io/docs/http/job.html
+        https://www.nomadproject.io/docs/http/job.html
 
-            arguments:
-              - id
-            returns: list of dicts
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id
+        returns: list of dicts
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, "versions", method="get").json()
+        return self.request(id_, "versions", method="get").json()
 
-    def get_allocations(self, id):
-        """ Query the allocations belonging to a single job.
+    def get_allocations(self, id_):
+        """Query the allocations belonging to a single job.
 
-           https://www.nomadproject.io/docs/http/job.html
+        https://www.nomadproject.io/docs/http/job.html
 
-            arguments:
-              - id
-            returns: list
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id_
+        returns: list
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, "allocations", method="get").json()
+        return self.request(id_, "allocations", method="get").json()
 
-    def get_evaluations(self, id):
-        """ Query the evaluations belonging to a single job.
+    def get_evaluations(self, id_):
+        """Query the evaluations belonging to a single job.
 
-           https://www.nomadproject.io/docs/http/job.html
+        https://www.nomadproject.io/docs/http/job.html
 
-            arguments:
-              - id
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id_
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, "evaluations", method="get").json()
+        return self.request(id_, "evaluations", method="get").json()
 
-    def get_deployments(self, id):
-        """ This endpoint lists a single job's deployments
+    def get_deployments(self, id_):
+        """This endpoint lists a single job's deployments
 
-           https://www.nomadproject.io/docs/http/job.html
+        https://www.nomadproject.io/docs/http/job.html
 
-            arguments:
-              - id
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id_
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, "deployments", method="get").json()
+        return self.request(id_, "deployments", method="get").json()
 
-    def get_deployment(self, id):
-        """ This endpoint returns a single job's most recent deployment.
+    def get_deployment(self, id_):
+        """This endpoint returns a single job's most recent deployment.
 
-           https://www.nomadproject.io/docs/http/job.html
+        https://www.nomadproject.io/docs/http/job.html
 
-            arguments:
-              - id
-            returns: list of dicts
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id_
+        returns: list of dicts
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, "deployment", method="get").json()
+        return self.request(id_, "deployment", method="get").json()
 
-    def get_summary(self, id):
-        """ Query the summary of a job.
+    def get_summary(self, id_):
+        """Query the summary of a job.
 
-           https://www.nomadproject.io/docs/http/job.html
+        https://www.nomadproject.io/docs/http/job.html
 
-            arguments:
-              - id
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id_
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, "summary", method="get").json()
+        return self.request(id_, "summary", method="get").json()
 
-    def register_job(self, id, job):
-        """ Registers a new job or updates an existing job
+    def register_job(self, id_, job):
+        """Registers a new job or updates an existing job
 
-           https://www.nomadproject.io/docs/http/job.html
+        https://www.nomadproject.io/docs/http/job.html
 
-            arguments:
-              - id
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id_
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, json=job, method="post").json()
+        return self.request(id_, json=job, method="post").json()
 
-    def evaluate_job(self, id):
-        """ Creates a new evaluation for the given job.
-            This can be used to force run the scheduling logic if necessary.
+    def evaluate_job(self, id_):
+        """Creates a new evaluation for the given job.
+        This can be used to force run the scheduling logic if necessary.
 
-           https://www.nomadproject.io/docs/http/job.html
+        https://www.nomadproject.io/docs/http/job.html
 
-            arguments:
-              - id
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id_
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, "evaluate", method="post").json()
+        return self.request(id_, "evaluate", method="post").json()
 
-    def plan_job(self, id, job, diff=False, policy_override=False):
-        """ Invoke a dry-run of the scheduler for the job.
+    def plan_job(self, id_, job, diff=False, policy_override=False):
+        """Invoke a dry-run of the scheduler for the job.
 
-           https://www.nomadproject.io/docs/http/job.html
+        https://www.nomadproject.io/docs/http/job.html
 
-            arguments:
-              - id
-              - job, dict
-              - diff, boolean
-              - policy_override, boolean
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id_
+          - job, dict
+          - diff, boolean
+          - policy_override, boolean
+         returns: dict
+         raises:
+           - nomad.api.exceptions.BaseNomadException
+           - nomad.api.exceptions.URLNotFoundNomadException
         """
         json_dict = {}
         json_dict.update(job)
-        json_dict.setdefault('Diff', diff)
-        json_dict.setdefault('PolicyOverride', policy_override)
-        return self.request(id, "plan", json=json_dict, method="post").json()
-
-    def periodic_job(self, id):
-        """ Forces a new instance of the periodic job. A new instance will be
-            created even if it violates the job's prohibit_overlap settings.
-            As such, this should be only used to immediately
-            run a periodic job.
-
-           https://www.nomadproject.io/docs/http/job.html
-
-            arguments:
-              - id
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
-        """
-        return self.request(id, "periodic", "force", method="post").json()
-
-    def dispatch_job(self, id, payload=None, meta=None):
-        """ Dispatches a new instance of a parameterized job.
-
-           https://www.nomadproject.io/docs/http/job.html
-
-            arguments:
-              - id
-              - payload
-              - meta
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        json_dict.setdefault("Diff", diff)
+        json_dict.setdefault("PolicyOverride", policy_override)
+        return self.request(id_, "plan", json=json_dict, method="post").json()
+
+    def periodic_job(self, id_):
+        """Forces a new instance of the periodic job. A new instance will be
+         created even if it violates the job's prohibit_overlap settings.
+         As such, this should be only used to immediately
+         run a periodic job.
+
+        https://www.nomadproject.io/docs/http/job.html
+
+        arguments:
+          - id_
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
+        """
+        return self.request(id_, "periodic", "force", method="post").json()
+
+    def dispatch_job(self, id_, payload=None, meta=None):
+        """Dispatches a new instance of a parameterized job.
+
+        https://www.nomadproject.io/docs/http/job.html
+
+        arguments:
+          - id_
+          - payload
+          - meta
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         dispatch_json = {"Meta": meta, "Payload": payload}
-        return self.request(id, "dispatch", json=dispatch_json, method="post").json()
+        return self.request(id_, "dispatch", json=dispatch_json, method="post").json()
 
-    def revert_job(self, id, version, enforce_prior_version=None):
-        """ This endpoint reverts the job to an older version.
+    def revert_job(self, id_, version, enforce_prior_version=None):
+        """This endpoint reverts the job to an older version.
 
-           https://www.nomadproject.io/docs/http/job.html
+        https://www.nomadproject.io/docs/http/job.html
 
-            arguments:
-              - id
-              - version, Specifies the job version to revert to.
-            optional_arguments:
-              - enforce_prior_version, Optional value specifying the current job's version.
-                                       This is checked and acts as a check-and-set value before reverting to the
-                                       specified job.
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
-        """
-        revert_json = {"JobID": id,
-                       "JobVersion": version,
-                       "EnforcePriorVersion": enforce_prior_version}
-        return self.request(id, "revert", json=revert_json, method="post").json()
-
-    def stable_job(self, id, version, stable):
-        """ This endpoint sets the job's stability.
-
-           https://www.nomadproject.io/docs/http/job.html
-
-            arguments:
-              - id
-              - version, Specifies the job version to revert to.
-              - stable, Specifies whether the job should be marked as stable or not.
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
-        """
-        revert_json = {"JobID": id,
-                       "JobVersion": version,
-                       "Stable": stable}
-        return self.request(id, "stable", json=revert_json, method="post").json()
-
-    def deregister_job(self, id, purge=None):
-        """ Deregisters a job, and stops all allocations part of it.
-
-           https://www.nomadproject.io/docs/http/job.html
-
-            arguments:
-              - id
-              - purge (bool), optionally specifies whether the job should be
-                stopped and purged immediately (`purge=True`) or deferred to the
-                Nomad garbage collector (`purge=False`).
-
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
-              - nomad.api.exceptions.InvalidParameters
+        arguments:
+           - id_
+           - version, Specifies the job version to revert to.
+        optional_arguments:
+          - enforce_prior_version, Optional value specifying the current job's version.
+                                   This is checked and acts as a check-and-set value before reverting to the
+                                   specified job.
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
+        """
+        revert_json = {"JobID": id_, "JobVersion": version, "EnforcePriorVersion": enforce_prior_version}
+        return self.request(id_, "revert", json=revert_json, method="post").json()
+
+    def stable_job(self, id_, version, stable):
+        """This endpoint sets the job's stability.
+
+        https://www.nomadproject.io/docs/http/job.html
+
+        arguments:
+          - id_
+          - version, Specifies the job version to revert to.
+          - stable, Specifies whether the job should be marked as stable or not.
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
+        """
+        revert_json = {"JobID": id_, "JobVersion": version, "Stable": stable}
+        return self.request(id_, "stable", json=revert_json, method="post").json()
+
+    def deregister_job(self, id_, purge=None):
+        """Deregisters a job, and stops all allocations part of it.
+
+        https://www.nomadproject.io/docs/http/job.html
+
+        arguments:
+          - id_
+          - purge (bool), optionally specifies whether the job should be
+            stopped and purged immediately (`purge=True`) or deferred to the
+            Nomad garbage collector (`purge=False`).
+
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
+          - nomad.api.exceptions.InvalidParameters
         """
         params = None
         if purge is not None:
             if not isinstance(purge, bool):
-                raise nomad.api.exceptions.InvalidParameters("purge is invalid "
-                        "(expected type %s but got %s)"%(type(bool()), type(purge)))
+                raise nomad.api.exceptions.InvalidParameters(
+                    "purge is invalid " f"(expected type {type(bool())} but got {type(purge)})"
+                )
             params = {"purge": purge}
-        return self.request(id, params=params, method="delete").json()
+        return self.request(id_, params=params, method="delete").json()
```

### Comparing `python-nomad-1.5.0/nomad/api/jobs.py` & `python-nomad-2.0.0/nomad/api/jobs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,48 @@
+"""Nomad job: https://developer.hashicorp.com/nomad/api-docs/jobs"""
+from typing import Optional
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Jobs(Requester):
-
     """
     The jobs endpoint is used to query the status of existing
     jobs in Nomad and to register new jobs.
     By default, the agent's local region is used.
 
     https://www.nomadproject.io/docs/http/jobs.html
     """
+
     ENDPOINT = "jobs"
 
     def __init__(self, **kwargs):
-        super(Jobs, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return "{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return "{self.__dict__}"
 
     def __getattr__(self, item):
-        msg = "{0} does not exist".format(item)
+        msg = f"{item} does not exist"
         raise AttributeError(msg)
 
     def __contains__(self, item):
         try:
             jobs = self.get_jobs()
 
             for j in jobs:
                 if j["ID"] == item:
                     return True
                 if j["Name"] == item:
                     return True
-            else:
-                return False
+            return False
         except nomad.api.exceptions.URLNotFoundNomadException:
             return False
 
     def __len__(self):
         jobs = self.get_jobs()
         return len(jobs)
 
@@ -50,60 +51,73 @@
             jobs = self.get_jobs()
 
             for j in jobs:
                 if j["ID"] == item:
                     return j
                 if j["Name"] == item:
                     return j
-            else:
-                raise KeyError
-        except nomad.api.exceptions.URLNotFoundNomadException:
             raise KeyError
+        except nomad.api.exceptions.URLNotFoundNomadException as exc:
+            raise KeyError from exc
 
     def __iter__(self):
         jobs = self.get_jobs()
         return iter(jobs)
 
-    def get_jobs(self, prefix=None, namespace=None):
-        """ Lists all the jobs registered with Nomad.
-
-           https://www.nomadproject.io/docs/http/jobs.html
-            arguments:
-              - prefix :(str) optional, specifies a string to filter jobs on based on an prefix.
-                        This is specified as a querystring parameter.
-              - namespace :(str) optional, specifies the target namespace. Specifying * would return all jobs.
-                        This is specified as a querystring parameter.
-            returns: list
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+    def get_jobs(
+        self,
+        prefix: Optional[str] = None,
+        namespace: Optional[str] = None,
+        filter_: Optional[str] = None,
+        meta: Optional[bool] = None,
+    ):
+        """Lists all the jobs registered with Nomad.
+
+        https://www.nomadproject.io/docs/http/jobs.html
+        arguments:
+          - prefix :(str) optional, specifies a string to filter jobs on based on an prefix.
+                    This is specified as a querystring parameter.
+          - namespace :(str) optional, specifies the target namespace. Specifying * would return all jobs.
+                    This is specified as a querystring parameter.
+          - filter_ :(str) optional, specifies the expression used to filter the result.
+                    Name has a trailing underscore not to conflict with builtin function.
+          - meta :(bool) optional, if set, jobs returned will include a meta field containing
+                    key-value pairs provided in the job specification's meta block.
+        returns: list
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        params = {"prefix": prefix}
-        if namespace:
-            params["namespace"] = namespace
-
+        params = {
+            "prefix": prefix,
+            "namespace": namespace,
+            "filter": filter_,
+            "meta": meta,
+        }
         return self.request(method="get", params=params).json()
 
     def register_job(self, job):
-        """ Register a job with Nomad.
+        """Register a job with Nomad.
 
-           https://www.nomadproject.io/docs/http/jobs.html
+        https://www.nomadproject.io/docs/http/jobs.html
 
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request(json=job, method="post").json()
 
     def parse(self, hcl, canonicalize=False):
-        """ Parse a HCL Job file. Returns a dict with the JSON formatted job.
-            This API endpoint is only supported from Nomad version 0.8.3.
+        """Parse a HCL Job file. Returns a dict with the JSON formatted job.
+        This API endpoint is only supported from Nomad version 0.8.3.
 
-            https://www.nomadproject.io/api/jobs.html#parse-job
+        https://www.nomadproject.io/api/jobs.html#parse-job
 
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request("parse", json={"JobHCL": hcl, "Canonicalize": canonicalize}, method="post", allow_redirects=True).json()
+        return self.request(
+            "parse", json={"JobHCL": hcl, "Canonicalize": canonicalize}, method="post", allow_redirects=True
+        ).json()
```

### Comparing `python-nomad-1.5.0/nomad/api/metrics.py` & `python-nomad-2.0.0/nomad/api/metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,41 @@
+"""Nomad Metrics: https://developer.hashicorp.com/nomad/api-docs/metrics"""
 from nomad.api.base import Requester
 
 
 class Metrics(Requester):
-
     """
     The /metrics endpoint returns metrics for the current Nomad process.
 
     https://www.nomadproject.io/api/metrics.html
 
     Key metrics delivered via the endpoint could be found in Telemetry section:
 
     https://www.nomadproject.io/docs/agent/telemetry.html
     """
+
     ENDPOINT = "metrics"
 
     def __init__(self, **kwargs):
-        super(Metrics, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        raise AttributeError
+        msg = f"{item} does not exist"
+        raise AttributeError(msg)
 
     def get_metrics(self):
-        """ Get the metrics
+        """Get the metrics
 
-           https://www.nomadproject.io/api/metrics.html
+        https://www.nomadproject.io/api/metrics.html
 
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request(method="get").json()
```

### Comparing `python-nomad-1.5.0/nomad/api/namespace.py` & `python-nomad-2.0.0/nomad/api/namespace.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,107 +1,106 @@
+"""Nomad namespace: https://developer.hashicorp.com/nomad/api-docs/namespaces"""
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Namespace(Requester):
-
     """
     The job endpoint is used for CRUD on a single namespace.
     By default, the agent's local region is used.
 
     https://www.nomadproject.io/api/namespaces.html
     """
+
     ENDPOINT = "namespace"
 
     def __init__(self, **kwargs):
-        super(Namespace, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        msg = "{0} does not exist".format(item)
+        msg = f"{item} does not exist"
         raise AttributeError(msg)
 
     def __contains__(self, item):
-
         try:
-            j = self.get_namespace(item)
+            self.get_namespace(item)
             return True
         except nomad.api.exceptions.URLNotFoundNomadException:
             return False
 
     def __getitem__(self, item):
-
         try:
-            j = self.get_namespace(item)
+            job = self.get_namespace(item)
+
+            if job["ID"] == item:
+                return job
+            if job["Name"] == item:
+                return job
 
-            if j["ID"] == item:
-                return j
-            if j["Name"] == item:
-                return j
-            else:
-                raise KeyError
-        except nomad.api.exceptions.URLNotFoundNomadException:
             raise KeyError
+        except nomad.api.exceptions.URLNotFoundNomadException as exc:
+            raise KeyError from exc
 
-    def get_namespace(self, id):
-        """ Query a single namespace.
+    def get_namespace(self, id_):
+        """Query a single namespace.
 
-           https://www.nomadproject.io/api/namespaces.html
+        https://www.nomadproject.io/api/namespaces.html
 
-            arguments:
-              - id
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id_
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, method="get").json()
+        return self.request(id_, method="get").json()
 
     def create_namespace(self, namespace):
-        """ create namespace
+        """create namespace
 
-           https://www.nomadproject.io/api/namespaces.html
+        https://www.nomadproject.io/api/namespaces.html
 
-            arguments:
-              - id
-              - namespace (dict)
-            returns: requests.Response
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id
+          - namespace (dict)
+        returns: requests.Response
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request(json=namespace, method="post")
 
-    def update_namespace(self, id, namespace):
-        """ Update namespace
+    def update_namespace(self, id_, namespace):
+        """Update namespace
 
-           https://www.nomadproject.io/api/namespaces.html
+        https://www.nomadproject.io/api/namespaces.html
 
-            arguments:
-              - id
-              - namespace (dict)
-            returns: requests.Response
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id_
+          - namespace (dict)
+        returns: requests.Response
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, json=namespace, method="post")
+        return self.request(id_, json=namespace, method="post")
 
-    def delete_namespace(self, id):
-        """ delete namespace.
+    def delete_namespace(self, id_):
+        """delete namespace.
 
-           https://www.nomadproject.io/api/namespaces.html
+        https://www.nomadproject.io/api/namespaces.html
 
-            arguments:
-              - id
-            returns: requests.Response
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id_
+        returns: requests.Response
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, method="delete")
+        return self.request(id_, method="delete")
```

### Comparing `python-nomad-1.5.0/nomad/api/namespaces.py` & `python-nomad-2.0.0/nomad/api/namespaces.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,74 @@
+"""Nomad namespace: https://developer.hashicorp.com/nomad/api-docs/namespaces"""
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Namespaces(Requester):
-
     """
     The namespaces from enterprise solution
 
     https://www.nomadproject.io/docs/enterprise/namespaces/index.html
     """
+
     ENDPOINT = "namespaces"
 
     def __init__(self, **kwargs):
-        super(Namespaces, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        msg = "{0} does not exist".format(item)
+        msg = f"{item} does not exist"
         raise AttributeError(msg)
 
     def __contains__(self, item):
         try:
             namespaces = self.get_namespaces()
 
-            for n in namespaces:
-                if n["Name"] == item:
+            for namespace in namespaces:
+                if namespace["Name"] == item:
                     return True
-            
+
             return False
         except nomad.api.exceptions.URLNotFoundNomadException:
             return False
 
     def __len__(self):
         namespaces = self.get_namespaces()
         return len(namespaces)
 
     def __getitem__(self, item):
         try:
             namespaces = self.get_namespaces()
 
-            for n in namespaces:
-                if n["Name"] == item:
-                    return n
-            
-            raise KeyError
-        except nomad.api.exceptions.URLNotFoundNomadException:
+            for namespace in namespaces:
+                if namespace["Name"] == item:
+                    return namespace
+
             raise KeyError
+        except nomad.api.exceptions.URLNotFoundNomadException as exc:
+            raise KeyError from exc
 
     def __iter__(self):
         namespaces = self.get_namespaces()
         return iter(namespaces)
 
     def get_namespaces(self, prefix=None):
-        """ Lists all the namespaces registered with Nomad.
+        """Lists all the namespaces registered with Nomad.
 
-           https://www.nomadproject.io/docs/enterprise/namespaces/index.html
-            arguments:
-              - prefix :(str) optional, specifies a string to filter namespaces on based on an prefix.
-                        This is specified as a querystring parameter.
-            returns: list
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        https://www.nomadproject.io/docs/enterprise/namespaces/index.html
+        arguments:
+          - prefix :(str) optional, specifies a string to filter namespaces on based on an prefix.
+                    This is specified as a querystring parameter.
+        returns: list
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         params = {"prefix": prefix}
         return self.request(method="get", params=params).json()
```

### Comparing `python-nomad-1.5.0/nomad/api/node.py` & `python-nomad-2.0.0/nomad/api/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,195 +1,183 @@
+"""Nomad Node: https://developer.hashicorp.com/nomad/api-docs/nodes"""
+from typing import Optional
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Node(Requester):
-
     """
     The node endpoint is used to query the a specific client node.
     By default, the agent's local region is used.
 
     https://www.nomadproject.io/docs/http/node.html
     """
+
     ENDPOINT = "node"
 
     def __init__(self, **kwargs):
-        super(Node, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        msg = "{0} does not exist".format(item)
+        msg = f"{item} does not exist"
         raise AttributeError(msg)
 
     def __contains__(self, item):
-
         try:
-            n = self.get_node(item)
+            self.get_node(item)
             return True
         except nomad.api.exceptions.URLNotFoundNomadException:
             return False
 
     def __getitem__(self, item):
-
         try:
-            n = self.get_node(item)
+            node = self.get_node(item)
+
+            if node["ID"] == item:
+                return node
+            if node["Name"] == item:
+                return node
 
-            if n["ID"] == item:
-                return n
-            if n["Name"] == item:
-                return n
-            else:
-                raise KeyError
-        except nomad.api.exceptions.URLNotFoundNomadException:
             raise KeyError
+        except nomad.api.exceptions.URLNotFoundNomadException as exc:
+            raise KeyError from exc
 
-    def get_node(self, id):
-        """ Query the status of a client node registered with Nomad.
+    def get_node(self, id_: str):
+        """Query the status of a client node registered with Nomad.
 
-           https://www.nomadproject.io/docs/http/node.html
+        https://www.nomadproject.io/docs/http/node.html
 
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, method="get").json()
+        return self.request(id_, method="get").json()
 
-    def get_allocations(self, id):
-        """ Query the allocations belonging to a single node.
+    def get_allocations(self, id_: str):
+        """Query the allocations belonging to a single node.
 
-           https://www.nomadproject.io/docs/http/node.html
+        https://www.nomadproject.io/docs/http/node.html
 
-            returns: list
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: list
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, "allocations", method="get").json()
+        return self.request(id_, "allocations", method="get").json()
 
-    def evaluate_node(self, id):
-        """ Creates a new evaluation for the given node.
-            This can be used to force run the 
-            scheduling logic if necessary.
+    def evaluate_node(self, id_: str):
+        """Creates a new evaluation for the given node.
+         This can be used to force run the
+         scheduling logic if necessary.
 
-           https://www.nomadproject.io/docs/http/node.html
+        https://www.nomadproject.io/docs/http/node.html
 
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id, "evaluate", method="post").json()
+        return self.request(id_, "evaluate", method="post").json()
 
-    def drain_node(self, id, enable=False):
-        """ Toggle the drain mode of the node.
-            When enabled, no further allocations will be
-            assigned and existing allocations will be migrated.
+    def drain_node(self, id_, enable: bool = False):
+        """Toggle the drain mode of the node.
+         When enabled, no further allocations will be
+         assigned and existing allocations will be migrated.
 
-           https://www.nomadproject.io/docs/http/node.html
+        https://www.nomadproject.io/docs/http/node.html
 
-            arguments:
-              - id (str uuid): node id
-              - enable (bool): enable node drain or not to enable node drain
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id_ (str uuid): node id
+          - enable (bool): enable node drain or not to enable node drain
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
 
-        return self.request(id, "drain", params={"enable": enable}, method="post").json()
+        return self.request(id_, "drain", params={"enable": enable}, method="post").json()
 
-    def drain_node_with_spec(self, id, drain_spec, mark_eligible=None):
-        """ This endpoint toggles the drain mode of the node. When draining is enabled,
-            no further allocations will be assigned to this node, and existing allocations
-            will be migrated to new nodes.
+    def drain_node_with_spec(self, id_, drain_spec: Optional[dict], mark_eligible: Optional[bool] = None):
+        """This endpoint toggles the drain mode of the node. When draining is enabled,
+        no further allocations will be assigned to this node, and existing allocations
+        will be migrated to new nodes.
 
-            If an empty dictionary is given as drain_spec this will disable/toggle the drain.
+        If an empty dictionary is given as drain_spec this will disable/toggle the drain.
 
-            https://www.nomadproject.io/docs/http/node.html
+        https://www.nomadproject.io/docs/http/node.html
 
-            arguments:
-              - id (str uuid): node id
-              - drain_spec (dict): https://www.nomadproject.io/api/nodes.html#drainspec
-              - mark_eligible (bool): https://www.nomadproject.io/api/nodes.html#markeligible
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id_ (str uuid): node id
+          - drain_spec (dict): https://www.nomadproject.io/api/nodes.html#drainspec
+          - mark_eligible (bool): https://www.nomadproject.io/api/nodes.html#markeligible
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         payload = {}
 
         if drain_spec and mark_eligible is not None:
-            payload = {
-                "NodeID": id,
-                "DrainSpec": drain_spec,
-                "MarkEligible": mark_eligible
-            }
+            payload = {"NodeID": id_, "DrainSpec": drain_spec, "MarkEligible": mark_eligible}
         elif drain_spec and mark_eligible is None:
-            payload = {
-                "NodeID": id,
-                "DrainSpec": drain_spec
-            }
+            payload = {"NodeID": id_, "DrainSpec": drain_spec}
         elif not drain_spec and mark_eligible is not None:
-            payload = {
-                "NodeID": id,
-                "DrainSpec": None,
-                "MarkEligible": mark_eligible
-            }
+            payload = {"NodeID": id_, "DrainSpec": None, "MarkEligible": mark_eligible}
         elif not drain_spec and mark_eligible is None:
             payload = {
-                "NodeID": id,
+                "NodeID": id_,
                 "DrainSpec": None,
             }
 
-        return self.request(id, "drain", json=payload, method="post").json()
+        return self.request(id_, "drain", json=payload, method="post").json()
 
-    def eligible_node(self, id, eligible=None, ineligible=None):
-        """ Toggle the eligibility of the node.
+    def eligible_node(self, id_: str, eligible: Optional[bool] = None, ineligible: Optional[bool] = None):
+        """Toggle the eligibility of the node.
 
-           https://www.nomadproject.io/docs/http/node.html
+        https://www.nomadproject.io/docs/http/node.html
 
-            arguments:
-              - id (str uuid): node id
-              - eligible (bool): Set to True to mark node eligible
-              - ineligible (bool): Set to True to mark node ineligible
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - id_ (str uuid): node id
+          - eligible (bool): Set to True to mark node eligible
+          - ineligible (bool): Set to True to mark node ineligible
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         payload = {}
 
         if eligible is not None and ineligible is not None:
             raise nomad.api.exceptions.InvalidParameters
         if eligible is None and ineligible is None:
             raise nomad.api.exceptions.InvalidParameters
 
         if eligible is not None and eligible:
-            payload = {"Eligibility": "eligible", "NodeID": id}
+            payload = {"Eligibility": "eligible", "NodeID": id_}
         elif eligible is not None and not eligible:
-            payload = {"Eligibility": "ineligible", "NodeID": id}
+            payload = {"Eligibility": "ineligible", "NodeID": id_}
         elif ineligible is not None:
-            payload = {"Eligibility": "ineligible", "NodeID": id}
+            payload = {"Eligibility": "ineligible", "NodeID": id_}
         elif ineligible is not None and not ineligible:
-            payload = {"Eligibility": "eligible", "NodeID": id}
+            payload = {"Eligibility": "eligible", "NodeID": id_}
 
-        return self.request(id, "eligibility", json=payload, method="post").json()
+        return self.request(id_, "eligibility", json=payload, method="post").json()
 
-    def purge_node(self, id):
-        """ This endpoint purges a node from the system. Nodes can still join the cluster if they are alive.
+    def purge_node(self, id_: str):
+        """This endpoint purges a node from the system. Nodes can still join the cluster if they are alive.
         arguments:
-          - id (str uuid): node id
+          - id_ (str uuid): node id
         returns: dict
         raises:
           - nomad.api.exceptions.BaseNomadException
           - nomad.api.exceptions.URLNotFoundNomadException
         """
 
-        return self.request(id, "purge", method="post").json()
-
+        return self.request(id_, "purge", method="post").json()
```

### Comparing `python-nomad-1.5.0/nomad/api/nodes.py` & `python-nomad-2.0.0/nomad/api/nodes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,94 @@
+"""Nomad Node: https://developer.hashicorp.com/nomad/api-docs/nodes"""
+from typing import Optional
+
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Nodes(Requester):
-
     """
     The nodes endpoint is used to query the status of client nodes.
     By default, the agent's local region is used
 
     https://www.nomadproject.io/docs/http/nodes.html
     """
+
     ENDPOINT = "nodes"
 
     def __init__(self, **kwargs):
-        super(Nodes, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        raise AttributeError
+        msg = f"{item} does not exist"
+        raise AttributeError(msg)
 
     def __contains__(self, item):
         try:
             nodes = self.get_nodes()
 
-            for n in nodes:
-                if n["ID"] == item:
+            for node in nodes:
+                if node["ID"] == item:
                     return True
-                if n["Name"] == item:
+                if node["Name"] == item:
                     return True
-            else:
-                return False
+            return False
         except nomad.api.exceptions.URLNotFoundNomadException:
             return False
 
     def __len__(self):
         nodes = self.get_nodes()
         return len(nodes)
 
     def __getitem__(self, item):
         try:
             nodes = self.get_nodes()
 
-            for n in nodes:
-                if n["ID"] == item:
-                    return n
-                if n["Name"] == item:
-                    return n
-            else:
-                raise KeyError
-        except nomad.api.exceptions.URLNotFoundNomadException:
+            for node in nodes:
+                if node["ID"] == item:
+                    return node
+                if node["Name"] == item:
+                    return node
             raise KeyError
+        except nomad.api.exceptions.URLNotFoundNomadException as exc:
+            raise KeyError from exc
 
     def __iter__(self):
         nodes = self.get_nodes()
         return iter(nodes)
 
-    def get_nodes(self, prefix=None):
-        """ Lists all the client nodes registered with Nomad.
-
-           https://www.nomadproject.io/docs/http/nodes.html
-            arguments:
-              - prefix :(str) optional, specifies a string to filter nodes on based on an prefix.
-                        This is specified as a querystring parameter.
-            returns: list
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+    def get_nodes(  # pylint: disable=too-many-arguments
+        self,
+        prefix: Optional[str] = None,
+        next_token: Optional[str] = None,
+        per_page: Optional[str] = None,
+        filter_: Optional[str] = None,
+        resources: Optional[bool] = None,
+        os: Optional[bool] = None,  # pylint: disable=invalid-name
+    ):
+        """Lists all the client nodes registered with Nomad.
+
+        https://www.nomadproject.io/docs/http/nodes.html
+        arguments:
+          - prefix :(str) optional, specifies a string to filter nodes on based on an prefix.
+                    This is specified as a querystring parameter.
+        returns: list
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        params = {"prefix": prefix}
+        params = {
+            "prefix": prefix,
+            "next_token": next_token,
+            "per_page": per_page,
+            "filter_": filter_,
+            "resources": resources,
+            "os": os,
+        }
         return self.request(method="get", params=params).json()
```

### Comparing `python-nomad-1.5.0/nomad/api/operator.py` & `python-nomad-2.0.0/nomad/api/operator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,63 @@
+"""Nomad Operator: https://developer.hashicorp.com/nomad/api-docs/operator"""
 from nomad.api.base import Requester
 
 
 class Operator(Requester):
-
     """
     The Operator endpoint provides cluster-level tools for
     Nomad operators, such as interacting with the Raft subsystem.
 
     https://www.nomadproject.io/docs/http/operator.html
     """
 
     ENDPOINT = "operator"
 
     def __init__(self, **kwargs):
-        super(Operator, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        raise AttributeError
+        msg = f"{item} does not exist"
+        raise AttributeError(msg)
 
     def get_configuration(self, stale=False):
-        """ Query the status of a client node registered with Nomad.
+        """Query the status of a client node registered with Nomad.
 
-            https://www.nomadproject.io/docs/http/operator.html
+        https://www.nomadproject.io/docs/http/operator.html
 
-            returns: dict
-            optional arguments:
-              - stale, (defaults to False), Specifies if the cluster should respond without an active leader.
-                                            This is specified as a querystring parameter.
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: dict
+        optional arguments:
+          - stale, (defaults to False), Specifies if the cluster should respond without an active leader.
+                                        This is specified as a querystring parameter.
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
 
         params = {"stale": stale}
         return self.request("raft", "configuration", params=params, method="get").json()
 
     def delete_peer(self, peer_address, stale=False):
-        """ Remove the Nomad server with given address from the Raft configuration.
-            The return code signifies success or failure.
+        """Remove the Nomad server with given address from the Raft configuration.
+        The return code signifies success or failure.
 
-            https://www.nomadproject.io/docs/http/operator.html
+        https://www.nomadproject.io/docs/http/operator.html
 
-            arguments:
-              - peer_address, The address specifies the server to remove and is given as an IP:port
-            optional arguments:
-              - stale, (defaults to False), Specifies if the cluster should respond without an active leader.
-                                            This is specified as a querystring parameter.
-            returns: Boolean
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - peer_address, The address specifies the server to remove and is given as an IP:port
+        optional arguments:
+          - stale, (defaults to False), Specifies if the cluster should respond without an active leader.
+                                        This is specified as a querystring parameter.
+        returns: Boolean
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
 
         params = {"address": peer_address, "stale": stale}
         return self.request("raft", "peer", params=params, method="delete").ok
```

### Comparing `python-nomad-1.5.0/nomad/api/regions.py` & `python-nomad-2.0.0/nomad/api/regions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,67 +1,67 @@
+"""Nomad region: https://developer.hashicorp.com/nomad/api-docs/regions"""
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Regions(Requester):
-
     """
     https://www.nomadproject.io/docs/http/regions.html
     """
+
     ENDPOINT = "regions"
 
     def __init__(self, **kwargs):
-        super(Regions, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        raise AttributeError
+        msg = f"{item} does not exist"
+        raise AttributeError(msg)
 
     def __contains__(self, item):
         try:
             regions = self.get_regions()
 
-            for r in regions:
-                if r == item:
+            for region in regions:
+                if region == item:
                     return True
-            else:
-                return False
+            return False
         except nomad.api.exceptions.URLNotFoundNomadException:
             return False
 
     def __len__(self):
         regions = self.get_regions()
         return len(regions)
 
     def __getitem__(self, item):
         try:
             regions = self.get_regions()
 
-            for r in regions:
-                if r == item:
-                    return r
-            else:
-                raise KeyError
-        except nomad.api.exceptions.URLNotFoundNomadException:
+            for region in regions:
+                if region == item:
+                    return region
             raise KeyError
+        except nomad.api.exceptions.URLNotFoundNomadException as exc:
+            raise KeyError from exc
 
     def __iter__(self):
         regions = self.get_regions()
         return iter(regions)
 
     def get_regions(self):
-        """ Returns the known region names.
+        """Returns the known region names.
 
-            https://www.nomadproject.io/docs/http/regions.html
+        https://www.nomadproject.io/docs/http/regions.html
 
-            returns: list
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: list
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request(method="get").json()
```

### Comparing `python-nomad-1.5.0/nomad/api/search.py` & `python-nomad-2.0.0/nomad/api/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,83 +1,88 @@
+"""Nomad Search API: https://developer.hashicorp.com/nomad/api-docs/search"""
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Search(Requester):
     """
     The endpoint returns matches for a given prefix and context, where a context can be jobs, allocations, evaluations,
     nodes, deployments, plugins, namespaces, or volumes.
     When using Nomad Enterprise, the allowed contexts include quotas.
     Additionally, a prefix can be searched for within every context.
 
     https://developer.hashicorp.com/nomad/api-docs/search
     """
+
     ENDPOINT = "search"
 
     def __init__(self, **kwargs):
-        super(Search, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        raise AttributeError
+        msg = f"{item} does not exist"
+        raise AttributeError(msg)
 
     def search(self, prefix, context):
-        """ The endpoint returns matches for a given prefix and context, where a context can be jobs,
-            allocations, evaluations, nodes, deployments, plugins, namespaces, or volumes.
+        """The endpoint returns matches for a given prefix and context, where a context can be jobs,
+        allocations, evaluations, nodes, deployments, plugins, namespaces, or volumes.
 
-            https://developer.hashicorp.com/nomad/api-docs/search
-            arguments:
-              - prefix:(str) required, specifies the identifier against which matches will be found.
-                For example, if the given prefix were "a", potential matches might be "abcd", or "aabb".
-              - context:(str) defines the scope in which a search for a prefix operates.
-                Contexts can be: "jobs", "evals", "allocs", "nodes", "deployment", "plugins",
-                "volumes" or "all", where "all" means every context will be searched.
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
-              - nomad.api.exceptions.InvalidParameters
+        https://developer.hashicorp.com/nomad/api-docs/search
+        arguments:
+          - prefix:(str) required, specifies the identifier against which matches will be found.
+            For example, if the given prefix were "a", potential matches might be "abcd", or "aabb".
+          - context:(str) defines the scope in which a search for a prefix operates.
+            Contexts can be: "jobs", "evals", "allocs", "nodes", "deployment", "plugins",
+            "volumes" or "all", where "all" means every context will be searched.
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
+          - nomad.api.exceptions.InvalidParameters
         """
         accetaple_contexts = ("jobs", "evals", "allocs", "nodes", "deployment", "plugins", "volumes", "all")
         if context not in accetaple_contexts:
-            raise nomad.api.exceptions.InvalidParameters("context is invalid "
-                "(expected values are {} but got {})".format(accetaple_contexts, context))
+            raise nomad.api.exceptions.InvalidParameters(
+                "context is invalid " f"(expected values are {accetaple_contexts} but got {context})"
+            )
         params = {"Prefix": prefix, "Context": context}
 
         return self.request(json=params, method="post").json()
 
     def fuzzy_search(self, text, context):
-        """ The /search/fuzzy endpoint returns partial substring matches for a given search term and context,
-            where a context can be jobs, allocations, nodes, plugins, or namespaces. Additionally, 
-            fuzzy searching can be done across all contexts.
-
-            https://developer.hashicorp.com/nomad/api-docs/search#fuzzy-searching
-            arguments:
-              - text:(str) required, specifies the identifier against which matches will be found.
-                For example, if the given text were "py", potential fuzzy matches might be "python", "spying",
-                or "happy".
-              - context:(str) defines the scope in which a search for a prefix operates. Contexts can be:
-                "jobs", "allocs", "nodes", "plugins", or "all", where "all" means every context will
-                be searched.
-                When "all" is selected, additional prefix matches will be included for the "deployments",
-                "evals", and "volumes" types. When searching in the "jobs" context, results that fuzzy match
-                "groups", "services", "tasks", "images", "commands", and "classes" are also included in the results.
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        """The /search/fuzzy endpoint returns partial substring matches for a given search term and context,
+        where a context can be jobs, allocations, nodes, plugins, or namespaces. Additionally,
+        fuzzy searching can be done across all contexts.
+
+        https://developer.hashicorp.com/nomad/api-docs/search#fuzzy-searching
+        arguments:
+          - text:(str) required, specifies the identifier against which matches will be found.
+            For example, if the given text were "py", potential fuzzy matches might be "python", "spying",
+            or "happy".
+          - context:(str) defines the scope in which a search for a prefix operates. Contexts can be:
+            "jobs", "allocs", "nodes", "plugins", or "all", where "all" means every context will
+            be searched.
+            When "all" is selected, additional prefix matches will be included for the "deployments",
+            "evals", and "volumes" types. When searching in the "jobs" context, results that fuzzy match
+            "groups", "services", "tasks", "images", "commands", and "classes" are also included in the results.
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
 
         params = {"Text": text, "Context": context}
 
         accetaple_contexts = ("jobs", "allocs", "nodes", "plugins", "all")
         if context not in accetaple_contexts:
-            raise nomad.api.exceptions.InvalidParameters("context is invalid "
-                "(expected values are {} but got {})".format(accetaple_contexts,context))
+            raise nomad.api.exceptions.InvalidParameters(
+                "context is invalid " f"(expected values are {accetaple_contexts} but got {context})"
+            )
 
         return self.request("fuzzy", json=params, method="post").json()
```

### Comparing `python-nomad-1.5.0/nomad/api/sentinel.py` & `python-nomad-2.0.0/nomad/api/sentinel.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,96 +1,97 @@
+"""Nomad Sentinel API: https://developer.hashicorp.com/nomad/api-docs/sentinel-policies"""
 from nomad.api.base import Requester
 
 
 class Sentinel(Requester):
-
     """
     The endpoint manage sentinel policies (Enterprise Only)
 
     https://www.nomadproject.io/api/sentinel-policies.html
     """
 
     ENDPOINT = "sentinel"
 
     def __init__(self, **kwargs):
-        super(Sentinel, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        raise AttributeError
+        msg = f"{item} does not exist"
+        raise AttributeError(msg)
 
     def get_policies(self):
-        """ Get a list of policies.
+        """Get a list of policies.
 
-            https://www.nomadproject.io/api/sentinel-policies.html
+        https://www.nomadproject.io/api/sentinel-policies.html
 
-            returns: list
+        returns: list
 
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request("policies", method="get").json()
 
-    def create_policy(self, id, policy):
-        """ Create policy.
+    def create_policy(self, id_, policy):
+        """Create policy.
 
-            https://www.nomadproject.io/api/sentinel-policies.html
+        https://www.nomadproject.io/api/sentinel-policies.html
 
-            arguments:
-                - policy
-            returns: requests.Response
-
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+            - policy
+        returns: requests.Response
+
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request("policy", id, json=policy, method="post")
+        return self.request("policy", id_, json=policy, method="post")
 
-    def get_policy(self, id):
-        """ Get a spacific policy.
+    def get_policy(self, id_):
+        """Get a spacific policy.
 
-            https://www.nomadproject.io/api/sentinel-policies.html
+        https://www.nomadproject.io/api/sentinel-policies.html
 
-            returns: dict
+        returns: dict
 
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request("policy", id, method="get").json()
+        return self.request("policy", id_, method="get").json()
 
-    def update_policy(self, id, policy):
-        """ Create policy.
+    def update_policy(self, id_, policy):
+        """Create policy.
 
-            https://www.nomadproject.io/api/sentinel-policies.html
+        https://www.nomadproject.io/api/sentinel-policies.html
 
-            arguments:
-                - name
-                - policy
-            returns: requests.Response
+        arguments:
+            - name
+            - policy
+        returns: requests.Response
 
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request("policy", id, json=policy, method="post")
+        return self.request("policy", id_, json=policy, method="post")
 
-    def delete_policy(self, id):
-        """ Delete specific policy.
+    def delete_policy(self, id_):
+        """Delete specific policy.
 
-            https://www.nomadproject.io/api/sentinel-policies.html
+        https://www.nomadproject.io/api/sentinel-policies.html
 
-            arguments:
-                - id
-            returns: Boolean
+        arguments:
+            - id_
+        returns: Boolean
 
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request("policy", id, method="delete").ok
+        return self.request("policy", id_, method="delete").ok
```

### Comparing `python-nomad-1.5.0/nomad/api/status.py` & `python-nomad-2.0.0/nomad/api/status.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,106 +1,107 @@
+"""Nomad Status API: https://developer.hashicorp.com/nomad/api-docs/status"""
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
-class Status(object):
-
+class Status:
     """
     By default, the agent's local region is used
 
     https://www.nomadproject.io/docs/http/status.html
     """
 
     def __init__(self, **kwargs):
         self.leader = Leader(**kwargs)
         self.peers = Peers(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        raise AttributeError
+        msg = f"{item} does not exist"
+        raise AttributeError(msg)
 
 
 class Leader(Requester):
+    """This endpoint returns the address of the current leader in the region."""
 
     ENDPOINT = "status/leader"
 
     def __contains__(self, item):
         try:
             leader = self.get_leader()
 
             if leader == item:
                 return True
-            else:
-                return False
+
+            return False
         except nomad.api.exceptions.URLNotFoundNomadException:
             return False
 
     def __len__(self):
         leader = self.get_leader()
         return len(leader)
 
     def get_leader(self):
-        """ Returns the address of the current leader in the region.
+        """Returns the address of the current leader in the region.
 
-            https://www.nomadproject.io/docs/http/status.html
+        https://www.nomadproject.io/docs/http/status.html
 
-            returns: string
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: string
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request(method="get").json()
 
 
 class Peers(Requester):
+    """This endpoint returns the set of raft peers in the region."""
 
     ENDPOINT = "status/peers"
 
     def __contains__(self, item):
         try:
             peers = self.get_peers()
 
-            for p in peers:
-                if p == item:
+            for peer in peers:
+                if peer == item:
                     return True
-            else:
-                return False
+            return False
         except nomad.api.exceptions.URLNotFoundNomadException:
             return False
 
     def __len__(self):
         peers = self.get_peers()
         return len(peers)
 
     def __getitem__(self, item):
         try:
             peers = self.get_peers()
 
-            for p in peers:
-                if p == item:
-                    return p
-            else:
-                raise KeyError
-        except nomad.api.exceptions.URLNotFoundNomadException:
+            for peer in peers:
+                if peer == item:
+                    return peer
             raise KeyError
+        except nomad.api.exceptions.URLNotFoundNomadException as exc:
+            raise KeyError from exc
 
     def __iter__(self):
         peers = self.get_peers()
         return iter(peers)
 
     def get_peers(self):
-        """ Returns the set of raft peers in the region.
+        """Returns the set of raft peers in the region.
 
-            https://www.nomadproject.io/docs/http/status.html
+        https://www.nomadproject.io/docs/http/status.html
 
-            returns: list
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        returns: list
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request(method="get").json()
```

### Comparing `python-nomad-1.5.0/nomad/api/validate.py` & `python-nomad-2.0.0/nomad/api/validate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Nomad Validate API: https://developer.hashicorp.com/nomad/api-docs/validate"""
 from nomad.api.base import Requester
 
 
 class Validate(Requester):
 
     """
     The system endpoint is used to for system maintenance
@@ -10,33 +11,34 @@
 
     https://www.nomadproject.io/docs/http/system.html
     """
 
     ENDPOINT = "validate"
 
     def __init__(self, **kwargs):
-        super(Validate, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        raise AttributeError
+        msg = f"{item} does not exist"
+        raise AttributeError(msg)
 
     def validate_job(self, nomad_job_dict):
-        """ This endpoint validates a Nomad job file. The local Nomad agent forwards the request to a server.
+        """This endpoint validates a Nomad job file. The local Nomad agent forwards the request to a server.
         In the event a server can't be reached the agent verifies the job file locally but skips validating driver
         configurations.
 
-            https://www.nomadproject.io/api/validate.html
+        https://www.nomadproject.io/api/validate.html
 
-            arguments:
-              - nomad_job_json, any valid nomad job IN dict FORMAT
-            returns: dict
-            raises:
-              - nomad.api.exceptions.BaseNomadException
-              - nomad.api.exceptions.URLNotFoundNomadException
+        arguments:
+          - nomad_job_json, any valid nomad job IN dict FORMAT
+        returns: dict
+        raises:
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request("job", json=nomad_job_dict, method="post")
```

### Comparing `python-nomad-1.5.0/nomad/api/variable.py` & `python-nomad-2.0.0/nomad/api/variable.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,108 +1,108 @@
+"""Nomad Valiables API: https://developer.hashicorp.com/nomad/api-docs/variables"""
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Variable(Requester):
-
     """
     The /var endpoints are used to read or create variables.
     https://developer.hashicorp.com/nomad/api-docs/variables
     """
 
     ENDPOINT = "var"
 
     def __init__(self, **kwargs):
-        super(Variable, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        raise AttributeError
+        msg = f"{item} does not exist"
+        raise AttributeError(msg)
 
     def __contains__(self, item):
         try:
             self.get_variable(item)
             return True
         except nomad.api.exceptions.URLNotFoundNomadException:
             return False
 
     def __getitem__(self, item):
         try:
             return self.get_variable(item)
-        except nomad.api.exceptions.URLNotFoundNomadException:
-            raise KeyError
+        except nomad.api.exceptions.URLNotFoundNomadException as exc:
+            raise KeyError from exc
 
     def get_variable(self, var_path, namespace=None):
         """
         This endpoint reads a specific variable by path. This API returns the decrypted variable body.
         https://developer.hashicorp.com/nomad/api-docs/variables#read-variable
 
         arguments:
-            - var_path :(str), path to variable
+          - var_path :(str), path to variable
         returns: dict
         raises:
-            - nomad.api.exceptions.BaseNomadException
-            - nomad.api.exceptions.URLNotFoundNomadException
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         params = {}
         if namespace:
             params["namespace"] = namespace
 
         return self.request(var_path, params=params, method="get").json()
 
     def create_variable(self, var_path, payload, namespace=None, cas=None):
         """
         This endpoint creates or updates a variable.
         https://developer.hashicorp.com/nomad/api-docs/variables#create-variable
 
         arguments:
-            - var_path :(str), path to variable
-            - payload :(dict), variable object. Example:
+          - var_path :(str), path to variable
+          - payload :(dict), variable object. Example:
             https://developer.hashicorp.com/nomad/api-docs/variables#sample-payload
-            - namespace :(str) optional, specifies the target namespace. Specifying * would return all jobs.
-                    This is specified as a querystring parameter.
-            - cas :(int) optional, If set, the variable will only be deleted if the cas value matches the
-                    current variables ModifyIndex.
+          - namespace :(str) optional, specifies the target namespace. Specifying * would return all jobs.
+                This is specified as a querystring parameter.
+          - cas :(int) optional, If set, the variable will only be deleted if the cas value matches the
+            current variables ModifyIndex.
         returns: dict
         raises:
-            - nomad.api.exceptions.BaseNomadException
-            - nomad.api.exceptions.URLNotFoundNomadException
-            - nomad.api.exceptions.VariableConflict
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
+          - nomad.api.exceptions.VariableConflict
         """
         params = {}
         if cas is not None:
             params["cas"] = cas
         if namespace:
             params["namespace"] = namespace
 
         return self.request(var_path, params=params, json=payload, method="put").json()
 
-
     def delete_variable(self, var_path, namespace=None, cas=None):
         """
         This endpoint reads a specific variable by path. This API returns the decrypted variable body.
         https://developer.hashicorp.com/nomad/api-docs/variables#delete-variable
 
         arguments:
-            - var_path :(str), path to variable
-            - namespace :(str) optional, specifies the target namespace. Specifying * would return all jobs.
-                    This is specified as a querystring parameter.
-            - cas :(int) optional, If set, the variable will only be deleted if the cas value matches the 
-                    current variables ModifyIndex.
+          - var_path :(str), path to variable
+          - namespace :(str) optional, specifies the target namespace. Specifying * would return all jobs.
+                This is specified as a querystring parameter.
+          - cas :(int) optional, If set, the variable will only be deleted if the cas value matches the
+                current variables ModifyIndex.
         returns: dict
         raises:
-            - nomad.api.exceptions.BaseNomadException
-            - nomad.api.exceptions.URLNotFoundNomadException
-            - nomad.api.exceptions.VariableConflict
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
+          - nomad.api.exceptions.VariableConflict
         """
         params = {}
         if cas is not None:
             params["cas"] = cas
         if namespace:
             params["namespace"] = namespace
```

### Comparing `python-nomad-1.5.0/nomad/api/variables.py` & `python-nomad-2.0.0/nomad/api/variables.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,65 @@
-import nomad.api.exceptions
-
+"""Nomad Valiables API: https://developer.hashicorp.com/nomad/api-docs/variables"""
 from nomad.api.base import Requester
 
 
 class Variables(Requester):
-
     """
     The /vars endpoints are used to query for and interact with variables.
     https://developer.hashicorp.com/nomad/api-docs/variables
     """
 
     ENDPOINT = "vars"
 
     def __init__(self, **kwargs):
-        super(Variables, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __repr__(self):
-        return "{0}".format(self.__dict__)
+        return f"{self.__dict__}"
 
     def __getattr__(self, item):
-        raise AttributeError
+        msg = f"{item} does not exist"
+        raise AttributeError(msg)
 
     def __contains__(self, item):
         variables = self.get_variables()
 
         for var in variables:
             if var["Path"] == item:
                 return True
-        else:
-            return False
+        return False
 
     def __getitem__(self, item):
         variables = self.get_variables()
 
         for var in variables:
             if var["Path"] == item:
                 return var
-        else:
-            raise KeyError
+        raise KeyError
 
     def __iter__(self):
         variables = self.get_variables()
         return iter(variables)
 
     def get_variables(self, prefix="", namespace=None):
-        """ 
+        """
         This endpoint lists variables.
         https://developer.hashicorp.com/nomad/api-docs/variables
 
         optional_arguments:
-            - prefix, (default "") Specifies a string to filter variables on based on an index prefix.
-                This is specified as a query string parameter.
-            - namespace :(str) optional, Specifies the target namespace.
-                Specifying * will return all variables across all the authorized namespaces.
+          - prefix, (default "") Specifies a string to filter variables on based on an index prefix.
+            This is specified as a query string parameter.
+          - namespace :(str) optional, Specifies the target namespace.
+            Specifying * will return all variables across all the authorized namespaces.
         returns: list of dicts
         raises:
-            - nomad.api.exceptions.BaseNomadException
-            - nomad.api.exceptions.URLNotFoundNomadException
+          - nomad.api.exceptions.BaseNomadException
+          - nomad.api.exceptions.URLNotFoundNomadException
         """
         params = {"prefix": prefix}
         if namespace:
             params["namespace"] = namespace
 
         return self.request(params=params, method="get").json()
-
-
```

### Comparing `python-nomad-1.5.0/python_nomad.egg-info/PKG-INFO` & `python-nomad-2.0.0/python_nomad.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: python-nomad
-Version: 1.5.0
+Version: 2.0.0
 Summary: Client library for Hashicorp Nomad
 Home-page: http://github.com/jrxfive/python-nomad
 Author: jrxfive
 Author-email: jrxfive@gmail.com
 License: MIT
 Keywords: nomad hashicorp client
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-nomad-1.5.0/setup.py` & `python-nomad-2.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,29 @@
+"""Nomad Python Library"""
 import setuptools
 
-with open("README.md", "r") as fh:
+with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='python-nomad',
-    version='1.5.0',
+    version='2.0.0',
     install_requires=['requests'],
     packages=['nomad', 'nomad.api'],
     url='http://github.com/jrxfive/python-nomad',
     license='MIT',
     author='jrxfive',
     author_email='jrxfive@gmail.com',
     description='Client library for Hashicorp Nomad',
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     keywords='nomad hashicorp client',
```

