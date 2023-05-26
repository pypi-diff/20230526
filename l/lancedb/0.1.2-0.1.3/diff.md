# Comparing `tmp/lancedb-0.1.2.tar.gz` & `tmp/lancedb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lancedb-0.1.2.tar", last modified: Fri May  5 18:28:58 2023, max compression
+gzip compressed data, was "lancedb-0.1.3.tar", last modified: Thu May 25 23:58:40 2023, max compression
```

## Comparing `lancedb-0.1.2.tar` & `lancedb-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-05-05 18:28:58.093741 lancedb-0.1.2/
--rw-r--r--   0 changshe   (501) staff       (20)     1003 2023-05-05 18:28:58.093630 lancedb-0.1.2/PKG-INFO
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-05-05 18:28:58.092912 lancedb-0.1.2/lancedb/
--rw-r--r--   0 changshe   (501) staff       (20)      922 2023-05-05 18:26:36.000000 lancedb-0.1.2/lancedb/__init__.py
--rw-r--r--   0 changshe   (501) staff       (20)      889 2023-05-05 18:26:36.000000 lancedb-0.1.2/lancedb/common.py
--rw-r--r--   0 changshe   (501) staff       (20)     2981 2023-05-05 01:55:15.000000 lancedb-0.1.2/lancedb/context.py
--rw-r--r--   0 changshe   (501) staff       (20)     3377 2023-05-05 18:26:36.000000 lancedb-0.1.2/lancedb/db.py
--rw-r--r--   0 changshe   (501) staff       (20)     3758 2023-05-05 18:26:42.000000 lancedb-0.1.2/lancedb/embeddings.py
--rw-r--r--   0 changshe   (501) staff       (20)     3970 2023-05-05 01:55:15.000000 lancedb-0.1.2/lancedb/query.py
--rw-r--r--   0 changshe   (501) staff       (20)     7884 2023-05-05 18:26:36.000000 lancedb-0.1.2/lancedb/table.py
--rw-r--r--   0 changshe   (501) staff       (20)     1376 2023-05-05 01:55:15.000000 lancedb-0.1.2/lancedb/util.py
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-05-05 18:28:58.093464 lancedb-0.1.2/lancedb.egg-info/
--rw-r--r--   0 changshe   (501) staff       (20)     1003 2023-05-05 18:28:58.000000 lancedb-0.1.2/lancedb.egg-info/PKG-INFO
--rw-r--r--   0 changshe   (501) staff       (20)      320 2023-05-05 18:28:58.000000 lancedb-0.1.2/lancedb.egg-info/SOURCES.txt
--rw-r--r--   0 changshe   (501) staff       (20)        1 2023-05-05 18:28:58.000000 lancedb-0.1.2/lancedb.egg-info/dependency_links.txt
--rw-r--r--   0 changshe   (501) staff       (20)      150 2023-05-05 18:28:58.000000 lancedb-0.1.2/lancedb.egg-info/requires.txt
--rw-r--r--   0 changshe   (501) staff       (20)        8 2023-05-05 18:28:58.000000 lancedb-0.1.2/lancedb.egg-info/top_level.txt
--rw-r--r--   0 changshe   (501) staff       (20)     1332 2023-05-05 18:25:41.000000 lancedb-0.1.2/pyproject.toml
--rw-r--r--   0 changshe   (501) staff       (20)       38 2023-05-05 18:28:58.093779 lancedb-0.1.2/setup.cfg
--rw-r--r--   0 changshe   (501) staff       (20)      660 2023-05-05 01:55:15.000000 lancedb-0.1.2/setup.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-05-25 23:58:40.888496 lancedb-0.1.3/
+-rw-r--r--   0 changshe   (501) staff       (20)     1003 2023-05-25 23:58:40.888410 lancedb-0.1.3/PKG-INFO
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-05-25 23:58:40.887747 lancedb-0.1.3/lancedb/
+-rw-r--r--   0 changshe   (501) staff       (20)      922 2023-05-05 18:26:36.000000 lancedb-0.1.3/lancedb/__init__.py
+-rw-r--r--   0 changshe   (501) staff       (20)      889 2023-05-05 18:26:36.000000 lancedb-0.1.3/lancedb/common.py
+-rw-r--r--   0 changshe   (501) staff       (20)     2981 2023-05-05 01:55:15.000000 lancedb-0.1.3/lancedb/context.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3377 2023-05-05 18:26:36.000000 lancedb-0.1.3/lancedb/db.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3758 2023-05-05 18:26:42.000000 lancedb-0.1.3/lancedb/embeddings.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3836 2023-05-25 23:57:48.000000 lancedb-0.1.3/lancedb/fts.py
+-rw-r--r--   0 changshe   (501) staff       (20)     4872 2023-05-25 23:57:48.000000 lancedb-0.1.3/lancedb/query.py
+-rw-r--r--   0 changshe   (501) staff       (20)     8833 2023-05-25 04:41:19.000000 lancedb-0.1.3/lancedb/table.py
+-rw-r--r--   0 changshe   (501) staff       (20)     1376 2023-05-05 01:55:15.000000 lancedb-0.1.3/lancedb/util.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-05-25 23:58:40.888248 lancedb-0.1.3/lancedb.egg-info/
+-rw-r--r--   0 changshe   (501) staff       (20)     1003 2023-05-25 23:58:40.000000 lancedb-0.1.3/lancedb.egg-info/PKG-INFO
+-rw-r--r--   0 changshe   (501) staff       (20)      335 2023-05-25 23:58:40.000000 lancedb-0.1.3/lancedb.egg-info/SOURCES.txt
+-rw-r--r--   0 changshe   (501) staff       (20)        1 2023-05-25 23:58:40.000000 lancedb-0.1.3/lancedb.egg-info/dependency_links.txt
+-rw-r--r--   0 changshe   (501) staff       (20)      151 2023-05-25 23:58:40.000000 lancedb-0.1.3/lancedb.egg-info/requires.txt
+-rw-r--r--   0 changshe   (501) staff       (20)        8 2023-05-25 23:58:40.000000 lancedb-0.1.3/lancedb.egg-info/top_level.txt
+-rw-r--r--   0 changshe   (501) staff       (20)     1333 2023-05-25 23:57:48.000000 lancedb-0.1.3/pyproject.toml
+-rw-r--r--   0 changshe   (501) staff       (20)       38 2023-05-25 23:58:40.888527 lancedb-0.1.3/setup.cfg
+-rw-r--r--   0 changshe   (501) staff       (20)      660 2023-05-05 01:55:15.000000 lancedb-0.1.3/setup.py
```

### Comparing `lancedb-0.1.2/PKG-INFO` & `lancedb-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.1.2
+Version: 0.1.3
 Summary: lancedb
 Author-email: LanceDB Devs <dev@lancedb.com>
 Project-URL: repository, https://github.com/eto-ai/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lancedb-0.1.2/lancedb/__init__.py` & `lancedb-0.1.3/lancedb/__init__.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.2/lancedb/common.py` & `lancedb-0.1.3/lancedb/common.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.2/lancedb/context.py` & `lancedb-0.1.3/lancedb/context.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.2/lancedb/db.py` & `lancedb-0.1.3/lancedb/db.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.2/lancedb/embeddings.py` & `lancedb-0.1.3/lancedb/embeddings.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.2/lancedb/query.py` & `lancedb-0.1.3/lancedb/query.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from __future__ import annotations
 
 import numpy as np
 import pandas as pd
