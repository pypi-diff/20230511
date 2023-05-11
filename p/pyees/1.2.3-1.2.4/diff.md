# Comparing `tmp/pyees-1.2.3.tar.gz` & `tmp/pyees-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.2.3.tar", last modified: Mon Apr 24 16:54:33 2023, max compression
+gzip compressed data, was "pyees-1.2.4.tar", last modified: Thu May 11 12:22:09 2023, max compression
```

## Comparing `pyees-1.2.3.tar` & `pyees-1.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 16:54:33.545760 pyees-1.2.3/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-04-24 16:54:33.549748 pyees-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 16:54:33.409657 pyees-1.2.3/pyees/
--rw-rw-rw-   0        0        0      445 2023-04-21 11:08:47.000000 pyees-1.2.3/pyees/__init__.py
--rw-rw-rw-   0        0        0    15214 2023-04-24 08:53:03.000000 pyees-1.2.3/pyees/fit.py
--rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.2.3/pyees/profilePyees.py
--rw-rw-rw-   0        0        0     9051 2023-04-21 09:09:36.000000 pyees-1.2.3/pyees/prop.py
--rw-rw-rw-   0        0        0    14733 2023-04-24 15:08:43.000000 pyees-1.2.3/pyees/readData.py
--rw-rw-rw-   0        0        0    10193 2023-04-21 12:20:02.000000 pyees-1.2.3/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.2.3/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     3889 2023-04-19 12:43:28.000000 pyees-1.2.3/pyees/testFit.py
--rw-rw-rw-   0        0        0    12431 2023-04-21 11:06:00.000000 pyees-1.2.3/pyees/testProp.py
--rw-rw-rw-   0        0        0     1059 2023-04-19 12:41:29.000000 pyees-1.2.3/pyees/testPyees.py
--rw-rw-rw-   0        0        0    15674 2023-04-24 15:13:29.000000 pyees-1.2.3/pyees/testReadData.py
--rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.2.3/pyees/testSolve.py
--rw-rw-rw-   0        0        0     8958 2023-04-15 19:26:44.000000 pyees-1.2.3/pyees/testUnit.py
--rw-rw-rw-   0        0        0    81276 2023-04-19 12:40:55.000000 pyees-1.2.3/pyees/testVariable.py
--rw-rw-rw-   0        0        0    45294 2023-04-15 19:24:42.000000 pyees-1.2.3/pyees/unit.py
--rw-rw-rw-   0        0        0    35819 2023-04-24 16:15:04.000000 pyees-1.2.3/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:54:33.526343 pyees-1.2.3/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-04-24 16:54:32.000000 pyees-1.2.3/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-04-24 16:54:33.494428 pyees-1.2.3/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 16:54:32.000000 pyees-1.2.3/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-24 16:54:32.000000 pyees-1.2.3/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-24 16:54:32.000000 pyees-1.2.3/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-24 16:54:33.573684 pyees-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1216 2023-04-24 16:54:27.000000 pyees-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 12:22:09.124577 pyees-1.2.4/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.2.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-05-11 12:22:09.140204 pyees-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 12:22:08.859592 pyees-1.2.4/pyees/
+-rw-rw-rw-   0        0        0      445 2023-04-21 11:08:47.000000 pyees-1.2.4/pyees/__init__.py
+-rw-rw-rw-   0        0        0    12829 2023-05-11 09:38:32.000000 pyees-1.2.4/pyees/fit.py
+-rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.2.4/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0     9126 2023-05-11 09:38:14.000000 pyees-1.2.4/pyees/prop.py
+-rw-rw-rw-   0        0        0    14733 2023-04-24 15:08:43.000000 pyees-1.2.4/pyees/readData.py
+-rw-rw-rw-   0        0        0    10193 2023-04-21 12:20:02.000000 pyees-1.2.4/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.2.4/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7669 2023-04-27 10:39:41.000000 pyees-1.2.4/pyees/testFit.py
+-rw-rw-rw-   0        0        0    12431 2023-05-11 09:11:30.000000 pyees-1.2.4/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1059 2023-04-27 11:06:19.000000 pyees-1.2.4/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    15674 2023-04-24 15:13:29.000000 pyees-1.2.4/pyees/testReadData.py
+-rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.2.4/pyees/testSolve.py
+-rw-rw-rw-   0        0        0     8958 2023-04-15 19:26:44.000000 pyees-1.2.4/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    81533 2023-05-11 11:53:42.000000 pyees-1.2.4/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    44518 2023-05-11 12:21:25.000000 pyees-1.2.4/pyees/unit.py
+-rw-rw-rw-   0        0        0    35130 2023-05-11 11:54:28.000000 pyees-1.2.4/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-05-11 12:22:09.062077 pyees-1.2.4/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-05-11 12:22:07.000000 pyees-1.2.4/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-05-11 12:22:07.000000 pyees-1.2.4/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 12:22:07.000000 pyees-1.2.4/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-11 12:22:07.000000 pyees-1.2.4/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-11 12:22:07.000000 pyees-1.2.4/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-11 12:22:09.171454 pyees-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1216 2023-05-11 12:21:41.000000 pyees-1.2.4/setup.py
```

### Comparing `pyees-1.2.3/LICENSE.txt` & `pyees-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.2.3/PKG-INFO` & `pyees-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.2.3
+Version: 1.2.4
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.2.3/README.md` & `pyees-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.2.3/pyees/profilePyees.py` & `pyees-1.2.4/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.3/pyees/prop.py` & `pyees-1.2.4/pyees/prop.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,17 @@
     
     if not (all([ns[0] == n] for n in ns)):
         raise ValueError('All parameters has to have the same length')
     
     if ns:
         n = ns[0]
         for i, param in enumerate(params):
