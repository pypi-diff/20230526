# Comparing `tmp/act4e_mcdp-0.3.7-py3-none-any.whl.zip` & `tmp/act4e_mcdp-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,16 @@
-Zip file size: 6362 bytes, number of entries: 10
--rw-r--r--  2.0 unx      275 b- defN 80-Jan-01 00:00 act4e_mcdp/__init__.py
--rw-r--r--  2.0 unx     8426 b- defN 80-Jan-01 00:00 act4e_mcdp/loading.py
--rw-r--r--  2.0 unx     3018 b- defN 80-Jan-01 00:00 act4e_mcdp/main.py
+Zip file size: 20739 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      347 b- defN 80-Jan-01 00:00 act4e_mcdp/__init__.py
+-rw-r--r--  2.0 unx    27668 b- defN 80-Jan-01 00:00 act4e_mcdp/autogen_packed_test_data.py
+-rw-r--r--  2.0 unx      571 b- defN 80-Jan-01 00:00 act4e_mcdp/download.py
+-rw-r--r--  2.0 unx     8457 b- defN 80-Jan-01 00:00 act4e_mcdp/loading.py
+-rw-r--r--  2.0 unx     3363 b- defN 80-Jan-01 00:00 act4e_mcdp/main.py
+-rw-r--r--  2.0 unx     4381 b- defN 80-Jan-01 00:00 act4e_mcdp/nameddps.py
+-rw-r--r--  2.0 unx     1790 b- defN 80-Jan-01 00:00 act4e_mcdp/posets.py
+-rw-r--r--  2.0 unx     8747 b- defN 80-Jan-01 00:00 act4e_mcdp/primitivedps.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 act4e_mcdp/py.typed
--rw-r--r--  2.0 unx      729 b- defN 80-Jan-01 00:00 act4e_mcdp/solution_interface.py
--rw-r--r--  2.0 unx     3239 b- defN 80-Jan-01 00:00 act4e_mcdp/structures.py
--rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 act4e_mcdp-0.3.7.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.3.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       58 b- defN 80-Jan-01 00:00 act4e_mcdp-0.3.7.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      785 b- defN 16-Jan-01 00:00 act4e_mcdp-0.3.7.dist-info/RECORD
-10 files, 16979 bytes uncompressed, 5022 bytes compressed:  70.4%
+-rw-r--r--  2.0 unx     3944 b- defN 80-Jan-01 00:00 act4e_mcdp/solution_interface.py
+-rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      109 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1119 b- defN 16-Jan-01 00:00 act4e_mcdp-0.4.0.dist-info/RECORD
+14 files, 60945 bytes uncompressed, 18887 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -1,31 +1,43 @@
 Filename: act4e_mcdp/__init__.py
 Comment: 
 
+Filename: act4e_mcdp/autogen_packed_test_data.py
+Comment: 
+
+Filename: act4e_mcdp/download.py
+Comment: 
+
 Filename: act4e_mcdp/loading.py
 Comment: 
 
 Filename: act4e_mcdp/main.py
 Comment: 
 
-Filename: act4e_mcdp/py.typed
+Filename: act4e_mcdp/nameddps.py
 Comment: 
 
-Filename: act4e_mcdp/solution_interface.py
+Filename: act4e_mcdp/posets.py
 Comment: 
 
-Filename: act4e_mcdp/structures.py
+Filename: act4e_mcdp/primitivedps.py
+Comment: 
+
+Filename: act4e_mcdp/py.typed
+Comment: 
+
+Filename: act4e_mcdp/solution_interface.py
 Comment: 
 
-Filename: act4e_mcdp-0.3.7.dist-info/METADATA
+Filename: act4e_mcdp-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: act4e_mcdp-0.3.7.dist-info/WHEEL
+Filename: act4e_mcdp-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: act4e_mcdp-0.3.7.dist-info/entry_points.txt
+Filename: act4e_mcdp-0.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: act4e_mcdp-0.3.7.dist-info/RECORD
+Filename: act4e_mcdp-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## act4e_mcdp/__init__.py