+import pyarrow as pa
 
 from .common import VECTOR_COLUMN_NAME
 
 
 class LanceQueryBuilder:
     """
     A builder for nearest neighbor queries for LanceDB.
@@ -127,21 +128,43 @@
         """
         Execute the query and return the results as a pandas DataFrame.
         In addition to the selected columns, LanceDB also returns a vector
         and also the "score" column which is the distance between the query
         vector and the returned vector.
         """
         ds = self._table.to_lance()
-        # TODO indexed search
         tbl = ds.to_table(
             columns=self._columns,
             filter=self._where,
             nearest={
                 "column": VECTOR_COLUMN_NAME,
                 "q": self._query,
                 "k": self._limit,
                 "metric": self._metric,
                 "nprobes": self._nprobes,
                 "refine_factor": self._refine_factor,
             },
         )
         return tbl.to_pandas()
+
+
+class LanceFtsQueryBuilder(LanceQueryBuilder):
+    def to_df(self) -> pd.DataFrame:
+        try:
+            import tantivy
+        except ImportError:
+            raise ImportError(
+                "Please install tantivy-py `pip install tantivy@git+https://github.com/quickwit-oss/tantivy-py#164adc87e1a033117001cf70e38c82a53014d985` to use the full text search feature."
+            )
+
+        from .fts import search_index
+
+        # get the index path
+        index_path = self._table._get_fts_index_path()
+        # open the index
+        index = tantivy.Index.open(index_path)
+        # get the scores and doc ids
+        row_ids, scores = search_index(index, self._query, self._limit)
+        scores = pa.array(scores)
+        output_tbl = self._table.to_lance().take(row_ids, columns=self._columns)
+        output_tbl = output_tbl.append_column("score", scores)
+        return output_tbl.to_pandas()
```

### Comparing `lancedb-0.1.2/lancedb/table.py` & `lancedb-0.1.3/lancedb/table.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,25 +10,28 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
 import os
+import shutil
 from functools import cached_property
+from typing import List, Union
 
 import lance
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 from lance import LanceDataset
 from lance.vector import vec_to_table
 
 from .common import DATA, VEC, VECTOR_COLUMN_NAME
-from .query import LanceQueryBuilder
+from .query import LanceFtsQueryBuilder, LanceQueryBuilder
+from .util import get_uri_scheme
 
 
 def _sanitize_data(data, schema):
     if isinstance(data, list):
         data = pa.Table.from_pylist(data)
         data = _sanitize_schema(data, schema=schema)
     if isinstance(data, dict):
@@ -126,14 +129,35 @@
             index_type="IVF_PQ",
             metric=metric,
             num_partitions=num_partitions,
             num_sub_vectors=num_sub_vectors,
         )
         self._reset_dataset()
 
+    def create_fts_index(self, field_names: Union[str, List[str]]):
+        """Create a full-text search index on the table.
+
+        Warning - this API is highly experimental and is highly likely to change
+        in the future.
+
+        Parameters
+        ----------
+        field_names: str or list of str
+            The name(s) of the field to index.
+        """
+        from .fts import create_index, populate_index
+
+        if isinstance(field_names, str):
+            field_names = [field_names]
+        index = create_index(self._get_fts_index_path(), field_names)
+        populate_index(index, self, field_names)
+
+    def _get_fts_index_path(self):
+        return os.path.join(self._dataset_uri, "_indices", "tantivy")
+
     @cached_property
     def _dataset(self) -> LanceDataset:
         return lance.dataset(self._dataset_uri, version=self._version)
 
     def to_lance(self) -> LanceDataset:
         """Return the LanceDataset backing this table."""
         return self._dataset
@@ -154,15 +178,15 @@
         The number of vectors added to the table.
         """
         data = _sanitize_data(data, self.schema)
         lance.write_dataset(data, self._dataset_uri, mode=mode)
         self._reset_dataset()
         return len(self)
 
