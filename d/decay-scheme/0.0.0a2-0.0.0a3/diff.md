# Comparing `tmp/decay_scheme-0.0.0a2.tar.gz` & `tmp/decay_scheme-0.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decay_scheme-0.0.0a2.tar", max compression
+gzip compressed data, was "decay_scheme-0.0.0a3.tar", max compression
```

## Comparing `decay_scheme-0.0.0a2.tar` & `decay_scheme-0.0.0a3.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      251 2023-04-27 11:24:31.788437 decay_scheme-0.0.0a2/decay_scheme/__init__.py
--rw-r--r--   0        0        0      134 2023-04-27 07:48:18.102851 decay_scheme-0.0.0a2/decay_scheme/data/arrowhead_codes.dat
--rw-r--r--   0        0        0     1078 2023-04-27 07:48:18.107848 decay_scheme-0.0.0a2/decay_scheme/data/arrowhead_vertices.dat
--rw-r--r--   0        0        0     4353 2023-04-27 11:24:31.791445 decay_scheme-0.0.0a2/decay_scheme/decay_scheme_classes.py
--rw-r--r--   0        0        0     7833 2023-04-27 11:38:12.008057 decay_scheme-0.0.0a2/decay_scheme/decay_scheme_drawer.py
--rw-r--r--   0        0        0        0 2023-04-27 11:20:20.477888 decay_scheme-0.0.0a2/LICENSE
--rw-r--r--   0        0        0      516 2023-04-27 11:46:24.173473 decay_scheme-0.0.0a2/pyproject.toml
--rw-r--r--   0        0        0      142 2023-04-27 07:48:18.102851 decay_scheme-0.0.0a2/README.md
--rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 decay_scheme-0.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-05-26 13:26:23.783245 decay_scheme-0.0.0a3/README.md
+-rw-r--r--   0        0        0      255 2023-05-26 13:37:09.254547 decay_scheme-0.0.0a3/decay_scheme/__init__.py
+-rw-r--r--   0        0        0       90 2023-05-26 13:26:23.783952 decay_scheme-0.0.0a3/decay_scheme/data/arrowhead_codes.dat
+-rw-r--r--   0        0        0     1034 2023-05-26 13:26:23.784312 decay_scheme-0.0.0a3/decay_scheme/data/arrowhead_vertices.dat
+-rw-r--r--   0        0        0     4197 2023-05-26 13:26:23.784685 decay_scheme-0.0.0a3/decay_scheme/decay_scheme_classes.py
+-rw-r--r--   0        0        0     7701 2023-05-26 13:28:01.976457 decay_scheme-0.0.0a3/decay_scheme/decay_scheme_drawer.py
+-rw-r--r--   0        0        0      496 2023-05-26 13:39:45.354254 decay_scheme-0.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 decay_scheme-0.0.0a3/PKG-INFO
```

### Comparing `decay_scheme-0.0.0a2/decay_scheme/data/arrowhead_vertices.dat` & `decay_scheme-0.0.0a3/decay_scheme/data/arrowhead_vertices.dat`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-1.24089308  0.14481206
-9.31854008  1.68520206
-9.31854008  1.68520206
-9.35018913  1.69123748
-9.38278384  1.69021146
-9.41399065  1.68219746
-9.44519745  1.67418346
-9.47425341  1.65937741
-9.49907831  1.63883932
-9.52390321  1.61830122
-9.54389013  1.59253321
-9.55760815  1.56338008
-9.57132617  1.53422695
-9.57843991  1.50240145
-9.57844008  1.47018206
-9.57844008 -1.47522794
-9.57844008 -1.47522794
-9.57843947 -1.50713128
-9.57130693 -1.53863465
-9.55756568 -1.56742702
-9.54382442 -1.5962194 
-9.52381889 -1.62157909
-9.49901663 -1.64164577
-9.47421438 -1.66171244
-9.44523709 -1.67598311
-9.41421047 -1.68341092
-9.38318386 -1.69083872
-9.35088562 -1.69123748
-9.31968508 -1.68457794
-1.23974808  0.04002206
-1.23974808  0.04002206
-1.22768246  0.04259313
-1.21687103  0.04926318
-1.2091603   0.05889303
-1.20144956  0.06852288
-1.19730501  0.08053119
-1.1974345   0.09286701
-1.19756399  0.10520284
-1.20195971  0.1171215 
-1.20987089  0.12658736
-1.21778208  0.13605322
-1.22873115  0.14249485
-1.24084808  0.14481206
-1.24089308  0.14481206
+1.24089308  0.14481206
+9.31854008  1.68520206
+9.31854008  1.68520206
+9.35018913  1.69123748
+9.38278384  1.69021146
+9.41399065  1.68219746
+9.44519745  1.67418346
+9.47425341  1.65937741
+9.49907831  1.63883932
+9.52390321  1.61830122
+9.54389013  1.59253321
+9.55760815  1.56338008
+9.57132617  1.53422695
+9.57843991  1.50240145
+9.57844008  1.47018206
+9.57844008 -1.47522794
+9.57844008 -1.47522794
+9.57843947 -1.50713128
+9.57130693 -1.53863465
+9.55756568 -1.56742702
+9.54382442 -1.5962194 
+9.52381889 -1.62157909
+9.49901663 -1.64164577
+9.47421438 -1.66171244
+9.44523709 -1.67598311
+9.41421047 -1.68341092
+9.38318386 -1.69083872
+9.35088562 -1.69123748
+9.31968508 -1.68457794
+1.23974808  0.04002206
+1.23974808  0.04002206
+1.22768246  0.04259313
+1.21687103  0.04926318
+1.2091603   0.05889303
+1.20144956  0.06852288
+1.19730501  0.08053119
+1.1974345   0.09286701
+1.19756399  0.10520284
+1.20195971  0.1171215 
+1.20987089  0.12658736
+1.21778208  0.13605322
+1.22873115  0.14249485
+1.24084808  0.14481206
+1.24089308  0.14481206
 1.24089308  0.14481206
```

