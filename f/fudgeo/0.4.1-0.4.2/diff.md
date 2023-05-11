# Comparing `tmp/fudgeo-0.4.1-py3-none-any.whl.zip` & `tmp/fudgeo-0.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 26635 bytes, number of entries: 17
--rw-r--r--  2.0 unx      117 b- defN 23-May-08 18:27 fudgeo/__init__.py
--rw-r--r--  2.0 unx     2538 b- defN 23-May-06 22:48 fudgeo/constant.py
+Zip file size: 26762 bytes, number of entries: 17
+-rw-r--r--  2.0 unx      117 b- defN 23-May-11 12:46 fudgeo/__init__.py
+-rw-r--r--  2.0 unx     2538 b- defN 23-May-11 01:39 fudgeo/constant.py
 -rw-r--r--  2.0 unx     1157 b- defN 23-Jan-04 21:53 fudgeo/enumeration.py
 -rw-r--r--  2.0 unx    20081 b- defN 23-May-06 22:48 fudgeo/geopkg.py
 -rw-r--r--  2.0 unx     2673 b- defN 23-May-06 22:48 fudgeo/geopkg.sql
 -rw-r--r--  2.0 unx     7768 b- defN 23-May-06 22:48 fudgeo/sql.py
 -rw-r--r--  2.0 unx      974 b- defN 23-May-06 22:48 fudgeo/geometry/__init__.py
--rw-r--r--  2.0 unx     3250 b- defN 23-May-08 18:26 fudgeo/geometry/base.py
--rw-r--r--  2.0 unx    16963 b- defN 23-May-08 18:26 fudgeo/geometry/linestring.py
--rw-r--r--  2.0 unx    17903 b- defN 23-May-08 18:26 fudgeo/geometry/point.py
--rw-r--r--  2.0 unx    22719 b- defN 23-May-08 18:26 fudgeo/geometry/polygon.py
--rw-r--r--  2.0 unx    14620 b- defN 23-May-08 18:26 fudgeo/geometry/util.py
--rw-r--r--  2.0 unx     1088 b- defN 23-May-08 18:29 fudgeo-0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     9095 b- defN 23-May-08 18:29 fudgeo-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-08 18:29 fudgeo-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-08 18:29 fudgeo-0.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1322 b- defN 23-May-08 18:29 fudgeo-0.4.1.dist-info/RECORD
-17 files, 122367 bytes uncompressed, 24503 bytes compressed:  80.0%
+-rw-r--r--  2.0 unx     2000 b- defN 23-May-11 12:45 fudgeo/geometry/base.py
+-rw-r--r--  2.0 unx    18653 b- defN 23-May-11 12:45 fudgeo/geometry/linestring.py
+-rw-r--r--  2.0 unx    19794 b- defN 23-May-11 12:45 fudgeo/geometry/point.py
+-rw-r--r--  2.0 unx    26366 b- defN 23-May-11 12:45 fudgeo/geometry/polygon.py
+-rw-r--r--  2.0 unx    15891 b- defN 23-May-11 12:45 fudgeo/geometry/util.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-May-11 12:46 fudgeo-0.4.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9095 b- defN 23-May-11 12:46 fudgeo-0.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-11 12:46 fudgeo-0.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-11 12:46 fudgeo-0.4.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1322 b- defN 23-May-11 12:46 fudgeo-0.4.2.dist-info/RECORD
+17 files, 129616 bytes uncompressed, 24630 bytes compressed:  81.0%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: fudgeo/geometry/polygon.py
 Comment: 
 
 Filename: fudgeo/geometry/util.py
 Comment: 
 
-Filename: fudgeo-0.4.1.dist-info/LICENSE
+Filename: fudgeo-0.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: fudgeo-0.4.1.dist-info/METADATA
+Filename: fudgeo-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: fudgeo-0.4.1.dist-info/WHEEL
+Filename: fudgeo-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: fudgeo-0.4.1.dist-info/top_level.txt
+Filename: fudgeo-0.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: fudgeo-0.4.1.dist-info/RECORD
+Filename: fudgeo-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fudgeo/__init__.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 """
 Package Initialization
 """
 
 
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 
 
 if __name__ == '__main__':
     pass
```

## fudgeo/geometry/base.py

```diff
@@ -3,142 +3,85 @@
 Base Classes
 """
 
 
 from abc import abstractmethod
 from functools import reduce
 from operator import add
-from typing import List
+from typing import List, Optional, Tuple
 
 from fudgeo.constant import EMPTY
 from fudgeo.geometry.util import EMPTY_ENVELOPE, Envelope, make_header
 
 
 class AbstractGeometry:
     """
     Abstract Geometry
     """
-    __slots__ = []
+    __slots__ = 'srs_id', '_env', '_args'
 
-    @staticmethod
-    def _join_geometries(geoms: List['AbstractGeometry']) -> bytes:
-        """
-        Join Geometries
-        """
-        return reduce(add, [geom._to_wkb() for geom in geoms], EMPTY)
-    # End _join_geometries method
-
-    @property
-    @abstractmethod
-    def is_empty(self) -> bool:
+    def __init__(self, srs_id: int) -> None:
         """
-        Is Empty
+        Initialize the AbstractGeometry class
         """
-        pass
-    # End is_empty property
+        super().__init__()
+        self.srs_id: int = srs_id
+        self._env: Envelope = EMPTY_ENVELOPE
+        self._args: Optional[Tuple[bytes, int]] = None
+    # End init built-in
 
     @abstractmethod
     def _to_wkb(self, use_prefix: bool = True) -> bytes:  # pragma: nocover
         """
         To WKB
         """
         pass
     # End _to_wkb method
-# End AbstractGeometry class
-
 
-# noinspection PyAbstractClass
-class AbstractSpatialGeometry(AbstractGeometry):
-    """
-    Abstract Spatial Geometry
-    """
-    __slots__ = 'srs_id',
-
-    def __init__(self, srs_id: int) -> None:
+    @staticmethod
+    def _join_geometries(geoms: List['AbstractGeometry']) -> bytes:
         """
-        Initialize the AbstractSpatialGeometry class
+        Join Geometries
         """
-        super().__init__()
-        self.srs_id: int = srs_id
-    # End init built-in
-# End AbstractSpatialGeometry class
-
-
-# noinspection PyAbstractClass
-class AbstractSpatialGeometryEnvelope(AbstractSpatialGeometry):
-    """
-    Abstract Spatial Geometry with Envelope
-    """
-    __slots__ = '_envelope',
+        return reduce(add, [geom._to_wkb() for geom in geoms], EMPTY)
+    # End _join_geometries method
 
-    def __init__(self, srs_id: int) -> None:
+    @property
+    @abstractmethod
+    def is_empty(self) -> bool:
         """
