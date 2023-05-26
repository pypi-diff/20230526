# Comparing `tmp/wayfarer-0.9.3.tar.gz` & `tmp/wayfarer-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wayfarer-0.9.3.tar", last modified: Wed May 24 08:07:28 2023, max compression
+gzip compressed data, was "wayfarer-0.9.4.tar", last modified: Fri May 26 13:36:04 2023, max compression
```

## Comparing `wayfarer-0.9.3.tar` & `wayfarer-0.9.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:28.487214 wayfarer-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-24 08:06:03.000000 wayfarer-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-24 08:07:28.487214 wayfarer-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-24 08:06:03.000000 wayfarer-0.9.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 08:07:28.487214 wayfarer-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-24 08:06:03.000000 wayfarer-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:28.483214 wayfarer-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-05-24 08:06:03.000000 wayfarer-0.9.3/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-05-24 08:06:03.000000 wayfarer-0.9.3/tests/test_linearref.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-24 08:06:03.000000 wayfarer-0.9.3/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-24 08:06:03.000000 wayfarer-0.9.3/tests/test_loops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-24 08:06:03.000000 wayfarer-0.9.3/tests/test_osmnx_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-24 08:06:03.000000 wayfarer-0.9.3/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-05-24 08:06:03.000000 wayfarer-0.9.3/tests/test_routing_ordered_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-05-24 08:06:03.000000 wayfarer-0.9.3/tests/test_splitting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:28.487214 wayfarer-0.9.3/wayfarer/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-24 08:06:03.000000 wayfarer-0.9.3/wayfarer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-05-24 08:06:03.000000 wayfarer-0.9.3/wayfarer/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-24 08:06:03.000000 wayfarer-0.9.3/wayfarer/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-05-24 08:06:03.000000 wayfarer-0.9.3/wayfarer/linearref.py
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-05-24 08:06:03.000000 wayfarer-0.9.3/wayfarer/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-24 08:06:03.000000 wayfarer-0.9.3/wayfarer/loops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:03.000000 wayfarer-0.9.3/wayfarer/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-24 08:06:03.000000 wayfarer-0.9.3/wayfarer/osmnx_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:03.000000 wayfarer-0.9.3/wayfarer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-05-24 08:06:03.000000 wayfarer-0.9.3/wayfarer/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-05-24 08:06:03.000000 wayfarer-0.9.3/wayfarer/splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-24 08:06:03.000000 wayfarer-0.9.3/wayfarer/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:28.487214 wayfarer-0.9.3/wayfarer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-24 08:07:28.000000 wayfarer-0.9.3/wayfarer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-24 08:07:28.000000 wayfarer-0.9.3/wayfarer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 08:07:28.000000 wayfarer-0.9.3/wayfarer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 08:06:30.000000 wayfarer-0.9.3/wayfarer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 08:07:28.000000 wayfarer-0.9.3/wayfarer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 08:07:28.000000 wayfarer-0.9.3/wayfarer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:36:04.100480 wayfarer-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-26 13:34:51.000000 wayfarer-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-26 13:36:04.100480 wayfarer-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-26 13:34:51.000000 wayfarer-0.9.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 13:36:04.100480 wayfarer-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-26 13:34:52.000000 wayfarer-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:36:04.092480 wayfarer-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-05-26 13:34:52.000000 wayfarer-0.9.4/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-05-26 13:34:52.000000 wayfarer-0.9.4/tests/test_linearref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-26 13:34:52.000000 wayfarer-0.9.4/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-26 13:34:52.000000 wayfarer-0.9.4/tests/test_loops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-26 13:34:52.000000 wayfarer-0.9.4/tests/test_osmnx_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-26 13:34:52.000000 wayfarer-0.9.4/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-05-26 13:34:52.000000 wayfarer-0.9.4/tests/test_routing_ordered_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-05-26 13:34:52.000000 wayfarer-0.9.4/tests/test_splitting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:36:04.096480 wayfarer-0.9.4/wayfarer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-26 13:34:52.000000 wayfarer-0.9.4/wayfarer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18851 2023-05-26 13:34:52.000000 wayfarer-0.9.4/wayfarer/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-26 13:34:52.000000 wayfarer-0.9.4/wayfarer/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-05-26 13:34:52.000000 wayfarer-0.9.4/wayfarer/linearref.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-05-26 13:34:52.000000 wayfarer-0.9.4/wayfarer/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-26 13:34:52.000000 wayfarer-0.9.4/wayfarer/loops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:52.000000 wayfarer-0.9.4/wayfarer/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-26 13:34:52.000000 wayfarer-0.9.4/wayfarer/osmnx_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:52.000000 wayfarer-0.9.4/wayfarer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-05-26 13:34:52.000000 wayfarer-0.9.4/wayfarer/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-05-26 13:34:52.000000 wayfarer-0.9.4/wayfarer/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-26 13:34:52.000000 wayfarer-0.9.4/wayfarer/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:36:04.100480 wayfarer-0.9.4/wayfarer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-26 13:36:04.000000 wayfarer-0.9.4/wayfarer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-26 13:36:04.000000 wayfarer-0.9.4/wayfarer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:36:04.000000 wayfarer-0.9.4/wayfarer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:35:10.000000 wayfarer-0.9.4/wayfarer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 13:36:04.000000 wayfarer-0.9.4/wayfarer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 13:36:04.000000 wayfarer-0.9.4/wayfarer.egg-info/top_level.txt
```

### Comparing `wayfarer-0.9.3/LICENSE` & `wayfarer-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/PKG-INFO` & `wayfarer-0.9.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wayfarer
-Version: 0.9.3
+Version: 0.9.4
 Summary: A library to add spatial functions to networkx
 Home-page: https://github.com/compassinformatics/wayfarer/
 Author: Seth Girvin
 Author-email: sgirvin@compass.ie
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wayfarer-0.9.3/README.rst` & `wayfarer-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/setup.py` & `wayfarer-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/tests/test_functions.py` & `wayfarer-0.9.4/tests/test_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -410,19 +410,19 @@
 def test_get_path_length():
     edges = [Edge(0, 1, "A", {"LEN_": 5}), Edge(1, 2, "B", {"LEN_": 5})]
     assert functions.get_path_length(edges) == 10
 
 
 def test_has_overlaps():
     edges = [
-        Edge(0, 1, "A", {"EDGE_ID": 1}),
-        Edge(1, 2, "B", {"EDGE_ID": 2}),
-        Edge(2, 3, "C", {"EDGE_ID": 3}),
-        Edge(2, 3, "C", {"EDGE_ID": 2}),
-        Edge(2, 3, "C", {"EDGE_ID": 4}),
+        Edge(0, 1, "A", {"EDGE_ID": 1, "OFFSET": 0, "LEN_": 10}),
+        Edge(1, 2, "B", {"EDGE_ID": 2, "OFFSET": 0, "LEN_": 10}),
+        Edge(2, 3, "C", {"EDGE_ID": 3, "OFFSET": 0, "LEN_": 10}),
+        Edge(2, 3, "C", {"EDGE_ID": 2, "OFFSET": 0, "LEN_": 10}),
+        Edge(2, 3, "C", {"EDGE_ID": 4, "OFFSET": 0, "LEN_": 10}),
     ]
     assert functions.has_overlaps(edges) is True
 
 
 def test_has_no_overlaps():
     edges = [
         Edge(0, 1, "A", {"EDGE_ID": 1}),
@@ -440,35 +440,48 @@
         Edge(2, 3, "C", {"EDGE_ID": 3}),
         Edge(0, 1, "D", {"EDGE_ID": 1}),
     ]
 
     assert functions.has_overlaps(edges) is False
 
 