### Comparing `decay_scheme-0.0.0a2/decay_scheme/decay_scheme_classes.py` & `decay_scheme-0.0.0a3/decay_scheme/decay_scheme_classes.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-from __future__ import annotations
-
-import enum
-import functools
-from typing import List, Iterable, Literal, Optional
-import bisect
-import dataclasses
-
-
-class DecaySchema:
-    def __init__(self):
-        self.nuclides: List[Nuclide] = []
-        self.current_nuclide: int = 0
-        self.num_nuclides: int = 0
-        self.decays: List[Decay] = []
-        # self.decays_to_coordinates = []
-        self.freetexts = []
-        self.freearrows = []
-    
-    def add_nuclide(self, nuclide: Nuclide):
-        bisect.insort(self.nuclides, nuclide)
-        self.num_nuclides += 1
-    
-    def __iter__(self) -> List[Nuclide]:
-        return self.nuclides
-    
-    def __str__(self) -> str:
-        result = "------ Decay schema ------\n"
-        for nuclide in self.nuclides:
-            result += str(nuclide) + "\n"
-        return result
-
-    def __repr__(self) -> str:
-        return f"<DecaySchema({self.nuclides})>"
-    
-    def add_decay(self, decay: Decay):
-        self.decays.append(decay)
-
-    def add_freetext(self, freetext: FreeText):
-        self.freetexts.append(freetext)
-
-    def add_freearrow(self, freearrow: FreeArrow):
-        self.freearrows.append(freearrow)
-
-
-@functools.total_ordering
-@dataclasses.dataclass(init=True, repr=True, kw_only=True, eq=True)
-class Nuclide:
-    index: int
-    name: str
-    horizontal_padding: float = 0
-
-    def __post_init__(self):
-        if self.index < 0:
-            raise ValueError(f"Nuclide index must be positive. Was {self.index}.")
-        self.levels: List[Level] = []
-        self.num_levels: int = 0
-    
-    def add_level(self, level: Level):
-        bisect.insort(self.levels, level)
-        self.num_levels += 1
-    
-    def __lt__(self, other: Nuclide):
-        return self.index < other.index
-
-
-class Parity(enum.Enum):
-    """Represents the two parity options available."""
-    UP = "+"
-    DOWN = "-"
-
-
-@functools.total_ordering
-@dataclasses.dataclass(init=True, kw_only=True, eq=True)
-class Level:
-    energy: float
-    spin: str
-    parity: Parity
-    ls: str = '-'
-    lw: float = 1.
-    color: str = 'k'
-    text_above: Optional[str] = None
-    text_below: Optional[str] = None
-    energy_format_string: Optional[str] = None
-    draw_QEC_level_below: bool = False
-    draw_reference_line: bool = False
-    hide_energy_spin_parity: bool = False
-    energy_spin_parity_below: bool = False
-    broad: bool = False
-    many: bool = False
-    width: float = 0
-    upper_energy: float = 0.
-    upper_spin: Optional[str] = None
-    upper_parity: Optional[Parity] = None
-    energy_x_adjust: float = 0.
-    energy_y_adjust: float = 0.
-    spin_parity_x_adjust: float = 0.
-    spin_parity_y_adjust: float = 0.
-    text_above_x_adjust: float = 0.
-    text_above_y_adjust: float = 0.
-    text_below_x_adjust: float = 0.
-    text_below_y_adjust: float = 0.
-    QEC_x_adjust: float = 0.
-    QEC_y_adjust: float = 0.
-    upper_energy_x_adjust: float = 0.
-    upper_energy_y_adjust: float = 0.
-    upper_spin_parity_x_adjust: float = 0.
-    upper_spin_parity_y_adjust: float = 0.
-
-    def __lt__(self, other: Level):
-        return self.energy < other.energy
-    
-    def __repr__(self) -> str:
-        f = "1.1f" if self.energy_format_string is None else self.energy_format_string
-        return f"<Level(E={self.energy:{f}}, J={self.spin}, pi={self.parity})>"
-
-
-@dataclasses.dataclass(init=True, kw_only=True, eq=True)
-class Decay:
-    parent_nuclide: Nuclide
-    parent_level: Level
-    daughter_nuclide: Nuclide
-    daughter_level: Level
-    color: str = "k"
-    ls: str = "-"
-#
-#
-# class decay_to_coordinate:
-#     def __init__(self, parent_nuclide, parent_level, x, y, color='k'):
-#         self.parent_nuclide = parent_nuclide
-#         self.parent_level = parent_level
-#         self.x = x
-#         self.y = y
-#         self.color = color
-#
-
-
-@dataclasses.dataclass(init=True, kw_only=True, eq=True)
-class FreeText:
-    text: str
-    x: float
-    y: float
-    va: str = "center"
-    ha: str = "center"
-    rotation: float = 0
-    color: str = "k"
-
-
-@dataclasses.dataclass(init=True, kw_only=True, eq=True)
-class FreeArrow:
-    startx: float
-    starty: float
-    endx: float
-    endy: float
-    color: str = "k"
-    ls: str = "-"
+from __future__ import annotations
+
+import enum
+import functools
+from typing import List, Iterable, Literal, Optional
+import bisect
+import dataclasses
+
+
+class DecaySchema:
+    def __init__(self):
+        self.nuclides: List[Nuclide] = []
+        self.current_nuclide: int = 0
+        self.num_nuclides: int = 0
+        self.decays: List[Decay] = []
+        # self.decays_to_coordinates = []
+        self.freetexts = []
+        self.freearrows = []
+    
+    def add_nuclide(self, nuclide: Nuclide):
+        bisect.insort(self.nuclides, nuclide)
+        self.num_nuclides += 1
+    
+    def __iter__(self) -> List[Nuclide]:
+        return self.nuclides
+    
+    def __str__(self) -> str:
+        result = "------ Decay schema ------\n"
+        for nuclide in self.nuclides:
+            result += str(nuclide) + "\n"
+        return result
+
+    def __repr__(self) -> str:
+        return f"<DecaySchema({self.nuclides})>"
+    
+    def add_decay(self, decay: Decay):
+        self.decays.append(decay)
+
+    def add_freetext(self, freetext: FreeText):
+        self.freetexts.append(freetext)
+
+    def add_freearrow(self, freearrow: FreeArrow):
+        self.freearrows.append(freearrow)
+
+
+@functools.total_ordering
+@dataclasses.dataclass(init=True, repr=True, kw_only=True, eq=True)
+class Nuclide:
+    index: int
+    name: str
+    horizontal_padding: float = 0
+
+    def __post_init__(self):
+        if self.index < 0:
+            raise ValueError(f"Nuclide index must be positive. Was {self.index}.")
+        self.levels: List[Level] = []
+        self.num_levels: int = 0
+    
+    def add_level(self, level: Level):
+        bisect.insort(self.levels, level)
+        self.num_levels += 1
+    
+    def __lt__(self, other: Nuclide):
+        return self.index < other.index
+
+
+class Parity(enum.Enum):
+    """Represents the two parity options available."""
+    UP = "+"
+    DOWN = "-"
+
+
+@functools.total_ordering
+@dataclasses.dataclass(init=True, kw_only=True, eq=True)
+class Level:
+    energy: float
+    spin: str
+    parity: Parity
+    ls: str = '-'
+    lw: float = 1.
+    color: str = 'k'
+    text_above: Optional[str] = None
+    text_below: Optional[str] = None
+    energy_format_string: Optional[str] = None
+    draw_QEC_level_below: bool = False
+    draw_reference_line: bool = False
+    hide_energy_spin_parity: bool = False
+    energy_spin_parity_below: bool = False
+    broad: bool = False
+    many: bool = False
+    width: float = 0
+    upper_energy: float = 0.
+    upper_spin: Optional[str] = None
+    upper_parity: Optional[Parity] = None
+    energy_x_adjust: float = 0.
+    energy_y_adjust: float = 0.
+    spin_parity_x_adjust: float = 0.
+    spin_parity_y_adjust: float = 0.
+    text_above_x_adjust: float = 0.
+    text_above_y_adjust: float = 0.
+    text_below_x_adjust: float = 0.
+    text_below_y_adjust: float = 0.
+    QEC_x_adjust: float = 0.
+    QEC_y_adjust: float = 0.
+    upper_energy_x_adjust: float = 0.
+    upper_energy_y_adjust: float = 0.
+    upper_spin_parity_x_adjust: float = 0.
+    upper_spin_parity_y_adjust: float = 0.
+
+    def __lt__(self, other: Level):
+        return self.energy < other.energy
+    
+    def __repr__(self) -> str:
+        f = "1.1f" if self.energy_format_string is None else self.energy_format_string
+        return f"<Level(E={self.energy:{f}}, J={self.spin}, pi={self.parity})>"
+
+
+@dataclasses.dataclass(init=True, kw_only=True, eq=True)
+class Decay:
+    parent_nuclide: Nuclide
+    parent_level: Level
+    daughter_nuclide: Nuclide
+    daughter_level: Level
+    color: str = "k"
+    ls: str = "-"
+#
+#
+# class decay_to_coordinate:
+#     def __init__(self, parent_nuclide, parent_level, x, y, color='k'):
+#         self.parent_nuclide = parent_nuclide
+#         self.parent_level = parent_level
+#         self.x = x
+#         self.y = y
+#         self.color = color
+#
+
+
+@dataclasses.dataclass(init=True, kw_only=True, eq=True)
+class FreeText:
+    text: str
+    x: float
+    y: float
+    va: str = "center"
+    ha: str = "center"
+    rotation: float = 0
+    color: str = "k"
+
+
+@dataclasses.dataclass(init=True, kw_only=True, eq=True)
+class FreeArrow:
+    startx: float
+    starty: float
+    endx: float
+    endy: float
+    color: str = "k"
+    ls: str = "-"
```

### Comparing `decay_scheme-0.0.0a2/PKG-INFO` & `decay_scheme-0.0.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decay-scheme
-Version: 0.0.0a2
+Version: 0.0.0a3
 Summary: A python package to draw nuclear decay schemas
 Author: Erik Asbjørn Mikkelsen Jensen
 Author-email: ej@phys.au.dk
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

