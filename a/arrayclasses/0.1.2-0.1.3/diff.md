# Comparing `tmp/arrayclasses-0.1.2.tar.gz` & `tmp/arrayclasses-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrayclasses-0.1.2.tar", max compression
+gzip compressed data, was "arrayclasses-0.1.3.tar", max compression
```

## Comparing `arrayclasses-0.1.2.tar` & `arrayclasses-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-05-26 18:48:49.288191 arrayclasses-0.1.2/LICENSE
--rw-r--r--   0        0        0      731 2023-05-26 18:39:05.635839 arrayclasses-0.1.2/README.md
--rw-r--r--   0        0        0      685 2023-05-26 19:04:05.537477 arrayclasses-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      121 2023-05-26 18:28:15.092746 arrayclasses-0.1.2/src/arrayclasses/__init__.py
--rw-r--r--   0        0        0     3290 2023-05-26 18:53:46.326271 arrayclasses-0.1.2/src/arrayclasses/wrapper.py
--rw-r--r--   0        0        0     1533 2023-05-26 19:07:00.413474 arrayclasses-0.1.2/setup.py
--rw-r--r--   0        0        0     1355 2023-05-26 19:07:00.413690 arrayclasses-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-26 18:48:49.288191 arrayclasses-0.1.3/LICENSE
+-rw-r--r--   0        0        0      731 2023-05-26 18:39:05.635839 arrayclasses-0.1.3/README.md
+-rw-r--r--   0        0        0      685 2023-05-26 19:45:38.991969 arrayclasses-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      121 2023-05-26 18:28:15.092746 arrayclasses-0.1.3/src/arrayclasses/__init__.py
+-rw-r--r--   0        0        0     3508 2023-05-26 19:44:05.265345 arrayclasses-0.1.3/src/arrayclasses/wrapper.py
+-rw-r--r--   0        0        0     1533 2023-05-26 19:45:43.327612 arrayclasses-0.1.3/setup.py
+-rw-r--r--   0        0        0     1355 2023-05-26 19:45:43.327820 arrayclasses-0.1.3/PKG-INFO
```

### Comparing `arrayclasses-0.1.2/LICENSE` & `arrayclasses-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arrayclasses-0.1.2/README.md` & `arrayclasses-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `arrayclasses-0.1.2/pyproject.toml` & `arrayclasses-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arrayclasses"
-version = "0.1.2"
+version = "0.1.3"
 description = "Analogue to dataclass that uses a numpy-backed array to store values."
 authors = ["Lukas Tenbrink <lukas.tenbrink@gmail.com>"]
 keywords = ["numpy", "dataclass"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/Ivorforce/python-arrayclass"
 repository = "https://github.com/Ivorforce/python-arrayclass"
```

### Comparing `arrayclasses-0.1.2/src/arrayclasses/wrapper.py` & `arrayclasses-0.1.3/src/arrayclasses/wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
         raise RuntimeError(
             f"cannot construct arrayclass '{cls}' of length {cls.__VALUES_LEN__} from array of length {len(array)}"
         )
 
     return cls(*np.split(array, cls.__VALUES_OFFSETS__[1:]))
 
 
-def to_array(object):
-    return np.copy(object.values)
+def to_array(object, *args, **kwargs):
+    return np.array(object.values, *args, **kwargs)
 
 
 def get_len(object):
     return len(object.values)
 
 
 def getitem(object, item):
@@ -65,29 +65,33 @@
         dataclasses._get_field(cls, name, type)
         for name, type in cls_annotations.items()
     ]
 
     value_count = 0
     properties = dict()
     values_offsets = []
+    types = []
 
     # This will be called when the first setter is called in __init__.
     def create_values_field(self):
-        self.values = np.empty(value_count)
+        self.values = np.empty(value_count, dtype=common_type)
 
     # Go through all the fields and prepare getters / setters.
     for f in cls_fields:
-        field_length = len(typing.get_args(f.type))
+        type_args = typing.get_args(f.type)
+        field_length = len(type_args)
         if field_length == 0:
             # Single value
             index = value_count
             field_length = 1
+            types.append(f.type)
         else:
             # Multi-Value
             index = slice(value_count, value_count + field_length)
+            types.extend(type_args)
 
         # index=index is a dirty hack; it would be better to construct the function from code
         # but eh, that takes effort, right?
         def get(self, *, index=index):
             return self.values[index]
 
         def set(self, value, *, index=index):
@@ -96,14 +100,16 @@
             self.values[index] = value
 
         properties[f.name] = property(fget=get, fset=set)
 
         values_offsets.append(value_count)
         value_count += field_length
 
+    common_type = np.find_common_type([], types)
+
     # cls.values will be treated as if added by the user, resolving to a field
     cls = dataclasses.dataclass(cls, **kwargs)
 
     # Add the created properties.
     # Needs to happen after dataclasses.dataclass() because that one queries the assignments (field() or defaults)
     for name, prop in properties.items():
         setattr(cls, name, prop)
```

### Comparing `arrayclasses-0.1.2/setup.py` & `arrayclasses-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.24.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'arrayclasses',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Analogue to dataclass that uses a numpy-backed array to store values.',
     'long_description': '# arrayclass\n\nA small `@dataclass`-like decorator for python classes. The class will store its values in a single contiguous [numpy](https://numpy.org) array. It can also be converted to and from plain numpy arrays.\n\n## Installation\n\n`poetry add dataclasses` or `pip install dataclasses`\n\n## Usage\n\n```py\nimport arrayclasses\n\n@arrayclasses.arrayclass\nclass State:\n    x: float\n    y: tuple[float, float]\n    z: float\n\n# Object creation\nstate = State(x=5, y=(0, 1), z=0)\nprint(np.x)  # Prints 5.0\nprint(np.y)  # Prints np.array([0.0, 1.0])\nstate.y = 2.0\nprint(np.y)  # Prints np.array([2.0, 2.0])\n\n# Array conversion.\nstate = arrayclasses.from_array((5, 0, 1, 0))\nprint(np.array(state))  # prints np.array([5.0, 0.0, 1.0, 0.0])\n```\n',
     'author': 'Lukas Tenbrink',
     'author_email': 'lukas.tenbrink@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Ivorforce/python-arrayclass',
```

### Comparing `arrayclasses-0.1.2/PKG-INFO` & `arrayclasses-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrayclasses
-Version: 0.1.2
+Version: 0.1.3
 Summary: Analogue to dataclass that uses a numpy-backed array to store values.
 Home-page: https://github.com/Ivorforce/python-arrayclass
 License: MIT
 Keywords: numpy,dataclass
 Author: Lukas Tenbrink
 Author-email: lukas.tenbrink@gmail.com
 Requires-Python: >=3.9,<4.0
```

