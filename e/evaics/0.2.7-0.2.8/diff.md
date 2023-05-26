# Comparing `tmp/evaics-0.2.7.tar.gz` & `tmp/evaics-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evaics-0.2.7.tar", last modified: Thu May 25 23:39:47 2023, max compression
+gzip compressed data, was "evaics-0.2.8.tar", last modified: Fri May 26 14:58:11 2023, max compression
```

## Comparing `evaics-0.2.7.tar` & `evaics-0.2.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-25 23:39:47.288528 evaics-0.2.7/
--rw-r--r--   0 divisor   (1000) root         (0)    10639 2022-06-30 23:31:52.000000 evaics-0.2.7/LICENSE
--rw-r--r--   0 divisor   (1000) root         (0)      637 2023-05-25 23:39:47.288528 evaics-0.2.7/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      141 2022-10-03 20:48:30.000000 evaics-0.2.7/README.md
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-25 23:39:47.288528 evaics-0.2.7/evaics/
--rw-r--r--   0 divisor   (1000) root         (0)        0 2023-05-25 22:53:36.000000 evaics-0.2.7/evaics/__init__.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-25 23:39:47.288528 evaics-0.2.7/evaics/client/
--rw-r--r--   0 divisor   (1000) root         (0)      131 2023-05-25 22:53:36.000000 evaics-0.2.7/evaics/client/__init__.py
--rw-r--r--   0 divisor   (1000) root         (0)     4559 2023-05-25 22:53:36.000000 evaics-0.2.7/evaics/client/http.py
--rw-r--r--   0 divisor   (1000) root         (0)     1821 2023-05-25 22:53:36.000000 evaics-0.2.7/evaics/exceptions.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-25 23:39:47.288528 evaics-0.2.7/evaics/sdk/
--rw-r--r--   0 divisor   (1000) root         (0)    25786 2023-05-25 22:53:36.000000 evaics-0.2.7/evaics/sdk/__init__.py
--rw-r--r--   0 divisor   (1000) root         (0)     1116 2023-05-25 22:53:36.000000 evaics-0.2.7/evaics/tools.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-25 23:39:47.288528 evaics-0.2.7/evaics.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)      637 2023-05-25 23:39:47.000000 evaics-0.2.7/evaics.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      302 2023-05-25 23:39:47.000000 evaics-0.2.7/evaics.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2023-05-25 23:39:47.000000 evaics-0.2.7/evaics.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)       28 2023-05-25 23:39:47.000000 evaics-0.2.7/evaics.egg-info/requires.txt
--rw-r--r--   0 divisor   (1000) root         (0)        7 2023-05-25 23:39:47.000000 evaics-0.2.7/evaics.egg-info/top_level.txt
--rw-r--r--   0 divisor   (1000) root         (0)       38 2023-05-25 23:39:47.288528 evaics-0.2.7/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)      787 2023-05-25 22:53:36.000000 evaics-0.2.7/setup.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-26 14:58:11.378689 evaics-0.2.8/
+-rw-r--r--   0 divisor   (1000) root         (0)    10639 2022-06-30 23:31:52.000000 evaics-0.2.8/LICENSE
+-rw-r--r--   0 divisor   (1000) root         (0)      637 2023-05-26 14:58:11.378689 evaics-0.2.8/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      141 2022-10-03 20:48:30.000000 evaics-0.2.8/README.md
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-26 14:58:11.378689 evaics-0.2.8/evaics/
+-rw-r--r--   0 divisor   (1000) root         (0)        0 2023-05-26 14:57:27.000000 evaics-0.2.8/evaics/__init__.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-26 14:58:11.378689 evaics-0.2.8/evaics/client/
+-rw-r--r--   0 divisor   (1000) root         (0)      131 2023-05-26 14:57:27.000000 evaics-0.2.8/evaics/client/__init__.py
+-rw-r--r--   0 divisor   (1000) root         (0)     4559 2023-05-26 14:57:27.000000 evaics-0.2.8/evaics/client/http.py
+-rw-r--r--   0 divisor   (1000) root         (0)     1821 2023-05-26 14:57:27.000000 evaics-0.2.8/evaics/exceptions.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-26 14:58:11.378689 evaics-0.2.8/evaics/sdk/
+-rw-r--r--   0 divisor   (1000) root         (0)    27404 2023-05-26 14:57:27.000000 evaics-0.2.8/evaics/sdk/__init__.py
+-rw-r--r--   0 divisor   (1000) root         (0)     1116 2023-05-26 14:57:27.000000 evaics-0.2.8/evaics/tools.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-26 14:58:11.378689 evaics-0.2.8/evaics.egg-info/
+-rw-r--r--   0 divisor   (1000) root         (0)      637 2023-05-26 14:58:11.000000 evaics-0.2.8/evaics.egg-info/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      302 2023-05-26 14:58:11.000000 evaics-0.2.8/evaics.egg-info/SOURCES.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        1 2023-05-26 14:58:11.000000 evaics-0.2.8/evaics.egg-info/dependency_links.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       28 2023-05-26 14:58:11.000000 evaics-0.2.8/evaics.egg-info/requires.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        7 2023-05-26 14:58:11.000000 evaics-0.2.8/evaics.egg-info/top_level.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       38 2023-05-26 14:58:11.378689 evaics-0.2.8/setup.cfg
+-rw-r--r--   0 divisor   (1000) root         (0)      787 2023-05-26 14:57:27.000000 evaics-0.2.8/setup.py
```

### Comparing `evaics-0.2.7/LICENSE` & `evaics-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `evaics-0.2.7/PKG-INFO` & `evaics-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evaics
-Version: 0.2.7
+Version: 0.2.8
 Summary: EVA ICS v4 Python SDK
 Home-page: https://github.com/eva-ics/eva4
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `evaics-0.2.7/evaics/client/http.py` & `evaics-0.2.8/evaics/client/http.py`

 * *Files identical despite different names*

### Comparing `evaics-0.2.7/evaics/exceptions.py` & `evaics-0.2.8/evaics/exceptions.py`

 * *Files identical despite different names*

### Comparing `evaics-0.2.7/evaics/sdk/__init__.py` & `evaics-0.2.8/evaics/sdk/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.7'
+__version__ = '0.2.8'
 
 import busrt
 import sys
 import msgpack
 import logging
 import time
 import signal