-        Initialize the AbstractSpatialGeometryEnvelope class
+        Is Empty
         """
-        super().__init__(srs_id=srs_id)
-        self._envelope: Envelope = EMPTY_ENVELOPE
-    # End init built-in
+        pass
+    # End is_empty property
 
     @property
     @abstractmethod
     def envelope(self) -> Envelope:
         """
         Envelope
         """
         pass
     # End envelope property
-# End AbstractSpatialGeometryEnvelope class
-
-
-class AbstractGeopackageGeometry(AbstractSpatialGeometry):
-    """
-    Abstract Geopackage Geometry
-    """
-    __slots__ = 'srs_id',
 
     def to_gpkg(self) -> bytes:
         """
         To Geopackage
         """
-        return (make_header(srs_id=self.srs_id, is_empty=self.is_empty) +
-                self._to_wkb())
+        env_code, env_wkb = self.envelope.to_wkb()
+        return (make_header(srs_id=self.srs_id, is_empty=self.is_empty,
+                            envelope_code=env_code) + env_wkb + self._to_wkb())
     # End to_gpkg method
 
     @classmethod
     @abstractmethod
     def from_gpkg(cls, value: bytes) -> 'AbstractGeometry':  # pragma: nocover
         """
         From Geopackage
         """
         pass
     # End from_gpkg method
-# End AbstractGeopackageGeometry class
-
-
-# noinspection PyAbstractClass
-class AbstractGeopackageGeometryEnvelope(AbstractGeopackageGeometry):
-    """
-    Abstract Spatial Geometry with Envelope
-    """
-    __slots__ = '_envelope',
-
-    def __init__(self, srs_id: int) -> None:
-        """
-        Initialize the AbstractGeopackageGeometryEnvelope class
-        """
-        super().__init__(srs_id=srs_id)
-        self._envelope: Envelope = EMPTY_ENVELOPE
-    # End init built-in
-
-    @property
-    @abstractmethod
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        pass
-    # End envelope property
-# End AbstractGeopackageGeometryEnvelope class
+# End AbstractGeometry class
 
 
 if __name__ == '__main__':  # pragma: no cover
     pass
```

## fudgeo/geometry/linestring.py

```diff
@@ -1,95 +1,70 @@
 # -*- coding: utf-8 -*-
 """
 Line String
 """
 
 
 from struct import pack
-from typing import Any, List, Type, Union
+from typing import List
 
 from fudgeo.constant import (
-    COUNT_CODE, DOUBLE, FOUR_D, HEADER_OFFSET, QUADRUPLE, THREE_D, TRIPLE,
-    TWO_D, WKB_LINESTRING_M_PRE, WKB_LINESTRING_PRE, WKB_LINESTRING_ZM_PRE,
+    COUNT_CODE, DOUBLE, FOUR_D, QUADRUPLE, THREE_D, TRIPLE, TWO_D,
+    WKB_LINESTRING_M_PRE, WKB_LINESTRING_PRE, WKB_LINESTRING_ZM_PRE,
     WKB_LINESTRING_Z_PRE, WKB_MULTI_LINESTRING_M_PRE, WKB_MULTI_LINESTRING_PRE,
     WKB_MULTI_LINESTRING_ZM_PRE, WKB_MULTI_LINESTRING_Z_PRE)
-from fudgeo.geometry.base import AbstractGeopackageGeometryEnvelope
+from fudgeo.geometry.base import AbstractGeometry
 from fudgeo.geometry.point import Point, PointM, PointZ, PointZM
 from fudgeo.geometry.util import (
     EMPTY_ENVELOPE, Envelope, envelope_from_coordinates,
     envelope_from_coordinates_m, envelope_from_coordinates_z,
     envelope_from_coordinates_zm, envelope_from_geometries,
     envelope_from_geometries_m, envelope_from_geometries_z,
-    envelope_from_geometries_zm, pack_coordinates, unpack_envelope,
-    unpack_header, unpack_line, unpack_lines)
+    envelope_from_geometries_zm, lazy_unpack, pack_coordinates, unpack_line,
+    unpack_lines)
 
 
-LINE_STRING_TYPES = Union[Type['LineString'], Type['LineStringZ'],
-                          Type['LineStringM'], Type['LineStringZM']]
-MULTI_LINE_STRING_TYPES = Union[
-    Type['MultiLineString'], Type['MultiLineStringZ'],
-    Type['MultiLineStringM'], Type['MultiLineStringZM']]
-
-
-def _unpack_linestring(cls: LINE_STRING_TYPES, value: bytes,
-                       dimension: int) -> Any:
-    """
-    Unpack LineString
-    """
-    srs_id, env_code, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
-    if is_empty:
-        return cls([], srs_id=srs_id)
-    # noinspection PyTypeChecker
-    obj = cls(unpack_line(value[offset:], dimension=dimension), srs_id=srs_id)
-    obj._envelope = unpack_envelope(code=env_code, value=value[:offset])
-    return obj
-# End _unpack_linestring function
-
-
-def _unpack_multi_linestring(cls: MULTI_LINE_STRING_TYPES, value: bytes,
-                             dimension: int) -> Any:
-    """
-    Unpack LineStrings into MultiLineString
-    """
-    srs_id, env_code, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
-    if is_empty:
-        return cls([], srs_id=srs_id)
-    # noinspection PyTypeChecker
-    obj = cls(unpack_lines(value[offset:], dimension=dimension), srs_id=srs_id)
-    obj._envelope = unpack_envelope(code=env_code, value=value[:offset])
-    return obj
-# End _unpack_multi_linestring function
-
-
-class LineString(AbstractGeopackageGeometryEnvelope):
+class LineString(AbstractGeometry):
     """
     LineString
     """
-    __slots__ = 'coordinates',
+    __slots__ = '_coordinates',
 
     def __init__(self, coordinates: List[DOUBLE], srs_id: int) -> None:
         """
         Initialize the LineString class
         """
         super().__init__(srs_id=srs_id)
-        self.coordinates: List[DOUBLE] = coordinates
+        self._coordinates: List[DOUBLE] = coordinates
     # End init built-in
 
     def __eq__(self, other: 'LineString') -> bool:
         """
         Equals
         """
         if not isinstance(other, LineString):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
+    def coordinates(self) -> List[DOUBLE]:
+        """
+        Coordinates
+        """
+        if self._args:
+            self._coordinates = unpack_line(*self._args)
+            self._args = None
+        # noinspection PyTypeChecker
+        return self._coordinates
+    # End coordinates property
+
+    @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
         return not len(self.coordinates)
     # End is_empty property
 
@@ -103,18 +78,18 @@
     # End points property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_coordinates(self.coordinates)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -122,45 +97,57 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LineString':
         """
         From Geopackage
         """
-        return _unpack_linestring(cls=cls, value=value, dimension=TWO_D)
+        return lazy_unpack(cls=cls, value=value, dimension=TWO_D)
     # End from_gpkg method
 # End LineString class
 
 
-class LineStringZ(AbstractGeopackageGeometryEnvelope):
+class LineStringZ(AbstractGeometry):
     """
     LineStringZ
     """
-    __slots__ = 'coordinates',
+    __slots__ = '_coordinates',
 
     def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
         """
         Initialize the LineStringZ class
         """
         super().__init__(srs_id=srs_id)
-        self.coordinates: List[TRIPLE] = coordinates
+        self._coordinates: List[TRIPLE] = coordinates
     # End init built-in
 
     def __eq__(self, other: 'LineStringZ') -> bool:
         """
         Equals
         """
         if not isinstance(other, LineStringZ):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
+    def coordinates(self) -> List[TRIPLE]:
+        """
+        Coordinates
+        """
+        if self._args:
+            self._coordinates = unpack_line(*self._args)
+            self._args = None
+        # noinspection PyTypeChecker
+        return self._coordinates
+    # End coordinates property
+
+    @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
         return not len(self.coordinates)
     # End is_empty property
 
@@ -175,18 +162,18 @@
     # End points property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_coordinates_z(self.coordinates)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -195,45 +182,57 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LineStringZ':
         """
         From Geopackage
         """
-        return _unpack_linestring(cls=cls, value=value, dimension=THREE_D)
+        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
     # End from_gpkg method
 # End LineStringZ class
 
 
-class LineStringM(AbstractGeopackageGeometryEnvelope):
+class LineStringM(AbstractGeometry):
     """
     LineStringM
     """
-    __slots__ = 'coordinates',
+    __slots__ = '_coordinates',
 
     def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
         """
         Initialize the LineStringM class
         """
         super().__init__(srs_id=srs_id)
-        self.coordinates: List[TRIPLE] = coordinates
+        self._coordinates: List[TRIPLE] = coordinates
     # End init built-in
 
     def __eq__(self, other: 'LineStringM') -> bool:
         """
         Equals
         """
         if not isinstance(other, LineStringM):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
+    def coordinates(self) -> List[TRIPLE]:
+        """
+        Coordinates
+        """
+        if self._args:
+            self._coordinates = unpack_line(*self._args)
+            self._args = None
+        # noinspection PyTypeChecker
+        return self._coordinates
+    # End coordinates property
+
+    @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
         return not len(self.coordinates)
     # End is_empty property
 
@@ -248,18 +247,18 @@
     # End points property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_coordinates_m(self.coordinates)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -268,45 +267,57 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LineStringM':
         """
         From Geopackage
         """
-        return _unpack_linestring(cls=cls, value=value, dimension=THREE_D)
+        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
     # End from_gpkg method
 # End LineStringM class
 
 
-class LineStringZM(AbstractGeopackageGeometryEnvelope):
+class LineStringZM(AbstractGeometry):
     """
     LineStringZM
     """
-    __slots__ = 'coordinates',
+    __slots__ = '_coordinates',
 
     def __init__(self, coordinates: List[QUADRUPLE], srs_id: int) -> None:
         """
         Initialize the LineStringZM class
         """
         super().__init__(srs_id=srs_id)
-        self.coordinates: List[QUADRUPLE] = coordinates
+        self._coordinates: List[QUADRUPLE] = coordinates
     # End init built-in
 
     def __eq__(self, other: 'LineStringZM') -> bool:
         """
         Equals
         """
         if not isinstance(other, LineStringZM):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
+    def coordinates(self) -> List[QUADRUPLE]:
+        """
+        Coordinates
+        """
+        if self._args:
+            self._coordinates = unpack_line(*self._args)
+            self._args = None
+        # noinspection PyTypeChecker
+        return self._coordinates
+    # End coordinates property
+
+    @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
         return not len(self.coordinates)
     # End is_empty property
 
@@ -321,18 +332,18 @@
     # End points property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_coordinates_zm(self.coordinates)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -341,51 +352,70 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LineStringZM':
         """
         From Geopackage
         """
-        return _unpack_linestring(cls=cls, value=value, dimension=FOUR_D)
+        return lazy_unpack(cls=cls, value=value, dimension=FOUR_D)
     # End from_gpkg method
 # End LineStringZM class
 
 
-class MultiLineString(AbstractGeopackageGeometryEnvelope):
+class MultiLineString(AbstractGeometry):
     """
     Multi LineString
     """
-    __slots__ = 'lines',
+    __slots__ = '_lines',
 
     def __init__(self, coordinates: List[List[DOUBLE]], srs_id: int) -> None:
         """
         Initialize the MultiLineString class
         """
         super().__init__(srs_id=srs_id)
-        self.lines: List[LineString] = [
-            LineString(coords, srs_id=srs_id) for coords in coordinates]
+        self._lines: List[LineString] = self._make_lines(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'MultiLineString') -> bool:
         """
         Equals
         """
         if not isinstance(other, MultiLineString):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.lines == other.lines
     # End eq built-in
 
+    def _make_lines(self, coordinates: List[List[DOUBLE]]) -> List[LineString]:
+        """
+        Make Lines
+        """
+        srs_id = self.srs_id
+        return [LineString(coords, srs_id=srs_id) for coords in coordinates]
+    # End init built-in
+
+    @property
+    def lines(self) -> List[LineString]:
+        """
+        Lines
+        """
+        if self._args:
+            # noinspection PyTypeChecker
+            self._lines = self._make_lines(unpack_lines(*self._args))
+            self._args = None
+        return self._lines
+    # End lines property
+
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return not len(self.lines)
+        return not (bool(self._args) or bool(self.lines))
     # End is_empty property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
         geoms = self.lines
@@ -394,74 +424,93 @@
     # End _to_wkb method
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_geometries(self.lines)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiLineString':
         """
         From Geopackage
         """
-        return _unpack_multi_linestring(cls=cls, value=value, dimension=TWO_D)
+        return lazy_unpack(cls=cls, value=value, dimension=TWO_D)
     # End from_gpkg method
 # End MultiLineString class
 
 
-class MultiLineStringZ(AbstractGeopackageGeometryEnvelope):
+class MultiLineStringZ(AbstractGeometry):
     """
     Multi LineString Z
     """
-    __slots__ = 'lines',
+    __slots__ = '_lines',
 
     def __init__(self, coordinates: List[List[TRIPLE]], srs_id: int) -> None:
         """
         Initialize the MultiLineStringZ class
         """
         super().__init__(srs_id=srs_id)
-        self.lines: List[LineStringZ] = [
-            LineStringZ(coords, srs_id=srs_id) for coords in coordinates]
+        self._lines: List[LineStringZ] = self._make_lines(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'MultiLineStringZ') -> bool:
         """
         Equals
         """
         if not isinstance(other, MultiLineStringZ):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.lines == other.lines
     # End eq built-in
 
+    def _make_lines(self, coordinates: List[List[TRIPLE]]) -> List[LineStringZ]:
+        """
+        Make Lines
+        """
+        srs_id = self.srs_id
+        return [LineStringZ(coords, srs_id=srs_id) for coords in coordinates]
+    # End init built-in
+
+    @property
+    def lines(self) -> List[LineStringZ]:
+        """
+        Lines
+        """
+        if self._args:
+            # noinspection PyTypeChecker
+            self._lines = self._make_lines(unpack_lines(*self._args))
+            self._args = None
+        return self._lines
+    # End lines property
+
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return not len(self.lines)
+        return not (bool(self._args) or bool(self.lines))
     # End is_empty property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_geometries_z(self.lines)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -471,62 +520,81 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiLineStringZ':
         """
         From Geopackage
         """
-        return _unpack_multi_linestring(cls=cls, value=value, dimension=THREE_D)
+        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
     # End from_gpkg method
 # End MultiLineStringZ class
 
 
-class MultiLineStringM(AbstractGeopackageGeometryEnvelope):
+class MultiLineStringM(AbstractGeometry):
     """
     Multi LineString M
     """
-    __slots__ = 'lines',
+    __slots__ = '_lines',
 
     def __init__(self, coordinates: List[List[TRIPLE]], srs_id: int) -> None:
         """
         Initialize the MultiLineStringM class
         """
         super().__init__(srs_id=srs_id)
-        self.lines: List[LineStringM] = [
-            LineStringM(coords, srs_id=srs_id) for coords in coordinates]
+        self._lines: List[LineStringM] = self._make_lines(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'MultiLineStringM') -> bool:
         """
         Equals
         """
         if not isinstance(other, MultiLineStringM):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.lines == other.lines
     # End eq built-in
 
+    def _make_lines(self, coordinates: List[List[TRIPLE]]) -> List[LineStringM]:
+        """
+        Make Lines
+        """
+        srs_id = self.srs_id
+        return [LineStringM(coords, srs_id=srs_id) for coords in coordinates]
+    # End init built-in
+
+    @property
+    def lines(self) -> List[LineStringM]:
+        """
+        Lines
+        """
+        if self._args:
+            # noinspection PyTypeChecker
+            self._lines = self._make_lines(unpack_lines(*self._args))
+            self._args = None
+        return self._lines
+    # End lines property
+
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return not len(self.lines)
+        return not (bool(self._args) or bool(self.lines))
     # End is_empty property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_geometries_m(self.lines)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -536,62 +604,82 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiLineStringM':
         """
         From Geopackage
         """
-        return _unpack_multi_linestring(cls=cls, value=value, dimension=THREE_D)
+        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
     # End from_gpkg method
 # End MultiLineStringM class
 
 
-class MultiLineStringZM(AbstractGeopackageGeometryEnvelope):
+class MultiLineStringZM(AbstractGeometry):
     """
     Multi LineString ZM
     """
-    __slots__ = 'lines',
+    __slots__ = '_lines',
 
     def __init__(self, coordinates: List[List[QUADRUPLE]], srs_id: int) -> None:
         """
         Initialize the MultiLineStringZM class
         """
         super().__init__(srs_id=srs_id)
-        self.lines: List[LineStringZM] = [
-            LineStringZM(coords, srs_id=srs_id) for coords in coordinates]
+        self._lines: List[LineStringZM] = self._make_lines(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'MultiLineStringZM') -> bool:
         """
         Equals
         """
         if not isinstance(other, MultiLineStringZM):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.lines == other.lines
     # End eq built-in
 
+    def _make_lines(self, coordinates: List[List[QUADRUPLE]]) \
+            -> List[LineStringZM]:
+        """
+        Make Lines
+        """
+        srs_id = self.srs_id
+        return [LineStringZM(coords, srs_id=srs_id) for coords in coordinates]
+    # End init built-in
+
+    @property
+    def lines(self) -> List[LineStringZM]:
+        """
+        Lines
+        """
+        if self._args:
+            # noinspection PyTypeChecker
+            self._lines = self._make_lines(unpack_lines(*self._args))
+            self._args = None
+        return self._lines
+    # End lines property
+
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return not len(self.lines)
+        return not (bool(self._args) or bool(self.lines))
     # End is_empty property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_geometries_zm(self.lines)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -601,14 +689,14 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiLineStringZM':
         """
         From Geopackage
         """
-        return _unpack_multi_linestring(cls=cls, value=value, dimension=FOUR_D)
+        return lazy_unpack(cls=cls, value=value, dimension=FOUR_D)
     # End from_gpkg method
 # End MultiLineStringZM class
 
 
 if __name__ == '__main__':  # pragma: no cover
     pass
```

## fudgeo/geometry/point.py

```diff
@@ -2,51 +2,31 @@
 """
 Points
 """
 
 
 from math import isnan, nan
 from struct import pack, unpack
-from typing import Any, List, Type, Union
+from typing import List
 
 from fudgeo.constant import (
     DOUBLE, EMPTY, FOUR_D, FOUR_D_PACK_CODE, FOUR_D_UNPACK_CODE, HEADER_OFFSET,
     QUADRUPLE, THREE_D, THREE_D_PACK_CODE, THREE_D_UNPACK_CODE, TRIPLE, TWO_D,
     TWO_D_PACK_CODE, TWO_D_UNPACK_CODE, WKB_MULTI_POINT_M_PRE,
     WKB_MULTI_POINT_PRE, WKB_MULTI_POINT_ZM_PRE, WKB_MULTI_POINT_Z_PRE,
     WKB_POINT_M_PRE, WKB_POINT_PRE, WKB_POINT_ZM_PRE, WKB_POINT_Z_PRE)
-from fudgeo.geometry.base import (
-    AbstractGeopackageGeometry, AbstractGeopackageGeometryEnvelope)
+from fudgeo.geometry.base import AbstractGeometry
 from fudgeo.geometry.util import (
     EMPTY_ENVELOPE, Envelope, envelope_from_coordinates,
     envelope_from_coordinates_m, envelope_from_coordinates_z,
-    envelope_from_coordinates_zm, pack_coordinates, unpack_envelope,
+    envelope_from_coordinates_zm, lazy_unpack, make_header, pack_coordinates,
     unpack_header, unpack_points)
 
 
-MULTI_POINT_TYPES = Union[Type['MultiPoint'], Type['MultiPointZ'],
-                          Type['MultiPointM'], Type['MultiPointZM']]
-
-
-def _unpack_multi_point(cls: MULTI_POINT_TYPES, value: bytes,
-                        dimension: int) -> Any:
-    """
-    Unpack Points into MultiPoint
-    """
-    srs_id, env_code, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
-    if is_empty:
-        return cls([], srs_id=srs_id)
-    # noinspection PyTypeChecker
-    obj = cls(unpack_points(value[offset:], dimension=dimension), srs_id=srs_id)
-    obj._envelope = unpack_envelope(code=env_code, value=value[:offset])
-    return obj
-# End _unpack_multi_point function
-
-
-class Point(AbstractGeopackageGeometry):
+class Point(AbstractGeometry):
     """
     Point
     """
     __slots__ = 'x', 'y'
 
     def __init__(self, *, x: float, y: float, srs_id: int) -> None:
         """
