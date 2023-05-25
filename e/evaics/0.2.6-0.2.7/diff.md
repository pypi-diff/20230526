# Comparing `tmp/evaics-0.2.6.tar.gz` & `tmp/evaics-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evaics-0.2.6.tar", last modified: Tue Mar 28 15:16:24 2023, max compression
+gzip compressed data, was "evaics-0.2.7.tar", last modified: Thu May 25 23:39:47 2023, max compression
```

## Comparing `evaics-0.2.6.tar` & `evaics-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 divisor   (1000) divisor   (1000)        0 2023-03-28 15:16:24.316418 evaics-0.2.6/
--rw-rw-r--   0 divisor   (1000) divisor   (1000)      674 2023-03-28 15:16:24.316418 evaics-0.2.6/PKG-INFO
--rw-rw-r--   0 divisor   (1000) divisor   (1000)      141 2022-10-03 21:34:26.000000 evaics-0.2.6/README.md
-drwxrwxr-x   0 divisor   (1000) divisor   (1000)        0 2023-03-28 15:16:24.316418 evaics-0.2.6/evaics/
--rw-rw-r--   0 divisor   (1000) divisor   (1000)        0 2023-03-28 15:16:23.000000 evaics-0.2.6/evaics/__init__.py
-drwxrwxr-x   0 divisor   (1000) divisor   (1000)        0 2023-03-28 15:16:24.316418 evaics-0.2.6/evaics/client/
--rw-rw-r--   0 divisor   (1000) divisor   (1000)      131 2023-03-28 15:16:23.000000 evaics-0.2.6/evaics/client/__init__.py
--rw-rw-r--   0 divisor   (1000) divisor   (1000)     4559 2023-03-28 15:16:23.000000 evaics-0.2.6/evaics/client/http.py
--rw-rw-r--   0 divisor   (1000) divisor   (1000)     1821 2023-03-28 15:16:23.000000 evaics-0.2.6/evaics/exceptions.py
-drwxrwxr-x   0 divisor   (1000) divisor   (1000)        0 2023-03-28 15:16:24.316418 evaics-0.2.6/evaics/sdk/
--rw-rw-r--   0 divisor   (1000) divisor   (1000)    25662 2023-03-28 15:16:23.000000 evaics-0.2.6/evaics/sdk/__init__.py
--rw-rw-r--   0 divisor   (1000) divisor   (1000)     1116 2023-03-28 15:16:23.000000 evaics-0.2.6/evaics/tools.py
-drwxrwxr-x   0 divisor   (1000) divisor   (1000)        0 2023-03-28 15:16:24.316418 evaics-0.2.6/evaics.egg-info/
--rw-rw-r--   0 divisor   (1000) divisor   (1000)      674 2023-03-28 15:16:24.000000 evaics-0.2.6/evaics.egg-info/PKG-INFO
--rw-rw-r--   0 divisor   (1000) divisor   (1000)      294 2023-03-28 15:16:24.000000 evaics-0.2.6/evaics.egg-info/SOURCES.txt
--rw-rw-r--   0 divisor   (1000) divisor   (1000)        1 2023-03-28 15:16:24.000000 evaics-0.2.6/evaics.egg-info/dependency_links.txt
--rw-rw-r--   0 divisor   (1000) divisor   (1000)       28 2023-03-28 15:16:24.000000 evaics-0.2.6/evaics.egg-info/requires.txt
--rw-rw-r--   0 divisor   (1000) divisor   (1000)        7 2023-03-28 15:16:24.000000 evaics-0.2.6/evaics.egg-info/top_level.txt
--rw-rw-r--   0 divisor   (1000) divisor   (1000)       38 2023-03-28 15:16:24.316418 evaics-0.2.6/setup.cfg
--rw-rw-r--   0 divisor   (1000) divisor   (1000)      787 2023-03-28 15:16:23.000000 evaics-0.2.6/setup.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-25 23:39:47.288528 evaics-0.2.7/
+-rw-r--r--   0 divisor   (1000) root         (0)    10639 2022-06-30 23:31:52.000000 evaics-0.2.7/LICENSE
+-rw-r--r--   0 divisor   (1000) root         (0)      637 2023-05-25 23:39:47.288528 evaics-0.2.7/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      141 2022-10-03 20:48:30.000000 evaics-0.2.7/README.md
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-25 23:39:47.288528 evaics-0.2.7/evaics/
+-rw-r--r--   0 divisor   (1000) root         (0)        0 2023-05-25 22:53:36.000000 evaics-0.2.7/evaics/__init__.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-25 23:39:47.288528 evaics-0.2.7/evaics/client/
+-rw-r--r--   0 divisor   (1000) root         (0)      131 2023-05-25 22:53:36.000000 evaics-0.2.7/evaics/client/__init__.py
+-rw-r--r--   0 divisor   (1000) root         (0)     4559 2023-05-25 22:53:36.000000 evaics-0.2.7/evaics/client/http.py
+-rw-r--r--   0 divisor   (1000) root         (0)     1821 2023-05-25 22:53:36.000000 evaics-0.2.7/evaics/exceptions.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-25 23:39:47.288528 evaics-0.2.7/evaics/sdk/
+-rw-r--r--   0 divisor   (1000) root         (0)    25786 2023-05-25 22:53:36.000000 evaics-0.2.7/evaics/sdk/__init__.py
+-rw-r--r--   0 divisor   (1000) root         (0)     1116 2023-05-25 22:53:36.000000 evaics-0.2.7/evaics/tools.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-25 23:39:47.288528 evaics-0.2.7/evaics.egg-info/
+-rw-r--r--   0 divisor   (1000) root         (0)      637 2023-05-25 23:39:47.000000 evaics-0.2.7/evaics.egg-info/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      302 2023-05-25 23:39:47.000000 evaics-0.2.7/evaics.egg-info/SOURCES.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        1 2023-05-25 23:39:47.000000 evaics-0.2.7/evaics.egg-info/dependency_links.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       28 2023-05-25 23:39:47.000000 evaics-0.2.7/evaics.egg-info/requires.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        7 2023-05-25 23:39:47.000000 evaics-0.2.7/evaics.egg-info/top_level.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       38 2023-05-25 23:39:47.288528 evaics-0.2.7/setup.cfg
+-rw-r--r--   0 divisor   (1000) root         (0)      787 2023-05-25 22:53:36.000000 evaics-0.2.7/setup.py
```

### Comparing `evaics-0.2.6/PKG-INFO` & `evaics-0.2.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: evaics
-Version: 0.2.6
+Version: 0.2.7
 Summary: EVA ICS v4 Python SDK
 Home-page: https://github.com/eva-ics/eva4
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
-Description: # EVA ICS v4 SDK (Python)
-        
-        EVA ICS v4 software development kit (Python)
-        
-        Technical documentation: <https://info.bma.ai/en/actual/eva4/sdk/>
-        
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Communications
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# EVA ICS v4 SDK (Python)
+
+EVA ICS v4 software development kit (Python)
+
+Technical documentation: <https://info.bma.ai/en/actual/eva4/sdk/>
+
+
+
```

### Comparing `evaics-0.2.6/evaics/client/http.py` & `evaics-0.2.7/evaics/client/http.py`

 * *Files identical despite different names*

### Comparing `evaics-0.2.6/evaics/exceptions.py` & `evaics-0.2.7/evaics/exceptions.py`

 * *Files identical despite different names*

### Comparing `evaics-0.2.6/evaics/sdk/__init__.py` & `evaics-0.2.7/evaics/sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.6'
+__version__ = '0.2.7'
 
 import busrt
 import sys
 import msgpack
 import logging
 import time
 import signal
