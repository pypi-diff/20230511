# Comparing `tmp/encomp-0.9.0.tar.gz` & `tmp/encomp-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encomp-0.9.0.tar", max compression
+gzip compressed data, was "encomp-0.9.1.tar", max compression
```

## Comparing `encomp-0.9.0.tar` & `encomp-0.9.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1072 2023-04-25 07:41:03.603957 encomp-0.9.0/LICENSE
--rw-r--r--   0        0        0    10441 2023-04-25 07:41:03.603957 encomp-0.9.0/README.md
--rw-r--r--   0        0        0       78 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/__init__.py
--rw-r--r--   0        0        0      710 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/constants.py
--rw-r--r--   0        0        0     1895 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/context.py
--rw-r--r--   0        0        0     1976 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/conversion.py
--rw-r--r--   0        0        0     4453 2023-03-12 08:05:11.060958 encomp-0.9.0/encomp/defs/constants.txt
--rw-r--r--   0        0        0    31139 2023-03-12 08:05:11.060958 encomp-0.9.0/encomp/defs/units.txt
--rw-r--r--   0        0        0    43604 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/fluids.py
--rw-r--r--   0        0        0    12415 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/gases.py
--rw-r--r--   0        0        0     7133 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/math.py
--rw-r--r--   0        0        0     5269 2023-04-25 08:07:46.797762 encomp-0.9.0/encomp/misc.py
--rw-r--r--   0        0        0        0 2023-03-12 08:05:11.060958 encomp-0.9.0/encomp/py.typed
--rw-r--r--   0        0        0    14354 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/serialize.py
--rw-r--r--   0        0        0      416 2023-04-25 07:32:25.073969 encomp-0.9.0/encomp/session.py
--rw-r--r--   0        0        0     2645 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/settings.py
--rw-r--r--   0        0        0     2882 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/structures.py
--rw-r--r--   0        0        0    23410 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/sympy.py
--rw-r--r--   0        0        0        0 2023-03-12 08:05:11.060958 encomp-0.9.0/encomp/tests/__init__.py
--rw-r--r--   0        0        0      197 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_constants.py
--rw-r--r--   0        0        0      904 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_context.py
--rw-r--r--   0        0        0      934 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_conversion.py
--rw-r--r--   0        0        0     9983 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_fluids.py
--rw-r--r--   0        0        0     3065 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_fluids_types.py
--rw-r--r--   0        0        0     2542 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_function_signatures.py
--rw-r--r--   0        0        0     1103 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_gases.py
--rw-r--r--   0        0        0      189 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_math.py
--rw-r--r--   0        0        0     2066 2023-04-25 08:08:32.357986 encomp-0.9.0/encomp/tests/test_misc.py
--rw-r--r--   0        0        0      155 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_pandas.py
--rw-r--r--   0        0        0      580 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_polars.py
--rw-r--r--   0        0        0     5478 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_quantity_combined.py
--rw-r--r--   0        0        0     1243 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_quantity_guard.py
--rw-r--r--   0        0        0     5200 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_quantity_inferred.py
--rw-r--r--   0        0        0      649 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_quantity_magnitude.py
--rw-r--r--   0        0        0    23222 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_quantity_types.py
--rw-r--r--   0        0        0     3453 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_serialize.py
--rw-r--r--   0        0        0      124 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_settings.py
--rw-r--r--   0        0        0     1768 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_structures.py
--rw-r--r--   0        0        0     1812 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_sympy.py
--rw-r--r--   0        0        0      929 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/tests/test_thermo.py
--rw-r--r--   0        0        0    36066 2023-04-25 08:10:27.594534 encomp-0.9.0/encomp/tests/test_units.py
--rw-r--r--   0        0        0     6402 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/thermo.py
--rw-r--r--   0        0        0    37618 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/units.py
--rw-r--r--   0        0        0    79871 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/units.pyi
--rw-r--r--   0        0        0    21236 2023-04-25 07:41:03.603957 encomp-0.9.0/encomp/utypes.py
--rw-r--r--   0        0        0     2883 2023-04-25 07:57:36.611552 encomp-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    11630 1970-01-01 00:00:00.000000 encomp-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-25 07:41:03.603957 encomp-0.9.1/LICENSE
+-rw-r--r--   0        0        0    10441 2023-04-25 07:41:03.603957 encomp-0.9.1/README.md
+-rw-r--r--   0        0        0       78 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/__init__.py
+-rw-r--r--   0        0        0      710 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/constants.py
+-rw-r--r--   0        0        0     1895 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/context.py
+-rw-r--r--   0        0        0     1976 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/conversion.py
+-rw-r--r--   0        0        0     4453 2023-03-12 08:05:11.060958 encomp-0.9.1/encomp/defs/constants.txt
+-rw-r--r--   0        0        0    31139 2023-03-12 08:05:11.060958 encomp-0.9.1/encomp/defs/units.txt
+-rw-r--r--   0        0        0    47991 2023-05-11 11:28:38.816542 encomp-0.9.1/encomp/fluids.py
+-rw-r--r--   0        0        0    12415 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/gases.py
+-rw-r--r--   0        0        0     7133 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/math.py
+-rw-r--r--   0        0        0     5269 2023-04-25 08:07:46.797762 encomp-0.9.1/encomp/misc.py
+-rw-r--r--   0        0        0        0 2023-03-12 08:05:11.060958 encomp-0.9.1/encomp/py.typed
+-rw-r--r--   0        0        0    14354 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/serialize.py
+-rw-r--r--   0        0        0      416 2023-04-25 07:32:25.073969 encomp-0.9.1/encomp/session.py
+-rw-r--r--   0        0        0     2645 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/settings.py
+-rw-r--r--   0        0        0     2882 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/structures.py
+-rw-r--r--   0        0        0    23410 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/sympy.py
+-rw-r--r--   0        0        0        0 2023-03-12 08:05:11.060958 encomp-0.9.1/encomp/tests/__init__.py
+-rw-r--r--   0        0        0      197 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/tests/test_constants.py
+-rw-r--r--   0        0        0      904 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/tests/test_context.py
+-rw-r--r--   0        0        0      934 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/tests/test_conversion.py
+-rw-r--r--   0        0        0    10665 2023-05-11 11:33:23.989583 encomp-0.9.1/encomp/tests/test_fluids.py
+-rw-r--r--   0        0        0     3065 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/tests/test_fluids_types.py
+-rw-r--r--   0        0        0     2542 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/tests/test_function_signatures.py
+-rw-r--r--   0        0        0     1103 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/tests/test_gases.py
+-rw-r--r--   0        0        0      189 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/tests/test_math.py
+-rw-r--r--   0        0        0     2066 2023-04-25 08:08:32.357986 encomp-0.9.1/encomp/tests/test_misc.py
+-rw-r--r--   0        0        0     1544 2023-05-11 10:09:11.799816 encomp-0.9.1/encomp/tests/test_pandas.py
+-rw-r--r--   0        0        0      777 2023-05-11 10:07:40.203132 encomp-0.9.1/encomp/tests/test_polars.py
+-rw-r--r--   0        0        0     5478 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/tests/test_quantity_combined.py
+-rw-r--r--   0        0        0     1243 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/tests/test_quantity_guard.py
+-rw-r--r--   0        0        0     5200 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/tests/test_quantity_inferred.py
+-rw-r--r--   0        0        0      649 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/tests/test_quantity_magnitude.py
+-rw-r--r--   0        0        0    23222 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/tests/test_quantity_types.py
+-rw-r--r--   0        0        0     3453 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/tests/test_serialize.py
+-rw-r--r--   0        0        0      124 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/tests/test_settings.py
+-rw-r--r--   0        0        0     1768 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/tests/test_structures.py
+-rw-r--r--   0        0        0     1812 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/tests/test_sympy.py
+-rw-r--r--   0        0        0      929 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/tests/test_thermo.py
+-rw-r--r--   0        0        0    36408 2023-05-11 11:02:54.448948 encomp-0.9.1/encomp/tests/test_units.py
+-rw-r--r--   0        0        0     6402 2023-04-25 07:41:03.603957 encomp-0.9.1/encomp/thermo.py
+-rw-r--r--   0        0        0    42107 2023-05-11 11:29:44.888790 encomp-0.9.1/encomp/units.py
+-rw-r--r--   0        0        0    79885 2023-05-11 11:09:23.050144 encomp-0.9.1/encomp/units.pyi
+-rw-r--r--   0        0        0    21664 2023-05-11 10:41:15.866326 encomp-0.9.1/encomp/utypes.py
+-rw-r--r--   0        0        0     2973 2023-05-11 10:21:30.435484 encomp-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    11685 1970-01-01 00:00:00.000000 encomp-0.9.1/PKG-INFO
```

### Comparing `encomp-0.9.0/LICENSE` & `encomp-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/README.md` & `encomp-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/constants.py` & `encomp-0.9.1/encomp/constants.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/context.py` & `encomp-0.9.1/encomp/context.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/conversion.py` & `encomp-0.9.1/encomp/conversion.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/defs/constants.txt` & `encomp-0.9.1/encomp/defs/constants.txt`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/defs/units.txt` & `encomp-0.9.1/encomp/defs/units.txt`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/fluids.py` & `encomp-0.9.1/encomp/fluids.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,42 +7,29 @@
     which is also included when installing ``encomp``.
     Avoid importing as a standalone module (``from encomp import fluids``) to differentiate between these.
 
 """
 
 import warnings
 from abc import ABC, abstractmethod
-from typing import Annotated, Callable
+from typing import Annotated, Any, Callable, Generic
 
 import numpy as np
+import pandas as pd
+import polars as pl
 
-try:
-    from CoolProp.CoolProp import PropsSI
-    from CoolProp.HumidAirProp import HAPropsSI
-
-except ImportError:
-    warnings.warn(
-        "CoolProp package not installed, install with"
-        "\npip install coolprop\n"
-        "or"
-        "\nconda install conda-forge::coolprop"
-    )
-
-    def PropsSI(*args, **kwargs):
-        raise NotImplementedError()
-
-    def HAPropsSI(*args, **kwargs):
-        raise NotImplementedError()
-
+from CoolProp.CoolProp import PropsSI
+from CoolProp.HumidAirProp import HAPropsSI
 
 from .misc import isinstance_types
 from .settings import SETTINGS
 from .structures import flatten
 from .units import DimensionalityError, ExpectedDimensionalityError, Quantity, Unit
 from .utypes import (
+    MT,
     Density,
     Dimensionless,
     DynamicViscosity,
     MixtureEnthalpyPerDryAir,
     MixtureEnthalpyPerHumidAir,
     MixtureEntropyPerDryAir,
     MixtureEntropyPerHumidAir,
@@ -58,33 +45,33 @@
     SpecificEntropy,
     SpecificHeatCapacity,
     SpecificHeatPerDryAir,
     SpecificHeatPerHumidAir,
     SpecificInternalEnergy,
     Temperature,
     ThermalConductivity,
+    Variable,
     Velocity,
 )
 
 if SETTINGS.ignore_coolprop_warnings:
     warnings.filterwarnings("ignore", message="CoolProp could not calculate")
 
 
 CProperty = Annotated[str, "CoolProp property name"]
 CName = Annotated[str, "CoolProp fluid name"]
 UnitString = Annotated[str, "Unit string"]
 
-# TODO: the type hints for the Quantity magnitude is incorrectly set to
-# np.ndarray, it could be float also if all inputs are scalar
-# might be best to change this API to always use np.ndarray for the outputs
+# NOTE: the generic magnitude type MT is not correct if the inputs
+# are not heterogenous (e.g. mixed np.ndarray and scalar inputs)
 
 
-class CoolPropFluid(ABC):
+class CoolPropFluid(ABC, Generic[MT]):
     name: CName
-    points: list[tuple[CProperty, Quantity]]
+    points: list[tuple[CProperty, Quantity[Variable, MT]]]
 
     BACKEND: Callable = PropsSI
 
     # PropsSI expects the fluid name as the first input, but not HAPropsSI
     _append_name_to_cp_inputs: bool = True
 
     # HAPropsSI fails if one or more inputs are incorrect,
@@ -270,16 +257,33 @@
 
     # numerical accuracy, determines if return values are zero
     _EPS: float = 1e-9
 
     # skip checking for zero for these properties
     _SKIP_ZERO_CHECK: tuple[CProperty, ...] = ("PHASE",)
 
+    @property
+    def _mt(self) -> type[MT]:
+        return type(self.points[0][1].m)
+
+    @property
+    def _mt_kwargs(self) -> dict[str, Any]:
+        kwargs = {}
+
+        m0 = self.points[0][1].m
+
+        if isinstance(m0, pd.Series):
+            # NOTE: the series name should not be propagated here,
+            # the outputs will be separate series that should not have the same name
+            kwargs |= {"index": m0.index}
+
+        return kwargs
+
     @abstractmethod
-    def __init__(self, name: CName, **kwargs: Quantity):
+    def __init__(self, name: CName, **kwargs: Quantity[Variable, MT]):
         """
         Base class that represents a fluid (pure or mixture, gas or liquid).
         Uses *CoolProp* as backend to determine fluid properties.
 
         This class should not be used directly, since it does not contain a fixed
         point to determine fluid properties (temperature, pressure, enthalpy, entropy, ...).
         Define a subclass of :py:class:`encomp.fluids.CoolPropFluid` that implements
