# Comparing `tmp/act4e_mcdp-0.4.0-py3-none-any.whl.zip` & `tmp/act4e_mcdp-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 20739 bytes, number of entries: 14
+Zip file size: 22093 bytes, number of entries: 14
 -rw-r--r--  2.0 unx      347 b- defN 80-Jan-01 00:00 act4e_mcdp/__init__.py
--rw-r--r--  2.0 unx    27668 b- defN 80-Jan-01 00:00 act4e_mcdp/autogen_packed_test_data.py
+-rw-r--r--  2.0 unx    30570 b- defN 80-Jan-01 00:00 act4e_mcdp/autogen_packed_test_data.py
 -rw-r--r--  2.0 unx      571 b- defN 80-Jan-01 00:00 act4e_mcdp/download.py
--rw-r--r--  2.0 unx     8457 b- defN 80-Jan-01 00:00 act4e_mcdp/loading.py
+-rw-r--r--  2.0 unx     8867 b- defN 80-Jan-01 00:00 act4e_mcdp/loading.py
 -rw-r--r--  2.0 unx     3363 b- defN 80-Jan-01 00:00 act4e_mcdp/main.py
 -rw-r--r--  2.0 unx     4381 b- defN 80-Jan-01 00:00 act4e_mcdp/nameddps.py
 -rw-r--r--  2.0 unx     1790 b- defN 80-Jan-01 00:00 act4e_mcdp/posets.py
--rw-r--r--  2.0 unx     8747 b- defN 80-Jan-01 00:00 act4e_mcdp/primitivedps.py
+-rw-r--r--  2.0 unx     9865 b- defN 80-Jan-01 00:00 act4e_mcdp/primitivedps.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 act4e_mcdp/py.typed
 -rw-r--r--  2.0 unx     3944 b- defN 80-Jan-01 00:00 act4e_mcdp/solution_interface.py
--rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      109 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1119 b- defN 16-Jan-01 00:00 act4e_mcdp-0.4.0.dist-info/RECORD
-14 files, 60945 bytes uncompressed, 18887 bytes compressed:  69.0%
+-rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      109 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1119 b- defN 16-Jan-01 00:00 act4e_mcdp-0.4.1.dist-info/RECORD
+14 files, 65375 bytes uncompressed, 20241 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: act4e_mcdp/py.typed
 Comment: 
 
 Filename: act4e_mcdp/solution_interface.py
 Comment: 
 
-Filename: act4e_mcdp-0.4.0.dist-info/METADATA
+Filename: act4e_mcdp-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: act4e_mcdp-0.4.0.dist-info/WHEEL
+Filename: act4e_mcdp-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: act4e_mcdp-0.4.0.dist-info/entry_points.txt
+Filename: act4e_mcdp-0.4.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: act4e_mcdp-0.4.0.dist-info/RECORD
+Filename: act4e_mcdp-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## act4e_mcdp/autogen_packed_test_data.py

