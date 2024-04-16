# Comparing `tmp/paicorelib-0.0.9.tar.gz` & `tmp/paicorelib-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paicorelib-0.0.9.tar", max compression
+gzip compressed data, was "paicorelib-1.0.0rc1.tar", max compression
```

## Comparing `paicorelib-0.0.9.tar` & `paicorelib-1.0.0rc1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0    35149 2024-01-16 02:40:54.542690 paicorelib-0.0.9/LICENSE
--rw-r--r--   0        0        0      847 2024-01-16 02:40:54.542690 paicorelib-0.0.9/README.md
--rw-r--r--   0        0        0     1408 2024-01-16 02:40:54.542690 paicorelib-0.0.9/paicorelib/__init__.py
--rw-r--r--   0        0        0    14720 2024-01-16 02:40:54.542690 paicorelib-0.0.9/paicorelib/coordinate.py
--rw-r--r--   0        0        0       75 2024-01-16 02:40:54.542690 paicorelib-0.0.9/paicorelib/framelib/__init__.py
--rw-r--r--   0        0        0      706 2024-01-16 02:40:54.542690 paicorelib-0.0.9/paicorelib/framelib/_types.py
--rw-r--r--   0        0        0     5104 2024-01-16 02:40:54.542690 paicorelib-0.0.9/paicorelib/framelib/base.py
--rw-r--r--   0        0        0     7150 2024-01-16 02:40:54.542690 paicorelib-0.0.9/paicorelib/framelib/frame_defs.py
--rw-r--r--   0        0        0     9969 2024-01-16 02:40:54.542690 paicorelib-0.0.9/paicorelib/framelib/frame_gen.py
--rw-r--r--   0        0        0    21856 2024-01-16 02:40:54.542690 paicorelib-0.0.9/paicorelib/framelib/frames.py
--rw-r--r--   0        0        0     5199 2024-01-16 02:40:54.542690 paicorelib-0.0.9/paicorelib/framelib/utils.py
--rw-r--r--   0        0        0     1461 2024-01-16 02:40:54.542690 paicorelib-0.0.9/paicorelib/hw_defs.py
--rw-r--r--   0        0        0     2365 2024-01-16 02:40:54.542690 paicorelib-0.0.9/paicorelib/hw_types.py
--rw-r--r--   0        0        0     7973 2024-01-16 02:40:54.542690 paicorelib-0.0.9/paicorelib/ram_model.py
--rw-r--r--   0        0        0     2654 2024-01-16 02:40:54.542690 paicorelib-0.0.9/paicorelib/ram_types.py
--rw-r--r--   0        0        0     5867 2024-01-16 02:40:54.542690 paicorelib-0.0.9/paicorelib/reg_model.py
--rw-r--r--   0        0        0     3904 2024-01-16 02:40:54.542690 paicorelib-0.0.9/paicorelib/reg_types.py
--rw-r--r--   0        0        0     5022 2024-01-16 02:40:54.542690 paicorelib-0.0.9/paicorelib/routing_defs.py
--rw-r--r--   0        0        0      996 2024-01-16 02:40:54.542690 paicorelib-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1834 1970-01-01 00:00:00.000000 paicorelib-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0       63 2024-04-16 07:52:04.051343 paicorelib-1.0.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0      888 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/README.md
+-rw-r--r--   0        0        0     1742 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/docs/Table-of-Terms.md
+-rw-r--r--   0        0        0     1189 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/__init__.py
+-rw-r--r--   0        0        0    14867 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/coordinate.py
+-rw-r--r--   0        0        0       75 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/framelib/__init__.py
+-rw-r--r--   0        0        0     5142 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/framelib/base.py
+-rw-r--r--   0        0        0     7150 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/framelib/frame_defs.py
+-rw-r--r--   0        0        0     9920 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/framelib/frame_gen.py
+-rw-r--r--   0        0        0    21957 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/framelib/frames.py
+-rw-r--r--   0        0        0      706 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/framelib/types.py
+-rw-r--r--   0        0        0     3988 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/framelib/utils.py
+-rw-r--r--   0        0        0     1461 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/hw_defs.py
+-rw-r--r--   0        0        0     2312 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/hw_types.py
+-rw-r--r--   0        0        0     7472 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/ram_model.py
+-rw-r--r--   0        0        0     2618 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/ram_types.py
+-rw-r--r--   0        0        0     5844 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/reg_model.py
+-rw-r--r--   0        0        0     4265 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/reg_types.py
+-rw-r--r--   0        0        0     5174 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/paicorelib/routing_defs.py
+-rw-r--r--   0        0        0     1571 2024-04-16 07:52:04.055343 paicorelib-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 paicorelib-1.0.0rc1/PKG-INFO
```

### Comparing `paicorelib-0.0.9/LICENSE` & `paicorelib-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `paicorelib-0.0.9/README.md` & `paicorelib-1.0.0rc1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIlib/blob/master/pyproject.toml">
         <img src="https://img.shields.io/pypi/pyversions/paicorelib">
     </a>
-    <a href="https://github.com/PAICookers/PAIlib/releases/tag/v0.0.9">
-        <img src="https://img.shields.io/github/v/release/PAICookers/PAIlib?color=orange">
+    <a href="https://github.com/PAICookers/PAIlib/releases/tag/v1.0.0rc1">
+        <img src="https://img.shields.io/github/v/release/PAICookers/PAIlib?include_prereleases&color=orange">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIlib">
       <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIlib/master?color=red">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIlib/master">
 	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIlib/master.svg" alt="pre-commit.ci status">
     </a>
 
 </p>
 
-This is the library of PAIBox & runtime.
+术语对照表：[Table of Terms](docs/Table-of-Terms.md)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
                            # Library of PAICORE 2.0
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_p_a_i_c_o_r_e_l_i_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-   _g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_l_i_b_?_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-   _c_o_d_e_f_a_c_t_o_r_/_g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_l_i_b_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
-                                    _s_t_a_t_u_s_]
-This is the library of PAIBox & runtime.
+ _g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_l_i_b_?_i_n_c_l_u_d_e___p_r_e_r_e_l_e_a_s_e_s_&_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/_g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_l_i_b_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-
+                               _c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
+æ¯è¯­å¯¹ç§è¡¨ï¼[Table of Terms](docs/Table-of-Terms.md)
```

### Comparing `paicorelib-0.0.9/paicorelib/__init__.py` & `paicorelib-1.0.0rc1/paicorelib/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from .coordinate import *
 from .framelib import *
 
 # In recent versions, `HwConfig` for external packages remain unchanged.
 from .hw_defs import HwParams as HwConfig
 from .hw_types import *
 from .ram_model import *
-from .ram_types import LeakingComparisonMode as LCM
-from .ram_types import LeakingDirectionMode as LDM
-from .ram_types import LeakingIntegrationMode as LIM
+from .ram_types import LeakComparisonMode as LCM
+from .ram_types import LeakDirectionMode as LDM
+from .ram_types import LeakIntegrationMode as LIM
 from .ram_types import NegativeThresholdMode as NTM
 from .ram_types import ResetMode as RM
 from .ram_types import SynapticIntegrationMode as SIM
 from .ram_types import ThresholdMode as TM
 from .reg_model import *
 from .reg_types import CoreMode as CoreMode
 from .reg_types import CoreModeDict as CoreModeDict
