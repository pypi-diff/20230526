# Comparing `tmp/algorithmadts-0.2.2.tar.gz` & `tmp/algorithmadts-0.3.3.tar.gz`

## Comparing `algorithmadts-0.2.2.tar` & `algorithmadts-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/.DS_Store
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/.vscode/settings.json
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/src/AlgorithmADTs/.DS_Store
--rw-r--r--   0        0        0    12364 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/src/AlgorithmADTs/AbstractDataTypes.py
--rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/src/AlgorithmADTs/GraphAlgorithms.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/src/AlgorithmADTs/__init__.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/tests/experimenting.ipynb
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/tests/test_GraphAlgorithms.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/LICENSE
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/README.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 algorithmadts-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/.DS_Store
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/.vscode/settings.json
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/src/AlgorithmADTs/.DS_Store
+-rw-r--r--   0        0        0    12365 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/src/AlgorithmADTs/AbstractDataTypes.py
+-rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/src/AlgorithmADTs/GraphAlgorithms.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/src/AlgorithmADTs/__init__.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/tests/experimenting.ipynb
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/tests/test_GraphAlgorithms.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/README.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 algorithmadts-0.3.3/PKG-INFO
```

### Comparing `algorithmadts-0.2.2/.DS_Store` & `algorithmadts-0.3.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.2.2/src/.DS_Store` & `algorithmadts-0.3.3/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.2.2/src/AlgorithmADTs/.DS_Store` & `algorithmadts-0.3.3/src/AlgorithmADTs/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.2.2/src/AlgorithmADTs/AbstractDataTypes.py` & `algorithmadts-0.3.3/src/AlgorithmADTs/AbstractDataTypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,15 @@
 
     @property
     def keys(self):
         return self._keys
 
     @property
     def values(self):
-        return self.values
+        return self._values
 
     def is_empty(self):
         return len(self._keys) == 0
 
     def get(self, key_element: Any):
         for key, value in zip(self._keys, self._values):
             if key == key_element:
```

### Comparing `algorithmadts-0.2.2/src/AlgorithmADTs/GraphAlgorithms.py` & `algorithmadts-0.3.3/src/AlgorithmADTs/GraphAlgorithms.py`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.2.2/src/AlgorithmADTs/__init__.py` & `algorithmadts-0.3.3/src/AlgorithmADTs/__init__.py`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.2.2/tests/experimenting.ipynb` & `algorithmadts-0.3.3/tests/experimenting.ipynb`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.2.2/tests/test_GraphAlgorithms.py` & `algorithmadts-0.3.3/tests/test_GraphAlgorithms.py`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.2.2/LICENSE` & `algorithmadts-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.2.2/README.md` & `algorithmadts-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -102,10 +102,11 @@
 - The Bellman-Ford algorithm which extends the functionality of Dijkstra's algorithm to allow for negative weights
 - The two variants of the Floyd-Warshall algorithm to calculate shortest path between all nodes and transitive closure of an unweighted graph
 - The PageRank algorithm for determining the relative importance of nodes in an unweighted graph
 
 ## Version things 
 To implement:
 - ALLOW `List([1,3,34])` rather than having to stupidly define every value separately.
+- Allow default value for Arrays
 - Optional hashing for graphs?
 - Search methods like DPS BFS
 - LEn of dict
```

### Comparing `algorithmadts-0.2.2/PKG-INFO` & `algorithmadts-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgorithmADTs
-Version: 0.2.2
+Version: 0.3.3
 Summary: General purpose Abstract Data Types for Algorithmics
 Author-email: Finlay <finlay3.141@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -114,10 +114,11 @@
 - The Bellman-Ford algorithm which extends the functionality of Dijkstra's algorithm to allow for negative weights
 - The two variants of the Floyd-Warshall algorithm to calculate shortest path between all nodes and transitive closure of an unweighted graph
 - The PageRank algorithm for determining the relative importance of nodes in an unweighted graph
 
 ## Version things 
 To implement:
 - ALLOW `List([1,3,34])` rather than having to stupidly define every value separately.
+- Allow default value for Arrays
 - Optional hashing for graphs?
 - Search methods like DPS BFS
 - LEn of dict
```

