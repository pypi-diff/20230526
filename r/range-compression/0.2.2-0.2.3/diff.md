# Comparing `tmp/range_compression-0.2.2.tar.gz` & `tmp/range_compression-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "range_compression-0.2.2.tar", max compression
+gzip compressed data, was "range_compression-0.2.3.tar", max compression
```

## Comparing `range_compression-0.2.2.tar` & `range_compression-0.2.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      488 2023-05-19 02:23:35.360031 range_compression-0.2.2/README.md
--rw-r--r--   0        0        0      622 2023-05-24 08:58:16.319690 range_compression-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       90 2023-05-24 08:58:09.212988 range_compression-0.2.2/range_compression/__init__.py
--rw-r--r--   0        0        0     7216 2023-05-24 08:58:01.719617 range_compression-0.2.2/range_compression/range_compression.py
--rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 range_compression-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      488 2023-05-19 02:23:35.360031 range_compression-0.2.3/README.md
+-rw-r--r--   0        0        0      650 2023-05-26 03:37:23.553567 range_compression-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       90 2023-05-24 08:58:09.212988 range_compression-0.2.3/range_compression/__init__.py
+-rw-r--r--   0        0        0     6686 2023-05-26 03:34:35.229373 range_compression-0.2.3/range_compression/range_compression.py
+-rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 range_compression-0.2.3/PKG-INFO
```

### Comparing `range_compression-0.2.2/pyproject.toml` & `range_compression-0.2.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "range-compression"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["myuan <zhengmy@ion.ac.cn>"]
 license = "LGPL"
 readme = "README.md"
 packages = [{include = "range_compression"}]
 repository = "https://github.com/myuanz/matrix-range-compression"
 
@@ -16,11 +16,12 @@
 importlib-metadata = { version = "^6.6.0", python = "^3.8" }
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 opencv-python-headless = "^4.7.0.72"
 tox = "^4.5.1"
+pytest-benchmark = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `range_compression-0.2.2/range_compression/range_compression.py` & `range_compression-0.2.3/range_compression/range_compression.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 from dataclasses import dataclass
 from datetime import datetime
 from os import PathLike
 from pathlib import Path
 from typing import Union, Optional
-import array
 
 import numba as nb
 import numpy as np
 import polars as pl
 
 
 @dataclass
@@ -147,29 +146,29 @@
         encodings=encodings_np,
         row_indexes=row_indexes_np
     )
 
 
 @nb.njit
 def find_encoding_in_row(row_encodings, col):
-    if len(row_encodings) == 1:
+    if len(row_encodings) == 1 and row_encodings[0, 0] == 0:
         return 0
 
     for start_index, stop_index, value in row_encodings:
         if start_index <= col <= stop_index:
             return value
         elif start_index > col:
             return 0
 
 
 @nb.njit
 def find_encoding_in_row_binary(row_encodings, col):
     # 在细胞中，二分搜索不影响速度，在分区中，二分搜索拖慢 50%
 
-    if len(row_encodings) == 1:
+    if len(row_encodings) == 1 and row_encodings[0, 0] == 0:
         return 0
 
     encoding_index = len(row_encodings) // 2
     upper_index = len(row_encodings)
     lower_index = 0
 
     while True:
@@ -214,28 +213,9 @@
         start_index, length = row_indexes[row]
         row_encoding = encodings_np[start_index : start_index + length, :3]
         res = find_encoding_in_row(row_encoding, col)
         out[i] = res
     return out
 
 
-def find_index(
-    mask_encoding_result: RangeCompressedMask, 
-    X: np.ndarray, Y: np.ndarray, 
-    binary_search=False
-):
-    if mask_encoding_result.encodings.shape[1] == 4:
-        import warnings
-        warnings.warn(f'`row_indexes` has 4 columns.')
-    if not isinstance(X, np.ndarray):
-        X = np.array(X)
-    if not isinstance(Y, np.ndarray):
-        Y = np.array(Y)
-
-    args = (mask_encoding_result.row_indexes, mask_encoding_result.encodings, X, Y)
-    if binary_search:
-        return _find_index_binary(*args)
-    else:
-        return _find_index(*args)
-
 rcm_load = RangeCompressedMask.load
 rcm_find_index = RangeCompressedMask.find_index
```

### Comparing `range_compression-0.2.2/PKG-INFO` & `range_compression-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: range-compression
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Home-page: https://github.com/myuanz/matrix-range-compression
 License: LGPL
 Author: myuan
 Author-email: zhengmy@ion.ac.cn
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
```

