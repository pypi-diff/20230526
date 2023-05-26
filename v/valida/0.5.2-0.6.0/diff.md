# Comparing `tmp/valida-0.5.2.tar.gz` & `tmp/valida-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valida-0.5.2.tar", max compression
+gzip compressed data, was "valida-0.6.0.tar", max compression
```

## Comparing `valida-0.5.2.tar` & `valida-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-04-25 11:25:07.571026 valida-0.5.2/LICENSE
--rw-r--r--   0        0        0     1439 2023-04-25 11:25:07.571026 valida-0.5.2/README.md
--rw-r--r--   0        0        0      720 2023-04-25 11:25:07.575026 valida-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      200 2023-04-25 11:25:07.575026 valida-0.5.2/valida/__init__.py
--rw-r--r--   0        0        0     2903 2023-04-25 11:25:07.575026 valida-0.5.2/valida/callables.py
--rw-r--r--   0        0        0      353 2023-04-25 11:25:07.575026 valida-0.5.2/valida/casting.py
--rw-r--r--   0        0        0    27447 2023-04-25 11:25:07.575026 valida-0.5.2/valida/conditions.py
--rw-r--r--   0        0        0    10524 2023-04-25 11:25:07.575026 valida-0.5.2/valida/data.py
--rw-r--r--   0        0        0    27707 2023-04-25 11:25:07.575026 valida-0.5.2/valida/datapath.py
--rw-r--r--   0        0        0      485 2023-04-25 11:25:07.575026 valida-0.5.2/valida/errors.py
--rw-r--r--   0        0        0     6560 2023-04-25 11:25:07.575026 valida-0.5.2/valida/rules.py
--rw-r--r--   0        0        0     3885 2023-04-25 11:25:07.575026 valida-0.5.2/valida/schema.py
--rw-r--r--   0        0        0      869 2023-04-25 11:25:07.575026 valida-0.5.2/valida/utils.py
--rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 valida-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-26 19:36:42.603934 valida-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1439 2023-05-26 19:36:42.603934 valida-0.6.0/README.md
+-rw-r--r--   0        0        0      720 2023-05-26 19:36:42.607935 valida-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      200 2023-05-26 19:36:42.607935 valida-0.6.0/valida/__init__.py
+-rw-r--r--   0        0        0     3015 2023-05-26 19:36:42.607935 valida-0.6.0/valida/callables.py
+-rw-r--r--   0        0        0      353 2023-05-26 19:36:42.607935 valida-0.6.0/valida/casting.py
+-rw-r--r--   0        0        0    31469 2023-05-26 19:36:42.607935 valida-0.6.0/valida/conditions.py
+-rw-r--r--   0        0        0    10524 2023-05-26 19:36:42.607935 valida-0.6.0/valida/data.py
+-rw-r--r--   0        0        0    29661 2023-05-26 19:36:42.607935 valida-0.6.0/valida/datapath.py
+-rw-r--r--   0        0        0      485 2023-05-26 19:36:42.607935 valida-0.6.0/valida/errors.py
+-rw-r--r--   0        0        0     6888 2023-05-26 19:36:42.607935 valida-0.6.0/valida/rules.py
+-rw-r--r--   0        0        0    14363 2023-05-26 19:36:42.607935 valida-0.6.0/valida/schema.py
+-rw-r--r--   0        0        0      968 2023-05-26 19:36:42.607935 valida-0.6.0/valida/utils.py
+-rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 valida-0.6.0/PKG-INFO
```

### Comparing `valida-0.5.2/LICENSE` & `valida-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `valida-0.5.2/README.md` & `valida-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `valida-0.5.2/valida/callables.py` & `valida-0.6.0/valida/callables.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,18 @@
     return keys_contain_at_most_N_of(trial_dict, 1, keys)
 
 
 def keys_equal_to(trial_dict, *keys):
     return set(trial_dict.keys()) == set(keys)
 
 
+def keys_is_instance(trial_dict, *classes):
+    return all(isinstance(i, classes) for i in trial_dict.keys())
+
+
 def items_contain(trial_dict, **items):
     for k, v in items.items():
         try:
             if trial_dict[k] != v:
                 return False
         except KeyError:
             return False
```

### Comparing `valida-0.5.2/valida/conditions.py` & `valida-0.6.0/valida/conditions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from __future__ import annotations
+import copy
+
 import enum
+from typing import Dict, List
 import operator
 import pathlib
-from subprocess import call
 import warnings
 
 
 import valida.data
 import valida.datapath
 from valida import callables as call_funcs
 from valida.errors import (
@@ -15,14 +18,24 @@
 )
 from valida.utils import (
     classproperty,
     get_func_args_by_kind,
     null_condition_binary_check,
 )
 
