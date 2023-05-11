# Comparing `tmp/euclidian-0.9.2.tar.gz` & `tmp/euclidian-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/euclidian-0.9.2.tar", last modified: Mon Jan 22 10:31:46 2018, max compression
+gzip compressed data, was "euclidian-0.9.4.tar", last modified: Thu May 11 09:27:57 2023, max compression
```

## Comparing `euclidian-0.9.2.tar` & `euclidian-0.9.4.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 rjs        (501) staff       (20)        0 2018-01-22 10:31:46.000000 euclidian-0.9.2/
--rw-r--r--   0 rjs        (501) staff       (20)     1073 2018-01-22 10:31:46.000000 euclidian-0.9.2/PKG-INFO
--rw-r--r--   0 rjs        (501) staff       (20)      138 2017-05-14 21:23:28.000000 euclidian-0.9.2/MANIFEST.in
--rw-r--r--   0 rjs        (501) staff       (20)     1660 2017-05-14 21:23:28.000000 euclidian-0.9.2/setup.py
--rw-r--r--   0 rjs        (501) staff       (20)       38 2018-01-22 10:31:46.000000 euclidian-0.9.2/setup.cfg
-drwxr-xr-x   0 rjs        (501) staff       (20)        0 2018-01-22 10:31:46.000000 euclidian-0.9.2/euclidian/
--rw-r--r--   0 rjs        (501) staff       (20)      699 2017-05-14 21:23:28.000000 euclidian-0.9.2/euclidian/util.py
--rw-r--r--   0 rjs        (501) staff       (20)      621 2017-05-14 21:23:28.000000 euclidian-0.9.2/euclidian/graycode.py
--rw-r--r--   0 rjs        (501) staff       (20)       22 2018-01-22 10:30:29.000000 euclidian-0.9.2/euclidian/__init__.py
--rw-r--r--   0 rjs        (501) staff       (20)      177 2017-05-14 21:23:28.000000 euclidian-0.9.2/euclidian/flipping.py
--rw-r--r--   0 rjs        (501) staff       (20)     4909 2017-05-14 21:23:28.000000 euclidian-0.9.2/euclidian/clipping.py
--rw-r--r--   0 rjs        (501) staff       (20)    60107 2018-01-11 06:30:03.000000 euclidian-0.9.2/euclidian/cartesian2.py
--rw-r--r--   0 rjs        (501) staff       (20)     1981 2017-05-14 21:23:28.000000 euclidian-0.9.2/euclidian/cartesian.py
--rw-r--r--   0 rjs        (501) staff       (20)    50043 2017-05-14 21:23:28.000000 euclidian-0.9.2/euclidian/cartesian3.py
--rw-r--r--   0 rjs        (501) staff       (20)      252 2017-05-14 21:23:28.000000 euclidian-0.9.2/README.rst
-drwxr-xr-x   0 rjs        (501) staff       (20)        0 2018-01-22 10:31:46.000000 euclidian-0.9.2/euclidian.egg-info/
--rw-r--r--   0 rjs        (501) staff       (20)     1073 2018-01-22 10:31:46.000000 euclidian-0.9.2/euclidian.egg-info/PKG-INFO
--rw-r--r--   0 rjs        (501) staff       (20)      340 2018-01-22 10:31:46.000000 euclidian-0.9.2/euclidian.egg-info/SOURCES.txt
--rw-r--r--   0 rjs        (501) staff       (20)       10 2018-01-22 10:31:46.000000 euclidian-0.9.2/euclidian.egg-info/top_level.txt
--rw-r--r--   0 rjs        (501) staff       (20)        1 2018-01-22 10:31:46.000000 euclidian-0.9.2/euclidian.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:27:57.299161 euclidian-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-11 09:27:40.000000 euclidian-0.9.4/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-11 09:27:57.299161 euclidian-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-11 09:27:40.000000 euclidian-0.9.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-11 09:27:40.000000 euclidian-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-11 09:27:57.299161 euclidian-0.9.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:27:57.291161 euclidian-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:27:57.295161 euclidian-0.9.4/src/euclidian/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 09:27:40.000000 euclidian-0.9.4/src/euclidian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-11 09:27:40.000000 euclidian-0.9.4/src/euclidian/cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60326 2023-05-11 09:27:40.000000 euclidian-0.9.4/src/euclidian/cartesian2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55393 2023-05-11 09:27:40.000000 euclidian-0.9.4/src/euclidian/cartesian3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-11 09:27:40.000000 euclidian-0.9.4/src/euclidian/clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-11 09:27:40.000000 euclidian-0.9.4/src/euclidian/flipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-11 09:27:40.000000 euclidian-0.9.4/src/euclidian/graycode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-11 09:27:40.000000 euclidian-0.9.4/src/euclidian/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 09:27:40.000000 euclidian-0.9.4/src/euclidian/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:27:57.299161 euclidian-0.9.4/src/euclidian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-11 09:27:57.000000 euclidian-0.9.4/src/euclidian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-11 09:27:57.000000 euclidian-0.9.4/src/euclidian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:27:57.000000 euclidian-0.9.4/src/euclidian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 09:27:57.000000 euclidian-0.9.4/src/euclidian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 09:27:57.000000 euclidian-0.9.4/src/euclidian.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:27:57.000000 euclidian-0.9.4/src/euclidian.egg-info/zip-safe
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `euclidian-0.9.2/PKG-INFO` & `euclidian-0.9.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: euclidian
-Version: 0.9.2
-Summary: Simple 2D and 3D geometric primitives and operations
-Home-page: http://code.sixty-north.com/euclidian
-Author: Robert Smallshire
-Author-email: rob@sixty-north.com
+Version: 0.9.4
+Summary: Basic geometric objects
+Home-page: https://github.com/sixty-north/euclidian
+Author: Sixty North
+Author-email: systems+euclidian@sixty-north.com
 License: MIT License
-Description-Content-Type: UNKNOWN
-Description: ``Euclidian`` is a lightweight 2D and 3D geometry library with no
-        pretentions to be fast, or especially robust around difficult edge
-        cases. The objectives are to be easy to use, be quick to learn, and
-        to be installable without onerous dependencies.
-        
-        
-        
-        
-Keywords: Python,geometry
-Platform: UNKNOWN
+Keywords: geometry vector point shape transformations
 Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+Provides-Extra: test
+License-File: LICENCE.txt
+
+*Euclidian* is a lightweight 2D and 3D geometry library with no
+pretensions to be fast, or especially robust around difficult edge
+cases. The objectives are to be easy to use, be quick to learn, and
+to be installable without onerous dependencies.
+
+
+
```