@@ -89,14 +69,30 @@
         """
         To WKB
         """
         pre = WKB_POINT_PRE if use_prefix else EMPTY
         return pre + pack(TWO_D_PACK_CODE, self.x, self.y)
     # End _to_wkb method
 
+    @property
+    def envelope(self) -> Envelope:
+        """
+        Envelope
+        """
+        return EMPTY_ENVELOPE
+    # End envelope property
+
+    def to_gpkg(self) -> bytes:
+        """
+        To Geopackage
+        """
+        return (make_header(srs_id=self.srs_id, is_empty=self.is_empty,
+                            envelope_code=0) + self._to_wkb())
+    # End to_gpkg method
+
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'Point':
         """
         From Geopackage
         """
         srs_id, _, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
         if is_empty:
@@ -120,15 +116,15 @@
         Empty Point
         """
         return cls(x=nan, y=nan, srs_id=srs_id)
     # End empty method
 # End Point class
 
 
-class PointZ(AbstractGeopackageGeometry):
+class PointZ(AbstractGeometry):
     """
     Point Z
     """
     __slots__ = 'x', 'y', 'z'
 
     def __init__(self, *, x: float, y: float, z: float, srs_id: int) -> None:
         """
@@ -172,14 +168,30 @@
         """
         To WKB
         """
         pre = WKB_POINT_Z_PRE if use_prefix else EMPTY
         return pre + pack(THREE_D_PACK_CODE, self.x, self.y, self.z)
     # End _to_wkb method
 