+INV_DTYPE_LOOKUP = {
+    int: "int",
+    float: "float",
+    str: "str",
+    list: "list",
+    dict: "dict",
+    bool: "bool",
+    pathlib.Path: "path",
+}
+
 
 class PreparedConditionCallable:
     def __init__(self, func, *args, **kwargs):
         self._func = func
         self._args = args
         self._kwargs = kwargs
 
@@ -188,14 +201,18 @@
         return cls(call_funcs.keys_contain_at_most_one_of, keys=keys)
 
     @classmethod
     def keys_equal_to(cls, *keys):
         return cls(call_funcs.keys_equal_to, *keys)
 
     @classmethod
+    def keys_is_instance(cls, *classes):
+        return cls(call_funcs.keys_is_instance, *classes)
+
+    @classmethod
     def items_contain(cls, **items):
         return cls(call_funcs.items_contain, **items)
 
     @classmethod
     def allowed_keys(cls, *keys):
         return cls(call_funcs.allowed_keys, *keys)
 
@@ -270,15 +287,14 @@
         except AttributeError:
             all_cnds.append(self)
 
         return all_cnds, all_ops
 
     @staticmethod
     def from_spec(spec):
-
         if not spec:
             return NullCondition()
         elif not isinstance(spec, dict):
             raise TypeError("`spec` must be a dict with a single item.")
 
         BINARY_OPS = {
             "and": ConditionAnd,
@@ -344,15 +360,14 @@
 
             condition_like = NullCondition()
             for i in spec_val:
                 i_obj = ConditionLike.from_spec(i)
                 condition_like = cls(condition_like, i_obj)
 
         elif spec_key_split[0] in CONDITION_DATUM_TYPES:
-
             if (
                 spec_key_split_len not in [2, 3]
                 or spec_key_split_len == 2
                 and spec_key_split[-1] in ALL_PRE_PROCS
             ):
                 raise MalformedConditionLikeSpec(
                     f"Condition specification must be a dot-delimited string with either "
@@ -362,15 +377,14 @@
                 )
 
             condition_type_str = spec_key_split[0]
             cls = CONDITION_DATUM_TYPES[condition_type_str]
             pre_proc_str = None
 
             if spec_key_split_len == 3:
-
                 try:
                     pre_proc_str = spec_key_split[1]
                     pre_proc_str = PRE_PROC_LOOKUP.get(pre_proc_str, pre_proc_str)
                     if pre_proc_str == "dtype":
                         try:
                             # convert strings to types
                             if isinstance(spec_val, list):
@@ -398,15 +412,15 @@
                         f'Available pre-processors are "length" and "type"/"dtype", but '
                         f"not all pre-processors are applicable to all condition types."
                     )
 
             cond_call_str = spec_key_split[-1]
             cond_call_str = CALLABLE_LOOKUP.get(cond_call_str, cond_call_str)
             # special case:
-            if cond_call_str == "is_instance":
+            if cond_call_str in ["is_instance", "keys_is_instance"]:
                 try:
                     # convert strings to types
                     if isinstance(spec_val, list):
                         spec_val = [
                             DTYPE_LOOKUP[i.lower() if isinstance(i, str) else i]
                             for i in spec_val
                         ]
@@ -477,15 +491,15 @@
                 # More than one positional-or-keyword, and no other kinds:
                 if isinstance(spec_val, dict):
                     condition = cond_method(**spec_val)
                 elif isinstance(spec_val, (list, tuple)):
                     condition = cond_method(*spec_val)
                 else:
                     raise MalformedConditionLikeSpec(
-                        f"Condition callable {cond_method} accepts multuple positional-or-"
+                        f"Condition callable {cond_method} accepts multiple positional-or-"
                         f"keyword arguments, and so must be parametrised with a dict or "
                         f"list/tuple of values, but the following was supplied: {spec_val!r}"
                     )
 
             elif len(func_args["VAR_POSITIONAL"]) == 1 and not any(
                 func_args[i] for i in ("POSITIONAL_OR_KEYWORD", "VAR_KEYWORD")
             ):
@@ -526,17 +540,46 @@
 
         return condition_like
 
     @classmethod
     def from_json_like(cls, json_like, *args, **kwargs):
         return cls.from_spec(json_like)
 