### Comparing `euclidian-0.9.2/euclidian/util.py` & `euclidian-0.9.4/src/euclidian/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 import sys
 
 
 def sign(x):
     return (x > 0) - (x < 0)
 
 def is_zero(x):
@@ -27,8 +28,17 @@
     return tuple(arg / s for arg in args)
 
 
 def almost_equal(x, y, epsilon=sys.float_info.epsilon):
     max_xy_one = max(1.0, abs(x), abs(y))
     e = epsilon * max_xy_one
     delta = abs(x - y)
-    return delta <= e
+    return delta <= e
+
+
+def safe_acos(
+    c):
+    if c > 1 and math.isclose(c, 1):
+        c = 1
+    if c < -1 and math.isclose(c, -1):
+        c = -1
+    return math.acos(c)
```

### Comparing `euclidian-0.9.2/euclidian/graycode.py` & `euclidian-0.9.4/src/euclidian/graycode.py`

 * *Files identical despite different names*

### Comparing `euclidian-0.9.2/euclidian/clipping.py` & `euclidian-0.9.4/src/euclidian/clipping.py`

 * *Files identical despite different names*

### Comparing `euclidian-0.9.2/euclidian/cartesian2.py` & `euclidian-0.9.4/src/euclidian/cartesian2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from collections import namedtuple
 import operator
 import sys
 import math
 
+
+from typename import typename
 from functools import singledispatch, total_ordering
 from numbers import Real
 from enum import Enum, unique
 import itertools
-from euclidian import graycode
 from euclidian.cartesian import Cartesian, SpaceMismatchError
 from euclidian.graycode import gray
 from euclidian.util import sign, all_equal, is_zero
 
 
 @unique
 class OrientedSide(Enum):
@@ -212,14 +213,17 @@
 
     def __len__(self):
         return len(self._d)
 
     def __iter__(self):
         return iter(self._d)
 
+    def items(self):
+        return zip(self.space, self._d)
+
     def __add__(self, rhs):
         if not isinstance(rhs, Vector2):
             return NotImplemented
         return Vector2(self._d[0] + rhs._d[0],
                        self._d[1] + rhs._d[1],
                        space=self.space)
 
@@ -421,15 +425,16 @@
         min_y = first[1]
         max_x = min_x
         max_y = min_y
 
         for index, point in enumerate(iterator, start=1):
             if point.space != space:
                 raise SpaceMismatchError(
-                    "Point at index {i} {!r} is not in the same space as first {!r}".format(index, point, first))
+                    f"Point at index {index} {point!r} is not in the same space as first {first!r}"
+                )
             min_x = min(min_x, point[0])
             min_y = min(min_y, point[1])
             max_x = max(max_x, point[0])
             max_y = max(max_y, point[1])
         return cls.from_extents(min_x - border, min_y - border, max_x + border, max_y + border)
 
     @classmethod
@@ -451,16 +456,17 @@
         min_y = first_bbox.min[1]
         max_x = first_bbox.max[0]
         max_y = first_bbox.max[1]
 
         for index, bounded in enumerate(iterator, start=1):
             if bounded.space != space:
                 raise SpaceMismatchError(
-                    "Bounded object at index {i} {!r} is not in the same space as first {!r}".format(index, bounded,
-                                                                                                     first))
+                    "Bounded object at index {index} {bounded!r} "
+                    "is not in the same space as first {first!r}"
+                )
 
             bbox = bounded.bounding_box()
             min_x = min(min_x, bbox.min[0])
             min_y = min(min_y, bbox.min[1])
             max_x = max(max_x, bbox.max[0])
             max_y = max(max_y, bbox.max[1])
         return cls.from_extents(min_x, min_y, max_x, max_y)