@@ -529,15 +533,15 @@
     def evaluate(
         self, output: CProperty, *points: tuple[CProperty, float | np.ndarray]
     ) -> float | np.ndarray:
         # case 1: all inputs are scalar, output is scalar
         if all(isinstance_types(pt[1], float) for pt in points):
             return self.evaluate_single(output, *points)  # type: ignore
 
-        # at this point, the output will be a vector of at least length 1
+        # at this point, the output will be a vector with length 1 or more
 
         def single_element_vector_to_float(x: float | np.ndarray) -> float | np.ndarray:
             if isinstance(x, float):
                 return x
 
             if isinstance(x, np.ndarray) and x.size == 1:
                 return float(x[0])
@@ -712,41 +716,54 @@
 
         if len(key) > 0 and key[0] in self.RETURN_UNITS:
             ret_unit = self.RETURN_UNITS[key[0]]
             qty.ito(ret_unit)
 
         return qty
 
-    def to_numeric(self, prop: CProperty, qty: Quantity) -> float | np.ndarray:
+    def to_numeric(
+        self, prop: CProperty, qty: Quantity[Variable, MT]
+    ) -> float | np.ndarray:
         unit = self.get_coolprop_unit(prop)
 
         try:
             m = qty.to(unit).m
         except DimensionalityError:
             raise ExpectedDimensionalityError(
                 f'CoolProp input for property "{prop}" is incorrect. '
                 f"expected {unit} ({unit.dimensionality}), but passed "
                 f"{qty.u} ({qty.dimensionality})"
             )
 
+        if isinstance(m, (pd.DatetimeIndex, pd.Timestamp)):
+            raise TypeError(f"Cannot pass datetime magnitude as input to CoolProp: {m}")
+
+        if isinstance(m, pl.Expr):
+            raise TypeError(f"Cannot pass Polars expression as input to CoolProp: {m}")
+
         if isinstance(m, list):
             m = np.array(m)
 
+        if isinstance(m, (pd.Series, pl.Series)):
+            m = m.to_numpy()
+
         return m
 
-    def get(self, output: CProperty, *points: tuple[CProperty, Quantity]) -> Quantity:
+    def get(
+        self, output: CProperty, *points: tuple[CProperty, Quantity[Variable, MT]]
+    ) -> Quantity:
         """
         Wraps the function ``CoolProp.CoolProp.PropsSI``, handles input
         and output with :py:class:`encomp.units.Quantity` objects.
 
         Parameters
         ----------
         output : CProperty
             Name of the output property
-        points : tuple[CProperty, Quantity]
+        points : tuple[CProperty, Quantity[Variable, MT]]
             Fixed state variables: name and value of the property.
             The number of points must match the number expected
             by the CoolProp backend function.
 
         Returns
         -------
         Quantity
@@ -756,25 +773,25 @@
         points_numeric = [(pt[0], self.to_numeric(*pt)) for pt in points]
 
         val = self.evaluate(output, *points_numeric)
 
         return self.construct_quantity(val, output)
 
 
-class Fluid(CoolPropFluid):
-    def __init__(self, name: CName, **kwargs: Quantity):
+class Fluid(CoolPropFluid[MT]):
+    def __init__(self, name: CName, **kwargs: Quantity[Variable, MT]):
         """
         Represents a fluid at a fixed state, for example at a
         specific temperature and pressure.
 
         Parameters
         ----------
         name : CName
             Name of the fluid