-            if not type(param) == arrayVariable:
+            if param is None:
+                paramVecs[i] = [None] * n
+            elif not type(param) == arrayVariable:
                 paramVecs[i] = variable([param.value] * n, param.unit, [param.uncert] * n)
         for i in range(n):
             params = [elem[i] for elem in paramVecs]
             out.append(scalarMethod(property, *params))
         return variable([elem.value for elem in out], out[0].unit, [elem.uncert for elem in out])
         
     return scalarMethod(property, *params)
@@ -241,15 +243,15 @@
         desiredUnits.append('m')
     else:
         desiredUnits.append('Pa')
         
     for Var, desiredUnit in zip(vars, desiredUnits):
         Var.convert(desiredUnit)
     
-    out = outputFromParameters(propHumidAirScalar, property, [T, Rh, H, P])
+    out = outputFromParameters(propHumidAirScalar, property, [T,Rh, H, P])
     
     for Var, varUnit in zip(vars, varUnits):
         Var.convert(varUnit)
     
     return out
 
 def propHumidAirScalar(property, T,Rh,H = None, P = None):
```

### Comparing `pyees-1.2.3/pyees/readData.py` & `pyees-1.2.4/pyees/readData.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.3/pyees/solve.py` & `pyees-1.2.4/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.3/pyees/stackOverflowODR.py` & `pyees-1.2.4/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.3/pyees/testProp.py` & `pyees-1.2.4/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.3/pyees/testPyees.py` & `pyees-1.2.4/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.3/pyees/testReadData.py` & `pyees-1.2.4/pyees/testReadData.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.3/pyees/testSolve.py` & `pyees-1.2.4/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.3/pyees/testUnit.py` & `pyees-1.2.4/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.3/pyees/testVariable.py` & `pyees-1.2.4/pyees/testVariable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1277,14 +1277,22 @@
         np.testing.assert_equal(c.uncert, uc)
 
     def testConvert(self):
         a = variable(1, 'km')
         b = variable(1, 'm')
         c = a * b
         c.convert('mm2')
+        
+        
+        diameter = variable(40, 'cm')
+        area = np.pi / 4 * diameter ** 2
+        area.convert('m2')
+        self.assertEqual(area.value, 0.12566370614359172953850573)
+        self.assertEqual(area.unit, 'm2')       
+        
 
     def testCompare(self):
         a = variable(1, 'm')
         b = variable([2, 3, 4], 'm')
         np.testing.assert_equal(a < b, [True, True, True])
         np.testing.assert_equal(a <= b, [True, True, True])
         np.testing.assert_equal(a > b, [False, False, False])