+    def get_always_applicable_key_conditions(self) -> List[Condition]:
+        """Get `allowed_keys` and `required_keys` conditions that always apply."""
+        out = []
+        conditions, binary_ops = self.flatten()
+        if not binary_ops or set(binary_ops) == {"and"}:
+            for i in conditions:
+                if i.callable.name in ("allowed_keys", "required_keys"):
+                    out.append(i)
+        return out
 
-class Condition(ConditionLike):
+    def get_always_applicable_type_like_conditions(
+        self,
+    ) -> Dict[str, List[Condition]]:
+        """Get `KeyDataType` and `ValueDataType` conditions that always apply."""
+        out = {"key_data_type": [], "value_data_type": []}
+        conditions, binary_ops = self.flatten()
+        if not binary_ops or set(binary_ops) == {"and"}:
+            for i in conditions:
+                if isinstance(i, KeyDataType):
+                    out["key_data_type"].append(i)
+                elif isinstance(i, ValueDataType):
+                    out["value_data_type"].append(i)
+                elif isinstance(i, Value) and i.callable.name == "is_instance":
+                    out["value_data_type"].append(i)
+                elif isinstance(i, Value) and i.callable.name == "in_":
+                    out["value_data_type"].append(i)
+                elif isinstance(i, Value) and i.callable.name == "keys_is_instance":
+                    out["key_data_type"].append(i)
+        return out
 
+
+class Condition(ConditionLike):
     PRE_PROCESSOR = None
 
     def __init__(self, callable, *args, **kwargs):
         """
         Parameters
         ----------
         callable : Callable
@@ -547,15 +590,14 @@
             Callable keyword arguments.
 
         """
 
         self.callable = PreparedConditionCallable(callable, *args, **kwargs)
 
     def __repr__(self):
-
         out = f"{self.__class__.__name__}.{self.callable.name}"
         args = [f"{v!r}" for v in self.callable.args] + [
             f"{k}={v!r}" for k, v in self.callable.kwargs.items()
         ]
         out += "(" + ", ".join(args) + ")"
 
         return out
@@ -570,21 +612,19 @@
         return (
             self.callable.name,
             self.callable.args,
             self.callable.kwargs,
         )
 
     def _filter(self, data, data_has_paths=False, source_data=None):
-
         processed = []
         pre_processor_error = []
         callable_error = []
         callable_false = []
         for datum in getattr(data, self.DATUM_TYPE.value)():
-
             if data_has_paths:
                 datum, _ = datum
 
             try:
                 processed_i = self.PRE_PROCESSOR(datum) if self.PRE_PROCESSOR else datum
                 is_valid_i = True
                 pre_processor_error_i = False
@@ -592,15 +632,14 @@
                 processed_i = None
                 is_valid_i = False
                 pre_processor_error_i = True
 
             callable_error_i = False
             callable_false_i = False
             if is_valid_i:
-
                 try:
                     result_i = self.callable(processed_i, source_data=source_data)
 
                     if not isinstance(result_i, bool):
                         raise InvalidCallable(
                             f"Callable {self.callable} did not return a boolean."
                         )
@@ -625,41 +664,85 @@
             data_has_paths=data_has_paths,
         )
 
     def to_json_like(self, *args, **kwargs):
         # need to return a single-item dict that can be passed to `from_spec` for
         # round-tripping.
 
-        INV_DTYPE_LOOKUP = {
-            int: "int",
-            float: "float",
-            str: "str",
-            list: "list",
-            dict: "dict",
-            bool: "bool",
-            pathlib.Path: "path",
-        }
-
-        # TODO: doesn't work for BinaryOps?
+        # Get the spec key:
         key = f"{self.js_like_label}.{self.callable.func.__name__}"
 
-        if len(self.callable.kwargs) == 1:
-            _, val = next(iter(self.callable.kwargs.items()))
-            if "dtype" in key:
-                val = INV_DTYPE_LOOKUP[val]
+        cast_types = "dtype" in key or "is_instance" in key
 