-        kwargs: Quantity
+        kwargs: Quantity[Variable, MT]
             Values for the two fixed points. The name of the keyword argument is the
             CoolProp property name.
         """
 
         self.name = name
 
         self.check_inputs(kwargs)
@@ -806,148 +823,264 @@
 
         elif isinstance(phase_idx_val, (int, float)):
             return self.PHASES.get(float(phase_idx_val), "N/A")
 
         raise TypeError(f"Cannot determine phase of {self} when " f"{phase_idx=}")
 
     @property
-    def PHASE(self) -> Quantity[Dimensionless, np.ndarray]:
-        return self.__getattr__("PHASE").asdim(Dimensionless)
+    def PHASE(self) -> Quantity[Dimensionless, MT]:
+        return (
+            self.__getattr__("PHASE")
+            .asdim(Dimensionless)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def PRANDTL(self) -> Quantity[Dimensionless, np.ndarray]:
-        return self.__getattr__("PRANDTL").asdim(Dimensionless)
+    def PRANDTL(self) -> Quantity[Dimensionless, MT]:
+        return (
+            self.__getattr__("PRANDTL")
+            .asdim(Dimensionless)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def P(self) -> Quantity[Pressure, np.ndarray]:
-        return self.__getattr__("P").asdim(Pressure)
+    def P(self) -> Quantity[Pressure, MT]:
+        return self.__getattr__("P").asdim(Pressure).astype(self._mt, **self._mt_kwargs)
 
     @property
-    def PCRIT(self) -> Quantity[Pressure, np.ndarray]:
-        return self.__getattr__("PCRIT").asdim(Pressure)
+    def PCRIT(self) -> Quantity[Pressure, MT]:
+        return (
+            self.__getattr__("PCRIT")
+            .asdim(Pressure)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def PMAX(self) -> Quantity[Pressure, np.ndarray]:
-        return self.__getattr__("PMAX").asdim(Pressure)
+    def PMAX(self) -> Quantity[Pressure, MT]:
+        return (
+            self.__getattr__("PMAX").asdim(Pressure).astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def PMIN(self) -> Quantity[Pressure, np.ndarray]:
-        return self.__getattr__("PMIN").asdim(Pressure)
+    def PMIN(self) -> Quantity[Pressure, MT]:
+        return (
+            self.__getattr__("PMIN").asdim(Pressure).astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def PTRIPLE(self) -> Quantity[Pressure, np.ndarray]:
-        return self.__getattr__("PTRIPLE").asdim(Pressure)
+    def PTRIPLE(self) -> Quantity[Pressure, MT]:
+        return (
+            self.__getattr__("PTRIPLE")
+            .asdim(Pressure)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def P_REDUCING(self) -> Quantity[Pressure, np.ndarray]:
-        return self.__getattr__("P_REDUCING").asdim(Pressure)
+    def P_REDUCING(self) -> Quantity[Pressure, MT]:
+        return (
+            self.__getattr__("P_REDUCING")
+            .asdim(Pressure)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def T(self) -> Quantity[Temperature, np.ndarray]:
-        return self.__getattr__("T").asdim(Temperature)
+    def T(self) -> Quantity[Temperature, MT]:
+        return (
+            self.__getattr__("T").asdim(Temperature).astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def TCRIT(self) -> Quantity[Temperature, np.ndarray]:
-        return self.__getattr__("TCRIT").asdim(Temperature)
+    def TCRIT(self) -> Quantity[Temperature, MT]:
+        return (
+            self.__getattr__("TCRIT")
+            .asdim(Temperature)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def TMAX(self) -> Quantity[Temperature, np.ndarray]:
-        return self.__getattr__("TMAX").asdim(Temperature)
+    def TMAX(self) -> Quantity[Temperature, MT]:
+        return (
+            self.__getattr__("TMAX")
+            .asdim(Temperature)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def TMIN(self) -> Quantity[Temperature, np.ndarray]:
-        return self.__getattr__("TMIN").asdim(Temperature)
+    def TMIN(self) -> Quantity[Temperature, MT]:
+        return (
+            self.__getattr__("TMIN")
+            .asdim(Temperature)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def TTRIPLE(self) -> Quantity[Temperature, np.ndarray]:
-        return self.__getattr__("TTRIPLE").asdim(Temperature)
+    def TTRIPLE(self) -> Quantity[Temperature, MT]:
+        return (
+            self.__getattr__("TTRIPLE")
+            .asdim(Temperature)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def T_FREEZING(self) -> Quantity[Temperature, np.ndarray]:
-        return self.__getattr__("T_FREEZING").asdim(Temperature)
+    def T_FREEZING(self) -> Quantity[Temperature, MT]:
+        return (
+            self.__getattr__("T_FREEZING")
+            .asdim(Temperature)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def T_REDUCING(self) -> Quantity[Temperature, np.ndarray]:
-        return self.__getattr__("T_REDUCING").asdim(Temperature)
+    def T_REDUCING(self) -> Quantity[Temperature, MT]:
+        return (
+            self.__getattr__("T_REDUCING")
+            .asdim(Temperature)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def Q(self) -> Quantity[Dimensionless, np.ndarray]:
-        return self.__getattr__("Q").asdim(Dimensionless)
+    def Q(self) -> Quantity[Dimensionless, MT]:
+        return (
+            self.__getattr__("Q")
+            .asdim(Dimensionless)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def H(self) -> Quantity[SpecificEnthalpy, np.ndarray]:
-        return self.__getattr__("H").asdim(SpecificEnthalpy)
+    def H(self) -> Quantity[SpecificEnthalpy, MT]:
+        return (
+            self.__getattr__("H")
+            .asdim(SpecificEnthalpy)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def HMOLAR(self) -> Quantity[MolarSpecificEnthalpy, np.ndarray]:
-        return self.__getattr__("HMOLAR").asdim(MolarSpecificEnthalpy)
+    def HMOLAR(self) -> Quantity[MolarSpecificEnthalpy, MT]:
+        return (
+            self.__getattr__("HMOLAR")
+            .asdim(MolarSpecificEnthalpy)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def S(self) -> Quantity[SpecificEntropy, np.ndarray]:
-        return self.__getattr__("S").asdim(SpecificEntropy)
+    def S(self) -> Quantity[SpecificEntropy, MT]:
+        return (
+            self.__getattr__("S")
+            .asdim(SpecificEntropy)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def SMOLAR(self) -> Quantity[MolarSpecificEntropy, np.ndarray]:
-        return self.__getattr__("SMOLAR").asdim(MolarSpecificEntropy)
+    def SMOLAR(self) -> Quantity[MolarSpecificEntropy, MT]:
+        return (
+            self.__getattr__("SMOLAR")
+            .asdim(MolarSpecificEntropy)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def U(self) -> Quantity[SpecificInternalEnergy, np.ndarray]:
-        return self.__getattr__("U").asdim(SpecificInternalEnergy)
+    def U(self) -> Quantity[SpecificInternalEnergy, MT]:
+        return (
+            self.__getattr__("U")
+            .asdim(SpecificInternalEnergy)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def UMOLAR(self) -> Quantity[MolarSpecificInternalEnergy, np.ndarray]:
-        return self.__getattr__("UMOLAR").asdim(MolarSpecificInternalEnergy)
+    def UMOLAR(self) -> Quantity[MolarSpecificInternalEnergy, MT]:
+        return (
+            self.__getattr__("UMOLAR")
+            .asdim(MolarSpecificInternalEnergy)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def V(self) -> Quantity[DynamicViscosity, np.ndarray]:
-        return self.__getattr__("V").asdim(DynamicViscosity)
+    def V(self) -> Quantity[DynamicViscosity, MT]:
+        return (
+            self.__getattr__("V")
+            .asdim(DynamicViscosity)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def Z(self) -> Quantity[Dimensionless, np.ndarray]:
-        return self.__getattr__("Z").asdim(Dimensionless)
+    def Z(self) -> Quantity[Dimensionless, MT]:
+        return (
+            self.__getattr__("Z")
+            .asdim(Dimensionless)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def DELTA(self) -> Quantity[Dimensionless, np.ndarray]:
-        return self.__getattr__("DELTA").asdim(Dimensionless)
+    def DELTA(self) -> Quantity[Dimensionless, MT]:
+        return (
+            self.__getattr__("DELTA")
+            .asdim(Dimensionless)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def D(self) -> Quantity[Density, np.ndarray]:
-        return self.__getattr__("D").asdim(Density)
+    def D(self) -> Quantity[Density, MT]:
+        return self.__getattr__("D").asdim(Density).astype(self._mt, **self._mt_kwargs)
 
     @property
-    def RHOMASS_REDUCING(self) -> Quantity[Density, np.ndarray]:
-        return self.__getattr__("RHOMASS_REDUCING").asdim(Density)
+    def RHOMASS_REDUCING(self) -> Quantity[Density, MT]:
+        return (
+            self.__getattr__("RHOMASS_REDUCING")
+            .asdim(Density)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def RHOMOLAR_CRITICAL(self) -> Quantity[MolarDensity, np.ndarray]:
-        return self.__getattr__("RHOMOLAR_CRITICAL").asdim(MolarDensity)
+    def RHOMOLAR_CRITICAL(self) -> Quantity[MolarDensity, MT]:
+        return (
+            self.__getattr__("RHOMOLAR_CRITICAL")
+            .asdim(MolarDensity)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def RHOMOLAR_REDUCING(self) -> Quantity[MolarDensity, np.ndarray]:
-        return self.__getattr__("RHOMOLAR_REDUCING").asdim(MolarDensity)
+    def RHOMOLAR_REDUCING(self) -> Quantity[MolarDensity, MT]:
+        return (
+            self.__getattr__("RHOMOLAR_REDUCING")
+            .asdim(MolarDensity)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def DMOLAR(self) -> Quantity[MolarDensity, np.ndarray]:
-        return self.__getattr__("DMOLAR").asdim(MolarDensity)
+    def DMOLAR(self) -> Quantity[MolarDensity, MT]:
+        return (
+            self.__getattr__("DMOLAR")
+            .asdim(MolarDensity)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def A(self) -> Quantity[Velocity, np.ndarray]:
-        return self.__getattr__("A").asdim(Velocity)
+    def A(self) -> Quantity[Velocity, MT]:
+        return self.__getattr__("A").asdim(Velocity).astype(self._mt, **self._mt_kwargs)
 
     @property
-    def L(self) -> Quantity[ThermalConductivity, np.ndarray]:
-        return self.__getattr__("L").asdim(ThermalConductivity)
+    def L(self) -> Quantity[ThermalConductivity, MT]:
+        return (
+            self.__getattr__("L")
+            .asdim(ThermalConductivity)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def C(self) -> Quantity[SpecificHeatCapacity, np.ndarray]:
-        return self.__getattr__("C").asdim(SpecificHeatCapacity)
+    def C(self) -> Quantity[SpecificHeatCapacity, MT]:
+        return (
+            self.__getattr__("C")
+            .asdim(SpecificHeatCapacity)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def M(self) -> Quantity[MolarMass, np.ndarray]:
-        return self.__getattr__("M").asdim(MolarMass)
+    def M(self) -> Quantity[MolarMass, MT]:
+        return (
+            self.__getattr__("M").asdim(MolarMass).astype(self._mt, **self._mt_kwargs)
+        )
 
     def __getattr__(self, attr: CProperty) -> Quantity:
         if attr not in self.ALL_PROPERTIES:
             raise AttributeError(attr)
 
         return super().get(attr, *self.points)
 
@@ -960,29 +1093,29 @@
         props_str = ", ".join(props)
 
         s = f'<{self.__class__.__name__} "{self.name}", {props_str}>'
 
         return s
 
 
-class Water(Fluid):
+class Water(Fluid[MT]):
     REPR_PROPERTIES: tuple[tuple[str, str], ...] = (
         ("P", ".0f"),
         ("T", ".1f"),
         ("D", ".1f"),
         ("V", ".1f"),
     )
 
-    def __init__(self, **kwargs: Quantity):
+    def __init__(self, **kwargs: Quantity[Variable, MT]):
         """
         Convenience class to access water and steam properties via CoolProp.
 
         Parameters
         ----------