```

### Comparing `pyees-1.2.3/pyees/unit.py` & `pyees-1.2.4/pyees/unit.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 class _unitConversion():
 
     def __init__(self, scale, offset=0) -> None:
         self.scale = scale
         self.offset = offset
 
+
+
     def __mul__(self, other):
         if isinstance(other, _unitConversion):
             scale = self.scale * other.scale
             offset = self.scale * other.offset + self.offset
         else:
             scale = self.scale * other
             offset = self.offset
@@ -20,23 +22,23 @@
         scale = 1
         offset = 0
         
         for _ in range(other):
             scale *= self.scale
             offset*= self.scale
             offset += self.offset
-
+            
         return _unitConversion(scale, offset)
 
+
     def __truediv__(self, other):
         if isinstance(other, _unitConversion):
             return _unitConversion(1 / other.scale, - other.offset / other.scale) * self
         return self * _unitConversion(1 / other)
 
-
     def convert(self, value, useOffset=True):
         if useOffset:
             return self.scale * value + self.offset
         else:
             return self.scale * value
 
 class neperConversion():
@@ -353,16 +355,15 @@
         # split the unit in upper and lower
         self.upper, self.upperPrefix, self.upperExp, self.lower, self.lowerPrefix, self.lowerExp = self._getLists(unitStr)
 
         # create the unit string
         self.unitStr = self._createUnitString()
 
         self._SIBaseUnit = self._getSIBaseUnit(self.upper, self.upperExp, self.lower, self.lowerExp)
-        otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp = self._getLists(self._SIBaseUnit)
-        self._converterToSI = self._getConverter(otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp)
+        self._converterToSI = self._getConverter(*self._getLists(self._SIBaseUnit))
 
     def _createUnitString(self):
         return self._combineUpperAndLower(self.upper, self.upperPrefix, self.upperExp, self.lower, self.lowerPrefix, self.lowerExp)
 
     @staticmethod
     def _cancleUnits(upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp):
         # cancle the units
@@ -479,37 +480,34 @@
         )
 
         out = unit._combineUpperAndLower(upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp)
 
         return out
 
     @staticmethod
-    def _splitUnitExponentAndPrefix(listOfUnitStrings):
-        n = len(listOfUnitStrings)
-        uList = [None] * n
-        prefixList = [None] * n
-        expList = [None] * n
-        for i in range(n):
-            prefixUnit, exponent = unit._removeExponentFromUnit(listOfUnitStrings[i])
-            u, prefix = unit._removePrefixFromUnit(prefixUnit)
-            uList[i] = u
-            prefixList[i] = prefix
-            expList[i] = exponent
-        return uList, prefixList, expList
+    def _splitUnitExponentAndPrefix(unitStr):
+        prefixUnit, exponent = unit._removeExponentFromUnit(unitStr)
+        u, prefix = unit._removePrefixFromUnit(prefixUnit)
+        return u, prefix, exponent
+
 
     @staticmethod
     def _getLists(unitStr):
         upper, lower = unit._splitCompositeUnit(unitStr)
-
-        upper, upperPrefix, upperExp = unit._splitUnitExponentAndPrefix(upper)
-        lower, lowerPrefix, lowerExp = unit._splitUnitExponentAndPrefix(lower)
-
+                
+        upper, upperPrefix, upperExp = map(list, zip(*[unit._splitUnitExponentAndPrefix(up) for up in upper]))
+        
         if lower:
+            lower, lowerPrefix, lowerExp = map(list, zip(*[unit._splitUnitExponentAndPrefix(low) for low in lower]))
             upper = ['DELTA' + elem if elem in temperature else elem for elem in upper]
             lower = ['DELTA' + elem if elem in temperature else elem for elem in lower]
+        else:
+            lowerPrefix = []
+            lowerExp = []
+
 
         return upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp
 
     @ staticmethod
     def _formatUnit(unitStr):
         
         if unitStr is None:
@@ -643,16 +641,14 @@
             if s == '(':
                 tally += 1
             if s == ')':
                 tally -= 1
       
         
         return unit.__formatUnit(unitStr)
-        
-    
             
     @staticmethod
     def __formatUnit(unitStr):
         # Removing any spaces
         unitStr = unitStr.replace(' ', '')
         unitStr = unitStr.split('/')
         
@@ -692,33 +688,29 @@
         upper = compositeUnit[0].split(hyphen)
         lower = compositeUnit[1].split(hyphen) if len(compositeUnit) > 1 else []
 
         return upper, lower
 
     @ staticmethod
     def _removeExponentFromUnit(u):
+        
         integerIndexes = [i for i, char in enumerate(u) if char in integers]
-        exponent = 1
+        
         if not integerIndexes:
-            return u, exponent
+            return u, 1
 
-        # override the exponent if there are any integerindexes
-        if integerIndexes:
-            # determine if all integers are consectutive together
-            # sum(a, a+1, ... b-1, b) = (b * (b-1) - a * (a-1)) / 2
-            minIndex, maxIndex = integerIndexes[0] - 1, integerIndexes[-1]
-            if sum(integerIndexes) != (maxIndex * (maxIndex + 1) - minIndex * (minIndex + 1)) / 2:
+        for i in range(len(integerIndexes)-1):
+            if integerIndexes[i+1] - integerIndexes[i] != 1:
                 raise ValueError('All numbers in the unit has to be grouped together')
 
-            # Determine if the last integer is placed at the end of the unit
-            if integerIndexes[-1] != len(u) - 1:
-                raise ValueError('Any number has to be placed at the end of the unit')
+        # Determine if the last integer is placed at the end of the unit
+        if integerIndexes[-1] != len(u) - 1:
+            raise ValueError('Any number has to be placed at the end of the unit')
 
-            exponent = int(u[minIndex+1:])
-            u = u[:minIndex+1]
+        u, exponent = u[:integerIndexes[0]], int(u[integerIndexes[0]:])
 
 
         # Ensure that the entire use was not removed by removing the integers
         if not u:
             # No symbols are left after removing the integers
             if exponent != 1:
                 raise ValueError(f'The unit {u} was stripped of all integers which left no symbols in the unit. This is normally due to the integers removed being equal to 1, as the unit is THE unit. Howver, the intergers removed was not equal to 1. The unit is therefore not known.')
@@ -777,46 +769,62 @@
 
         # look for the unit without the prefix
         if not unit in knownUnits:
             raise ValueError(f'The unit ({prefix}{unit}) was not found. Therefore it was interpreted as a prefix and a unit. However the unit ({unit}) was not found')
         return unit, prefix
 
     @staticmethod
-    def _getSIBaseUnit(upper, upperExp, lower, lowerExp):       
+    def _splitCompositeAndIncreaseExponent(unitStr, exp):
+            
+        up, low = unit._splitCompositeUnit(knownUnits[unitStr][0])
+        
+        up, upExp = map(list, zip(*[unit._removeExponentFromUnit(elem) for elem in up]))
+        low, lowExp = map(list, zip(*[unit._removeExponentFromUnit(elem) for elem in low])) if low else [[],[]]
+        
+        upExp = [elem * exp for elem in upExp]
+        lowExp = [elem * exp for elem in lowExp]
+        
+        return up, upExp, low, lowExp
+
+    @staticmethod
+    def _getSIBaseUnit(upper, upperExp, lower, lowerExp):    
+                
         nUpper = len(upper)
-        upperOut = []
-        lowerOut = []
-        upperExpOut = []
-        lowerExpOut = []
+        upperOut, lowerOut, upperExpOut, lowerExpOut = [], [], [], []
+        
         for i, (elem, exp) in enumerate(zip(upper + lower, upperExp + lowerExp)):
+            
             up,low = unit._splitCompositeUnit(knownUnits[elem][0])
+            
             if (i >= nUpper):
                 up, low = low, up
+            
             for elem in up:
                 elem, elemExp = unit._removeExponentFromUnit(elem)
