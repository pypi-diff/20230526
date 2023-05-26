# Comparing `tmp/ortoolpy-0.6.1-py3-none-any.whl.zip` & `tmp/ortoolpy-0.6.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 27780 bytes, number of entries: 8
+Zip file size: 27796 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     1216 b- defN 80-Jan-01 00:00 ortoolpy/__init__.py
 -rw-r--r--  2.0 unx     3325 b- defN 80-Jan-01 00:00 ortoolpy/cover_by_rect.py
--rw-r--r--  2.0 unx    50154 b- defN 80-Jan-01 00:00 ortoolpy/etc.py
+-rw-r--r--  2.0 unx    50134 b- defN 80-Jan-01 00:00 ortoolpy/etc.py
 -rw-r--r--  2.0 unx    28688 b- defN 80-Jan-01 00:00 ortoolpy/optimization/__init__.py
--rw-r--r--  2.0 unx    10757 b- defN 80-Jan-01 00:00 ortoolpy-0.6.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1552 b- defN 80-Jan-01 00:00 ortoolpy-0.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ortoolpy-0.6.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx      622 b- defN 16-Jan-01 00:00 ortoolpy-0.6.1.dist-info/RECORD
-8 files, 96402 bytes uncompressed, 26712 bytes compressed:  72.3%
+-rw-r--r--  2.0 unx    10763 b- defN 80-Jan-01 00:00 ortoolpy-0.6.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1552 b- defN 80-Jan-01 00:00 ortoolpy-0.6.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ortoolpy-0.6.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx      622 b- defN 16-Jan-01 00:00 ortoolpy-0.6.2.dist-info/RECORD
+8 files, 96388 bytes uncompressed, 26728 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: ortoolpy/etc.py
 Comment: 
 
 Filename: ortoolpy/optimization/__init__.py
 Comment: 
 
-Filename: ortoolpy-0.6.1.dist-info/LICENSE
+Filename: ortoolpy-0.6.2.dist-info/LICENSE
 Comment: 
 
-Filename: ortoolpy-0.6.1.dist-info/METADATA
+Filename: ortoolpy-0.6.2.dist-info/METADATA
 Comment: 
 
-Filename: ortoolpy-0.6.1.dist-info/WHEEL
+Filename: ortoolpy-0.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: ortoolpy-0.6.1.dist-info/RECORD
+Filename: ortoolpy-0.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ortoolpy/etc.py

```diff
@@ -1,12 +1,11 @@
-"""
-Copyright: 2015-2022 Saito Tsutomu
-License: Python Software Foundation License
-"""
+# Copyright: 2015-2023 Saito Tsutomu
+# License: Apache-2.0 License
 from collections import defaultdict
+from functools import lru_cache
 from math import ceil, sqrt
 from typing import Iterable, Tuple
 
 import numpy as np
 import pandas as pd
 from more_itertools import always_iterable, pairwise
 from pulp import (
@@ -1206,15 +1205,15 @@
     """
     facprd = [fac, prd]
     m = LpProblem()
     tbpr = tbfa[facprd].sort_values(facprd).drop_duplicates()
     tbdi2 = pd.merge(tbdi, tbpr, on=fac)
     tbdi2["VarX"] = addvars(tbdi2.shape[0])
     tbfa["VarY"] = addvars(tbfa.shape[0])
-    tbsm = pd.concat([tbdi2.groupby(facprd).VarX.sum(), tbfa.groupby(facprd).VarY.sum()], 1)
+    tbsm = pd.concat([tbdi2.groupby(facprd).VarX.sum(), tbfa.groupby(facprd).VarY.sum()], axis=1)
     tbde2 = pd.merge(tbde, tbdi2.groupby([dep, prd]).VarX.sum().reset_index())
     m += lpDot(tbdi2[tcs], tbdi2.VarX) + lpDot(tbfa[pcs], tbfa.VarY)
     tbsm.apply(lambda r: m.addConstraint(r.VarX <= r.VarY), 1)
     tbde2.apply(lambda r: m.addConstraint(r.VarX >= r[dem]), 1)
     if lwb in tbfa:
 
         def flwb(r):
@@ -1427,16 +1426,14 @@
     def fromkeys(iterable, value=None):
         return AutoCountDict(dict.fromkeys(iterable, value))
 
 
 class CacheDict:
     """Cached Dictionary"""
 
-    from functools import lru_cache
-
     def __init__(self, a=None):
         self._dct = {} if a is None else dict(a)
 
     @lru_cache(maxsize=2048)
     def __getitem__(self, k):
         return self._dct.__getitem__(k)
```

## Comparing `ortoolpy-0.6.1.dist-info/LICENSE` & `ortoolpy-0.6.2.dist-info/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -171,20 +171,20 @@
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
-   Copyright 2022 Saito Tsutomu
+   Copyright 2015-2023 Saito Tsutomu
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

## Comparing `ortoolpy-0.6.1.dist-info/METADATA` & `ortoolpy-0.6.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortoolpy
-Version: 0.6.1
+Version: 0.6.2
 Summary: `ortoolpy` is a package for Operations Research.
 Home-page: https://github.com/SaitoTsutomu/ortoolpy
 License: Apache-2.0
 Author: SaitoTsutomu
 Author-email: tsutomu7@hotmail.co.jp
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 1 - Planning
```