-        kwargs: Quantity
+        kwargs: Quantity[Variable, MT]
             Values for the two fixed points. The name of the keyword argument is the
             CoolProp property name.
         """
 
         self.name = "Water"
 
         self.check_inputs(kwargs)
@@ -1013,15 +1146,15 @@
         )
 
         s = f"<{self.__class__.__name__} ({self.phase}), {props_str}>"
 
         return s
 
 
-class HumidAir(CoolPropFluid):
+class HumidAir(CoolPropFluid[MT]):
     BACKEND = HAPropsSI
     _append_name_to_cp_inputs = False
     _evaluate_invalid_separately = True
 
     # unit and description for properties in function HAPropsSI
     PROPERTY_MAP: dict[tuple[CProperty, ...], tuple[str, str]] = {
         ("B", "Twb", "T_wb", "WetBulb"): ("K", "Wet-Bulb Temperature"),
@@ -1075,22 +1208,22 @@
         ("T", ".1f"),
         ("R", ".2f"),
         ("Vda", ".1f"),
         ("Vha", ".1f"),
         ("M", ".2g"),
     )
 
-    def __init__(self, **kwargs: Quantity):
+    def __init__(self, **kwargs: Quantity[Variable, MT]):
         """
         Interface to the CoolProp function for humid air, ``CoolProp.CoolProp.HAPropsSI``.
         Needs three fixed points instead of two.
 
         Parameters
         ----------
-        kwargs: Quantity
+        kwargs: Quantity[Variable, MT]
             Values for the three fixed points. The name of the keyword argument is the
             CoolProp property name.
         """
 
         self.name = "Humid air"
 
         self.check_inputs(kwargs)
@@ -1105,88 +1238,152 @@
         self.point_1 = kwargs_list[0]
         self.point_2 = kwargs_list[1]
         self.point_3 = kwargs_list[2]
 
         self.points = [self.point_1, self.point_2, self.point_3]
 
     @property
-    def psi_w(self) -> Quantity[Dimensionless, np.ndarray]:
-        return self.__getattr__("psi_w").asdim(Dimensionless)
+    def psi_w(self) -> Quantity[Dimensionless, MT]:
+        return (
+            self.__getattr__("psi_w")
+            .asdim(Dimensionless)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def W(self) -> Quantity[Dimensionless, np.ndarray]:
-        return self.__getattr__("W").asdim(Dimensionless)
+    def W(self) -> Quantity[Dimensionless, MT]:
+        return (
+            self.__getattr__("W")
+            .asdim(Dimensionless)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def Z(self) -> Quantity[Dimensionless, np.ndarray]:
-        return self.__getattr__("Z").asdim(Dimensionless)
+    def Z(self) -> Quantity[Dimensionless, MT]:
+        return (
+            self.__getattr__("Z")
+            .asdim(Dimensionless)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def R(self) -> Quantity[Dimensionless, np.ndarray]:
-        return self.__getattr__("R").asdim(Dimensionless)
+    def R(self) -> Quantity[Dimensionless, MT]:
+        return (
+            self.__getattr__("R")
+            .asdim(Dimensionless)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def P(self) -> Quantity[Pressure, np.ndarray]:
-        return self.__getattr__("P").asdim(Pressure)
+    def P(self) -> Quantity[Pressure, MT]:
+        return self.__getattr__("P").asdim(Pressure).astype(self._mt, **self._mt_kwargs)
 
     @property
-    def P_w(self) -> Quantity[Pressure, np.ndarray]:
-        return self.__getattr__("P_w").asdim(Pressure)
+    def P_w(self) -> Quantity[Pressure, MT]:
+        return (
+            self.__getattr__("P_w").asdim(Pressure).astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def B(self) -> Quantity[Temperature, np.ndarray]:
-        return self.__getattr__("B").asdim(Temperature)
+    def B(self) -> Quantity[Temperature, MT]:
+        return (
+            self.__getattr__("B").asdim(Temperature).astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def T(self) -> Quantity[Temperature, np.ndarray]:
-        return self.__getattr__("T").asdim(Temperature)
+    def T(self) -> Quantity[Temperature, MT]:
+        return (
+            self.__getattr__("T").asdim(Temperature).astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def D(self) -> Quantity[Temperature, np.ndarray]:
-        return self.__getattr__("D").asdim(Temperature)
+    def D(self) -> Quantity[Temperature, MT]:
+        return (
+            self.__getattr__("D").asdim(Temperature).astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def K(self) -> Quantity[ThermalConductivity, np.ndarray]:
-        return self.__getattr__("K").asdim(ThermalConductivity)
+    def K(self) -> Quantity[ThermalConductivity, MT]:
+        return (
+            self.__getattr__("K")
+            .asdim(ThermalConductivity)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def M(self) -> Quantity[DynamicViscosity, np.ndarray]:
-        return self.__getattr__("M").asdim(DynamicViscosity)
+    def M(self) -> Quantity[DynamicViscosity, MT]:
+        return (
+            self.__getattr__("M")
+            .asdim(DynamicViscosity)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def C(self) -> Quantity[SpecificHeatPerDryAir, np.ndarray]:
-        return self.__getattr__("C").asdim(SpecificHeatPerDryAir)
+    def C(self) -> Quantity[SpecificHeatPerDryAir, MT]:
+        return (
+            self.__getattr__("C")
+            .asdim(SpecificHeatPerDryAir)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def Cha(self) -> Quantity[SpecificHeatPerHumidAir, np.ndarray]:
-        return self.__getattr__("Cha").asdim(SpecificHeatPerHumidAir)
+    def Cha(self) -> Quantity[SpecificHeatPerHumidAir, MT]:
+        return (
+            self.__getattr__("Cha")
+            .asdim(SpecificHeatPerHumidAir)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def H(self) -> Quantity[MixtureEnthalpyPerDryAir, np.ndarray]:
-        return self.__getattr__("H").asdim(MixtureEnthalpyPerDryAir)
+    def H(self) -> Quantity[MixtureEnthalpyPerDryAir, MT]:
+        return (
+            self.__getattr__("H")
+            .asdim(MixtureEnthalpyPerDryAir)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def Hha(self) -> Quantity[MixtureEnthalpyPerHumidAir, np.ndarray]:
-        return self.__getattr__("Hha").asdim(MixtureEnthalpyPerHumidAir)
+    def Hha(self) -> Quantity[MixtureEnthalpyPerHumidAir, MT]:
+        return (
+            self.__getattr__("Hha")
+            .asdim(MixtureEnthalpyPerHumidAir)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def S(self) -> Quantity[MixtureEntropyPerDryAir, np.ndarray]:
-        return self.__getattr__("S").asdim(MixtureEntropyPerDryAir)
+    def S(self) -> Quantity[MixtureEntropyPerDryAir, MT]:
+        return (
+            self.__getattr__("S")
+            .asdim(MixtureEntropyPerDryAir)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def Sha(self) -> Quantity[MixtureEntropyPerHumidAir, np.ndarray]:
-        return self.__getattr__("Sha").asdim(MixtureEntropyPerHumidAir)
+    def Sha(self) -> Quantity[MixtureEntropyPerHumidAir, MT]:
+        return (
+            self.__getattr__("Sha")
+            .asdim(MixtureEntropyPerHumidAir)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def V(self) -> Quantity[MixtureVolumePerDryAir, np.ndarray]:
-        return self.__getattr__("V").asdim(MixtureVolumePerDryAir)
+    def V(self) -> Quantity[MixtureVolumePerDryAir, MT]:
+        return (
+            self.__getattr__("V")
+            .asdim(MixtureVolumePerDryAir)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     @property
-    def Vha(self) -> Quantity[MixtureVolumePerHumidAir, np.ndarray]:
-        return self.__getattr__("Vha").asdim(MixtureVolumePerHumidAir)
+    def Vha(self) -> Quantity[MixtureVolumePerHumidAir, MT]:
+        return (
+            self.__getattr__("Vha")
+            .asdim(MixtureVolumePerHumidAir)
+            .astype(self._mt, **self._mt_kwargs)
+        )
 
     def __getattr__(self, attr: CProperty) -> Quantity:
         if attr not in self.ALL_PROPERTIES:
             raise AttributeError(attr)
 
         # this is called in case attr does not exist
         return super().get(attr, *self.points)
```

### Comparing `encomp-0.9.0/encomp/gases.py` & `encomp-0.9.1/encomp/gases.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/math.py` & `encomp-0.9.1/encomp/math.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/misc.py` & `encomp-0.9.1/encomp/misc.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/serialize.py` & `encomp-0.9.1/encomp/serialize.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/settings.py` & `encomp-0.9.1/encomp/settings.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/structures.py` & `encomp-0.9.1/encomp/structures.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/sympy.py` & `encomp-0.9.1/encomp/sympy.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/tests/test_context.py` & `encomp-0.9.1/encomp/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/tests/test_conversion.py` & `encomp-0.9.1/encomp/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/tests/test_fluids.py` & `encomp-0.9.1/encomp/tests/test_fluids.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import pandas as pd
 import pytest
 
 from ..fluids import Fluid, HumidAir, Water
 from ..units import Quantity as Q
 from ..utypes import Density, SpecificEntropy
 
 
@@ -382,7 +383,28 @@
 
     for T, P, R in zip(Ts, Ps, Rs):
         ha = HumidAir(T=Q(T, "°C"), P=Q(P, "bar"), R=Q(R))
         repr(ha)
 
         for p in props:
             getattr(ha, p)
+
+
+def test_magnitude_type():
+    index = pd.DatetimeIndex(["2021-01-01", "2021-01-02", "2021-01-03"])
+
+    s1 = pd.Series([1, 2, 3], name="s1", index=index)
+
+    assert Water(P=Q(s1, "kPa"), T=Q(25, "degC")).H.m.index[0] == pd.Timestamp(
+        "2021-01-01"
+    )
+
+    assert Fluid("water", P=Q(s1, "kPa"), T=Q(25, "degC")).H.m.index[0] == pd.Timestamp(
+        "2021-01-01"
+    )
+
+    assert HumidAir(P=Q(s1, "kPa"), T=Q(25, "degC"), R=Q(0.5)).H.m.index[
+        0
+    ] == pd.Timestamp("2021-01-01")
+
+    # in case the input dtypes are mixed, np.ndarray will be used as a fallback
+    assert isinstance(Water(T=Q(25, "degC"), P=Q(s1, "kPa")).H.m, np.ndarray)
```

### Comparing `encomp-0.9.0/encomp/tests/test_fluids_types.py` & `encomp-0.9.1/encomp/tests/test_fluids_types.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/tests/test_function_signatures.py` & `encomp-0.9.1/encomp/tests/test_function_signatures.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/tests/test_gases.py` & `encomp-0.9.1/encomp/tests/test_gases.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/tests/test_misc.py` & `encomp-0.9.1/encomp/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/tests/test_quantity_combined.py` & `encomp-0.9.1/encomp/tests/test_quantity_combined.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/tests/test_quantity_guard.py` & `encomp-0.9.1/encomp/tests/test_quantity_guard.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/tests/test_quantity_inferred.py` & `encomp-0.9.1/encomp/tests/test_quantity_inferred.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/tests/test_quantity_magnitude.py` & `encomp-0.9.1/encomp/tests/test_quantity_magnitude.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/tests/test_quantity_types.py` & `encomp-0.9.1/encomp/tests/test_quantity_types.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/tests/test_serialize.py` & `encomp-0.9.1/encomp/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/tests/test_structures.py` & `encomp-0.9.1/encomp/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/tests/test_sympy.py` & `encomp-0.9.1/encomp/tests/test_sympy.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/tests/test_thermo.py` & `encomp-0.9.1/encomp/tests/test_thermo.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/tests/test_units.py` & `encomp-0.9.1/encomp/tests/test_units.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import copy
 from contextlib import contextmanager
 from decimal import Decimal
 from typing import TypedDict
 
 import numpy as np
 import pandas as pd
+import polars as pl
 import pytest
 from pandas.api.types import is_list_like as pandas_is_list_like  # type: ignore
 from pint.errors import OffsetUnitCalculusError
 from pydantic import BaseModel
 from pydantic.error_wrappers import ValidationError
 from pytest import approx
 from typeguard import typechecked
@@ -26,14 +27,15 @@
     Unit,
     define_dimensionality,
     ureg,
 )
 from ..units import Quantity as Q
 from ..utypes import (
     DT,
+    DT_,
     Area,
     Dimensionality,
     Dimensionless,
     EnergyPerMass,
     Length,
     LowerHeatingValue,
     Mass,
@@ -44,14 +46,15 @@
     Pressure,
     SpecificEnthalpy,
     Temperature,
     TemperatureDifference,
     UnitsContainer,
     Unknown,
     Unset,
+    Variable,
     Velocity,
     Volume,
     VolumeFlow,
     get_registered_units,
 )
 
 
@@ -708,22 +711,19 @@
 
     with pytest.raises(TypeError):
         Q["string"]
 
     with pytest.raises(TypeError):
         Q[None]
 
-    # the Unknown and Unset dimensionalities cannot
-    # be resolved at runtime
-
-    with pytest.raises(TypeError):
-        Q[Unknown]
-
-    with pytest.raises(TypeError):
-        Q[Unset]
+    Q[Unknown]
+    Q[Unset]
+    Q[Variable]
+    Q[DT]
+    Q[DT_]
 
 
 def test_dynamic_dimensionalities():
     # this will create a new dimensionality type
     q1 = Q(1, "kg^2/K^4")
 
     # this will reuse the previously created one
@@ -1321,7 +1321,18 @@
     assert isinstance(m0, Q[Mass, float])
 
     ts = Q(pd.DatetimeIndex([pd.Timestamp.now(), pd.Timestamp.now()]))
     assert isinstance(ts, Q[Dimensionless, pd.DatetimeIndex])
 
     t0 = ts[0]
     assert isinstance(t0, Q[Dimensionless, pd.Timestamp])
+
+
+def test_astype():
+    assert isinstance(Q(25).astype(list[float]).m[0], float)
+
+    assert isinstance(Q([1, 2, 3]).astype(np.ndarray).m, np.ndarray)
+    assert isinstance(Q([1, 2, 3]).astype(pd.Series).m, pd.Series)
+    assert isinstance(Q([1, 2, 3]).astype(pl.Series).m, pl.Series)
+
+    assert Q([1, 2, 3]).astype(pd.Series, name="s1").m.name == "s1"
+    assert Q([1, 2, 3]).astype(pl.Series, name="s1").m.name == "s1"
```

### Comparing `encomp-0.9.0/encomp/thermo.py` & `encomp-0.9.1/encomp/thermo.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.0/encomp/units.py` & `encomp-0.9.1/encomp/units.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from __future__ import annotations
 
 import copy
 import numbers
 import re
 import warnings
-from typing import Any, Generic, Literal, TypeVar
+from typing import Any, ClassVar, Generic, Iterable, Literal, TypeVar
 
 import numpy as np
 import pandas as pd
 import pint
 import polars as pl
 import sympy as sp
 from pint.errors import DimensionalityError
@@ -35,14 +35,15 @@
 from .misc import isinstance_types
 from .settings import SETTINGS
 from .utypes import (
     _BASE_SI_UNITS,
     DT,
     DT_,
     MT,
+    MT_,
     Dimensionality,
     Temperature,
     TemperatureDifference,
     Unknown,
     Unset,
     Variable,
 )
@@ -221,39 +222,40 @@
     ``__mul__, __truediv__, __rtruediv__, __pow__`` methods.
 
     .. note::
         The overload signatures are defined in a separate file (``units.pyi``)
 
     """
 