-    def search(self, query: VEC) -> LanceQueryBuilder:
+    def search(self, query: Union[VEC, str]) -> LanceQueryBuilder:
         """Create a search query to find the nearest neighbors
         of the given query vector.
 
         Parameters
         ----------
         query: list, np.ndarray
             The query vector.
@@ -170,14 +194,18 @@
         Returns
         -------
         A LanceQueryBuilder object representing the query.
         Once executed, the query returns selected columns, the vector,
         and also the "score" column which is the distance between the query
         vector and the returned vector.
         """
+        if isinstance(query, str):
+            # fts
+            return LanceFtsQueryBuilder(self, query)
+
         if isinstance(query, list):
             query = np.array(query)
         if isinstance(query, np.ndarray):
             query = query.astype(np.float32)
         else:
             raise TypeError(f"Unsupported query type: {type(query)}")
         return LanceQueryBuilder(self, query)
```

### Comparing `lancedb-0.1.2/lancedb/util.py` & `lancedb-0.1.3/lancedb/util.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.2/lancedb.egg-info/PKG-INFO` & `lancedb-0.1.3/lancedb.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.1.2
+Version: 0.1.3
 Summary: lancedb
 Author-email: LanceDB Devs <dev@lancedb.com>
 Project-URL: repository, https://github.com/eto-ai/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lancedb-0.1.2/pyproject.toml` & `lancedb-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "lancedb"
-version = "0.1.2"
-dependencies = ["pylance>=0.4.6", "ratelimiter", "retry", "tqdm"]
+version = "0.1.3"
+dependencies = ["pylance>=0.4.15", "ratelimiter", "retry", "tqdm"]
 description = "lancedb"
 authors = [
     { name = "LanceDB Devs", email = "dev@lancedb.com" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `lancedb-0.1.2/setup.py` & `lancedb-0.1.3/setup.py`

 * *Files identical despite different names*

