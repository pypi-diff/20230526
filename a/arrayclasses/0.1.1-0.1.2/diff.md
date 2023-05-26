# Comparing `tmp/arrayclasses-0.1.1.tar.gz` & `tmp/arrayclasses-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrayclasses-0.1.1.tar", max compression
+gzip compressed data, was "arrayclasses-0.1.2.tar", max compression
```

## Comparing `arrayclasses-0.1.1.tar` & `arrayclasses-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-05-26 18:48:49.288191 arrayclasses-0.1.1/LICENSE
--rw-r--r--   0        0        0      731 2023-05-26 18:39:05.635839 arrayclasses-0.1.1/README.md
--rw-r--r--   0        0        0      667 2023-05-26 18:45:09.172843 arrayclasses-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      121 2023-05-26 18:28:15.092746 arrayclasses-0.1.1/src/arrayclasses/__init__.py
--rw-r--r--   0        0        0     3295 2023-05-26 18:31:27.283474 arrayclasses-0.1.1/src/arrayclasses/wrapper.py
--rw-r--r--   0        0        0     1533 2023-05-26 18:49:19.350574 arrayclasses-0.1.1/setup.py
--rw-r--r--   0        0        0     1405 2023-05-26 18:49:19.350813 arrayclasses-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-26 18:48:49.288191 arrayclasses-0.1.2/LICENSE
+-rw-r--r--   0        0        0      731 2023-05-26 18:39:05.635839 arrayclasses-0.1.2/README.md
+-rw-r--r--   0        0        0      685 2023-05-26 19:04:05.537477 arrayclasses-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      121 2023-05-26 18:28:15.092746 arrayclasses-0.1.2/src/arrayclasses/__init__.py
+-rw-r--r--   0        0        0     3290 2023-05-26 18:53:46.326271 arrayclasses-0.1.2/src/arrayclasses/wrapper.py
+-rw-r--r--   0        0        0     1533 2023-05-26 19:07:00.413474 arrayclasses-0.1.2/setup.py
+-rw-r--r--   0        0        0     1355 2023-05-26 19:07:00.413690 arrayclasses-0.1.2/PKG-INFO
```

### Comparing `arrayclasses-0.1.1/LICENSE` & `arrayclasses-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arrayclasses-0.1.1/README.md` & `arrayclasses-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `arrayclasses-0.1.1/pyproject.toml` & `arrayclasses-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arrayclasses"
-version = "0.1.1"
+version = "0.1.2"
 description = "Analogue to dataclass that uses a numpy-backed array to store values."
 authors = ["Lukas Tenbrink <lukas.tenbrink@gmail.com>"]
 keywords = ["numpy", "dataclass"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/Ivorforce/python-arrayclass"
 repository = "https://github.com/Ivorforce/python-arrayclass"
@@ -12,15 +12,16 @@
     "LICENSE",
 ]
 packages = [
     { include = "arrayclasses", from = "src" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 numpy = "^1.24.3"
 
 [tool.poetry.dev-dependencies]
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `arrayclasses-0.1.1/src/arrayclasses/wrapper.py` & `arrayclasses-0.1.2/src/arrayclasses/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
         properties[f.name] = property(fget=get, fset=set)
 
         values_offsets.append(value_count)
         value_count += field_length
 
     # cls.values will be treated as if added by the user, resolving to a field
-    cls = dataclasses._process_class(cls, **kwargs)
+    cls = dataclasses.dataclass(cls, **kwargs)
 
     # Add the created properties.
     # Needs to happen after dataclasses.dataclass() because that one queries the assignments (field() or defaults)
     for name, prop in properties.items():
         setattr(cls, name, prop)
         pass
```

### Comparing `arrayclasses-0.1.1/setup.py` & `arrayclasses-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.24.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'arrayclasses',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Analogue to dataclass that uses a numpy-backed array to store values.',
     'long_description': '# arrayclass\n\nA small `@dataclass`-like decorator for python classes. The class will store its values in a single contiguous [numpy](https://numpy.org) array. It can also be converted to and from plain numpy arrays.\n\n## Installation\n\n`poetry add dataclasses` or `pip install dataclasses`\n\n## Usage\n\n```py\nimport arrayclasses\n\n@arrayclasses.arrayclass\nclass State:\n    x: float\n    y: tuple[float, float]\n    z: float\n\n# Object creation\nstate = State(x=5, y=(0, 1), z=0)\nprint(np.x)  # Prints 5.0\nprint(np.y)  # Prints np.array([0.0, 1.0])\nstate.y = 2.0\nprint(np.y)  # Prints np.array([2.0, 2.0])\n\n# Array conversion.\nstate = arrayclasses.from_array((5, 0, 1, 0))\nprint(np.array(state))  # prints np.array([5.0, 0.0, 1.0, 0.0])\n```\n',
     'author': 'Lukas Tenbrink',
     'author_email': 'lukas.tenbrink@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Ivorforce/python-arrayclass',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `arrayclasses-0.1.1/PKG-INFO` & `arrayclasses-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: arrayclasses
-Version: 0.1.1
+Version: 0.1.2
 Summary: Analogue to dataclass that uses a numpy-backed array to store values.
 Home-page: https://github.com/Ivorforce/python-arrayclass
 License: MIT
 Keywords: numpy,dataclass
 Author: Lukas Tenbrink
 Author-email: lukas.tenbrink@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Project-URL: Repository, https://github.com/Ivorforce/python-arrayclass
 Description-Content-Type: text/markdown
 
 # arrayclass
```

