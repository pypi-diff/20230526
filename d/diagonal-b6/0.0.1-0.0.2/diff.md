# Comparing `tmp/diagonal_b6-0.0.1.tar.gz` & `tmp/diagonal_b6-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diagonal_b6-0.0.1.tar", last modified: Sat Apr 22 07:37:35 2023, max compression
+gzip compressed data, was "diagonal_b6-0.0.2.tar", last modified: Fri May 26 15:49:04 2023, max compression
```

## Comparing `diagonal_b6-0.0.1.tar` & `diagonal_b6-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-04-22 07:37:35.922431 diagonal_b6-0.0.1/
--rw-r--r--   0 andrew     (501) staff       (20)      647 2023-04-22 07:37:35.921957 diagonal_b6-0.0.1/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)       71 2023-04-21 08:22:48.000000 diagonal_b6-0.0.1/README.md
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-04-22 07:37:35.918110 diagonal_b6-0.0.1/diagonal_b6/
--rw-r--r--   0 andrew     (501) staff       (20)      171 2023-04-20 09:50:03.000000 diagonal_b6-0.0.1/diagonal_b6/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)    53040 2023-04-21 13:55:49.000000 diagonal_b6-0.0.1/diagonal_b6/api_generated.py
--rw-r--r--   0 andrew     (501) staff       (20)     8336 2023-04-21 13:55:49.000000 diagonal_b6-0.0.1/diagonal_b6/api_pb2.py
--rw-r--r--   0 andrew     (501) staff       (20)     2355 2023-04-21 13:55:49.000000 diagonal_b6-0.0.1/diagonal_b6/api_pb2_grpc.py
--rwxr-xr-x   0 andrew     (501) staff       (20)    26093 2023-04-21 14:01:38.000000 diagonal_b6-0.0.1/diagonal_b6/b6_test.py
--rw-r--r--   0 andrew     (501) staff       (20)      909 2023-04-20 09:50:03.000000 diagonal_b6-0.0.1/diagonal_b6/connect.py
--rw-r--r--   0 andrew     (501) staff       (20)     4181 2023-04-20 09:50:03.000000 diagonal_b6-0.0.1/diagonal_b6/expression.py
--rw-r--r--   0 andrew     (501) staff       (20)     6691 2023-04-20 09:50:03.000000 diagonal_b6-0.0.1/diagonal_b6/features.py
--rw-r--r--   0 andrew     (501) staff       (20)     3894 2023-04-21 13:55:49.000000 diagonal_b6-0.0.1/diagonal_b6/features_pb2.py
--rw-r--r--   0 andrew     (501) staff       (20)      159 2023-04-21 13:55:49.000000 diagonal_b6-0.0.1/diagonal_b6/features_pb2_grpc.py
--rwxr-xr-x   0 andrew     (501) staff       (20)     8375 2023-04-20 09:50:03.000000 diagonal_b6-0.0.1/diagonal_b6/generate_api.py
--rw-r--r--   0 andrew     (501) staff       (20)     3791 2023-04-20 09:50:03.000000 diagonal_b6-0.0.1/diagonal_b6/geometry.py
--rw-r--r--   0 andrew     (501) staff       (20)     1782 2023-04-21 13:55:49.000000 diagonal_b6-0.0.1/diagonal_b6/geometry_pb2.py
--rw-r--r--   0 andrew     (501) staff       (20)      159 2023-04-21 13:55:49.000000 diagonal_b6-0.0.1/diagonal_b6/geometry_pb2_grpc.py
--rw-r--r--   0 andrew     (501) staff       (20)     2168 2023-04-20 09:50:03.000000 diagonal_b6-0.0.1/diagonal_b6/query.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-04-22 07:37:35.921284 diagonal_b6-0.0.1/diagonal_b6.egg-info/
--rw-r--r--   0 andrew     (501) staff       (20)      647 2023-04-22 07:37:35.000000 diagonal_b6-0.0.1/diagonal_b6.egg-info/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)      593 2023-04-22 07:37:35.000000 diagonal_b6-0.0.1/diagonal_b6.egg-info/SOURCES.txt
--rw-r--r--   0 andrew     (501) staff       (20)        1 2023-04-22 07:37:35.000000 diagonal_b6-0.0.1/diagonal_b6.egg-info/dependency_links.txt
--rw-r--r--   0 andrew     (501) staff       (20)       48 2023-04-22 07:37:35.000000 diagonal_b6-0.0.1/diagonal_b6.egg-info/requires.txt
--rw-r--r--   0 andrew     (501) staff       (20)       22 2023-04-22 07:37:35.000000 diagonal_b6-0.0.1/diagonal_b6.egg-info/top_level.txt
--rw-r--r--   0 andrew     (501) staff       (20)      801 2023-04-22 07:37:27.000000 diagonal_b6-0.0.1/pyproject.toml
--rw-r--r--   0 andrew     (501) staff       (20)       38 2023-04-22 07:37:35.922567 diagonal_b6-0.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 15:49:04.846417 diagonal_b6-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-05-26 15:49:04.846417 diagonal_b6-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       71 2023-04-21 14:05:17.000000 diagonal_b6-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 15:49:04.843417 diagonal_b6-0.0.2/diagonal_b6/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-04-21 14:05:17.000000 diagonal_b6-0.0.2/diagonal_b6/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53768 2023-05-26 15:48:53.000000 diagonal_b6-0.0.2/diagonal_b6/api_generated.py
+-rw-r--r--   0 root         (0) root         (0)     8373 2023-05-26 15:48:09.000000 diagonal_b6-0.0.2/diagonal_b6/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-05-26 15:48:09.000000 diagonal_b6-0.0.2/diagonal_b6/api_pb2_grpc.py
+-rwxr-xr-x   0 root         (0) root         (0)    26093 2023-04-21 14:05:17.000000 diagonal_b6-0.0.2/diagonal_b6/b6_test.py
+-rw-r--r--   0 root         (0) root         (0)      976 2023-05-26 12:46:25.000000 diagonal_b6-0.0.2/diagonal_b6/connect.py
+-rw-r--r--   0 root         (0) root         (0)     4181 2023-04-21 14:05:17.000000 diagonal_b6-0.0.2/diagonal_b6/expression.py
+-rw-r--r--   0 root         (0) root         (0)     6684 2023-05-26 12:46:25.000000 diagonal_b6-0.0.2/diagonal_b6/features.py
+-rw-r--r--   0 root         (0) root         (0)     3894 2023-04-21 14:11:40.000000 diagonal_b6-0.0.2/diagonal_b6/features_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-04-21 14:11:40.000000 diagonal_b6-0.0.2/diagonal_b6/features_pb2_grpc.py
+-rwxr-xr-x   0 root         (0) root         (0)     8424 2023-05-26 12:46:25.000000 diagonal_b6-0.0.2/diagonal_b6/generate_api.py
+-rw-r--r--   0 root         (0) root         (0)     3791 2023-04-21 14:05:17.000000 diagonal_b6-0.0.2/diagonal_b6/geometry.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-04-21 14:11:40.000000 diagonal_b6-0.0.2/diagonal_b6/geometry_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-04-21 14:11:40.000000 diagonal_b6-0.0.2/diagonal_b6/geometry_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-04-21 14:05:17.000000 diagonal_b6-0.0.2/diagonal_b6/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 15:49:04.845417 diagonal_b6-0.0.2/diagonal_b6.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-05-26 15:49:04.000000 diagonal_b6-0.0.2/diagonal_b6.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      593 2023-05-26 15:49:04.000000 diagonal_b6-0.0.2/diagonal_b6.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 15:49:04.000000 diagonal_b6-0.0.2/diagonal_b6.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-26 15:49:04.000000 diagonal_b6-0.0.2/diagonal_b6.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-26 15:49:04.000000 diagonal_b6-0.0.2/diagonal_b6.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      803 2023-05-26 15:48:09.000000 diagonal_b6-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 15:49:04.846417 diagonal_b6-0.0.2/setup.cfg
```

### Comparing `diagonal_b6-0.0.1/PKG-INFO` & `diagonal_b6-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: diagonal_b6
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python client library for b6, Diagonal's geospatial analysis engine.
 Author-email: Diagonal Works <hello@diagonal.works>
 License: Apache License
