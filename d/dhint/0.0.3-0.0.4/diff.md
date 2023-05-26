# Comparing `tmp/dhint-0.0.3.tar.gz` & `tmp/dhint-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhint-0.0.3.tar", max compression
+gzip compressed data, was "dhint-0.0.4.tar", max compression
```

## Comparing `dhint-0.0.3.tar` & `dhint-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      191 2023-05-25 18:46:03.990541 dhint-0.0.3/dhint/__init__.py
--rw-r--r--   0        0        0     8346 2023-05-26 02:38:50.037408 dhint-0.0.3/dhint/base.py
--rw-r--r--   0        0        0     3902 2023-05-25 16:30:23.252226 dhint-0.0.3/dhint/collections.py
--rw-r--r--   0        0        0     2111 2023-05-21 17:56:59.467134 dhint-0.0.3/dhint/functions.py
--rw-r--r--   0        0        0     1425 2023-05-24 11:39:17.174355 dhint-0.0.3/dhint/hints.py
--rw-r--r--   0        0        0     1459 2023-05-26 03:01:24.856969 dhint-0.0.3/dhint/json_encoder.py
--rw-r--r--   0        0        0      375 2023-05-24 11:39:53.142615 dhint-0.0.3/dhint/protocols.py
--rw-r--r--   0        0        0     1444 2023-05-25 16:14:08.029403 dhint-0.0.3/dhint/subdescriptor.py
--rw-r--r--   0        0        0     9880 2023-05-25 18:15:02.476932 dhint-0.0.3/dhint/type_hint.py
--rw-r--r--   0        0        0     3171 2023-05-26 02:38:50.034497 dhint-0.0.3/dhint/types.py
--rw-r--r--   0        0        0      330 2023-05-26 03:01:24.854398 dhint-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      616 2023-05-26 03:01:31.558007 dhint-0.0.3/setup.py
--rw-r--r--   0        0        0      382 2023-05-26 03:01:31.558198 dhint-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      191 2023-05-25 18:46:03.990541 dhint-0.0.4/dhint/__init__.py
+-rw-r--r--   0        0        0     7712 2023-05-26 12:31:13.795539 dhint-0.0.4/dhint/base.py
+-rw-r--r--   0        0        0     3902 2023-05-25 16:30:23.252226 dhint-0.0.4/dhint/collections.py
+-rw-r--r--   0        0        0     2111 2023-05-21 17:56:59.467134 dhint-0.0.4/dhint/functions.py
+-rw-r--r--   0        0        0     1425 2023-05-24 11:39:17.174355 dhint-0.0.4/dhint/hints.py
+-rw-r--r--   0        0        0     1459 2023-05-26 03:01:24.856969 dhint-0.0.4/dhint/json_encoder.py
+-rw-r--r--   0        0        0      375 2023-05-24 11:39:53.142615 dhint-0.0.4/dhint/protocols.py
+-rw-r--r--   0        0        0     1466 2023-05-26 12:08:08.808018 dhint-0.0.4/dhint/subdescriptor.py
+-rw-r--r--   0        0        0     9880 2023-05-25 18:15:02.476932 dhint-0.0.4/dhint/type_hint.py
+-rw-r--r--   0        0        0     3171 2023-05-26 02:38:50.034497 dhint-0.0.4/dhint/types.py
+-rw-r--r--   0        0        0      330 2023-05-26 12:39:27.703971 dhint-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      616 2023-05-26 12:39:30.953703 dhint-0.0.4/setup.py
+-rw-r--r--   0        0        0      382 2023-05-26 12:39:30.953943 dhint-0.0.4/PKG-INFO
```

### Comparing `dhint-0.0.3/dhint/collections.py` & `dhint-0.0.4/dhint/collections.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.3/dhint/functions.py` & `dhint-0.0.4/dhint/functions.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.3/dhint/hints.py` & `dhint-0.0.4/dhint/hints.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.3/dhint/json_encoder.py` & `dhint-0.0.4/dhint/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.3/dhint/subdescriptor.py` & `dhint-0.0.4/dhint/subdescriptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 __all__ = ['SearchDescriptor', 'AutoDescriptor', 'NumberDescriptor', 'TextAreaDescriptor', 'RangeDescriptor',
            'NoFormDescriptor', 'HiddenDescriptor', 'KeyDescriptor', 'ModelKeyDescriptor', 'SelectDescriptor',
            'StringDescriptor', 'DecimalDescriptor', 'FloatDescriptor', 'IntDescriptor', 'BoolDescriptor',
-           'MultipleDescriptor']
+           'MultipleDescriptor', 'DescriptorSubclass']
 
 from abc import ABC
 
 
 class DescriptorSubclass(ABC):
     """Used for make base subclasses for specific descriptor classes"""
```

### Comparing `dhint-0.0.3/dhint/type_hint.py` & `dhint-0.0.4/dhint/type_hint.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.3/dhint/types.py` & `dhint-0.0.4/dhint/types.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.3/setup.py` & `dhint-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Unidecode>=1.3.6,<2.0.0', 'typing-extensions>=4.6.2,<5.0.0']
 
 setup_kwargs = {
     'name': 'dhint',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

