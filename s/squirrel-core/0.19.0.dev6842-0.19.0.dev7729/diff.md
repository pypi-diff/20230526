# Comparing `tmp/squirrel_core-0.19.0.dev6842.tar.gz` & `tmp/squirrel_core-0.19.0.dev7729.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squirrel_core-0.19.0.dev6842.tar", max compression
+gzip compressed data, was "squirrel_core-0.19.0.dev7729.tar", max compression
```

## Comparing `squirrel_core-0.19.0.dev6842.tar` & `squirrel_core-0.19.0.dev7729.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    11348 2023-03-02 12:53:47.212815 squirrel_core-0.19.0.dev6842/LICENSE
--rw-r--r--   0        0        0     5424 2023-03-02 12:53:47.212815 squirrel_core-0.19.0.dev6842/README.md
--rw-r--r--   0        0        0     2982 2023-03-02 13:02:43.273350 squirrel_core-0.19.0.dev6842/pyproject.toml
--rw-r--r--   0        0        0       80 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/__init__.py
--rw-r--r--   0        0        0     3253 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/benchmark/quantify_randomness.py
--rw-r--r--   0        0        0      147 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/catalog/__init__.py
--rw-r--r--   0        0        0    14080 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/catalog/catalog.py
--rw-r--r--   0        0        0      937 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/catalog/source.py
--rw-r--r--   0        0        0     2208 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/catalog/yaml.py
--rw-r--r--   0        0        0      581 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/constants.py
--rw-r--r--   0        0        0      887 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/driver/__init__.py
--rw-r--r--   0        0        0     1182 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/driver/csv.py
--rw-r--r--   0        0        0     4511 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/driver/data_frame.py
--rw-r--r--   0        0        0     8479 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/driver/driver.py
--rw-r--r--   0        0        0      977 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/driver/excel.py
--rw-r--r--   0        0        0     1045 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/driver/feather.py
--rw-r--r--   0        0        0     2127 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/driver/file.py
--rw-r--r--   0        0        0     2192 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/driver/jsonl.py
--rw-r--r--   0        0        0     1099 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/driver/msgpack.py
--rw-r--r--   0        0        0     1203 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/driver/parquet.py
--rw-r--r--   0        0        0     5113 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/driver/source_combiner.py
--rw-r--r--   0        0        0     4586 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/driver/store.py
--rw-r--r--   0        0        0     3230 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/driver/zarr.py
--rw-r--r--   0        0        0        0 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/framework/__init__.py
--rw-r--r--   0        0        0      165 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/framework/exceptions.py
--rw-r--r--   0        0        0     2234 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/framework/io.py
--rw-r--r--   0        0        0       30 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/framework/plugins/__init__.py
--rw-r--r--   0        0        0      788 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/framework/plugins/hookimpl.py
--rw-r--r--   0        0        0      644 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/framework/plugins/hookspec.py
--rw-r--r--   0        0        0     1566 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/framework/plugins/plugin_manager.py
--rw-r--r--   0        0        0      410 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/fsspec/__init__.py
--rw-r--r--   0        0        0     1313 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/fsspec/custom_gcsfs.py
--rw-r--r--   0        0        0     2211 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/fsspec/fs.py
--rw-r--r--   0        0        0        0 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/integration_test/__init__.py
--rw-r--r--   0        0        0      466 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/integration_test/conftest.py
--rw-r--r--   0        0        0     1747 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/integration_test/helpers.py
--rw-r--r--   0        0        0     3774 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/integration_test/shared_fixtures.py
--rw-r--r--   0        0        0     5841 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py
--rw-r--r--   0        0        0      471 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/iterstream/__init__.py
--rw-r--r--   0        0        0    23740 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/iterstream/base.py
--rw-r--r--   0        0        0     9230 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/iterstream/iterators.py
--rw-r--r--   0        0        0     2289 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/iterstream/metrics.py
--rw-r--r--   0        0        0     5999 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/iterstream/source.py
--rw-r--r--   0        0        0     5202 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/iterstream/torch_composables.py
--rw-r--r--   0        0        0      224 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/py.typed
--rw-r--r--   0        0        0      263 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/serialization/__init__.py
--rw-r--r--   0        0        0     4805 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/serialization/jsonl.py
--rw-r--r--   0        0        0     3471 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/serialization/msgpack.py
--rw-r--r--   0        0        0      750 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/serialization/serializer.py
--rw-r--r--   0        0        0      222 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/store/__init__.py
--rw-r--r--   0        0        0     4588 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/store/filesystem.py
--rw-r--r--   0        0        0     4864 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/store/squirrel_store.py
--rw-r--r--   0        0        0     1880 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/store/store.py
--rw-r--r--   0        0        0      110 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/zarr/__init__.py
--rw-r--r--   0        0        0     6137 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/zarr/group.py
--rw-r--r--   0        0        0     2041 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/zarr/key.py
--rw-r--r--   0        0        0     3794 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/zarr/store.py
--rw-r--r--   0        0        0      832 2023-03-02 12:53:47.224815 squirrel_core-0.19.0.dev6842/squirrel/zarr/sync.py
--rw-r--r--   0        0        0     8100 1970-01-01 00:00:00.000000 squirrel_core-0.19.0.dev6842/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-02-28 12:04:31.666615 squirrel_core-0.19.0.dev7729/LICENSE
+-rw-r--r--   0        0        0     5424 2023-02-28 12:04:31.666615 squirrel_core-0.19.0.dev7729/README.md
+-rw-r--r--   0        0        0     2982 2023-02-28 12:12:45.870924 squirrel_core-0.19.0.dev7729/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-02-28 12:04:31.674615 squirrel_core-0.19.0.dev7729/squirrel/__init__.py
+-rw-r--r--   0        0        0     3253 2023-02-28 12:04:31.674615 squirrel_core-0.19.0.dev7729/squirrel/benchmark/quantify_randomness.py
+-rw-r--r--   0        0        0      147 2023-02-28 12:04:31.674615 squirrel_core-0.19.0.dev7729/squirrel/catalog/__init__.py
+-rw-r--r--   0        0        0    14080 2023-02-28 12:04:31.674615 squirrel_core-0.19.0.dev7729/squirrel/catalog/catalog.py
+-rw-r--r--   0        0        0      937 2023-02-28 12:04:31.674615 squirrel_core-0.19.0.dev7729/squirrel/catalog/source.py
+-rw-r--r--   0        0        0     2208 2023-02-28 12:04:31.674615 squirrel_core-0.19.0.dev7729/squirrel/catalog/yaml.py
+-rw-r--r--   0        0        0      581 2023-02-28 12:04:31.674615 squirrel_core-0.19.0.dev7729/squirrel/constants.py
+-rw-r--r--   0        0        0      887 2023-02-28 12:04:31.674615 squirrel_core-0.19.0.dev7729/squirrel/driver/__init__.py
+-rw-r--r--   0        0        0     1182 2023-02-28 12:04:31.674615 squirrel_core-0.19.0.dev7729/squirrel/driver/csv.py
+-rw-r--r--   0        0        0     4511 2023-02-28 12:04:31.674615 squirrel_core-0.19.0.dev7729/squirrel/driver/data_frame.py
+-rw-r--r--   0        0        0     8479 2023-02-28 12:04:31.674615 squirrel_core-0.19.0.dev7729/squirrel/driver/driver.py
+-rw-r--r--   0        0        0      977 2023-02-28 12:04:31.674615 squirrel_core-0.19.0.dev7729/squirrel/driver/excel.py
+-rw-r--r--   0        0        0     1045 2023-02-28 12:04:31.674615 squirrel_core-0.19.0.dev7729/squirrel/driver/feather.py
+-rw-r--r--   0        0        0     2127 2023-02-28 12:04:31.674615 squirrel_core-0.19.0.dev7729/squirrel/driver/file.py
+-rw-r--r--   0        0        0     2192 2023-02-28 12:04:31.674615 squirrel_core-0.19.0.dev7729/squirrel/driver/jsonl.py
+-rw-r--r--   0        0        0     1099 2023-02-28 12:04:31.674615 squirrel_core-0.19.0.dev7729/squirrel/driver/msgpack.py
+-rw-r--r--   0        0        0     1203 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/driver/parquet.py
+-rw-r--r--   0        0        0     5113 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/driver/source_combiner.py
+-rw-r--r--   0        0        0     4586 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/driver/store.py
+-rw-r--r--   0        0        0     3230 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/driver/zarr.py
+-rw-r--r--   0        0        0        0 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/framework/__init__.py
+-rw-r--r--   0        0        0      165 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/framework/exceptions.py
+-rw-r--r--   0        0        0     2234 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/framework/io.py
+-rw-r--r--   0        0        0       30 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/framework/plugins/__init__.py
+-rw-r--r--   0        0        0      788 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/framework/plugins/hookimpl.py
+-rw-r--r--   0        0        0      644 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/framework/plugins/hookspec.py
+-rw-r--r--   0        0        0     1566 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/framework/plugins/plugin_manager.py
+-rw-r--r--   0        0        0      410 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/fsspec/__init__.py
+-rw-r--r--   0        0        0     1313 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/fsspec/custom_gcsfs.py
+-rw-r--r--   0        0        0     2211 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/fsspec/fs.py
+-rw-r--r--   0        0        0        0 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/integration_test/__init__.py
+-rw-r--r--   0        0        0      466 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/integration_test/conftest.py
+-rw-r--r--   0        0        0     1747 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/integration_test/helpers.py
+-rw-r--r--   0        0        0     3774 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/integration_test/shared_fixtures.py
+-rw-r--r--   0        0        0     5841 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py
+-rw-r--r--   0        0        0      471 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/iterstream/__init__.py
+-rw-r--r--   0        0        0    23740 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/iterstream/base.py
+-rw-r--r--   0        0        0     9230 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/iterstream/iterators.py
+-rw-r--r--   0        0        0     2289 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/iterstream/metrics.py
+-rw-r--r--   0        0        0     5999 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/iterstream/source.py
+-rw-r--r--   0        0        0     5202 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/iterstream/torch_composables.py
+-rw-r--r--   0        0        0      224 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/py.typed
+-rw-r--r--   0        0        0      263 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/serialization/__init__.py
+-rw-r--r--   0        0        0     4805 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/serialization/jsonl.py
+-rw-r--r--   0        0        0     3471 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/serialization/msgpack.py
+-rw-r--r--   0        0        0      750 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/serialization/serializer.py
+-rw-r--r--   0        0        0      222 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/store/__init__.py
+-rw-r--r--   0        0        0     4588 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/store/filesystem.py
+-rw-r--r--   0        0        0     4864 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/store/squirrel_store.py
+-rw-r--r--   0        0        0     1880 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/store/store.py
+-rw-r--r--   0        0        0      110 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/zarr/__init__.py
+-rw-r--r--   0        0        0     6137 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/zarr/group.py
+-rw-r--r--   0        0        0     2041 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/zarr/key.py
+-rw-r--r--   0        0        0     3794 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/zarr/store.py
+-rw-r--r--   0        0        0      832 2023-02-28 12:04:31.678615 squirrel_core-0.19.0.dev7729/squirrel/zarr/sync.py
+-rw-r--r--   0        0        0     8100 1970-01-01 00:00:00.000000 squirrel_core-0.19.0.dev7729/PKG-INFO
```

### Comparing `squirrel_core-0.19.0.dev6842/LICENSE` & `squirrel_core-0.19.0.dev7729/LICENSE`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/README.md` & `squirrel_core-0.19.0.dev7729/README.md`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/pyproject.toml` & `squirrel_core-0.19.0.dev7729/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squirrel-core"
-version = "0.19.0-dev6842"
+version = "0.19.0-dev7729"
 description = "Squirrel is a Python library that enables ML teams to share, load, and transform data in a collaborative, flexible and efficient way."
 authors = ["Merantix Momentum"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "squirrel"}]
 homepage = "https://merantix-momentum.com/technology/squirrel/"
 repository = "https://github.com/merantix-momentum/squirrel-core"
