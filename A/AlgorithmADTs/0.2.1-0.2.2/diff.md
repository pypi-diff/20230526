# Comparing `tmp/algorithmadts-0.2.1.tar.gz` & `tmp/algorithmadts-0.2.2.tar.gz`

## Comparing `algorithmadts-0.2.1.tar` & `algorithmadts-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/.DS_Store
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/.vscode/settings.json
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/src/AlgorithmADTs/.DS_Store
--rw-r--r--   0        0        0    12193 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/src/AlgorithmADTs/AbstractDataTypes.py
--rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/src/AlgorithmADTs/GraphAlgorithms.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/src/AlgorithmADTs/__init__.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/tests/experimenting.ipynb
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/tests/test_GraphAlgorithms.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/LICENSE
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/README.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 algorithmadts-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/.DS_Store
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/src/AlgorithmADTs/.DS_Store
+-rw-r--r--   0        0        0    12364 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/src/AlgorithmADTs/AbstractDataTypes.py
+-rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/src/AlgorithmADTs/GraphAlgorithms.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/src/AlgorithmADTs/__init__.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/tests/experimenting.ipynb
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/tests/test_GraphAlgorithms.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/README.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/PKG-INFO
```

### Comparing `algorithmadts-0.2.1/.DS_Store` & `algorithmadts-0.2.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.2.1/src/.DS_Store` & `algorithmadts-0.2.2/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.2.1/src/AlgorithmADTs/.DS_Store` & `algorithmadts-0.2.2/src/AlgorithmADTs/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.2.1/src/AlgorithmADTs/AbstractDataTypes.py` & `algorithmadts-0.2.2/src/AlgorithmADTs/AbstractDataTypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,16 +310,24 @@
 
 class Dictionary:
     @staticmethod
     def create():
         return Dictionary()
 
     def __init__(self):
-        self._keys: list[Any] = []
-        self._values: list[Any] = []
+        self._keys = List()
+        self._values = List()
+
+    @property
+    def keys(self):
+        return self._keys
+
+    @property
+    def values(self):
+        return self.values
 
     def is_empty(self):
         return len(self._keys) == 0
 
     def get(self, key_element: Any):
         for key, value in zip(self._keys, self._values):
             if key == key_element:
@@ -339,16 +347,16 @@
         self._keys.append(key_element)
         self._values.append(value_element)
         return self
 
     def remove(self, key_element: Any):
         for i, key in enumerate(self._keys):
             if key == key_element:
-                self._values.pop(i)
-                self._keys.pop(i)
+                self._values.delete(i)
+                self._keys.delete(i)
                 return self
 
     def has_key(self, key_element: Any):
         return key_element in self._keys
 
     def __getitem__(self, key: Any):
         return self.get(key)
@@ -368,14 +376,17 @@
         return f"keys: {str(self._keys)}"
 
     def __eq__(self, other):
         if isinstance(other, Dictionary):
             return self._keys == other._keys and self._values == other._values
         return False
 
+    def __len__(self):
+        return len(self.keys)
+
 
 class Graph:
     @staticmethod
     def create(*, directed=False):
         return Graph(directed=directed)
 
     def __init__(self, *, directed=False):
```

### Comparing `algorithmadts-0.2.1/src/AlgorithmADTs/GraphAlgorithms.py` & `algorithmadts-0.2.2/src/AlgorithmADTs/GraphAlgorithms.py`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.2.1/src/AlgorithmADTs/__init__.py` & `algorithmadts-0.2.2/src/AlgorithmADTs/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "PageRank",
 ]
 
 from importlib.metadata import version
 __version__ = version("AlgorithmADTs")
 
 def __check_version__():
-    print("Checking version...\t")
+    print("Checking version...", end='\t')
     import requests 
     import xml.etree.ElementTree as ET
     page = requests.get("https://pypi.org/rss/project/algorithmadts/releases.xml")
 
     if page.status_code != 200:
         print("Connection error")
         return ValueError()
@@ -56,13 +56,15 @@
     channel = element_tree.find('channel')
     try:
         item = channel.find('item') #type: ignore
         version = item.find('title').text # type: ignore
 
         if version == __version__:
             print("All up to date!")
+            return True
         else:
-            print(f"There is a new version of AlgorithmADTs available. Try updating to version {version}")
+            print(f"There is a new version of AlgorithmADTs available! Try updating to version {version}")
+            return False
 
     except:
         print("Parsing error")
         return ValueError()
```

