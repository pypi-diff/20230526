# Comparing `tmp/pandas-indexing-0.2.6.tar.gz` & `tmp/pandas-indexing-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-indexing-0.2.6.tar", last modified: Thu May 25 16:41:15 2023, max compression
+gzip compressed data, was "pandas-indexing-0.2.7.tar", last modified: Fri May 26 20:05:07 2023, max compression
```

## Comparing `pandas-indexing-0.2.6.tar` & `pandas-indexing-0.2.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:41:15.975780 pandas-indexing-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-25 16:41:15.975780 pandas-indexing-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:41:15.967780 pandas-indexing-0.2.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:41:15.967780 pandas-indexing-0.2.6/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   362791 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/notebooks/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 16:41:15.975780 pandas-indexing-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:41:15.959780 pandas-indexing-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:41:15.971780 pandas-indexing-0.2.6/src/pandas_indexing/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (123)    20201 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:41:15.975780 pandas-indexing-0.2.6/src/pandas_indexing/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/datasets/remindhighre_power.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-25 16:40:57.000000 pandas-indexing-0.2.6/src/pandas_indexing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:41:15.971780 pandas-indexing-0.2.6/src/pandas_indexing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-25 16:41:15.000000 pandas-indexing-0.2.6/src/pandas_indexing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-25 16:41:15.000000 pandas-indexing-0.2.6/src/pandas_indexing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:41:15.000000 pandas-indexing-0.2.6/src/pandas_indexing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 16:41:15.000000 pandas-indexing-0.2.6/src/pandas_indexing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 16:41:15.000000 pandas-indexing-0.2.6/src/pandas_indexing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:05:07.290772 pandas-indexing-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-26 20:05:07.290772 pandas-indexing-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:05:07.282772 pandas-indexing-0.2.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:05:07.282772 pandas-indexing-0.2.7/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   362791 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/notebooks/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:05:07.290772 pandas-indexing-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:05:07.278771 pandas-indexing-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:05:07.286772 pandas-indexing-0.2.7/src/pandas_indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:05:07.290772 pandas-indexing-0.2.7/src/pandas_indexing/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/datasets/remindhighre_power.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:05:07.290772 pandas-indexing-0.2.7/src/pandas_indexing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-26 20:05:07.000000 pandas-indexing-0.2.7/src/pandas_indexing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-26 20:05:07.000000 pandas-indexing-0.2.7/src/pandas_indexing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:05:07.000000 pandas-indexing-0.2.7/src/pandas_indexing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-26 20:05:07.000000 pandas-indexing-0.2.7/src/pandas_indexing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 20:05:07.000000 pandas-indexing-0.2.7/src/pandas_indexing.egg-info/top_level.txt
```

### Comparing `pandas-indexing-0.2.6/CHANGELOG.rst` & `pandas-indexing-0.2.7/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 .. currentmodule:: pandas_indexing
 
 Changelog
 =========
 
+v0.2.7 (2023-06-26)
+------------------------------------------------------------
+* Compatibility release to re-include Python 3.8 support and fix CI testing
+* :func:`~accessors.IndexIdxAccessor.extract` gains single-level index support
+* Minimal doc improvements
+
 v0.2.6 (2023-05-25)
 ------------------------------------------------------------
 * :func:`~core.extractlevel` can be used on non-multiindex, like
