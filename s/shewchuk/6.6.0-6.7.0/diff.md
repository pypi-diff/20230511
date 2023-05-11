# Comparing `tmp/shewchuk-6.6.0.tar.gz` & `tmp/shewchuk-6.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shewchuk-6.6.0.tar", last modified: Sat Jan 21 00:31:02 2023, max compression
+gzip compressed data, was "shewchuk-6.7.0.tar", last modified: Thu May 11 00:21:19 2023, max compression
```

## Comparing `shewchuk-6.6.0.tar` & `shewchuk-6.7.0.tar`

### file list

```diff
@@ -1,20 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 00:31:02.779261 shewchuk-6.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-21 00:30:52.000000 shewchuk-6.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-21 00:30:52.000000 shewchuk-6.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-01-21 00:31:02.779261 shewchuk-6.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-01-21 00:30:52.000000 shewchuk-6.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-21 00:31:02.779261 shewchuk-6.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-01-21 00:30:52.000000 shewchuk-6.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 00:31:02.779261 shewchuk-6.6.0/shewchuk/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-01-21 00:30:52.000000 shewchuk-6.6.0/shewchuk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-01-21 00:30:52.000000 shewchuk-6.6.0/shewchuk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    68507 2023-01-21 00:30:52.000000 shewchuk-6.6.0/shewchuk/_shewchuk.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-21 00:30:52.000000 shewchuk-6.6.0/shewchuk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 00:31:02.779261 shewchuk-6.6.0/shewchuk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-01-21 00:31:02.000000 shewchuk-6.6.0/shewchuk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-21 00:31:02.000000 shewchuk-6.6.0/shewchuk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-21 00:31:02.000000 shewchuk-6.6.0/shewchuk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-21 00:31:02.000000 shewchuk-6.6.0/shewchuk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-21 00:31:02.000000 shewchuk-6.6.0/shewchuk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 00:31:02.779261 shewchuk-6.6.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)   119625 2023-01-21 00:30:52.000000 shewchuk-6.6.0/src/shewchuk.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:21:19.961995 shewchuk-6.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-11 00:21:06.000000 shewchuk-6.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-11 00:21:06.000000 shewchuk-6.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-11 00:21:19.961995 shewchuk-6.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-11 00:21:06.000000 shewchuk-6.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-11 00:21:06.000000 shewchuk-6.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 00:21:19.961995 shewchuk-6.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-11 00:21:06.000000 shewchuk-6.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:21:19.961995 shewchuk-6.7.0/shewchuk/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-11 00:21:06.000000 shewchuk-6.7.0/shewchuk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-11 00:21:06.000000 shewchuk-6.7.0/shewchuk/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    69147 2023-05-11 00:21:06.000000 shewchuk-6.7.0/shewchuk/_shewchuk.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:21:06.000000 shewchuk-6.7.0/shewchuk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:21:19.961995 shewchuk-6.7.0/shewchuk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-11 00:21:19.000000 shewchuk-6.7.0/shewchuk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-11 00:21:19.000000 shewchuk-6.7.0/shewchuk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:21:19.000000 shewchuk-6.7.0/shewchuk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:21:19.000000 shewchuk-6.7.0/shewchuk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 00:21:19.000000 shewchuk-6.7.0/shewchuk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 00:21:19.000000 shewchuk-6.7.0/shewchuk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:21:19.961995 shewchuk-6.7.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)   124073 2023-05-11 00:21:06.000000 shewchuk-6.7.0/src/shewchuk.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:21:19.961995 shewchuk-6.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-11 00:21:06.000000 shewchuk-6.7.0/tests/test_incircle_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-11 00:21:06.000000 shewchuk-6.7.0/tests/test_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-11 00:21:06.000000 shewchuk-6.7.0/tests/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-11 00:21:06.000000 shewchuk-6.7.0/tests/test_vectors_cross_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-11 00:21:06.000000 shewchuk-6.7.0/tests/test_vectors_dot_product.py
```

### Comparing `shewchuk-6.6.0/LICENSE` & `shewchuk-6.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shewchuk-6.6.0/PKG-INFO` & `shewchuk-6.7.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: shewchuk
-Version: 6.6.0
-Summary: Robust floating point operations.
-Home-page: https://github.com/lycantropos/shewchuk/
-Download-URL: https://github.com/lycantropos/shewchuk/archive/master.zip
-Author: Azat Ibrakov
-Author-email: azatibrakov@gmail.com
-License: MIT License
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 shewchuk
 ========
 
 [![](https://github.com/lycantropos/shewchuk/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/lycantropos/shewchuk/actions/workflows/ci.yml "Github Actions")
 [![](https://readthedocs.org/projects/shewchuk/badge/?version=latest)](https://shewchuk.readthedocs.io/en/latest/?badge=latest "Documentation")
 [![](https://codecov.io/gh/lycantropos/shewchuk/branch/master/graph/badge.svg)](https://codecov.io/gh/lycantropos/shewchuk "Codecov")
 [![](https://img.shields.io/github/license/lycantropos/shewchuk.svg)](https://github.com/lycantropos/shewchuk/blob/master/LICENSE "License")
```

### Comparing `shewchuk-6.6.0/shewchuk/__init__.py` & `shewchuk-6.7.0/shewchuk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Robust floating point operations."""
 
-__version__ = '6.6.0'
+__version__ = '6.7.0'
 
 try:
     from ._cshewchuk import (Expansion,
                              incircle_test,
                              kind,
                              orientation,
                              vectors_cross_product,
```

### Comparing `shewchuk-6.6.0/shewchuk/__init__.pyi` & `shewchuk-6.7.0/shewchuk/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     def real(self) -> _Real:
         ...
 
     @property
     def imag(self) -> _Real:
         ...
 
+    def as_integer_ratio(self) -> _t.Tuple[int, int]:
+        ...
+
     @_t.overload
     def __new__(cls, value: _t.Union[Expansion, _Number]) -> Expansion:
         ...
 
     @_t.overload
     def __new__(cls, *args: float) -> Expansion:
         ...
```

### Comparing `shewchuk-6.6.0/shewchuk/_shewchuk.py` & `shewchuk-6.7.0/shewchuk/_shewchuk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from __future__ import annotations
 
 import typing as _t
 from functools import reduce as _reduce
-from itertools import (dropwhile as _dropwhile,
-                       repeat as _repeat)
+from itertools import repeat as _repeat
 from math import (ceil as _ceil,
                   floor as _floor,
+                  gcd as _gcd,
                   isfinite as _isfinite,
                   modf as _modf)
 from numbers import (Rational as _Rational,
                      Real as _Real)
-from operator import not_ as _not
 from sys import float_info as _float_info
 
 _Number = _t.Union[_Rational, float, int]
 
 
 @_Real.register
 class Expansion:
@@ -26,14 +25,33 @@
         return self
 
     @property
     def imag(self) -> _Number:
         """The real part of the expansion."""
         return 0
 
+    def as_integer_ratio(self) -> _t.Tuple[int, int]:
+        result_numerator, result_denominator = (
+            self._components[0].as_integer_ratio()
+        )
+        for component in self._components[1:]:
+            component_numerator, component_denominator = (
+                component.as_integer_ratio()
+            )
+            result_numerator = (
+                    result_numerator * component_denominator
+                    + component_numerator * result_denominator
+            )
+            result_denominator = result_denominator * component_denominator
+            gcd = _gcd(result_numerator, result_denominator)
+            if gcd != 1:
+                result_numerator //= gcd
+                result_denominator //= gcd
+        return result_numerator, result_denominator
+
     _components: _t.Sequence[float]
 
     __slots__ = '_components',
 
     def __new__(cls,
                 _argument: _t.Union[Expansion, _Number] = 0.0,
                 *args: float,
@@ -135,44 +153,45 @@
                         else NotImplemented))))
 
     def __float__(self) -> float:
         assert sum(self._components) == self._components[-1], self
         return self._components[-1]
 
     def __floor__(self) -> int:
-        return (_components_to_integer(self._components)
-                + _floor(_components_to_accumulated_fraction(
-                        self._components)))
+        return (
+                _components_to_integer(self._components)
+                + _floor(_components_to_accumulated_fraction(self._components))
+        )
 
     @_t.overload
     def __ge__(self, other: _t.Union[Expansion, _Number]) -> bool:
         ...
 
     @_t.overload
     def __ge__(self, other: _t.Any) -> _t.Any:
         ...
 
     def __ge__(self,
                other: _t.Union[Expansion, _Number]) -> _t.Union[_t.Any, bool]:
-        return (not _are_components_lesser_than(self._components,
-                                                other._components)
-                if isinstance(other, Expansion)
-                else
-                (not _are_components_lesser_than_float(self._components,
-                                                       other)
-                 if isinstance(other, float)
-                 else
-                 (not _are_components_lesser_than_int(self._components,
-                                                      other)
-                  if isinstance(other, int)
-                  else
-                  (not _are_components_lesser_than_rational(
-                          self._components, other)
-                   if isinstance(other, _Rational)
-                   else NotImplemented))))
+        return (
+            not _are_components_lesser_than(self._components,
+                                            other._components)
+            if isinstance(other, Expansion)
+            else
+            (not _are_components_lesser_than_float(self._components, other)
+             if isinstance(other, float)
+             else
+             (not _are_components_lesser_than_int(self._components, other)
+              if isinstance(other, int)
+              else
+              (not _are_components_lesser_than_rational(self._components,
+                                                        other)
+               if isinstance(other, _Rational)
+               else NotImplemented)))
+        )
 
     @_t.overload
     def __gt__(self, other: _t.Union[Expansion, _Number]) -> bool:
         ...
 
     @_t.overload
     def __gt__(self, other: _t.Any) -> _t.Any:
@@ -472,16 +491,16 @@
 
 
 def _are_components_equal_to_float(components: _t.Sequence[float],
                                    value: float) -> bool:
     return len(components) == 1 and components[0] == value
 
 
-def _are_components_equal_to_int(components: _t.Sequence[float], value: int
-                                 ) -> bool:
+def _are_components_equal_to_int(components: _t.Sequence[float],
+                                 value: int) -> bool:
     return (_to_fraction(components[0]) == 0.
             and _components_to_integer(components) == value)
 
 
 def _are_components_equal_to_rational(components: _t.Sequence[float],
                                       value: _Rational) -> bool:
     return components == tuple(_rational_to_components(value))
```

### Comparing `shewchuk-6.6.0/shewchuk.egg-info/PKG-INFO` & `shewchuk-6.7.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,46 @@
 Metadata-Version: 2.1
 Name: shewchuk
-Version: 6.6.0
-Summary: Robust floating point operations.
+Version: 6.7.0
 Home-page: https://github.com/lycantropos/shewchuk/
 Download-URL: https://github.com/lycantropos/shewchuk/archive/master.zip
-Author: Azat Ibrakov
-Author-email: azatibrakov@gmail.com
+Author-email: Azat Ibrakov <azatibrakov@gmail.com>
 License: MIT License
+        
+        Copyright (c) 2021 Azat Ibrakov
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 License-File: LICENSE
 
 shewchuk
 ========
 
 [![](https://github.com/lycantropos/shewchuk/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/lycantropos/shewchuk/actions/workflows/ci.yml "Github Actions")
 [![](https://readthedocs.org/projects/shewchuk/badge/?version=latest)](https://shewchuk.readthedocs.io/en/latest/?badge=latest "Documentation")
```

### Comparing `shewchuk-6.6.0/src/shewchuk.c` & `shewchuk-6.7.0/src/shewchuk.c`

 * *Files 2% similar despite different names*

```diff
@@ -1941,14 +1941,136 @@
                                                  (ExpansionObject *)other)
 
                : Expansion_PyObject_multiply((ExpansionObject *)self, other);
   else
     return Expansion_PyObject_multiply((ExpansionObject *)other, self);
 }
 
+static int is_unit_Object(PyObject *self) {
+  PyObject *tmp = PyLong_FromLong(1);
+  int result = PyObject_RichCompareBool(self, tmp, Py_EQ);
+  Py_DECREF(tmp);
+  return result;
+}
+
+static int normalize_fraction_components(PyObject **result_numerator,
+                                         PyObject **result_denominator) {
+  PyObject *gcd = _PyLong_GCD(*result_numerator, *result_denominator);
+  if (!gcd) return -1;
+  int is_gcd_unit = is_unit_Object(gcd);
+  if (is_gcd_unit < 0) {
+    Py_DECREF(gcd);
+    return -1;
+  } else if (!is_gcd_unit) {
+    PyObject *numerator = PyNumber_FloorDivide(*result_numerator, gcd);
+    if (!numerator) {
+      Py_DECREF(gcd);
+      return -1;
+    }
+    PyObject *denominator = PyNumber_FloorDivide(*result_denominator, gcd);
+    if (!denominator) {
+      Py_DECREF(numerator);
+      Py_DECREF(gcd);
+      return -1;
+    }
+    PyObject *tmp = *result_numerator;
+    *result_numerator = numerator;
+    Py_DECREF(tmp);
+    tmp = *result_denominator;
+    *result_denominator = denominator;
+    Py_DECREF(tmp);
+  }
+  Py_DECREF(gcd);
+  return 0;
+}
+
+static int fractions_components_add(PyObject *numerator, PyObject *denominator,
+                                    PyObject *other_numerator,
+                                    PyObject *other_denominator,
+                                    PyObject **result_numerator,
+                                    PyObject **result_denominator) {
+  PyObject *first_result_numerator_component =
+      PyNumber_Multiply(numerator, other_denominator);
+  if (!first_result_numerator_component) return -1;
+  PyObject *second_result_numerator_component =
+      PyNumber_Multiply(other_numerator, denominator);
+  if (!second_result_numerator_component) {
+    Py_DECREF(first_result_numerator_component);
+    return -1;
+  }
+  *result_numerator = PyNumber_Add(first_result_numerator_component,
+                                   second_result_numerator_component);
+  Py_DECREF(second_result_numerator_component);
+  Py_DECREF(first_result_numerator_component);
+  if (*result_numerator == NULL) return -1;
+  *result_denominator = PyNumber_Multiply(denominator, other_denominator);
+  if (*result_denominator == NULL) {
+    Py_DECREF(*result_numerator);
+    return -1;
+  }
+  if (normalize_fraction_components(result_numerator, result_denominator)) {
+    Py_DECREF(*result_denominator);
+    Py_DECREF(*result_numerator);
+    return -1;
+  }
+  return 0;
+}
+
+static PyObject *double_as_integer_ratio(double value) {
+  PyObject *as_integer_ratio_method_name = PyUnicode_FromString("as_integer_ratio");
+  if (!as_integer_ratio_method_name) return NULL;
+  PyObject *tmp = PyFloat_FromDouble(value);
+  PyObject* result =
+#if PY39_OR_MORE
+      PyObject_CallMethodNoArgs(tmp, as_integer_ratio_method_name);
+#else
+      PyObject_CallMethodObjArgs(tmp, as_integer_ratio_method_name, NULL)
+#endif
+  ;
+  Py_DECREF(tmp);
+  return result;
+}
+
+static PyObject *Expansion_as_integer_ratio(ExpansionObject *self,
+                                            PyObject *Py_UNUSED(args)) {
+  PyObject *result = double_as_integer_ratio(self->components[0]);
+  if (self->size == 1 || result == NULL) {
+    return result;
+  }
+  PyObject *result_numerator = PyTuple_GET_ITEM(result, 0);
+  PyObject *result_denominator = PyTuple_GET_ITEM(result, 1);
+  Py_INCREF(result_numerator);
+  Py_INCREF(result_denominator);
+  Py_DECREF(result);
+  for (size_t index = 1; index < self->size; ++index) {
+    PyObject *step = double_as_integer_ratio(self->components[index]);
+    if (step == NULL) {
+      return NULL;
+    }
+    PyObject *step_numerator = PyTuple_GET_ITEM(step, 0);
+    PyObject *step_denominator = PyTuple_GET_ITEM(step, 1);
+    PyObject *next_result_numerator, *next_result_denominator;
+    if (fractions_components_add(result_numerator, result_denominator,
+                                 step_numerator, step_denominator,
+                                 &next_result_numerator,
+                                 &next_result_denominator) < 0) {
+      Py_DECREF(step);
+      Py_DECREF(result_denominator);
+      Py_DECREF(result_numerator);
+      return NULL;
+    }
+    Py_DECREF(step);
+    Py_DECREF(result_denominator);
+    Py_DECREF(result_numerator);
+    result_numerator = next_result_numerator;
+    result_denominator = next_result_denominator;
+  }
+  return PyTuple_Pack(2, result_numerator, result_denominator);
+}
+
 static PyObject *Expansion_new(PyTypeObject *cls, PyObject *args,
                                PyObject *kwargs) {
   if (!_PyArg_NoKeywords("Expansion", kwargs)) return NULL;
   double *components;
   Py_ssize_t raw_size = PyTuple_Size(args);
   if (raw_size < 0) return NULL;
   size_t size = (size_t)raw_size;
@@ -2645,14 +2767,15 @@
      "The real part of the expansion.", NULL},
     {"imag", (getter)Expansion_getimag, (setter)NULL,
      "The imaginary part of the expansion.", NULL},
     {NULL} /* Sentinel */
 };
 
 static PyMethodDef Expansion_methods[] = {
+    {"as_integer_ratio", (PyCFunction)Expansion_as_integer_ratio, METH_NOARGS, NULL},
     {"__ceil__", (PyCFunction)Expansion_ceil, METH_NOARGS, NULL},
     {"__floor__", (PyCFunction)Expansion_floor, METH_NOARGS, NULL},
     {"__getnewargs__", (PyCFunction)Expansion_getnewargs, METH_NOARGS, NULL},
     {"__round__", (PyCFunction)Expansion_round, METH_VARARGS, NULL},
     {"__trunc__", (PyCFunction)Expansion_trunc, METH_NOARGS, NULL},
     {NULL, NULL} /* sentinel */
 };
```