+    @property
+    def envelope(self) -> Envelope:
+        """
+        Envelope
+        """
+        return EMPTY_ENVELOPE
+    # End envelope property
+
+    def to_gpkg(self) -> bytes:
+        """
+        To Geopackage
+        """
+        return (make_header(srs_id=self.srs_id, is_empty=self.is_empty,
+                            envelope_code=0) + self._to_wkb())
+    # End to_gpkg method
+
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PointZ':
         """
         From Geopackage
         """
         srs_id, _, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
         if is_empty:
@@ -203,15 +215,15 @@
         Empty PointZ
         """
         return cls(x=nan, y=nan, z=nan, srs_id=srs_id)
     # End empty method
 # End PointZ class
 
 
-class PointM(AbstractGeopackageGeometry):
+class PointM(AbstractGeometry):
     """
     Point M
     """
     __slots__ = 'x', 'y', 'm'
 
     def __init__(self, *, x: float, y: float, m: float, srs_id: int) -> None:
         """
@@ -255,14 +267,30 @@
         """
         To WKB
         """
         pre = WKB_POINT_M_PRE if use_prefix else EMPTY
         return pre + pack(THREE_D_PACK_CODE, self.x, self.y, self.m)
     # End _to_wkb method
 
+    @property
+    def envelope(self) -> Envelope:
+        """
+        Envelope
+        """
+        return EMPTY_ENVELOPE
+    # End envelope property
+
+    def to_gpkg(self) -> bytes:
+        """
+        To Geopackage
+        """
+        return (make_header(srs_id=self.srs_id, is_empty=self.is_empty,
+                            envelope_code=0) + self._to_wkb())
+    # End to_gpkg method
+
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PointM':
         """
         From Geopackage
         """
         srs_id, _, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
         if is_empty:
@@ -286,15 +314,15 @@
         Empty PointM
         """
         return cls(x=nan, y=nan, m=nan, srs_id=srs_id)
     # End empty method
 # End PointM class
 
 
-class PointZM(AbstractGeopackageGeometry):
+class PointZM(AbstractGeometry):
     """
     Point ZM
     """
     __slots__ = 'x', 'y', 'z', 'm'
 
     def __init__(self, *, x: float, y: float, z: float, m: float,
                  srs_id: int) -> None:
@@ -342,14 +370,30 @@
         """
         To WKB
         """
         pre = WKB_POINT_ZM_PRE if use_prefix else EMPTY
         return pre + pack(FOUR_D_PACK_CODE, self.x, self.y, self.z, self.m)
     # End _to_wkb method
 
+    @property
+    def envelope(self) -> Envelope:
+        """
+        Envelope
+        """
+        return EMPTY_ENVELOPE
+    # End envelope property
+
+    def to_gpkg(self) -> bytes:
+        """
+        To Geopackage
+        """
+        return (make_header(srs_id=self.srs_id, is_empty=self.is_empty,
+                            envelope_code=0) + self._to_wkb())
+    # End to_gpkg method
+
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PointZM':
         """
         From Geopackage
         """
         srs_id, _, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
         if is_empty:
@@ -373,40 +417,52 @@
         Empty Point
         """
         return cls(x=nan, y=nan, z=nan, m=nan, srs_id=srs_id)
     # End empty method
 # End PointZM class
 
 
-class MultiPoint(AbstractGeopackageGeometryEnvelope):
+class MultiPoint(AbstractGeometry):
     """
     Multi Point
     """
-    __slots__ = 'coordinates',
+    __slots__ = '_coordinates',
 
     def __init__(self, coordinates: List[DOUBLE], srs_id: int) -> None:
         """
         Initialize the MultiPoint class
         """
         super().__init__(srs_id=srs_id)
-        self.coordinates: List[DOUBLE] = coordinates
+        self._coordinates: List[DOUBLE] = coordinates
     # End init built-in
 
     def __eq__(self, other: 'MultiPoint') -> bool:
         """
         Equals
         """
         if not isinstance(other, MultiPoint):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
+    def coordinates(self) -> List[DOUBLE]:
+        """
+        Coordinates
+        """
+        if self._args:
+            self._coordinates = unpack_points(*self._args)
+            self._args = None
+        # noinspection PyTypeChecker
+        return self._coordinates
+    # End coordinates property
+
+    @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
         return not len(self.coordinates)
     # End is_empty property
 
@@ -420,18 +476,18 @@
     # End points property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_coordinates(self.coordinates)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -440,45 +496,57 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPoint':
         """
         From Geopackage
         """
-        return _unpack_multi_point(cls=cls, value=value, dimension=TWO_D)
+        return lazy_unpack(cls=cls, value=value, dimension=TWO_D)
     # End from_gpkg method
 # End MultiPoint class
 
 
-class MultiPointZ(AbstractGeopackageGeometryEnvelope):
+class MultiPointZ(AbstractGeometry):
     """
     Multi Point Z
     """
-    __slots__ = 'coordinates',
+    __slots__ = '_coordinates',
 
     def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
         """
         Initialize the MultiPointZ class
         """
         super().__init__(srs_id=srs_id)
-        self.coordinates: List[TRIPLE] = coordinates
+        self._coordinates: List[TRIPLE] = coordinates
     # End init built-in
 
     def __eq__(self, other: 'MultiPointZ') -> bool:
         """
         Equals
         """
         if not isinstance(other, MultiPointZ):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
+    def coordinates(self) -> List[TRIPLE]:
+        """
+        Coordinates
+        """
+        if self._args:
+            self._coordinates = unpack_points(*self._args)
+            self._args = None
+        # noinspection PyTypeChecker
+        return self._coordinates
+    # End coordinates property
+
+    @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
         return not len(self.coordinates)
     # End is_empty property
 
@@ -493,18 +561,18 @@
     # End points property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_coordinates_z(self.coordinates)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -513,45 +581,57 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPointZ':
         """
         From Geopackage
         """
-        return _unpack_multi_point(cls=cls, value=value, dimension=THREE_D)
+        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
     # End from_gpkg method
 # End MultiPointZ class
 
 
-class MultiPointM(AbstractGeopackageGeometryEnvelope):
+class MultiPointM(AbstractGeometry):
     """
     Multi Point M
     """
-    __slots__ = 'coordinates',
+    __slots__ = '_coordinates',
 
     def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
         """
         Initialize the MultiPointM class
         """
         super().__init__(srs_id=srs_id)
-        self.coordinates: List[TRIPLE] = coordinates
+        self._coordinates: List[TRIPLE] = coordinates
     # End init built-in
 
     def __eq__(self, other: 'MultiPointM') -> bool:
         """
         Equals
         """
         if not isinstance(other, MultiPointM):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
+    def coordinates(self) -> List[TRIPLE]:
+        """
+        Coordinates
+        """
+        if self._args:
+            self._coordinates = unpack_points(*self._args)
+            self._args = None
+        # noinspection PyTypeChecker
+        return self._coordinates
+    # End coordinates property
+
+    @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
         return not len(self.coordinates)
     # End is_empty property
 
@@ -566,18 +646,18 @@
     # End points property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_coordinates_m(self.coordinates)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -586,45 +666,57 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPointM':
         """
         From Geopackage
         """
-        return _unpack_multi_point(cls=cls, value=value, dimension=THREE_D)
+        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
     # End from_gpkg method
 # End MultiPointM class
 
 