@@ -19,24 +19,14 @@
 from .reg_types import LCNExtensionType as LCN_EX
 from .reg_types import MaxPoolingEnableType as MaxPoolingEnable
 from .reg_types import SNNModeEnableType as SNNModeEnable
 from .reg_types import SpikeWidthFormatType as SpikeWidthFormat
 from .reg_types import WeightPrecisionType as WeightPrecision
 from .routing_defs import *
 
-__major__ = 0
-__minor__ = 0
-__revision__ = 9
-__version__ = f"{__major__}.{__minor__}.{__revision__}"
 
+from importlib.metadata import version
 
-def get_version_json():
-    return {
-        "major": __major__,
-        "minor": __minor__,
-        "revision": __revision__,
-        "version": __version__,
-    }
-
-
-def get_version():
-    return (__major__, __minor__, __revision__)
+try:
+    __version__ = version("paicorelib")
+except Exception:
+    __version__ = None
```

### Comparing `paicorelib-0.0.9/paicorelib/coordinate.py` & `paicorelib-1.0.0rc1/paicorelib/coordinate.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 
 CoordTuple: TypeAlias = Tuple[int, int]
 
 
 def _xy_parser(other: Union[CoordTuple, "CoordOffset"]) -> CoordTuple:
     """Parse the coordinate in tuple format."""
     if not isinstance(other, (tuple, CoordOffset)):
-        raise TypeError(f"Unsupported type: {type(other)}")
+        raise TypeError(f"unsupported type: {type(other)}.")
 
     if isinstance(other, tuple):
         if len(other) != 2:
-            raise ValueError(f"Expect a tuple of 2 elements, but got {len(other)}.")
+            raise ValueError(f"expected a tuple of 2 elements, but got {len(other)}.")
 
         return CoordOffset.from_tuple(other).to_tuple()
     else:
         return other.to_tuple()
 
 
 class _CoordIdentifier(ABC):
@@ -88,15 +88,15 @@
         >>> c2 = c1 + CoordOffset(1, 1)
         >>> c1
         >>> Coord(2, 2)
 
         NOTE: `Coord` + `Coord` is meaningless.
         """
         if not isinstance(__other, CoordOffset):
-            raise TypeError(f"Unsupported type: {type(__other)}")
+            raise TypeError(f"unsupported type: {type(__other)}.")
 
         sum_x, sum_y = _sum_carry(self.x + __other.delta_x, self.y + __other.delta_y)
 
         return Coord(sum_x, sum_y)
 
     def __iadd__(self, __other: Union[CoordTuple, "CoordOffset"]) -> "Coord":
         """
@@ -108,41 +108,39 @@
         """
         bx, by = _xy_parser(__other)
         self.x, self.y = _sum_carry(self.x + bx, self.y + by)
 
         return self
 
     @overload
-    def __sub__(self, __other: "Coord") -> "CoordOffset":
-        ...
+    def __sub__(self, __other: "Coord") -> "CoordOffset": ...
 
     @overload
-    def __sub__(self, __other: "CoordOffset") -> "Coord":
-        ...
+    def __sub__(self, __other: "CoordOffset") -> "Coord": ...
 
     def __sub__(
         self, __other: Union["Coord", "CoordOffset"]
     ) -> Union["Coord", "CoordOffset"]:
         """
         Example:
         >>> c1 = Coord(1, 1)
         >>> c2 = Coord(2, 2) - c1
         >>> c2
         >>> CoordOffset(1, 1)
         """
         if isinstance(__other, Coord):
             return CoordOffset(self.x - __other.x, self.y - __other.y)
 
-        if isinstance(__other, CoordOffset):
+        elif isinstance(__other, CoordOffset):
             diff_x, diff_y = _sum_carry(
                 self.x - __other.delta_x, self.y - __other.delta_y
             )
             return Coord(diff_x, diff_y)
-
-        raise TypeError(f"Unsupported type: {type(__other)}")
+        else:
+            raise TypeError(f"unsupported type: {type(__other)}.")
 
     def __isub__(self, __other: Union[CoordTuple, "CoordOffset"]) -> "Coord":
         """
         Example:
         >>> c1 = Coord(2, 2)
         >>> c1 -= CoordOffset(1, 1)
         >>> c1
@@ -162,15 +160,15 @@
         >>> False
         """
         if isinstance(__other, tuple):
             return self.to_tuple() == __other
         elif isinstance(__other, Coord):
             return self.x == __other.x and self.y == __other.y
         else:
-            raise TypeError(f"Unsupported type: {type(__other)}")
+            raise TypeError(f"unsupported type: {type(__other)}.")
 
     def __ne__(self, __other: Union[CoordTuple, "Coord"]) -> bool:
         return not self.__eq__(__other)
 
     # def __lt__(self, __other: "Coord") -> bool:
     #     """Whether the coord is on the left OR below of __other.
 
@@ -238,14 +236,18 @@
     def address(self) -> int:
         """Convert to address, 10 bits"""
         return (self.x << HwParams.N_BIT_CORE_Y) | self.y
 
 
 @final
 class ReplicationId(Coord):
+    @classmethod
+    def from_addr(cls, addr: int) -> "ReplicationId":
+        return cls(addr >> HwParams.N_BIT_CORE_Y, addr & HwParams.CORE_Y_MAX)
+
     def __and__(self, __other: Union[Coord, "ReplicationId"]) -> "ReplicationId":
         return ReplicationId(self.x & __other.x, self.y & __other.y)
 
     def __or__(self, __other: Union[Coord, "ReplicationId"]) -> "ReplicationId":
         return ReplicationId(self.x | __other.x, self.y | __other.y)
 
     def __xor__(self, __other: Union[Coord, "ReplicationId"]) -> "ReplicationId":
@@ -276,20 +278,18 @@
     )
 
     @classmethod
     def from_tuple(cls, pos: CoordTuple) -> "CoordOffset":
         return cls(*pos)
 
     @overload
-    def __add__(self, __other: Coord) -> Coord:
-        ...
+    def __add__(self, __other: Coord) -> Coord: ...
 
     @overload
-    def __add__(self, __other: "CoordOffset") -> "CoordOffset":
-        ...
+    def __add__(self, __other: "CoordOffset") -> "CoordOffset": ...
 
     def __add__(
         self, __other: Union["CoordOffset", Coord]
     ) -> Union["CoordOffset", Coord]:
         """
         Examples:
         >>> delta_c1 = CoordOffset(1, 1)
@@ -311,15 +311,15 @@
             )
         elif isinstance(__other, Coord):
             sum_x, sum_y = _sum_carry(
                 self.delta_x + __other.x, self.delta_y + __other.y
             )
             return Coord(sum_x, sum_y)
         else:
-            raise TypeError(f"Unsupported type: {type(__other)}")
+            raise TypeError(f"unsupported type: {type(__other)}.")
 
     def __iadd__(self, __other: Union[CoordTuple, "CoordOffset"]) -> "CoordOffset":
         """
         Example:
         >>> delta_c = CoordOffset(1, 1)
         >>> delta_c += CoordOffset(1, 1)
         >>> delta_c
@@ -338,15 +338,15 @@
         >>> delta_c1 = CoordOffset(1, 1)
         >>> delta_c2 = CoordOffset(2, 2)
         >>> delta_c = delta_c1 - delta_c2
         >>> delta_c
         >>> CoordOffset(-1, -1)
         """
         if not isinstance(__other, CoordOffset):
-            raise TypeError(f"Unsupported type: {type(__other)}")
+            raise TypeError(f"unsupported type: {type(__other)}.")
 
         return CoordOffset(
             self.delta_x - __other.delta_x, self.delta_y - __other.delta_y
         )
 
     def __isub__(self, __other: Union[CoordTuple, "CoordOffset"]) -> "CoordOffset":
         """