+                elemExp *= exp
                 if not elem in upperOut:
                     upperOut.append(elem)
-                    upperExpOut.append(elemExp * exp)
+                    upperExpOut.append(elemExp)
                 else:
                     index = upperOut.index(elem)
-                    upperExpOut[index] += elemExp * exp
+                    upperExpOut[index] += elemExp
+                    
             for elem in low:
                 elem, elemExp = unit._removeExponentFromUnit(elem)
+                elemExp *= exp
                 if not elem in lowerOut:
                     lowerOut.append(elem)
-                    lowerExpOut.append(elemExp * exp)
+                    lowerExpOut.append(elemExp)
                 else:
                     index = lowerOut.index(elem)
-                    lowerExpOut[index] += elemExp * exp
-
-        upperPrefix = [None] * len(upperOut)
-        lowerPrefix = [None] * len(lowerOut)
+                    lowerExpOut[index] += elemExp
+        
         
         upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp = unit._cancleUnits(
-            upperOut, upperPrefix, upperExpOut, lowerOut, lowerPrefix, lowerExpOut
+            upperOut, [None] * len(upperOut), upperExpOut, lowerOut, [None] * len(lowerOut), lowerExpOut
         )
 
         return unit._combineUpperAndLower(upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp)
 
     def isCombinationUnit(self):
         if len(self.upper) > 1:
             return True
@@ -1069,15 +1077,15 @@
         newUnit = unit._formatUnit(newUnit)
 
         # get the upper, upperExp, lower and lowerExp of the newUnit without creating a unit
         otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp = self._getLists(newUnit)
 
         # determine if the SI bases are identical
         otherSIBase = self._getSIBaseUnit(otherUpper, otherUpperExp, otherLower, otherLowerExp)
-
+        
         if unit._assertEqualStatic(self._SIBaseUnit, otherSIBase) == False:
             raise ValueError(f'You tried to convert from {self} to {newUnit}. But these do not have the same base units')
         
         return self._getConverter(otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp)
 
     def getUnitWithoutPrefix(self):
         return self._removePrefixFromUnit(self.unitStr)[0]
@@ -1089,49 +1097,35 @@
         return knownUnits[u][1]
    
     def _getConverter(self, otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp):
         
         # initialize the scale and offset
         out = _unitConversion(1, 0)
 
-        # get conversions for all upper and lower units in self
-        upperConversions = [knownUnits[elem][1] for elem in self.upper]
-        lowerConversions = [knownUnits[elem][1] for elem in self.lower]
-
-        # modify the scale and offset using the conversions
-        conversions = upperConversions + lowerConversions
-        nUpper = len(upperConversions)
+        nUpper = len(self.upper)
+        units = self.upper + self.lower 
         prefixes = self.upperPrefix + self.lowerPrefix
         exponents = self.upperExp + self.lowerExp
-        for i, (conv, prefix, exp) in enumerate(zip(conversions, prefixes, exponents)):
-            if exp > 1: conv = conv ** exp
+        for i, (unit, prefix, exp) in enumerate(zip(units, prefixes, exponents)):
+            conv = knownUnits[unit][1]
             if not prefix is None:
                 conv *= knownPrefixes[prefix]
-            if i < nUpper:
-                out *= conv
-            else:
-                out /= conv
-                        
-        # get all conversions from the upper and lower units in the new unit
-        upperConversions = [knownUnits[elem][1] for elem in otherUpper]
-        lowerConversions = [knownUnits[elem][1] for elem in otherLower]
+            if exp > 1: conv = conv ** exp
+            out = out * conv if i < nUpper else out / conv
 
-        # modify the scale and offset based on the conversions
-        conversions = upperConversions + lowerConversions
         nUpper = len(otherUpper)
+        units = otherUpper + otherLower
         prefixes = otherUpperPrefix + otherLowerPrefix
         exponents = otherUpperExp + otherLowerExp