-        out = {key: val}
+        # Get the spec value (the value of the returned dict):
+
+        func_args = get_func_args_by_kind(self.callable.func, exclude_first=True)
+        if not any(
+            func_args[i]
+            for i in ("POSITIONAL_OR_KEYWORD", "VAR_POSITIONAL", "VAR_KEYWORD")
+        ):
+            # no arguments, set spec val to None
+            spec_val = None
+
+        elif len(func_args["POSITIONAL_OR_KEYWORD"]) == 1 and not any(
+            func_args[i] for i in ("VAR_POSITIONAL", "VAR_KEYWORD")
+        ):
+            # single pos-or-kw and nothing else, spec val is just that single value:
+            spec_val = copy.deepcopy(next(iter(self.callable.kwargs.values())))
+            if cast_types:
+                spec_val = INV_DTYPE_LOOKUP[spec_val]
+
+        elif len(func_args["POSITIONAL_OR_KEYWORD"]) > 1 and not any(
+            func_args[i] for i in ("VAR_POSITIONAL", "VAR_KEYWORD")
+        ):
+            # more than one pos-or-kw and nothing else, spec val is a dict of kwargs:
+            spec_val = copy.deepcopy(self.callable.kwargs)
+            if cast_types:
+                for k, v in spec_val.items():
+                    try:
+                        spec_val[k] = INV_DTYPE_LOOKUP[v]
+                    except KeyError:
+                        continue
+
+        elif len(func_args["VAR_POSITIONAL"]) == 1 and not any(
+            func_args[i] for i in ("POSITIONAL_OR_KEYWORD", "VAR_KEYWORD")
+        ):
+            # one var-positional and nothing else, spec val is a list of args:
+            spec_val = copy.deepcopy(list(self.callable.args))
+            if cast_types:
+                for idx, val in enumerate(spec_val):
+                    try:
+                        spec_val[idx] = INV_DTYPE_LOOKUP[val]
+                    except KeyError:
+                        continue
+
+        elif len(func_args["VAR_KEYWORD"]) == 1 and not func_args["VAR_POSITIONAL"]:
+            # zero or more pos-or-kw args and a var-kw arg, spec val is a dict of kwargs:
+            spec_val = copy.deepcopy(self.callable.kwargs)
+            if cast_types:
+                for k, v in spec_val.items():
+                    try:
+                        spec_val[k] = INV_DTYPE_LOOKUP[v]
+                    except KeyError:
+                        continue
+
+        else:
+            raise NotImplementedError(
+                f"Condition callable arguments {self.callable.ags!r} and keyword-arguments "
+                f"{self.callable.kwargs!r} cannot be written in JSON form."
+            )
+
+        out = {key: spec_val}
         if "shared_data" in kwargs:
             return out, kwargs["shared_data"]
         else:
             return out
 
 
 class FilterDatumType(enum.Enum):
-
     KEYS = "keys"
     VALUES = "values"
 
 
 class NullCondition(Condition):
     """Class to represent a null condition that all data satisfies."""
 
@@ -681,15 +764,14 @@
 class ConditionBinaryOp(ConditionLike):
     def __new__(cls, *conditions):
         """If one of the conditions is a NullCondition, then abort object construction,
         and just return the non-null condition."""
         return null_condition_binary_check(*conditions) or super().__new__(cls)
 
     def __init__(self, *conditions):
-
         super().__init__()
 
         self.children = conditions
 
         # Nonsensical to combine key-like and index-like conditions:
         flattened_conds = self.flatten()[0]
         num_key_likes = sum(isinstance(i, KeyLike) for i in flattened_conds)
@@ -711,28 +793,30 @@
                 and self.children[1] == other.children[0]
             )
         ):
             return True
         return False
 
     def _filter(self, data, binary_op, data_has_paths=False, source_data=None):
-
         if data_has_paths:
             # Data paths will be removed on the first child _filter:
             data_has_paths = [True, False]
         else:
             data_has_paths = [False, False]
 
         return binary_op(
             *(
                 i._filter(data, data_has_paths[idx], source_data=source_data)
                 for idx, i in enumerate(self.children)
             )
         )
 
