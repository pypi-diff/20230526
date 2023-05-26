# Comparing `tmp/act4e_mcdp-0.4.1-py3-none-any.whl.zip` & `tmp/act4e_mcdp-0.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 22093 bytes, number of entries: 14
+Zip file size: 22388 bytes, number of entries: 14
 -rw-r--r--  2.0 unx      347 b- defN 80-Jan-01 00:00 act4e_mcdp/__init__.py
 -rw-r--r--  2.0 unx    30570 b- defN 80-Jan-01 00:00 act4e_mcdp/autogen_packed_test_data.py
 -rw-r--r--  2.0 unx      571 b- defN 80-Jan-01 00:00 act4e_mcdp/download.py
--rw-r--r--  2.0 unx     8867 b- defN 80-Jan-01 00:00 act4e_mcdp/loading.py
+-rw-r--r--  2.0 unx     9138 b- defN 80-Jan-01 00:00 act4e_mcdp/loading.py
 -rw-r--r--  2.0 unx     3363 b- defN 80-Jan-01 00:00 act4e_mcdp/main.py
 -rw-r--r--  2.0 unx     4381 b- defN 80-Jan-01 00:00 act4e_mcdp/nameddps.py
 -rw-r--r--  2.0 unx     1790 b- defN 80-Jan-01 00:00 act4e_mcdp/posets.py
--rw-r--r--  2.0 unx     9865 b- defN 80-Jan-01 00:00 act4e_mcdp/primitivedps.py
+-rw-r--r--  2.0 unx    10766 b- defN 80-Jan-01 00:00 act4e_mcdp/primitivedps.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 act4e_mcdp/py.typed
 -rw-r--r--  2.0 unx     3944 b- defN 80-Jan-01 00:00 act4e_mcdp/solution_interface.py
--rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      109 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1119 b- defN 16-Jan-01 00:00 act4e_mcdp-0.4.1.dist-info/RECORD
-14 files, 65375 bytes uncompressed, 20241 bytes compressed:  69.0%
+-rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      109 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1120 b- defN 16-Jan-01 00:00 act4e_mcdp-0.4.2.dist-info/RECORD
+14 files, 66548 bytes uncompressed, 20536 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: act4e_mcdp/py.typed
 Comment: 
 
 Filename: act4e_mcdp/solution_interface.py
 Comment: 
 
-Filename: act4e_mcdp-0.4.1.dist-info/METADATA
+Filename: act4e_mcdp-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: act4e_mcdp-0.4.1.dist-info/WHEEL
+Filename: act4e_mcdp-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: act4e_mcdp-0.4.1.dist-info/entry_points.txt
+Filename: act4e_mcdp-0.4.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: act4e_mcdp-0.4.1.dist-info/RECORD
+Filename: act4e_mcdp-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## act4e_mcdp/loading.py

```diff
@@ -12,16 +12,18 @@
     NodeFunctionality,
     NodeResource,
     SimpleWrap,
 )
 from .posets import FinitePoset, Numbers, Poset, PosetProduct
 from .primitivedps import (
     AmbientConversion,
+    CatalogueDP,
     Constant,
     DPSeries,
+    EntryInfo,
     JoinNDP,
     Limit,
     M_Ceil_DP,
     M_FloorFun_DP,
     M_Fun_AddConstant_DP,
     M_Fun_AddMany_DP,
     M_Fun_MultiplyConstant_DP,
@@ -93,14 +95,23 @@
 def load_ValueFromPoset(ob: dict):
     poset = load_repr1(ob["poset"], Poset)
     value = ob["value"]
     value = parse_yaml_value(poset, value)
     return ValueFromPoset(value=value, poset=poset)
 
 
+@loader_for("CatalogueDP")
+def load_CatalogueDP(ob: dict):
+    fields = _load_DP_fields(ob)
+    entries = fields["entries"] = {}
+    for k, v in ob["entries"].items():
+        entries[k] = EntryInfo(**v)
+    return CatalogueDP(**fields)
+
+
 @loader_for("M_Res_MultiplyConstant_DP")
 def load_M_Res_MultiplyConstant_DP(ob: dict):
     fields = _load_DP_fields(ob)
     return M_Res_MultiplyConstant_DP(**fields)
 
 
 @loader_for("M_Fun_MultiplyConstant_DP")
```

## act4e_mcdp/primitivedps.py