```diff
@@ -136,42 +136,46 @@
     "lib1_parts_e07_ceil_models_mcdpr1_yaml_fresh",
     "lib1_parts_e07_floor_models_mcdpr1_yaml",
     "lib1_parts_e07_floor_models_mcdpr1_yaml_fresh",
     "lib1_parts_e10_conversions1_models_mcdpr1_yaml",
     "lib1_parts_e10_conversions1_models_mcdpr1_yaml_fresh",
     "lib1_parts_e10_conversions2_models_mcdpr1_yaml",
     "lib1_parts_e10_conversions2_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e11_constant_fun_models_mcdpr1_yaml",
+    "lib1_parts_e11_constant_fun_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e11_constant_res_models_mcdpr1_yaml",
+    "lib1_parts_e11_constant_res_models_mcdpr1_yaml_fresh",
     "lib1_parts_nats_posets_mcdpr1_yaml",
     "lib1_parts_nats_posets_mcdpr1_yaml_fresh",
     "lib1_parts_reals_posets_mcdpr1_yaml",
     "lib1_parts_reals_posets_mcdpr1_yaml_fresh",
     "lib1_parts_reals_with_units_posets_mcdpr1_yaml",
     "lib1_parts_reals_with_units_posets_mcdpr1_yaml_fresh",
     "resources",
 ]
 
 
 lib1_parts_discrete_posets_mcdpr1_yaml: str = decode_to_str(
-    b"eJxNijkKwDAMBHu/QkXafEAPSJ0v+FiwiA+I9X8i202Kgd1hjhEzqmdHpKIFTJc0Udx9QE0+0hLTfiio"
-    b"aDrYnZSNaAQjGd6Ae1G8Sm8rmZJoJzOeO60dfns38efhPkb+JHg=",
+    b"eJxNirsNwCAMBXumcJE2CzBA6qzA50lYASMF768YaFKcdH6+Y6SCFrwjUtYKTxcLK+4+oDY+LNnTvlDR"
+    b"IDq8OykYxUhGNqIB96IG5S4rmRHRfs1wel4el+Pn+dcn9wFHAiR4",
 )
 
 
 def lib1_parts_discrete_posets_mcdpr1_yaml_fresh() -> str:
     return get_updated_str(
         lib1_parts_discrete_posets_mcdpr1_yaml,
         "../../assets/test-data/downloaded/lib1-parts.discrete.posets.mcdpr1.yaml",
     )
 
 
 _check_md5(
     "lib1_parts_discrete_posets_mcdpr1_yaml",
     lib1_parts_discrete_posets_mcdpr1_yaml,
     149,
-    "da99ccdf93e76923fea64b4e4e3d047b",
+    "c9661b0bd5daf948643f6b0043954d36",
     "../../assets/test-data/downloaded/lib1-parts.discrete.posets.mcdpr1.yaml",
 )
 lib1_parts_e01_empty_models_mcdpr1_yaml: str = decode_to_str(
     b"eJw1yjEOgCAMheGdU3TwFKw6G3fjQKDGRmgNlMl4d4nB7X15/1D8gclZA6CkES2Mki4ppDi7hGFa2nMS"
     b"Bwu/98peSdhFUsJi4X5MxiI1+y6W0JcXZvzq5nUzL1bHJqc=",
 )
 
@@ -564,14 +568,66 @@
 _check_md5(
     "lib1_parts_e10_conversions2_models_mcdpr1_yaml",
     lib1_parts_e10_conversions2_models_mcdpr1_yaml,
     6550,
     "c82585c7a83af500a45a04c8042d5736",
     "../../assets/test-data/downloaded/lib1-parts.e10_conversions2.models.mcdpr1.yaml",
 )
+lib1_parts_e11_constant_fun_models_mcdpr1_yaml: str = decode_to_str(
+    b"eJzFVd1KwzAYve9TfBeDXQ2229zJZCCIDAW9EBn9STHY/JCkgyE+gO/hk/kkJlnamqWdOjfWi5KcNN85"
+    b"p8lJRip/xjRFCYAmusII5pwKrojGNynFxeXSjLwQViBo+mXNck04SyuiCVZ2amlfAKOumH2205ZcYe0R"
+    b"T3FT0wxL5cCMa80pgvF07PqaCwRXrCSM6I1DatNSCGgiseK1zA0lvL4ljBdb8lVF6KxXgKe7I1RU+EGm"
+    b"IhDW+TMGYk/2WVVNK6rdb3DAZGB05p22bgOkdWs7oWOLFKIREOnxvNeEkk6OlygtSNbY23WVsMolEdY1"
+    b"ghI+3z9gNvW8AIvzGgfI9wrwVPdpVeOF5DSUsrbwTnlhv/heoqfqkLFBawPm+uxFBlPGGu7bw3+2g5eS"
+    b"F3Xejao6M0SPTzYcOWdrI9ms8qkywsX0BJtld68ER0L0O7ugNKpk1z7PFv45qRc0I5jpebtCh6VWnjCy"
+    b"f1sFk1pOKWfHFzKJiH8l5x/BOs4p5kJuIsiwi47ZkhMozXmFokRtzHLaS5hvh+zthoL0tvBqZ5oNYFB2"
+    b"39wmKMglJCa0d+kwU5V8AeZ+IyY=",
+)
+
+
+def lib1_parts_e11_constant_fun_models_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e11_constant_fun_models_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e11_constant_fun.models.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e11_constant_fun_models_mcdpr1_yaml",
+    lib1_parts_e11_constant_fun_models_mcdpr1_yaml,
+    2092,
+    "563104572fd6b5530dd4813ca08b645a",
+    "../../assets/test-data/downloaded/lib1-parts.e11_constant_fun.models.mcdpr1.yaml",
+)
+lib1_parts_e11_constant_res_models_mcdpr1_yaml: str = decode_to_str(
+    b"eJzFVctKAzEU3c9X3IXQVaHdZieVgptSFHQhUuaRweDkQZIpFPED/A+/zC8xSTOPtBm1OtJZlNybzD3n"
+    b"3NwzvVD5E6YpSgA00RVGsOBUcEU0XqUUF1drs/NMWIGgicua5ZpwllZEE6wQvLwmEitey9xE5ri0PwAX"
+    b"XWn77IusucLaZzzgqqYZlsolM641pwgms4mLNRcIrllJGNE7l6nNymDShPFiD7fJo3i++i2hosL3MhUB"
+    b"j04cQEyQzQei7NMgRdDiCgdUBkrnXmorN8i0cm1QiAbuCL29PKZ0yjp8z0kSarRtsVfsimGVSyKscATz"
+    b"GVD4eHsH6fe/VurR7tKqxkvJaah5a9MHOoQ90S8RqTrUwcEeDnQx1seDTgLcnPcqAVLGGsTl77m49Fry"
+    b"os67XVVnBujh0ZmDs60ha255PrJNGlNwMTtvL499Krv1iJQOGQXfpSNW35v1kmYEM71ob+hU15aBZf8w"
+    b"ReNMdM4p5Wx8FtOjRv+g/f/j8NNGwJvcWJBhZx0zlVMozQdzz8T+hSFj0TbYNKPss5qHBzsvd6/0bblD"
+    b"zo5RkNi7PTiz7AF2GzL5BESnHiE=",
+)
+
+
+def lib1_parts_e11_constant_res_models_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e11_constant_res_models_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e11_constant_res.models.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e11_constant_res_models_mcdpr1_yaml",
+    lib1_parts_e11_constant_res_models_mcdpr1_yaml,
+    2079,
+    "1befc235bc8bd89ea9f9221a291625be",
+    "../../assets/test-data/downloaded/lib1-parts.e11_constant_res.models.mcdpr1.yaml",
+)
 lib1_parts_nats_posets_mcdpr1_yaml: str = decode_to_str(
     b"eJwNx7ENgEAIAMCeKShMaLVlAxvjCr5iJPqPESzcXrq7ztdD6sKAeGrbGGdziVxoXMI4vbXI41Aswioj"
     b"9QRhN+PYdm0aH3hIlgaCN+9Jgh+sjBrN",
 )
 
 
 def lib1_parts_nats_posets_mcdpr1_yaml_fresh() -> str:
@@ -643,11 +699,13 @@
     "lib1-parts.e06_addf.models.mcdpr1.yaml": lib1_parts_e06_addf_models_mcdpr1_yaml,
     "lib1-parts.e06_addr.models.mcdpr1.yaml": lib1_parts_e06_addr_models_mcdpr1_yaml,
     "lib1-parts.e06_sumr.models.mcdpr1.yaml": lib1_parts_e06_sumr_models_mcdpr1_yaml,
     "lib1-parts.e07_ceil.models.mcdpr1.yaml": lib1_parts_e07_ceil_models_mcdpr1_yaml,
     "lib1-parts.e07_floor.models.mcdpr1.yaml": lib1_parts_e07_floor_models_mcdpr1_yaml,
     "lib1-parts.e10_conversions1.models.mcdpr1.yaml": lib1_parts_e10_conversions1_models_mcdpr1_yaml,
     "lib1-parts.e10_conversions2.models.mcdpr1.yaml": lib1_parts_e10_conversions2_models_mcdpr1_yaml,
+    "lib1-parts.e11_constant_fun.models.mcdpr1.yaml": lib1_parts_e11_constant_fun_models_mcdpr1_yaml,
+    "lib1-parts.e11_constant_res.models.mcdpr1.yaml": lib1_parts_e11_constant_res_models_mcdpr1_yaml,
     "lib1-parts.nats.posets.mcdpr1.yaml": lib1_parts_nats_posets_mcdpr1_yaml,
     "lib1-parts.reals.posets.mcdpr1.yaml": lib1_parts_reals_posets_mcdpr1_yaml,
     "lib1-parts.reals_with_units.posets.mcdpr1.yaml": lib1_parts_reals_with_units_posets_mcdpr1_yaml,
 }
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
+    Constant,
     DPSeries,
     JoinNDP,
+    Limit,
     M_Ceil_DP,
     M_FloorFun_DP,
     M_Fun_AddConstant_DP,
     M_Fun_AddMany_DP,
     M_Fun_MultiplyConstant_DP,
     M_Fun_MultiplyMany_DP,
     M_Res_AddConstant_DP,
@@ -68,16 +70,20 @@
     description = ob["$schema"].get("description", None)
     F = load_repr1(ob["F"], Poset)
     R = load_repr1(ob["R"], Poset)
     fields = dict(description=description, F=F, R=R)
 
     if "vu" in ob:
         fields["vu"] = load_repr1(ob["vu"], ValueFromPoset)
+    if "c" in ob:
+        fields["c"] = load_repr1(ob["c"], ValueFromPoset)
     if "opspace" in ob:
         fields["opspace"] = load_repr1(ob["opspace"], Poset)
+    if "common" in ob:
+        fields["common"] = load_repr1(ob["common"], Poset)
     if "C" in ob:
         fields["opspace"] = load_repr1(ob["C"], Poset)
     if "factor" in ob:
         from fractions import Fraction
 
         fields["factor"] = Fraction(ob["factor"])
     return fields
@@ -205,14 +211,26 @@
 
 @loader_for("MeetNDualDP")
 def load_MeetNDualDP(ob: dict):
     fields = _load_DP_fields(ob)
     return MeetNDualDP(**fields)
 
 
+@loader_for("Limit")
+def load_Limit(ob: dict):
+    fields = _load_DP_fields(ob)
+    return Limit(**fields)
+
+
+@loader_for("Constant")
+def load_Constant(ob: dict):
+    fields = _load_DP_fields(ob)
+    return Constant(**fields)
+
+
 #
 # @loader_for('M_Fun_MultiplyConstant_DP')
 # def load_M_Fun_MultiplyConstant_DP(ob: dict):
 #     F = load_repr1(ob['F'], Poset)
 #     R = load_repr1(ob['R'], Poset)
 #
 #     return PrimitiveDP(F=F, R=R)
```