-class MultiPointZM(AbstractGeopackageGeometryEnvelope):
+class MultiPointZM(AbstractGeometry):
     """
     Multi Point ZM
     """
-    __slots__ = 'coordinates',
+    __slots__ = '_coordinates',
 
     def __init__(self, coordinates: List[QUADRUPLE], srs_id: int) -> None:
         """
         Initialize the MultiPointZM class
         """
         super().__init__(srs_id=srs_id)
-        self.coordinates: List[QUADRUPLE] = coordinates
+        self._coordinates: List[QUADRUPLE] = coordinates
     # End init built-in
 
     def __eq__(self, other: 'MultiPointZM') -> bool:
         """
         Equals
         """
         if not isinstance(other, MultiPointZM):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
+    def coordinates(self) -> List[QUADRUPLE]:
+        """
+        Coordinates
+        """
+        if self._args:
+            self._coordinates = unpack_points(*self._args)
+            self._args = None
+        # noinspection PyTypeChecker
+        return self._coordinates
+    # End coordinates property
+
+    @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
         return not len(self.coordinates)
     # End is_empty property
 
@@ -639,18 +731,18 @@
     # End points property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_coordinates_zm(self.coordinates)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -659,14 +751,14 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPointZM':
         """
         From Geopackage
         """
-        return _unpack_multi_point(cls=cls, value=value, dimension=FOUR_D)
+        return lazy_unpack(cls=cls, value=value, dimension=FOUR_D)
     # End from_gpkg method
 # End MultiPointZM class
 
 
 if __name__ == '__main__':  # pragma: no cover
     pass
```

## fudgeo/geometry/polygon.py

```diff
@@ -1,71 +1,33 @@
 # -*- coding: utf-8 -*-
 """
 Polygons
 """
 
 
 from struct import pack
-from typing import Any, List, Type, Union
+from typing import List
 
 from fudgeo.constant import (
-    COUNT_CODE, DOUBLE, FOUR_D, HEADER_OFFSET, QUADRUPLE, THREE_D, TRIPLE,
-    TWO_D, WKB_MULTI_POLYGON_M_PRE, WKB_MULTI_POLYGON_PRE,
-    WKB_MULTI_POLYGON_ZM_PRE, WKB_MULTI_POLYGON_Z_PRE, WKB_POLYGON_M_PRE,
-    WKB_POLYGON_PRE, WKB_POLYGON_ZM_PRE, WKB_POLYGON_Z_PRE)
-from fudgeo.geometry.base import (
-    AbstractGeopackageGeometryEnvelope, AbstractSpatialGeometryEnvelope)
+    COUNT_CODE, DOUBLE, FOUR_D, QUADRUPLE, THREE_D, TRIPLE, TWO_D,
+    WKB_MULTI_POLYGON_M_PRE, WKB_MULTI_POLYGON_PRE, WKB_MULTI_POLYGON_ZM_PRE,
+    WKB_MULTI_POLYGON_Z_PRE, WKB_POLYGON_M_PRE, WKB_POLYGON_PRE,
+    WKB_POLYGON_ZM_PRE, WKB_POLYGON_Z_PRE)
+from fudgeo.geometry.base import AbstractGeometry
 from fudgeo.geometry.point import Point, PointM, PointZ, PointZM
 from fudgeo.geometry.util import (
     EMPTY_ENVELOPE, Envelope, envelope_from_coordinates,
     envelope_from_coordinates_m, envelope_from_coordinates_z,
     envelope_from_coordinates_zm, envelope_from_geometries,
     envelope_from_geometries_m, envelope_from_geometries_z,
-    envelope_from_geometries_zm, pack_coordinates, unpack_envelope,
-    unpack_header, unpack_lines, unpack_polygons)
+    envelope_from_geometries_zm, lazy_unpack, pack_coordinates, unpack_lines,
+    unpack_polygons)
 
 
-POLYGON_TYPES = Union[Type['Polygon'], Type['PolygonZ'],
-                      Type['PolygonM'], Type['PolygonZM']]
-MULTI_POLYGON_TYPES = Union[Type['MultiPolygon'], Type['MultiPolygonZ'],
-                            Type['MultiPolygonM'], Type['MultiPolygonZM']]
-
-
-def _unpack_polygon(cls: POLYGON_TYPES, value: bytes, dimension: int) -> Any:
-    """
-    Unpack Linear Rings into Polygon
-    """
-    srs_id, env_code, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
-    if is_empty:
-        return cls([], srs_id=srs_id)
-    # noinspection PyTypeChecker
-    obj = cls(unpack_lines(value[offset:], dimension=dimension, is_ring=True),
-              srs_id=srs_id)
-    obj._envelope = unpack_envelope(code=env_code, value=value[:offset])
-    return obj
-# End _unpack_polygon function
-
-
-def _unpack_multi_polygon(cls: MULTI_POLYGON_TYPES, value: bytes,
-                          dimension: int) -> Any:
-    """
-    Unpack Polygons into MultiPolygon
-    """
-    srs_id, env_code, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
-    if is_empty:
-        return cls([], srs_id=srs_id)
-    # noinspection PyTypeChecker
-    obj = cls(unpack_polygons(value[offset:], dimension=dimension),
-              srs_id=srs_id)
-    obj._envelope = unpack_envelope(code=env_code, value=value[:offset])
-    return obj
-# End _unpack_multi_polygon function
-
-
-class LinearRing(AbstractSpatialGeometryEnvelope):
+class LinearRing(AbstractGeometry):
     """
     Linear Ring
     """
     __slots__ = 'coordinates',
 
     def __init__(self, coordinates: List[DOUBLE], srs_id: int) -> None:
         """
@@ -104,31 +66,39 @@
     # End points property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_coordinates(self.coordinates)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
         return pack_coordinates(self.coordinates)
     # End _to_wkb method
+
+    @classmethod
+    def from_gpkg(cls, value: bytes) -> 'LinearRing':  # pragma: nocover
+        """
+        From Geopackage, no-op for Linear Ring
+        """
+        pass
+    # End from_gpkg method
 # End LinearRing class
 
 
-class LinearRingZ(AbstractSpatialGeometryEnvelope):
+class LinearRingZ(AbstractGeometry):
     """
     Linear Ring Z
     """
     __slots__ = 'coordinates',
 
     def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
         """
@@ -175,24 +145,32 @@
     # End _to_wkb method
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_coordinates_z(self.coordinates)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
+
+    @classmethod
+    def from_gpkg(cls, value: bytes) -> 'LinearRingZ':  # pragma: nocover
+        """
+        From Geopackage, no-op for Linear Ring
+        """
+        pass
+    # End from_gpkg method
 # End LinearRingZ class
 
 