+def test_has_no_overlaps_loop_with_split():
+    edges = [
+        Edge(0, 1, "A", {"EDGE_ID": 1, "OFFSET": 5, "LEN_": 10}),
+        Edge(1, 2, "B", {"EDGE_ID": 2, "OFFSET": 0, "LEN_": 10}),
+        Edge(1, 2, "B", {"EDGE_ID": 2, "OFFSET": 10, "LEN_": 10}),
+        Edge(2, 3, "C", {"EDGE_ID": 3, "OFFSET": 0, "LEN_": 10}),
+        Edge(3, 0, "C", {"EDGE_ID": 4, "OFFSET": 0, "LEN_": 5}),
+    ]
+    assert functions.has_overlaps(edges) is False
+
+
 def test_doctest():
     import doctest
 
     print(doctest.testmod(functions))
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.DEBUG)
     # test_get_edges_from_nodes()
     # test_edges_to_graph()
     # test_get_edges_from_nodes()
     # test_edges_to_graph()
-    test_get_shortest_edge()
-    test_get_shortest_edge_identical()
-    test_get_shortest_edge_mixed_keys()
+    # test_get_shortest_edge()
+    # test_get_shortest_edge_identical()
+    # test_get_shortest_edge_mixed_keys()
     # test_get_unique_ordered_list()
     # test_get_edges_from_node_pair()
     # test_to_edge()
     # test_to_edge_no_attributes()
     # test_edges_to_graph_no_keys()
     # test_get_edge_by_key_missing()
     # test_get_all_paths_from_nodes_with_direction()
     # test_get_path_length()
     # test_doctest()
     # test_get_edges_from_nodes_non_unique()
     # test_has_no_overlaps()
     # test_has_no_overlaps_loop()
+    # test_has_overlaps()
+    test_has_no_overlaps_loop_with_split()
     print("Done!")