```diff
@@ -6,10 +6,13 @@
 
 logger = getLogger(__name__)
 logger.setLevel(DEBUG)
 
 # __version__ = "0.2.1"
 
 from .loading import *
-from .structures import *
 from .main import *
 from .solution_interface import *
+from .nameddps import *
+from .primitivedps import *
+from .posets import *
+from .download import *
```

## act4e_mcdp/loading.py

```diff
@@ -1,40 +1,39 @@
 from decimal import Decimal
 from typing import Optional, Type, TypeVar
 
 import yaml
 
 from . import logger
-from .structures import (
-    AmbientConversion,
+from .nameddps import (
     CompositeNamedDP,
     Connection,
+    ModelFunctionality,
+    ModelResource,
+    NodeFunctionality,
+    NodeResource,
+    SimpleWrap,
+)
+from .posets import FinitePoset, Numbers, Poset, PosetProduct
+from .primitivedps import (
+    AmbientConversion,
     DPSeries,
-    FinitePoset,
     JoinNDP,
     M_Ceil_DP,
     M_FloorFun_DP,
     M_Fun_AddConstant_DP,
     M_Fun_AddMany_DP,
     M_Fun_MultiplyConstant_DP,
     M_Fun_MultiplyMany_DP,
     M_Res_AddConstant_DP,
     M_Res_AddMany_DP,
     M_Res_MultiplyConstant_DP,
     M_Res_MultiplyMany_DP,
     MeetNDualDP,
-    ModelFunctionality,
-    ModelResource,
-    NodeFunctionality,
-    NodeResource,
-    Numbers,
-    Poset,
-    PosetProduct,
     PrimitiveDP,
-    SimpleWrap,
     UnitConversion,
     ValueFromPoset,
 )
 
 loaders = {}
 
 __all__ = [
```

## act4e_mcdp/main.py

```diff
@@ -3,16 +3,16 @@
 import sys
 from importlib import import_module
 
 import yaml
 
 from . import logger
 from .loading import load_repr1, parse_yaml_value
-from .solution_interface import SolutionInterface
-from .structures import NamedDP
+from .solution_interface import SolverInterface
+from .nameddps import NamedDP
 
 
 def import_from_string(dot_path: str) -> object:
     module_path, _, name = dot_path.rpartition(".")
     module = import_module(module_path)
     return getattr(module, name)
 
@@ -33,35 +33,45 @@
     model_source = args.model
     try:
         solver0 = import_from_string(args.solver)
     except Exception as e:
         logger.error("Could not import solver %r", args.solver, exc_info=e)
         sys.exit(1)
 
-    solver: SolutionInterface
+    solver: SolverInterface
 
-    if isinstance(solver0, SolutionInterface):
+    if isinstance(solver0, SolverInterface):
         solver = solver0
     else:
         solver = solver0()  # type: ignore
 
     query = args.query
 
     if query not in queries:
         logger.error("Unknown query %r. Known: %r", query, queries)
         sys.exit(1)
 
     query_data = args.data
+    if model_source.startswith("http"):
+        import requests
 
-    if os.path.exists(model_source):
-        model_source = open(model_source).read()
+        r = requests.get(model_source)
+        if r.status_code != 200:
+            logger.error("Cannot download model from %r", model_source)
+            sys.exit(1)
+
+        model_source = r.text
         data = yaml.load(model_source, Loader=yaml.SafeLoader)
     else:
-        logger.error("URL not implemented yet: %r", model_source)
-        sys.exit(1)
+        if os.path.exists(model_source):
+            model_source = open(model_source).read()
+            data = yaml.load(model_source, Loader=yaml.SafeLoader)
+        else:
+            logger.error("Cannot open file: %r", model_source)
+            sys.exit(1)
 
     model = load_repr1(data, NamedDP)
     logger.info("model: %s", model)
 
     yaml_query = yaml.load(query_data, Loader=yaml.SafeLoader)
     if not isinstance(yaml_query, dict):
         raise ValueError(f"Expected dict, got {yaml_query!r}")
```