-Project-URL: Homepage, https://diagonal.works/
+Project-URL: Homepage, https://diagonal.works/b6
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `diagonal_b6-0.0.1/diagonal_b6/api_generated.py` & `diagonal_b6-0.0.2/diagonal_b6/api_generated.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,43 +1,48 @@
+# Code generated by generate_api.py. DO NOT EDIT.
 # Client library for Diagonal's geospatial analysis engine, b6.
-# Autogenerated Fri Apr 21 14:55:49 2023
 
 from __future__ import annotations
 
 from typing import Callable
 
 import diagonal_b6.expression
 from diagonal_b6.expression import Call, Symbol, Lambda, Result
 
+VERSION = '0.0.2+modified'
+
 class CollectionTraits:
 
     def take(self, a0: IntTraits) -> CollectionResult:
         return take(self, a0)
 
-    def filter(self, a0: Callable[[AnyTraits],BoolTraits]) -> CollectionResult:
-        return filter(self, a0)
-
     def map_items(self, a0: Callable[[PairTraits],AnyTraits]) -> CollectionResult:
         return map_items(self, a0)
 
-    def count(self) -> IntTraits:
-        return count(self)
+    def count_values(self) -> CollectionResult:
+        return count_values(self)
 
-    def map(self, a0: Callable[[AnyTraits],AnyTraits]) -> CollectionResult:
-        return map(self, a0)
+    def map_parallel(self, a0: Callable[[AnyTraits],AnyTraits]) -> CollectionResult:
+        return map_parallel(self, a0)
 
     def sum_by_key(self) -> CollectionResult:
         return sum_by_key(self)
 
-    def count_values(self) -> CollectionResult:
-        return count_values(self)
+    def count(self) -> IntTraits:
+        return count(self)
+
+    def filter(self, a0: Callable[[AnyTraits],BoolTraits]) -> CollectionResult:
+        return filter(self, a0)
 
     def flattern(self) -> CollectionResult:
         return flattern(self)
 
+    def map(self, a0: Callable[[AnyTraits],AnyTraits]) -> CollectionResult:
+        return map(self, a0)
+
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class RenderableTraits:
 
     def to_geojson(self) -> GeoJSONTraits:
@@ -59,479 +64,485 @@
 
     @classmethod
     def _values(cls):
         return RenderableResult
 
 class GeometryTraits(RenderableTraits):
 
-    def tile_paths(self, a0: IntTraits) -> IntStringCollectionResult:
-        return tile_paths(self, a0)
-
-    def intersecting(self) -> QueryTraits:
-        return intersecting(self)
+    def centroid(self) -> PointTraits:
+        return centroid(self)
 
     def points(self) -> PointCollectionResult:
         return points(self)
 
-    def centroid(self) -> PointTraits:
-        return centroid(self)
+    def intersecting(self) -> QueryTraits:
+        return intersecting(self)
+
+    def tile_paths(self, a0: IntTraits) -> IntStringCollectionResult:
+        return tile_paths(self, a0)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class GeometryValuesTraits(RenderableValuesTraits):
 
-    def tile_paths(self, a0: IntTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: tile_paths(x, a0), [self._values()]))
-
-    def intersecting(self) -> CollectionTraits:
-        return self.map(Lambda(intersecting, [self._values()]))
+    def centroid(self) -> PointCollectionTraits:
+        return self.map(Lambda(centroid, [self._values()]))
 
     def points(self) -> CollectionTraits:
         return self.map(Lambda(points, [self._values()]))
 
-    def centroid(self) -> PointCollectionTraits:
-        return self.map(Lambda(centroid, [self._values()]))
+    def intersecting(self) -> CollectionTraits:
+        return self.map(Lambda(intersecting, [self._values()]))
+
+    def tile_paths(self, a0: IntTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: tile_paths(x, a0), [self._values()]))
 
 class AnyGeometryValuesResult(Result, GeometryValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return GeometryResult
 
 class IdentifiableTraits:
 
-    def get_int(self, a0: StringTraits) -> IntTraits:
-        return get_int(self, a0)
-
-    def get(self, a0: StringTraits) -> TagTraits:
-        return get(self, a0)
-
-    def remove_tag(self, a0: StringTraits) -> ChangeTraits:
-        return remove_tag(self, a0)
+    def get_string(self, a0: StringTraits) -> StringTraits:
+        return get_string(self, a0)
 
     def add_tag(self, a0: TagTraits) -> ChangeTraits:
         return add_tag(self, a0)
 
+    def get(self, a0: StringTraits) -> TagTraits:
+        return get(self, a0)
+
     def all_tags(self) -> IntTagCollectionResult:
         return all_tags(self)
 
+    def debug_tokens(self) -> IntStringCollectionResult:
+        return debug_tokens(self)
+
+    def get_int(self, a0: StringTraits) -> IntTraits:
+        return get_int(self, a0)
+
     def count_tag_value(self, a0: StringTraits) -> CollectionResult:
         return count_tag_value(self, a0)
 
-    def get_string(self, a0: StringTraits) -> StringTraits:
-        return get_string(self, a0)
-
     def get_float(self, a0: StringTraits) -> FloatTraits:
         return get_float(self, a0)
 
-    def debug_tokens(self) -> IntStringCollectionResult:
-        return debug_tokens(self)
+    def remove_tag(self, a0: StringTraits) -> ChangeTraits:
+        return remove_tag(self, a0)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class IdentifiableValuesTraits:
 
-    def get_int(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: get_int(x, a0), [self._values()]))
-
-    def get(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: get(x, a0), [self._values()]))
-
-    def remove_tag(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: remove_tag(x, a0), [self._values()]))
+    def get_string(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: get_string(x, a0), [self._values()]))
 
     def add_tag(self, a0: TagTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: add_tag(x, a0), [self._values()]))
 
+    def get(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: get(x, a0), [self._values()]))
+
     def all_tags(self) -> CollectionTraits:
         return self.map(Lambda(all_tags, [self._values()]))
 
+    def debug_tokens(self) -> CollectionTraits:
+        return self.map(Lambda(debug_tokens, [self._values()]))
+
+    def get_int(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: get_int(x, a0), [self._values()]))
+
     def count_tag_value(self, a0: StringTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: count_tag_value(x, a0), [self._values()]))
 
-    def get_string(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: get_string(x, a0), [self._values()]))
-
     def get_float(self, a0: StringTraits) -> AnyFloatCollectionTraits:
         return self.map(Lambda(lambda x: get_float(x, a0), [self._values()]))
 
-    def debug_tokens(self) -> CollectionTraits:
-        return self.map(Lambda(debug_tokens, [self._values()]))
+    def remove_tag(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: remove_tag(x, a0), [self._values()]))
 
 class AnyIdentifiableValuesResult(Result, IdentifiableValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return IdentifiableResult
 
 class FeatureTraits(IdentifiableTraits, RenderableTraits):
 
-    def point_features(self) -> PointFeatureCollectionResult:
-        return point_features(self)
+    def closest_distance(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FloatTraits:
+        return closest_distance(self, a0, a1, a2)
+
+    def has_key(self, a0: StringTraits) -> BoolTraits:
+        return has_key(self, a0)
 
     def paths_to_reach(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FeatureIDIntCollectionResult:
         return paths_to_reach(self, a0, a1, a2)
 
+    def reachable(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FeatureCollectionResult:
+        return reachable(self, a0, a1, a2)
+
+    def point_features(self) -> PointFeatureCollectionResult:
+        return point_features(self)
+
     def tile_ids(self) -> FeatureIDIntCollectionResult:
         return tile_ids(self)
 
+    def reachable_points(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> PointFeatureCollectionResult:
+        return reachable_points(self, a0, a1, a2)
+
     def closest(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FeatureTraits:
         return closest(self, a0, a1, a2)
 
-    def connect_to_network(self) -> ChangeTraits:
-        return connect_to_network(self)
-
-    def has_key(self, a0: StringTraits) -> BoolTraits:
-        return has_key(self, a0)
-
-    def reachable(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FeatureCollectionResult:
-        return reachable(self, a0, a1, a2)
-
     def tile_ids_hex(self) -> FeatureIDStringCollectionResult:
         return tile_ids_hex(self)
 
-    def closest_distance(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FloatTraits:
-        return closest_distance(self, a0, a1, a2)
-
-    def reachable_points(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> PointFeatureCollectionResult:
-        return reachable_points(self, a0, a1, a2)
-
     def reachable_area(self, a0: StringTraits, a1: FloatTraits) -> FloatTraits:
         return reachable_area(self, a0, a1)
 
+    def connect_to_network(self) -> ChangeTraits:
+        return connect_to_network(self)
+
     @classmethod
     def _collection(cls):
         return FeatureCollectionResult
 
 class FeatureValuesTraits(IdentifiableValuesTraits, RenderableValuesTraits):
 
-    def point_features(self) -> CollectionTraits:
-        return self.map(Lambda(point_features, [self._values()]))
+    def closest_distance(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(lambda x: closest_distance(x, a0, a1, a2), [self._values()]))
+
+    def has_key(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: has_key(x, a0), [self._values()]))
 
     def paths_to_reach(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: paths_to_reach(x, a0, a1, a2), [self._values()]))
 
+    def reachable(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: reachable(x, a0, a1, a2), [self._values()]))
+
+    def point_features(self) -> CollectionTraits:
+        return self.map(Lambda(point_features, [self._values()]))
+
     def tile_ids(self) -> CollectionTraits:
         return self.map(Lambda(tile_ids, [self._values()]))
 
+    def reachable_points(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: reachable_points(x, a0, a1, a2), [self._values()]))
+
     def closest(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FeatureCollectionTraits:
         return self.map(Lambda(lambda x: closest(x, a0, a1, a2), [self._values()]))
 
-    def connect_to_network(self) -> CollectionTraits:
-        return self.map(Lambda(connect_to_network, [self._values()]))
-
-    def has_key(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: has_key(x, a0), [self._values()]))
-
-    def reachable(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: reachable(x, a0, a1, a2), [self._values()]))
-
     def tile_ids_hex(self) -> CollectionTraits:
         return self.map(Lambda(tile_ids_hex, [self._values()]))
 
-    def closest_distance(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(lambda x: closest_distance(x, a0, a1, a2), [self._values()]))
-
-    def reachable_points(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: reachable_points(x, a0, a1, a2), [self._values()]))
-
     def reachable_area(self, a0: StringTraits, a1: FloatTraits) -> AnyFloatCollectionTraits:
         return self.map(Lambda(lambda x: reachable_area(x, a0, a1), [self._values()]))
 
+    def connect_to_network(self) -> CollectionTraits:
+        return self.map(Lambda(connect_to_network, [self._values()]))
+
 class AnyFeatureValuesResult(Result, FeatureValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return FeatureResult
 
-class PointTraits(GeometryTraits):
-
-    def distance_meters(self, a0: PointTraits) -> FloatTraits:
-        return distance_meters(self, a0)
-
-    def add_point(self, a0: StringPointCollectionResult) -> StringPointCollectionResult:
-        return add_point(self, a0)
-
-    def sightline(self, a0: FloatTraits) -> AreaTraits:
-        return sightline(self, a0)
-
-    def within_cap(self, a0: FloatTraits) -> QueryTraits:
-        return within_cap(self, a0)
-
-    def rectangle_polygon(self, a0: PointTraits) -> AreaTraits:
-        return rectangle_polygon(self, a0)
+class NumberTraits:
 
-    def cap_polygon(self, a0: FloatTraits) -> AreaTraits:
-        return cap_polygon(self, a0)
+    def divide(self, a0: NumberTraits) -> NumberTraits:
+        return divide(self, a0)
 
     @classmethod
     def _collection(cls):
-        return PointCollectionResult
-
-class PointValuesTraits(GeometryValuesTraits):
-
-    def distance_meters(self, a0: PointTraits) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(lambda x: distance_meters(x, a0), [self._values()]))
-
-    def add_point(self, a0: StringPointCollectionResult) -> CollectionTraits:
-        return self.map(Lambda(lambda x: add_point(x, a0), [self._values()]))
-
-    def sightline(self, a0: FloatTraits) -> AreaCollectionTraits:
-        return self.map(Lambda(lambda x: sightline(x, a0), [self._values()]))
-
-    def within_cap(self, a0: FloatTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: within_cap(x, a0), [self._values()]))
+        return CollectionResult
 
-    def rectangle_polygon(self, a0: PointTraits) -> AreaCollectionTraits:
-        return self.map(Lambda(lambda x: rectangle_polygon(x, a0), [self._values()]))
+class NumberValuesTraits:
 
-    def cap_polygon(self, a0: FloatTraits) -> AreaCollectionTraits:
-        return self.map(Lambda(lambda x: cap_polygon(x, a0), [self._values()]))
+    def divide(self, a0: NumberTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: divide(x, a0), [self._values()]))
 
-class AnyPointValuesResult(Result, PointValuesTraits, CollectionTraits):
+class AnyNumberValuesResult(Result, NumberValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return PointResult
+        return NumberResult
 
 class AreaTraits(GeometryTraits):
 
-    def s2_grid(self, a0: IntTraits) -> StringStringCollectionResult:
-        return s2_grid(self, a0)
+    def area(self) -> FloatTraits:
+        return area(self)
 
     def s2_points(self, a0: IntTraits, a1: IntTraits) -> StringPointCollectionResult:
         return s2_points(self, a0, a1)
 
-    def area(self) -> FloatTraits:
-        return area(self)
-
-    def s2_covering(self, a0: IntTraits, a1: IntTraits) -> StringStringCollectionResult:
-        return s2_covering(self, a0, a1)
+    def snap_area_edges(self, a0: QueryTraits, a1: FloatTraits) -> AreaTraits:
+        return snap_area_edges(self, a0, a1)
 
     def within(self) -> QueryTraits:
         return within(self)
 
-    def snap_area_edges(self, a0: QueryTraits, a1: FloatTraits) -> AreaTraits:
-        return snap_area_edges(self, a0, a1)
+    def s2_covering(self, a0: IntTraits, a1: IntTraits) -> StringStringCollectionResult:
+        return s2_covering(self, a0, a1)
+
+    def s2_grid(self, a0: IntTraits) -> StringStringCollectionResult:
+        return s2_grid(self, a0)
 
     @classmethod
     def _collection(cls):
         return AreaCollectionResult
 
 class AreaValuesTraits(GeometryValuesTraits):
 
-    def s2_grid(self, a0: IntTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: s2_grid(x, a0), [self._values()]))
+    def area(self) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(area, [self._values()]))
 
     def s2_points(self, a0: IntTraits, a1: IntTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: s2_points(x, a0, a1), [self._values()]))
 
-    def area(self) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(area, [self._values()]))
-
-    def s2_covering(self, a0: IntTraits, a1: IntTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: s2_covering(x, a0, a1), [self._values()]))
+    def snap_area_edges(self, a0: QueryTraits, a1: FloatTraits) -> AreaCollectionTraits:
+        return self.map(Lambda(lambda x: snap_area_edges(x, a0, a1), [self._values()]))
 
     def within(self) -> CollectionTraits:
         return self.map(Lambda(within, [self._values()]))
 
-    def snap_area_edges(self, a0: QueryTraits, a1: FloatTraits) -> AreaCollectionTraits:
-        return self.map(Lambda(lambda x: snap_area_edges(x, a0, a1), [self._values()]))
+    def s2_covering(self, a0: IntTraits, a1: IntTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: s2_covering(x, a0, a1), [self._values()]))
+
+    def s2_grid(self, a0: IntTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: s2_grid(x, a0), [self._values()]))
 
 class AnyAreaValuesResult(Result, AreaValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return AreaResult
 
-class NumberTraits:
-
-    def divide(self, a0: NumberTraits) -> NumberTraits:
-        return divide(self, a0)
-
-    @classmethod
-    def _collection(cls):
-        return CollectionResult
-
-class NumberValuesTraits:
-
-    def divide(self, a0: NumberTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: divide(x, a0), [self._values()]))
-
-class AnyNumberValuesResult(Result, NumberValuesTraits, CollectionTraits):
-
-    def __init__(self, node):
-        Result.__init__(self, node)
+class PointTraits(GeometryTraits):
 
-    @classmethod
-    def _values(cls):
-        return NumberResult
+    def cap_polygon(self, a0: FloatTraits) -> AreaTraits:
+        return cap_polygon(self, a0)
 
-class PathTraits(GeometryTraits):
+    def distance_meters(self, a0: PointTraits) -> FloatTraits:
+        return distance_meters(self, a0)
 
-    def join(self, a0: PathTraits) -> PathTraits:
-        return join(self, a0)
+    def intersecting_cap(self, a0: FloatTraits) -> QueryTraits:
+        return intersecting_cap(self, a0)
 
-    def sample_points(self, a0: FloatTraits) -> StringPointCollectionResult:
-        return sample_points(self, a0)
+    def add_point(self, a0: StringPointCollectionResult) -> StringPointCollectionResult:
+        return add_point(self, a0)
 
-    def interpolate(self, a0: FloatTraits) -> PointTraits:
-        return interpolate(self, a0)
+    def within_cap(self, a0: FloatTraits) -> QueryTraits:
+        return within_cap(self, a0)
 
-    def distance_to_point_meters(self, a0: PointTraits) -> FloatTraits:
-        return distance_to_point_meters(self, a0)
+    def rectangle_polygon(self, a0: PointTraits) -> AreaTraits:
+        return rectangle_polygon(self, a0)
 
-    def ordered_join(self, a0: PathTraits) -> PathTraits:
-        return ordered_join(self, a0)
+    def sightline(self, a0: FloatTraits) -> AreaTraits:
+        return sightline(self, a0)
 
     @classmethod
     def _collection(cls):
-        return PathCollectionResult
+        return PointCollectionResult
 
-class PathValuesTraits(GeometryValuesTraits):
+class PointValuesTraits(GeometryValuesTraits):
 
-    def join(self, a0: PathTraits) -> PathCollectionTraits:
-        return self.map(Lambda(lambda x: join(x, a0), [self._values()]))
+    def cap_polygon(self, a0: FloatTraits) -> AreaCollectionTraits:
+        return self.map(Lambda(lambda x: cap_polygon(x, a0), [self._values()]))
 
-    def sample_points(self, a0: FloatTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: sample_points(x, a0), [self._values()]))
+    def distance_meters(self, a0: PointTraits) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(lambda x: distance_meters(x, a0), [self._values()]))
 
-    def interpolate(self, a0: FloatTraits) -> PointCollectionTraits:
-        return self.map(Lambda(lambda x: interpolate(x, a0), [self._values()]))
+    def intersecting_cap(self, a0: FloatTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: intersecting_cap(x, a0), [self._values()]))
 
-    def distance_to_point_meters(self, a0: PointTraits) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(lambda x: distance_to_point_meters(x, a0), [self._values()]))
+    def add_point(self, a0: StringPointCollectionResult) -> CollectionTraits:
+        return self.map(Lambda(lambda x: add_point(x, a0), [self._values()]))
 
-    def ordered_join(self, a0: PathTraits) -> PathCollectionTraits:
-        return self.map(Lambda(lambda x: ordered_join(x, a0), [self._values()]))
+    def within_cap(self, a0: FloatTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: within_cap(x, a0), [self._values()]))
 
-class AnyPathValuesResult(Result, PathValuesTraits, CollectionTraits):
+    def rectangle_polygon(self, a0: PointTraits) -> AreaCollectionTraits:
+        return self.map(Lambda(lambda x: rectangle_polygon(x, a0), [self._values()]))
+
+    def sightline(self, a0: FloatTraits) -> AreaCollectionTraits:
+        return self.map(Lambda(lambda x: sightline(x, a0), [self._values()]))
+
+class AnyPointValuesResult(Result, PointValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return PathResult
+        return PointResult
 
 class StringTraits:
 
+    def s2_polygon(self) -> AreaTraits:
+        return s2_polygon(self)
+
     def tagged(self, a0: StringTraits) -> QueryTraits:
         return tagged(self, a0)
 
     def debug_all_query(self) -> QueryTraits:
         return debug_all_query(self)
 
-    def export_world(self) -> IntTraits:
-        return export_world(self)
-
     def keyed(self) -> QueryTraits:
         return keyed(self)
 
-    def import_geojson_file(self, a0: StringTraits) -> ChangeTraits:
-        return import_geojson_file(self, a0)
-
-    def s2_polygon(self) -> AreaTraits:
-        return s2_polygon(self)
+    def tag(self, a0: StringTraits) -> TagTraits:
+        return tag(self, a0)
 
     def parse_geojson(self) -> GeoJSONTraits:
         return parse_geojson(self)
 
-    def tag(self, a0: StringTraits) -> TagTraits:
-        return tag(self, a0)
+    def import_geojson_file(self, a0: StringTraits) -> ChangeTraits:
+        return import_geojson_file(self, a0)
 
     def s2_center(self) -> PointTraits:
         return s2_center(self)
 
+    def export_world(self) -> IntTraits:
+        return export_world(self)
+
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class StringValuesTraits:
 
+    def s2_polygon(self) -> AreaCollectionTraits:
+        return self.map(Lambda(s2_polygon, [self._values()]))
+
     def tagged(self, a0: StringTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: tagged(x, a0), [self._values()]))
 
     def debug_all_query(self) -> CollectionTraits:
         return self.map(Lambda(debug_all_query, [self._values()]))
 
-    def export_world(self) -> CollectionTraits:
-        return self.map(Lambda(export_world, [self._values()]))
-
     def keyed(self) -> CollectionTraits:
         return self.map(Lambda(keyed, [self._values()]))
 
-    def import_geojson_file(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: import_geojson_file(x, a0), [self._values()]))
-
-    def s2_polygon(self) -> AreaCollectionTraits:
-        return self.map(Lambda(s2_polygon, [self._values()]))
+    def tag(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: tag(x, a0), [self._values()]))
 
     def parse_geojson(self) -> CollectionTraits:
         return self.map(Lambda(parse_geojson, [self._values()]))
 
-    def tag(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: tag(x, a0), [self._values()]))
+    def import_geojson_file(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: import_geojson_file(x, a0), [self._values()]))
 
     def s2_center(self) -> PointCollectionTraits:
         return self.map(Lambda(s2_center, [self._values()]))
 
+    def export_world(self) -> CollectionTraits:
+        return self.map(Lambda(export_world, [self._values()]))
+
 class AnyStringValuesResult(Result, StringValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return StringResult
 
+class PathTraits(GeometryTraits):
+
+    def ordered_join(self, a0: PathTraits) -> PathTraits:
+        return ordered_join(self, a0)
+
+    def join(self, a0: PathTraits) -> PathTraits:
+        return join(self, a0)
+
+    def sample_points(self, a0: FloatTraits) -> StringPointCollectionResult:
+        return sample_points(self, a0)
+
+    def distance_to_point_meters(self, a0: PointTraits) -> FloatTraits:
+        return distance_to_point_meters(self, a0)
+
+    def interpolate(self, a0: FloatTraits) -> PointTraits:
+        return interpolate(self, a0)
+
+    @classmethod
+    def _collection(cls):
+        return PathCollectionResult
+
+class PathValuesTraits(GeometryValuesTraits):
+
+    def ordered_join(self, a0: PathTraits) -> PathCollectionTraits:
+        return self.map(Lambda(lambda x: ordered_join(x, a0), [self._values()]))
+
+    def join(self, a0: PathTraits) -> PathCollectionTraits:
+        return self.map(Lambda(lambda x: join(x, a0), [self._values()]))
+
+    def sample_points(self, a0: FloatTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: sample_points(x, a0), [self._values()]))
+
+    def distance_to_point_meters(self, a0: PointTraits) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(lambda x: distance_to_point_meters(x, a0), [self._values()]))
+
+    def interpolate(self, a0: FloatTraits) -> PointCollectionTraits:
+        return self.map(Lambda(lambda x: interpolate(x, a0), [self._values()]))
+
+class AnyPathValuesResult(Result, PathValuesTraits, CollectionTraits):
+
+    def __init__(self, node):
+        Result.__init__(self, node)
+
+    @classmethod
+    def _values(cls):
+        return PathResult
+
 class TagTraits:
 
-    def int_value(self) -> IntTraits:
-        return int_value(self)
+    def float_value(self) -> FloatTraits:
+        return float_value(self)
 
     def value(self) -> StringTraits:
         return value(self)
 
-    def float_value(self) -> FloatTraits:
-        return float_value(self)
+    def int_value(self) -> IntTraits:
+        return int_value(self)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class TagValuesTraits:
 
-    def int_value(self) -> CollectionTraits:
-        return self.map(Lambda(int_value, [self._values()]))
+    def float_value(self) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(float_value, [self._values()]))
 
     def value(self) -> CollectionTraits:
         return self.map(Lambda(value, [self._values()]))
 
-    def float_value(self) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(float_value, [self._values()]))
+    def int_value(self) -> CollectionTraits:
+        return self.map(Lambda(int_value, [self._values()]))
 
 class AnyTagValuesResult(Result, TagValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
@@ -557,123 +568,111 @@
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return IdentifiablePointResult
 
-class RelationFeatureTraits(FeatureTraits, GeometryTraits):
+class AreaFeatureTraits(AreaTraits, FeatureTraits):
     @classmethod
     def _collection(cls):
-        return RelationFeatureCollectionResult
+        return AreaFeatureCollectionResult
 
-class RelationFeatureValuesTraits(FeatureValuesTraits, GeometryValuesTraits):
+class AreaFeatureValuesTraits(AreaValuesTraits, FeatureValuesTraits):
     pass
 
-class AnyRelationFeatureValuesResult(Result, RelationFeatureValuesTraits, CollectionTraits):
+class AnyAreaFeatureValuesResult(Result, AreaFeatureValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return RelationFeatureResult
+        return AreaFeatureResult
 
-class PathFeatureTraits(PathTraits, FeatureTraits):
+class AnyTraits:
 
-    def length(self) -> FloatTraits:
-        return length(self)
+    def pair(self, a0: AnyTraits) -> PairTraits:
+        return pair(self, a0)
+
+    def gt(self, a0: AnyTraits) -> BoolTraits:
+        return gt(self, a0)
+
+    def collection(self, a0: AnyTraits) -> CollectionResult:
+        return collection(self, a0)
 
     @classmethod
     def _collection(cls):
-        return PathFeatureCollectionResult
+        return CollectionResult
 
-class PathFeatureValuesTraits(PathValuesTraits, FeatureValuesTraits):
+class AnyValuesTraits:
 
-    def length(self) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(length, [self._values()]))
+    def pair(self, a0: AnyTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: pair(x, a0), [self._values()]))
 
-class AnyPathFeatureValuesResult(Result, PathFeatureValuesTraits, CollectionTraits):
+    def gt(self, a0: AnyTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: gt(x, a0), [self._values()]))
+
+    def collection(self, a0: AnyTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: collection(x, a0), [self._values()]))
+
+class AnyAnyValuesResult(Result, AnyValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return PathFeatureResult
-
-class IntTraits(NumberTraits):
+        return AnyResult
 
-    def clamp(self, a0: IntTraits, a1: IntTraits) -> IntTraits:
-        return clamp(self, a0, a1)
+class PointFeatureTraits(PointTraits, IdentifiablePointTraits, FeatureTraits):
 
-    def add_ints(self, a0: IntTraits) -> IntTraits:
-        return add_ints(self, a0)
+    def degree(self) -> IntTraits:
+        return degree(self)
 
-    def divide_int(self, a0: FloatTraits) -> FloatTraits:
-        return divide_int(self, a0)
+    def connect(self, a0: PointFeatureTraits) -> ChangeTraits:
+        return connect(self, a0)
 
     @classmethod
     def _collection(cls):
-        return CollectionResult
-
-class IntValuesTraits(NumberValuesTraits):
+        return PointFeatureCollectionResult
 
-    def clamp(self, a0: IntTraits, a1: IntTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: clamp(x, a0, a1), [self._values()]))
+class PointFeatureValuesTraits(PointValuesTraits, IdentifiablePointValuesTraits, FeatureValuesTraits):
 
-    def add_ints(self, a0: IntTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: add_ints(x, a0), [self._values()]))
+    def degree(self) -> CollectionTraits:
+        return self.map(Lambda(degree, [self._values()]))
 
-    def divide_int(self, a0: FloatTraits) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(lambda x: divide_int(x, a0), [self._values()]))
+    def connect(self, a0: PointFeatureTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: connect(x, a0), [self._values()]))
 
-class AnyIntValuesResult(Result, IntValuesTraits, CollectionTraits):
+class AnyPointFeatureValuesResult(Result, PointFeatureValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return IntResult
-
-class AnyTraits:
-
-    def gt(self, a0: AnyTraits) -> BoolTraits:
-        return gt(self, a0)
-
-    def collection(self, a0: AnyTraits) -> CollectionResult:
-        return collection(self, a0)
-
-    def pair(self, a0: AnyTraits) -> PairTraits:
-        return pair(self, a0)
+        return PointFeatureResult
 
+class RelationFeatureTraits(FeatureTraits, GeometryTraits):
     @classmethod
     def _collection(cls):
-        return CollectionResult
-
-class AnyValuesTraits:
-
-    def gt(self, a0: AnyTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: gt(x, a0), [self._values()]))
-
-    def collection(self, a0: AnyTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: collection(x, a0), [self._values()]))
+        return RelationFeatureCollectionResult
 
-    def pair(self, a0: AnyTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: pair(x, a0), [self._values()]))
+class RelationFeatureValuesTraits(FeatureValuesTraits, GeometryValuesTraits):
+    pass
 
-class AnyAnyValuesResult(Result, AnyValuesTraits, CollectionTraits):
+class AnyRelationFeatureValuesResult(Result, RelationFeatureValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return AnyResult
+        return RelationFeatureResult
 
 class FloatTraits(NumberTraits):
 
     def ll(self, a0: FloatTraits) -> PointTraits:
         return ll(self, a0)
 
     @classmethod
@@ -690,290 +689,302 @@
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return FloatResult
 
-class PathCollectionTraits(CollectionTraits, PathValuesTraits):
-
-    def sample_points_along_paths(self, a0: FloatTraits) -> PointCollectionResult:
-        return sample_points_along_paths(self, a0)
-
+class PointCollectionTraits(CollectionTraits, PointValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class AreaFeatureTraits(FeatureTraits, AreaTraits):
+class IntTraits(NumberTraits):
+
+    def clamp(self, a0: IntTraits, a1: IntTraits) -> IntTraits:
+        return clamp(self, a0, a1)
+
+    def add_ints(self, a0: IntTraits) -> IntTraits:
+        return add_ints(self, a0)
+
+    def divide_int(self, a0: FloatTraits) -> FloatTraits:
+        return divide_int(self, a0)
+
     @classmethod
     def _collection(cls):
-        return AreaFeatureCollectionResult
+        return CollectionResult
 
-class AreaFeatureValuesTraits(FeatureValuesTraits, AreaValuesTraits):
-    pass
+class IntValuesTraits(NumberValuesTraits):
 
-class AnyAreaFeatureValuesResult(Result, AreaFeatureValuesTraits, CollectionTraits):
+    def clamp(self, a0: IntTraits, a1: IntTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: clamp(x, a0, a1), [self._values()]))
+
+    def add_ints(self, a0: IntTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: add_ints(x, a0), [self._values()]))
+
+    def divide_int(self, a0: FloatTraits) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(lambda x: divide_int(x, a0), [self._values()]))
+
+class AnyIntValuesResult(Result, IntValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return AreaFeatureResult
+        return IntResult
+
+class PathFeatureTraits(PathTraits, FeatureTraits):
+
+    def length(self) -> FloatTraits:
+        return length(self)
 
-class AreaCollectionTraits(CollectionTraits, AreaValuesTraits):
     @classmethod
     def _collection(cls):
-        return CollectionResult
+        return PathFeatureCollectionResult
 
-class FeatureIDTraits(IdentifiableTraits):
+class PathFeatureValuesTraits(PathValuesTraits, FeatureValuesTraits):
 
-    def find_relation(self) -> RelationFeatureTraits:
-        return find_relation(self)
+    def length(self) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(length, [self._values()]))
 
-    def find_point(self) -> PointFeatureTraits:
-        return find_point(self)
+class AnyPathFeatureValuesResult(Result, PathFeatureValuesTraits, CollectionTraits):
+
+    def __init__(self, node):
+        Result.__init__(self, node)
+
+    @classmethod
+    def _values(cls):
+        return PathFeatureResult
+
+class FeatureIDTraits(IdentifiableTraits):
 
     def find_feature(self) -> FeatureTraits:
         return find_feature(self)
 
+    def find_point(self) -> PointFeatureTraits:
+        return find_point(self)
+
     def find_area(self) -> AreaFeatureTraits:
         return find_area(self)
 
     def find_path(self) -> PathFeatureTraits:
         return find_path(self)
 
+    def find_relation(self) -> RelationFeatureTraits:
+        return find_relation(self)
+
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class FeatureIDValuesTraits(IdentifiableValuesTraits):
 
-    def find_relation(self) -> RelationFeatureCollectionTraits:
-        return self.map(Lambda(find_relation, [self._values()]))
+    def find_feature(self) -> FeatureCollectionTraits:
+        return self.map(Lambda(find_feature, [self._values()]))
 
     def find_point(self) -> PointFeatureCollectionTraits:
         return self.map(Lambda(find_point, [self._values()]))
 
-    def find_feature(self) -> FeatureCollectionTraits:
-        return self.map(Lambda(find_feature, [self._values()]))
-
     def find_area(self) -> AreaFeatureCollectionTraits:
         return self.map(Lambda(find_area, [self._values()]))
 
     def find_path(self) -> PathFeatureCollectionTraits:
         return self.map(Lambda(find_path, [self._values()]))
 
+    def find_relation(self) -> RelationFeatureCollectionTraits:
+        return self.map(Lambda(find_relation, [self._values()]))
+
 class AnyFeatureIDValuesResult(Result, FeatureIDValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return FeatureIDResult
 
-class PointCollectionTraits(CollectionTraits, PointValuesTraits):
+class AreaCollectionTraits(CollectionTraits, AreaValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class PointFeatureTraits(FeatureTraits, IdentifiablePointTraits, PointTraits):
-
-    def connect(self, a0: PointFeatureTraits) -> ChangeTraits:
-        return connect(self, a0)
-
-    def degree(self) -> IntTraits:
-        return degree(self)
-
-    @classmethod
-    def _collection(cls):
-        return PointFeatureCollectionResult
-
-class PointFeatureValuesTraits(FeatureValuesTraits, IdentifiablePointValuesTraits, PointValuesTraits):
-
-    def connect(self, a0: PointFeatureTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: connect(x, a0), [self._values()]))
-
-    def degree(self) -> CollectionTraits:
-        return self.map(Lambda(degree, [self._values()]))
-
-class AnyPointFeatureValuesResult(Result, PointFeatureValuesTraits, CollectionTraits):
-
-    def __init__(self, node):
-        Result.__init__(self, node)
+class PathCollectionTraits(CollectionTraits, PathValuesTraits):
 
-    @classmethod
-    def _values(cls):
-        return PointFeatureResult
+    def sample_points_along_paths(self, a0: FloatTraits) -> PointCollectionResult:
+        return sample_points_along_paths(self, a0)
 
-class AreaFeatureCollectionTraits(AreaCollectionTraits, AreaFeatureValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class FeatureIDTagCollectionTraits(CollectionTraits, TagValuesTraits):
+class AnyRenderableCollectionTraits(CollectionTraits, RenderableValuesTraits):
 
-    def add_tags(self) -> ChangeTraits:
-        return add_tags(self)
+    def to_geojson_collection(self) -> GeoJSONTraits:
+        return to_geojson_collection(self)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class PathFeatureCollectionTraits(PathCollectionTraits, PathFeatureValuesTraits):
+class QueryProtoTraits:
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class FeatureCollectionTraits(CollectionTraits, FeatureValuesTraits):
-
-    def building_access(self, a0: FloatTraits, a1: StringTraits) -> FeatureIDFeatureIDCollectionResult:
-        return building_access(self, a0, a1)
-
+class StringPointCollectionTraits(CollectionTraits, PointValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class PairTraits:
-
-    def first(self) -> AnyTraits:
-        return first(self)
-
-    def second(self) -> AnyTraits:
-        return second(self)
-
+class IntStringCollectionTraits(CollectionTraits, StringValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class RelationFeatureCollectionTraits(CollectionTraits, RelationFeatureValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class GeoJSONTraits:
-
-    def import_geojson(self, a0: StringTraits) -> ChangeTraits:
-        return import_geojson(self, a0)
-
-    def map_geometries(self, a0: Callable[[GeometryTraits],GeometryTraits]) -> GeoJSONTraits:
-        return map_geometries(self, a0)
+class AnyFloatCollectionTraits(CollectionTraits, FloatValuesTraits):
 
-    def geojson_areas(self) -> StringAreaCollectionResult:
-        return geojson_areas(self)
+    def percentiles(self) -> AnyFloatCollectionResult:
+        return percentiles(self)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class IntTagCollectionTraits(CollectionTraits, TagValuesTraits):
+class PointFeatureCollectionTraits(PointCollectionTraits, PointFeatureValuesTraits):
+
+    def containing_areas(self, a0: QueryTraits) -> AreaFeatureCollectionResult:
+        return containing_areas(self, a0)
+
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class StringAreaCollectionTraits(CollectionTraits, AreaValuesTraits):
+class StringStringCollectionTraits(CollectionTraits, StringValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class StringStringCollectionTraits(CollectionTraits, StringValuesTraits):
+class AreaFeatureCollectionTraits(AreaCollectionTraits, AreaFeatureValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class FeatureIDIntCollectionTraits(CollectionTraits, IntValuesTraits):
+class StringAreaCollectionTraits(CollectionTraits, AreaValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class PointFeatureCollectionTraits(PointCollectionTraits, PointFeatureValuesTraits):
+class FeatureCollectionTraits(CollectionTraits, FeatureValuesTraits):
 
-    def containing_areas(self, a0: QueryTraits) -> AreaFeatureCollectionResult:
-        return containing_areas(self, a0)
+    def building_access(self, a0: FloatTraits, a1: StringTraits) -> FeatureIDFeatureIDCollectionResult:
+        return building_access(self, a0, a1)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class QueryProtoTraits:
+class IntTagCollectionTraits(CollectionTraits, TagValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class FeatureIDFeatureIDCollectionTraits(CollectionTraits, FeatureIDValuesTraits):
+class GeoJSONTraits:
+
+    def geojson_areas(self) -> StringAreaCollectionResult:
+        return geojson_areas(self)
+
+    def map_geometries(self, a0: Callable[[GeometryTraits],GeometryTraits]) -> GeoJSONTraits:
+        return map_geometries(self, a0)
+
+    def import_geojson(self, a0: StringTraits) -> ChangeTraits:
+        return import_geojson(self, a0)
+
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class BoolTraits:
+class FeatureIDIntCollectionTraits(CollectionTraits, IntValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class FeatureIDStringCollectionTraits(CollectionTraits, StringValuesTraits):
+class QueryTraits:
 
-    def remove_tags(self) -> ChangeTraits:
-        return remove_tags(self)
+    def and_(self, a0: QueryTraits) -> QueryTraits:
+        return and_(self, a0)
+
+    def find_areas(self) -> AreaFeatureCollectionResult:
+        return find_areas(self)
+
+    def find_points(self) -> PointFeatureCollectionResult:
+        return find_points(self)
+
+    def or_(self, a0: QueryTraits) -> QueryTraits:
+        return or_(self, a0)
+
+    def find_relations(self) -> RelationFeatureCollectionResult:
+        return find_relations(self)
+
+    def find_paths(self) -> PathFeatureCollectionResult:
+        return find_paths(self)
+
+    def find(self) -> FeatureCollectionResult:
+        return find(self)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class IntStringCollectionTraits(CollectionTraits, StringValuesTraits):
+class BoolTraits:
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class AnyFloatCollectionTraits(CollectionTraits, FloatValuesTraits):
+class PairTraits:
 
-    def percentiles(self) -> AnyFloatCollectionResult:
-        return percentiles(self)
+    def second(self) -> AnyTraits:
+        return second(self)
+
+    def first(self) -> AnyTraits:
+        return first(self)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class StringPointCollectionTraits(CollectionTraits, PointValuesTraits):
+class PathFeatureCollectionTraits(PathCollectionTraits, PathFeatureValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class AnyRenderableCollectionTraits(CollectionTraits, RenderableValuesTraits):
+class FeatureIDTagCollectionTraits(CollectionTraits, TagValuesTraits):
 
-    def to_geojson_collection(self) -> GeoJSONTraits:
-        return to_geojson_collection(self)
+    def add_tags(self) -> ChangeTraits:
+        return add_tags(self)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class QueryTraits:
-
-    def find_points(self) -> PointFeatureCollectionResult:
-        return find_points(self)
-
-    def or_(self, a0: QueryTraits) -> QueryTraits:
-        return or_(self, a0)
-
-    def find_paths(self) -> PathFeatureCollectionResult:
-        return find_paths(self)
-
-    def find_relations(self) -> RelationFeatureCollectionResult:
-        return find_relations(self)
-
-    def find_areas(self) -> AreaFeatureCollectionResult:
-        return find_areas(self)
+class FeatureIDStringCollectionTraits(CollectionTraits, StringValuesTraits):
 
-    def and_(self, a0: QueryTraits) -> QueryTraits:
-        return and_(self, a0)
+    def remove_tags(self) -> ChangeTraits:
+        return remove_tags(self)
 
-    def find(self) -> FeatureCollectionResult:
-        return find(self)
+    @classmethod
+    def _collection(cls):
+        return CollectionResult
 
+class FeatureIDFeatureIDCollectionTraits(CollectionTraits, FeatureIDValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class ChangeTraits:
 
     def with_change(self, a0: Callable[[],AnyTraits]) -> AnyTraits:
@@ -1003,626 +1014,632 @@
     def __init__(self, node):
         Result.__init__(self, node)
 
 class FeatureResult(Result, FeatureTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class PointResult(Result, PointTraits):
+class NumberResult(Result, NumberTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
 class AreaResult(Result, AreaTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class NumberResult(Result, NumberTraits):
+class PointResult(Result, PointTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class PathResult(Result, PathTraits):
+class StringResult(Result, StringTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class StringResult(Result, StringTraits):
+class PathResult(Result, PathTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
 class TagResult(Result, TagTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
 class IdentifiablePointResult(Result, IdentifiablePointTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class RelationFeatureResult(Result, RelationFeatureTraits):
+class AreaFeatureResult(Result, AreaFeatureTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class PathFeatureResult(Result, PathFeatureTraits):
+class AnyResult(Result, AnyTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class IntResult(Result, IntTraits):
+class PointFeatureResult(Result, PointFeatureTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class AnyResult(Result, AnyTraits):
+class RelationFeatureResult(Result, RelationFeatureTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
 class FloatResult(Result, FloatTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class PathCollectionResult(Result, PathCollectionTraits):
+class PointCollectionResult(Result, PointCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return PathResult
+        return PointResult
 
-class AreaFeatureResult(Result, AreaFeatureTraits):
+class IntResult(Result, IntTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class AreaCollectionResult(Result, AreaCollectionTraits):
+class PathFeatureResult(Result, PathFeatureTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-    @classmethod
-    def _values(cls):
-        return AreaResult
-
 class FeatureIDResult(Result, FeatureIDTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class PointCollectionResult(Result, PointCollectionTraits):
+class AreaCollectionResult(Result, AreaCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return PointResult
-
-class PointFeatureResult(Result, PointFeatureTraits):
-    def __init__(self, node):
-        Result.__init__(self, node)
+        return AreaResult
 
-class AreaFeatureCollectionResult(Result, AreaFeatureCollectionTraits):
+class PathCollectionResult(Result, PathCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return AreaFeatureResult
+        return PathResult
 
-class FeatureIDTagCollectionResult(Result, FeatureIDTagCollectionTraits):
+class AnyRenderableCollectionResult(Result, AnyRenderableCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return TagResult
+        return RenderableResult
 
-class PathFeatureCollectionResult(Result, PathFeatureCollectionTraits):
+class QueryProtoResult(Result, QueryProtoTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-    @classmethod
-    def _values(cls):
-        return PathFeatureResult
-
-class FeatureCollectionResult(Result, FeatureCollectionTraits):
+class StringPointCollectionResult(Result, StringPointCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return FeatureResult
+        return PointResult
 
-class PairResult(Result, PairTraits):
+class IntStringCollectionResult(Result, IntStringCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
+    @classmethod
+    def _values(cls):
+        return StringResult
+
 class RelationFeatureCollectionResult(Result, RelationFeatureCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return RelationFeatureResult
 
-class GeoJSONResult(Result, GeoJSONTraits):
-    def __init__(self, node):
-        Result.__init__(self, node)
-
-class IntTagCollectionResult(Result, IntTagCollectionTraits):
+class AnyFloatCollectionResult(Result, AnyFloatCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return TagResult
+        return FloatResult
 
-class StringAreaCollectionResult(Result, StringAreaCollectionTraits):
+class PointFeatureCollectionResult(Result, PointFeatureCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return AreaResult
+        return PointFeatureResult
 
 class StringStringCollectionResult(Result, StringStringCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return StringResult
 
-class FeatureIDIntCollectionResult(Result, FeatureIDIntCollectionTraits):
+class AreaFeatureCollectionResult(Result, AreaFeatureCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return IntResult
+        return AreaFeatureResult
 
-class PointFeatureCollectionResult(Result, PointFeatureCollectionTraits):
+class StringAreaCollectionResult(Result, StringAreaCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return PointFeatureResult
+        return AreaResult
 
-class QueryProtoResult(Result, QueryProtoTraits):
+class FeatureCollectionResult(Result, FeatureCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class FeatureIDFeatureIDCollectionResult(Result, FeatureIDFeatureIDCollectionTraits):
+    @classmethod
+    def _values(cls):
+        return FeatureResult
+
+class IntTagCollectionResult(Result, IntTagCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return FeatureIDResult
+        return TagResult
 
-class BoolResult(Result, BoolTraits):
+class GeoJSONResult(Result, GeoJSONTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class FeatureIDStringCollectionResult(Result, FeatureIDStringCollectionTraits):
+class FeatureIDIntCollectionResult(Result, FeatureIDIntCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return StringResult
+        return IntResult
 
-class IntStringCollectionResult(Result, IntStringCollectionTraits):
+class QueryResult(Result, QueryTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-    @classmethod
-    def _values(cls):
-        return StringResult
+class BoolResult(Result, BoolTraits):
+    def __init__(self, node):
+        Result.__init__(self, node)
 
-class AnyFloatCollectionResult(Result, AnyFloatCollectionTraits):
+class PairResult(Result, PairTraits):
+    def __init__(self, node):
+        Result.__init__(self, node)
+
+class PathFeatureCollectionResult(Result, PathFeatureCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return FloatResult
+        return PathFeatureResult
 
-class StringPointCollectionResult(Result, StringPointCollectionTraits):
+class FeatureIDTagCollectionResult(Result, FeatureIDTagCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return PointResult
+        return TagResult
 
-class AnyRenderableCollectionResult(Result, AnyRenderableCollectionTraits):
+class FeatureIDStringCollectionResult(Result, FeatureIDStringCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return RenderableResult
+        return StringResult
 
-class QueryResult(Result, QueryTraits):
+class FeatureIDFeatureIDCollectionResult(Result, FeatureIDFeatureIDCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
+    @classmethod
+    def _values(cls):
+        return FeatureIDResult
+
 class ChangeResult(Result, ChangeTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class FunctionPathGeometryResult(Result, Callable[[PathTraits],GeometryTraits]):
+class FunctionAreaGeometryResult(Result, Callable[[AreaTraits],GeometryTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, a0 : PathTraits) -> GeometryTraits:
+    def __call__(self, a0 : AreaTraits) -> GeometryTraits:
         raise NotImplementedError()
 
-class FunctionAnyBoolResult(Result, Callable[[AnyTraits],BoolTraits]):
+class FunctionAnyAnyResult(Result, Callable[[AnyTraits],AnyTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, a0 : AnyTraits) -> BoolTraits:
+    def __call__(self, a0 : AnyTraits) -> AnyTraits:
         raise NotImplementedError()
 
 class FunctionPointGeometryResult(Result, Callable[[PointTraits],GeometryTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     def __call__(self, a0 : PointTraits) -> GeometryTraits:
         raise NotImplementedError()
 
-class FunctionAnyResult(Result, Callable[[],AnyTraits]):
+class FunctionPairAnyResult(Result, Callable[[PairTraits],AnyTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, ) -> AnyTraits:
+    def __call__(self, a0 : PairTraits) -> AnyTraits:
         raise NotImplementedError()
 
-class FunctionGeometryGeometryResult(Result, Callable[[GeometryTraits],GeometryTraits]):
+class FunctionPathGeometryResult(Result, Callable[[PathTraits],GeometryTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, a0 : GeometryTraits) -> GeometryTraits:
+    def __call__(self, a0 : PathTraits) -> GeometryTraits:
         raise NotImplementedError()
 
-class FunctionPairAnyResult(Result, Callable[[PairTraits],AnyTraits]):
+class FunctionAnyBoolResult(Result, Callable[[AnyTraits],BoolTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, a0 : PairTraits) -> AnyTraits:
+    def __call__(self, a0 : AnyTraits) -> BoolTraits:
         raise NotImplementedError()
 
-class FunctionAnyAnyResult(Result, Callable[[AnyTraits],AnyTraits]):
+class FunctionAnyResult(Result, Callable[[],AnyTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, a0 : AnyTraits) -> AnyTraits:
+    def __call__(self, ) -> AnyTraits:
         raise NotImplementedError()
 
-class FunctionAreaGeometryResult(Result, Callable[[AreaTraits],GeometryTraits]):
+class FunctionGeometryGeometryResult(Result, Callable[[GeometryTraits],GeometryTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, a0 : AreaTraits) -> GeometryTraits:
+    def __call__(self, a0 : GeometryTraits) -> GeometryTraits:
         raise NotImplementedError()
 
-def tagged(a0: StringTraits, a1: StringTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('tagged'), [a0, a1]))
-
-def point_paths(a0: IdentifiablePointTraits) -> PathFeatureCollectionResult:
-    return PathFeatureCollectionResult(Call(Symbol('point-paths'), [a0]))
-
-def join(a0: PathTraits, a1: PathTraits) -> PathTraits:
-    return PathResult(Call(Symbol('join'), [a0, a1]))
-
-def distance_meters(a0: PointTraits, a1: PointTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('distance-meters'), [a0, a1]))
+def closest_distance(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FloatTraits:
+    return FloatResult(Call(Symbol('closest-distance'), [a0, a1, a2, a3]))
 
-def containing_areas(a0: PointFeatureCollectionResult, a1: QueryTraits) -> AreaFeatureCollectionResult:
-    return AreaFeatureCollectionResult(Call(Symbol('containing-areas'), [a0, a1]))
+def cap_polygon(a0: PointTraits, a1: FloatTraits) -> AreaTraits:
+    return AreaResult(Call(Symbol('cap-polygon'), [a0, a1]))
 
-def find_relation(a0: FeatureIDTraits) -> RelationFeatureTraits:
-    return RelationFeatureResult(Call(Symbol('find-relation'), [a0]))
+def apply_to_area(a0: Callable[[AreaTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
+    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-area'), [a0]))
 
-def find_points(a0: QueryTraits) -> PointFeatureCollectionResult:
-    return PointFeatureCollectionResult(Call(Symbol('find-points'), [a0]))
+def pair(a0: AnyTraits, a1: AnyTraits) -> PairTraits:
+    return PairResult(Call(Symbol('pair'), [a0, a1]))
 
-def find_point(a0: FeatureIDTraits) -> PointFeatureTraits:
-    return PointFeatureResult(Call(Symbol('find-point'), [a0]))
+def and_(a0: QueryTraits, a1: QueryTraits) -> QueryTraits:
+    return QueryResult(Call(Symbol('and'), [a0, a1]))
 
 def take(a0: CollectionResult, a1: IntTraits) -> CollectionResult:
     return CollectionResult(Call(Symbol('take'), [a0, a1]))
 
-def or_(a0: QueryTraits, a1: QueryTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('or'), [a0, a1]))
+def find_feature(a0: FeatureIDTraits) -> FeatureTraits:
+    return FeatureResult(Call(Symbol('find-feature'), [a0]))
 
-def point_features(a0: FeatureTraits) -> PointFeatureCollectionResult:
-    return PointFeatureCollectionResult(Call(Symbol('point-features'), [a0]))
+def point_paths(a0: IdentifiablePointTraits) -> PathFeatureCollectionResult:
+    return PathFeatureCollectionResult(Call(Symbol('point-paths'), [a0]))
 
-def gt(a0: AnyTraits, a1: AnyTraits) -> BoolTraits:
-    return BoolResult(Call(Symbol('gt'), [a0, a1]))
+def ordered_join(a0: PathTraits, a1: PathTraits) -> PathTraits:
+    return PathResult(Call(Symbol('ordered-join'), [a0, a1]))
 
-def tile_paths(a0: GeometryTraits, a1: IntTraits) -> IntStringCollectionResult:
-    return IntStringCollectionResult(Call(Symbol('tile-paths'), [a0, a1]))
+def area(a0: AreaTraits) -> FloatTraits:
+    return FloatResult(Call(Symbol('area'), [a0]))
 
-def add_tags(a0: FeatureIDTagCollectionResult) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('add-tags'), [a0]))
+def find_areas(a0: QueryTraits) -> AreaFeatureCollectionResult:
+    return AreaFeatureCollectionResult(Call(Symbol('find-areas'), [a0]))
 
-filter = diagonal_b6.expression._filter
+def degree(a0: PointFeatureTraits) -> IntTraits:
+    return IntResult(Call(Symbol('degree'), [a0]))
 
-def collection(a0: AnyTraits, a1: AnyTraits) -> CollectionResult:
-    return CollectionResult(Call(Symbol('collection'), [a0, a1]))
+def s2_polygon(a0: StringTraits) -> AreaTraits:
+    return AreaResult(Call(Symbol('s2-polygon'), [a0]))
 
-def debug_all_query(a0: StringTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('debug-all-query'), [a0]))
+def has_key(a0: FeatureTraits, a1: StringTraits) -> BoolTraits:
+    return BoolResult(Call(Symbol('has-key'), [a0, a1]))
 
-def map_items(a0: CollectionResult, a1: Callable[[PairTraits],AnyTraits]) -> CollectionResult:
-    return CollectionResult(Call(Symbol('map-items'), [a0, a1]))
+def join(a0: PathTraits, a1: PathTraits) -> PathTraits:
+    return PathResult(Call(Symbol('join'), [a0, a1]))
 
-def first(a0: PairTraits) -> AnyTraits:
-    return AnyResult(Call(Symbol('first'), [a0]))
+def s2_points(a0: AreaTraits, a1: IntTraits, a2: IntTraits) -> StringPointCollectionResult:
+    return StringPointCollectionResult(Call(Symbol('s2-points'), [a0, a1, a2]))
+
+def snap_area_edges(a0: AreaTraits, a1: QueryTraits, a2: FloatTraits) -> AreaTraits:
+    return AreaResult(Call(Symbol('snap-area-edges'), [a0, a1, a2]))
 
 def paths_to_reach(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FeatureIDIntCollectionResult:
     return FeatureIDIntCollectionResult(Call(Symbol('paths-to-reach'), [a0, a1, a2, a3]))
 
-def pair(a0: AnyTraits, a1: AnyTraits) -> PairTraits:
-    return PairResult(Call(Symbol('pair'), [a0, a1]))
-
-def s2_grid(a0: AreaTraits, a1: IntTraits) -> StringStringCollectionResult:
-    return StringStringCollectionResult(Call(Symbol('s2-grid'), [a0, a1]))
-
-def import_geojson(a0: GeoJSONTraits, a1: StringTraits) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('import-geojson'), [a0, a1]))
-
-def export_world(a0: StringTraits) -> IntTraits:
-    return IntResult(Call(Symbol('export-world'), [a0]))
-
-def int_value(a0: TagTraits) -> IntTraits:
-    return IntResult(Call(Symbol('int-value'), [a0]))
-
-def tile_ids(a0: FeatureTraits) -> FeatureIDIntCollectionResult:
-    return FeatureIDIntCollectionResult(Call(Symbol('tile-ids'), [a0]))
+def to_geojson(a0: RenderableTraits) -> GeoJSONTraits:
+    return GeoJSONResult(Call(Symbol('to-geojson'), [a0]))
 
-def get_int(a0: IdentifiableTraits, a1: StringTraits) -> IntTraits:
-    return IntResult(Call(Symbol('get-int'), [a0, a1]))
+def map_items(a0: CollectionResult, a1: Callable[[PairTraits],AnyTraits]) -> CollectionResult:
+    return CollectionResult(Call(Symbol('map-items'), [a0, a1]))
 
-def all() -> QueryTraits:
-    return QueryResult(Call(Symbol('all'), []))
+def tagged(a0: StringTraits, a1: StringTraits) -> QueryTraits:
+    return QueryResult(Call(Symbol('tagged'), [a0, a1]))
 
 def clamp(a0: IntTraits, a1: IntTraits, a2: IntTraits) -> IntTraits:
     return IntResult(Call(Symbol('clamp'), [a0, a1, a2]))
 
-def percentiles(a0: AnyFloatCollectionResult) -> AnyFloatCollectionResult:
-    return AnyFloatCollectionResult(Call(Symbol('percentiles'), [a0]))
+def connect(a0: PointFeatureTraits, a1: PointFeatureTraits) -> ChangeTraits:
+    return ChangeResult(Call(Symbol('connect'), [a0, a1]))
 
-def count(a0: CollectionResult) -> IntTraits:
-    return IntResult(Call(Symbol('count'), [a0]))
+def to_geojson_collection(a0: AnyRenderableCollectionResult) -> GeoJSONTraits:
+    return GeoJSONResult(Call(Symbol('to-geojson-collection'), [a0]))
 
-def remove_tags(a0: FeatureIDStringCollectionResult) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('remove-tags'), [a0]))
+def apply_to_path(a0: Callable[[PathTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
+    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-path'), [a0]))
 
-def get(a0: IdentifiableTraits, a1: StringTraits) -> TagTraits:
-    return TagResult(Call(Symbol('get'), [a0, a1]))
+def type_point() -> QueryProtoTraits:
+    return QueryProtoResult(Call(Symbol('type-point'), []))
 
-def closest(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FeatureTraits:
-    return FeatureResult(Call(Symbol('closest'), [a0, a1, a2, a3]))
+def float_value(a0: TagTraits) -> FloatTraits:
+    return FloatResult(Call(Symbol('float-value'), [a0]))
 
-def add_ints(a0: IntTraits, a1: IntTraits) -> IntTraits:
-    return IntResult(Call(Symbol('add-ints'), [a0, a1]))
+def geojson_areas(a0: GeoJSONTraits) -> StringAreaCollectionResult:
+    return StringAreaCollectionResult(Call(Symbol('geojson-areas'), [a0]))
 
-def connect_to_network(a0: FeatureTraits) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('connect-to-network'), [a0]))
+def find_point(a0: FeatureIDTraits) -> PointFeatureTraits:
+    return PointFeatureResult(Call(Symbol('find-point'), [a0]))
 
-def map_geometries(a0: GeoJSONTraits, a1: Callable[[GeometryTraits],GeometryTraits]) -> GeoJSONTraits:
-    return GeoJSONResult(Call(Symbol('map-geometries'), [a0, a1]))
+def find_points(a0: QueryTraits) -> PointFeatureCollectionResult:
+    return PointFeatureCollectionResult(Call(Symbol('find-points'), [a0]))
 
-def has_key(a0: FeatureTraits, a1: StringTraits) -> BoolTraits:
-    return BoolResult(Call(Symbol('has-key'), [a0, a1]))
+def value(a0: TagTraits) -> StringTraits:
+    return StringResult(Call(Symbol('value'), [a0]))
 
 def reachable(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FeatureCollectionResult:
     return FeatureCollectionResult(Call(Symbol('reachable'), [a0, a1, a2, a3]))
 
+def distance_meters(a0: PointTraits, a1: PointTraits) -> FloatTraits:
+    return FloatResult(Call(Symbol('distance-meters'), [a0, a1]))
+
+def add_tags(a0: FeatureIDTagCollectionResult) -> ChangeTraits:
+    return ChangeResult(Call(Symbol('add-tags'), [a0]))
+
+def intersecting_cap(a0: PointTraits, a1: FloatTraits) -> QueryTraits:
+    return QueryResult(Call(Symbol('intersecting-cap'), [a0, a1]))
+
 def add_point(a0: PointTraits, a1: StringPointCollectionResult) -> StringPointCollectionResult:
     return StringPointCollectionResult(Call(Symbol('add-point'), [a0, a1]))
 
-def apply_to_point(a0: Callable[[PointTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
-    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-point'), [a0]))
+def find_area(a0: FeatureIDTraits) -> AreaFeatureTraits:
+    return AreaFeatureResult(Call(Symbol('find-area'), [a0]))
 
-def apply_to_path(a0: Callable[[PathTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
-    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-path'), [a0]))
+def gt(a0: AnyTraits, a1: AnyTraits) -> BoolTraits:
+    return BoolResult(Call(Symbol('gt'), [a0, a1]))
 
-def find_paths(a0: QueryTraits) -> PathFeatureCollectionResult:
-    return PathFeatureCollectionResult(Call(Symbol('find-paths'), [a0]))
+def collection(a0: AnyTraits, a1: AnyTraits) -> CollectionResult:
+    return CollectionResult(Call(Symbol('collection'), [a0, a1]))
+
+def or_(a0: QueryTraits, a1: QueryTraits) -> QueryTraits:
+    return QueryResult(Call(Symbol('or'), [a0, a1]))
+
+def int_value(a0: TagTraits) -> IntTraits:
+    return IntResult(Call(Symbol('int-value'), [a0]))
+
+def get_string(a0: IdentifiableTraits, a1: StringTraits) -> StringTraits:
+    return StringResult(Call(Symbol('get-string'), [a0, a1]))
+
+def empty_points() -> StringPointCollectionResult:
+    return StringPointCollectionResult(Call(Symbol('empty-points'), []))
+
+def second(a0: PairTraits) -> AnyTraits:
+    return AnyResult(Call(Symbol('second'), [a0]))
+
+def find_relations(a0: QueryTraits) -> RelationFeatureCollectionResult:
+    return RelationFeatureCollectionResult(Call(Symbol('find-relations'), [a0]))
+
+def map_geometries(a0: GeoJSONTraits, a1: Callable[[GeometryTraits],GeometryTraits]) -> GeoJSONTraits:
+    return GeoJSONResult(Call(Symbol('map-geometries'), [a0, a1]))
 
 def building_access(a0: FeatureCollectionResult, a1: FloatTraits, a2: StringTraits) -> FeatureIDFeatureIDCollectionResult:
     return FeatureIDFeatureIDCollectionResult(Call(Symbol('building-access'), [a0, a1, a2]))
 
-def remove_tag(a0: IdentifiableTraits, a1: StringTraits) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('remove-tag'), [a0, a1]))
+def debug_all_query(a0: StringTraits) -> QueryTraits:
+    return QueryResult(Call(Symbol('debug-all-query'), [a0]))
 
-def intersecting(a0: GeometryTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('intersecting'), [a0]))
+def count_values(a0: CollectionResult) -> CollectionResult:
+    return CollectionResult(Call(Symbol('count-values'), [a0]))
+
+def within(a0: AreaTraits) -> QueryTraits:
+    return QueryResult(Call(Symbol('within'), [a0]))
+
+def import_geojson(a0: GeoJSONTraits, a1: StringTraits) -> ChangeTraits:
+    return ChangeResult(Call(Symbol('import-geojson'), [a0, a1]))
 
 def add_tag(a0: IdentifiableTraits, a1: TagTraits) -> ChangeTraits:
     return ChangeResult(Call(Symbol('add-tag'), [a0, a1]))
 
-def s2_points(a0: AreaTraits, a1: IntTraits, a2: IntTraits) -> StringPointCollectionResult:
-    return StringPointCollectionResult(Call(Symbol('s2-points'), [a0, a1, a2]))
+def map_parallel(a0: CollectionResult, a1: Callable[[AnyTraits],AnyTraits]) -> CollectionResult:
+    return CollectionResult(Call(Symbol('map-parallel'), [a0, a1]))
+
+def sum_by_key(a0: CollectionResult) -> CollectionResult:
+    return CollectionResult(Call(Symbol('sum-by-key'), [a0]))
+
+def keyed(a0: StringTraits) -> QueryTraits:
+    return QueryResult(Call(Symbol('keyed'), [a0]))
 
 def sample_points(a0: PathTraits, a1: FloatTraits) -> StringPointCollectionResult:
     return StringPointCollectionResult(Call(Symbol('sample-points'), [a0, a1]))
 
-def connect(a0: PointFeatureTraits, a1: PointFeatureTraits) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('connect'), [a0, a1]))
+def find_paths(a0: QueryTraits) -> PathFeatureCollectionResult:
+    return PathFeatureCollectionResult(Call(Symbol('find-paths'), [a0]))
 
-def interpolate(a0: PathTraits, a1: FloatTraits) -> PointTraits:
-    return PointResult(Call(Symbol('interpolate'), [a0, a1]))
+def type_path() -> QueryProtoTraits:
+    return QueryProtoResult(Call(Symbol('type-path'), []))
 
-def sightline(a0: PointTraits, a1: FloatTraits) -> AreaTraits:
-    return AreaResult(Call(Symbol('sightline'), [a0, a1]))
+def type_area() -> QueryProtoTraits:
+    return QueryProtoResult(Call(Symbol('type-area'), []))
 
-def all_tags(a0: IdentifiableTraits) -> IntTagCollectionResult:
-    return IntTagCollectionResult(Call(Symbol('all-tags'), [a0]))
+def within_cap(a0: PointTraits, a1: FloatTraits) -> QueryTraits:
+    return QueryResult(Call(Symbol('within-cap'), [a0, a1]))
 
-def type_point() -> QueryProtoTraits:
-    return QueryProtoResult(Call(Symbol('type-point'), []))
+def s2_covering(a0: AreaTraits, a1: IntTraits, a2: IntTraits) -> StringStringCollectionResult:
+    return StringStringCollectionResult(Call(Symbol('s2-covering'), [a0, a1, a2]))
 
-def length(a0: PathFeatureTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('length'), [a0]))
+def centroid(a0: GeometryTraits) -> PointTraits:
+    return PointResult(Call(Symbol('centroid'), [a0]))
 
-def points(a0: GeometryTraits) -> PointCollectionResult:
-    return PointCollectionResult(Call(Symbol('points'), [a0]))
+def find(a0: QueryTraits) -> FeatureCollectionResult:
+    return FeatureCollectionResult(Call(Symbol('find'), [a0]))
 
-def geojson_areas(a0: GeoJSONTraits) -> StringAreaCollectionResult:
-    return StringAreaCollectionResult(Call(Symbol('geojson-areas'), [a0]))
+def all() -> QueryTraits:
+    return QueryResult(Call(Symbol('all'), []))
 
-def second(a0: PairTraits) -> AnyTraits:
-    return AnyResult(Call(Symbol('second'), [a0]))
+def distance_to_point_meters(a0: PathTraits, a1: PointTraits) -> FloatTraits:
+    return FloatResult(Call(Symbol('distance-to-point-meters'), [a0, a1]))
 
-def count_tag_value(a0: IdentifiableTraits, a1: StringTraits) -> CollectionResult:
-    return CollectionResult(Call(Symbol('count-tag-value'), [a0, a1]))
+def point_features(a0: FeatureTraits) -> PointFeatureCollectionResult:
+    return PointFeatureCollectionResult(Call(Symbol('point-features'), [a0]))
 
-def divide(a0: NumberTraits, a1: NumberTraits) -> NumberTraits:
-    return NumberResult(Call(Symbol('divide'), [a0, a1]))
+def count(a0: CollectionResult) -> IntTraits:
+    return IntResult(Call(Symbol('count'), [a0]))
 
-def to_geojson_collection(a0: AnyRenderableCollectionResult) -> GeoJSONTraits:
-    return GeoJSONResult(Call(Symbol('to-geojson-collection'), [a0]))
+def tile_ids(a0: FeatureTraits) -> FeatureIDIntCollectionResult:
+    return FeatureIDIntCollectionResult(Call(Symbol('tile-ids'), [a0]))
 
-def keyed(a0: StringTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('keyed'), [a0]))
+def find_path(a0: FeatureIDTraits) -> PathFeatureTraits:
+    return PathFeatureResult(Call(Symbol('find-path'), [a0]))
 
-def get_string(a0: IdentifiableTraits, a1: StringTraits) -> StringTraits:
-    return StringResult(Call(Symbol('get-string'), [a0, a1]))
+def tag(a0: StringTraits, a1: StringTraits) -> TagTraits:
+    return TagResult(Call(Symbol('tag'), [a0, a1]))
 
-def value(a0: TagTraits) -> StringTraits:
-    return StringResult(Call(Symbol('value'), [a0]))
+def points(a0: GeometryTraits) -> PointCollectionResult:
+    return PointCollectionResult(Call(Symbol('points'), [a0]))
 
-def get_float(a0: IdentifiableTraits, a1: StringTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('get-float'), [a0, a1]))
+def apply_to_point(a0: Callable[[PointTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
+    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-point'), [a0]))
 
-def tile_ids_hex(a0: FeatureTraits) -> FeatureIDStringCollectionResult:
-    return FeatureIDStringCollectionResult(Call(Symbol('tile-ids-hex'), [a0]))
+def get(a0: IdentifiableTraits, a1: StringTraits) -> TagTraits:
+    return TagResult(Call(Symbol('get'), [a0, a1]))
 
-def find_relations(a0: QueryTraits) -> RelationFeatureCollectionResult:
-    return RelationFeatureCollectionResult(Call(Symbol('find-relations'), [a0]))
+def rectangle_polygon(a0: PointTraits, a1: PointTraits) -> AreaTraits:
+    return AreaResult(Call(Symbol('rectangle-polygon'), [a0, a1]))
 
-def distance_to_point_meters(a0: PathTraits, a1: PointTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('distance-to-point-meters'), [a0, a1]))
+def s2_grid(a0: AreaTraits, a1: IntTraits) -> StringStringCollectionResult:
+    return StringStringCollectionResult(Call(Symbol('s2-grid'), [a0, a1]))
 
-def debug_tokens(a0: IdentifiableTraits) -> IntStringCollectionResult:
-    return IntStringCollectionResult(Call(Symbol('debug-tokens'), [a0]))
+def sightline(a0: PointTraits, a1: FloatTraits) -> AreaTraits:
+    return AreaResult(Call(Symbol('sightline'), [a0, a1]))
 
-def find_areas(a0: QueryTraits) -> AreaFeatureCollectionResult:
-    return AreaFeatureCollectionResult(Call(Symbol('find-areas'), [a0]))
+def parse_geojson(a0: StringTraits) -> GeoJSONTraits:
+    return GeoJSONResult(Call(Symbol('parse-geojson'), [a0]))
 
-def float_value(a0: TagTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('float-value'), [a0]))
+def remove_tags(a0: FeatureIDStringCollectionResult) -> ChangeTraits:
+    return ChangeResult(Call(Symbol('remove-tags'), [a0]))
 
-def within_cap(a0: PointTraits, a1: FloatTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('within-cap'), [a0, a1]))
+filter = diagonal_b6.expression._filter
 
-def rectangle_polygon(a0: PointTraits, a1: PointTraits) -> AreaTraits:
-    return AreaResult(Call(Symbol('rectangle-polygon'), [a0, a1]))
+def intersecting(a0: GeometryTraits) -> QueryTraits:
+    return QueryResult(Call(Symbol('intersecting'), [a0]))
 
-def to_geojson(a0: RenderableTraits) -> GeoJSONTraits:
-    return GeoJSONResult(Call(Symbol('to-geojson'), [a0]))
+def percentiles(a0: AnyFloatCollectionResult) -> AnyFloatCollectionResult:
+    return AnyFloatCollectionResult(Call(Symbol('percentiles'), [a0]))
 
-map = diagonal_b6.expression._map
+def tile_paths(a0: GeometryTraits, a1: IntTraits) -> IntStringCollectionResult:
+    return IntStringCollectionResult(Call(Symbol('tile-paths'), [a0, a1]))
 
-def and_(a0: QueryTraits, a1: QueryTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('and'), [a0, a1]))
+def all_tags(a0: IdentifiableTraits) -> IntTagCollectionResult:
+    return IntTagCollectionResult(Call(Symbol('all-tags'), [a0]))
 
-def cap_polygon(a0: PointTraits, a1: FloatTraits) -> AreaTraits:
-    return AreaResult(Call(Symbol('cap-polygon'), [a0, a1]))
+def reachable_points(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> PointFeatureCollectionResult:
+    return PointFeatureCollectionResult(Call(Symbol('reachable-points'), [a0, a1, a2, a3]))
 
-def empty_points() -> StringPointCollectionResult:
-    return StringPointCollectionResult(Call(Symbol('empty-points'), []))
+def closest(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FeatureTraits:
+    return FeatureResult(Call(Symbol('closest'), [a0, a1, a2, a3]))
+
+def interpolate(a0: PathTraits, a1: FloatTraits) -> PointTraits:
+    return PointResult(Call(Symbol('interpolate'), [a0, a1]))
 
 def import_geojson_file(a0: StringTraits, a1: StringTraits) -> ChangeTraits:
     return ChangeResult(Call(Symbol('import-geojson-file'), [a0, a1]))
 
-def find(a0: QueryTraits) -> FeatureCollectionResult:
-    return FeatureCollectionResult(Call(Symbol('find'), [a0]))
-
-def closest_distance(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('closest-distance'), [a0, a1, a2, a3]))
+def debug_tokens(a0: IdentifiableTraits) -> IntStringCollectionResult:
+    return IntStringCollectionResult(Call(Symbol('debug-tokens'), [a0]))
 
-def area(a0: AreaTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('area'), [a0]))
+def first(a0: PairTraits) -> AnyTraits:
+    return AnyResult(Call(Symbol('first'), [a0]))
 
-def apply_to_area(a0: Callable[[AreaTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
-    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-area'), [a0]))
+def sample_points_along_paths(a0: PathCollectionResult, a1: FloatTraits) -> PointCollectionResult:
+    return PointCollectionResult(Call(Symbol('sample-points-along-paths'), [a0, a1]))
 
-def s2_covering(a0: AreaTraits, a1: IntTraits, a2: IntTraits) -> StringStringCollectionResult:
-    return StringStringCollectionResult(Call(Symbol('s2-covering'), [a0, a1, a2]))
+def divide(a0: NumberTraits, a1: NumberTraits) -> NumberTraits:
+    return NumberResult(Call(Symbol('divide'), [a0, a1]))
 
-def centroid(a0: GeometryTraits) -> PointTraits:
-    return PointResult(Call(Symbol('centroid'), [a0]))
+def ll(a0: FloatTraits, a1: FloatTraits) -> PointTraits:
+    return PointResult(Call(Symbol('ll'), [a0, a1]))
 
-def s2_polygon(a0: StringTraits) -> AreaTraits:
-    return AreaResult(Call(Symbol('s2-polygon'), [a0]))
+def tile_ids_hex(a0: FeatureTraits) -> FeatureIDStringCollectionResult:
+    return FeatureIDStringCollectionResult(Call(Symbol('tile-ids-hex'), [a0]))
 
-def degree(a0: PointFeatureTraits) -> IntTraits:
-    return IntResult(Call(Symbol('degree'), [a0]))
+def find_relation(a0: FeatureIDTraits) -> RelationFeatureTraits:
+    return RelationFeatureResult(Call(Symbol('find-relation'), [a0]))
 
-def within(a0: AreaTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('within'), [a0]))
+def add_ints(a0: IntTraits, a1: IntTraits) -> IntTraits:
+    return IntResult(Call(Symbol('add-ints'), [a0, a1]))
 
-def reachable_points(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> PointFeatureCollectionResult:
-    return PointFeatureCollectionResult(Call(Symbol('reachable-points'), [a0, a1, a2, a3]))
+def flattern(a0: CollectionResult) -> CollectionResult:
+    return CollectionResult(Call(Symbol('flattern'), [a0]))
 
-def parse_geojson(a0: StringTraits) -> GeoJSONTraits:
-    return GeoJSONResult(Call(Symbol('parse-geojson'), [a0]))
+def get_int(a0: IdentifiableTraits, a1: StringTraits) -> IntTraits:
+    return IntResult(Call(Symbol('get-int'), [a0, a1]))
 
-def find_feature(a0: FeatureIDTraits) -> FeatureTraits:
-    return FeatureResult(Call(Symbol('find-feature'), [a0]))
+def s2_center(a0: StringTraits) -> PointTraits:
+    return PointResult(Call(Symbol('s2-center'), [a0]))
 
 def with_change(a0: ChangeTraits, a1: Callable[[],AnyTraits]) -> AnyTraits:
     return AnyResult(Call(Symbol('with-change'), [a0, a1]))
 
-def find_area(a0: FeatureIDTraits) -> AreaFeatureTraits:
-    return AreaFeatureResult(Call(Symbol('find-area'), [a0]))
+def export_world(a0: StringTraits) -> IntTraits:
+    return IntResult(Call(Symbol('export-world'), [a0]))
 
-def type_area() -> QueryProtoTraits:
-    return QueryProtoResult(Call(Symbol('type-area'), []))
+def containing_areas(a0: PointFeatureCollectionResult, a1: QueryTraits) -> AreaFeatureCollectionResult:
+    return AreaFeatureCollectionResult(Call(Symbol('containing-areas'), [a0, a1]))
 
-def tag(a0: StringTraits, a1: StringTraits) -> TagTraits:
-    return TagResult(Call(Symbol('tag'), [a0, a1]))
+def count_tag_value(a0: IdentifiableTraits, a1: StringTraits) -> CollectionResult:
+    return CollectionResult(Call(Symbol('count-tag-value'), [a0, a1]))
 
 def reachable_area(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits) -> FloatTraits:
     return FloatResult(Call(Symbol('reachable-area'), [a0, a1, a2]))
 
-def snap_area_edges(a0: AreaTraits, a1: QueryTraits, a2: FloatTraits) -> AreaTraits:
-    return AreaResult(Call(Symbol('snap-area-edges'), [a0, a1, a2]))
-
-def sum_by_key(a0: CollectionResult) -> CollectionResult:
-    return CollectionResult(Call(Symbol('sum-by-key'), [a0]))
-
-def count_values(a0: CollectionResult) -> CollectionResult:
-    return CollectionResult(Call(Symbol('count-values'), [a0]))
-
-def type_path() -> QueryProtoTraits:
-    return QueryProtoResult(Call(Symbol('type-path'), []))
-
-def sample_points_along_paths(a0: PathCollectionResult, a1: FloatTraits) -> PointCollectionResult:
-    return PointCollectionResult(Call(Symbol('sample-points-along-paths'), [a0, a1]))
-
-def ordered_join(a0: PathTraits, a1: PathTraits) -> PathTraits:
-    return PathResult(Call(Symbol('ordered-join'), [a0, a1]))
+def get_float(a0: IdentifiableTraits, a1: StringTraits) -> FloatTraits:
+    return FloatResult(Call(Symbol('get-float'), [a0, a1]))
 
-def s2_center(a0: StringTraits) -> PointTraits:
-    return PointResult(Call(Symbol('s2-center'), [a0]))
+def length(a0: PathFeatureTraits) -> FloatTraits:
+    return FloatResult(Call(Symbol('length'), [a0]))
 
-def flattern(a0: CollectionResult) -> CollectionResult:
-    return CollectionResult(Call(Symbol('flattern'), [a0]))
+def remove_tag(a0: IdentifiableTraits, a1: StringTraits) -> ChangeTraits:
+    return ChangeResult(Call(Symbol('remove-tag'), [a0, a1]))
 
 def divide_int(a0: IntTraits, a1: FloatTraits) -> FloatTraits:
     return FloatResult(Call(Symbol('divide-int'), [a0, a1]))
 
-def ll(a0: FloatTraits, a1: FloatTraits) -> PointTraits:
-    return PointResult(Call(Symbol('ll'), [a0, a1]))
+map = diagonal_b6.expression._map
 
-def find_path(a0: FeatureIDTraits) -> PathFeatureTraits:
-    return PathFeatureResult(Call(Symbol('find-path'), [a0]))
+def connect_to_network(a0: FeatureTraits) -> ChangeTraits:
+    return ChangeResult(Call(Symbol('connect-to-network'), [a0]))
```