## act4e_mcdp/primitivedps.py

```diff
@@ -2,16 +2,18 @@
 from fractions import Fraction
 from typing import Optional
 
 from .posets import Poset
 
 __all__ = [
     "AmbientConversion",
+    "Constant",
     "DPSeries",
     "JoinNDP",
+    "Limit",
     "M_Ceil_DP",
     "M_FloorFun_DP",
     "M_Fun_AddConstant_DP",
     "M_Fun_AddMany_DP",
     "M_Fun_MultiplyConstant_DP",
     "M_Fun_MultiplyMany_DP",
     "M_Fun_MultiplyMany_DP",
@@ -395,7 +397,61 @@
         F (Poset): The functionality poset $\F$
         R (Poset): The resources poset $\R$
         common: The common ambient poset $\common$
 
     """
 
     common: Poset
+
+
+@dataclass
+class Limit(PrimitiveDP):
+    r"""
+    Implements a bound on the functionality.
+
+    This is the dual of [Constant][act4e_mcdp.primitivedps.Constant].
+
+    Relation:
+
+        $$
+          \fun \leq  c
+        $$
+
+    Note that the resources $\res$ do not appear in the relation.
+    As long as the functionality is below the limit, the resources can be anything.
+
+    Attributes:
+
+        F (Poset): The functionality poset $\F$
+        R (Poset): The resources poset $\R$
+        c: The constant $c$
+
+    """
+
+    c: ValueFromPoset
+
+
+@dataclass
+class Constant(PrimitiveDP):
+    r"""
+    Implements a bound on the resources.
+
+    This is the dual of [Limit][act4e_mcdp.primitivedps.Limit].
+
+    Relation:
+
+        $$
+          c \leq  \res
+        $$
+
+    Note that the functionality $\fun$ do not appear in the relation.
+    As long as the resources is above the limit, the functionality can be anything.
+
+    Attributes:
+
+        F (Poset): The functionality poset $\F$
+        R (Poset): The resources poset $\R$
+        c: The constant $c$
+
+    """
+
+    c: ValueFromPoset
```