```diff
@@ -439,19 +439,56 @@
 
     Relation:
 
         $$
           c \leq  \res
         $$
 
-    Note that the functionality $\fun$ do not appear in the relation.
-    As long as the resources is above the limit, the functionality can be anything.
+        Note that the functionality $\fun$ do not appear in the relation.
+        As long as the resources is above the limit, the functionality can be anything.
 
     Attributes:
 
         F (Poset): The functionality poset $\F$
         R (Poset): The resources poset $\R$
         c: The constant $c$
 
     """
 
     c: ValueFromPoset
+
+
+@dataclass
+class EntryInfo:
+    r"""
+    Describes $\fun^{\max}_{\imp}$ and $\res^{\min}_{\imp}$ for an implementation.
+    """
+    f_max: object
+    r_min: object
+
+
+@dataclass
+class CatalogueDP(PrimitiveDP):
+    r"""
+    Implements a catalogue.
+
+    The available implementations are strings and each of them has a (max) functionality and a (min) resource.
+
+    Relation:
+
+        $$
+           \bigvee_{\imp \in \impspace}   ( \fun \leq \fun^{\max}_{\imp}) \wedge (\res^{\min}_{\imp} \leq
+           \res)
+        $$
+
+        where $\impspace$ is the set of implementations and $\fun^{\max}_{\imp}, \res^{\min}_{\imp}$ are
+        the functionality and resources of the implementation $\imp$.
+
+    Attributes:
+
+        F (Poset): The functionality poset $\F$
+        R (Poset): The resources poset $\R$
+        entries: A dictionary of entries.
+
+    """
+
+    entries: dict[str, EntryInfo]
```

## Comparing `act4e_mcdp-0.4.1.dist-info/RECORD` & `act4e_mcdp-0.4.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 act4e_mcdp/__init__.py,sha256=E_ujpgzc-ou4a5DKP7fNLO7NZVky0K3bl5mp2ob3ahU,347
 act4e_mcdp/autogen_packed_test_data.py,sha256=C2PZegLbjS0c2lWXVBSP0EIivpLM3lyVrfSY_mzx6gs,30570
 act4e_mcdp/download.py,sha256=fXm46ISIYvpFjouSMB0l0XLuJWw5CxZSpgi-fvmxMGA,571
-act4e_mcdp/loading.py,sha256=fgC-e50Hs7-OWdnS4BG1mcq5xqRlJstx0VlTHv06bmo,8867
+act4e_mcdp/loading.py,sha256=xrozob-NEjeAUT7LYslgnn7obwTKad23Atd-BCGdCuI,9138
 act4e_mcdp/main.py,sha256=c_Fy0nmJrrikwDQpdv_y0shFrH3AHg1auOdk1Dsc_Hs,3363
 act4e_mcdp/nameddps.py,sha256=OaYt-P9pGt6TQa9oXWWHZI4PFRt9kPyfQatPEx9rH60,4381
 act4e_mcdp/posets.py,sha256=7iijB7waZd3nTyK-_eNBR6YZOWhcTUYtKqCm7irpFKE,1790
-act4e_mcdp/primitivedps.py,sha256=wZkeJTu7MuApU0mO0_WKWY95gRlS9PiurOMbsEqaUCk,9865
+act4e_mcdp/primitivedps.py,sha256=yyXovQ4cfb4SzSpGRFf46Xg1cnTeiOxgBREHnDVdSAg,10766
 act4e_mcdp/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 act4e_mcdp/solution_interface.py,sha256=7TjPbeJKbZ_29c1l5eW-TlWQEP0TxEl9I9JclJY9pi4,3944
-act4e_mcdp-0.4.1.dist-info/METADATA,sha256=WKlABsGaVWiwR_t3YeXWXzB4VYXVW5NWfeuaA93ZbJk,361
-act4e_mcdp-0.4.1.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-act4e_mcdp-0.4.1.dist-info/entry_points.txt,sha256=ab4CbY_rBOTC8YJBuIQeKxZExEYTrXx6fDsX1GivxXo,109
-act4e_mcdp-0.4.1.dist-info/RECORD,,
+act4e_mcdp-0.4.2.dist-info/METADATA,sha256=o1CpGI6Z181wCKnrcdlDPQ0HWcQuUHv9XyX8XItAa0w,361
+act4e_mcdp-0.4.2.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+act4e_mcdp-0.4.2.dist-info/entry_points.txt,sha256=ab4CbY_rBOTC8YJBuIQeKxZExEYTrXx6fDsX1GivxXo,109
+act4e_mcdp-0.4.2.dist-info/RECORD,,
```

