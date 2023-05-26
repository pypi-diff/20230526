# Comparing `tmp/dhint-0.0.4.tar.gz` & `tmp/dhint-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhint-0.0.4.tar", max compression
+gzip compressed data, was "dhint-0.0.5.tar", max compression
```

## Comparing `dhint-0.0.4.tar` & `dhint-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      191 2023-05-25 18:46:03.990541 dhint-0.0.4/dhint/__init__.py
--rw-r--r--   0        0        0     7712 2023-05-26 12:31:13.795539 dhint-0.0.4/dhint/base.py
--rw-r--r--   0        0        0     3902 2023-05-25 16:30:23.252226 dhint-0.0.4/dhint/collections.py
--rw-r--r--   0        0        0     2111 2023-05-21 17:56:59.467134 dhint-0.0.4/dhint/functions.py
--rw-r--r--   0        0        0     1425 2023-05-24 11:39:17.174355 dhint-0.0.4/dhint/hints.py
--rw-r--r--   0        0        0     1459 2023-05-26 03:01:24.856969 dhint-0.0.4/dhint/json_encoder.py
--rw-r--r--   0        0        0      375 2023-05-24 11:39:53.142615 dhint-0.0.4/dhint/protocols.py
--rw-r--r--   0        0        0     1466 2023-05-26 12:08:08.808018 dhint-0.0.4/dhint/subdescriptor.py
--rw-r--r--   0        0        0     9880 2023-05-25 18:15:02.476932 dhint-0.0.4/dhint/type_hint.py
--rw-r--r--   0        0        0     3171 2023-05-26 02:38:50.034497 dhint-0.0.4/dhint/types.py
--rw-r--r--   0        0        0      330 2023-05-26 12:39:27.703971 dhint-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      616 2023-05-26 12:39:30.953703 dhint-0.0.4/setup.py
--rw-r--r--   0        0        0      382 2023-05-26 12:39:30.953943 dhint-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      220 2023-05-26 17:43:41.774221 dhint-0.0.5/dhint/__init__.py
+-rw-r--r--   0        0        0     7759 2023-05-26 17:43:41.772127 dhint-0.0.5/dhint/base.py
+-rw-r--r--   0        0        0     3902 2023-05-25 16:30:23.252226 dhint-0.0.5/dhint/collections.py
+-rw-r--r--   0        0        0     2111 2023-05-21 17:56:59.467134 dhint-0.0.5/dhint/functions.py
+-rw-r--r--   0        0        0     1425 2023-05-24 11:39:17.174355 dhint-0.0.5/dhint/hints.py
+-rw-r--r--   0        0        0     1459 2023-05-26 03:01:24.856969 dhint-0.0.5/dhint/json_encoder.py
+-rw-r--r--   0        0        0      375 2023-05-24 11:39:53.142615 dhint-0.0.5/dhint/protocols.py
+-rw-r--r--   0        0        0     1466 2023-05-26 12:08:08.808018 dhint-0.0.5/dhint/subdescriptor.py
+-rw-r--r--   0        0        0     9880 2023-05-25 18:15:02.476932 dhint-0.0.5/dhint/type_hint.py
+-rw-r--r--   0        0        0     3171 2023-05-26 02:38:50.034497 dhint-0.0.5/dhint/types.py
+-rw-r--r--   0        0        0      330 2023-05-26 17:45:55.539685 dhint-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      616 2023-05-26 17:46:02.951814 dhint-0.0.5/setup.py
+-rw-r--r--   0        0        0      382 2023-05-26 17:46:02.952010 dhint-0.0.5/PKG-INFO
```

### Comparing `dhint-0.0.4/dhint/base.py` & `dhint-0.0.5/dhint/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,16 @@
     def options(cls, default: str = None):
         if default:
             if isinstance(default, cls):
                 default = default.name
         return ''.join([cls.option(), *[cls.option(member, member.key == default) for member in cls.members()]])
 
 
+
+
 @dataclass
 class BaseDataclass(ABC):
     PRIVATE_PARAMS: ClassVar[Optional[str]] = None
     PLURAL: ClassVar[Optional[str]] = None
     SINGULAR: ClassVar[Optional[str]] = None
     INITVARS_NAMES: ClassVar[Optional[list[str]]] = None
     INITFIELDS_NAMES: ClassVar[Optional[list[str]]] = None
@@ -69,14 +71,15 @@
     
     @classmethod
     def class_setup(cls):
         cls.INITVARS_NAMES = cls.initvars_names()
         cls.INITFIELDS_NAMES = cls.initfields_names()
         cls.FIELDS_NAMES = cls.fields_names()
         cls.FIELDS = cls.fields()
+        cls.DESCRIPTORS = cls.descriptors()
     
     @classmethod
     def descriptors(cls):
         mapping = ChainMap(*[vars(item) for item in [m for m in cls.bases() if issubclass(m, BaseDataclass)]])
         return {key: value for key, value in mapping.items() if isinstance(value, BaseDescriptor)}
     
     @classmethod
@@ -145,14 +148,15 @@
         return cls.INITFIELDS_NAMES or [*cls.initvars_names(), *cls.fields_names()]
     
     @classmethod
     def initvars_names(cls) -> list[str]:
         return cls.INITVARS_NAMES or list(cls.init_var_fields().keys())
 
 
+
 @dataclass
 class BaseDetaModel(BaseDataclass):
     TABLE: ClassVar[Optional[str]] = None
     ITEM_NAME: ClassVar[Optional[str]] = None
 
     @classmethod
     def table(cls):
```

### Comparing `dhint-0.0.4/dhint/collections.py` & `dhint-0.0.5/dhint/collections.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.4/dhint/functions.py` & `dhint-0.0.5/dhint/functions.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.4/dhint/hints.py` & `dhint-0.0.5/dhint/hints.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.4/dhint/json_encoder.py` & `dhint-0.0.5/dhint/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.4/dhint/subdescriptor.py` & `dhint-0.0.5/dhint/subdescriptor.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.4/dhint/type_hint.py` & `dhint-0.0.5/dhint/type_hint.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.4/dhint/types.py` & `dhint-0.0.5/dhint/types.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.4/setup.py` & `dhint-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Unidecode>=1.3.6,<2.0.0', 'typing-extensions>=4.6.2,<5.0.0']
 
 setup_kwargs = {
     'name': 'dhint',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