## Comparing `act4e_mcdp-0.4.0.dist-info/RECORD` & `act4e_mcdp-0.4.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 act4e_mcdp/__init__.py,sha256=E_ujpgzc-ou4a5DKP7fNLO7NZVky0K3bl5mp2ob3ahU,347
-act4e_mcdp/autogen_packed_test_data.py,sha256=74ahEQkoC9jnCsNsZCAft34NJPHHQER3j8T1Bij86iM,27668
+act4e_mcdp/autogen_packed_test_data.py,sha256=C2PZegLbjS0c2lWXVBSP0EIivpLM3lyVrfSY_mzx6gs,30570
 act4e_mcdp/download.py,sha256=fXm46ISIYvpFjouSMB0l0XLuJWw5CxZSpgi-fvmxMGA,571
-act4e_mcdp/loading.py,sha256=yvLGVxHk08lr7WB_SWMAs8A5IjonRugKOLsuRHXE_9g,8457
+act4e_mcdp/loading.py,sha256=fgC-e50Hs7-OWdnS4BG1mcq5xqRlJstx0VlTHv06bmo,8867
 act4e_mcdp/main.py,sha256=c_Fy0nmJrrikwDQpdv_y0shFrH3AHg1auOdk1Dsc_Hs,3363
 act4e_mcdp/nameddps.py,sha256=OaYt-P9pGt6TQa9oXWWHZI4PFRt9kPyfQatPEx9rH60,4381
 act4e_mcdp/posets.py,sha256=7iijB7waZd3nTyK-_eNBR6YZOWhcTUYtKqCm7irpFKE,1790
