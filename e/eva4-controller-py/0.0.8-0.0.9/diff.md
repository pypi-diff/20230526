# Comparing `tmp/eva4-controller-py-0.0.8.tar.gz` & `tmp/eva4-controller-py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eva4-controller-py-0.0.8.tar", last modified: Mon Apr 25 14:14:33 2022, max compression
+gzip compressed data, was "eva4-controller-py-0.0.9.tar", last modified: Wed Apr 27 02:37:48 2022, max compression
```

## Comparing `eva4-controller-py-0.0.8.tar` & `eva4-controller-py-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-25 14:14:33.855457 eva4-controller-py-0.0.8/
--rw-r--r--   0 divisor   (1000) root         (0)    10639 2022-03-19 18:20:58.000000 eva4-controller-py-0.0.8/LICENSE
--rw-r--r--   0 divisor   (1000) root         (0)      520 2022-04-25 14:14:33.855457 eva4-controller-py-0.0.8/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)       46 2022-04-01 21:38:20.000000 eva4-controller-py-0.0.8/README.md
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-25 14:14:33.851457 eva4-controller-py-0.0.8/bin/
--rwxr-xr-x   0 divisor   (1000) root         (0)       75 2022-04-01 21:42:50.000000 eva4-controller-py-0.0.8/bin/eva4-svc-controller-py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-25 14:14:33.851457 eva4-controller-py-0.0.8/eva4_controller_py/
--rw-r--r--   0 divisor   (1000) root         (0)     5501 2022-04-25 14:14:32.000000 eva4-controller-py-0.0.8/eva4_controller_py/__init__.py
--rw-r--r--   0 divisor   (1000) root         (0)    18005 2022-04-25 14:14:32.000000 eva4-controller-py-0.0.8/eva4_controller_py/macro_api.py
--rw-r--r--   0 divisor   (1000) root         (0)     1049 2022-04-25 14:14:32.000000 eva4-controller-py-0.0.8/eva4_controller_py/macro_builtins.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-25 14:14:33.855457 eva4-controller-py-0.0.8/eva4_controller_py.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)      520 2022-04-25 14:14:33.000000 eva4-controller-py-0.0.8/eva4_controller_py.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      362 2022-04-25 14:14:33.000000 eva4-controller-py-0.0.8/eva4_controller_py.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2022-04-25 14:14:33.000000 eva4-controller-py-0.0.8/eva4_controller_py.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)       62 2022-04-25 14:14:33.000000 eva4-controller-py-0.0.8/eva4_controller_py.egg-info/requires.txt
--rw-r--r--   0 divisor   (1000) root         (0)       19 2022-04-25 14:14:33.000000 eva4-controller-py-0.0.8/eva4_controller_py.egg-info/top_level.txt
--rw-r--r--   0 divisor   (1000) root         (0)       38 2022-04-25 14:14:33.855457 eva4-controller-py-0.0.8/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)     1077 2022-04-25 14:14:32.000000 eva4-controller-py-0.0.8/setup.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-27 02:37:48.204387 eva4-controller-py-0.0.9/
+-rw-r--r--   0 divisor   (1000) root         (0)    10639 2022-03-19 18:20:58.000000 eva4-controller-py-0.0.9/LICENSE
+-rw-r--r--   0 divisor   (1000) root         (0)      520 2022-04-27 02:37:48.204387 eva4-controller-py-0.0.9/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)       46 2022-04-01 21:38:20.000000 eva4-controller-py-0.0.9/README.md
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-27 02:37:48.204387 eva4-controller-py-0.0.9/bin/
+-rwxr-xr-x   0 divisor   (1000) root         (0)       75 2022-04-01 21:42:50.000000 eva4-controller-py-0.0.9/bin/eva4-svc-controller-py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-27 02:37:48.204387 eva4-controller-py-0.0.9/eva4_controller_py/
+-rw-r--r--   0 divisor   (1000) root         (0)     5544 2022-04-27 02:18:07.000000 eva4-controller-py-0.0.9/eva4_controller_py/__init__.py
+-rw-r--r--   0 divisor   (1000) root         (0)    18005 2022-04-27 02:18:07.000000 eva4-controller-py-0.0.9/eva4_controller_py/macro_api.py
+-rw-r--r--   0 divisor   (1000) root         (0)     1049 2022-04-27 02:18:07.000000 eva4-controller-py-0.0.9/eva4_controller_py/macro_builtins.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-27 02:37:48.204387 eva4-controller-py-0.0.9/eva4_controller_py.egg-info/
+-rw-r--r--   0 divisor   (1000) root         (0)      520 2022-04-27 02:37:48.000000 eva4-controller-py-0.0.9/eva4_controller_py.egg-info/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      362 2022-04-27 02:37:48.000000 eva4-controller-py-0.0.9/eva4_controller_py.egg-info/SOURCES.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        1 2022-04-27 02:37:48.000000 eva4-controller-py-0.0.9/eva4_controller_py.egg-info/dependency_links.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       62 2022-04-27 02:37:48.000000 eva4-controller-py-0.0.9/eva4_controller_py.egg-info/requires.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       19 2022-04-27 02:37:48.000000 eva4-controller-py-0.0.9/eva4_controller_py.egg-info/top_level.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       38 2022-04-27 02:37:48.204387 eva4-controller-py-0.0.9/setup.cfg
+-rw-r--r--   0 divisor   (1000) root         (0)     1077 2022-04-27 02:18:07.000000 eva4-controller-py-0.0.9/setup.py
```

### Comparing `eva4-controller-py-0.0.8/LICENSE` & `eva4-controller-py-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eva4-controller-py-0.0.8/PKG-INFO` & `eva4-controller-py-0.0.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eva4-controller-py
-Version: 0.0.8
+Version: 0.0.9
 Summary: EVA ICS v4 Python macros controller service
 Home-page: https://github.com/alttch/eva4
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eva4-controller-py-0.0.8/eva4_controller_py/__init__.py` & `eva4-controller-py-0.0.9/eva4_controller_py/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 from evaics.sdk import Service, Controller, Action, no_rpc_method, ServiceInfo
 from evaics.sdk import OID
 
 from timeouter import Timer
 
 import msgpack
