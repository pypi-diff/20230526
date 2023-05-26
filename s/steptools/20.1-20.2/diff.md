# Comparing `tmp/steptools-20.1-cp37-abi3-win_amd64.whl.zip` & `tmp/steptools-20.2-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7353794 bytes, number of entries: 8
+Zip file size: 7379375 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat        2 b- defN 22-Aug-19 14:38 steptools/py.typed
--rw-rw-rw-  2.0 fat 30832360 b- defN 23-May-15 22:31 steptools/step.pyd
--rw-rw-rw-  2.0 fat   107772 b- defN 23-May-15 19:45 steptools/step.pyi
--rw-rw-rw-  2.0 fat     3043 b- defN 23-May-15 22:32 steptools-20.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7014 b- defN 23-May-15 22:32 steptools-20.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-15 22:32 steptools-20.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-May-15 22:32 steptools-20.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      620 b- defN 23-May-15 22:32 steptools-20.1.dist-info/RECORD
-8 files, 30950926 bytes uncompressed, 7352728 bytes compressed:  76.2%
+-rw-rw-rw-  2.0 fat 30931688 b- defN 23-May-26 00:34 steptools/step.pyd
+-rw-rw-rw-  2.0 fat   120367 b- defN 23-May-25 18:36 steptools/step.pyi
+-rw-rw-rw-  2.0 fat     3043 b- defN 23-May-26 00:34 steptools-20.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7014 b- defN 23-May-26 00:34 steptools-20.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-26 00:34 steptools-20.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-May-26 00:34 steptools-20.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      620 b- defN 23-May-26 00:34 steptools-20.2.dist-info/RECORD
+8 files, 31062849 bytes uncompressed, 7378309 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: steptools/step.pyd
 Comment: 
 
 Filename: steptools/step.pyi
 Comment: 
 
-Filename: steptools-20.1.dist-info/LICENSE
+Filename: steptools-20.2.dist-info/LICENSE
 Comment: 
 
-Filename: steptools-20.1.dist-info/METADATA
+Filename: steptools-20.2.dist-info/METADATA
 Comment: 
 
-Filename: steptools-20.1.dist-info/WHEEL
+Filename: steptools-20.2.dist-info/WHEEL
 Comment: 
 
-Filename: steptools-20.1.dist-info/top_level.txt
+Filename: steptools-20.2.dist-info/top_level.txt
 Comment: 
 
-Filename: steptools-20.1.dist-info/RECORD
+Filename: steptools-20.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## steptools/step.pyi