-act4e_mcdp/primitivedps.py,sha256=2STRQwuMGDbh_jE7WYBWoOq4evMjUiqyf0Bc6c82sWY,8747
+act4e_mcdp/primitivedps.py,sha256=wZkeJTu7MuApU0mO0_WKWY95gRlS9PiurOMbsEqaUCk,9865
 act4e_mcdp/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 act4e_mcdp/solution_interface.py,sha256=7TjPbeJKbZ_29c1l5eW-TlWQEP0TxEl9I9JclJY9pi4,3944
-act4e_mcdp-0.4.0.dist-info/METADATA,sha256=qujNtxFrBz2w8T4r5tf81OUNTgbA6kZvfRQDWhYZ4eQ,361
-act4e_mcdp-0.4.0.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-act4e_mcdp-0.4.0.dist-info/entry_points.txt,sha256=ab4CbY_rBOTC8YJBuIQeKxZExEYTrXx6fDsX1GivxXo,109
-act4e_mcdp-0.4.0.dist-info/RECORD,,
+act4e_mcdp-0.4.1.dist-info/METADATA,sha256=WKlABsGaVWiwR_t3YeXWXzB4VYXVW5NWfeuaA93ZbJk,361
+act4e_mcdp-0.4.1.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+act4e_mcdp-0.4.1.dist-info/entry_points.txt,sha256=ab4CbY_rBOTC8YJBuIQeKxZExEYTrXx6fDsX1GivxXo,109
+act4e_mcdp-0.4.1.dist-info/RECORD,,
```