@@ -169,14 +169,15 @@
     _d.service = service
     _d.controller = Controller(service.bus)
     _d.logger = service.init_logs()
     _d.env = {
         '_polldelay': poll_delay,
         'is_shutdown': service.is_shutdown_requested
     }
+    _d.env.update(config.get('cvars', {}))
     _d.env.update(macro_api.api_globals)
     macro_api.service = service
     macro_api.locker_svc = config.get('locker_svc')
     macro_api.mailer_svc = config.get('mailer_svc')
     service.on_rpc_call = handle_rpc
     service.init_rpc(info)
     _d.logger.info(f'Python macros controller started ({service.id}), '
```

### Comparing `eva4-controller-py-0.0.8/eva4_controller_py/macro_api.py` & `eva4-controller-py-0.0.9/eva4_controller_py/macro_api.py`

 * *Files identical despite different names*

### Comparing `eva4-controller-py-0.0.8/eva4_controller_py/macro_builtins.py` & `eva4-controller-py-0.0.9/eva4_controller_py/macro_builtins.py`

 * *Files identical despite different names*

### Comparing `eva4-controller-py-0.0.8/eva4_controller_py.egg-info/PKG-INFO` & `eva4-controller-py-0.0.9/eva4_controller_py.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eva4-controller-py
-Version: 0.0.8
+Version: 0.0.9
 Summary: EVA ICS v4 Python macros controller service
 Home-page: https://github.com/alttch/eva4
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eva4-controller-py-0.0.8/setup.py` & `eva4-controller-py-0.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='eva4-controller-py',
```