@@ -363,14 +363,20 @@
 
 class Service:
     """
     The primary service class
     """
 
     def __init__(self):
+        self.svc_info = None
+        self.logger = None
+        self.signals_registered = False
+        self.marked_ready = False
+        self.marked_terminating = False
+        self.privileges_dropped = False
         self.active = True
         stdin = sys.stdin.buffer
         payload_code = stdin.read(1)
         if payload_code[0] != SERVICE_PAYLOAD_INITIAL:
             raise RuntimeError('invalid payload')
         payload_len = int.from_bytes(stdin.read(4), 'little', signed=False)
         self.initial = unpack(stdin.read(payload_len))
@@ -450,14 +456,35 @@
         """
         config = self.initial.get('config')
         if config is None:
             return {}
         else:
             return config
 
+    def init(self, info=None, on_frame=None, on_rpc_call=None):
+        """
+        Init the service
+
+        Automatically calls init_bus, drop_privileges, init_logs and init_rpc
+        (if info specified)
+
+        Optional:
+            info: RPC info
+            on_frame: bus frame handler
+        """
+        self.init_bus()
+        self.drop_privileges()
+        self.init_logs()
+        if info:
+            self.init_rpc(info)
+            if on_frame:
+                self.rpc.on_frame = on_frame
+            if on_rpc_call:
+                self.on_rpc_call = on_rpc_call
+
     def init_bus(self):
         """
         Init the local bus
         """
         bus_config = self.initial['bus']
         if bus_config['type'] != 'native':
             raise ValueError(f'bus {bus_config["type"]} is not supported')
@@ -467,15 +494,16 @@
         self.bus.ping_interval = bus_config['ping_interval']
         self.bus.connect()
 
     def init_rpc(self, svc_info):
         """
         Init bus RPC layer
         """
-        self._svc_info = pack(svc_info.serialize())
+        self.svc_info = svc_info
+        self._svc_info_packed = pack(svc_info.serialize())
         self.rpc = busrt.rpc.Rpc(self.bus)
         self.rpc.on_call = self._handle_rpc_call
 
     def wait_core(self, timeout=None, wait_forever=True):
         """
         Wait until the EVA ICS core is started
         """
@@ -496,15 +524,15 @@
             time.sleep(self.sleep_step)
 
     def _handle_rpc_call(self, event):
         method = event.method
         if method == b'test':
             return
         elif method == b'info':
-            return self._svc_info
+            return self._svc_info_packed
         elif method == b'stop':
             self.active = False
             return
         else:
             return self.on_rpc_call(event)
 
     def init_logs(self):
@@ -522,49 +550,67 @@
         self.log_handler.setFormatter(self.log_formatter)
         logger.addHandler(self.log_handler)
 
         def log_trace(msg, *args, **kwargs):
             logger.log(1, msg, *args, **kwargs)
 
         logger.trace = log_trace
-        return logger
+        self.logger = logger
+        return self.logger
 
     def block(self):
         """
         Block the service until terminated