-        for i, (conv, prefix, exp) in enumerate(zip(conversions, prefixes, exponents)):
-            if exp > 1: conv = conv ** exp
+        for i, (unit, prefix, exp) in enumerate(zip(units, prefixes, exponents)):
+            conv = knownUnits[unit][1]
             if not prefix is None:
                 conv *= knownPrefixes[prefix]
-            if i < nUpper:
-                out /= conv
-            else:
-                out *= conv
+            if exp > 1: conv = conv ** exp
+            out = out / conv if i < nUpper else out * conv
 
         return out
 
     def convert(self, unitStr):
         if unitStr == '':
             unitStr = '1'
 
@@ -1144,14 +1138,7 @@
         # create the unit string
         self.unitStr = self._createUnitString()
 
         self._SIBaseUnit = self._getSIBaseUnit(self.upper, self.upperExp, self.lower, self.lowerExp)
         otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp = self._getLists(self._SIBaseUnit)
         self._converterToSI = self._getConverter(otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp)
 
-
-if __name__ == "__main__":
-    
-    print(unit('((s/m6)2)'))
-
-    
-
```

### Comparing `pyees-1.2.3/pyees/variable.py` & `pyees-1.2.4/pyees/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,15 +238,15 @@
             raise ValueError(f'You tried to set the covariance between {self} and {var} with a non scalar value')
         
         covUnit = unit(unitStr)
         selfVarUnit = unit(self._unitObject * var._unitObject)
         if not unit._assertEqualStatic(covUnit._SIBaseUnit, selfVarUnit._SIBaseUnit):
             raise ValueError(f'The covariance of {covariance} [{unitStr}] does not match the units of {self} and {var}')
         
-        covariance *=  self._converterToSI.convert(1, useOffset=False) * var._converterToSI.convert(1, useOffset=False)
+        covariance *= covUnit._converterToSI.convert(1, useOffset=False)
         
         self.covariance[var] = covariance        
         var.covariance[self] = covariance
         
     def _calculateUncertanty(self):
  
         # variance from each measurement
@@ -932,15 +932,15 @@
             case np.cos:
                 return self.cos()
             case np.tan:
                 return self.tan()
             case np.sqrt:
                 return self.sqrt()
         raise NotImplementedError()
-    
+        
     def min(self):
         index = np.argmin(self.value)
         return variable(self.value[index], self.unit, self.uncert[index])
 
     def max(self):
         index = np.argmax(self.value)
         return variable(self.value[index], self.unit, self.uncert[index])
@@ -1000,33 +1000,13 @@
     
     if isinstance(value, np.ndarray):
         return arrayVariable(value = value, unitStr = unit, uncert = uncert, nDigits = nDigits)
     else:
         return scalarVariable(value, unit, uncert, nDigits)
 
 
-if __name__ == "__main__":
-  
-    # value  
-    # [0.02994473968569557, 0.212143804427421, 1.8607179520279966]
-
-    # cov
-    # [[ 2.91453531e-06 -3.25319114e-04  7.98892818e-03]
-    #  [-3.25319114e-04  3.72796202e-02 -9.34366573e-01]
-    #  [ 7.98892818e-03 -9.34366573e-01  2.40059033e+01]]
 
-
-    b = variable(0.212143804427421, 'mbar-min/L', np.sqrt(3.72796202e-02))
-    c = variable(1.8607179520279966, 'mbar', np.sqrt(2.40059033e+01))
-    
-    b.addCovariance(c, -9.34366573e-01, 'mbar2-min/L')
-    
-    flow = variable(100,'L/min')
-    
-    dp = b*flow + c
-
-    print(dp)
-    
-    
+if __name__ == "__main__":
+    diameter = variable(40, 'cm')
+    area = np.pi / 4 * diameter ** 2
     
-
-## TODO major error - use sheet 1 in PS 2312-1: calculation flow1 - flow2. The covariance will create a negative varianace - and return an uncertanty of nan
+    print(area.value)
```

### Comparing `pyees-1.2.3/pyees.egg-info/PKG-INFO` & `pyees-1.2.4/pyees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.2.3
+Version: 1.2.4
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.2.3/setup.py` & `pyees-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.2.3',
+    version='1.2.4',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

