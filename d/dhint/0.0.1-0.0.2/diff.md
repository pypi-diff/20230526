# Comparing `tmp/dhint-0.0.1.tar.gz` & `tmp/dhint-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhint-0.0.1.tar", max compression
+gzip compressed data, was "dhint-0.0.2.tar", max compression
```

## Comparing `dhint-0.0.1.tar` & `dhint-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      191 2023-05-25 18:46:03.990541 dhint-0.0.1/dhint/__init__.py
--rw-r--r--   0        0        0     8362 2023-05-25 18:49:40.131419 dhint-0.0.1/dhint/base.py
--rw-r--r--   0        0        0     3902 2023-05-25 16:30:23.252226 dhint-0.0.1/dhint/collections.py
--rw-r--r--   0        0        0     2111 2023-05-21 17:56:59.467134 dhint-0.0.1/dhint/functions.py
--rw-r--r--   0        0        0     1425 2023-05-24 11:39:17.174355 dhint-0.0.1/dhint/hints.py
--rw-r--r--   0        0        0     1456 2023-05-25 16:30:23.245883 dhint-0.0.1/dhint/json_encoder.py
--rw-r--r--   0        0        0      375 2023-05-24 11:39:53.142615 dhint-0.0.1/dhint/protocols.py
--rw-r--r--   0        0        0     1444 2023-05-25 16:14:08.029403 dhint-0.0.1/dhint/subdescriptor.py
--rw-r--r--   0        0        0     9880 2023-05-25 18:15:02.476932 dhint-0.0.1/dhint/type_hint.py
--rw-r--r--   0        0        0     3175 2023-05-25 16:30:23.242768 dhint-0.0.1/dhint/types.py
--rw-r--r--   0        0        0      301 2023-05-25 15:44:37.614977 dhint-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      581 2023-05-25 19:39:11.765049 dhint-0.0.1/setup.py
--rw-r--r--   0        0        0      332 2023-05-25 19:39:11.765248 dhint-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      191 2023-05-25 18:46:03.990541 dhint-0.0.2/dhint/__init__.py
+-rw-r--r--   0        0        0     8346 2023-05-26 02:38:50.037408 dhint-0.0.2/dhint/base.py
+-rw-r--r--   0        0        0     3902 2023-05-25 16:30:23.252226 dhint-0.0.2/dhint/collections.py
+-rw-r--r--   0        0        0     2111 2023-05-21 17:56:59.467134 dhint-0.0.2/dhint/functions.py
+-rw-r--r--   0        0        0     1425 2023-05-24 11:39:17.174355 dhint-0.0.2/dhint/hints.py
+-rw-r--r--   0        0        0     1480 2023-05-25 19:55:03.353830 dhint-0.0.2/dhint/json_encoder.py
+-rw-r--r--   0        0        0      375 2023-05-24 11:39:53.142615 dhint-0.0.2/dhint/protocols.py
+-rw-r--r--   0        0        0     1444 2023-05-25 16:14:08.029403 dhint-0.0.2/dhint/subdescriptor.py
+-rw-r--r--   0        0        0     9880 2023-05-25 18:15:02.476932 dhint-0.0.2/dhint/type_hint.py
+-rw-r--r--   0        0        0     3171 2023-05-26 02:38:50.034497 dhint-0.0.2/dhint/types.py
+-rw-r--r--   0        0        0      301 2023-05-26 02:39:04.492682 dhint-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      581 2023-05-26 02:39:13.853251 dhint-0.0.2/setup.py
+-rw-r--r--   0        0        0      332 2023-05-26 02:39:13.853444 dhint-0.0.2/PKG-INFO
```

### Comparing `dhint-0.0.1/dhint/base.py` & `dhint-0.0.2/dhint/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__all__ = ['BaseDetaModel', 'BaseCollection', 'AbstractDescriptor', 'BaseDataclass', 'BaseEnum', 'SearchDescriptor',
+__all__ = ['BaseDetaModel', 'BaseCollection', 'BaseDescriptor', 'BaseDataclass', 'BaseEnum', 'SearchDescriptor',
            'AutoDescriptor', 'NumberDescriptor', 'TextAreaDescriptor', 'RangeDescriptor', 'NoFormDescriptor',
            'HiddenDescriptor', 'BaseContext', 'KeyDescriptor', 'ModelKeyDescriptor', 'SelectDescriptor', ]
 
 from enum import Enum
 from abc import ABC, abstractmethod
 from typing_extensions import Self
 from typing import Callable, Optional, Any, ClassVar, get_type_hints, Union
@@ -58,15 +58,15 @@
     PRIVATE_PARAMS: ClassVar[Optional[str]] = None
     PLURAL: ClassVar[Optional[str]] = None
     SINGULAR: ClassVar[Optional[str]] = None
     INITVARS_NAMES: ClassVar[Optional[list[str]]] = None
     INITFIELDS_NAMES: ClassVar[Optional[list[str]]] = None
     FIELDS_NAMES: ClassVar[Optional[list[str]]] = None
     FIELDS: ClassVar[dict[str, Field]] = None
-    DESCRIPTORS: ClassVar[dict[str, AbstractDescriptor]] = None
+    DESCRIPTORS: ClassVar[dict[str, BaseDescriptor]] = None
     
     @classmethod
     def class_name(cls):
         return cls.__name__
     
     @classmethod
     def class_setup(cls):
@@ -74,15 +74,15 @@
         cls.INITFIELDS_NAMES = cls.initfields_names()
         cls.FIELDS_NAMES = cls.fields_names()
         cls.FIELDS = cls.fields()
     
     @classmethod
     def descriptors(cls):
         mapping = ChainMap(*[vars(item) for item in [m for m in cls.bases() if issubclass(m, BaseDataclass)]])
-        return {key: value for key, value in mapping.items() if isinstance(value, AbstractDescriptor)}
+        return {key: value for key, value in mapping.items() if isinstance(value, BaseDescriptor)}
     
     @classmethod
     def singular(cls):
         return cls.SINGULAR or cls.class_name()
     
     @classmethod
     def plural(cls):
@@ -182,15 +182,15 @@
         assert isinstance(self, (UserString, UserDict, UserList))
 
     @abstractmethod
     def init_data(self)-> Union[str, dict, list]:
         return NotImplemented
 
 
-class AbstractDescriptor(ABC):
+class BaseDescriptor(ABC):
     FIELD_TYPE: ClassVar[Optional[type]] = None
 
     def __init__(self, *args, **kwargs):
         self.args = [item for item in args if not item in [None, '']]
         self._default = kwargs.pop('default', MISSING if self.is_required else None)
         self._default_factory: Callable = kwargs.pop('default_factory', MISSING)
         self._label: Callable = kwargs.pop('label', None)
```

### Comparing `dhint-0.0.1/dhint/collections.py` & `dhint-0.0.2/dhint/collections.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.1/dhint/functions.py` & `dhint-0.0.2/dhint/functions.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.1/dhint/hints.py` & `dhint-0.0.2/dhint/hints.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.1/dhint/json_encoder.py` & `dhint-0.0.2/dhint/json_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 __all__ = [
         'json_dumps',
         'json_parse',
         'json_loads',
-        'JsonEncoder'
+        'JsonEncoder',
+        'JsonEngine'
 ]
 
 import json
 import datetime
 from enum import Enum
 from dataclasses import asdict
 from collections import UserString
 from typing import Any
 from .types import *
 from .collections import *
 from .hints import *
 
+
 class JsonEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, datetime.datetime):
             return obj.isoformat()[:16]
         elif isinstance(obj, datetime.date):
             return obj.isoformat()
         elif isinstance(obj, Enum):