@@ -1076,28 +1082,22 @@
         ay1 = self.length_a() * self.a[1]
         by2 = self.length_b() * self.b[1]
         cy3 = self.length_c() * self.c[1]
         y = (ay1 + by2 + cy3) / self.perimeter()
         return Point2(x, y, space=self.space)
 
     def circumcenter(self):
-        if hasattr(self, '_circumcenter'):
-            return self._circumcenter
-
         if abs(self.a[1] - self.b[1]) < sys.float_info.epsilon and abs(self.b[1] - self.c[1]) < sys.float_info.epsilon:
             raise ArithmeticError("Cannot compute circumcenter for degenerate triangle")
 
         if abs(self.b[1] - self.a[1]) < sys.float_info.epsilon:
-            self._circumcenter = self._circumcenter_1()
+            return self._circumcenter_1()
         elif abs(self.c[1] - self.b[1]) < sys.float_info.epsilon:
-            self._circumcenter = self._circumcenter_2()
-        else:
-            self._circumcenter = self._circumcenter_3()
-
-        return self._circumcenter
+            return self._circumcenter_2()
+        return self._circumcenter_3()
 
     def _circumcenter_3(self):
         a = self.a
         b = self.b
         c = self.c
         m1 = -(b[0] - a[0]) / (b[1] - a[1])
         m2 = -(c[0] - b[0]) / (c[1] - b[1])
@@ -1406,27 +1406,27 @@
         yield self.angle_c()
         yield self.angle_d()
 
     @staticmethod
     def _angle_from_side_vectors(p, q):
         return p.angle(q)
 
-    def diagonal_ac(self):
+    def diagonal_ac(self) -> Segment2:
         return Segment2(self.a, self.c)
 
-    def diagonal_bd(self):
+    def diagonal_bd(self) -> Segment2:
         return Segment2(self.b, self.d)
 
     def is_convex(self):
-        return self.diagonal_ac.intersects(self.diagonal_bd)
+        return self.diagonal_ac().intersects(self.diagonal_bd)
 
-    def rectangularity(self):
+    def rectangularity(self) -> float:
         return max(self.angles()) - min(self.angles())
 
-    def is_rectangle(self):
+    def is_rectangle(self) -> bool:
         return self.rectangularity() == 0
 
     def __eq__(self, rhs):
         if not isinstance(rhs, Quadrilateral2):
             return NotImplemented
         return self.space == rhs.space and self._p == rhs._p
 
@@ -1539,15 +1539,21 @@
             return NotImplemented
         return self._m == rhs._m
 
     def __ne__(self, rhs):
         return not self == rhs
 
     def __repr__(self):
-        return '{}(a={}, c={}, b={}, d={}, tx={}, ty={})'.format(self.a, self.c, self.b, self.d, self.tx, self.ty)
+        return (
+            f"{typename(self)}("
+            f"a={self.a}, c={self.c}, "
+            f"b={self.b}, d={self.d}, "
+            f"tx={self.tx}, ty={self.ty}"
+            f")"
+        )
 
     def __mul__(self, rhs):
         if not isinstance(rhs, Transform2):
             return NotImplemented
         a1 = self.a
         b1 = self.b
         c1 = self.c
@@ -1634,14 +1640,15 @@
         if angle_degrees % 90 == 0:
             quadrant = int(angle_degrees) % 360
             method = getattr(self, 'rotate_{}_degrees'.format(quadrant))
             return method(center)
         return self.rotate(math.radians(angle_degrees), center)
 
     def rotate_0_degrees(self, center=None):
+        _ = center  # Keep the linter happy
         return self
 
     def rotate_90_degrees(self, center=None):
         center = Point2(0, 0) if center is None else center
         x = center[0]
         y = center[1]
         tx = x + y
@@ -1792,17 +1799,25 @@
         return self.a == 1 and self.c == 0 and self.b == 0 and self.d == 1 and self.tx == 0 and self.tx == 0
 
 IDENTITY_TRANSFORM2 = Transform2(1, 0, 0, 1, 0, 0)
 
 # TODO: Ensure these are in the right order, so we can reduce the transformations.
 Decomposition = namedtuple('Decomposition', ['translation', 'scaling', 'rotation', 'shearing'])
 
+def rotate2(obj, angle_radians):
+    t = Transform2.from_rotation(angle_radians)
+    return t(obj)
+
+def rotate_degrees2(obj, angle_degrees):
+    t = Transform2.from_rotation_degrees(angle_degrees)
+    return t(obj)
+
 @singledispatch
 def transform2(obj, transform):
-    raise NotImplemented("Transformation of {!r} not implemented".format(obj))
+    raise NotImplemented(f"Transformation of {obj!r} by {transform} not implemented")
 
 
 @transform2.register(Point2)
 def _(point, transform):
     return Point2(point.x * transform.a + point.y * transform.b + transform.tx,
                   point.x * transform.c + point.y * transform.d + transform.ty)
 