-    _magnitude: MT
+    # constants
+    NORMAL_M3_VARIANTS = ("nm³", "Nm³", "nm3", "Nm3", "nm**3", "Nm**3", "nm^3", "Nm^3")
+    TEMPERATURE_DIFFERENCE_UCS = (Unit("delta_degC")._units, Unit("delta_degF")._units)
+    # compact, Latex, HTML, Latex/siunitx formatting
+    FORMATTING_SPECS = ("~P", "~L", "~H", "~Lx")
 
-    _REGISTRY: UnitRegistry = ureg  # type: ignore
+    # class attributes
+    _REGISTRY: ClassVar[UnitRegistry] = ureg
 
     # mapping from dimensionality subclass name to quantity subclass
     # this dict will be populated at runtime
     # use a custom class attribute (not cls.__subclasses__()) for more control
-    _subclasses: dict[tuple[str, str | None], type[Quantity]] = {}
+    _subclasses: ClassVar[dict[tuple[str, str | None], type[Quantity]]] = {}
+    _dimension_symbol_map: ClassVar[dict[sp.Basic, Unit]] = {}
 
     # used to validate dimensionality and magnitude type,
     # if None the dimensionality is not checked
     # subclasses of Quantity have this class attribute set, which
     # will restrict the dimensionality when creating the object
-    _dimensionality_type: type[Dimensionality] = Unset
-    _magnitude_type: type[MT]
-    _original_magnitude_type: type[MT] | None = None
-
-    _dimension_symbol_map: dict[sp.Basic, Unit] | None = None
-
-    # compact, Latex, HTML, Latex/siunitx formatting
-    FORMATTING_SPECS = ("~P", "~L", "~H", "~Lx")
-
-    NORMAL_M3_VARIANTS = ("nm³", "Nm³", "nm3", "Nm3", "nm**3", "Nm**3", "nm^3", "Nm^3")
+    _dimensionality_type: ClassVar[type[Dimensionality]] = Unset
 
-    TEMPERATURE_DIFFERENCE_UCS = (Unit("delta_degC")._units, Unit("delta_degF")._units)
+    # instance attributes
+    _magnitude: MT
+    _magnitude_type: type[MT]
+    _original_magnitude_type: type[MT]
+    _original_magnitude_kwargs: dict[str, Any]
 
     def __hash__(self) -> int:
         return super().__hash__()
 
     def __str__(self) -> str:
         return self.__format__(self._REGISTRY.default_format)
 
@@ -313,15 +315,21 @@
         # default magnitude type is np.ndarray, this is hard-coded in several places
 
         try:
             dim, mt = types
         except Exception:
             dim, mt = types, None
 
-        if isinstance(dim, TypeVar):
+        # avoid runtime errors when evaluating type hints
+        if (
+            isinstance(dim, TypeVar)
+            or dim is Unknown
+            or dim is Variable
+            or dim is Unset
+        ):
             return cls._get_dimensional_subclass(Variable, mt)
 
         if not isinstance(dim, type):
             raise TypeError(
                 "Generic type parameter to Quantity must be a type object, "
                 f"passed an instance of {type(dim)}: {dim}"
             )
@@ -345,14 +353,21 @@
 
         return subcls
 
     @staticmethod
     def _validate_unit(
         unit: Unit[DT_] | UnitsContainer | str | dict[str, numbers.Number] | None
     ) -> Unit[DT_]:
+        if isinstance(unit, Quantity):
+            raise TypeError(
+                f"Input unit has incorrect type Quantity: {unit}. "
+                "Do not create nested Quantity objects, convert "
+                "to separate magnitude and unit objects first."
+            )
+
         if unit is None:
             return Unit("dimensionless")
 
         if isinstance(unit, Unit):
             return Unit(unit)
 
         # compatibility with internal pint API
@@ -368,34 +383,70 @@
 
         raise ValueError(
             f"Incorrect input for unit: {unit} ({type(unit)}), "
             "expected Unit, UnitsContainer, str, dict[str, Number], Quantity or None"
         )
 
     @staticmethod
+    def _validate_magnitude(val: MT) -> MT:
+        # NOTE: container types (e.g. list[int]) are tested using only the first element
+
+        if isinstance(val, str):
+            raise TypeError(f'Input magnitude has incorrect type str: "{val}"')
+
+        # bool is always converted to float, the type hints don't consider bool at all
+        if isinstance(val, bool):
+            val = float(val)
+        if isinstance_types(val, list[bool]):
+            val = [float(n) for n in val]
+
+        # TODO: list of int is converted to np.ndarray, type hints cannot represent this properly
+        # do not input list[int] in code that should be type checked
+        # however, this input is still allowed for convenience, for example Q([1, 2, 3], 'kg')
+        if isinstance_types(val, list[int]):
+            val = np.array(val)
+
+        # list[float] is not converted
+        if isinstance_types(val, list[float]):
+            pass
+
+        # int is considered equivalent to float by type checkers
+        if isinstance(val, int):
+            val = float(val)
+
+        return val
+
+    @staticmethod
     def _get_magnitude_type(val: MT) -> type[MT]:
         if isinstance(val, list):
             if not len(val):
                 return list
 