-class LinearRingM(AbstractSpatialGeometryEnvelope):
+class LinearRingM(AbstractGeometry):
     """
     Linear Ring M
     """
     __slots__ = 'coordinates',
 
     def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
         """
@@ -232,135 +210,171 @@
     # End points property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_coordinates_m(self.coordinates)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
         return pack_coordinates(self.coordinates, has_m=True)
     # End _to_wkb method
+
+    @classmethod
+    def from_gpkg(cls, value: bytes) -> 'LinearRingM':  # pragma: nocover
+        """
+        From Geopackage, no-op for Linear Ring
+        """
+        pass
+    # End from_gpkg method
 # End LinearRingM class
 
 
-class LinearRingZM(AbstractSpatialGeometryEnvelope):
+class LinearRingZM(AbstractGeometry):
     """
     Linear Ring ZM
     """
     __slots__ = 'coordinates',
 
     def __init__(self, coordinates: List[QUADRUPLE], srs_id: int) -> None:
         """
         Initialize the LinearRingZM class
         """
         super().__init__(srs_id=srs_id)
         self.coordinates: List[QUADRUPLE] = coordinates
     # End init built-in
 
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not len(self.coordinates)
-    # End is_empty property
-
     def __eq__(self, other: 'LinearRingZM') -> bool:
         """
         Equals
         """
         if not isinstance(other, LinearRingZM):  # pragma: nocover
             return NotImplemented
         return self.points == other.points
     # End eq built-in
 
     @property
+    def is_empty(self) -> bool:
+        """
+        Is Empty
+        """
+        return not len(self.coordinates)
+    # End is_empty property
+
+    @property
     def points(self) -> List[PointZM]:
         """
         Points
         """
         srs_id = self.srs_id
         return [PointZM(x=x, y=y, z=z, m=m, srs_id=srs_id)
                 for x, y, z, m in self.coordinates]
     # End points property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_coordinates_zm(self.coordinates)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
         return pack_coordinates(self.coordinates, has_z=True, has_m=True)
     # End _to_wkb method
+
+    @classmethod
+    def from_gpkg(cls, value: bytes) -> 'LinearRingZM':  # pragma: nocover
+        """
+        From Geopackage, no-op for Linear Ring
+        """
+        pass
+    # End from_gpkg method
 # End LinearRingZM class
 
 
-class Polygon(AbstractGeopackageGeometryEnvelope):
+class Polygon(AbstractGeometry):
     """
     Polygon
     """
-    __slots__ = 'rings',
+    __slots__ = '_rings',
 
     def __init__(self, coordinates: List[List[DOUBLE]], srs_id: int) -> None:
         """
         Initialize the Polygon class
         """
         super().__init__(srs_id=srs_id)
-        self.rings: List[LinearRing] = [
-            LinearRing(coords, srs_id=srs_id) for coords in coordinates]
+        self._rings: List[LinearRing] = self._make_rings(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'Polygon') -> bool:
         """
         Equals
         """
         if not isinstance(other, Polygon):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.rings == other.rings
     # End eq built-in
 
+    def _make_rings(self, coordinates: List[List[DOUBLE]]) -> List[LinearRing]:
+        """
+        Make Rings
+        """
+        srs_id = self.srs_id
+        return [LinearRing(coords, srs_id=srs_id) for coords in coordinates]
+    # End _make_rings method
+
+    @property
+    def rings(self) -> List[LinearRing]:
+        """
+        Rings
+        """
+        if self._args:
+            # noinspection PyTypeChecker
+            self._rings = self._make_rings(
+                unpack_lines(*self._args, is_ring=True))
+            self._args = None
+        return self._rings
+    # End rings property
+
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return not len(self.rings)
+        return not (bool(self._args) or bool(self.rings))
     # End is_empty property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_geometries(self.rings)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -370,62 +384,82 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'Polygon':
         """
         From Geopackage
         """
-        return _unpack_polygon(cls=cls, value=value, dimension=TWO_D)
+        return lazy_unpack(cls=cls, value=value, dimension=TWO_D)
     # End from_gpkg method
 # End Polygon class
 
 
-class PolygonZ(AbstractGeopackageGeometryEnvelope):
+class PolygonZ(AbstractGeometry):
     """
     Polygon Z
     """
-    __slots__ = 'rings',
+    __slots__ = '_rings',
 
     def __init__(self, coordinates: List[List[TRIPLE]], srs_id: int) -> None:
         """
         Initialize the PolygonZ class
         """
         super().__init__(srs_id=srs_id)
-        self.rings: List[LinearRingZ] = [
-            LinearRingZ(coords, srs_id=srs_id) for coords in coordinates]
+        self._rings: List[LinearRingZ] = self._make_rings(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'PolygonZ') -> bool:
         """
         Equals
         """
         if not isinstance(other, PolygonZ):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.rings == other.rings
     # End eq built-in
 
+    def _make_rings(self, coordinates: List[List[TRIPLE]]) -> List[LinearRingZ]:
+        """
+        Make Rings
+        """
+        srs_id = self.srs_id
+        return [LinearRingZ(coords, srs_id=srs_id) for coords in coordinates]
+    # End _make_rings method
+
+    @property
+    def rings(self) -> List[LinearRingZ]:
+        """
+        Rings
+        """
+        if self._args:
+            # noinspection PyTypeChecker
+            self._rings = self._make_rings(
+                unpack_lines(*self._args, is_ring=True))
+            self._args = None
+        return self._rings
+    # End rings property
+
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return not len(self.rings)
+        return not (bool(self._args) or bool(self.rings))
     # End is_empty property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_geometries_z(self.rings)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -435,62 +469,82 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PolygonZ':
         """
         From Geopackage
         """
-        return _unpack_polygon(cls=cls, value=value, dimension=THREE_D)
+        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
     # End from_gpkg method
 # End PolygonZ class
 
 
-class PolygonM(AbstractGeopackageGeometryEnvelope):
+class PolygonM(AbstractGeometry):
     """
     Polygon M
     """
-    __slots__ = 'rings',
+    __slots__ = '_rings',
 
     def __init__(self, coordinates: List[List[TRIPLE]], srs_id: int) -> None:
         """
         Initialize the PolygonM class
         """
         super().__init__(srs_id=srs_id)
-        self.rings: List[LinearRingM] = [
-            LinearRingM(coords, srs_id=srs_id) for coords in coordinates]
+        self._rings: List[LinearRingM] = self._make_rings(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'PolygonM') -> bool:
         """
         Equals
         """
         if not isinstance(other, PolygonM):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.rings == other.rings
     # End eq built-in
 
+    def _make_rings(self, coordinates: List[List[TRIPLE]]) -> List[LinearRingM]:
+        """
+        Make Rings
+        """
+        srs_id = self.srs_id
+        return [LinearRingM(coords, srs_id=srs_id) for coords in coordinates]
+    # End _make_rings method
+
+    @property
+    def rings(self) -> List[LinearRingM]:
+        """
+        Rings
+        """
+        if self._args:
+            # noinspection PyTypeChecker
+            self._rings = self._make_rings(
+                unpack_lines(*self._args, is_ring=True))
+            self._args = None
+        return self._rings
+    # End rings property
+
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return not len(self.rings)
+        return not (bool(self._args) or bool(self.rings))
     # End is_empty property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_geometries_m(self.rings)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -500,62 +554,83 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PolygonM':
         """
         From Geopackage
         """
-        return _unpack_polygon(cls=cls, value=value, dimension=THREE_D)
+        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
     # End from_gpkg method
 # End PolygonM class
 
 
-class PolygonZM(AbstractGeopackageGeometryEnvelope):
+class PolygonZM(AbstractGeometry):
     """
     Polygon ZM
     """
-    __slots__ = 'rings',
+    __slots__ = '_rings',
 
     def __init__(self, coordinates: List[List[QUADRUPLE]], srs_id: int) -> None:
         """
         Initialize the PolygonZM class
         """
         super().__init__(srs_id=srs_id)
-        self.rings: List[LinearRingZM] = [
-            LinearRingZM(coords, srs_id=srs_id) for coords in coordinates]
+        self._rings: List[LinearRingZM] = self._make_rings(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'PolygonZM') -> bool:
         """
         Equals
         """
         if not isinstance(other, PolygonZM):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.rings == other.rings
     # End eq built-in
 
+    def _make_rings(self, coordinates: List[List[QUADRUPLE]]) \
+            -> List[LinearRingZM]:
+        """
+        Make Rings
+        """
+        srs_id = self.srs_id
+        return [LinearRingZM(coords, srs_id=srs_id) for coords in coordinates]
+    # End _make_rings method
+
+    @property
+    def rings(self) -> List[LinearRingZM]:
+        """
+        Rings
+        """
+        if self._args:
+            # noinspection PyTypeChecker
+            self._rings = self._make_rings(
+                unpack_lines(*self._args, is_ring=True))
+            self._args = None
+        return self._rings
+    # End rings property
+
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return not len(self.rings)
+        return not (bool(self._args) or bool(self.rings))
     # End is_empty property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_geometries_zm(self.rings)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -565,63 +640,83 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PolygonZM':
         """
         From Geopackage
         """
-        return _unpack_polygon(cls=cls, value=value, dimension=FOUR_D)
+        return lazy_unpack(cls=cls, value=value, dimension=FOUR_D)
     # End from_gpkg method
 # End PolygonZM class
 
 
-class MultiPolygon(AbstractGeopackageGeometryEnvelope):
+class MultiPolygon(AbstractGeometry):
     """
     Multi Polygon
     """
-    __slots__ = 'polygons',
+    __slots__ = '_polygons',
 
     def __init__(self, coordinates: List[List[List[DOUBLE]]],
                  srs_id: int) -> None:
         """
         Initialize the MultiPolygon class
         """
         super().__init__(srs_id=srs_id)
-        self.polygons: List[Polygon] = [
-            Polygon(coords, srs_id=srs_id) for coords in coordinates]
+        self._polygons: List[Polygon] = self._make_polygons(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'MultiPolygon') -> bool:
         """
         Equals
         """
         if not isinstance(other, MultiPolygon):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.polygons == other.polygons
     # End eq built-in
 
+    def _make_polygons(self, coordinates: List[List[List[DOUBLE]]]) \
+            -> List[Polygon]:
+        """
+        Make Polygons
+        """
+        srs_id = self.srs_id
+        return [Polygon(coords, srs_id=srs_id) for coords in coordinates]
+    # End _make_polygons method
+
+    @property
+    def polygons(self) -> List[Polygon]:
+        """
+        Polygons
+        """
+        if self._args:
+            # noinspection PyTypeChecker
+            self._polygons = self._make_polygons(unpack_polygons(*self._args))
+            self._args = None
+        return self._polygons
+    # End polygons property
+
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return not len(self.polygons)
+        return not (bool(self._args) or bool(self.polygons))
     # End is_empty property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_geometries(self.polygons)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -631,63 +726,83 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPolygon':
         """
         From Geopackage
         """
-        return _unpack_multi_polygon(cls=cls, value=value, dimension=TWO_D)
+        return lazy_unpack(cls=cls, value=value, dimension=TWO_D)
     # End from_gpkg method
 # End MultiPolygon class
 
 
-class MultiPolygonZ(AbstractGeopackageGeometryEnvelope):
+class MultiPolygonZ(AbstractGeometry):
     """
     Multi Polygon Z
     """
-    __slots__ = 'polygons',
+    __slots__ = '_polygons',
 
     def __init__(self, coordinates: List[List[List[TRIPLE]]],
                  srs_id: int) -> None:
         """
         Initialize the MultiPolygonZ class
         """
         super().__init__(srs_id=srs_id)
-        self.polygons: List[PolygonZ] = [
-            PolygonZ(coords, srs_id=srs_id) for coords in coordinates]
+        self._polygons: List[PolygonZ] = self._make_polygons(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'MultiPolygonZ') -> bool:
         """
         Equals
         """
         if not isinstance(other, MultiPolygonZ):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.polygons == other.polygons
     # End eq built-in
 
+    def _make_polygons(self, coordinates: List[List[List[TRIPLE]]]) \
+            -> List[PolygonZ]:
+        """
+        Make Polygons
+        """
+        srs_id = self.srs_id
+        return [PolygonZ(coords, srs_id=srs_id) for coords in coordinates]
+    # End _make_polygons method
+
+    @property
+    def polygons(self) -> List[PolygonZ]:
+        """
+        Polygons
+        """
+        if self._args:
+            # noinspection PyTypeChecker
+            self._polygons = self._make_polygons(unpack_polygons(*self._args))
+            self._args = None
+        return self._polygons
+    # End polygons property
+
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return not len(self.polygons)
+        return not (bool(self._args) or bool(self.polygons))
     # End is_empty property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_geometries_z(self.polygons)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -697,63 +812,83 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPolygonZ':
         """
         From Geopackage
         """
-        return _unpack_multi_polygon(cls=cls, value=value, dimension=THREE_D)
+        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
     # End from_gpkg method
 # End MultiPolygonZ class
 
 
-class MultiPolygonM(AbstractGeopackageGeometryEnvelope):
+class MultiPolygonM(AbstractGeometry):
     """
     Multi Polygon M
     """
-    __slots__ = 'polygons',
+    __slots__ = '_polygons',
 
     def __init__(self, coordinates: List[List[List[TRIPLE]]],
                  srs_id: int) -> None:
         """
         Initialize the MultiPolygonM class
         """
         super().__init__(srs_id=srs_id)
-        self.polygons: List[PolygonM] = [
-            PolygonM(coords, srs_id=srs_id) for coords in coordinates]
+        self._polygons: List[PolygonM] = self._make_polygons(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'MultiPolygonM') -> bool:
         """
         Equals
         """
         if not isinstance(other, MultiPolygonM):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.polygons == other.polygons
     # End eq built-in
 
+    def _make_polygons(self, coordinates: List[List[List[TRIPLE]]]) \
+            -> List[PolygonM]:
+        """
+        Make Polygons
+        """
+        srs_id = self.srs_id
+        return [PolygonM(coords, srs_id=srs_id) for coords in coordinates]
+    # End _make_polygons method
+
+    @property
+    def polygons(self) -> List[PolygonM]:
+        """
+        Polygons
+        """
+        if self._args:
+            # noinspection PyTypeChecker
+            self._polygons = self._make_polygons(unpack_polygons(*self._args))
+            self._args = None
+        return self._polygons
+    # End polygons property
+
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return not len(self.polygons)
+        return not (bool(self._args) or bool(self.polygons))
     # End is_empty property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_geometries_m(self.polygons)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -763,63 +898,83 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPolygonM':
         """
         From Geopackage
         """
-        return _unpack_multi_polygon(cls=cls, value=value, dimension=THREE_D)
+        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
     # End from_gpkg method
 # End MultiPolygonM class
 
 
-class MultiPolygonZM(AbstractGeopackageGeometryEnvelope):
+class MultiPolygonZM(AbstractGeometry):
     """
     Multi Polygon M
     """
-    __slots__ = 'polygons',
+    __slots__ = '_polygons',
 
     def __init__(self, coordinates: List[List[List[QUADRUPLE]]],
                  srs_id: int) -> None:
         """
         Initialize the MultiPolygonZM class
         """
         super().__init__(srs_id=srs_id)
-        self.polygons: List[PolygonZM] = [
-            PolygonZM(coords, srs_id=srs_id) for coords in coordinates]
+        self._polygons: List[PolygonZM] = self._make_polygons(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'MultiPolygonZM') -> bool:
         """
         Equals
         """
         if not isinstance(other, MultiPolygonZM):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.polygons == other.polygons
     # End eq built-in
 
+    def _make_polygons(self, coordinates: List[List[List[QUADRUPLE]]]) \
+            -> List[PolygonZM]:
+        """
+        Make Polygons
+        """
+        srs_id = self.srs_id
+        return [PolygonZM(coords, srs_id=srs_id) for coords in coordinates]
+    # End _make_rings method
+
+    @property
+    def polygons(self) -> List[PolygonZM]:
+        """
+        Polygons
+        """
+        if self._args:
+            # noinspection PyTypeChecker
+            self._polygons = self._make_polygons(unpack_polygons(*self._args))
+            self._args = None
+        return self._polygons
+    # End polygons property
+
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return not len(self.polygons)
+        return not (bool(self._args) or bool(self.polygons))
     # End is_empty property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
-        if self._envelope is not EMPTY_ENVELOPE:
-            return self._envelope
+        if self._env is not EMPTY_ENVELOPE:
+            return self._env
         env = envelope_from_geometries_zm(self.polygons)
-        self._envelope = env
+        self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -829,14 +984,14 @@
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPolygonZM':
         """
         From Geopackage
         """
-        return _unpack_multi_polygon(cls=cls, value=value, dimension=FOUR_D)
+        return lazy_unpack(cls=cls, value=value, dimension=FOUR_D)
     # End from_gpkg method
 # End MultiPolygonZM class
 
 
 if __name__ == '__main__':  # pragma: no cover
     pass
```

## fudgeo/geometry/util.py

```diff
@@ -5,15 +5,15 @@
 
 
 from functools import lru_cache, reduce
 from math import isfinite, nan
 from operator import add
 # noinspection PyPep8Naming
 from struct import error as StructError, pack, unpack
-from typing import List, TYPE_CHECKING, Tuple, Union
+from typing import Any, List, TYPE_CHECKING, Tuple, Union
 
 from fudgeo.constant import (
     COORDINATES, COUNT_CODE, DOUBLE, EMPTY, ENVELOPE_COUNT, ENVELOPE_OFFSET,
     GP_MAGIC, HEADER_CODE, HEADER_OFFSET, POINT_PREFIX, QUADRUPLE, TRIPLE,
     TWO_D)
 
 
@@ -92,14 +92,33 @@
             return same_z
         same_m = self.min_m == other.min_m and self.max_m == other.max_m
         if code == 3:
             return same_m
         return same_m and same_z
     # End eq built-in
 
+    def to_wkb(self) -> Tuple[int, bytes]:
+        """
+        To WKB
+        """
+        code = self.code
+        if code not in {1, 2, 3, 4}:
+            return 0, EMPTY
+        values = self.min_x, self.max_x, self.min_y, self.max_y
+        if code == 1:
+            pass
+        elif code == 2:
+            values = *values, self.min_z, self.max_z
+        elif code == 3:
+            values = *values, self.min_m, self.max_m
+        elif code == 4:
+            values = *values, self.min_z, self.max_z, self.min_m, self.max_m
+        return code, pack(f'<{ENVELOPE_COUNT[code]}d', *values)
+    # End to_wkb method
+
     @property
     def code(self) -> int:
         """
         Envelope Code
         """
         return self._code
     # End code property
@@ -169,14 +188,28 @@
     # End max_m property
 # End Envelope class
 
 
 EMPTY_ENVELOPE = Envelope(code=0, min_x=nan, max_x=nan, min_y=nan, max_y=nan)
 
 
+def lazy_unpack(cls: Any, value: bytes, dimension: int) -> Any:
+    """
+    Unpack just the header and envelope, adding data to class for later use.
+    """
+    srs_id, env_code, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
+    obj = cls([], srs_id=srs_id)
+    if is_empty:
+        return obj
+    obj._env = unpack_envelope(code=env_code, value=value[:offset])
+    obj._args = value[offset:], dimension
+    return obj
+# End lazy_unpack function
+
+
 def unpack_line(value: bytes, dimension: int,
                 is_ring: bool = False) -> List[Tuple[float, ...]]:
     """
     Unpack Values for LineString
     """
     count, data = get_count_and_data(value, is_ring=is_ring)
     total = dimension * count
@@ -269,21 +302,23 @@
     header, data = value[first: second], value[second:]
     count, = unpack(COUNT_CODE, header)
     return count, data
 # End get_count_and_data function
 
 
 @lru_cache(maxsize=None)
-def make_header(srs_id: int, is_empty: bool) -> bytes:
+def make_header(srs_id: int, is_empty: bool, envelope_code: int = 0) -> bytes:
     """
     Cached Creation of a GeoPackage Geometry Header
     """
     flags = 1
     if is_empty:
         flags |= (1 << 4)
+        envelope_code = 0
+    flags |= (envelope_code << 1)
     return pack(HEADER_CODE, GP_MAGIC, 0, flags, srs_id)
 # End make_header function
 
 
 @lru_cache(maxsize=None)
 def unpack_header(value: bytes) -> Tuple[int, int, int, bool]:
     """