### Comparing `algorithmadts-0.2.1/tests/experimenting.ipynb` & `algorithmadts-0.2.2/tests/experimenting.ipynb`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.2.1/tests/test_GraphAlgorithms.py` & `algorithmadts-0.2.2/tests/test_GraphAlgorithms.py`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.2.1/LICENSE` & `algorithmadts-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.2.1/README.md` & `algorithmadts-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Algorithm Abstract Data Types
 Finlay's package for Abstract Data Types written for Algorithmics class
 
 ## Installation
 Run the following command in your terminal: 
-`pip install AlgorithmADTs`
+`pip install AlgorithmADTs --force-reinstall`
 
 AlgorithmADTs can now be imported into your python scripts! 
 
 I recommend `from AlgorithmADTs import *` to include all functionality, but you can also import from `AlgorithmADTs.AbstractDataTypes` or `AlgorithmADTs.GraphAlgorithms` 
 
 ## ADTS:
 ```
@@ -89,20 +89,23 @@
 - `__getitem__` and `__setitem__` for classes with a 'get' and 'set' function.
     This allows you to call `instance[key]` and `instance[key] = value`.
 - `__iter__` for Array and List, which operates as expected. Dictionary iter returns an iterable of keys.
     This enables iterating through a class like `for elem in instance`
 - `__str__` and `__repr__` are defined for all classes except graphs and allow for classes to be easily viewed through printing
     Note that only the head element is visible for a stack or queue, so it is the only information that can be returned by these methods
 - Numerical magic methods (e.g. `__add__`) are defined for matrices
+- `__len__` is defined for Array, List and Dictionary 
 
 ## Graph Algorithms
 Currently, the following graph algorithms are defined:
 - Prim's algorithm for computing the Minimal Spanning Tree of a weighted, undirected graph
 - Dijkstra's algorithm for finding the single source shortest path in a weighted graph 
 - The Bellman-Ford algorithm which extends the functionality of Dijkstra's algorithm to allow for negative weights
 - The two variants of the Floyd-Warshall algorithm to calculate shortest path between all nodes and transitive closure of an unweighted graph
 - The PageRank algorithm for determining the relative importance of nodes in an unweighted graph
 
 ## Version things 
 To implement:
+- ALLOW `List([1,3,34])` rather than having to stupidly define every value separately.
 - Optional hashing for graphs?
-- Search methods like DPS BFS
+- Search methods like DPS BFS
+- LEn of dict
```

### Comparing `algorithmadts-0.2.1/PKG-INFO` & `algorithmadts-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: AlgorithmADTs
-Version: 0.2.1
+Version: 0.2.2
 Summary: General purpose Abstract Data Types for Algorithmics
 Author-email: Finlay <finlay3.141@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Algorithm Abstract Data Types
 Finlay's package for Abstract Data Types written for Algorithmics class
 
 ## Installation
 Run the following command in your terminal: 
-`pip install AlgorithmADTs`
+`pip install AlgorithmADTs --force-reinstall`
 
 AlgorithmADTs can now be imported into your python scripts! 
 
 I recommend `from AlgorithmADTs import *` to include all functionality, but you can also import from `AlgorithmADTs.AbstractDataTypes` or `AlgorithmADTs.GraphAlgorithms` 
 
 ## ADTS:
 ```
@@ -101,20 +101,23 @@
 - `__getitem__` and `__setitem__` for classes with a 'get' and 'set' function.
     This allows you to call `instance[key]` and `instance[key] = value`.
 - `__iter__` for Array and List, which operates as expected. Dictionary iter returns an iterable of keys.
     This enables iterating through a class like `for elem in instance`
 - `__str__` and `__repr__` are defined for all classes except graphs and allow for classes to be easily viewed through printing
     Note that only the head element is visible for a stack or queue, so it is the only information that can be returned by these methods
 - Numerical magic methods (e.g. `__add__`) are defined for matrices
+- `__len__` is defined for Array, List and Dictionary 
 
 ## Graph Algorithms
 Currently, the following graph algorithms are defined:
 - Prim's algorithm for computing the Minimal Spanning Tree of a weighted, undirected graph
 - Dijkstra's algorithm for finding the single source shortest path in a weighted graph 
 - The Bellman-Ford algorithm which extends the functionality of Dijkstra's algorithm to allow for negative weights
 - The two variants of the Floyd-Warshall algorithm to calculate shortest path between all nodes and transitive closure of an unweighted graph
 - The PageRank algorithm for determining the relative importance of nodes in an unweighted graph
 
 ## Version things 
 To implement:
+- ALLOW `List([1,3,34])` rather than having to stupidly define every value separately.
 - Optional hashing for graphs?
-- Search methods like DPS BFS
+- Search methods like DPS BFS
+- LEn of dict
```