## act4e_mcdp/solution_interface.py

```diff
@@ -1,29 +1,146 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Any, Collection, Generic, Mapping, TypeVar
+from typing import Any, Generic, Mapping, TypeVar
 
-from .structures import NamedDP
+from .nameddps import NamedDP
 
-__all__ = ["LowerSet", "SolutionInterface", "UpperSet"]
+__all__ = ["LowerSet", "SolverInterface", "UpperSet"]
 
 X = TypeVar("X")
 
 
 @dataclass
 class UpperSet(Generic[X]):
-    minima: Collection[X]
+    """
+    Describes a finitely-supported **upper set** of elements of type X.
+
+    Attributes:
+        minima: A list of elements of type X, which are the minimal elements of the set.
+
+    """
+
+    minima: list[X]
 
 
 @dataclass
 class LowerSet(Generic[X]):
-    maxima: Collection[X]
+    """
+    Describes a finitely-supported **lower set** of elements of type X.
+
+    Attributes:
+        maxima: A list of elements of type X, which are the minimal elements of the set.
+
+    """
+
+    maxima: list[X]
 
 
-class SolutionInterface(ABC):
+class SolverInterface(ABC):
+    """
+    An abstract class that describes the interface of a solver.
+
+    """
+
     @abstractmethod
-    def solve_FixFunMinRes(self, model: NamedDP, query: Mapping[str, Any]) -> UpperSet[Mapping[str, Any]]:
+    def solve_FixFunMinRes(
+        self, model: NamedDP, functionality_needed: Mapping[str, Any], /
+    ) -> UpperSet[Mapping[str, Any]]:
+        """
+
+        Solves the problem of finding the minimal resources needed to satisfy a given functional requirement.
+
+        The problem is defined by a model and a query. The model is a NamedDP, and the query is a mapping from
+        the names of the resources to the values of the resources.
+
+        The solution is a finitely-supported upper set.
+
+
+        For example, this is what we expect from a solver for the empty model:
+
+        ```python
+
+            solver: SolverInterface = ...
+
+            empty = CompositeNamedDP(functionalities={}, resources={}, nodes={}, connections=[])
+
+            result: UpperSet = solver.solve_FixFunMinRes(empty, {})
+
+            # We expect that the result is a list containing the empty dictionary
+
+            assert list(result.minima) == [{}]
+
+        ```
+
+        In a more complex example, we can have a model describing the identity:
+
+        ```python
+
+            solver: SolverInterface = ...
+
+            P = FinitePoset({'a', 'b'}, {('a', 'b')})
+
+            identity = CompositeNamedDP(
+                functionalities={'f1': P},
+                resources={'r1': P},
+                nodes={},
+                connections=[
+                    Connection(
+                        source=ModelFunctionality('f1'),
+                        target=ModelResource('r1')
+                    )]
+            )
+
+            result: UpperSet = solver.solve_FixFunMinRes(identity, {'f1': 'a'})
+
+            # We expect that the result is a list containing only one element
+
+            assert list(result.minima) == [{'r1': 'a'}]
+        ```
+
+
+        Parameters:
+            model: The model of the problem.
+            functionality_needed: The functionality needed (key-value dictionary).
+
+        Returns:
+
+            A finitely-supported upper set of resources.
+        """
         raise NotImplementedError
 
     @abstractmethod
-    def solve_FixResMaxFun(self, model: NamedDP, query: Mapping[str, Any]) -> LowerSet[Mapping[str, Any]]:
+    def solve_FixResMaxFun(
+        self, model: NamedDP, resources_budget: Mapping[str, Any], /
+    ) -> LowerSet[Mapping[str, Any]]:
+        """
+        This is the dual of solve_FixFunMinRes. It solves the problem of finding the maximal functionality
+        that can be provided with a given budget of resources.
+
+
+        For example, this is what we expect from a solver for the empty model:
+
+        ```python
+
+            solver: SolverInterface = ...
+
+            empty = CompositeNamedDP(functionalities={}, resources={}, nodes={}, connections=[])
+
+            result: LowerSet = solver.solve_FixResMaxFun(empty, {})
+
+            # We expect that the result is a list containing the empty dictionary
+
+            assert list(result.maxima) == [{}]
+
+        ```
+
+        Parameters:
+            model: The model of the problem.
+            resources_budget: The maximum budget that we have (key-value dictionary).
+
+        Returns:
+
+            A finitely-supported upper set of resources.
+
+
+        """
         raise NotImplementedError
```