-            # NOTE: this does not work for lists with multiple types
+            # NOTE: this does not work for heterogenous lists,
+            # don't use this type of input to avoid issues
             return list[type(val[0])]
 
         return type(val)
 
     @classmethod
     def get_unit(cls, unit_name: str) -> Unit:
         return Unit(cls._REGISTRY.parse_units(unit_name))
 
     @property
     def subclass(self) -> type[Quantity[DT, MT]]:
         return self._get_dimensional_subclass(
             self._dimensionality_type, self._magnitude_type
         )
 
+    def _set_original_magnitude_attributes(
+        self, mt_orig: MT, mt_orig_kwargs: dict[str, Any]
+    ) -> None:
+        self._original_magnitude_type = mt_orig
+        self._original_magnitude_kwargs = mt_orig_kwargs
+
     def __len__(self) -> int:
         # __len__() must return an integer
         # the len() function ensures this at a lower level
         if isinstance(self._magnitude, (float, int)):
             raise TypeError(
                 f"Quantity with scalar magnitude ({self._magnitude}) has no length"
             )
@@ -404,28 +455,67 @@
             raise TypeError(
                 f"Cannot determine length of Polars expression: {self._magnitude}"
             )
 
         return len(self._magnitude)
 
     def __copy__(self) -> Quantity[DT, MT]:
-        ret = self.subclass(copy.copy(self._magnitude), self._units)
+        ret = self._call_subclass(copy.copy(self._magnitude), self._units)
 
         return ret
 
     def __deepcopy__(self, memo: dict[int, Any] | None = None) -> Quantity[DT, MT]:
         if memo is None:
             memo = {}
 
-        ret = self.subclass(
+        ret = self._call_subclass(
             copy.deepcopy(self._magnitude, memo), copy.deepcopy(self._units, memo)
         )
 
         return ret
 
+    @classmethod
+    def _validate_datetime_magnitude(
+        cls,
+        magnitude: MT,
+        unit: Unit[DT] | UnitsContainer | str | None,
+        valid_unit: Unit[DT],
+    ) -> None:
+        _val_datetime = isinstance(
+            magnitude, (pd.DatetimeIndex, pl.Datetime, pd.Timestamp)
+        )
+
+        if _val_datetime:
+            if (
+                not valid_unit.dimensionless
+                or Quantity(1, valid_unit).to_base_units().m != 1
+            ):
+                raise ValueError(
+                    f"Passing datetime magnitude(s) ({magnitude}) "
+                    "is only valid for dimensionless Quantities with no scaling factor, "
+                    f"passed unit {unit} ({valid_unit.dimensionality})"
+                )
+
+        _magnitude_type_datetime = cls._magnitude_type in (
+            pd.Timestamp,
+            pd.DatetimeIndex,
+            pl.Datetime,
+        )
+
+        if _magnitude_type_datetime:
+            if (
+                not valid_unit.dimensionless
+                or Quantity(1, valid_unit).to_base_units().m != 1
+            ):
+                raise ValueError(
+                    f"Setting a datetime magnitude type ({cls._magnitude_type.__name__}) "
+                    "is only valid for dimensionless Quantities with no scaling factor, "
+                    f"passed unit {unit} ({valid_unit.dimensionality})"
+                )
+
     @staticmethod
     def _cast_array_float(inp: np.ndarray) -> np.ndarray:
         # don't fail in case the array contains unsupported objects,
         # for example uncertainties.ufloat
         try:
             return inp.astype(np.float64, casting="unsafe", copy=True)
         except TypeError:
@@ -437,153 +527,121 @@
         unit: Unit[DT] | UnitsContainer | str | None = None,
         # # this is a hack to force the type checker to default to Unknown
         # # in case the generic type is not specified at all
         # # do not pass the _dt parameter directly, always use square brackets to
         # # specify the dimensionality type
         # TODO: why is this required when the TypeVar has default=Unknown?
         _dt: type[DT] = Unknown,  # type: ignore
+        _mt_orig: type[MT] | None = None,
+        _mt_orig_kwargs: dict[str, Any] | None = None,
     ) -> Quantity[DT]:
+        if _dt is not Unknown:
+            raise ValueError(
+                f'Cannot pass a value for private parameter "_dt", passed {_dt} ({type(_dt)})'
+            )
+
         if isinstance(val, Quantity):
             if unit is not None:
                 raise ValueError(
                     f"Cannot pass unit: {unit} when "
                     f"input val is a Quantity: {val}. "
-                    "The unit must be None when passing a Quantity as val"
+                    "The unit must be None when passing a Quantity as input"
                 )
 
             val, unit = val.m, val.u
 
-        if isinstance(val, str):
-            raise TypeError(f'Input parameter "val" has incorrect type str: {val}')
-
-        if isinstance(unit, Quantity):
-            raise TypeError(
-                f'Input parameter "units" has incorrect type Quantity: {val}. '
-                "Do not create nested Quantity objects, convert "
-                "to separate magnitude and unit objects first."
-            )
-
         valid_unit = cls._validate_unit(unit)
+        valid_magnitude = cls._validate_magnitude(val)
 
-        # bool is always converted to float, the type hints don't consider bool at all
-        if isinstance(val, bool):
-            val = float(val)
-
-        if isinstance_types(val, list[bool]):
-            val = [float(n) for n in val]
-
-        # TODO: list of int is converted to np.ndarray, type hints cannot represent this properly
-        # do not input list[int] in code that should be type checked
-        # however, this input is still allowed for convenience, for example Q([1, 2, 3], 'kg')
-        if isinstance_types(val, list[int]):
-            val = np.array(val)
-
-        # int is considered equivalent to float by type checkers
-        if isinstance(val, int):
-            val = float(val)
-
+        # NOTE: "original" in this case does not necessarily refer to the type
+        # of the input magnitude, for example list[int] is converted to np.ndarray before
+        # this magnitude type is checked
         _original_magnitude_type = (
-            cls._original_magnitude_type or cls._get_magnitude_type(val)
+            _mt_orig
+            if _mt_orig is not None
+            else cls._get_magnitude_type(valid_magnitude)
         )
 
-        if isinstance(val, pd.Series):
-            val = val.to_numpy()
-
-        # TODO: how to validate that the subclass has the same dimensionality
-        # as the input unit?
-        # cannot raise error here since this breaks the pint.PlainQuantity methods
-        # that use return self.__class__(...)
-        if cls._dimensionality_type is Unset or str(
-            cls._dimensionality_type.dimensions
-        ) != str(valid_unit.dimensionality):
-            # special case for temperature difference
-            if valid_unit._units in cls.TEMPERATURE_DIFFERENCE_UCS:
-                subcls = cls._get_dimensional_subclass(TemperatureDifference, type(val))
-                return subcls(val, valid_unit)
-
-            dim = Dimensionality.get_dimensionality(valid_unit.dimensionality)
+        _original_magnitude_kwargs = (
+            _mt_orig_kwargs if _mt_orig_kwargs is not None else {}
+        )
 
-            # the __new__ method of the new subclass will be called instead
-            subcls = cls._get_dimensional_subclass(dim, type(val))
-            subcls._original_magnitude_type = _original_magnitude_type
+        # special case for pd.Series, must convert to np.ndarray to avoid
+        # TypeError: PlainQuantity cannot wrap upcast type
+        # NOTE: pl.Series and pl.Expr don't require this type of workaround
+        if isinstance(valid_magnitude, pd.Series):
+            # preserve pd.Series metadata (not dtype, this would cause issues with float/int)
+            _original_magnitude_kwargs |= {
+                "index": valid_magnitude.index,
+                "name": valid_magnitude.name,
+            }
 
-            return subcls(val, valid_unit)
+            valid_magnitude = valid_magnitude.to_numpy()
 
-        # TODO:
+        is_incomplete_subclass = cls._dimensionality_type is Unset or str(
+            cls._dimensionality_type.dimensions
+        ) != str(valid_unit.dimensionality)
 
-        _val_datetime = isinstance(val, (pd.DatetimeIndex, pl.Datetime, pd.Timestamp))
+        if is_incomplete_subclass:
+            # TODO: how to validate that the subclass has the same dimensionality
+            # as the input unit?
+            # cannot raise error here since this breaks the pint.PlainQuantity methods
+            # that use return self.__class__(...)
 