```diff
@@ -9,15 +9,15 @@
 # follow that pattern and can not be split into more managable chunks.
 #
 # Also, be aware that there can be no tool tips for the EXPRESS or ARM
 # attributes because those are made available at run time based on the
 # underlying step data, and the IDEs seem to only use the static type
 # files, not anything at runtime.
 
-from typing import overload, Set, List, Union, Optional, Sequence, Callable
+from typing import overload, Any, Set, List, Union, Optional, Sequence, Callable, TypedDict
 from enum import IntEnum
 
 from _typeshed import (
     StrOrBytesPath
     )
 
 # ==================================================
@@ -235,15 +235,15 @@
         pass
 
 
 # ==================================================
 # ADAPTIVE PROCESS CURSOR CLASS
 #
 # 
-class RoseUnit(IntEnum,auto):
+class Unit(IntEnum,auto):
     '''Enumeration that identifies common units'''
     UNKNOWN = auto()
     AS_IS = auto()
     
     MM = auto()
     CM = auto()
     M = auto()
@@ -320,15 +320,15 @@
 
     MAX_VALUE = AUTO()
     def fullname(self) -> str:
         '''Return full descriptive name of unit enum''' 
         pass
 
     @classmethod
-    def find(cls, name:str) -> 'RoseUnit':
+    def find(cls, name:str) -> 'Unit':
         '''Return unit enum for full or abbreviated name'''
         pass
 
 
 class CtlEvent(IntEnum,auto):
     '''
     Identifies the different process conditions (Tool move,
@@ -545,18 +545,18 @@
         pass
     def get_active_param(self) -> float:
         '''
         Get numeric parameter associated with STEP object at current moment
         in process, such as a curve parameter or position within sequence.
         '''
         pass
-    def get_active_lenunit(self) -> RoseUnit:
+    def get_active_lenunit(self) -> Unit:
         '''Get length unit at current process location'''
         pass
-    def get_active_angunit(self) -> RoseUnit:
+    def get_active_angunit(self) -> Unit:
         '''Get angle unit at current process location'''
         pass
     
     def get_active_type(self) -> CtlType:
         '''Get type of process element at current process location'''
         pass
     def get_active_status(self) -> CtlStatus:
@@ -588,25 +588,25 @@
         '''Get position id for entire arc in WCS or optional CtlCsys'''
         pass
     def get_move_probe(self, csys: CtlCsys = CtlCsys.WCS) -> int:
         '''Get position id for entire probe in WCS or optional CtlCsys'''
         pass
 
 
-    def get_move_feed(self, u: RoseUnit = RoseUnit.AS_IS) -> float:
+    def get_move_feed(self, u: Unit = Unit.AS_IS) -> float:
         '''Get feedrate in effect with optional unit for conversion'''
         pass
-    def get_move_feed_unit(self) -> RoseUnit:
+    def get_move_feed_unit(self) -> Unit:
         '''Get feedrate unit used by the process.'''
         pass
 
-    def get_move_spindle(self, u: RoseUnit = RoseUnit.AS_IS) -> float:
+    def get_move_spindle(self, u: Unit = Unit.AS_IS) -> float:
         '''Get spindle speed in effect with optional unit for conversion'''
         pass
-    def get_move_spindle_unit(self) -> RoseUnit:
+    def get_move_spindle_unit(self) -> Unit:
         '''Get spindle speed unit used by the process.'''
         pass
 
 
     def get_move_is_rapid(self) -> bool:
         '''Return true if move is rapid.'''
         pass
@@ -617,36 +617,36 @@
         '''Return true if move has mist coolant on.'''
         pass
     def get_move_is_thru_coolant(self) -> bool:
         '''Return true if move has through-spindle coolant on.'''
         pass
 
 
-    def get_dwell_time(self, u: RoseUnit = RoseUnit.AS_IS) -> float:
+    def get_dwell_time(self, u: Unit = Unit.AS_IS) -> float:
         '''Get dwell time from a feedstop toolpath with optional unit for conversion'''
         pass
-    def get_dwell_time_unit(self) -> RoseUnit:
+    def get_dwell_time_unit(self) -> Unit:
         '''Get dwell time from a feedstop toolpath.'''
         pass
 
 
-    def get_pos_lenunit(self, posid: int) -> RoseUnit:
+    def get_pos_lenunit(self, posid: int) -> Unit:
         '''Get length unit for position id.'''
         pass
-    def get_pos_angunit(self, posid: int) -> RoseUnit:
+    def get_pos_angunit(self, posid: int) -> Unit:
         '''Get angle unit for position id.'''
         pass
     def get_pos_csys(self, posid: int) -> CtlCsys:
         '''Get coordinate system code for position id.'''
         pass
     def get_pos_type(self, posid: int) -> CtlPosType:
         '''Get type code for position id.'''
         pass
 
-    def get_pos_xyz(self, posid: int, u: RoseUnit = RoseUnit.AS_IS) -> tuple[float, float, float]:
+    def get_pos_xyz(self, posid: int, u: Unit = Unit.AS_IS) -> tuple[float, float, float]:
         '''Return (X,Y,Z) values for position id and optional unit for conversion.'''
         pass
 
     def get_pos_dirz(self, posid: int) -> tuple[float, float, float]:
         '''Return (i,j,k) of Z direction for position id.'''
         pass
     def get_pos_default_dirz(self, posid: int) -> tuple[float, float, float]:
@@ -666,15 +666,15 @@
     def get_pos_snorm_dir(self, posid: int) -> tuple[float, float, float]:
         '''Return (i,j,k) of surface normal direction for position id.'''
         pass
 
     def get_pos_speed_ratio(self, posid: int) -> float:
         '''Return speed ratio multiplier for position id.'''
         pass
-    def get_pos_xsect(self, posid: int, u: RoseUnit = RoseUnit.AS_IS) -> dict[str, float]
+    def get_pos_xsect(self, posid: int, u: Unit = Unit.AS_IS) -> dict[str, float]
         '''Return dictionary of cross section parameters for position id and optional unit for conversion.'''
         pass
     
     def get_pos_param(self, posid: int) -> float:
         '''Return the numeric parameter associated with the position id.'''
         pass
 
@@ -699,28 +699,28 @@
         pass
 
 
     def get_pos_is_equal(self, pos1: int, pos2: int) -> bool:
         '''Test whether two positions ids have same position, Z and X directions'''
         pass
 
-    def get_arc_center(self, posid: int, u: RoseUnit = RoseUnit.AS_IS) -> tuple[float, float, float]:
+    def get_arc_center(self, posid: int, u: Unit = Unit.AS_IS) -> tuple[float, float, float]:
         '''Return (X,Y,Z) values for center of arc position id with optional unit for conversion.'''
         pass
     def get_arc_axis(self, posid: int) -> tuple[float, float, float]:
         '''Return (i,j,k) values for axis of arc position id.'''
         pass
 
-    def get_arc_radius(self, posid: int, u: RoseUnit = RoseUnit.AS_IS) -> float:
+    def get_arc_radius(self, posid: int, u: Unit = Unit.AS_IS) -> float:
         '''Return radius value for arc position id with optional unit for conversion.'''
         pass
-    def get_arc_angle(self, posid: int, u: RoseUnit = RoseUnit.AS_IS) -> float:
+    def get_arc_angle(self, posid: int, u: Unit = Unit.AS_IS) -> float:
         '''Return angle value for arc position id with optional unit for conversion.'''
         pass
-    def get_arc_height(self, posid: int, u: RoseUnit = RoseUnit.AS_IS) -> float:
+    def get_arc_height(self, posid: int, u: Unit = Unit.AS_IS) -> float:
         '''Return helix height value for arc position id with optional unit for conversion.'''
         pass
 
     def get_arc_is_cw(self, posid: int) -> bool:
         '''Return true if arc position id is clockwise'''
         pass
     def get_arc_is_over180(self, posid: int) -> bool:
@@ -730,22 +730,22 @@
         '''Return true if arc position id is a complete circle'''
         pass
 
 
     def get_probe_direction(self, posid: int) -> tuple[float, float, float]:
         '''Return (i,j,k) values for direction of probe position id'''
         pass
-    def get_probe_end(self, posid: int, u: RoseUnit = RoseUnit.AS_IS) -> tuple[float, float, float]:
+    def get_probe_end(self, posid: int, u: Unit = Unit.AS_IS) -> tuple[float, float, float]:
         '''Return (X,Y,Z) values for end of probe position id with optional unit for conversion.'''
         pass
-    def get_probe_start(self, posid: int, u: RoseUnit = RoseUnit.AS_IS) -> tuple[float, float, float]:
+    def get_probe_start(self, posid: int, u: Unit = Unit.AS_IS) -> tuple[float, float, float]:
         '''Return (X,Y,Z) values for start of probe position id with optional unit for conversion.'''
         pass
 
-    def get_probe_expected(self, posid: int, u: RoseUnit = RoseUnit.AS_IS) -> float:
+    def get_probe_expected(self, posid: int, u: Unit = Unit.AS_IS) -> float:
         '''Return expected distance of probe position id with optional unit for conversion.'''
         pass
     
     def get_probe_expected_obj(self, posid: int) -> Object:
         '''Return STEP object for expected distance of probe position id.'''
         pass
 
@@ -781,18 +781,18 @@
     def get_frame_aux(self, idx: int, auxidx: int) -> Object:
         '''Return auxillary STEP object for stack frame'''
         pass
     
     def get_frame_param(self, idx: int) -> float:
         '''Return numeric parameter associated with STEP object for stack frame.'''
         pass
-    def get_frame_lenunit(self, idx: int) -> RoseUnit:
+    def get_frame_lenunit(self, idx: int) -> Unit:
         '''Return length unit for stack frame'''
         pass
-    def get_frame_angunit(self, idx: int) -> RoseUnit:
+    def get_frame_angunit(self, idx: int) -> Unit:
         '''Return angle unit for stack frame'''
         pass
     
     def get_frame_type(self, idx: int) -> CtlType:
         '''Return event type for stack frame'''
         pass
     def get_frame_status(self, idx: int) -> CtlStatus:
@@ -1021,48 +1021,48 @@
     def get_program_number(self) -> int:
         '''Program number for fanuc and some other code styles.'''
         pass
     def set_program_number(self, pn: int) -> None:
         '''Program number for fanuc and some other code styles.'''
         pass
 
-    def get_program_unit(self) -> RoseUnit:
+    def get_program_unit(self) -> Unit:
         '''Preferred length unit to use when generating code.'''
         pass
-    def set_program_unit(self, u: RoseUnit) -> None:
+    def set_program_unit(self, u: Unit) -> None:
         '''Preferred length unit to use when generating code.'''
         pass
     
     
     def set_unit_system(self, cursor: Adaptive) -> None:
         '''
         Set length, feed, and spindle to match the program units.
         If AS_IS, use length unit of toolpaths from cursor.
         '''
         pass
 
     
-    def get_len_unit(self) -> RoseUnit:
+    def get_len_unit(self) -> Unit:
         '''Length unit to use when generating coordinates in code.'''
         pass
-    def set_len_unit(self, u: RoseUnit) -> None:
+    def set_len_unit(self, u: Unit) -> None:
         '''Length unit to use when generating coordinates in code.'''
         pass
 
-    def get_feed_unit(self) -> RoseUnit:
+    def get_feed_unit(self) -> Unit:
         '''Feedrate unit to use when generating feed commands in code.'''
         pass
-    def set_feed_unit(self, u: RoseUnit) -> None:
+    def set_feed_unit(self, u: Unit) -> None:
         '''Feedrate unit to use when generating feed commands in code.'''
         pass
 
-    def get_spindle_unit(self) -> RoseUnit:
+    def get_spindle_unit(self) -> Unit:
         '''Spindle speed unit to use when generating spindle commands in code.'''
         pass
-    def set_spindle_unit(self, u: RoseUnit) -> None:
+    def set_spindle_unit(self, u: Unit) -> None:
         '''Spindle speed unit to use when generating spindle commands in code.'''
         pass
 
     def get_move_is_modal(self) -> bool:
         '''
         Modal move emits G0/G1 once at start of a series of moves.
         Non-modal move emits the G0/G1 command for every move.
@@ -1183,15 +1183,15 @@
     
     def is_formatted_ijk(self,
                          i1: float, j1: float, k1: float,
                          i2: float, j2: float, k2: float) -> bool:
         '''Do two sets of IJK numbers result in the same formatted values.'''
         pass
     
-    def get_out_xyz(self, cursor: Adaptive, pos: int, u: RoseUnit = RoseUnit.AS_IS) -> tuple[float, float, float]:
+    def get_out_xyz(self, cursor: Adaptive, pos: int, u: Unit = Unit.AS_IS) -> tuple[float, float, float]:
         '''Return (X,Y,Z) values for position id with output transform applied and optional unit conversion'''
         pass
 
     def get_out_dirz(self, cursor: Adaptive, pos: int) -> tuple[float, float, float]:
         '''Return (i,j,k) of Z direction for position id with output transform applied.'''
         pass
     def get_out_dirx(self, cursor: Adaptive, pos: int) -> tuple[float, float, float]:
@@ -1201,15 +1201,15 @@
         '''Return (i,j,k) of surface normal direction for position id with output transform applied.'''
         pass
     def get_out_move_dir(self, cursor: Adaptive, pos: int) -> tuple[float, float, float]:
         '''Return (i,j,k) of move direction for position id with output transform applied.'''
         pass
 
     
-    def get_out_arc_center(self, cursor: Adaptive, pos: int, u: RoseUnit = RoseUnit.AS_IS) -> tuple[float, float, float]:
+    def get_out_arc_center(self, cursor: Adaptive, pos: int, u: Unit = Unit.AS_IS) -> tuple[float, float, float]:
         '''Return (X,Y,Z) values for center of arc position id with output transform applied and optional unit conversion'''
         pass
     def get_out_arc_axis(self, cursor: Adaptive, pos: int) -> tuple[float, float, float]:
         '''Return (i,j,k) of axis of arc position id with output transform applied.'''
         pass
     
 
@@ -2607,14 +2607,391 @@
 	    a: float = 1, b: float = 0, c: float = 0) -> None:
         '''Add setup placement to workplan.'''
         pass
 
 
     
 # ==================================================
+# FINDER API CLASS
+#
+
+class FinderBounds(TypedDict):
+    value: float
+    unit: Unit
+    lower: float
+    lower_reason: str
+    upper: float
+    upper_reason: str
+    
+class FinderAPI:
+    '''High level API for examining process contents'''
+    @classmethod
+    def design(cls) -> Design:
+        '''Get the current design object.'''
+        pass
+    @classmethod
+    def open_project(cls, filename: StrOrBytesPath) -> Design:
+        '''Read STEP or STEP-NC file.'''
+        pass
+
+
+    @classmethod
+    def get_probe_ball_radius(cls, ws_or_tool: Object) -> float:
+        '''Get ball radius of probe tool.'''
+        pass
+    @classmethod
+    def get_probe_ball_radius_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get unit for ball radius of probe tool.'''
+        pass
+    @classmethod
+    def get_probe_ball_radius_bounds(cls, ws_or_tool: Object) -> FinderBounds:
+        '''Get upper/lower value bounds for ball radius of probe tool.'''
+        pass
+
+    @classmethod
+    def get_probe_stylus_diameter(cls, ws_or_tool: Object) -> float:
+        '''Get stylus diameter of probe tool.'''
+        pass
+    @classmethod
+    def get_probe_stylus_diameter_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get unit for stylus diameter of probe tool.'''
+        pass
+    @classmethod
+    def get_probe_stylus_diameter_bounds(cls, ws_or_tool: Object) -> FinderBounds:
+        '''Get upper/lower value bounds for stylus diameter of probe tool.'''
+        pass
+
+    @classmethod
+    def get_tool_all(cls) -> List[Object]:
+        '''Get a list of all tool objects'''
+        pass
+    def get_tool_category(cls, ws_or_tool: Object) -> str:
+        '''Get string description of tool category'''
+        pass
+    @classmethod
+    def get_tool_coolant_through_tool(cls, ws_or_tool: Object) -> bool:
+        '''Get whether coolant through tool is supported.'''
+        pass
+
+    @classmethod
+    def get_tool_corner_radius(cls, ws_or_tool: Object) -> float:
+        '''Get corner radius of tool.'''
+        pass
+    @classmethod
+    def get_tool_corner_radius_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get unit for corner radius of tool.'''
+        pass
+    @classmethod
+    def get_tool_corner_radius_bounds(cls, ws_or_tool: Object) -> FinderBounds:
+        '''Get upper/lower value bounds for corner radius of tool.'''
+        pass
+
+    @classmethod
+    def get_tool_current_diameter(cls, ws_or_tool: Object) -> Tuple[float,float]
+        '''Get nominal and current diameter of tool.'''
+        pass
+    @classmethod
+    def get_tool_current_length(cls, ws_or_tool: Object) -> Tuple[float,float]
+        '''Get nominal and current length of tool.'''
+        pass
+    @classmethod
+    def get_tool_current_corner_radius(cls, ws_or_tool: Object) -> Tuple[float,float]
+        '''Get nominal and current radius of tool.'''
+        pass
+
+    @classmethod
+    def get_tool_diameter(cls, ws_or_tool: Object) -> float:
+        '''Get diameter of tool.'''
+        pass
+    @classmethod
+    def get_tool_diameter_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get unit for diameter of tool.'''
+        pass
+    @classmethod
+    def get_tool_diameter_bounds(cls, ws_or_tool: Object) -> FinderBounds:
+        '''Get upper/lower value bounds for diameter of tool.'''
+        pass
+
+    @classmethod
+    def get_tool_expected_life(cls, ws_or_tool: Object) -> float:
+        '''Get expected life of tool.'''
+        pass
+    @classmethod
+    def get_tool_expected_life_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get unit for expected life of tool.'''
+        pass
+    @classmethod
+    def get_tool_expected_life_bounds(cls, ws_or_tool: Object) -> FinderBounds:
+        '''Get upper/lower value bounds for expected life of tool.'''
+        pass
+
+    @classmethod
+    def get_tool_flute_count(cls, ws_or_tool: Object) -> float:
+        '''Get number of flutes of tool.'''
+        pass
+    @classmethod
+    def get_tool_flute_length(cls, ws_or_tool: Object) -> float:
+        '''Get flute length of tool.'''
+        pass
+    @classmethod
+    def get_tool_flute_length_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get unit for flute length of tool.'''
+        pass
+    @classmethod
+    def get_tool_flute_length_bounds(cls, ws_or_tool: Object) -> FinderBounds:
+        '''Get upper/lower value bounds for flute length of tool.'''
+        pass
+
+    @classmethod
+    def get_tool_functional_length(cls, ws_or_tool: Object) -> float:
+        '''Get functional length of tool.'''
+        pass
+    @classmethod
+    def get_tool_functional_length_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get unit for functional length of tool.'''
+        pass
+
+    @classmethod
+    def get_tool_geometry_length_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get length unit for geometry of tool.'''
+        pass
+
+    @classmethod
+    def get_tool_hand_of_cut(cls, ws_or_tool: Object) -> str:
+        '''Get hand of cut of tool'''
+        pass
+    
+    @classmethod
+    def get_tool_horizontal_distance(cls, ws_or_tool: Object) -> float:
+        '''Get horizontal distance of tool.'''
+        pass
+    @classmethod
+    def get_tool_horizontal_distance_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get unit for horizontal distance length of tool.'''
+        pass
+
+
+    @classmethod
+    def get_tool_identifier(cls, ws_or_tool: Object) -> str:
+        '''Get manufacturers name for a tool'''
+        pass
+    
+    @classmethod
+    def get_tool_iso13399_atts(cls, ws_or_tool: Object) -> dict[str, Any]
+        '''Get ISO 13399 attribute dictionary for a tool'''
+        pass
+
+    @classmethod
+    def get_tool_length(cls, ws_or_tool: Object) -> float:
+        '''Get length of tool.'''
+        pass
+    @classmethod
+    def get_tool_length_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get unit for length of tool.'''
+        pass
+    @classmethod
+    def get_tool_length_bounds(cls, ws_or_tool: Object) -> FinderBounds:
+        '''Get upper/lower value bounds for length of tool.'''
+        pass
+
+    @classmethod
+    def get_tool_material(cls, ws_or_tool: Object) -> str:
+        '''Get material of tool'''
+        pass
+    @classmethod
+    def get_tool_material_standard(cls, ws_or_tool: Object) -> str:
+        '''Get material standard of tool'''
+        pass
+    
+    @classmethod
+    def get_tool_number(cls, ws_or_tool: Object) -> str:
+        '''Get number of tool'''
+        pass
+    @classmethod
+    def get_tool_number_as_number(cls, ws_or_tool: Object) -> int:
+        '''Get number of tool'''
+        pass
+
+    @classmethod
+    def get_tool_overall_length(cls, ws_or_tool: Object) -> float:
+        '''Get overall assembly length of tool.'''
+        pass
+    @classmethod
+    def get_tool_overall_length_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get unit for overall assembly length of tool.'''
+        pass
+    @classmethod
+    def get_tool_overall_length_bounds(cls, ws_or_tool: Object) -> FinderBounds:
+        '''Get upper/lower value bounds for overall assembly length of tool.'''
+        pass
+
+    @classmethod
+    def get_tool_part_name(cls, ws_or_tool: Object) -> str:
+        '''Get part name for a tool'''
+        pass
+    
+    @classmethod
+    def get_tool_recommended_feed(cls, ws_or_tool: Object) -> float:
+        '''Get recommended feedrate of tool.'''
+        pass
+    @classmethod
+    def get_tool_recommended_feed_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get unit for recommended feedrate of tool.'''
+        pass
+    @classmethod
+    def get_tool_recommended_feed_bounds(cls, ws_or_tool: Object) -> FinderBounds:
+        '''Get upper/lower value bounds for recommended feedrate of tool.'''
+        pass
+
+    @classmethod
+    def get_tool_recommended_speed(cls, ws_or_tool: Object) -> float:
+        '''Get recommended spindle speed of tool.'''
+        pass
+    @classmethod
+    def get_tool_recommended_speed_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get unit for recommended spindle speed of tool.'''
+        pass
+    @classmethod
+    def get_tool_recommended_speed_bounds(cls, ws_or_tool: Object) -> FinderBounds:
+        '''Get upper/lower value bounds for recommended spindle speed of tool.'''
+        pass
+
+    @classmethod
+    def get_tool_similar(
+            cls, ws_or_tool: Object,
+            tooltype: bool = False,
+	    diameter: bool = False,
+	    length: bool = False,
+	    radius: bool = False,
+	    flute_count: bool = False,
+	    manufacturer: bool = False) -> List[Object]:
+        '''Get list of tools matching certain parameters'''
+        pass
+
+    @classmethod
+    def get_tool_mill_matching(
+            cls, 
+	    diameter: float = 0,
+	    length: float = 0,
+	    radius: float = 0,
+	    flute_count: float = 0,
+	    tooltype: str = None) ->; List[Object]:
+        '''Get list of milling tools matching certain parameters'''
+        pass
+    
+    @classmethod
+    def get_tool_drill_matching(
+            cls, 
+	    diameter: float = 0,
+	    length: float = 0,
+	    tip_angle: float = 0,
+	    tooltype: str = None) -> List[Object]:
+        '''Get list of drilling tools matching certain parameters'''
+        pass
+    
+    @classmethod
+    def get_tool_taper_angle(cls, ws_or_tool: Object) -> float:
+        '''Get taper angle of tool.'''
+        pass
+    @classmethod
+    def get_tool_taper_angle_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get unit for taper angle of tool.'''
+        pass
+    @classmethod
+    def get_tool_taper_angle_bounds(cls, ws_or_tool: Object) -> FinderBounds:
+        '''Get upper/lower value bounds for taper angle of tool.'''
+        pass
+
+    @classmethod
+    def get_tool_technology(cls, tool: Object) -> List[Object]:
+        '''Get list of technologies used by tool'''
+        pass
+
+    @classmethod
+    def get_tool_thread_form_type(cls, ws_or_tool: Object) -> str:
+        '''Get thread taper form type of tool'''
+        pass
+    @classmethod
+    def get_tool_thread_taper_count(cls, ws_or_tool: Object) -> float:
+        '''Get thread taper count of tool'''
+        pass
+
+    @classmethod
+    def get_tool_thread_pitch(cls, ws_or_tool: Object) -> float:
+        '''Get thread pitch of tool.'''
+        pass
+    @classmethod
+    def get_tool_thread_pitch_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get unit for thread pitch of tool.'''
+        pass
+    @classmethod
+    def get_tool_thread_pitch_bounds(cls, ws_or_tool: Object) -> FinderBounds:
+        '''Get upper/lower value bounds for thread pitch of tool.'''
+        pass
+
+    @classmethod
+    def get_tool_thread_size(cls, ws_or_tool: Object) -> float:
+        '''Get thread size of tool.'''
+        pass
+    @classmethod
+    def get_tool_thread_size_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get unit for thread size of tool.'''
+        pass
+    @classmethod
+    def get_tool_thread_size_bounds(cls, ws_or_tool: Object) -> FinderBounds:
+        '''Get upper/lower value bounds for thread size of tool.'''
+        pass
+    
+    @classmethod
+    def get_tool_tip_angle(cls, ws_or_tool: Object) -> float:
+        '''Get tip angle of tool'''
+        pass
+    @classmethod
+    def get_tool_tip_angle_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get unit for tip angle of tool'''
+        pass
+    @classmethod
+    def get_tool_tip_angle_bounds(cls, ws_or_tool: Object) -> FinderBounds:
+        '''Get upper/lower value bounds for tip angle of tool'''
+        pass
+    @classmethod
+    def get_tool_type(cls, ws_or_tool: Object) -> str:
+        '''Get string type of tool'''
+        pass
+
+    @classmethod
+    def get_tool_using_identifier(cls, mfg_id: str) -> Object:
+        '''Get tool by manufacturers name'''
+        pass
+    @classmethod
+    def get_tool_using_number(cls, num_id: str) -> Object:
+        '''Get tool by number id'''
+        pass
+    @classmethod
+    def get_tool_using_workpiece(cls, workpiece: Object) -> Object:
+        '''Get tool by geometry workpiece object'''
+        pass
+    
+    @classmethod
+    def get_tool_vertical_distance(cls, ws_or_tool: Object) -> float:
+        '''Get vertical distance of tool.'''
+        pass
+    @classmethod
+    def get_tool_vertical_distance_unit(cls, ws_or_tool: Object) -> Unit:
+        '''Get unit for vertical distance length of tool.'''
+        pass
+    
+    def get_tool_workpiece(cls, ws_or_tool: Object) -> Object:
+        '''Get workpiece that defines geometry of tool'''
+        pass
+
+
+
+    
+# ==================================================
 # TOLERANCE API CLASS
 #
 class ToleranceAPI:
     '''High level API for tolerance related operations'''
 
     @classmethod
     def add_workpiece_hardness(cls, workpiece: Object, value: float, measuring_method: str) -> Object:
@@ -2814,15 +3191,15 @@
 
     @classmethod
     def compose_rotation(
             self, xf: Sequence[float],
             axis: Sequence[float],
             origin: Sequence[float],
             angle: float,
-            angle_unit: RoseUnit = RoseUnit.RAD
+            angle_unit: Unit = Unit.RAD
     ) -> List[float]:
         '''Return matrix resulting from rotation applied to a source matrix, given an axis, angle and origin'''
         pass
 
     @classmethod
     def compose_scale(self, xf: Sequence[float], scale: float) -> List[float]:
         '''Return matrix resulting from scaling applied to a source matrix'''
@@ -2831,15 +3208,15 @@
     
     @classmethod
     def det(self, xf: Sequence[float]) -> float:
         '''Return determinant of the 4x4 transform matrix'''
         pass
 
     @classmethod
-    def get_euler_angles(self, xf: Sequence[float], angle_unit: RoseUnit = RoseUnit.RAD) -> Tuple[float,float,float]
+    def get_euler_angles(self, xf: Sequence[float], angle_unit: Unit = Unit.RAD) -> Tuple[float,float,float]
         '''Return Euler angles for the rotation portion of transform, computed by ZXZ convention'''
         pass
     
     @classmethod
     def identity(self) -> List[float]:
         '''Return identity matrix'''
         pass
```