@@ -1846,15 +1861,15 @@
                 transform2(ray.point, transform))
 
 
 @transform2.register(Box2)
 def _(box, transform):
     # Not strictly a transformation of the box as such. Returns
     # A new axis-aligned Box2 which bounds the transformed box
-    return Box2.from_points(transform2(p) for p in box.vertices())
+    return Box2.from_points(transform2(p, transform) for p in box.vertices())
 
 
 def intersection2(a, b):
     return a.intersection(b)
 
 
 @singledispatch
```

### Comparing `euclidian-0.9.2/euclidian/cartesian.py` & `euclidian-0.9.4/src/euclidian/cartesian.py`

 * *Files identical despite different names*

### Comparing `euclidian-0.9.2/euclidian/cartesian3.py` & `euclidian-0.9.4/src/euclidian/cartesian3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from functools import total_ordering, singledispatch
 import math
 import itertools
 from numbers import Real
 import sys
+
 from euclidian.cartesian import SpaceMismatchError, Cartesian
 from euclidian.cartesian2 import determinant_2, Box2, Point2, Vector2, Direction2
 from euclidian.graycode import gray
-from euclidian.util import sign, is_zero, all_equal
+from euclidian.util import sign, is_zero, all_equal, safe_acos
 
 
 class Cartesian3(Cartesian):
 
     DEFAULT_AXES = ('x', 'y', 'z')
 
     @property
@@ -28,14 +29,26 @@
 
     @classmethod
     def from_vector(cls, vector, space=None):
         s = space if space is not None else vector.space
         return cls(vector[0], vector[1], vector[2], space=s)
 
     @classmethod
+    def from_subspace_point(cls, point2, space=None, **kwargs):
+        s = space if space is not None else Cartesian3.DEFAULT_AXES
+        v_args = dict(point2.items())
+        return cls(space=s, **v_args, **kwargs)
+
+    @classmethod
+    def from_subspace_vector(cls, vector2, space=None, **kwargs):
+        s = space if space is not None else Cartesian3.DEFAULT_AXES
+        v_args = dict(vector2.items())
+        return cls(space=s, **v_args, **kwargs)
+
+    @classmethod
     def as_midpoint(cls, p, q):
         if p.space != q.space:
             raise SpaceMismatchError("{!r} and {!r} are in different spaces".format(p, q))
         return cls((p[0] + q[0]) / 2,
                    (p[1] + q[1]) / 2,
                    (p[2] + q[2]) / 2,
                    space=p.space)
@@ -63,14 +76,23 @@
         except ValueError:
             raise AttributeError("Axis '{}' not recognized.".format(axis))
         return self._p[i]
 
     def __getitem__(self, index):
         return self._p[index]
 