### Comparing `diagonal_b6-0.0.1/diagonal_b6/api_pb2.py` & `diagonal_b6-0.0.2/diagonal_b6/api_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 import diagonal_b6.geometry_pb2 as geometry__pb2
 import diagonal_b6.features_pb2 as features__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tapi.proto\x12\x03\x61pi\x1a\x0egeometry.proto\x1a\x0e\x66\x65\x61tures.proto\"]\n\x0f\x43ollectionProto\x12#\n\x04keys\x18\x02 \x03(\x0b\x32\x15.api.LiteralNodeProto\x12%\n\x06values\x18\x04 \x03(\x0b\x32\x15.api.LiteralNodeProto\"X\n\tPairProto\x12$\n\x05\x66irst\x18\x01 \x01(\x0b\x32\x15.api.LiteralNodeProto\x12%\n\x06second\x18\x02 \x01(\x0b\x32\x15.api.LiteralNodeProto\">\n\x15ModifiedFeaturesProto\x12%\n\x03ids\x18\x01 \x03(\x0b\x32\x18.features.FeatureIDProto\"l\n\x12\x41ppliedChangeProto\x12*\n\x08original\x18\x01 \x03(\x0b\x32\x18.features.FeatureIDProto\x12*\n\x08modified\x18\x02 \x03(\x0b\x32\x18.features.FeatureIDProto\"\xb8\x01\n\tNodeProto\x12\x10\n\x06symbol\x18\x01 \x01(\tH\x00\x12(\n\x07literal\x18\x02 \x01(\x0b\x32\x15.api.LiteralNodeProtoH\x00\x12\"\n\x04\x63\x61ll\x18\x03 \x01(\x0b\x32\x12.api.CallNodeProtoH\x00\x12\'\n\x07lambda_\x18\x04 \x01(\x0b\x32\x14.api.LambdaNodeProtoH\x00\x12\r\n\x05\x42\x65gin\x18\x06 \x01(\x05\x12\x0b\n\x03\x45nd\x18\x07 \x01(\x05\x42\x06\n\x04node\"\xe9\x04\n\x10LiteralNodeProto\x12\x12\n\x08nilValue\x18\x01 \x01(\x08H\x00\x12\x13\n\tboolValue\x18\x02 \x01(\x08H\x00\x12\x15\n\x0bstringValue\x18\x03 \x01(\tH\x00\x12\x12\n\x08intValue\x18\x04 \x01(\x03H\x00\x12\x14\n\nfloatValue\x18\x05 \x01(\x01H\x00\x12/\n\x0f\x63ollectionValue\x18\x06 \x01(\x0b\x32\x14.api.CollectionProtoH\x00\x12#\n\tpairValue\x18\x07 \x01(\x0b\x32\x0e.api.PairProtoH\x00\x12.\n\x0c\x66\x65\x61tureValue\x18\x08 \x01(\x0b\x32\x16.features.FeatureProtoH\x00\x12%\n\nqueryValue\x18\t \x01(\x0b\x32\x0f.api.QueryProtoH\x00\x12\x32\n\x0e\x66\x65\x61tureIDValue\x18\n \x01(\x0b\x32\x18.features.FeatureIDProtoH\x00\x12*\n\npointValue\x18\x0b \x01(\x0b\x32\x14.geometry.PointProtoH\x00\x12,\n\tpathValue\x18\x0c \x01(\x0b\x32\x17.geometry.PolylineProtoH\x00\x12\x30\n\tareaValue\x18\r \x01(\x0b\x32\x1b.geometry.MultiPolygonProtoH\x00\x12\x35\n\x12\x61ppliedChangeValue\x18\x0e \x01(\x0b\x32\x17.api.AppliedChangeProtoH\x00\x12\x16\n\x0cgeoJSONValue\x18\x0f \x01(\x0cH\x00\x12&\n\x08tagValue\x18\x10 \x01(\x0b\x32\x12.features.TagProtoH\x00\x42\x07\n\x05value\"O\n\rCallNodeProto\x12 \n\x08\x66unction\x18\x01 \x01(\x0b\x32\x0e.api.NodeProto\x12\x1c\n\x04\x61rgs\x18\x02 \x03(\x0b\x32\x0e.api.NodeProto\"=\n\x0fLambdaNodeProto\x12\x0c\n\x04\x61rgs\x18\x01 \x03(\t\x12\x1c\n\x04node\x18\x02 \x01(\x0b\x32\x0e.api.NodeProto\"\x1c\n\rKeyQueryProto\x12\x0b\n\x03key\x18\x01 \x01(\t\"0\n\x12KeyValueQueryProto\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"V\n\x0fTypedQueryProto\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.features.FeatureType\x12\x1e\n\x05query\x18\x02 \x01(\x0b\x32\x0f.api.QueryProto\"0\n\x0cQueriesProto\x12 \n\x07queries\x18\x01 \x03(\x0b\x32\x0f.api.QueryProto\"\x0f\n\rAllQueryProto\"\x11\n\x0f\x45mptyQueryProto\"F\n\x08\x43\x61pProto\x12$\n\x06\x63\x65nter\x18\x01 \x01(\x0b\x32\x14.geometry.PointProto\x12\x14\n\x0cradiusMeters\x18\x02 \x01(\x01\"#\n\x0eS2CellIDsProto\x12\x11\n\ts2CellIDs\x18\x01 \x03(\x04\"\xf1\x04\n\nQueryProto\x12!\n\x03\x61ll\x18\x01 \x01(\x0b\x32\x12.api.AllQueryProtoH\x00\x12%\n\x05\x65mpty\x18\x02 \x01(\x0b\x32\x14.api.EmptyQueryProtoH\x00\x12\x0f\n\x05keyed\x18\x03 \x01(\tH\x00\x12$\n\x06tagged\x18\x04 \x01(\x0b\x32\x12.features.TagProtoH\x00\x12%\n\x05typed\x18\x05 \x01(\x0b\x32\x14.api.TypedQueryProtoH\x00\x12)\n\x0cintersection\x18\x06 \x01(\x0b\x32\x11.api.QueriesProtoH\x00\x12\"\n\x05union\x18\x07 \x01(\x0b\x32\x11.api.QueriesProtoH\x00\x12&\n\rintersectsCap\x18\x08 \x01(\x0b\x32\r.api.CapProtoH\x00\x12\x35\n\x11intersectsFeature\x18\t \x01(\x0b\x32\x18.features.FeatureIDProtoH\x00\x12/\n\x0fintersectsPoint\x18\n \x01(\x0b\x32\x14.geometry.PointProtoH\x00\x12\x35\n\x12intersectsPolyline\x18\x0b \x01(\x0b\x32\x17.geometry.PolylineProtoH\x00\x12=\n\x16intersectsMultiPolygon\x18\x0c \x01(\x0b\x32\x1b.geometry.MultiPolygonProtoH\x00\x12.\n\x0fintersectsCells\x18\r \x01(\x0b\x32\x13.api.S2CellIDsProtoH\x00\x12-\n\x0emightIntersect\x18\x0e \x01(\x0b\x32\x13.api.S2CellIDsProtoH\x00\x42\x07\n\x05query\"C\n\x1b\x46indFeatureByIDRequestProto\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.features.FeatureIDProto\"G\n\x1c\x46indFeatureByIDResponseProto\x12\'\n\x07\x66\x65\x61ture\x18\x01 \x01(\x0b\x32\x16.features.FeatureProto\":\n\x18\x46indFeaturesRequestProto\x12\x1e\n\x05query\x18\x01 \x01(\x0b\x32\x0f.api.QueryProto\"E\n\x19\x46indFeaturesResponseProto\x12(\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32\x16.features.FeatureProto\"`\n\x16ModifyTagsRequestProto\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.features.FeatureIDProto\x12 \n\x04tags\x18\x02 \x03(\x0b\x32\x12.features.TagProto\"L\n\x1bModifyTagsBatchRequestProto\x12-\n\x08requests\x18\x01 \x03(\x0b\x32\x1b.api.ModifyTagsRequestProto\"\x1e\n\x1cModifyTagsBatchResponseProto\"7\n\x14\x45valuateRequestProto\x12\x1f\n\x07request\x18\x01 \x01(\x0b\x32\x0e.api.NodeProto\"7\n\x15\x45valuateResponseProto\x12\x1e\n\x06result\x18\x01 \x01(\x0b\x32\x0e.api.NodeProto2G\n\x02\x42\x36\x12\x41\n\x08\x45valuate\x12\x19.api.EvaluateRequestProto\x1a\x1a.api.EvaluateResponseProtoB\x19Z\x17\x64iagonal.works/b6/protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tapi.proto\x12\x03\x61pi\x1a\x0egeometry.proto\x1a\x0e\x66\x65\x61tures.proto\"]\n\x0f\x43ollectionProto\x12#\n\x04keys\x18\x02 \x03(\x0b\x32\x15.api.LiteralNodeProto\x12%\n\x06values\x18\x04 \x03(\x0b\x32\x15.api.LiteralNodeProto\"X\n\tPairProto\x12$\n\x05\x66irst\x18\x01 \x01(\x0b\x32\x15.api.LiteralNodeProto\x12%\n\x06second\x18\x02 \x01(\x0b\x32\x15.api.LiteralNodeProto\">\n\x15ModifiedFeaturesProto\x12%\n\x03ids\x18\x01 \x03(\x0b\x32\x18.features.FeatureIDProto\"l\n\x12\x41ppliedChangeProto\x12*\n\x08original\x18\x01 \x03(\x0b\x32\x18.features.FeatureIDProto\x12*\n\x08modified\x18\x02 \x03(\x0b\x32\x18.features.FeatureIDProto\"\xb8\x01\n\tNodeProto\x12\x10\n\x06symbol\x18\x01 \x01(\tH\x00\x12(\n\x07literal\x18\x02 \x01(\x0b\x32\x15.api.LiteralNodeProtoH\x00\x12\"\n\x04\x63\x61ll\x18\x03 \x01(\x0b\x32\x12.api.CallNodeProtoH\x00\x12\'\n\x07lambda_\x18\x04 \x01(\x0b\x32\x14.api.LambdaNodeProtoH\x00\x12\r\n\x05\x42\x65gin\x18\x06 \x01(\x05\x12\x0b\n\x03\x45nd\x18\x07 \x01(\x05\x42\x06\n\x04node\"\xe9\x04\n\x10LiteralNodeProto\x12\x12\n\x08nilValue\x18\x01 \x01(\x08H\x00\x12\x13\n\tboolValue\x18\x02 \x01(\x08H\x00\x12\x15\n\x0bstringValue\x18\x03 \x01(\tH\x00\x12\x12\n\x08intValue\x18\x04 \x01(\x03H\x00\x12\x14\n\nfloatValue\x18\x05 \x01(\x01H\x00\x12/\n\x0f\x63ollectionValue\x18\x06 \x01(\x0b\x32\x14.api.CollectionProtoH\x00\x12#\n\tpairValue\x18\x07 \x01(\x0b\x32\x0e.api.PairProtoH\x00\x12.\n\x0c\x66\x65\x61tureValue\x18\x08 \x01(\x0b\x32\x16.features.FeatureProtoH\x00\x12%\n\nqueryValue\x18\t \x01(\x0b\x32\x0f.api.QueryProtoH\x00\x12\x32\n\x0e\x66\x65\x61tureIDValue\x18\n \x01(\x0b\x32\x18.features.FeatureIDProtoH\x00\x12*\n\npointValue\x18\x0b \x01(\x0b\x32\x14.geometry.PointProtoH\x00\x12,\n\tpathValue\x18\x0c \x01(\x0b\x32\x17.geometry.PolylineProtoH\x00\x12\x30\n\tareaValue\x18\r \x01(\x0b\x32\x1b.geometry.MultiPolygonProtoH\x00\x12\x35\n\x12\x61ppliedChangeValue\x18\x0e \x01(\x0b\x32\x17.api.AppliedChangeProtoH\x00\x12\x16\n\x0cgeoJSONValue\x18\x0f \x01(\x0cH\x00\x12&\n\x08tagValue\x18\x10 \x01(\x0b\x32\x12.features.TagProtoH\x00\x42\x07\n\x05value\"O\n\rCallNodeProto\x12 \n\x08\x66unction\x18\x01 \x01(\x0b\x32\x0e.api.NodeProto\x12\x1c\n\x04\x61rgs\x18\x02 \x03(\x0b\x32\x0e.api.NodeProto\"=\n\x0fLambdaNodeProto\x12\x0c\n\x04\x61rgs\x18\x01 \x03(\t\x12\x1c\n\x04node\x18\x02 \x01(\x0b\x32\x0e.api.NodeProto\"\x1c\n\rKeyQueryProto\x12\x0b\n\x03key\x18\x01 \x01(\t\"0\n\x12KeyValueQueryProto\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"V\n\x0fTypedQueryProto\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.features.FeatureType\x12\x1e\n\x05query\x18\x02 \x01(\x0b\x32\x0f.api.QueryProto\"0\n\x0cQueriesProto\x12 \n\x07queries\x18\x01 \x03(\x0b\x32\x0f.api.QueryProto\"\x0f\n\rAllQueryProto\"\x11\n\x0f\x45mptyQueryProto\"F\n\x08\x43\x61pProto\x12$\n\x06\x63\x65nter\x18\x01 \x01(\x0b\x32\x14.geometry.PointProto\x12\x14\n\x0cradiusMeters\x18\x02 \x01(\x01\"#\n\x0eS2CellIDsProto\x12\x11\n\ts2CellIDs\x18\x01 \x03(\x04\"\xf1\x04\n\nQueryProto\x12!\n\x03\x61ll\x18\x01 \x01(\x0b\x32\x12.api.AllQueryProtoH\x00\x12%\n\x05\x65mpty\x18\x02 \x01(\x0b\x32\x14.api.EmptyQueryProtoH\x00\x12\x0f\n\x05keyed\x18\x03 \x01(\tH\x00\x12$\n\x06tagged\x18\x04 \x01(\x0b\x32\x12.features.TagProtoH\x00\x12%\n\x05typed\x18\x05 \x01(\x0b\x32\x14.api.TypedQueryProtoH\x00\x12)\n\x0cintersection\x18\x06 \x01(\x0b\x32\x11.api.QueriesProtoH\x00\x12\"\n\x05union\x18\x07 \x01(\x0b\x32\x11.api.QueriesProtoH\x00\x12&\n\rintersectsCap\x18\x08 \x01(\x0b\x32\r.api.CapProtoH\x00\x12\x35\n\x11intersectsFeature\x18\t \x01(\x0b\x32\x18.features.FeatureIDProtoH\x00\x12/\n\x0fintersectsPoint\x18\n \x01(\x0b\x32\x14.geometry.PointProtoH\x00\x12\x35\n\x12intersectsPolyline\x18\x0b \x01(\x0b\x32\x17.geometry.PolylineProtoH\x00\x12=\n\x16intersectsMultiPolygon\x18\x0c \x01(\x0b\x32\x1b.geometry.MultiPolygonProtoH\x00\x12.\n\x0fintersectsCells\x18\r \x01(\x0b\x32\x13.api.S2CellIDsProtoH\x00\x12-\n\x0emightIntersect\x18\x0e \x01(\x0b\x32\x13.api.S2CellIDsProtoH\x00\x42\x07\n\x05query\"C\n\x1b\x46indFeatureByIDRequestProto\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.features.FeatureIDProto\"G\n\x1c\x46indFeatureByIDResponseProto\x12\'\n\x07\x66\x65\x61ture\x18\x01 \x01(\x0b\x32\x16.features.FeatureProto\":\n\x18\x46indFeaturesRequestProto\x12\x1e\n\x05query\x18\x01 \x01(\x0b\x32\x0f.api.QueryProto\"E\n\x19\x46indFeaturesResponseProto\x12(\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32\x16.features.FeatureProto\"`\n\x16ModifyTagsRequestProto\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.features.FeatureIDProto\x12 \n\x04tags\x18\x02 \x03(\x0b\x32\x12.features.TagProto\"L\n\x1bModifyTagsBatchRequestProto\x12-\n\x08requests\x18\x01 \x03(\x0b\x32\x1b.api.ModifyTagsRequestProto\"\x1e\n\x1cModifyTagsBatchResponseProto\"H\n\x14\x45valuateRequestProto\x12\x1f\n\x07request\x18\x01 \x01(\x0b\x32\x0e.api.NodeProto\x12\x0f\n\x07version\x18\x02 \x01(\t\"7\n\x15\x45valuateResponseProto\x12\x1e\n\x06result\x18\x01 \x01(\x0b\x32\x0e.api.NodeProto2G\n\x02\x42\x36\x12\x41\n\x08\x45valuate\x12\x19.api.EvaluateRequestProto\x1a\x1a.api.EvaluateResponseProtoB\x19Z\x17\x64iagonal.works/b6/protob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\027diagonal.works/b6/proto'
@@ -68,13 +68,13 @@
   _MODIFYTAGSREQUESTPROTO._serialized_start=2624
   _MODIFYTAGSREQUESTPROTO._serialized_end=2720
   _MODIFYTAGSBATCHREQUESTPROTO._serialized_start=2722
   _MODIFYTAGSBATCHREQUESTPROTO._serialized_end=2798
   _MODIFYTAGSBATCHRESPONSEPROTO._serialized_start=2800
   _MODIFYTAGSBATCHRESPONSEPROTO._serialized_end=2830
   _EVALUATEREQUESTPROTO._serialized_start=2832
-  _EVALUATEREQUESTPROTO._serialized_end=2887
-  _EVALUATERESPONSEPROTO._serialized_start=2889
-  _EVALUATERESPONSEPROTO._serialized_end=2944
-  _B6._serialized_start=2946
-  _B6._serialized_end=3017
+  _EVALUATEREQUESTPROTO._serialized_end=2904
+  _EVALUATERESPONSEPROTO._serialized_start=2906
+  _EVALUATERESPONSEPROTO._serialized_end=2961
+  _B6._serialized_start=2963
+  _B6._serialized_end=3034
 # @@protoc_insertion_point(module_scope)
```

### Comparing `diagonal_b6-0.0.1/diagonal_b6/api_pb2_grpc.py` & `diagonal_b6-0.0.2/diagonal_b6/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `diagonal_b6-0.0.1/diagonal_b6/b6_test.py` & `diagonal_b6-0.0.2/diagonal_b6/b6_test.py`

 * *Files identical despite different names*

### Comparing `diagonal_b6-0.0.1/diagonal_b6/expression.py` & `diagonal_b6-0.0.2/diagonal_b6/expression.py`

 * *Files identical despite different names*

### Comparing `diagonal_b6-0.0.1/diagonal_b6/features.py` & `diagonal_b6-0.0.2/diagonal_b6/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,13 +227,13 @@
 def osm_relation_area_id(id):
     return FeatureID(FEATURE_TYPE_AREA, NAMESPACE_OSM_RELATION, id)
 
 def osm_relation_id(id):
     return FeatureID(FEATURE_TYPE_RELATION, NAMESPACE_OSM_RELATION, id)
 
 def uk_ons_boundary_id(id, year=2011):
-    # See newIDForONSArea in src/diagonal.works/diagonal/cmd/ingestons/ingestons.go
+    # See GBONS2011IDStrategy in src/diagonal.works/b6/ingest/gdal/source.go
     if len(id) != 9:
         raise "Expected a string of 9 characters"
     codeBits = ord(id[0]) << 40
     yearBits = (year-1900) << 32
     return FeatureID(FEATURE_TYPE_AREA, NAMESPACE_UK_ONS_BOUNDARIES, codeBits|yearBits|int(id[1:]))
```

### Comparing `diagonal_b6-0.0.1/diagonal_b6/features_pb2.py` & `diagonal_b6-0.0.2/diagonal_b6/features_pb2.py`

 * *Files identical despite different names*

### Comparing `diagonal_b6-0.0.1/diagonal_b6/generate_api.py` & `diagonal_b6-0.0.2/diagonal_b6/generate_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python3
 
-import ast
 import sys
 import json
 
 from copy import copy
 from datetime import datetime
 
 def name_for_function(name):
@@ -129,24 +128,26 @@
     while len(queue) > 0:
         ancestors.append(queue.pop())
         queue.extend(parents.get(ancestors[-1], []))
     return ancestors
 
 def main():
     api = json.load(sys.stdin)
+    print("# Code generated by generate_api.py. DO NOT EDIT.")
     print("# Client library for Diagonal's geospatial analysis engine, b6.")
-    print("# Autogenerated %s" % (datetime.now().strftime("%c")))
     print("")
     print("from __future__ import annotations")
     print("")
     print("from typing import Callable")
     print("")
     print("import diagonal_b6.expression")
     print("from diagonal_b6.expression import Call, Symbol, Lambda, Result")
     print("")
+    print("VERSION = %s" % repr(api["Version"]))
+    print("")
 
     traits = set()
     parents = {}
     hints = {}
     for t in ("any", "int", "float64", "bool", "string"):
         traits.add(t)
         parents[t] = []
```

### Comparing `diagonal_b6-0.0.1/diagonal_b6/geometry.py` & `diagonal_b6-0.0.2/diagonal_b6/geometry.py`

 * *Files identical despite different names*

### Comparing `diagonal_b6-0.0.1/diagonal_b6/geometry_pb2.py` & `diagonal_b6-0.0.2/diagonal_b6/geometry_pb2.py`

 * *Files identical despite different names*

### Comparing `diagonal_b6-0.0.1/diagonal_b6/query.py` & `diagonal_b6-0.0.2/diagonal_b6/query.py`

 * *Files identical despite different names*

### Comparing `diagonal_b6-0.0.1/diagonal_b6.egg-info/PKG-INFO` & `diagonal_b6-0.0.2/diagonal_b6.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: diagonal-b6
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python client library for b6, Diagonal's geospatial analysis engine.
 Author-email: Diagonal Works <hello@diagonal.works>
 License: Apache License
-Project-URL: Homepage, https://diagonal.works/
+Project-URL: Homepage, https://diagonal.works/b6
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `diagonal_b6-0.0.1/diagonal_b6.egg-info/SOURCES.txt` & `diagonal_b6-0.0.2/diagonal_b6.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diagonal_b6-0.0.1/pyproject.toml` & `diagonal_b6-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "diagonal_b6"
 description = "A Python client library for b6, Diagonal's geospatial analysis engine."
 readme = "README.md"
 license = {text = "Apache License"}
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   {name="Diagonal Works", email="hello@diagonal.works"},
 ]
 requires-python = ">=3.10"
 dependencies = [
     "grpcio>=1.43.0",
     "protobuf>=3.14.0",
@@ -22,12 +22,12 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 
 [project.urls]
-"Homepage" = "https://diagonal.works/"
+"Homepage" = "https://diagonal.works/b6"
 
 [tool.setuptools.packages]
 find = {}
```

