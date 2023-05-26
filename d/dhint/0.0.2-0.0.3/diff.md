# Comparing `tmp/dhint-0.0.2.tar.gz` & `tmp/dhint-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhint-0.0.2.tar", max compression
+gzip compressed data, was "dhint-0.0.3.tar", max compression
```

## Comparing `dhint-0.0.2.tar` & `dhint-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      191 2023-05-25 18:46:03.990541 dhint-0.0.2/dhint/__init__.py
--rw-r--r--   0        0        0     8346 2023-05-26 02:38:50.037408 dhint-0.0.2/dhint/base.py
--rw-r--r--   0        0        0     3902 2023-05-25 16:30:23.252226 dhint-0.0.2/dhint/collections.py
--rw-r--r--   0        0        0     2111 2023-05-21 17:56:59.467134 dhint-0.0.2/dhint/functions.py
--rw-r--r--   0        0        0     1425 2023-05-24 11:39:17.174355 dhint-0.0.2/dhint/hints.py
--rw-r--r--   0        0        0     1480 2023-05-25 19:55:03.353830 dhint-0.0.2/dhint/json_encoder.py
--rw-r--r--   0        0        0      375 2023-05-24 11:39:53.142615 dhint-0.0.2/dhint/protocols.py
--rw-r--r--   0        0        0     1444 2023-05-25 16:14:08.029403 dhint-0.0.2/dhint/subdescriptor.py
--rw-r--r--   0        0        0     9880 2023-05-25 18:15:02.476932 dhint-0.0.2/dhint/type_hint.py
--rw-r--r--   0        0        0     3171 2023-05-26 02:38:50.034497 dhint-0.0.2/dhint/types.py
--rw-r--r--   0        0        0      301 2023-05-26 02:39:04.492682 dhint-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      581 2023-05-26 02:39:13.853251 dhint-0.0.2/setup.py
--rw-r--r--   0        0        0      332 2023-05-26 02:39:13.853444 dhint-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      191 2023-05-25 18:46:03.990541 dhint-0.0.3/dhint/__init__.py
+-rw-r--r--   0        0        0     8346 2023-05-26 02:38:50.037408 dhint-0.0.3/dhint/base.py
+-rw-r--r--   0        0        0     3902 2023-05-25 16:30:23.252226 dhint-0.0.3/dhint/collections.py
+-rw-r--r--   0        0        0     2111 2023-05-21 17:56:59.467134 dhint-0.0.3/dhint/functions.py
+-rw-r--r--   0        0        0     1425 2023-05-24 11:39:17.174355 dhint-0.0.3/dhint/hints.py
+-rw-r--r--   0        0        0     1459 2023-05-26 03:01:24.856969 dhint-0.0.3/dhint/json_encoder.py
+-rw-r--r--   0        0        0      375 2023-05-24 11:39:53.142615 dhint-0.0.3/dhint/protocols.py
+-rw-r--r--   0        0        0     1444 2023-05-25 16:14:08.029403 dhint-0.0.3/dhint/subdescriptor.py
+-rw-r--r--   0        0        0     9880 2023-05-25 18:15:02.476932 dhint-0.0.3/dhint/type_hint.py
+-rw-r--r--   0        0        0     3171 2023-05-26 02:38:50.034497 dhint-0.0.3/dhint/types.py
+-rw-r--r--   0        0        0      330 2023-05-26 03:01:24.854398 dhint-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      616 2023-05-26 03:01:31.558007 dhint-0.0.3/setup.py
+-rw-r--r--   0        0        0      382 2023-05-26 03:01:31.558198 dhint-0.0.3/PKG-INFO
```

### Comparing `dhint-0.0.2/dhint/base.py` & `dhint-0.0.3/dhint/base.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.2/dhint/collections.py` & `dhint-0.0.3/dhint/collections.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.2/dhint/functions.py` & `dhint-0.0.3/dhint/functions.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.2/dhint/hints.py` & `dhint-0.0.3/dhint/hints.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.2/dhint/json_encoder.py` & `dhint-0.0.3/dhint/json_encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 __all__ = [
         'json_dumps',
         'json_parse',
         'json_loads',
         'JsonEncoder',
-        'JsonEngine'
 ]
 
 import json
 import datetime
 from enum import Enum
 from dataclasses import asdict
 from collections import UserString
```

### Comparing `dhint-0.0.2/dhint/subdescriptor.py` & `dhint-0.0.3/dhint/subdescriptor.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.2/dhint/type_hint.py` & `dhint-0.0.3/dhint/type_hint.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.2/dhint/types.py` & `dhint-0.0.3/dhint/types.py`

 * *Files identical despite different names*