+    def __len__(self):
+        return len(self._p)
+
+    def __iter__(self):
+        return iter(self._p)
+
+    def items(self):
+        return zip(self.space, self._p)
+
     def __sub__(self, rhs):
         if not isinstance(rhs, (Point3, Vector3)):
             return NotImplemented
         if self.space != rhs.space:
             raise SpaceMismatchError("Different spaces")
         if isinstance(rhs, Vector3):
             return Point3(self._p[0] - rhs[0],
@@ -283,39 +305,46 @@
         if m == 0:
             raise ZeroDivisionError("Cannot produce degenerate unit vector")
         return Vector3(self._d[0] / m,
                        self._d[1] / m,
                        self._d[2] / m,
                        space=self.space)
 
+    def vector(self):
+        return self
+
     def direction(self):
         return Direction3(self._d[0], self._d[1], self._d[2], space=self.space)
 
     def dot(self, rhs):
         return self._d[0] * rhs._d[0] + self._d[1] * rhs._d[1] + self._d[2] * rhs._d[2]
 
     def cross(self, rhs):
-        return Vector3(self._d[1]*rhs._d[2] - self._d[1]*rhs._d[1],
-                       self._d[1]*rhs._d[1] - self._d[1]*rhs._d[2],
-                       self._d[1]*rhs._d[1] - self._d[1]*rhs._d[1],
+        return Vector3(self._d[1]*rhs._d[2] - self._d[2]*rhs._d[1],
+                       self._d[2]*rhs._d[0] - self._d[0]*rhs._d[2],
+                       self._d[0]*rhs._d[1] - self._d[1]*rhs._d[0],
                        space=self.space)
 
     # def det(self, rhs):
     #     """If det (the determinant) is positive the angle between A (this) and B (rhs) is positive (counter-clockwise).
     #     If the determinant is negative the angle goes clockwise. Finally, if the determinant is 0, the
     #     vectors point in the same direction. In Schneider & Eberly this operator is called Kross.
-    #     Is is also often known as PerpDot.
+    #     It is also often known as PerpDot.
     #     """
     #     return determinant_2(self._d[0], self._d[1], rhs._d[0], rhs._d[1])
 
     # def angle(self, rhs):
     #     return math.atan2(abs(self.determinant(rhs)), self.dot(rhs))
 
     def angle(self, rhs):
-         theta = math.acos(self.dot(rhs) / (self.magnitude() * rhs.magnitude()))
+         dot = self.dot(rhs)
+         m1 = self.magnitude()
+         m2 = rhs.magnitude()
+         c = dot / (m1 * m2)
+         theta = safe_acos(c)
          return theta
 
     def components(self):
         """Decompose into three component vectors parallel to the basis vectors.
 
         Returns:
             A 3-tuple containing three Vector3 instances.
@@ -335,17 +364,23 @@
         return not self == rhs
 
     def __hash__(self):
         base_hash = super().__hash__()
         return hash((base_hash, self._d))
 
     def __repr__(self):
+        return format(self)
+
+    def __str__(self):
+        return format(self)
+
+    def __format__(self, f):
         return "{}({})".format(
-            self.__class__.__name__,
-            ', '.join('{}={}'.format(*item) for item in self.items()))
+            type(self).__name__,
+            ', '.join('{}={}'.format(key, format(value, f)) for key, value in self.items()))
 
     def subspace(self, subspace_axes):
         """Obtain a two-dimensional subspace representation of this vector.
 
         Args:
             subspace_axes: A 2-sequence of which each element is either and axis names as a string an integer
                 axis index.
@@ -359,18 +394,69 @@
         axis_specs = [self.axis_spec(subspace_axis) for subspace_axis in subspace_axes]
 
         return Vector2(self._d[axis_specs[0].index],
                        self._d[axis_specs[1].index],
                        space=[axis_spec.name for axis_spec in axis_specs])
 
 
+class SphericalCoordinates:
+
+    @classmethod
+    def from_direction(cls, direction):
+        u = direction.vector()
+        return cls.from_vector(u)
+
+    @classmethod
+    def from_vector(cls, u):
+        r = u.magnitude()
+        inclination = math.acos(u[2] / r)
+        azimuth = math.atan2(u[1], u[0])
+        return cls(azimuth, inclination)
+
+    @classmethod
+    def from_degrees(cls, azimuth_degrees, elevation_degrees):
+        return cls(math.radians(azimuth_degrees), math.radians(elevation_degrees))
+
+    def __init__(self, azimuth_radians, elevation_radians):
+        self._azimuth = azimuth_radians
+        self._elevation = elevation_radians
+
+    @property
+    def azimuth(self):
+        return self._azimuth
+
+
+    @property
+    def elevation(self):
+        return self._elevation
+
+
+    @property
+    def azimuth_degrees(self):
+        return math.degrees(self._azimuth)
+
+
+    @property
+    def elevation_degrees(self):
+        return math.degrees(self._elevation)
+
+
+BASIS_VECTOR3_0 = Vector3(1, 0, 0)
+BASIS_VECTOR3_1 = Vector3(0, 1, 0)
+BASIS_VECTOR3_2 = Vector3(0, 0, 1)
+
+
 class Direction3(Cartesian3):
     __slots__ = ['_d']
 
     @classmethod
+    def orthogonal_to(cls, v, w):
+        return v.vector().cross(w.vector()).direction()
+
+    @classmethod
     def between_points(cls, p, q):
         return (q - p).direction()
 
     def __init__(self, *args, **kwargs):
         try:
             space = kwargs.pop('space')
         except KeyError:
@@ -395,61 +481,108 @@
     def __getattr__(self, axis):
         try:
             i = self._space.index(axis)
         except ValueError:
             raise AttributeError("Axis '{}' not recognized.".format(axis))
         return self._d[i]
 
+    def __len__(self):
+        return 3
+
     def __getitem__(self, index):
         return self._d[index]
 
+    def direction(self):
+        return self
+
     def vector(self):
         return Vector3(self._d[0], self._d[1], self._d[2], space=self.space)
 
     def __eq__(self, rhs):
         if not isinstance(rhs, Direction3):
             return NotImplemented
-        # TODO!
-        raise NotImplementedError
+        u = self.vector().unit()
+        v = rhs.vector().unit()
+        return u.angle(v) == 0
+
+    def isclose(self, rhs, *, abs_tol=None):
+        if abs_tol is None:
+            abs_tol = 1e15
+        if not isinstance(rhs, Direction3):
+            raise TypeError("Can only compare to another Direction3")
+        return math.isclose(self.vector().unit().angle(rhs.vector().unit()), 0, abs_tol=abs_tol)
 
     def __ne__(self, rhs):
         if not isinstance(rhs, Direction3):
             return NotImplemented
         return not self == rhs
 
     def __pos__(self):
         return self
 
     def __neg__(self):
         return Direction3(-self._d[0], -self._d[1], -self._d[2], space=self.space)
 
     def __hash__(self):
         base_hash = super().__hash__()
-        return hash((base_hash, self._d))
+        u = self.vector().unit()  # Normalize so equal directions have equal hashes
+        return hash((base_hash, u._d))
 
     def __repr__(self):
         return "{}({})".format(
             self.__class__.__name__,
             ', '.join('{}={}'.format(axis, coord) for axis, coord in zip(self.space, self._d)))
 
     def angle(self, rhs):
         return self.vector().angle(rhs.vector())
 
-    def scalar_projection(self, vector):
-        """Scalar projection onto this direction."""
-        return self.vector().unit().dot(vector)
+    def scalar_projection(self, b):
+        """Scalar projection of a vector onto this direction.
+
+        Args:
+            b: The vector to project onto this direction.
 
-    def vector_projection(self, vector):
+        Returns:
+            The length of the projection of b onto this direction. If this direction
+            and the direction of b are in the same hemisphere, the result will be positive.
+            If b is perpendicular to this direction the result will be zero. If this direction
+            and the direction of b are in opposite hemispheres, the result will be negative.
+        """
+        a = self.vector().unit()
+        d = a.dot(b)
+        m = b.magnitude()
+        s = d / m
+        return s
+
+    def vector_projection(self, b):
         """The projection of a vector onto this direction.
+
+        Args:
+            b: The vector to project onto this direction.
+
+        Returns:
+            A vector with the length of the projection of b onto this
+            direction. If this direction and the direction of b are in the same hemisphere, the
+            result will be parallel to this direction. If b is perpendicular to this direction,
+            the result will be degenerate. If this direction and the direction of b are in opposite
+            hemispheres, the result will be antiparallel with this direction.
         """
-        unit = self.vector().unit()
-        return unit.dot(vector) * unit
+        return self.scalar_projection(b) * self.vector().unit()
+
+    def vector_rejection(self, b):
+        """The projection of a vector onto a place perpendicular to this vector.
 
-    def vector_rejection(self, vector):
-        return vector - self.vector_projection(vector)
+        Args:
+            b: The vector to project onto the perpendicular plane.
+
+        Returns:
+            The projection of b onto a plane perpendicular to this vector. If b is parallel or
+            antiparallel to this vector, the result is degenerate.
+        """
+        return b - self.vector_projection(b)
 
     def subspace(self, subspace_axes):
         """Obtain a two-dimensional subspace representation of this vector.
 
         Args:
             subspace_axes: A 2-sequence of which each element is either and axis names as a string an integer
                 axis index.
@@ -462,14 +595,17 @@
 
         axis_specs = [self.axis_spec(subspace_axis) for subspace_axis in subspace_axes]
 
         return Direction2(self._c[axis_specs[0].index],
                           self._c[axis_specs[1].index],
                           space=[axis_spec.name for axis_spec in axis_specs])
 
+    def reverse(self):
+        return Direction3(-self[0], -self[1], -self[2], space=self.space)
+
 
 class Box3(Cartesian3):
     __slots__ = ['_p']
 
     @classmethod
     def from_points(cls, points, border=0):
 
@@ -488,15 +624,16 @@
         max_y = min_y
         max_z = min_z
 
 
         for index, point in enumerate(iterator, start=1):
             if point.space != space:
                 raise SpaceMismatchError(
-                    "Point at index {i} {!r} is not in the same space as first {!r}".format(index, point, first))
+                    f"Point at index {index} {point!r} is not in the same space as first {first!r}"
+                )
             min_x = min(min_x, point[0])
             min_y = min(min_y, point[1])
             min_z = min(min_z, point[2])
             max_x = max(max_x, point[0])
             max_y = max(max_y, point[1])
             max_z = max(max_z, point[2])
 
@@ -524,16 +661,17 @@
         max_x = first_bbox.max[0]
         max_y = first_bbox.max[1]
         max_z = first_bbox.max[2]
 
         for index, bounded in enumerate(iterator, start=1):
             if bounded.space != space:
                 raise SpaceMismatchError(
-                    "Bounded object at index {i} {!r} is not in the same space as first {!r}".format(index, bounded,
-                                                                                                     first))
+                    "Bounded object at index {index} {bounded!r} "
+                    "is not in the same space as first {first!r}"
+                )
 
             bbox = bounded.bounding_box()
             min_x = min(min_x, bbox.min[0])
             min_y = min(min_y, bbox.min[1])
             min_z = min(min_z, bbox.min[2])
             max_x = max(max_x, bbox.max[0])
             max_y = max(max_y, bbox.max[1])
@@ -695,28 +833,45 @@
         b = c1 / c2
         return self._point + b * v
 
     def distance_to(self, p):
         projection = self.projection_from(p)
         return self._point.distance_to(projection)
 
+    def shortest_segment_between(self, l2):
+        """A segment between the nearest points on this line and another line.
+        """
+        l1 = self
+        p1 = l1.point()
+        p2 = l2.point()
+        d1 = l1.vector()
+        d2 = l2.vector()
+        n1 = d1.cross(d2)
+        n2 = d2.cross(n1)
+        c1 = p1 + ((p2 - p1).dot(n2)/d1.dot(n2)) * d1
+        c2 = p2 + ((p1 - p2).dor(n1)/d2.dot(n1)) * d2
+        return Segment3(c1, c2)
+
+
     def vector(self):
         """Vector parallel the line"""
         return self._vector
 
     def point(self, i=0):
         """Generate a point on the line.
 
         Args:
             i: By providing different values of i (which defaults to 0) distinct
                points on the line can be produced.
 
         Returns:
             A Point3 on the line.
         """
+        if i == 0:
+            return self._point
         return self._point + i * self._vector
 
     def is_parallel_to(self, line):
         v1 = self._vector
         v2 = line._vector
         s = v1.dot(v2) / (v1.magnitude() * v2.magnitude())
         return s >= 1 - sys.float_info.epsilon
@@ -823,15 +978,15 @@
         projection = self._p[0] + b * v
         return p.distance_to(projection)
 
     def projected_from(self, p):
         """Project a point onto this ray.
 
         Args:
-            point: The point to be projected.
+            p: The point to be projected.
 
         Return:
             The perpendicular projection of point onto this ray, or None.
         """
         if p.space != self.space:
             raise SpaceMismatchError("{!r} and {!r} are not in the same space".format(p, self))
 
@@ -903,20 +1058,29 @@
         dz = self.target[2] - self.source[2]
         return math.sqrt(dx*dx + dy*dy + dz*dz)
 
     def reversed(self):
         return Segment3(self.target, self.source)
 
     def lerp(self, t):
-        # TODO: Consider using this version which is more numerically stable lerp(p0, p1, t) = p0 * (1 - t) + p1 * t
+        # TODO: Consider using this version which is more numerically stable
+        #       lerp(p0, p1, t) = p0 * (1 - t) + p1 * t
         return Point3(self.source[0] + t * (self.target[0] - self.source[0]),
                       self.source[1] + t * (self.target[1] - self.source[1]),
                       self.source[2] + t * (self.target[2] - self.source[2]),
                       space=self.space)
 
+    def point_at_distance_from_source(self, distance):
+        t = distance / self.length()
+        return self.lerp(t)
+
+    def point_at_distance_from_target(self, distance):
+        t = 1 - (distance / self.length())
+        return self.lerp(t)
+
     def bounding_box(self):
         return Box3(*self._p)
 
     def distance_to(self, p):
         if p.space != self.space:
             raise SpaceMismatchError("{!r} and {!r} are not in the same space".format(p, self))
 
@@ -935,15 +1099,15 @@
         projection = self._p[0] + b * v
         return p.distance_to(projection)
 
     def projected_from(self, p):
         """Project a point onto this segment.
 
         Args:
-            point: The point to be projected.
+            p: The point to be projected.
 
         Return:
             The perpendicular projection of point onto this segment, or None.
         """
         if p.space != self.space:
             raise SpaceMismatchError("{!r} and {!r} are not in the same space".format(p, self))
 
@@ -1161,16 +1325,19 @@
         a, b, c, d = self._c
         if b == 0:
             raise ZeroDivisionError("Cannot solve for plane parallel to axis")
         y = -(a*x + c*z + d) / b
         return y
 
     def _solve_for_0(self, *args, **kwargs):
-        """Solve for axis 0 (the x axis) providing coordinates for axis 1 and axis 2 as either positional or
-        named arguments consistent with space axis naming."""
+        """Solve for axis 0 (the x-axis) providing coordinates for axis 1 and axis 2.
+
+        Coordinates may be provided as either positional or named arguments consistent with space
+        axis naming.
+        """
         y, z = self._parse_solve_args(args, kwargs, 1, 2)
         a, b, c, d = self._c
         if b == 0:
             raise ZeroDivisionError("Cannot solve for plane parallel to axis")
         x = -(b*y + c*z + d) / a
         return x
 
@@ -1261,45 +1428,57 @@
 
 class Transform3:
 
     @staticmethod
     def identity():
         return IDENTITY_TRANSFORM3
 
-    # @classmethod
-    # def from_rotation(cls, angle_radians, axis):
-    #      cos_theta = math.cos(angle_radians)
-    #      sin_theta = math.sin(angle_radians)
-    #
-    #      unit_axis = axis.unit()
-    #      l = unit_axis[0]
-    #      m = unit_axis[1]
-    #      n = unit_axis[2]
-    #
-    #      a = l*l*(1 - cos_theta) + cos_theta
-    #      b = l*m*(1 - cos_theta) + n*sin_theta
-    #      c = l*n*(1 - cos_theta) - m*sin_theta
-    #
-    #      d = m*l*(1 - cos_theta) - n*sin_theta
-    #      e = m*m*(1 - cos_theta) + cos_theta
-    #      f = m*n*(1 - cos_theta) + l*sin_theta
-    #
-    #      g = n*l*(1 - cos_theta) + m*sin_theta
-    #      h = n*m*(1 - cos_theta) - l*sin_theta
-    #      i = n*n*(1 - cos_theta) + cos_theta
-    #
-    #      return cls(a, d, g, b, e, h, c, f, i, 0, 0, 0)
+    @classmethod
+    def from_orthonormal_basis_vectors(
+            cls,
+            to_basis_0: Vector3,
+            to_basis_1: Vector3,
+            to_basis_2: Vector3,
+            from_basis_0=BASIS_VECTOR3_0,
+            from_basis_1=BASIS_VECTOR3_1,
+            from_basis_2=BASIS_VECTOR3_2,
+    ):
+        # Works for C node
+        # a = Vector3.dot(to_basis_0, from_basis_0)
+        # d = Vector3.dot(to_basis_0, from_basis_1)
+        # g = Vector3.dot(to_basis_0, from_basis_2)
+        # b = Vector3.dot(to_basis_1, from_basis_0)
+        # e = Vector3.dot(to_basis_1, from_basis_1)
+        # h = Vector3.dot(to_basis_1, from_basis_2)
+        # c = Vector3.dot(to_basis_2, from_basis_0)
+        # f = Vector3.dot(to_basis_2, from_basis_1)
+        # i = Vector3.dot(to_basis_2, from_basis_2)
+
+        # Works for B node
+        a = Vector3.dot(from_basis_0, to_basis_0)
+        d = Vector3.dot(from_basis_0, to_basis_1)
+        g = Vector3.dot(from_basis_0, to_basis_2)
+        b = Vector3.dot(from_basis_1, to_basis_0)
+        e = Vector3.dot(from_basis_1, to_basis_1)
+        h = Vector3.dot(from_basis_1, to_basis_2)
+        c = Vector3.dot(from_basis_2, to_basis_0)
+        f = Vector3.dot(from_basis_2, to_basis_1)
+        i = Vector3.dot(from_basis_2, to_basis_2)
+
+        return cls(a, d, g, b, e, h, c, f, i)
+
+
 
 
     @classmethod
     def from_rotation(cls, angle_radians, axis):
          cos_theta = math.cos(angle_radians)
          sin_theta = math.sin(angle_radians)
 
-         unit_axis = axis.unit()
+         unit_axis = axis.vector().unit()
          u = unit_axis[0]
          v = unit_axis[1]
          w = unit_axis[2]
 
          a = u*u + (1 - u*u)*cos_theta
          b = u*v*(1 - cos_theta) + w*sin_theta
          c = u*w*(1 - cos_theta) - v*sin_theta
@@ -1328,15 +1507,14 @@
 
     @classmethod
     def from_rotation_z(cls, angle_radians):
         return cls.identity().rotate_z(angle_radians)
 
     @classmethod
     def from_scale(cls, scale_factor, center=None):
-       # TODO: Optimise
        return cls.identity().scale(scale_factor, center)
 
     @classmethod
     def from_translation(cls, vector):
         return cls(1, 0, 0, 0, 1, 0, 0, 0, 1, vector[0], vector[1], vector[2])
 
     def __init__(self, a=0, d=0, g=0, b=0, e=0, h=0, c=0, f=0, i=0, tx=0, ty=0, tz=0):
@@ -1549,15 +1727,15 @@
         return self.a == 1 and self.d == 0 and self.c == 0 and self.b == 0 and self.e == 1 and self.h == 0 and self.c == 0 and self.f == 0 and self.i == 1 and self.tx == 0 and self.tx == 0 and self.tz == 0
 
 IDENTITY_TRANSFORM3 = Transform3(1, 0, 0, 0, 1, 0, 0, 0, 1, 0, 0, 0)
 
 
 @singledispatch
 def transform3(obj, transform):
-    raise NotImplemented("Transformation of {!r} not implemented".format(obj))
+    raise NotImplemented(f"Transformation of {obj!r} by {transform} not implemented")
 
 
 @transform3.register(Point3)
 def _(point, transform):
     return Point3(point.x * transform.a + point.y * transform.b + point.z * transform.c + transform.tx,
                   point.x * transform.d + point.y * transform.e + point.z * transform.f + transform.ty,
                   point.x * transform.g + point.y * transform.h + point.z * transform.i + transform.tz)
```

### Comparing `euclidian-0.9.2/euclidian.egg-info/PKG-INFO` & `euclidian-0.9.4/src/euclidian.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: euclidian
-Version: 0.9.2
-Summary: Simple 2D and 3D geometric primitives and operations
-Home-page: http://code.sixty-north.com/euclidian
-Author: Robert Smallshire
-Author-email: rob@sixty-north.com
+Version: 0.9.4
+Summary: Basic geometric objects
+Home-page: https://github.com/sixty-north/euclidian
+Author: Sixty North
+Author-email: systems+euclidian@sixty-north.com
 License: MIT License
-Description-Content-Type: UNKNOWN
-Description: ``Euclidian`` is a lightweight 2D and 3D geometry library with no
-        pretentions to be fast, or especially robust around difficult edge
-        cases. The objectives are to be easy to use, be quick to learn, and
-        to be installable without onerous dependencies.
-        
-        
-        
-        
-Keywords: Python,geometry
-Platform: UNKNOWN
+Keywords: geometry vector point shape transformations
 Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+Provides-Extra: test
+License-File: LICENCE.txt
+
+*Euclidian* is a lightweight 2D and 3D geometry library with no
+pretensions to be fast, or especially robust around difficult edge
+cases. The objectives are to be easy to use, be quick to learn, and
+to be installable without onerous dependencies.
+
+
+
```

