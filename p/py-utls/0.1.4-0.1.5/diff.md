# Comparing `tmp/py-utls-0.1.4.tar.gz` & `tmp/py-utls-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-utls-0.1.4.tar", last modified: Wed Mar 15 09:53:37 2023, max compression
+gzip compressed data, was "py-utls-0.1.5.tar", last modified: Fri May 26 08:54:48 2023, max compression
```

## Comparing `py-utls-0.1.4.tar` & `py-utls-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-03-15 09:53:37.493081 py-utls-0.1.4/
--rw-r--r--   0 cyrildever   (501) staff       (20)     1068 2022-02-18 10:33:22.000000 py-utls-0.1.4/LICENSE
--rw-r--r--   0 cyrildever   (501) staff       (20)       19 2022-02-18 13:13:47.000000 py-utls-0.1.4/MANIFEST.in
--rw-r--r--   0 cyrildever   (501) staff       (20)     2016 2023-03-15 09:53:37.492769 py-utls-0.1.4/PKG-INFO
--rw-r--r--   0 cyrildever   (501) staff       (20)     1519 2023-03-14 18:31:44.000000 py-utls-0.1.4/README.md
--rw-r--r--   0 cyrildever   (501) staff       (20)      103 2022-02-18 12:53:08.000000 py-utls-0.1.4/pyproject.toml
--rw-r--r--   0 cyrildever   (501) staff       (20)       38 2023-03-15 09:53:37.493169 py-utls-0.1.4/setup.cfg
--rw-r--r--   0 cyrildever   (501) staff       (20)      882 2023-03-15 09:53:05.000000 py-utls-0.1.4/setup.py
-drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-03-15 09:53:37.486347 py-utls-0.1.4/src/
-drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-03-15 09:53:37.489661 py-utls-0.1.4/src/py_utls.egg-info/
--rw-r--r--   0 cyrildever   (501) staff       (20)     2016 2023-03-15 09:53:37.000000 py-utls-0.1.4/src/py_utls.egg-info/PKG-INFO
--rw-r--r--   0 cyrildever   (501) staff       (20)      293 2023-03-15 09:53:37.000000 py-utls-0.1.4/src/py_utls.egg-info/SOURCES.txt
--rw-r--r--   0 cyrildever   (501) staff       (20)        1 2023-03-15 09:53:37.000000 py-utls-0.1.4/src/py_utls.egg-info/dependency_links.txt
--rw-r--r--   0 cyrildever   (501) staff       (20)        7 2023-03-15 09:53:37.000000 py-utls-0.1.4/src/py_utls.egg-info/top_level.txt
-drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-03-15 09:53:37.490990 py-utls-0.1.4/src/pyutls/
--rw-r--r--   0 cyrildever   (501) staff       (20)        0 2022-02-18 12:53:08.000000 py-utls-0.1.4/src/pyutls/__init__.py
--rw-r--r--   0 cyrildever   (501) staff       (20)      414 2022-11-28 14:20:58.000000 py-utls-0.1.4/src/pyutls/hex.py
--rw-r--r--   0 cyrildever   (501) staff       (20)      104 2022-02-18 12:53:08.000000 py-utls-0.1.4/src/pyutls/list.py
-drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-03-15 09:53:37.492050 py-utls-0.1.4/tests/
--rw-r--r--   0 cyrildever   (501) staff       (20)      291 2022-02-18 12:53:08.000000 py-utls-0.1.4/tests/test_flatten.py
--rw-r--r--   0 cyrildever   (501) staff       (20)      380 2022-04-04 09:55:49.000000 py-utls-0.1.4/tests/test_hex.py
+drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-05-26 08:54:48.914570 py-utls-0.1.5/
+-rw-r--r--   0 cyrildever   (501) staff       (20)     1068 2022-02-18 10:33:22.000000 py-utls-0.1.5/LICENSE
+-rw-r--r--   0 cyrildever   (501) staff       (20)       19 2022-02-18 13:13:47.000000 py-utls-0.1.5/MANIFEST.in
+-rw-r--r--   0 cyrildever   (501) staff       (20)     2158 2023-05-26 08:54:48.914076 py-utls-0.1.5/PKG-INFO
+-rw-r--r--   0 cyrildever   (501) staff       (20)     1654 2023-05-26 08:52:00.000000 py-utls-0.1.5/README.md
+-rw-r--r--   0 cyrildever   (501) staff       (20)      103 2022-02-18 12:53:08.000000 py-utls-0.1.5/pyproject.toml
+-rw-r--r--   0 cyrildever   (501) staff       (20)       38 2023-05-26 08:54:48.914662 py-utls-0.1.5/setup.cfg
+-rw-r--r--   0 cyrildever   (501) staff       (20)      900 2023-05-26 08:45:28.000000 py-utls-0.1.5/setup.py
+drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-05-26 08:54:48.908375 py-utls-0.1.5/src/
+drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-05-26 08:54:48.911261 py-utls-0.1.5/src/py_utls.egg-info/
+-rw-r--r--   0 cyrildever   (501) staff       (20)     2158 2023-05-26 08:54:48.000000 py-utls-0.1.5/src/py_utls.egg-info/PKG-INFO
+-rw-r--r--   0 cyrildever   (501) staff       (20)      290 2023-05-26 08:54:48.000000 py-utls-0.1.5/src/py_utls.egg-info/SOURCES.txt
+-rw-r--r--   0 cyrildever   (501) staff       (20)        1 2023-05-26 08:54:48.000000 py-utls-0.1.5/src/py_utls.egg-info/dependency_links.txt
+-rw-r--r--   0 cyrildever   (501) staff       (20)        7 2023-05-26 08:54:48.000000 py-utls-0.1.5/src/py_utls.egg-info/top_level.txt
+drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-05-26 08:54:48.912371 py-utls-0.1.5/src/pyutls/
+-rw-r--r--   0 cyrildever   (501) staff       (20)        0 2022-02-18 12:53:08.000000 py-utls-0.1.5/src/pyutls/__init__.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)      414 2022-11-28 14:20:58.000000 py-utls-0.1.5/src/pyutls/hex.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)      251 2023-05-26 08:50:51.000000 py-utls-0.1.5/src/pyutls/list.py
+drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-05-26 08:54:48.913501 py-utls-0.1.5/tests/
+-rw-r--r--   0 cyrildever   (501) staff       (20)      380 2022-04-04 09:55:49.000000 py-utls-0.1.5/tests/test_hex.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)      758 2023-05-26 08:52:37.000000 py-utls-0.1.5/tests/test_list.py
```

### Comparing `py-utls-0.1.4/LICENSE` & `py-utls-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py-utls-0.1.4/PKG-INFO` & `py-utls-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: py-utls
-Version: 0.1.4
+Version: 0.1.5
 Summary: Utilities for Python
 Home-page: https://github.com/cyrildever/py-utls
 Author: Cyril Dever
 Project-URL: Bug Tracker, https://github.com/cyrildever/py-utls/issues