```

### Comparing `wayfarer-0.9.3/tests/test_linearref.py` & `wayfarer-0.9.4/tests/test_linearref.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/tests/test_loader.py` & `wayfarer-0.9.4/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/tests/test_loops.py` & `wayfarer-0.9.4/tests/test_loops.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/tests/test_osmnx_compat.py` & `wayfarer-0.9.4/tests/test_osmnx_compat.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/tests/test_routing.py` & `wayfarer-0.9.4/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/tests/test_routing_ordered_path.py` & `wayfarer-0.9.4/tests/test_routing_ordered_path.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/tests/test_splitting.py` & `wayfarer-0.9.4/tests/test_splitting.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/wayfarer/__init__.py` & `wayfarer-0.9.4/wayfarer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import NamedTuple
 
 
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 
 LENGTH_FIELD = "LEN_"
 EDGE_ID_FIELD = "EDGE_ID"
 OFFSET_FIELD = "OFFSET"
 
 NODEID_FROM_FIELD = "NODEID_FROM"
 NODEID_TO_FIELD = "NODEID_TO"
```

### Comparing `wayfarer-0.9.3/wayfarer/functions.py` & `wayfarer-0.9.4/wayfarer/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from wayfarer import (
     EDGE_ID_FIELD,
     LENGTH_FIELD,
     NODEID_FROM_FIELD,
     NODEID_TO_FIELD,
     WITH_DIRECTION_FIELD,
+    OFFSET_FIELD,
     Edge,
 )
 
 
 log = logging.getLogger("wayfarer")
 
 
@@ -608,31 +609,37 @@
     multiconnected_nodes = [n for n in out_degree if out_degree[n] >= connections]
     return multiconnected_nodes
 
 
 def has_overlaps(edges: list[Edge]) -> bool:
     """
     Checks if the provided list of edges has overlaps
-    where the same edge id is repeated in the sequence.
-    Edge ids can be adjacent e.g. 1,2,2,3 returns False
-    and the same edge id can be found at the start and end of the sequence
-    e.g. 1,2,3,1 returns False
+    If an edge is split but the measures don't overlap then this will return False
+    The same edge id can be found at the start and end of the sequence if there is
+    no overlap of measures
 
-    >>> edges = [Edge(0, 1, "A", {"EDGE_ID": 1}), Edge(1, 2, "B", {"EDGE_ID": 2})]
+    >>> edges = [Edge(0, 1, "A", {"EDGE_ID": 1, "OFFSET": 0, "LEN_": 10}), \
+Edge(1, 2, "B", {"EDGE_ID": 2, "OFFSET": 0, "LEN_": 10})]
     >>> has_overlaps(edges)
     False
     """
     # get the edge id from the attributes rather than the edge key in case
     # there are split edges which will have modified keys
 
-    edge_ids = [e.attributes[EDGE_ID_FIELD] for e in edges]
+    sorted_edges = sorted(edges, key=lambda e: e.attributes[EDGE_ID_FIELD])
+    grouped_edges = itertools.groupby(
+        sorted_edges, key=lambda e: e.attributes[EDGE_ID_FIELD]
+    )
 
-    grouped_edge_ids = [k for k, g in itertools.groupby(edge_ids)]
-    unique_edge_count = len(set(edge_ids))
+    for _, edge_group in grouped_edges:
+        for edge1, edge2 in itertools.combinations(edge_group, 2):
 
-    if edge_ids[0] == edge_ids[-1]:
-        unique_edge_count += 1  # allow looping back onto start edge
+            from_m1 = edge1.attributes.get(OFFSET_FIELD, 0)
+            to_m1 = from_m1 + edge1.attributes.get(LENGTH_FIELD, 0)
 
-    if len(grouped_edge_ids) > unique_edge_count:
-        return True
-    else:
-        return False
+            from_m2 = edge2.attributes.get(OFFSET_FIELD, 0)
+            to_m2 = from_m2 + edge2.attributes.get(LENGTH_FIELD, 0)
+
+            if max(from_m1, from_m2) < min(to_m1, to_m2):
+                return True
+
+    return False
```

### Comparing `wayfarer-0.9.3/wayfarer/io.py` & `wayfarer-0.9.4/wayfarer/io.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/wayfarer/linearref.py` & `wayfarer-0.9.4/wayfarer/linearref.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/wayfarer/loader.py` & `wayfarer-0.9.4/wayfarer/loader.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/wayfarer/loops.py` & `wayfarer-0.9.4/wayfarer/loops.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/wayfarer/osmnx_compat.py` & `wayfarer-0.9.4/wayfarer/osmnx_compat.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/wayfarer/routing.py` & `wayfarer-0.9.4/wayfarer/routing.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/wayfarer/splitter.py` & `wayfarer-0.9.4/wayfarer/splitter.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/wayfarer/validator.py` & `wayfarer-0.9.4/wayfarer/validator.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.3/wayfarer.egg-info/PKG-INFO` & `wayfarer-0.9.4/wayfarer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wayfarer
-Version: 0.9.3
+Version: 0.9.4
 Summary: A library to add spatial functions to networkx
 Home-page: https://github.com/compassinformatics/wayfarer/
 Author: Seth Girvin
 Author-email: sgirvin@compass.ie
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wayfarer-0.9.3/wayfarer.egg-info/SOURCES.txt` & `wayfarer-0.9.4/wayfarer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