-  f.ex. ``extractlevel(df, "{sector}|{gas}")`` :pull:`17`
+  f.ex. ``extractlevel(df, "{sector}|{gas}")`` :pull:`18`
 * :func:`~selectors.isin` accepts callable filters :pull:`16`, f.ex.
   ``df.loc[isin(year=lambda s: s>2000)]``
 * New function :func:`~core.concat` makes concatenation level aware :pull:`14`
 
 v0.2.5 (2023-05-04)
 ------------------------------------------------------------
 * :func:`~core.formatlevel` and :func:`~core.extractlevel` (or their equivalents
```

### Comparing `pandas-indexing-0.2.6/CODE_OF_CONDUCT.md` & `pandas-indexing-0.2.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.6/CONTRIBUTING.rst` & `pandas-indexing-0.2.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.6/LICENSE` & `pandas-indexing-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.6/PKG-INFO` & `pandas-indexing-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.2.6
+Version: 0.2.7
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
```

### Comparing `pandas-indexing-0.2.6/README.rst` & `pandas-indexing-0.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.6/docs/api.rst` & `pandas-indexing-0.2.7/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.6/docs/conf.py` & `pandas-indexing-0.2.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.6/docs/notebooks/introduction.ipynb` & `pandas-indexing-0.2.7/docs/notebooks/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.6/pyproject.toml` & `pandas-indexing-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.6/src/pandas_indexing/__init__.py` & `pandas-indexing-0.2.7/src/pandas_indexing/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 
 
 from importlib.metadata import version as _version
 
 from . import core, datasets
 from .arithmetics import add, divide, multiply, subtract
 from .core import (
-    alignlevel,
-    alignlevels,
     assignlevel,
     concat,
     describelevel,
     dropnalevel,
     extractlevel,
     formatlevel,
     index_names,
```

### Comparing `pandas-indexing-0.2.6/src/pandas_indexing/accessors.py` & `pandas-indexing-0.2.7/src/pandas_indexing/accessors.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,17 @@
         axis: Axis = 0,
         **labels: Any,
     ) -> Union[DataFrame, Series, MultiIndex]:
         return assignlevel(self._obj, frame=frame, order=order, axis=axis, **labels)
 
     @doc(extractlevel, index_or_data="")
     def extract(
-        self, axis: Axis = 0, **templates: str
+        self, template: Optional[str] = None, *, axis: Axis = 0, **templates: str
     ) -> Union[DataFrame, Series, Index]:
-        return extractlevel(self._obj, axis=axis, **templates)
+        return extractlevel(self._obj, template, axis=axis, **templates)
 
     @doc(formatlevel, index_or_data="")
     def format(
         self, axis: Axis = 0, **templates: str
     ) -> Union[DataFrame, Series, Index]:
         return formatlevel(self._obj, axis=axis, **templates)
```

### Comparing `pandas-indexing-0.2.6/src/pandas_indexing/arithmetics.py` & `pandas-indexing-0.2.7/src/pandas_indexing/arithmetics.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.6/src/pandas_indexing/core.py` & `pandas-indexing-0.2.7/src/pandas_indexing/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 """
 Core module.
 """
 import re
 from functools import reduce
 from itertools import chain
 from operator import and_, or_
-from typing import Any, Iterable, Literal, Mapping, Optional, Sequence, Tuple, Union
+from typing import (
+    Any,
+    Iterable,
+    List,
+    Literal,
+    Mapping,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
 
 import numpy as np
 import pandas as pd
 from deprecated import deprecated
 from pandas import DataFrame, Index, MultiIndex, Series
 from pandas.core.indexes.frozen import FrozenList
 
@@ -430,42 +440,14 @@
 def ensure_multiindex(s: T) -> T:
     if isinstance(s, Index):
         return _ensure_multiindex(s)
 
     return s.set_axis(_ensure_multiindex(s.index))
 
 
-def alignlevel(s, other):
-    names = index_names(
-        other,
-        raise_on_index=RuntimeError(
-            "For alignment, both indices must be of type MultiIndex"
-            "; use alignlevels instead."
-        ),
-    )
-    s_names = index_names(s)
-    if names.difference(s_names):
-        raise RuntimeError("Both indices need to be aligned; use alignlevels instead.")
-    return ensure_multiindex(s).reorder_levels(names.union(s_names.difference(names)))
-
-
-def alignlevels(l, r):
-    l_names = index_names(l)
-    r_names = index_names(r)
-
-    l_and_r = FrozenList([l for l in l_names if l in r_names])
-    l_but_not_r = l_names.difference(r_names)
-    r_but_not_l = r_names.difference(l_names)
-
-    return (
-        ensure_multiindex(l).reorder_levels(l_and_r.union(l_but_not_r)),
-        ensure_multiindex(r).reorder_levels(l_and_r.union(r_but_not_l)),
-    )
-
-
 @doc(
     frame_or_series="""
     frame_or_series : DataFrame or Series
         Data to be filtered\
     """
 )
 def semijoin(
@@ -495,16 +477,17 @@
 
     Returns
     -------
     DataFrame or Series
 
     Raises
     ------
+    ValueError
+        If axis is not 0, "index" or 1, "columns"
     TypeError
-        If axis is not 0 or 1, or
         if frame_or_series does not derive from DataFrame or Series
 
     See also
     --------
     pandas.Index.join
     """
 
@@ -546,20 +529,20 @@
     elif isinstance(frame_or_series, Series):
         data = np.where(left_idx != -1, frame_or_series.values[left_idx], np.nan)
     else:
         raise TypeError(
             f"frame_or_series must derive from DataFrame or Series, but is {type(frame_or_series)}"
         )
 
-    return cls(data, *axes).__finalize__(frame_or_series)
+    return cls(data, *axes).__finalize__(frame_or_series, method="semijoin")
 
 
 def _extractlevel(
     index: Index, template: Optional[str] = None, drop: bool = False, **templates: str
-) -> Tuple[Index, list[str]]:
+) -> Tuple[Index, List[str]]:
     index = ensure_multiindex(index)
     all_identifiers = set()
 
     if template is not None:
         if len(index.names) > 1:
             raise ValueError("``template`` may only be non-null for single index level")
         templates[index.names[0]] = template
```

### Comparing `pandas-indexing-0.2.6/src/pandas_indexing/datasets/__init__.py` & `pandas-indexing-0.2.7/src/pandas_indexing/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.6/src/pandas_indexing/datasets/remindhighre_power.csv` & `pandas-indexing-0.2.7/src/pandas_indexing/datasets/remindhighre_power.csv`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.6/src/pandas_indexing/selectors.py` & `pandas-indexing-0.2.7/src/pandas_indexing/selectors.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.6/src/pandas_indexing/utils.py` & `pandas-indexing-0.2.7/src/pandas_indexing/utils.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.6/src/pandas_indexing.egg-info/PKG-INFO` & `pandas-indexing-0.2.7/src/pandas_indexing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.2.6
+Version: 0.2.7
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
```

### Comparing `pandas-indexing-0.2.6/src/pandas_indexing.egg-info/SOURCES.txt` & `pandas-indexing-0.2.7/src/pandas_indexing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