## Comparing `act4e_mcdp-0.3.7.dist-info/RECORD` & `act4e_mcdp-0.4.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-act4e_mcdp/__init__.py,sha256=JWTYSE98iP09iyikVZvXH56EkuuyUbAonMxHbKnSJcQ,275
-act4e_mcdp/loading.py,sha256=dGRBzIsjeJEEAoW9dvJ8N1pa58CTLx-Wq2kGTS-aX4M,8426
-act4e_mcdp/main.py,sha256=P93v6jFVfeeD-CePlZa0yCdmm2KwRkK3asDeabv1Ezw,3018
+act4e_mcdp/__init__.py,sha256=E_ujpgzc-ou4a5DKP7fNLO7NZVky0K3bl5mp2ob3ahU,347
+act4e_mcdp/autogen_packed_test_data.py,sha256=74ahEQkoC9jnCsNsZCAft34NJPHHQER3j8T1Bij86iM,27668
+act4e_mcdp/download.py,sha256=fXm46ISIYvpFjouSMB0l0XLuJWw5CxZSpgi-fvmxMGA,571
+act4e_mcdp/loading.py,sha256=yvLGVxHk08lr7WB_SWMAs8A5IjonRugKOLsuRHXE_9g,8457
+act4e_mcdp/main.py,sha256=c_Fy0nmJrrikwDQpdv_y0shFrH3AHg1auOdk1Dsc_Hs,3363
+act4e_mcdp/nameddps.py,sha256=OaYt-P9pGt6TQa9oXWWHZI4PFRt9kPyfQatPEx9rH60,4381
+act4e_mcdp/posets.py,sha256=7iijB7waZd3nTyK-_eNBR6YZOWhcTUYtKqCm7irpFKE,1790
+act4e_mcdp/primitivedps.py,sha256=2STRQwuMGDbh_jE7WYBWoOq4evMjUiqyf0Bc6c82sWY,8747
 act4e_mcdp/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-act4e_mcdp/solution_interface.py,sha256=mwhfSGZlZSfufKdQn5qpho16dfOW4-tI1ZP0IVgqTRk,729
-act4e_mcdp/structures.py,sha256=n9kCF82W82eqqquWWv2txi2nTfy5FPDWRvh7T-FyXK0,3239
-act4e_mcdp-0.3.7.dist-info/METADATA,sha256=t1lmyU8oRdDQUmnvFcam4Rl8AuO4jJZMgtETXvsOKJk,361
-act4e_mcdp-0.3.7.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-act4e_mcdp-0.3.7.dist-info/entry_points.txt,sha256=cfj1OzFHMtFmK8Wl5Ulxkv9yficQNQ60fnULm1eq70w,58
-act4e_mcdp-0.3.7.dist-info/RECORD,,
+act4e_mcdp/solution_interface.py,sha256=7TjPbeJKbZ_29c1l5eW-TlWQEP0TxEl9I9JclJY9pi4,3944
+act4e_mcdp-0.4.0.dist-info/METADATA,sha256=qujNtxFrBz2w8T4r5tf81OUNTgbA6kZvfRQDWhYZ4eQ,361
+act4e_mcdp-0.4.0.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+act4e_mcdp-0.4.0.dist-info/entry_points.txt,sha256=ab4CbY_rBOTC8YJBuIQeKxZExEYTrXx6fDsX1GivxXo,109
+act4e_mcdp-0.4.0.dist-info/RECORD,,
```