## Comparing `steptools-20.1.dist-info/LICENSE` & `steptools-20.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `steptools-20.1.dist-info/METADATA` & `steptools-20.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steptools
-Version: 20.1
+Version: 20.2
 Summary: STEP and STEP-NC (ISO 10303) native extension for large CAD/CAM/CAE models and machine tool interfaces.
 Author-email: "STEP Tools, Inc" <support@steptools.com>
 License: 
         STEP Python Interface
         END USER LICENSE AGREEMENT
         REDISTRIBUTION NOT PERMITTED        
         STEP Tools, Inc. ("STI") grants you ("Customer") a non-exclusive,
```

## Comparing `steptools-20.1.dist-info/RECORD` & `steptools-20.2.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 steptools/py.typed,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-steptools/step.pyd,sha256=ixSEgVfbJwRwTs90WNQxllgfMzhuYo8_MXTet30J4Ak,30832360
-steptools/step.pyi,sha256=ysnryjjUvwv8bGDgBSrnLtxWpT_al7GT84ghHOFOOuI,107772
-steptools-20.1.dist-info/LICENSE,sha256=95amYWPb2yYw4mlPrV5p700ZxQc4vF6T7PMfLNDqqdk,3043
-steptools-20.1.dist-info/METADATA,sha256=6aLp0XqZKj_8vDwlm4f8v83Lhm5Lee_PhRTc4A2J6ik,7014
-steptools-20.1.dist-info/WHEEL,sha256=QoQ88D2Q13BOm7mJoRsoyU9fyfiVmeZqJb4AUpJxoBg,100
-steptools-20.1.dist-info/top_level.txt,sha256=makmMXVcR2PLphCyKXpEBALUpobuOltlpF-6P2Xkhas,15
-steptools-20.1.dist-info/RECORD,,
+steptools/step.pyd,sha256=OMYYE6UN-YdLoFPQ0Z5YkVxa8bo2NH3-02ZMc2ydXsM,30931688
+steptools/step.pyi,sha256=VlxE2iPZArMbpNFWJvL9x9yFl5DrSty-IuPAxaUPDJw,120367
+steptools-20.2.dist-info/LICENSE,sha256=95amYWPb2yYw4mlPrV5p700ZxQc4vF6T7PMfLNDqqdk,3043
+steptools-20.2.dist-info/METADATA,sha256=xCb5xRMfMyM2kC-vDWIc3c8UIQo_mGz0oCePdoiYXCg,7014
+steptools-20.2.dist-info/WHEEL,sha256=QoQ88D2Q13BOm7mJoRsoyU9fyfiVmeZqJb4AUpJxoBg,100
+steptools-20.2.dist-info/top_level.txt,sha256=makmMXVcR2PLphCyKXpEBALUpobuOltlpF-6P2Xkhas,15
+steptools-20.2.dist-info/RECORD,,
```