+
+        Automatically calls register_signals, mark_ready, mark_terminating
+        (after receiving a termination signal/event)
         """
+        self.register_signals()
+        self.mark_ready()
         sleep_step = self.sleep_step
         while self.active and self.bus.is_connected():
             time.sleep(sleep_step)
+        self.mark_terminating()
 
     def mark_ready(self):
         """
         Mark the service ready
+
+        Automatically logs the service is started if logs are initialized
         """
-        self._mark('ready')
+        if not self.marked_ready:
+            self._mark('ready')
+            self.marked_ready = True
+            if self.logger:
+                desc = self.svc_info.description if self.svc_info else None
+                self.logger.info(f'{desc} started' if desc else 'started')
 
     def mark_terminating(self):
         """
         Mark the service terminating
         """
         self.active = False
         self.shutdown_requested = True
-        self._mark('terminating')
+        if not self.marked_terminating:
+            self._mark('terminating')
+            self.marked_terminating = True
 
     def drop_privileges(self):
         """
         Drop service process privileges
         """
-        user = self.initial.get('user')
-        if user is not None:
-            u = pwd.getpwnam(user)
-            groups = os.getgrouplist(user, u.pw_gid)
-            os.setgroups(groups)
-            os.setgid(u.pw_gid)
-            os.setuid(u.pw_uid)
+        if not self.privileges_dropped:
+            user = self.initial.get('user')
+            if user is not None:
+                u = pwd.getpwnam(user)
+                groups = os.getgrouplist(user, u.pw_gid)
+                os.setgroups(groups)
+                os.setgid(u.pw_gid)
+                os.setuid(u.pw_uid)
+            self.privileges_dropped = True
 
     def _mark(self, status):
         self.bus.send(
             'SVC/ST',
             busrt.client.Frame(pack({'status': status}),
                                tp=busrt.client.OP_PUBLISH,
                                qos=0))
```

### Comparing `evaics-0.2.7/evaics/tools.py` & `evaics-0.2.8/evaics/tools.py`

 * *Files identical despite different names*

### Comparing `evaics-0.2.7/evaics.egg-info/PKG-INFO` & `evaics-0.2.8/evaics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evaics
-Version: 0.2.7
+Version: 0.2.8
 Summary: EVA ICS v4 Python SDK
 Home-page: https://github.com/eva-ics/eva4
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `evaics-0.2.7/setup.py` & `evaics-0.2.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.7'
+__version__ = '0.2.8'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
```