+    def to_json_like(self):
+        return {self.FLATTEN_SYMBOL: [i.to_json_like() for i in self.children]}
+
 
 class ConditionAnd(ConditionBinaryOp):
     FLATTEN_SYMBOL = "and"
 
     def _filter(self, data, data_has_paths=False, source_data=None):
         return super()._filter(
             data, operator.and_, data_has_paths=data_has_paths, source_data=source_data
@@ -769,15 +853,14 @@
     DATUM_TYPE = FilterDatumType.VALUES
 
 
 class KeyLike(Condition):
     DATUM_TYPE = FilterDatumType.KEYS
 
     def filter(self, data, data_has_paths=False, source_data=None):
-
         if (isinstance(data, valida.data.Data) and data.is_list) or not isinstance(
             data, (valida.data.Data, dict)
         ):
             raise TypeError("`Key` condition can only filter a mapping (i.e. a dict).")
 
         return super().filter(
             data, data_has_paths=data_has_paths, source_data=source_data
@@ -790,15 +873,14 @@
         return self.filter(datum).result[0]
 
 
 class IndexLike(Condition):
     DATUM_TYPE = FilterDatumType.KEYS
 
     def filter(self, data, data_has_paths=False, source_data=None):
-
         if (isinstance(data, valida.data.Data) and not data.is_list) or not isinstance(
             data, (valida.data.Data, list)
         ):
             raise TypeError("`Index` condition can only filter a list.")
         return super().filter(
             data, data_has_paths=data_has_paths, source_data=source_data
         )
```

### Comparing `valida-0.5.2/valida/data.py` & `valida-0.6.0/valida/data.py`

 * *Files identical despite different names*

### Comparing `valida-0.5.2/valida/datapath.py` & `valida-0.6.0/valida/datapath.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import enum
+from typing import Tuple
 
 import valida.data
 import valida.conditions as cnds
 from valida.errors import (
     DuplicateRule,
     IncompatibleRules,
     MalformedDataPathSpec,
@@ -14,15 +15,14 @@
     condition,
     datum_condition,
     cls,
     cls_like,
     condition_label="condition",
     datum_condition_label="value",
 ):
-
     if condition is not None:
         if not isinstance(condition, cnds.ConditionLike):
             raise TypeError(
                 f"If specified, `{condition_label}` must be a cnds.ConditionLike object."
             )
     else:
         condition = cnds.NullCondition()
@@ -37,68 +37,64 @@
                 )
         condition = condition & datum_condition
 
     return condition
 
 
 class Container(enum.Enum):
-
     CONTAINER = -1
     LIST = 0
     MAP = 1
 
 
 class DataPathDatumType(enum.Enum):
-
     NONE = None
     DTYPE = 1
     LENGTH = 2
     MAP_KEYS = 3
     MAP_VALUES = 4
 
 
 class DataPathMultiType(enum.Enum):
-
     NONE = None
     FIRST = 1  # Use just the first returned match
     LAST = 2  # Use just the final returned match
     SINGLE = 3  # As in FIRST, but raise/fail if more than one exists
     ALL = 4  #
     ANY = 5  #
 
 
 class DataPath:
     """Class to represent a path within a nested data structure.
 
     A DataPath locates nodes within a nested data structure. It comprises an
     address of nested data types (mapping values or list items) that can be further
-    refined using one ore more conditions. Validation rules are applied (i.e. tested) at
+    refined using one or more conditions. Validation rules are applied (i.e. tested) at
     the nodes identified by a ContainerPath.
 
     """
 
     DATUM_TYPE = DataPathDatumType.NONE
     MULTI_TYPE = DataPathMultiType.NONE
 
     def __init__(self, *parts, datum_type=None, multi_type=None, source_data=None):
-
         part_objs = []
         is_concrete = True
         for i in parts:
             if isinstance(i, ContainerValue):
                 is_concrete = False
             else:
                 if isinstance(i, (str, float)):
                     i = MapValue(i)
                 elif isinstance(i, int):
                     i = MapOrListValue(key=i, index=i)  # could be either map or list
                 else:
-                    raise TypeError(
-                        f"Cannot construct a DataPath from part of type: {type(i)}"
-                    )
+                    msg = f"Cannot construct a DataPath from part of type: {type(i)!r}"
+                    raise TypeError(msg)
+
             part_objs.append(i)
 
         self.parts = tuple(part_objs)
         self.is_concrete = is_concrete
         self.source_data = source_data
         self.DATUM_TYPE = DataPathDatumType(datum_type)
         self.MULTI_TYPE = DataPathMultiType(multi_type)
@@ -137,15 +133,14 @@
             and self.source_data == other.source_data
         ):
             return True
         return False
 
     @classmethod
     def from_spec(cls, spec):
-
         general_msg = (
             f'The specification key must start with "path" and optionally include, as '
             f'additional dot-delimited tokens, a `DATUM_TYPE` specifier (e.g. "path.map_keys", '
             f'"path.map_values", "path.type", "path.length") and/or a `MULTI_TYPE`'
             f' specifier (e.g. "path.single", "path.first", "path.last", '
             f'"path.all" or "path.single.map_keys" etc).'
         )
@@ -213,35 +208,40 @@
 
     @classmethod
     def from_part_specs(cls, *parts):
         """Construct a DataPath from parts that might include dicts, where each dict
         describes the required ContainerItem using string keys."""
 
         spec_resolved_parts = []
-        for i in parts:
+        for i in copy.deepcopy(parts):
             if isinstance(i, dict):
                 i = ContainerValue.from_spec(i)
             spec_resolved_parts.append(i)
 
         return cls(*spec_resolved_parts)
 
     def to_part_specs(self):
         parts = []
         for i in self.parts:
             try:
                 part_spec = i.condition.callable.kwargs["value"]
             except KeyError:
                 if isinstance(i, MapOrListValue):
                     part_spec = i.list_condition.callable.kwargs["value"]