@@ -609,17 +609,21 @@
             topic_pfx = LOCAL_STATE_TOPIC
         else:
             raise ValueError('Invalid event kind (accepted:'
                              ' any, remote, remote_arcive or local)')
         topics = []
         if oids:
             for oid in oids:
-                if isinstance(oid, str):
-                    oid = OID(oid)
-                topics.append(f'{topic_pfx}{oid.to_path()}')
+                if oid == '#':
+                    path = oid
+                else:
+                    if isinstance(oid, str):
+                        oid = OID(oid)
+                    path = oid.to_path()
+                topics.append(f'{topic_pfx}{path}')
             self.bus.subscribe(topics).wait_completed()
 
 
 def no_rpc_method():
     """
     Raise an exception on invalid RPC method
     """
```

### Comparing `evaics-0.2.6/evaics/tools.py` & `evaics-0.2.7/evaics/tools.py`

 * *Files identical despite different names*

### Comparing `evaics-0.2.6/evaics.egg-info/PKG-INFO` & `evaics-0.2.7/evaics.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: evaics
-Version: 0.2.6
+Version: 0.2.7
 Summary: EVA ICS v4 Python SDK
 Home-page: https://github.com/eva-ics/eva4
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
-Description: # EVA ICS v4 SDK (Python)
-        
-        EVA ICS v4 software development kit (Python)
-        
-        Technical documentation: <https://info.bma.ai/en/actual/eva4/sdk/>
-        
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Communications
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# EVA ICS v4 SDK (Python)
+
+EVA ICS v4 software development kit (Python)
+
+Technical documentation: <https://info.bma.ai/en/actual/eva4/sdk/>
+
+
+
```

### Comparing `evaics-0.2.6/setup.py` & `evaics-0.2.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.6'
+__version__ = '0.2.7'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
```

