# Comparing `tmp/pixeldb-1.1.2.tar.gz` & `tmp/pixeldb-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixeldb-1.1.2.tar", max compression
+gzip compressed data, was "pixeldb-1.1.3.tar", max compression
```

## Comparing `pixeldb-1.1.2.tar` & `pixeldb-1.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      309 2023-05-25 12:49:33.790602 pixeldb-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      578 2023-05-25 12:44:26.919128 pixeldb-1.1.2/src/pixeldb/__init__.py
--rw-r--r--   0        0        0      568 2023-05-25 12:49:43.461638 pixeldb-1.1.2/setup.py
--rw-r--r--   0        0        0      603 2023-05-25 12:49:43.461856 pixeldb-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      309 2023-05-26 11:53:05.909789 pixeldb-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      591 2023-05-26 11:52:56.333799 pixeldb-1.1.3/src/pixeldb/__init__.py
+-rw-r--r--   0        0        0      568 2023-05-26 11:53:17.559316 pixeldb-1.1.3/setup.py
+-rw-r--r--   0        0        0      603 2023-05-26 11:53:17.559660 pixeldb-1.1.3/PKG-INFO
```

### Comparing `pixeldb-1.1.2/src/pixeldb/__init__.py` & `pixeldb-1.1.3/src/pixeldb/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# PxlDB v1.1 (By PxlmastrXD)
+# PxlDB v1.1.3 (By PxlmastrXD)
 import pickle
 
 
 def version():
   print('PxlDB v1.1')
 
 
@@ -19,12 +19,12 @@
     with open(database, 'rb') as f:
       opendatabase = pickle.load(f)
     self.database = opendatabase
     self.openedfile = database
 
   def set(self, key, value):
     self.database[key] = value
-    with open(self.openedfile) as f:
-      pickle.dump(self.database, f)
+    with open(self.openedfile, 'wb') as f:
+      pickle.dump(str(self.database), f)
 
   def get(self, key):
     return (self.database[key])
```

### Comparing `pixeldb-1.1.2/setup.py` & `pixeldb-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['pixeldb']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'pixeldb',
-    'version': '1.1.2',
+    'version': '1.1.3',
     'description': 'A simple database written in Python.',
     'long_description': None,
     'author': 'PxlmastrXD',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `pixeldb-1.1.2/PKG-INFO` & `pixeldb-1.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixeldb
-Version: 1.1.2
+Version: 1.1.3
 Summary: A simple database written in Python.
 License: MIT
 Author: PxlmastrXD
 Requires-Python: >=3,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