-Keywords: python,utils,flatten,hexadecimal
+Keywords: python,utils,chunks,flatten,hexadecimal
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -34,28 +34,31 @@
 ```
 
 This repository contains the following modules:
 * `hex`:
   - `from_hex`: builds the byte array from a string;
   - `to_hex`: creates the hexadecimal representation of a byte array;
 * `list`:
+  - `chunk`: split a list into chunks of a maximum size;
   - `flatten`: transforms a list of list of items to a list of items.
 
 
 ```python
 from pyutls.hex import from_hex, to_hex
-from pyutls.list import flatten
+from pyutls.list import chunk, flatten
 
 # Hex utilities
 barray = from_hex('1234abcd')
 hex_string = to_hex(barray)
-assert(hex_string == '1234abcd')
+assertEqual(hex_string == '1234abcd')
 
 # Flatten a list of list
-flat_list = flatten(list1, list2)
+chunks = chunk(some_list, size)
+flat_list = flatten(chunks)
+assertListEqual(flat_list == some_list)
 ```
 
 
 ### Tests
 
 ```console
 $ python3 -m unittest discover
```

### Comparing `py-utls-0.1.4/README.md` & `py-utls-0.1.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -19,28 +19,31 @@
 ```
 
 This repository contains the following modules:
 * `hex`:
   - `from_hex`: builds the byte array from a string;
   - `to_hex`: creates the hexadecimal representation of a byte array;
 * `list`:
+  - `chunk`: split a list into chunks of a maximum size;
   - `flatten`: transforms a list of list of items to a list of items.
 
 
 ```python
 from pyutls.hex import from_hex, to_hex
-from pyutls.list import flatten
+from pyutls.list import chunk, flatten
 
 # Hex utilities
 barray = from_hex('1234abcd')
 hex_string = to_hex(barray)
-assert(hex_string == '1234abcd')
+assertEqual(hex_string == '1234abcd')
 
 # Flatten a list of list
-flat_list = flatten(list1, list2)
+chunks = chunk(some_list, size)
+flat_list = flatten(chunks)
+assertListEqual(flat_list == some_list)
 ```
 
 
 ### Tests
 
 ```console
 $ python3 -m unittest discover
```

### Comparing `py-utls-0.1.4/setup.py` & `py-utls-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py-utls",
-    version="0.1.4",
+    version="0.1.5",
     author="Cyril Dever",
     author_mail="cdever@pep-s.com",
     description="Utilities for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cyrildever/py-utls",
     project_urls={
@@ -19,14 +19,15 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     keywords=[
         "python",
         "utils",
+        "chunks",
         "flatten",
         "hexadecimal",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
 )
```

### Comparing `py-utls-0.1.4/src/py_utls.egg-info/PKG-INFO` & `py-utls-0.1.5/src/py_utls.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: py-utls
-Version: 0.1.4
+Version: 0.1.5
 Summary: Utilities for Python
 Home-page: https://github.com/cyrildever/py-utls
 Author: Cyril Dever
 Project-URL: Bug Tracker, https://github.com/cyrildever/py-utls/issues
-Keywords: python,utils,flatten,hexadecimal
+Keywords: python,utils,chunks,flatten,hexadecimal
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -34,28 +34,31 @@
 ```
 
 This repository contains the following modules:
 * `hex`:
   - `from_hex`: builds the byte array from a string;
   - `to_hex`: creates the hexadecimal representation of a byte array;
 * `list`:
+  - `chunk`: split a list into chunks of a maximum size;
   - `flatten`: transforms a list of list of items to a list of items.
 
 
 ```python
 from pyutls.hex import from_hex, to_hex
-from pyutls.list import flatten
+from pyutls.list import chunk, flatten
 
 # Hex utilities
 barray = from_hex('1234abcd')
 hex_string = to_hex(barray)
-assert(hex_string == '1234abcd')
+assertEqual(hex_string == '1234abcd')
 
 # Flatten a list of list
-flat_list = flatten(list1, list2)
+chunks = chunk(some_list, size)
+flat_list = flatten(chunks)
+assertListEqual(flat_list == some_list)
 ```
 
 
 ### Tests
 
 ```console
 $ python3 -m unittest discover
```