-        if _val_datetime:
-            if (
-                not valid_unit.dimensionless
-                or Quantity(1, valid_unit).to_base_units().m != 1
-            ):
-                raise ValueError(
-                    f"Passing datetime magnitude(s) ({val}) "
-                    "is only valid for dimensionless Quantities with no scaling factor, "
-                    f"passed unit {unit} ({valid_unit.dimensionality})"
+            # special case for temperature difference
+            if valid_unit._units in cls.TEMPERATURE_DIFFERENCE_UCS:
+                subcls = cls._get_dimensional_subclass(
+                    TemperatureDifference, type(valid_magnitude)
                 )
+            else:
+                dim = Dimensionality.get_dimensionality(valid_unit.dimensionality)
+                subcls = cls._get_dimensional_subclass(dim, type(valid_magnitude))
 
-        _magnitude_type_datetime = cls._magnitude_type in (
-            pd.Timestamp,
-            pd.DatetimeIndex,
-            pl.Datetime,
-        )
-
-        if _magnitude_type_datetime:
-            if (
-                not valid_unit.dimensionless
-                or Quantity(1, valid_unit).to_base_units().m != 1
-            ):
-                raise ValueError(
-                    f"Setting a datetime magnitude type ({cls._magnitude_type.__name__}) "
-                    "is only valid for dimensionless Quantities with no scaling factor, "
-                    f"passed unit {unit} ({valid_unit.dimensionality})"
-                )
+            return subcls(
+                valid_magnitude,
+                valid_unit,
+                _mt_orig=_original_magnitude_type,
+                _mt_orig_kwargs=_original_magnitude_kwargs,
+            )
 
-        # at this point the value and dimensionality of the units are verified to be correct
-        # pass the inputs to pint to actually construct the Quantity
+        cls._validate_datetime_magnitude(valid_magnitude, unit, valid_unit)
 
-        # pint.quantity.Quantity uses Generic[_MagnitudeType] instead of Generic[DT, MT],
-        # ignore this type mismatch since the Generic is overridden
         qty: Quantity[DT, MT] = super().__new__(  # type: ignore
-            cls, val, units=valid_unit
+            cls, valid_magnitude, units=valid_unit
         )
 
-        qty._original_magnitude_type = _original_magnitude_type
-
         # ensure that pint did not change the dtype of numpy arrays
         if isinstance(qty._magnitude, np.ndarray):
             qty._magnitude = cls._cast_array_float(qty._magnitude)
 
+        # propagate the original magnitude type and constructor kwargs
+        qty._set_original_magnitude_attributes(
+            _original_magnitude_type, _original_magnitude_kwargs
+        )
+
         return qty
 
     @property
     def m(self) -> MT:
-        if self._original_magnitude_type is None:
-            return self._magnitude
-
-        # TODO: is it possible to make this generic?
-
-        # NOTE: this is a workaround to match the type checker output
-        # list[int] and list[float] are not interchangeable,
-        # but int and float are (mostly?)
         if self._original_magnitude_type == list[int]:
+            # NOTE: this is a workaround to match the type checker output (np.ndarray)
+            # this is not consistent with the behavior for list[float]
             return self._magnitude
 
-        if self._original_magnitude_type == list[float]:
+        elif self._original_magnitude_type == list[float]:
             return [float(n) for n in self._magnitude]
 
-        if self._original_magnitude_type == pd.Timestamp:
-            return pd.Timestamp(self._magnitude)
+        elif self._original_magnitude_type == pd.Timestamp:
+            return pd.Timestamp(self._magnitude, **self._original_magnitude_kwargs)
 
-        if self._original_magnitude_type == pd.Series:
-            return pd.Series(self._magnitude)
+        elif self._original_magnitude_type == pd.Series:
+            return pd.Series(self._magnitude, **self._original_magnitude_kwargs)
 
-        return self._magnitude
+        else:
+            return self._magnitude
 
     @property
     def u(self) -> Unit[DT]:
         return Unit(super().u)
 
     @property
     def units(self) -> Unit[DT]:
@@ -600,43 +658,53 @@
                 new_name = Quantity(1, unit)._dimensionality_type.__name__
 
                 raise DimensionalityTypeError(
                     f"Cannot convert {self.units} (dimensionality {current_name}) "
                     f"to {unit} (dimensionality {new_name})"
                 )
 
+    def _call_subclass(self, *args) -> Quantity[DT, MT]:
+        return self.subclass(
+            *args,
+            _mt_orig=self._original_magnitude_type,
+            _mt_orig_kwargs=self._original_magnitude_kwargs,
+        )
+
     def to_reduced_units(self) -> Quantity[DT, MT]:
         ret = super().to_reduced_units()
-        return self.subclass(ret)
+        return self._call_subclass(ret)
 
     def to_root_units(self) -> Quantity[DT, MT]:
         ret = super().to_root_units()
-        return self.subclass(ret)
+        return self._call_subclass(ret)
 
     def to_base_units(self) -> Quantity[DT, MT]:
         self._check_temperature_compatibility(Unit("kelvin"))
 
         ret = super().to_base_units()
-        return self.subclass(ret)
+        return self._call_subclass(ret)
 
     def _to_unit(self, unit: Unit[DT_] | UnitsContainer | str | dict) -> Unit[DT_]:
         return self._validate_unit(unit)
 
     def to(self, unit: Unit[DT] | UnitsContainer | str | dict) -> Quantity[DT, MT]:
         unit = self._to_unit(unit)
 
         self._check_temperature_compatibility(unit)
-
         m = self._convert_magnitude_not_inplace(unit)
 
         if unit._units in self.TEMPERATURE_DIFFERENCE_UCS:
-            return Quantity[TemperatureDifference](m, unit)
+            return Quantity[TemperatureDifference](
+                m,
+                unit,
+                _mt_orig=self._original_magnitude_type,
+                _mt_orig_kwargs=self._original_magnitude_kwargs,
+            )
 
-        converted = self.subclass(m, unit)
-        converted._original_magnitude_type = self._original_magnitude_type
+        converted = self._call_subclass(m, unit)
 
         return converted
 
     def ito(self, unit: Unit[DT] | UnitsContainer | str) -> None:
         # NOTE: this method cannot convert the dimensionality type
 
         unit = self._to_unit(unit)
@@ -792,35 +860,31 @@
         return expr
 
     @staticmethod
     def get_unit_symbol(s: str) -> sp.Symbol:
         return sp.Symbol("\\text{" + s + "}", nonzero=True, positive=True)
 
     @classmethod
-    def get_dimension_symbol_map(cls) -> dict[sp.Basic, Unit]:
-        if cls._dimension_symbol_map is not None:
-            return cls._dimension_symbol_map
-
+    def _populate_dimension_symbol_map(cls) -> None:
         # also consider custom dimensions defined with encomp.units.define_dimensionality
-        cls._dimension_symbol_map = {
+        cls._dimension_symbol_map |= {
             cls.get_unit_symbol(n): cls.get_unit(n)
             for n in list(_BASE_SI_UNITS) + CUSTOM_DIMENSIONS
         }
 
-        return cls._dimension_symbol_map
-
     @classmethod
     def from_expr(cls, expr: sp.Basic) -> Quantity[Unknown, float]:
         """
         Converts a Sympy expression with unit symbols
         into a Quantity. This only works in case expression
         *only* contains base SI unit symbols.
         """
 
-        _dimension_symbol_map = cls.get_dimension_symbol_map()
+        # this needs to be populated here to account for custom dimensions
+        cls._populate_dimension_symbol_map()
 
         expr = expr.simplify()
         args = expr.args
 
         if not args:
             return cls(float(expr), "dimensionless")  # type: ignore
 
@@ -833,15 +897,15 @@
 
         unit = cls.get_unit("")
 
         for d in dimensions:
             unit_i = cls.get_unit("")
 
             for symbol, power in d.as_powers_dict().items():  # type: ignore
-                unit_i *= _dimension_symbol_map[symbol] ** power
+                unit_i *= cls._dimension_symbol_map[symbol] ** power
 
             unit *= unit_i
 
         return cls(magnitude, unit).to_base_units()
 
     @classmethod
     def __get_validators__(cls):
@@ -935,31 +999,32 @@
 
             return np.zeros_like(is_equal).astype(bool)
 
         return is_equal and self.is_compatible_with(other)
 
     def __mul__(self, other):
         ret = super().__mul__(other)
-        ret._original_magnitude_type = self._original_magnitude_type
 
         if self.dimensionless and isinstance(other, Quantity):
             return other.subclass(ret)
 
-        return self.subclass(ret)
+        return self._call_subclass(ret)
 
     def __rmul__(self, other):
         ret = super().__rmul__(other)
-        ret._original_magnitude_type = self._original_magnitude_type
 
-        return self.subclass(ret)
+        return self._call_subclass(ret)
 
     def __truediv__(self, other):
         ret = super().__truediv__(other)
+        return self._call_subclass(ret)
 
-        return self.subclass(ret)
+    def __rtruediv__(self, other):
+        ret = super().__rtruediv__(other)
+        return self._call_subclass(ret)
 
     def _temperature_difference_add_sub(
         self: Quantity[Temperature, MT],
         other: Quantity[TemperatureDifference, MT],
         operator: Literal["add", "sub"],
     ) -> Quantity[Temperature, MT]:
         v1 = self.to("degC").m
@@ -989,15 +1054,15 @@
 
                 return self._temperature_difference_add_sub(other, "add")
 
             raise e
 
         ret = super().__add__(other)
 
-        return self.subclass(ret)
+        return self._call_subclass(ret)
 
     def __sub__(self, other):
         try:
             self.check_compatibility(other)
         except DimensionalityTypeError as e:
             if isinstance_types(
                 self, Quantity[Temperature] | Quantity[TemperatureDifference]
@@ -1015,15 +1080,15 @@
 
         if (
             self._dimensionality_type is Temperature
             and other._dimensionality_type is Temperature
         ):
             return Quantity[TemperatureDifference, type(ret.m)](ret.m, ret.u)
 
-        return self.subclass(ret)
+        return self._call_subclass(ret)
 
     def __gt__(self, other):
         try:
             return super().__gt__(other)
         except ValueError as e:
             raise DimensionalityComparisonError(str(e)) from e
 
@@ -1055,35 +1120,38 @@
         ret = super().__getitem__(index)
 
         if isinstance(ret._magnitude, pd.Timestamp):
             scalar_type = pd.Timestamp
         else:
             scalar_type = float
 
-        ret._original_magnitude_type = scalar_type
+        # NOTE: this is a special case, scalar magnitudes cannot have kwargs
 
         subcls = self._get_dimensional_subclass(self._dimensionality_type, scalar_type)
-        subcls._original_magnitude_type = scalar_type
+        ret._original_magnitude_type = scalar_type
 
-        return subcls(ret.m, ret.u)
+        return subcls(
+            ret.m,
+            ret.u,
+        )
 
     @property
     def ndim(self) -> int:
         # compatibility with pandas broadcasting
         # if ndim == 0, pandas considers the object
         # a scalar and will fill array when assigning columns
         # this is similar to setting ureg.force_ndarray_like
         # except that it still allows for scalar magnitudes
 
         if isinstance(self.m, (float, int)):
             return 0
 
         return self.m.ndim
 
-    def asdim(self, other):
+    def asdim(self, other: type[DT_] | Quantity[DT_, MT]) -> Quantity[DT_, MT]:
         if isinstance(other, Quantity):
             dim = other._dimensionality_type
             assert dim is not None
         else:
             dim = other
 
         if str(self._dimensionality_type.dimensions) != str(dim.dimensions):
@@ -1092,14 +1160,68 @@
                 f"the dimensions do not match: {self._dimensionality_type.dimensions} != "
                 f"{dim.dimensions}"
             )
 
         subcls = self._get_dimensional_subclass(dim, self._magnitude_type)
         return subcls(self)
 
+    def astype(self, magnitude_type: type[MT_], **kwargs: Any) -> Quantity[DT, MT_]:
+        m, u = self.m, self.u
+
+        _is_iterable = isinstance(m, Iterable)
+
+        # astype for np.ndarray should be called directly except for some special cases
+        custom_conversion = [pd.Series, pl.Series, list[float]]
+
+        if isinstance(m, np.ndarray) and magnitude_type not in custom_conversion:
+            return self.subclass(m.astype(magnitude_type), u)
+
+        if magnitude_type in (pd.DatetimeIndex, pd.Timestamp):
+            raise ValueError(
+                f"Cannot convert to datetime magnitude type: {magnitude_type}"
+            )
+
+        if magnitude_type == pl.Expr:
+            raise ValueError("Cannot convert magnitude to Polars expression")
+
+        if magnitude_type == list[int]:
+            raise NotImplementedError(
+                "Cannot convert magnitude to list[int], use list[float] instead"
+            )
+
+        if magnitude_type in (float, int):
+            if _is_iterable:
+                return self.subclass([float(n) for n in m], u)
+            else:
+                return self.subclass(float(m), u)
+
+        if magnitude_type == list[float]:
+            if not _is_iterable:
+                m = [m]
+            return self.subclass([float(n) for n in m], u)
+
+        if magnitude_type == np.ndarray:
+            if not _is_iterable:
+                m = [m]
+            return self.subclass(np.array(m), u)
+
+        if magnitude_type == pd.Series:
+            if not _is_iterable:
+                m = [m]
+            return self.subclass(pd.Series(m, **kwargs), u)
+
+        if magnitude_type == pl.Series:
+            if not _is_iterable:
+                m = [m]
+            kwargs["values"] = m
+            return self.subclass(pl.Series(**kwargs), u)
+
+        # ensure that this method returns a new instance
+        return self.__copy__()
+
 
 # override the implementations for the Quantity and Unit classes for the current registry
 # this ensures that all Quantity objects created with this registry are the correct type
 ureg.Quantity = Quantity
 ureg.Unit = Unit
 
 # the default format must be set after Quantity and Unit are registered
```

### Comparing `encomp-0.9.0/encomp/units.pyi` & `encomp-0.9.1/encomp/units.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from pint.registry import UnitRegistry
 from pint.util import UnitsContainer
 
 from .utypes import (
     DT,
     DT_,
     MT,
+    MT_,
     Area,
     AreaUnits,
     Currency,
     CurrencyPerEnergy,
     CurrencyPerEnergyUnits,
     CurrencyPerMass,
     CurrencyPerMassUnits,
@@ -167,14 +168,15 @@
     @property
     def units(self) -> Unit[DT]: ...
     @property
     def ndim(self) -> int: ...
     def to_reduced_units(self) -> Quantity[DT, MT]: ...
     def to_base_units(self) -> Quantity[DT, MT]: ...
     def asdim(self, other: type[DT_] | Quantity[DT_, MT]) -> Quantity[DT_, MT]: ...
+    def astype(self, magnitude_type: type[MT_], **kwargs: Any) -> Quantity[DT, MT_]: ...
     def to(self, unit: Unit[DT] | UnitsContainer | str | dict) -> Quantity[DT, MT]: ...
     def ito(self, unit: Unit[DT] | UnitsContainer | str) -> None: ...
     def check(
         self,
         unit: Quantity[Unknown, Any]
         | UnitsContainer
         | Unit
@@ -184,16 +186,14 @@
     ) -> bool: ...
     def __format__(self, format_type: str) -> str: ...
     @staticmethod
     def correct_unit(unit: str) -> str: ...
     @staticmethod
     def get_unit_symbol(s: str) -> sp.Symbol: ...
     @classmethod
-    def get_dimension_symbol_map(cls) -> dict[sp.Basic, Unit]: ...
-    @classmethod
     def from_expr(cls, expr: sp.Basic) -> Quantity[Unknown, float]: ...
     @classmethod
     def __get_validators__(cls) -> Generator[Incomplete, None, None]: ...
     @classmethod
     def validate(cls, qty: Quantity[DT, MT]) -> Quantity[DT, MT]: ...
     def is_compatible_with(
         self, other: Quantity | float | int, *contexts, **ctx_kwargs
```

### Comparing `encomp-0.9.0/encomp/utypes.py` & `encomp-0.9.1/encomp/utypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -539,14 +539,27 @@
         pd.DatetimeIndex,
         pd.Timestamp,
         pl.Series,
         pl.Expr,
         default=np.ndarray,
     )
 
+    MT_ = TypeVar(
+        "MT_",
+        float,
+        list[float],
+        np.ndarray,
+        pd.Series,
+        pd.DatetimeIndex,
+        pd.Timestamp,
+        pl.Series,
+        pl.Expr,
+        default=np.ndarray,
+    )
+
     # type variables that represent a certain dimensionality
     # the DT_ type variable is used to signify a different (possible identical) dimensionality than DT
     # these type variables are invariant, since
     # Q[DimA] is not a subclass of Q[DimB] if DimA is a subclass of DimB
     # all Q[DT] subclasses are direct subclasses of Q
     # it might make sense to consider DT as covariant, but it won't have any practical advantages,
     # and it does not match the actual implementation
@@ -560,14 +573,26 @@
         float,
         list[float],
         np.ndarray,
         pd.Series,
         pd.DatetimeIndex,
         pd.Timestamp,
         pl.Series,
+        pl.Expr,
+    )
+
+    MT_ = TypeVar(
+        "MT_",
+        float,
+        list[float],
+        np.ndarray,
+        pd.Series,
+        pd.DatetimeIndex,
+        pd.Timestamp,
+        pl.Series,
         pl.Expr,
     )
 
     DT = TypeVar("DT", bound=Dimensionality)
     DT_ = TypeVar("DT_", bound=Dimensionality)
```

### Comparing `encomp-0.9.0/pyproject.toml` & `encomp-0.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [tool.poetry]
 name = "encomp"
-version = "0.9.0"
+version = "0.9.1"
 description = "General-purpose library for engineering calculations"
 authors = ["William Laurén <lauren.william.a@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{ include = "encomp" }]
 include = ["encomp/defs"]
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
+urllib3 = "^1"             # https://github.com/urllib3/urllib3/issues/3010
 python-dateutil = "*"
 python-dotenv = "*"
 pydantic = "*"
 typeguard = "^3"
 typing-extensions = "*"
 asttokens = "*"
 numpy = "*"
 pandas = "*"
+pyarrow = "*"
 polars = "*"
 sympy = "*"
 symbolic-equation = "*"
-pint = "^0.20"
+pint = "~0.21"
 coolprop = "^6.4"
 uncertainties = "*"
 matplotlib = { version = "*", optional = true }
 seaborn = { version = "*", optional = true }
 scipy = { version = "*", optional = true }
 fire = { version = "*", optional = true }
 fluids = { version = "*", optional = true }
@@ -76,15 +78,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.black]
 line-length = 88
-target-version = ["py310"]
+target-version = ["py311"]
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
@@ -128,15 +130,15 @@
 ]
 
 line-length = 120
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-target-version = "py310"
+target-version = "py311"
 
 [tool.ruff.mccabe]
 max-complexity = 10
 
 [tool.pytest.ini_options]
 filterwarnings = [
   # ignore the mypy-testing marks when this plugin is disabled
```

### Comparing `encomp-0.9.0/PKG-INFO` & `encomp-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encomp
-Version: 0.9.0
+Version: 0.9.1
 Summary: General-purpose library for engineering calculations
 License: MIT
 Author: William Laurén
 Author-email: lauren.william.a@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,27 +15,29 @@
 Requires-Dist: coolprop (>=6.4,<7.0)
 Requires-Dist: fire ; extra == "optional"
 Requires-Dist: fluids ; extra == "optional"
 Requires-Dist: ht ; extra == "optional"
 Requires-Dist: matplotlib ; extra == "optional"
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: pint (>=0.20,<0.21)
+Requires-Dist: pint (>=0.21,<0.22)
 Requires-Dist: polars
+Requires-Dist: pyarrow
 Requires-Dist: pydantic
 Requires-Dist: python-dateutil
 Requires-Dist: python-dotenv
 Requires-Dist: scipy ; extra == "optional"
 Requires-Dist: seaborn ; extra == "optional"
 Requires-Dist: symbolic-equation
 Requires-Dist: sympy
 Requires-Dist: thermo ; extra == "optional"
 Requires-Dist: typeguard (>=3,<4)
 Requires-Dist: typing-extensions
 Requires-Dist: uncertainties
+Requires-Dist: urllib3 (>=1,<2)
 Description-Content-Type: text/markdown
 
 # encomp
 
 > General-purpose library for *en*gineering *comp*utations, with focus on clean and consistent interfaces.
 
 Documentation at <https://encomp.readthedocs.io/en/latest/>
```