@@ -45,7 +47,8 @@
 def json_dumps(obj: Any) -> str:
     return json.dumps(obj, cls=JsonEncoder, indent=2, ensure_ascii=False)
 
 
 def json_parse(obj: Any) -> Jsonable:
     return json_loads(json_dumps(obj))
 
+
```

### Comparing `dhint-0.0.1/dhint/subdescriptor.py` & `dhint-0.0.2/dhint/subdescriptor.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.1/dhint/type_hint.py` & `dhint-0.0.2/dhint/type_hint.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.1/dhint/types.py` & `dhint-0.0.2/dhint/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     return is_dataclass(obj) and not isinstance_of_type(obj)
 
 
 def isdetamodel_instance(obj: Any) -> bool:
     return not isinstance_of_type(obj) and isinstance(obj, BaseDetaModel)
 
 def isdescriptor(obj: Any) -> bool:
-    return isinstance(obj, AbstractDescriptor)
+    return isinstance(obj, BaseDescriptor)
 
 def issearchfield(obj: Any) -> bool:
     return isinstance(obj, SearchDescriptor) and isdescriptor(obj)
 
 def isautofield(obj: Any) -> bool:
     return isinstance(obj, AutoDescriptor) and isdescriptor(obj)
```

### Comparing `dhint-0.0.1/setup.py` & `dhint-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Unidecode>=1.3.6,<2.0.0']
 
 setup_kwargs = {
     'name': 'dhint',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