+                elif i.CONTAINER_TYPE is Container.MAP:
+                    part_spec = {"type": "map_value"}
+                elif i.CONTAINER_TYPE is Container.LIST:
+                    part_spec = {"type": "list_value"}
+                else:
+                    raise RuntimeError(f"Cannot convert part to a part spec: {i!r}.")
             parts.append(part_spec)
         return parts
 
     @classmethod
     def from_str(cls, path_str, delimiter="/"):
-
         if path_str:
             path_str_parts = path_str.split(delimiter)
         else:
             path_str_parts = []
 
         path_parts = []
         for i in path_str_parts:
@@ -360,15 +360,14 @@
             elif self.DATUM_TYPE == DataPathDatumType.MAP_KEYS:
                 data = [list(i.keys()) for i in data]
             elif self.DATUM_TYPE == DataPathDatumType.MAP_VALUES:
                 data = [list(i.values()) for i in data]
         return data
 
     def _match_specified_multi_type(self, data, concrete_paths):
-
         if self.MULTI_TYPE.value:
             if self.MULTI_TYPE == DataPathMultiType.FIRST:
                 data = data[0]
             elif self.MULTI_TYPE == DataPathMultiType.LAST:
                 data = data[-1]
             elif self.MULTI_TYPE == DataPathMultiType.SINGLE:
                 if len(data) > 1:
@@ -409,19 +408,17 @@
             else:
                 return data
 
         data = [data]
         concrete_paths = []
 
         for part_idx, part in enumerate(self.parts):
-
             new_data = []
             new_concrete_paths = []
             for datum_idx, datum in enumerate(data):
-
                 try:
                     filtered_data = part.filter(datum)
                 except TypeError:
                     continue
 
                 new_data.extend(filtered_data.data)
 
@@ -448,14 +445,49 @@
         else:
             out = data
 
         out = self._match_specified_multi_type(out, concrete_paths)
 
         return out
 