```

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/benchmark/quantify_randomness.py` & `squirrel_core-0.19.0.dev7729/squirrel/benchmark/quantify_randomness.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/catalog/catalog.py` & `squirrel_core-0.19.0.dev7729/squirrel/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/catalog/source.py` & `squirrel_core-0.19.0.dev7729/squirrel/catalog/source.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/catalog/yaml.py` & `squirrel_core-0.19.0.dev7729/squirrel/catalog/yaml.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/constants.py` & `squirrel_core-0.19.0.dev7729/squirrel/constants.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/driver/__init__.py` & `squirrel_core-0.19.0.dev7729/squirrel/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/driver/csv.py` & `squirrel_core-0.19.0.dev7729/squirrel/driver/csv.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/driver/data_frame.py` & `squirrel_core-0.19.0.dev7729/squirrel/driver/data_frame.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/driver/driver.py` & `squirrel_core-0.19.0.dev7729/squirrel/driver/driver.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/driver/excel.py` & `squirrel_core-0.19.0.dev7729/squirrel/driver/excel.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/driver/feather.py` & `squirrel_core-0.19.0.dev7729/squirrel/driver/feather.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/driver/file.py` & `squirrel_core-0.19.0.dev7729/squirrel/driver/file.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/driver/jsonl.py` & `squirrel_core-0.19.0.dev7729/squirrel/driver/jsonl.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/driver/msgpack.py` & `squirrel_core-0.19.0.dev7729/squirrel/driver/msgpack.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/driver/parquet.py` & `squirrel_core-0.19.0.dev7729/squirrel/driver/parquet.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/driver/source_combiner.py` & `squirrel_core-0.19.0.dev7729/squirrel/driver/source_combiner.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/driver/store.py` & `squirrel_core-0.19.0.dev7729/squirrel/driver/store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/driver/zarr.py` & `squirrel_core-0.19.0.dev7729/squirrel/driver/zarr.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/framework/io.py` & `squirrel_core-0.19.0.dev7729/squirrel/framework/io.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/framework/plugins/hookimpl.py` & `squirrel_core-0.19.0.dev7729/squirrel/framework/plugins/hookimpl.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/framework/plugins/hookspec.py` & `squirrel_core-0.19.0.dev7729/squirrel/framework/plugins/hookspec.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/framework/plugins/plugin_manager.py` & `squirrel_core-0.19.0.dev7729/squirrel/framework/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/fsspec/custom_gcsfs.py` & `squirrel_core-0.19.0.dev7729/squirrel/fsspec/custom_gcsfs.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/fsspec/fs.py` & `squirrel_core-0.19.0.dev7729/squirrel/fsspec/fs.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/integration_test/helpers.py` & `squirrel_core-0.19.0.dev7729/squirrel/integration_test/helpers.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/integration_test/shared_fixtures.py` & `squirrel_core-0.19.0.dev7729/squirrel/integration_test/shared_fixtures.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py` & `squirrel_core-0.19.0.dev7729/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/iterstream/base.py` & `squirrel_core-0.19.0.dev7729/squirrel/iterstream/base.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/iterstream/iterators.py` & `squirrel_core-0.19.0.dev7729/squirrel/iterstream/iterators.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/iterstream/metrics.py` & `squirrel_core-0.19.0.dev7729/squirrel/iterstream/metrics.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/iterstream/source.py` & `squirrel_core-0.19.0.dev7729/squirrel/iterstream/source.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/iterstream/torch_composables.py` & `squirrel_core-0.19.0.dev7729/squirrel/iterstream/torch_composables.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/serialization/jsonl.py` & `squirrel_core-0.19.0.dev7729/squirrel/serialization/jsonl.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/serialization/msgpack.py` & `squirrel_core-0.19.0.dev7729/squirrel/serialization/msgpack.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/serialization/serializer.py` & `squirrel_core-0.19.0.dev7729/squirrel/serialization/serializer.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/store/filesystem.py` & `squirrel_core-0.19.0.dev7729/squirrel/store/filesystem.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/store/squirrel_store.py` & `squirrel_core-0.19.0.dev7729/squirrel/store/squirrel_store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/store/store.py` & `squirrel_core-0.19.0.dev7729/squirrel/store/store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/zarr/group.py` & `squirrel_core-0.19.0.dev7729/squirrel/zarr/group.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/zarr/key.py` & `squirrel_core-0.19.0.dev7729/squirrel/zarr/key.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/zarr/store.py` & `squirrel_core-0.19.0.dev7729/squirrel/zarr/store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/squirrel/zarr/sync.py` & `squirrel_core-0.19.0.dev7729/squirrel/zarr/sync.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.0.dev6842/PKG-INFO` & `squirrel_core-0.19.0.dev7729/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squirrel-core
-Version: 0.19.0.dev6842
+Version: 0.19.0.dev7729
 Summary: Squirrel is a Python library that enables ML teams to share, load, and transform data in a collaborative, flexible and efficient way.
 Home-page: https://merantix-momentum.com/technology/squirrel/
 License: Apache 2.0
 Author: Merantix Momentum
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