@@ -370,15 +370,15 @@
         >>> False
         """
         if isinstance(__other, tuple):
             return self.to_tuple() == __other
         elif isinstance(__other, CoordOffset):
             return self.delta_x == __other.delta_x and self.delta_y == __other.delta_y
         else:
-            raise TypeError(f"Unsupported type: {type(__other)}")
+            raise TypeError(f"unsupported type: {type(__other)}.")
 
     def __ne__(self, __other: "CoordOffset") -> bool:
         return not self.__eq__(__other)
 
     def to_tuple(self) -> CoordTuple:
         """Convert to tuple"""
         return (self.delta_x, self.delta_y)
@@ -407,15 +407,15 @@
         return max(abs(self.delta_x), abs(self.delta_y))
 
     def _check(self) -> None:
         if (not -HwParams.CORE_X_MAX <= self.delta_x <= HwParams.CORE_X_MAX) or (
             not -HwParams.CORE_Y_MAX <= self.delta_y <= HwParams.CORE_Y_MAX
         ):
             raise ValueError(
-                f"Offset of coordinate is out of range: ({self.delta_x}, {self.delta_y})."
+                f"offset of coordinate is out of range ({self.delta_x}, {self.delta_y})."
             )
 
 
 _x_crange = HwParams.CORE_X_MAX - HwParams.CORE_X_MIN + 1
 _y_crange = HwParams.CORE_Y_MAX - HwParams.CORE_Y_MIN + 1
 
 
@@ -423,40 +423,40 @@
     if HwParams.COORD_Y_PRIORITY:
         if cx > HwParams.CORE_X_MAX:
             if cy < HwParams.CORE_Y_MAX:
                 cx -= _x_crange
                 cy += 1
             else:
                 raise ValueError(
-                    f"Coordinate of Y out of high limit: {HwParams.CORE_Y_MAX-1}({cy})."
+                    f"coordinate of Y out of high limit {HwParams.CORE_Y_MAX-1} ({cy})."
                 )
         elif cx < HwParams.CORE_X_MIN:
             if cy > HwParams.CORE_Y_MIN:
                 cx += _x_crange
                 cy -= 1
             else:
                 raise ValueError(
-                    f"Coordinate of Y out of low limit: {HwParams.CORE_Y_MIN}."
+                    f"coordinate of Y out of low limit {HwParams.CORE_Y_MIN}."
                 )
     else:
         if cy > HwParams.CORE_Y_MAX:
             if cx < HwParams.CORE_X_MAX:
                 cx += 1
                 cy -= _y_crange
             else:
                 raise ValueError(
-                    f"Coordinate of X out of high limit: {HwParams.CORE_X_MAX-1}({cx})."
+                    f"coordinate of X out of high limit {HwParams.CORE_X_MAX-1} ({cx})."
                 )
         elif cy < HwParams.CORE_Y_MIN:
             if cx > HwParams.CORE_X_MIN:
                 cx -= 1
                 cy += _y_crange
             else:
                 raise ValueError(
-                    f"Coordinate of X out of low limit: {HwParams.CORE_X_MIN}."
+                    f"coordinate of X out of low limit {HwParams.CORE_X_MIN}."
                 )
 
     return cx, cy
 
 
 CoordLike = TypeVar("CoordLike", Coord, int, List[int], CoordTuple)
 RIdLike = TypeVar("RIdLike", ReplicationId, int, List[int], CoordTuple)
@@ -465,15 +465,15 @@
 def to_coord(coordlike: CoordLike) -> Coord:
     if isinstance(coordlike, int):
         return Coord.from_addr(coordlike)
 
     if isinstance(coordlike, (list, tuple)):
         if len(coordlike) != 2:
             raise TypeError(
-                f"Expect a tuple or list of 2 elements, but got {len(coordlike)}."
+                f"expected a tuple or list of 2 elements, but got {len(coordlike)}."
             )
 
         return Coord(*coordlike)
 
     return coordlike
 
 
@@ -490,13 +490,13 @@
 def to_rid(ridlike: RIdLike) -> ReplicationId:
     if isinstance(ridlike, int):
         return ReplicationId.from_addr(ridlike)
 
     if isinstance(ridlike, (list, tuple)):
         if len(ridlike) != 2:
             raise ValueError(
-                f"Expect a tuple or list of 2 elements, but got {len(ridlike)}."
+                f"expected a tuple or list of 2 elements, but got {len(ridlike)}."
             )
 
         return ReplicationId(*ridlike)
 
     return ridlike
```

### Comparing `paicorelib-0.0.9/paicorelib/framelib/_types.py` & `paicorelib-1.0.0rc1/paicorelib/framelib/types.py`

 * *Files identical despite different names*

### Comparing `paicorelib-0.0.9/paicorelib/framelib/base.py` & `paicorelib-1.0.0rc1/paicorelib/framelib/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass, field
 from typing import Union
 import copy
 import numpy as np
 
 from paicorelib import Coord, ReplicationId as RId
-from ._types import FRAME_DTYPE, FrameArrayType
+from .types import FRAME_DTYPE, FrameArrayType
 from .frame_defs import FrameFormat as FF, FrameHeader as FH, FrameType as FT
 from .utils import header2type
 
 
 @dataclass
 class Frame:
     """frames which contains information.
@@ -56,15 +56,15 @@
     @property
     def rid_addr(self) -> int:
         return self.rid.address
 
     @property
     def value(self) -> FrameArrayType:
         """Get the full frames of the single frame."""
-        if isinstance(self.payload, (int, FRAME_DTYPE)):
+        if isinstance(self.payload, (int, np.integer)):
             pl = np.asarray([self.payload], dtype=FRAME_DTYPE)
         else:
             pl = self.payload
 
         value = self._frame_common + (pl & FF.GENERAL_PAYLOAD_MASK)
         value = np.asarray(value, dtype=FRAME_DTYPE)
         value.setflags(write=False)
@@ -82,15 +82,15 @@
             (header << FF.GENERAL_HEADER_OFFSET)
             + (chip_addr << FF.GENERAL_CHIP_ADDR_OFFSET)
             + (core_addr << FF.GENERAL_CORE_ADDR_OFFSET)
             + (rid_addr << FF.GENERAL_CORE_EX_ADDR_OFFSET)
         )
 
     def __len__(self) -> int:
-        return self.payload.size
+        return 1 if isinstance(self.payload, int) else self.payload.size
 
     def __str__(self) -> str:
         return (
             f"Frame info:\n"
             f"Head:                 {self.header}\n"
             f"Chip address:         {self.chip_coord}\n"
             f"Core address:         {self.core_coord}\n"
```

### Comparing `paicorelib-0.0.9/paicorelib/framelib/frame_defs.py` & `paicorelib-1.0.0rc1/paicorelib/framelib/frame_defs.py`

 * *Files identical despite different names*

### Comparing `paicorelib-0.0.9/paicorelib/framelib/frame_gen.py` & `paicorelib-1.0.0rc1/paicorelib/framelib/frame_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 from numpy.typing import NDArray
 
 from paicorelib import Coord, LCN_EX, NeuronAttrs, NeuronDestInfo, ParamsReg
 from paicorelib import ReplicationId as RId
 from paicorelib import WeightPrecision as WP
 from .frames import *
-from ._types import (
+from .types import (
     DataArrayType,
     FrameArrayType,
     FRAME_DTYPE,
     IntScalarType,
 )
 
 
@@ -26,23 +26,21 @@
     ) -> OfflineConfigFrame1:
         return OfflineConfigFrame1(chip_coord, core_coord, rid, int(random_seed))
 
     @overload
     @staticmethod
     def gen_config_frame2(
         chip_coord: Coord, core_coord: Coord, rid: RId, /, params_reg: ParamsReg
-    ) -> OfflineConfigFrame2:
-        ...
+    ) -> OfflineConfigFrame2: ...
 
     @overload
     @staticmethod
     def gen_config_frame2(
         chip_coord: Coord, core_coord: Coord, rid: RId, /, params_reg: Dict[str, Any]
-    ) -> OfflineConfigFrame2:
-        ...
+    ) -> OfflineConfigFrame2: ...
 
     @staticmethod
     def gen_config_frame2(
         chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
         /,
@@ -65,16 +63,15 @@
         sram_start_addr: IntScalarType,
         n_neuron: IntScalarType,
         attrs: NeuronAttrs,
         dest_info: NeuronDestInfo,
         *,
         lcn_ex: LCN_EX = LCN_EX.LCN_1X,
         weight_precision: WP = WP.WEIGHT_WIDTH_1BIT,
-    ) -> OfflineConfigFrame3:
-        ...
+    ) -> OfflineConfigFrame3: ...
 
     @overload
     @staticmethod
     def gen_config_frame3(
         chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
@@ -82,16 +79,15 @@
         sram_start_addr: IntScalarType,
         n_neuron: IntScalarType,
         attrs: Dict[str, Any],
         dest_info: Dict[str, Any],
         *,
         lcn_ex: LCN_EX = LCN_EX.LCN_1X,
         weight_precision: WP = WP.WEIGHT_WIDTH_1BIT,
-    ) -> OfflineConfigFrame3:
-        ...
+    ) -> OfflineConfigFrame3: ...
 
     @staticmethod
     def gen_config_frame3(
         chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
         /,
@@ -184,27 +180,25 @@
     ) -> OfflineTestInFrame2:
         return OfflineTestInFrame2(chip_coord, core_coord, rid)
 
     @overload
     @staticmethod
     def gen_testout_frame2(
         test_chip_coord: Coord, core_coord: Coord, rid: RId, /, params_reg: ParamsReg
-    ) -> OfflineTestOutFrame2:
-        ...
+    ) -> OfflineTestOutFrame2: ...
 
     @overload
     @staticmethod
     def gen_testout_frame2(
         test_chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
         /,
         params_reg: Dict[str, Any],
-    ) -> OfflineTestOutFrame2:
-        ...
+    ) -> OfflineTestOutFrame2: ...
 
     @staticmethod
     def gen_testout_frame2(
         test_chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
         /,
@@ -316,19 +310,19 @@
     @staticmethod
     def gen_work_frame1_fast(
         frame_dest_info: FrameArrayType, data: NDArray[np.uint8]
     ) -> FrameArrayType:
         _max, _min = np.max(data, axis=None), np.min(data, axis=None)
 
         if _min < np.iinfo(np.uint8).min or _max > np.iinfo(np.uint8).max:
-            raise ValueError(f"Data out of range int8 ({_min}, {_max}).")
+            raise ValueError(f"data out of range int8 ({_min}, {_max}).")
 
         if frame_dest_info.size != data.size:
             raise ValueError(
-                f"The size of frame dest info and data are not equal({frame_dest_info.size}, {data.size})."
+                f"the size of frame dest info & data are not equal, {frame_dest_info.size} != {data.size}."
             )
 
         return OfflineWorkFrame1._gen_frame_fast(frame_dest_info, data.flatten())
 
     @staticmethod
     def gen_work_frame2(chip_coord: Coord, n_sync: IntScalarType) -> OfflineWorkFrame2:
         return OfflineWorkFrame2(chip_coord, int(n_sync))
```

### Comparing `paicorelib-0.0.9/paicorelib/framelib/frames.py` & `paicorelib-1.0.0rc1/paicorelib/framelib/frames.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import warnings
-from typing import Any, ClassVar, Dict, Optional
+from typing import Any, ClassVar, Dict, Optional, Union
 
 import numpy as np
 from numpy.typing import NDArray
 
 from paicorelib import Coord, CoordLike
 from paicorelib import ReplicationId as RId
 from paicorelib import RIdLike
 from paicorelib import to_coord, to_rid
 from paicorelib.hw_defs import HwParams
 from paicorelib.ram_model import NeuronAttrsChecker, NeuronDestInfoChecker
 from paicorelib.reg_model import ParamsRegChecker
-from ._types import FRAME_DTYPE, ArrayType, DataType, FrameArrayType
+from .types import FRAME_DTYPE, ArrayType, DataType, FrameArrayType
 from .base import Frame, FramePackage
 from .frame_defs import (
     FrameFormat as FF,
     FrameHeader as FH,
     ParameterRAMFormat as RAMF,
     ParameterRegFormat as RegF,
     SpikeFrameFormat as WF1F,
@@ -153,15 +153,15 @@
         reg_frame3 = (
             tca_low7 & RegF.TEST_CHIP_ADDR_LOW7_MASK
         ) << RegF.TEST_CHIP_ADDR_LOW7_OFFSET
 
         return np.asarray([reg_frame1, reg_frame2, reg_frame3], dtype=FRAME_DTYPE)
 
     @property
-    def params_reg(self) -> FrameArrayType:
+    def params_reg(self) -> Union[int, FRAME_DTYPE, FrameArrayType]:
         return self.payload
 
 
 class _NeuronRAMFrame(FramePackage):
     def __init__(
         self,
         header: FH,
@@ -211,16 +211,17 @@
         threshold_mask_ctrl_high4, threshold_mask_ctrl_low1 = bin_split(
             attrs["threshold_mask_ctrl"], 1, 4
         )
         addr_core_x_high3, addr_core_x_low2 = bin_split(dest_info["addr_core_x"], 2, 3)
 
         # LSB: [63:0], [127:64], [191:128], [213:192]
         # Package #1, [63:0]
+        vjt_init = attrs.get("vjt_init", 0)
         ram_frame1 = (
-            ((attrs["vjt_pre"] & RAMF.VJT_PRE_MASK) << RAMF.VJT_PRE_OFFSET)
+            ((vjt_init & RAMF.VJT_PRE_MASK) << RAMF.VJT_PRE_OFFSET)
             | (
                 (attrs["bit_truncate"] & RAMF.BIT_TRUNCATE_MASK)
                 << RAMF.BIT_TRUNCATE_OFFSET
             )
             | (
                 (attrs["weight_det_stoch"] & RAMF.WEIGHT_DET_STOCH_MASK)
                 << RAMF.WEIGHT_DET_STOCH_OFFSET
@@ -629,15 +630,15 @@
         if timeslots is not None:
             _timeslots = np.asarray(timeslots, dtype=FRAME_DTYPE).flatten()
         else:
             _timeslots = np.zeros_like(_axons)
 
         if _axons.size != _timeslots.size:
             raise ValueError(
-                f"The size of axons & timeslots are not equal ({_axons.size}, {_timeslots.size})"
+                f"the size of axons & timeslots are not equal, {_axons.size} !={_timeslots.size}."
             )
 
         _chip_coord = to_coord(chip_coord)
         _core_coord = to_coord(core_coord)
         _rid = to_rid(rid)
 
         header = cls.header.value & FF.GENERAL_HEADER_MASK
@@ -703,18 +704,20 @@
         )
 
 
 def _package_arg_check(
     sram_start_addr: int, data_package_num: int, package_type: int
 ) -> FRAME_DTYPE:
     if sram_start_addr > RAMF.GENERAL_PACKAGE_SRAM_ADDR_MASK or sram_start_addr < 0:
-        raise ValueError(f"SRAM start address out of range, {sram_start_addr}")
+        raise ValueError(f"SRAM start address out of range, {sram_start_addr}.")
 
     if data_package_num > RAMF.GENERAL_PACKAGE_NUM_MASK or data_package_num < 0:
-        raise ValueError(f"#N of data package out of range, {data_package_num}")
+        raise ValueError(
+            f"the numeber of data package out of range, {data_package_num}."
+        )
 
     return FRAME_DTYPE(
         (
             (sram_start_addr & FF.GENERAL_PACKAGE_SRAM_ADDR_MASK)
             << FF.GENERAL_PACKAGE_SRAM_ADDR_OFFSET
         )
         | (
```

### Comparing `paicorelib-0.0.9/paicorelib/hw_defs.py` & `paicorelib-1.0.0rc1/paicorelib/hw_defs.py`

 * *Files identical despite different names*

### Comparing `paicorelib-0.0.9/paicorelib/hw_types.py` & `paicorelib-1.0.0rc1/paicorelib/hw_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import ClassVar, List, NamedTuple, Tuple
+from typing import ClassVar, List, NamedTuple
 
 from .hw_defs import HwParams
 from .reg_types import CoreMode
 
 __all__ = ["NeuronSegment", "AxonCoord", "AxonSegment", "HwCore"]
 
 
@@ -28,20 +28,26 @@
     """The interval of address when mapping neuron attributes on the RAM."""
 
     @property
     def n_neuron(self) -> int:
         return self.index.stop - self.index.start
 
     @property
+    def n_addr(self) -> int:
+        return self.interval * self.n_neuron
+
+    @property
     def addr_max(self) -> int:
         if (
             _addr_max := self.addr_offset
             + self.interval * (self.index.stop - self.index.start)
         ) > HwParams.ADDR_RAM_MAX:
-            raise ValueError(f"RAM Address out of {HwParams.ADDR_RAM_MAX}: {_addr_max}.")
+            raise ValueError(
+                f"RAM address out of range {HwParams.ADDR_RAM_MAX} ({_addr_max})."
+            )
 
         return _addr_max
 
     @property
     def addr_ram(self) -> List[int]:
         """Convert index of neuron into RAM address."""
         return list(range(self.addr_offset, self.addr_max, 1))
@@ -73,21 +79,14 @@
 class HwCore(ABC):
     """Hardware core abstraction."""
 
     RUNTIME_MODE: ClassVar[CoreMode]
 
     @property
     @abstractmethod
-    def shape(self) -> Tuple[int, int]:
-        """Shape of the core."""
-        raise NotImplementedError
-
-    @property
-    @abstractmethod
     def n_core_required(self) -> int:
         """#N of cores required to accommodate neurons inside self."""
-        raise NotImplementedError
+        ...
 
     @classmethod
     @abstractmethod
-    def build(cls):
-        ...
+    def build(cls): ...
```

### Comparing `paicorelib-0.0.9/paicorelib/ram_model.py` & `paicorelib-1.0.0rc1/paicorelib/ram_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,24 +7,26 @@
     InstanceOf,
     field_serializer,
     field_validator,
     model_validator,
 )
 from pydantic.type_adapter import TypeAdapter
 from pydantic.types import NonNegativeInt
-from typing_extensions import TypedDict  # Use `typing_extensions.TypedDict`.
+from typing_extensions import (
+    NotRequired,
+    TypedDict,  # Use `typing_extensions.TypedDict`.
+)
 
 from .hw_defs import HwParams
 from .hw_types import AxonCoord
 from .ram_types import *
 
 __all__ = ["NeuronDestInfo", "NeuronAttrs"]
 
 TICK_RELATIVE_BIT_MAX = 8
-ADDR_AXON_BIT_MAX = 11
 ADDR_CORE_X_BIT_MAX = 5
 ADDR_CORE_Y_BIT_MAX = 5
 ADDR_CORE_X_EX_BIT_MAX = 5
 ADDR_CORE_Y_EX_BIT_MAX = 5
 ADDR_CHIP_X_BIT_MAX = 5
 ADDR_CHIP_Y_BIT_MAX = 5
 
@@ -34,31 +36,27 @@
 
     NOTE: The parameters input in the model are declared in `docs/Table-of-Terms.md`.
     """
 
     model_config = ConfigDict(extra="ignore", validate_assignment=True)
 
     addr_chip_x: NonNegativeInt = Field(
-        lt=(1 << ADDR_CHIP_X_BIT_MAX),
-        description="Address X of destination chip.",
+        lt=(1 << ADDR_CHIP_X_BIT_MAX), description="Address X of destination chip."
     )
 
     addr_chip_y: NonNegativeInt = Field(
-        lt=(1 << ADDR_CHIP_Y_BIT_MAX),
-        description="Address Y of destination chip.",
+        lt=(1 << ADDR_CHIP_Y_BIT_MAX), description="Address Y of destination chip."
     )
 
     addr_core_x: NonNegativeInt = Field(
-        lt=(1 << ADDR_CORE_X_BIT_MAX),
-        description="Address X of destination core.",
+        lt=(1 << ADDR_CORE_X_BIT_MAX), description="Address X of destination core."
     )
 
     addr_core_y: NonNegativeInt = Field(
-        lt=(1 << ADDR_CORE_Y_BIT_MAX),
-        description="Address Y of destination core.",
+        lt=(1 << ADDR_CORE_Y_BIT_MAX), description="Address Y of destination core."
     )
 
     addr_core_x_ex: NonNegativeInt = Field(
         lt=(1 << ADDR_CORE_X_EX_BIT_MAX),
         description="Broadcast address X of destination core.",
     )
 
@@ -78,54 +76,48 @@
     )
 
     @field_validator("tick_relative")
     @classmethod
     def _tick_relative_check(cls, v):
         if any(tr >= (1 << TICK_RELATIVE_BIT_MAX) or tr < 0 for tr in v):
             # DO NOT change the type of exception `ValueError` in the validators below.
-            raise ValueError("Parameter 'tick relative' out of range.")
+            raise ValueError("parameter 'tick relative' out of range.")
 
         return v
 
     @field_validator("addr_axon")
     @classmethod
     def _addr_axon_check(cls, v):
         if any(addr > HwParams.ADDR_AXON_MAX or addr < 0 for addr in v):
-            raise ValueError("Parameter 'addr_axon' out of range.")
+            raise ValueError("parameter 'addr_axon' out of range.")
 
         return v
 
     @model_validator(mode="after")
     def _length_match_check(self):
         if len(self.tick_relative) != len(self.addr_axon):
             raise ValueError(
-                "Parameter 'tick relative' & 'addr_axon' must have the same "
+                "parameter 'tick relative' & 'addr_axon' must have the same "
                 f"length: {len(self.tick_relative)}, {len(self.addr_axon)}."
             )
 
         return self
 
 
 class OutpuNeuronDestInfo(_BasicNeuronDest):
     # TODO
     start_axon_coord: AxonCoord = Field(description="Address X of destination chip.")
     end_axon_coord: AxonCoord = Field(description="Address X of destination chip.")
 
 
-RESET_MODE_BIT_MAX = 2  # Not used
 RESET_V_BIT_MAX = 30
-LEAKING_COMPARISON_BIT_MAX = 1  # Not used
 THRESHOLD_MASK_CTRL_BIT_MAX = 5
-NEGATIVE_THRESHOLD_MODE_BIT_MAX = 1  # Not used
 NEGATIVE_THRESHOLD_VALUE_BIT_MAX = 29
 POSITIVE_THRESHOLD_VALUE_BIT_MAX = 29
-LEAKING_DIRECTION_BIT_MAX = 1  # Not used
-LEAKING_MODE_BIT_MAX = 1  # Not used
 LEAK_V_BIT_MAX = 30
-WEIGHT_MODE_BIT_MAX = 1  # Not used
 BIT_TRUNCATE_BIT_MAX = 5
 VJT_PRE_BIT_MAX = 30
 
 
 class NeuronAttrs(BaseModel):
     model_config = ConfigDict(extra="ignore", validate_assignment=True)
 
@@ -135,17 +127,17 @@
 
     reset_v: int = Field(
         ge=-(1 << (RESET_V_BIT_MAX - 1)),
         lt=(1 << (RESET_V_BIT_MAX - 1)),
         description="Reset value of membrane potential, 30-bit signed.",
     )
 
-    leaking_comparison: LeakingComparisonMode = Field(
+    leak_comparison: LeakComparisonMode = Field(
         serialization_alias="leak_post",
-        description="Leaking after threshold comparison or before.",
+        description="Leak after threshold comparison or before.",
     )
 
     threshold_mask_bits: NonNegativeInt = Field(
         lt=(1 << THRESHOLD_MASK_CTRL_BIT_MAX),
         serialization_alias="threshold_mask_ctrl",
         description="X-bits mask for random threshold.",
     )
@@ -163,69 +155,62 @@
 
     pos_threshold: NonNegativeInt = Field(
         lt=(1 << POSITIVE_THRESHOLD_VALUE_BIT_MAX),
         serialization_alias="threshold_pos",
         description="Positive threshold, 29-bit unsigned.",
     )
 
-    leaking_direction: LeakingDirectionMode = Field(
+    leak_direction: LeakDirectionMode = Field(
         serialization_alias="leak_reversal_flag",
-        description="Direction of leaking, forward or reversal.",
+        description="Direction of leak, forward or reversal.",
     )
 
-    leaking_integration_mode: LeakingIntegrationMode = Field(
+    leak_integration_mode: LeakIntegrationMode = Field(
         serialization_alias="leak_det_stoch",
-        description="Modes of leaking integration, deterministic or stochastic.",
+        description="Modes of leak integration, deterministic or stochastic.",
     )
 
     leak_v: int = Field(
         ge=-(1 << (LEAK_V_BIT_MAX - 1)),
         lt=(1 << (LEAK_V_BIT_MAX - 1)),
-        description="Leaking potential, 30-bit signed.",
+        description="Leak voltage, 30-bit signed.",
     )
 
     synaptic_integration_mode: SynapticIntegrationMode = Field(
         serialization_alias="weight_det_stoch",
         description="Modes of synaptic integration, deterministic or stochastic.",
     )
 
     bit_truncation: NonNegativeInt = Field(
         lt=(1 << BIT_TRUNCATE_BIT_MAX),
         serialization_alias="bit_truncate",
         description="Position of truncation, unsigned int, 5-bits.",
     )
 
-    vjt_init: int = Field(
-        ge=-(1 << (VJT_PRE_BIT_MAX - 1)),
-        lt=(1 << (VJT_PRE_BIT_MAX - 1)),
-        serialization_alias="vjt_pre",
-        description="Membrane potential of neuron at last time step, 30-bit signed. \
-            0 at initialization.",
-    )
-
-    """Parameter serializers"""
+    vjt_init: int = 0
+    """Membrane potential of neuron at last timestep, 30-bit signed. Must be 0 at initialization."""
 
     @field_serializer("reset_mode")
     def _reset_mode(self, reset_mode: ResetMode) -> int:
         return reset_mode.value
 
-    @field_serializer("leaking_comparison")
-    def _leaking_comparison(self, leaking_comparison: LeakingComparisonMode) -> int:
-        return leaking_comparison.value
+    @field_serializer("leak_comparison")
+    def _leak_comparison(self, leak_comparison: LeakComparisonMode) -> int:
+        return leak_comparison.value
 
     @field_serializer("neg_thres_mode")
     def _neg_thres_mode(self, neg_thres_mode: NegativeThresholdMode) -> int:
         return neg_thres_mode.value
 
-    @field_serializer("leaking_direction")
-    def _leaking_direction(self, leaking_direction: LeakingDirectionMode) -> int:
-        return leaking_direction.value
+    @field_serializer("leak_direction")
+    def _leak_direction(self, leak_direction: LeakDirectionMode) -> int:
+        return leak_direction.value
 
-    @field_serializer("leaking_integration_mode")
-    def _lim(self, lim: LeakingIntegrationMode) -> int:
+    @field_serializer("leak_integration_mode")
+    def _lim(self, lim: LeakIntegrationMode) -> int:
         return lim.value
 
     @field_serializer("synaptic_integration_mode")
     def _sim(self, sim: SynapticIntegrationMode) -> int:
         return sim.value
 
 
@@ -240,15 +225,15 @@
     threshold_neg: int
     threshold_pos: int
     leak_reversal_flag: int
     leak_det_stoch: int
     leak_v: int
     weight_det_stoch: int
     bit_truncate: int
-    vjt_pre: int
+    vjt_init: NotRequired[int]  # Reserved.
 
 
 class _NeuronDestInfoDict(TypedDict):
     """Typed dictionary of `NeuronDestInfo` for typing check."""
 
     addr_core_x: int
     addr_core_y: int
```

### Comparing `paicorelib-0.0.9/paicorelib/ram_types.py` & `paicorelib-1.0.0rc1/paicorelib/ram_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum, IntEnum, unique
 
 __all__ = [
     "ResetMode",
-    "LeakingComparisonMode",
+    "LeakComparisonMode",
     "NegativeThresholdMode",
-    "LeakingDirectionMode",
-    "LeakingIntegrationMode",
+    "LeakDirectionMode",
+    "LeakIntegrationMode",
     "SynapticIntegrationMode",
     "ThresholdMode",
 ]
 
 """
     Type defines of RAM parameters.
     See Section 2.4.2 in V2.1 Manual for details.
@@ -29,15 +29,15 @@
 
     MODE_NORMAL = 0  # Default value.
     MODE_LINEAR = 1
     MODE_NONRESET = 2
 
 
 @unique
-class LeakingComparisonMode(Enum):
+class LeakComparisonMode(Enum):
     """Leak after comparison or before. 1-bit.
 
     - `LEAK_BEFORE_COMP`: leak before comparison.
     - `LEAK_AFTER_COMP`: leak after comparison. Default value.
 
     NOTE: Same as `leak_post` in V2.1.
     """
@@ -57,33 +57,33 @@
     """
 
     MODE_RESET = 0  # Default value.
     MODE_SATURATION = 1
 
 
 @unique
-class LeakingDirectionMode(Enum):
-    """Direction of leaking, forward or reversal.
+class LeakDirectionMode(Enum):
+    """Direction of Leak, forward or reversal.
 
-    - `MODE_FORWARD`: forward leaking. Default value.
-    - `MODE_REVERSAL`: reversal leaking.
+    - `MODE_FORWARD`: forward Leak. Default value.
+    - `MODE_REVERSAL`: reversal Leak.
 
     NOTE: Same as `leak_reversal_flag` in V2.1.
     """
 
     MODE_FORWARD = 0  # Default value.
     MODE_REVERSAL = 1
 
 
 @unique
-class LeakingIntegrationMode(Enum):
-    """Mode of leaking integration, deterministic or stochastic.
+class LeakIntegrationMode(Enum):
+    """Mode of Leak integration, deterministic or stochastic.
 
-    - `MODE_DETERMINISTIC`: deterministic leaking. Default value.
-    - `MODE_STOCHASTIC`: stochastic leaking.
+    - `MODE_DETERMINISTIC`: deterministic Leak. Default value.
+    - `MODE_STOCHASTIC`: stochastic Leak.
 
     NOTE: Same as `leak_det_stoch` in V2.1.
     """
 
     MODE_DETERMINISTIC = 0  # Default value.
     MODE_STOCHASTIC = 1
```

### Comparing `paicorelib-0.0.9/paicorelib/reg_model.py` & `paicorelib-1.0.0rc1/paicorelib/reg_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Literal
 from pydantic import (
     BaseModel,
     ConfigDict,
     Field,
     field_serializer,
     model_validator,
 )
@@ -11,26 +12,34 @@
 
 from .coordinate import Coord
 from .hw_defs import HwParams
 from .reg_types import *
 
 __all__ = ["CoreParams", "ParamsReg"]
 
-WEIGHT_PRECISION_BIT_MAX = 2  # Not used
-LCN_EXTENSION_BIT_MAX = 2  # Not used
-INPUT_WIDTH_FORMAT_BIT_MAX = 2  # Not used
-SPIKE_WIDTH_FORMAT_BIT_MAX = 2  # Not used
 NUM_DENDRITE_BIT_MAX = 13
-POOL_MAX_EN_BIT_MAX = 1  # Not used
 TICK_WAIT_START_BIT_MAX = 15
 TICK_WAIT_END_BIT_MAX = 15
-SNN_MODE_EN_BIT_MAX = 1  # Not used
 TARGET_LCN_BIT_MAX = 4
 TEST_CHIP_ADDR_BIT_MAX = 10
 
+NUM_DENDRITE_OUT_OF_RANGE_FORMAT = (
+    "param 'num_dendrite' out of range. When input width is 8-bit in {0} mode, "
+    + "the number of dendrites should be no more than {1}."
+)
+
+
+def _num_dendrite_out_of_range_repr(mode: Literal["ANN", "SNN"]) -> str:
+    if mode == "ANN":
+        max_limit = HwParams.N_DENDRITE_MAX_ANN
+    else:
+        max_limit = HwParams.N_DENDRITE_MAX_SNN
+
+    return NUM_DENDRITE_OUT_OF_RANGE_FORMAT.format(mode, max_limit)
+
 
 class CoreParams(BaseModel):
     """Parameter model of register parameters listed in Section 2.4.1.
 
     NOTE: The parameters input in the model are declared in `docs/Table-of-Terms.md`.
     """
 
@@ -47,21 +56,19 @@
     lcn_extension: LCNExtensionType = Field(
         le=LCNExtensionType.LCN_64X,
         serialization_alias="LCN",
         description="Scale of fan-in extension.",
     )
 
     input_width_format: InputWidthFormatType = Field(
-        serialization_alias="input_width",
-        description="Format of input spike.",
+        serialization_alias="input_width", description="Format of input spike."
     )
 
     spike_width_format: SpikeWidthFormatType = Field(
-        serialization_alias="spike_width",
-        description="Format of output spike.",
+        serialization_alias="spike_width", description="Format of output spike."
     )
 
     num_dendrite: NonNegativeInt = Field(
         lt=(1 << NUM_DENDRITE_BIT_MAX),
         serialization_alias="neuron_num",
         description="The number of used dendrites.",
     )
@@ -69,58 +76,50 @@
     max_pooling_en: MaxPoolingEnableType = Field(
         default=MaxPoolingEnableType.DISABLE,
         serialization_alias="pool_max",
         description="Enable max pooling or not in 8-bit input format.",
     )
 
     tick_wait_start: NonNegativeInt = Field(
-        default=0,
+        default=1,
         lt=(1 << TICK_WAIT_START_BIT_MAX),
-        description="The core begins to work at #N sync_all. 0 for not starting. Default is 0.",
+        description="The core begins to work at #N sync_all. 0 for not starting while 1 for staring forever.",
     )
 
     tick_wait_end: NonNegativeInt = Field(
         default=0,
         lt=(1 << TICK_WAIT_END_BIT_MAX),
-        description="The core keeps working within #N sync_all. 0 for not stopping. Default is 0.",
+        description="The core keeps working within #N sync_all. 0 for not stopping.",
     )
 
     snn_mode_en: SNNModeEnableType = Field(
-        default=SNNModeEnableType.ENABLE,
-        serialization_alias="snn_en",
-        description="Enable SNN mode or not.",
+        serialization_alias="snn_en", description="Enable SNN mode or not."
     )
 
     target_lcn: LCNExtensionType = Field(
-        le=LCNExtensionType.LCN_64X,
-        serialization_alias="target_LCN",
-        description="LCN of the target core.",
+        serialization_alias="target_LCN", description="LCN extension of the core."
     )
 
     test_chip_addr: Coord = Field(
-        default=Coord(0, 0),
-        description="Destination address of output test frames.",
+        description="Destination address of output test frames."
     )
 
     """Parameter checks"""
 
     @model_validator(mode="after")
     def _neuron_num_range_limit(self):
-        if self.input_width_format is InputWidthFormatType.WIDTH_1BIT:
+        if self.input_width_format is InputWidthFormatType.WIDTH_8BIT:
+            if self.num_dendrite > HwParams.N_DENDRITE_MAX_ANN:
+                raise ValueError(_num_dendrite_out_of_range_repr("ANN"))
+        elif self.snn_mode_en is SNNModeEnableType.DISABLE:
             if self.num_dendrite > HwParams.N_DENDRITE_MAX_ANN:
-                raise ValueError(
-                    f"Param 'num_dendrite' out of range. When input width is 1-bit,"
-                    f"The #N of dendrites should be no more than {HwParams.N_DENDRITE_MAX_ANN}."
-                )
+                raise ValueError(_num_dendrite_out_of_range_repr("ANN"))
         else:
             if self.num_dendrite > HwParams.N_DENDRITE_MAX_SNN:
-                raise ValueError(
-                    f"Param 'num_dendrite' out of range. When input width is 8-bit,"
-                    f"The #N of dendrite should be no more than {HwParams.N_DENDRITE_MAX_SNN}."
-                )
+                raise ValueError(_num_dendrite_out_of_range_repr("SNN"))
 
         return self
 
     @model_validator(mode="after")
     def _max_pooling_en_check(self):
         if (
             self.input_width_format is InputWidthFormatType.WIDTH_1BIT
```

### Comparing `paicorelib-0.0.9/paicorelib/reg_types.py` & `paicorelib-1.0.0rc1/paicorelib/reg_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,28 @@
+import sys
 from enum import Enum, IntEnum, unique
 from typing import Dict, Tuple
 
+if sys.version_info >= (3, 10):
+    from typing import TypeAlias
+else:
+    from typing_extensions import TypeAlias
+
+__all__ = [
+    "WeightPrecisionType",
+    "LCNExtensionType",
+    "InputWidthFormatType",
+    "SpikeWidthFormatType",
+    "MaxPoolingEnableType",
+    "SNNModeEnableType",
+    "CoreType",
+    "CoreMode",
+    "CoreModeDict",
+]
+
 """
     Type defines of parameters of registers & parameters of neuron RAM.
     See Section 2.4.1 in V2.1 Manual for details.
 """
 
 
 @unique
@@ -86,15 +104,15 @@
 
     DISABLE = 0
     ENABLE = 1  # Default value.
 
 
 @unique
 class CoreType(Enum):
-    """Type of core. Reserved."""
+    """Types of cores."""
 
     TYPE_OFFLINE = "OFFLINE"
     TYPE_ONLINE = "ONLINE"
 
 
 @unique
 class CoreMode(Enum):
@@ -117,17 +135,17 @@
     MODE_BANN = 1  # SNN mode like.
     MODE_ANN = 2
     MODE_BANN_OR_SNN_TO_ANN = 3
     MODE_BANN_OR_SNN_TO_SNN = 4
     MODE_ANN_TO_BANN_OR_SNN = 5
 
 
-_ModeParamRef = Tuple[InputWidthFormatType, SpikeWidthFormatType, SNNModeEnableType]
-
-
+_ModeParamRef: TypeAlias = Tuple[
+    InputWidthFormatType, SpikeWidthFormatType, SNNModeEnableType
+]
 CoreModeDict: Dict[CoreMode, _ModeParamRef] = {
     CoreMode.MODE_BANN: (
         InputWidthFormatType.WIDTH_1BIT,
         SpikeWidthFormatType.WIDTH_1BIT,
         SNNModeEnableType.DISABLE,
     ),
     CoreMode.MODE_SNN: (
```

### Comparing `paicorelib-0.0.9/paicorelib/routing_defs.py` & `paicorelib-1.0.0rc1/paicorelib/routing_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,20 @@
     "get_multicast_cores",
     "get_replication_id",
 ]
 
 
 @unique
 class RoutingLevel(IntEnum):
+    """The level of routing node.
+
+    L0-level nodes are leaves of tree to store data. A L0-cluster is a physical core.
+    """
+
     L0 = 0
-    """Leaves of tree to store the data. A L0-cluster is a physical core."""
     L1 = 1
     L2 = 2
     L3 = 3
     L4 = 4
     L5 = 5
 
 
@@ -166,14 +170,17 @@
 
 def get_replication_id(coords: Sequence[Coord]) -> RId:
     """Get the replication ID by given the coordinates.
 
     Args:
         - coords: sequence of coordinates.
     """
+    if len(coords) < 1:
+        raise ValueError("the length of coordinates must be at least 1.")
+
     base_coord = coords[0]
     rid = RId(0, 0)
 
     for coord in coords[1:]:
         rid |= base_coord ^ coord
 
     return rid
```

### Comparing `paicorelib-0.0.9/PKG-INFO` & `paicorelib-1.0.0rc1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: paicorelib
-Version: 0.0.9
-Summary: Library of PAICORE 2.0 in Python.
+Version: 1.0.0rc1
+Summary: Library of PAICORE 2.0.
 Home-page: https://github.com/PAICookers/PAIlib
 License: GPL-3.0-or-later
 Keywords: PAICORE 2.0,PAIBox,PAILib
 Author: Ziru Pan
 Author-email: zrpan@stu.pku.edu.cn
 Maintainer: Ziru Pan
 Maintainer-email: zrpan@stu.pku.edu.cn
 Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: numpy (>=1.23.0,<2.0.0)
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: numpy (>=1.24.0,<2.0.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Project-URL: Documentation, https://github.com/PAICookers/PAIlib#readme
 Project-URL: Repository, https://github.com/PAICookers/PAIlib
 Description-Content-Type: text/markdown
 
 <div align="center">
 
@@ -29,21 +34,21 @@
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIlib/blob/master/pyproject.toml">
         <img src="https://img.shields.io/pypi/pyversions/paicorelib">
     </a>
-    <a href="https://github.com/PAICookers/PAIlib/releases/tag/v0.0.9">
-        <img src="https://img.shields.io/github/v/release/PAICookers/PAIlib?color=orange">
+    <a href="https://github.com/PAICookers/PAIlib/releases/tag/v1.0.0rc1">
+        <img src="https://img.shields.io/github/v/release/PAICookers/PAIlib?include_prereleases&color=orange">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIlib">
       <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIlib/master?color=red">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIlib/master">
 	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIlib/master.svg" alt="pre-commit.ci status">
     </a>
 
 </p>
 
-This is the library of PAIBox & runtime.
+术语对照表：[Table of Terms](docs/Table-of-Terms.md)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,20 +1,23 @@
-Metadata-Version: 2.1 Name: paicorelib Version: 0.0.9 Summary: Library of
-PAICORE 2.0 in Python. Home-page: https://github.com/PAICookers/PAIlib License:
-GPL-3.0-or-later Keywords: PAICORE 2.0,PAIBox,PAILib Author: Ziru Pan Author-
-email: zrpan@stu.pku.edu.cn Maintainer: Ziru Pan Maintainer-email:
-zrpan@stu.pku.edu.cn Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
-Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
-Dist: numpy (>=1.23.0,<2.0.0) Requires-Dist: pydantic (>=2.0,<3.0) Project-URL:
-Documentation, https://github.com/PAICookers/PAIlib#readme Project-URL:
-Repository, https://github.com/PAICookers/PAIlib Description-Content-Type:
-text/markdown
+Metadata-Version: 2.1 Name: paicorelib Version: 1.0.0rc1 Summary: Library of
+PAICORE 2.0. Home-page: https://github.com/PAICookers/PAIlib License: GPL-3.0-
+or-later Keywords: PAICORE 2.0,PAIBox,PAILib Author: Ziru Pan Author-email:
+zrpan@stu.pku.edu.cn Maintainer: Ziru Pan Maintainer-email:
+zrpan@stu.pku.edu.cn Requires-Python: >=3.8,<4.0 Classifier: Intended Audience
+:: Science/Research Classifier: License :: OSI Approved :: GNU General Public
+License v3 or later (GPLv3+) Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Development :: Libraries Requires-Dist: numpy (>=1.24.0,<2.0.0) Requires-Dist:
+pydantic (>=2.0,<3.0) Project-URL: Documentation, https://github.com/
+PAICookers/PAIlib#readme Project-URL: Repository, https://github.com/
+PAICookers/PAIlib Description-Content-Type: text/markdown
                            # Library of PAICORE 2.0
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_p_a_i_c_o_r_e_l_i_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-   _g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_l_i_b_?_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-   _c_o_d_e_f_a_c_t_o_r_/_g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_l_i_b_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
-                                    _s_t_a_t_u_s_]
-This is the library of PAIBox & runtime.
+ _g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_l_i_b_?_i_n_c_l_u_d_e___p_r_e_r_e_l_e_a_s_e_s_&_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/_g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_l_i_b_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-
+                               _c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
+æ¯è¯­å¯¹ç§è¡¨ï¼[Table of Terms](docs/Table-of-Terms.md)
```