@@ -305,19 +340,19 @@
     1: envelope is [minx, maxx, miny, maxy], 32 bytes
     2: envelope is [minx, maxx, miny, maxy, minz, maxz], 48 bytes
     3: envelope is [minx, maxx, miny, maxy, minm, maxm], 48 bytes
     4: envelope is [minx, maxx, miny, maxy, minz, maxz, minm, maxm], 64 bytes
     """
     if not code:
         return EMPTY_ENVELOPE
-    if code not in ENVELOPE_COUNT:
+    if code not in ENVELOPE_COUNT:  # pragma: no cover
         return EMPTY_ENVELOPE
     try:
         values = unpack(f'<{ENVELOPE_COUNT[code]}d', value[HEADER_OFFSET:])
-    except StructError:
+    except StructError:  # pragma: no cover
         return EMPTY_ENVELOPE
     min_x = max_x = min_y = max_y = min_z = max_z = min_m = max_m = nan
     if code == 1:
         min_x, max_x, min_y, max_y = values
     elif code == 2:
         min_x, max_x, min_y, max_y, min_z, max_z = values
     elif code == 3:
@@ -331,15 +366,15 @@
 
 
 def _min_max(values: Union[VALUES, Tuple[float, ...]]) \
         -> Tuple[float, float]:
     """
     Min and Max values, returns nan's if empty list or no finite values.
     """
-    if not values:
+    if not len(values):
         return nan, nan
     values = [v for v in values if isfinite(v)]
     if not values:
         return nan, nan
     return min(values), max(values)
 # End _min_max function
 
@@ -359,15 +394,15 @@
 # End envelope_from_geometries function
 
 
 def envelope_from_geometries_z(geoms: GEOMS_Z) -> Envelope:
     """
     Envelope from Geometries with Z
     """
-    if not geoms:
+    if not geoms:  # pragma: no cover
         return EMPTY_ENVELOPE
     xs, ys, zs = [], [], []
     for geom in geoms:
         env = geom.envelope
         xs.extend((env.min_x, env.max_x))
         ys.extend((env.min_y, env.max_y))
         zs.extend((env.min_z, env.max_z))
@@ -375,15 +410,15 @@
 # End envelope_from_geometries_z function
 
 
 def envelope_from_geometries_m(geoms: GEOMS_M) -> Envelope:
     """
     Envelope from Geometries with M
     """
-    if not geoms:
+    if not geoms:  # pragma: no cover
         return EMPTY_ENVELOPE
     xs, ys, ms = [], [], []
     for geom in geoms:
         env = geom.envelope
         xs.extend((env.min_x, env.max_x))
         ys.extend((env.min_y, env.max_y))
         ms.extend((env.min_m, env.max_m))
@@ -408,45 +443,45 @@
 # End envelope_from_geometries_zm function
 
 
 def envelope_from_coordinates(coordinates: List[DOUBLE]) -> Envelope:
     """
     Envelope from Coordinates
     """
-    if not coordinates:
+    if not len(coordinates):
         return EMPTY_ENVELOPE
     return _envelope_xy(*zip(*coordinates))
 # End envelope_from_coordinates function
 
 
 def envelope_from_coordinates_z(coordinates: List[TRIPLE]) -> Envelope:
     """
     Envelope from Coordinates with Z
     """
-    if not coordinates:
+    if not len(coordinates):
         return EMPTY_ENVELOPE
     return _envelope_xyz(*zip(*coordinates))
 # End envelope_from_coordinates_z function
 
 
 def envelope_from_coordinates_m(coordinates: List[TRIPLE]) -> Envelope:
     """
     Envelope from Coordinates with M
     """
-    if not coordinates:
+    if not len(coordinates):
         return EMPTY_ENVELOPE
     return _envelope_xym(*zip(*coordinates))
 # End envelope_from_coordinates_m function
 
 
 def envelope_from_coordinates_zm(coordinates: List[QUADRUPLE]) -> Envelope:
     """
     Envelope from Coordinates with ZM
     """
-    if not coordinates:
+    if not len(coordinates):
         return EMPTY_ENVELOPE
     return _envelope_xyzm(*zip(*coordinates))
 # End envelope_from_coordinates_zm function
 
 
 def _envelope_xy(xs: VALUES, ys: VALUES) -> Envelope:
     """