+    def simplify(self) -> Tuple:
+        """Convert parts to simple primitives where possible, and leave other parts alone.
+
+        The output from this method can be passed back to the `DataPath` constructor
+        `parts` argument to generate the same `DataPath`.
+
+        """
+        out = []
+        for part in self.parts:
+            # note: we don't "simplify" a `ListValue` like `ListValue(0)` (meaning index 0
+            # of a list), because if passing the result back into a new  `DataPath`, a
+            # lone integer will be converted to a `MapOrListValue`, not a `ListValue`.
+            is_single_cond = not part.condition.flatten()[1]
+            if (
+                isinstance(part, MapValue)
+                and is_single_cond
+                and isinstance(part.condition, cnds.Key)
+                and part.condition.callable.name == "equal_to"
+            ):
+                out.append(part.condition.callable.kwargs["value"])
+            elif (
+                isinstance(part, MapOrListValue)
+                and part.condition == cnds.NullCondition()
+                and isinstance(part.list_condition, cnds.Index)
+                and not part.list_condition.flatten()[1]
+                and part.list_condition.callable.name == "equal_to"
+                and isinstance(part.map_condition, cnds.Key)
+                and not part.map_condition.flatten()[1]
+                and part.map_condition.callable.name == "equal_to"
+            ):
+                out.append(part.list_condition.callable.kwargs["value"])
+            else:
+                out.append(part)
+        return tuple(out)
+
 
 class ContainerValue:
     """Class for representing a container value (i.e. an item within either a list or a
     mapping). A container item can be filtered according to both its relationship to its
     parent container (i.e. position within the list for a list item, or key for a mapping
     item) and its value.
 
@@ -527,15 +559,14 @@
         # shorthand specs:
         value_short_keys = [i for i in spec if i.startswith("value.")]
         value_short_cond_specs = {i: spec.pop(i) for i in value_short_keys}
         for spec_k, spec_v in value_short_cond_specs.items():
             condition = condition & cnds.ConditionLike.from_spec({spec_k: spec_v})
 
         if cls == MapValue:
-
             # shorthand specs:
             key_short_keys = [i for i in spec if i.startswith("key.")]
             key_short_cond_specs = {i: spec.pop(i) for i in key_short_keys}
             for spec_k, spec_v in key_short_cond_specs.items():
                 condition = condition & cnds.ConditionLike.from_spec({spec_k: spec_v})
 
             key = spec.pop("key", None)
@@ -545,15 +576,14 @@
                     raise ValueError(
                         'Conditions specified in the "key" specification '
                         "must be key-like."
                     )
                 condition = condition & new_cond
 
         elif cls == ListValue:
-
             # shorthand specs:
             index_short_keys = [i for i in spec if i.startswith("index.")]
             index_short_cond_specs = {i: spec.pop(i) for i in index_short_keys}
             for spec_k, spec_v in index_short_cond_specs.items():
                 condition = condition & cnds.ConditionLike.from_spec({spec_k: spec_v})
 
             index = spec.pop("index", None)
@@ -563,15 +593,14 @@
                     raise ValueError(
                         'Conditions specified in the "index" specification '
                         "must be index-like."
                     )
                 condition = condition & new_cond
 
         elif cls == MapOrListValue:
-
             # shorthand specs:
             index_short_keys = [i for i in spec if i.startswith("index.")]
             index_short_cond_specs = {i: spec.pop(i) for i in index_short_keys}
             for spec_k, spec_v in index_short_cond_specs.items():
                 list_condition = list_condition & cnds.ConditionLike.from_spec(
                     {spec_k: spec_v}
                 )
@@ -625,19 +654,17 @@
         return DataPath(self, other)
 
     def __rtruediv__(self, other):
         return DataPath(other) / self
 
 
 class MapValue(ContainerValue):
-
     CONTAINER_TYPE = Container.MAP
 
     def __init__(self, key=None, value=None, condition=None, label=None):
-
         condition = get_container_value_condition(
             condition,
             key,
             cnds.Key,
             cnds.KeyLike,
             datum_condition_label="key",
         )
@@ -657,19 +684,17 @@
             raise TypeError(
                 "`MapValue` container can only filter a mapping (i.e. a dict)."
             )
         return self.condition.filter(data)
 
 
 class ListValue(ContainerValue):
-
     CONTAINER_TYPE = Container.LIST
 
     def __init__(self, index=None, value=None, condition=None, label=None):
-
         condition = get_container_value_condition(
             condition,
             index,
             cnds.Index,
             cnds.IndexLike,
             datum_condition_label="index",
         )
@@ -701,15 +726,14 @@
         index=None,
         value=None,
         list_condition=None,
         map_condition=None,
         condition=None,
         label=None,
     ):
-
         list_condition = get_container_value_condition(
             list_condition,
             index,
             cnds.Index,
             cnds.IndexLike,
             "lst_condition",
             "index",
@@ -732,15 +756,15 @@
         self.condition = condition
         self.list_condition = list_condition
         self.map_condition = map_condition
         self.label = label
 
     def __repr__(self):
         return (
-            f"{self.__class__.__name__}(condition={self.condition!r}"
+            f"{self.__class__.__name__}(condition={self.condition!r},"
             f" list_condition={self.list_condition!r}, map_condition={self.map_condition!r}"
             f'{f", label={self.label!r}" if self.label else ""}'
             f")"
         )
 
     def filter(self, data):
         if not isinstance(data, valida.data.Data):
@@ -750,32 +774,29 @@
         else:
             condition = self.map_condition & self.condition
 
         return condition.filter(data)
 
 
 def resolve_implicit_types(path):
-
     types = []
     for i in path:
-
         # Note: we don't support "complex mappings" from YAML where keys are themselves
         # mappings or lists
         try:
             type_i = i.CONTAINER_TYPE
         except AttributeError:
             raise TypeError(f'Unknown container item type: "{type(i)}"')
 
         types.append(type_i)
 
     return types
 
 
 def validate_rule_paths(rules):
-
     seen_paths = []
     predicted_types = {}
     for r_idx, r in enumerate(rules):
         r_path = r["path"]
         if r_path in seen_paths:
             msg = f"Rule index {r_idx} shares with another rule the path: {r_path}"
             raise DuplicateRule(msg)
@@ -797,15 +818,14 @@
                 predicted_types[partial_path_str] = {
                     "rules": [r_idx],
                     "types": [r_types[path_end_idx]],
                 }
 
     # Identify type, where possible, for each node
     for path, types_info in predicted_types.items():
-
         uniq_types = set(types_info["types"])
 
         if len(uniq_types) == 1:
             actual_type = list(uniq_types)[0]
 
         elif Container.LIST in uniq_types and Container.MAP in uniq_types:
             path_rules = [(i, rules[i]["path"]) for i in types_info["rules"]]
@@ -817,15 +837,14 @@
                 f"Incompatible rules specified for path {path}; at least one rule "
                 f"implies this node is a mapping, but at least one other rule implies "
                 f"this node is a list. Associated rule paths are: {path_rules_fmt}"
             )
             raise IncompatibleRules(msg)
 
         elif Container.CONTAINER in uniq_types:
-
             if Container.LIST in uniq_types:
                 actual_type = Container.LIST
 
             elif Container.MAP in uniq_types:
                 actual_type = Container.MAP
 
         else:
```

### Comparing `valida-0.5.2/valida/rules.py` & `valida-0.6.0/valida/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import copy
+from typing import List, Optional
 from valida.conditions import ConditionLike
 from valida.casting import CAST_DTYPE_LOOKUP, CAST_LOOKUP
 from valida.data import Data, set_datum
 from valida.datapath import DataPath
 from valida.errors import MalformedRuleSpec
 
 
 class Rule:
-    def __init__(self, path, condition, cast=None):
-
+    def __init__(self, path, condition, cast=None, doc: Optional[List[str]] = None):
         if not isinstance(path, DataPath):
             path = DataPath(*path)
 
         self.path = path
         self.condition = condition
         self.cast = cast
+        self.doc = doc
 
     def __repr__(self):
         return (
             f"{self.__class__.__name__}("
             f"path={self.path!r}, condition={self.condition!r}, cast={self.cast!r}"
             f")"
         )
@@ -33,17 +34,26 @@
                 return True
         return False
 
     @classmethod
     def from_spec(cls, spec):
         path = DataPath.from_part_specs(*spec["path"])
         cond = ConditionLike.from_spec(spec["condition"])
+        doc = spec.get("doc")
+
+        if doc:
+            if not isinstance(doc, list):
+                doc = [doc]
+
+            # strip final new lines:
+            for idx, i in enumerate(doc):
+                doc[idx] = i.strip()
+
         cast = spec.get("cast")
         for cast_from in list((cast or {}).keys()):
-
             cast_to = cast.pop(cast_from)
             try:
                 cast_from = CAST_DTYPE_LOOKUP[cast_from]
             except KeyError:
                 raise MalformedRuleSpec(f"Unknown cast_from type: {cast_from!r}")
 
             try:
@@ -54,15 +64,15 @@
             try:
                 cast[cast_from] = CAST_LOOKUP[(cast_from, cast_to)]
             except KeyError:
                 raise MalformedRuleSpec(
                     f"Unsupported cast from type {cast_from!r} to type {cast_to!r}."
                 )
 
-        return cls(path=path, condition=cond, cast=cast)
+        return cls(path=path, condition=cond, cast=cast, doc=doc)
 
     @classmethod
     def from_json_like(cls, json_like, *args, **kwargs):
         return cls.from_spec(json_like)
 
     def to_json_like(self, *args, **kwargs):
         out = {
@@ -72,15 +82,14 @@
         }
         if "shared_data" in kwargs:
             return out, kwargs["shared_data"]
         else:
             return out
 
     def test(self, data, _data_copy=None):
-
         if not isinstance(data, Data):
             data = Data(data)
 
         if not self.cast:
             data_copy = data
         else:
             data_copy = _data_copy or copy.deepcopy(data.get_original())
@@ -101,15 +110,14 @@
                     set_datum(data_copy, datum_path, datum)
 
         return RuleTest(self, data_copy)
 
 
 class RuleTestFailureItem:
     def __init__(self, rule_test, index, value, path, reasons):
-
         self.rule_test = rule_test
         self.index = index
         self.value = value
         self.path = path
         self.reasons = reasons
 
     def __repr__(self):
@@ -118,15 +126,14 @@
             f"value={self.value!r}, path={self.path!r}), reasons={self.reasons!r}"
             f")"
         )
 
 
 class RuleTest:
     def __init__(self, rule, data):
-
         if not isinstance(data, Data):
             data = Data(data)
 
         self.rule = rule
         self.data = data
 
         self._tested = False  # assigned by `_test()` - True if the rule path existed
@@ -174,15 +181,14 @@
                 out += " " + reason + "\n"
         return out
 
     def print_failures(self):
         print(self.get_failures_string())
 
     def _test(self):
-
         sub_data = self.rule.path.get_data(self.data, return_paths=True)
         path_exists = sub_data not in [None, []]
 
         if self.rule.path.is_concrete:
             sub_data = [sub_data]
 
         self.sub_data = sub_data
```

### Comparing `valida-0.5.2/PKG-INFO` & `valida-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valida
-Version: 0.5.2
+Version: 0.6.0
 Summary: Comprehensive validation library for nested data structures.
 License: MIT
 Author: Adam J. Plowman
 Author-email: adam.plowman@manchester.ac.uk
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

