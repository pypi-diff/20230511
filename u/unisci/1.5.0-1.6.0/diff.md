# Comparing `tmp/unisci-1.5.0.tar.gz` & `tmp/unisci-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unisci-1.5.0.tar", last modified: Wed May 10 02:20:04 2023, max compression
+gzip compressed data, was "unisci-1.6.0.tar", last modified: Thu May 11 03:34:49 2023, max compression
```

## Comparing `unisci-1.5.0.tar` & `unisci-1.6.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-10 02:20:04.080374 unisci-1.5.0/
--rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.5.0/LICENSE
--rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.5.0/MANIFEST.in
--rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-10 02:20:04.079946 unisci-1.5.0/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)     1286 2023-04-28 05:01:19.000000 unisci-1.5.0/README.md
--rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-10 02:20:04.080481 unisci-1.5.0/setup.cfg
--rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-05-10 02:18:12.000000 unisci-1.5.0/setup.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-10 02:20:04.073398 unisci-1.5.0/unisci/
--rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-05-10 02:18:07.000000 unisci-1.5.0/unisci/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1503 2023-05-01 22:47:16.000000 unisci-1.5.0/unisci/_conversion_factors.py
--rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.5.0/unisci/_error.py
--rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.5.0/unisci/constants.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-10 02:20:04.076481 unisci-1.5.0/unisci/formulas/
--rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.5.0/unisci/formulas/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     2264 2023-04-30 22:55:51.000000 unisci-1.5.0/unisci/formulas/_validation.py
--rw-r--r--   0 vivaan     (501) staff       (20)    14458 2023-04-30 22:56:45.000000 unisci-1.5.0/unisci/formulas/chemistry.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1881 2023-05-09 23:31:16.000000 unisci-1.5.0/unisci/metric.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-10 02:20:04.079304 unisci-1.5.0/unisci/periodic/
--rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.5.0/unisci/periodic/periodic-table-lookup.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-05-03 23:47:40.000000 unisci-1.5.0/unisci/periodic/periodic-table-numbers.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.5.0/unisci/periodic/periodic-table-symbols.json
--rw-r--r--   0 vivaan     (501) staff       (20)    39894 2023-05-10 02:15:41.000000 unisci-1.5.0/unisci/types.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-10 02:20:04.075215 unisci-1.5.0/unisci.egg-info/
--rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-10 02:20:04.000000 unisci-1.5.0/unisci.egg-info/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)      525 2023-05-10 02:20:04.000000 unisci-1.5.0/unisci.egg-info/SOURCES.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-10 02:20:04.000000 unisci-1.5.0/unisci.egg-info/dependency_links.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-05-10 02:20:04.000000 unisci-1.5.0/unisci.egg-info/requires.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-05-10 02:20:04.000000 unisci-1.5.0/unisci.egg-info/top_level.txt
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-11 03:34:49.715493 unisci-1.6.0/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.6.0/LICENSE
+-rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.6.0/MANIFEST.in
+-rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-11 03:34:49.715202 unisci-1.6.0/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)     1286 2023-04-28 05:01:19.000000 unisci-1.6.0/README.md
+-rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-11 03:34:49.715582 unisci-1.6.0/setup.cfg
+-rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-05-11 03:34:18.000000 unisci-1.6.0/setup.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-11 03:34:49.706079 unisci-1.6.0/unisci/
+-rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-05-11 03:33:54.000000 unisci-1.6.0/unisci/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1503 2023-05-01 22:47:16.000000 unisci-1.6.0/unisci/_conversion_factors.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.6.0/unisci/_error.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.6.0/unisci/constants.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-11 03:34:49.708895 unisci-1.6.0/unisci/formulas/
+-rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.6.0/unisci/formulas/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     2264 2023-04-30 22:55:51.000000 unisci-1.6.0/unisci/formulas/_validation.py
+-rw-r--r--   0 vivaan     (501) staff       (20)    14458 2023-04-30 22:56:45.000000 unisci-1.6.0/unisci/formulas/chemistry.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1881 2023-05-09 23:31:16.000000 unisci-1.6.0/unisci/metric.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-11 03:34:49.713788 unisci-1.6.0/unisci/periodic/
+-rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.6.0/unisci/periodic/periodic-table-lookup.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-05-03 23:47:40.000000 unisci-1.6.0/unisci/periodic/periodic-table-numbers.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.6.0/unisci/periodic/periodic-table-symbols.json
+-rw-r--r--   0 vivaan     (501) staff       (20)    40292 2023-05-11 03:32:51.000000 unisci-1.6.0/unisci/types.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-11 03:34:49.707791 unisci-1.6.0/unisci.egg-info/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-11 03:34:49.000000 unisci-1.6.0/unisci.egg-info/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)      525 2023-05-11 03:34:49.000000 unisci-1.6.0/unisci.egg-info/SOURCES.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-11 03:34:49.000000 unisci-1.6.0/unisci.egg-info/dependency_links.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-05-11 03:34:49.000000 unisci-1.6.0/unisci.egg-info/requires.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-05-11 03:34:49.000000 unisci-1.6.0/unisci.egg-info/top_level.txt
```

### Comparing `unisci-1.5.0/LICENSE` & `unisci-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unisci-1.5.0/PKG-INFO` & `unisci-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.5.0
+Version: 1.6.0
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `unisci-1.5.0/README.md` & `unisci-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `unisci-1.5.0/setup.py` & `unisci-1.6.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.readlines()
 
 setup(
     name='unisci',
-    version='1.5.0',
+    version='1.6.0',
     author='Vivaan Singhvi',
     author_email='singhvi.vivaan@gmail.com',
     description='Units Conversions, and Science Package',
     long_description=description,
     long_description_content_type="text/markdown",
     license='MIT',
     packages=find_packages(),
```

### Comparing `unisci-1.5.0/unisci/_conversion_factors.py` & `unisci-1.6.0/unisci/_conversion_factors.py`

 * *Files identical despite different names*

### Comparing `unisci-1.5.0/unisci/_error.py` & `unisci-1.6.0/unisci/_error.py`

 * *Files identical despite different names*

### Comparing `unisci-1.5.0/unisci/formulas/_validation.py` & `unisci-1.6.0/unisci/formulas/_validation.py`

 * *Files identical despite different names*

### Comparing `unisci-1.5.0/unisci/formulas/chemistry.py` & `unisci-1.6.0/unisci/formulas/chemistry.py`

 * *Files identical despite different names*

### Comparing `unisci-1.5.0/unisci/metric.py` & `unisci-1.6.0/unisci/metric.py`

 * *Files identical despite different names*

### Comparing `unisci-1.5.0/unisci/periodic/periodic-table-lookup.json` & `unisci-1.6.0/unisci/periodic/periodic-table-lookup.json`

 * *Files identical despite different names*

### Comparing `unisci-1.5.0/unisci/periodic/periodic-table-numbers.json` & `unisci-1.6.0/unisci/periodic/periodic-table-numbers.json`

 * *Files identical despite different names*

### Comparing `unisci-1.5.0/unisci/periodic/periodic-table-symbols.json` & `unisci-1.6.0/unisci/periodic/periodic-table-symbols.json`

 * *Files identical despite different names*

### Comparing `unisci-1.5.0/unisci/types.py` & `unisci-1.6.0/unisci/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -802,58 +802,56 @@
 
         """
         Performs multiplcation as defined in __mul__().
         """
 
         return self * other
     
-    def __add__(self, other: Temperature) -> Temperature:
+    def __add__(self, other: Quantity | Temperature) -> Temperature:
 
         """
+        Takes the second argument as an absolute increase in temperature, which is added to the first temperature.
+
         Arguments: Another temperature object to add to self.
 
         Raises: TypeError for wrong types (anything other than Temperature).
 
         Returns: A new Temperature object - the sum.
         """
 
+        # detects for a Quantity being added
+        if isinstance(other, Quantity):
+            other = other.converted_temperature(target='K')
+            if other.units != {'K': 1}:
+                raise TypeError("Incorrect types for addition with a temperature.")
+            return Temperature(self.number + other.converted_temperature(target=self.type).number, self.type)
+
         # detects for incorrect type
         if not isinstance(other, Temperature):
             raise TypeError("Only Temperature objects can be added to Temperatre objects.")
 
         # converts other to the same type and then returns
         return Temperature(self.number + CONVERT_TO_KELVIN[other.type] / CONVERT_TO_KELVIN[self.type] * other.number, self.type)
     
-    def __radd__(self, other: Temperature) -> Temperature:
+    def __sub__(self, other: Temperature) -> Quantity:
 
         """
-        Simply reversed addition. See __add__() for more information.
-        """
+        Determines the absolute temperature difference between the two Temperatures.
 
-        return other + self
-    
-    def __sub__(self, other: Temperature) -> Temperature:
-
-        """
         Arguments: Another temperature object to subtract from self.
 
         Raises: TypeError for wrong types (anything other than Temperature).
 
-        Returns: A new Temperature object - the difference.
-        """
-
-        return self + (-1 * other)
-    
-    def __rsub__(self, other: Temperature) -> Temperature:
-
-        """
-        Back-up method for subtracting. See __sub__() for more information.
+        Returns: A new Quantity object - the difference.
         """
+        
+        if not isinstance(other, Temperature):
+            raise UnsupportedError("Unsupported type for temperature subtraction.")
 
-        return other + (-1 * self)
+        return Quantity(self.number - other.converted(target=self.type).value, {self.type: 1})
     
     def __pow__(self, power: int) -> UnsupportedError:
 
         """
         Raises UnsupportedError, because Temperature do not support being multiplied by other units.
         """
```

### Comparing `unisci-1.5.0/unisci.egg-info/PKG-INFO` & `unisci-1.6.0/unisci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.5.0
+Version: 1.6.0
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `unisci-1.5.0/unisci.egg-info/SOURCES.txt` & `unisci-1.6.0/unisci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