```

## Comparing `fudgeo-0.4.1.dist-info/LICENSE` & `fudgeo-0.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fudgeo-0.4.1.dist-info/METADATA` & `fudgeo-0.4.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fudgeo
-Version: 0.4.1
+Version: 0.4.2
 Summary: GeoPackage support from Python.  fudgeo is a simple package for creating OGC GeoPackages, Feature Classes, Tables, and geometries (read and write).
 Author-email: "Integrated Informatics Inc." <contact@integrated-informatics.com>
 License: MIT License
         
         Copyright (c) 2021-2023 Integrated Informatics Inc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

## Comparing `fudgeo-0.4.1.dist-info/RECORD` & `fudgeo-0.4.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-fudgeo/__init__.py,sha256=f96KQWKKaRHvdLvNXZ9Rv3ANscOL_YEUJ6HTiAuCAms,117
+fudgeo/__init__.py,sha256=cfn0YWn5FEj8wmuqGYdPLxgfr48nxgwhRxVRhoq4R-4,117
 fudgeo/constant.py,sha256=-fE2Lyobm43rnDNzxsLUhaCfMMlaO5cCUmOFEL05LCQ,2538
 fudgeo/enumeration.py,sha256=NvgtVBYxfULGVIks-J0rFLRxvGrtU2DM1bjZB0HxZRU,1157
 fudgeo/geopkg.py,sha256=LL5uO82kL5CgTlIdxbr_2hiUf-kqDVXdtz8vDASXj_g,20081
 fudgeo/geopkg.sql,sha256=Tt0Fi4w-ySR7tDUJsPt-5mA_Sw2oUs8co5rFGEleS24,2673
 fudgeo/sql.py,sha256=AJcNZAjvGHvmc88NCU1TTsfjJ0tVZ6muTyNzA8yZcW0,7768
 fudgeo/geometry/__init__.py,sha256=N4sf5FJB13JoNxB_GyyO9ohXbtKoSoVvbKTnltMXq-0,974
-fudgeo/geometry/base.py,sha256=ETJLZMa6jb6A68QIzgPDWNjDoKnU7jq7AR_HevnDcEI,3250
-fudgeo/geometry/linestring.py,sha256=5tdWjJ9plRcvmU9PgXduVMQo_5cSz4XYK-PhZ2vixmQ,16963
-fudgeo/geometry/point.py,sha256=cgONWVNWC4C-c5TvZ3VuVoIRgnpBxfGo-SxypvARScc,17903
-fudgeo/geometry/polygon.py,sha256=pTVE2DXSAyzL1RmpBY5uOjlSKa21CpG7EvA2dC601CA,22719
-fudgeo/geometry/util.py,sha256=MkN3M-baAvzOvxNnLo6PHhX54j7MW4JfZVKJ3DAzlAY,14620
-fudgeo-0.4.1.dist-info/LICENSE,sha256=kg8K68wjqhzaDoPNP6FWgXT2UuLmZbswzv72syix3Gw,1088
-fudgeo-0.4.1.dist-info/METADATA,sha256=fm_GG0c2uPqvWvZ3cLfdSHb1qMNyQD7UEUxk8H5PUiQ,9095
-fudgeo-0.4.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fudgeo-0.4.1.dist-info/top_level.txt,sha256=RlcnukuWGTUINTexweATRDqQgM1d0q2iaOd6B6tBWWI,7
-fudgeo-0.4.1.dist-info/RECORD,,
+fudgeo/geometry/base.py,sha256=hON9Oft3X-8uOkqiFV7s74ZIgDKORmWkZkQjiY2d21o,2000
+fudgeo/geometry/linestring.py,sha256=2zN-nYmZ0vSEUmGnp5JhKjFCuXMjvmaZEoFSiKWEZK4,18653
+fudgeo/geometry/point.py,sha256=t32pw6nY9xJZCupzuETgywu2MDVhy-Wkc8b0YKfT1CM,19794
+fudgeo/geometry/polygon.py,sha256=8fZjh19hCjyakvk8Bt7SgbKO6I2n8Ldyft4FEczVHJo,26366
+fudgeo/geometry/util.py,sha256=pszHc8-5sKBJLtq7e4aZJhFs61gOfoxU7BK3HWI29kQ,15891
+fudgeo-0.4.2.dist-info/LICENSE,sha256=kg8K68wjqhzaDoPNP6FWgXT2UuLmZbswzv72syix3Gw,1088
+fudgeo-0.4.2.dist-info/METADATA,sha256=9Qk1zxRwRUEv_l6WGVGmUykZ71Tozap-xyOGnGW_8uc,9095
+fudgeo-0.4.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fudgeo-0.4.2.dist-info/top_level.txt,sha256=RlcnukuWGTUINTexweATRDqQgM1d0q2iaOd6B6tBWWI,7
+fudgeo-0.4.2.dist-info/RECORD,,
```

