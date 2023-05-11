# Comparing `tmp/unisci-1.6.0.tar.gz` & `tmp/unisci-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unisci-1.6.0.tar", last modified: Thu May 11 03:34:49 2023, max compression
+gzip compressed data, was "unisci-1.7.0.tar", last modified: Thu May 11 03:47:55 2023, max compression
```

## Comparing `unisci-1.6.0.tar` & `unisci-1.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-11 03:34:49.715493 unisci-1.6.0/
--rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.6.0/LICENSE
--rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.6.0/MANIFEST.in
--rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-11 03:34:49.715202 unisci-1.6.0/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)     1286 2023-04-28 05:01:19.000000 unisci-1.6.0/README.md
--rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-11 03:34:49.715582 unisci-1.6.0/setup.cfg
--rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-05-11 03:34:18.000000 unisci-1.6.0/setup.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-11 03:34:49.706079 unisci-1.6.0/unisci/
--rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-05-11 03:33:54.000000 unisci-1.6.0/unisci/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1503 2023-05-01 22:47:16.000000 unisci-1.6.0/unisci/_conversion_factors.py
--rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.6.0/unisci/_error.py
--rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.6.0/unisci/constants.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-11 03:34:49.708895 unisci-1.6.0/unisci/formulas/
--rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.6.0/unisci/formulas/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     2264 2023-04-30 22:55:51.000000 unisci-1.6.0/unisci/formulas/_validation.py
--rw-r--r--   0 vivaan     (501) staff       (20)    14458 2023-04-30 22:56:45.000000 unisci-1.6.0/unisci/formulas/chemistry.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1881 2023-05-09 23:31:16.000000 unisci-1.6.0/unisci/metric.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-11 03:34:49.713788 unisci-1.6.0/unisci/periodic/
--rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.6.0/unisci/periodic/periodic-table-lookup.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-05-03 23:47:40.000000 unisci-1.6.0/unisci/periodic/periodic-table-numbers.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.6.0/unisci/periodic/periodic-table-symbols.json
--rw-r--r--   0 vivaan     (501) staff       (20)    40292 2023-05-11 03:32:51.000000 unisci-1.6.0/unisci/types.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-11 03:34:49.707791 unisci-1.6.0/unisci.egg-info/
--rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-11 03:34:49.000000 unisci-1.6.0/unisci.egg-info/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)      525 2023-05-11 03:34:49.000000 unisci-1.6.0/unisci.egg-info/SOURCES.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-11 03:34:49.000000 unisci-1.6.0/unisci.egg-info/dependency_links.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-05-11 03:34:49.000000 unisci-1.6.0/unisci.egg-info/requires.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-05-11 03:34:49.000000 unisci-1.6.0/unisci.egg-info/top_level.txt
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-11 03:47:55.982802 unisci-1.7.0/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.7.0/LICENSE
+-rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.7.0/MANIFEST.in
+-rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-11 03:47:55.982518 unisci-1.7.0/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)     1286 2023-04-28 05:01:19.000000 unisci-1.7.0/README.md
+-rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-11 03:47:55.982895 unisci-1.7.0/setup.cfg
+-rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-05-11 03:44:19.000000 unisci-1.7.0/setup.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-11 03:47:55.978690 unisci-1.7.0/unisci/
+-rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-05-11 03:44:15.000000 unisci-1.7.0/unisci/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1503 2023-05-01 22:47:16.000000 unisci-1.7.0/unisci/_conversion_factors.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.7.0/unisci/_error.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.7.0/unisci/constants.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-11 03:47:55.980905 unisci-1.7.0/unisci/formulas/
+-rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.7.0/unisci/formulas/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     2264 2023-04-30 22:55:51.000000 unisci-1.7.0/unisci/formulas/_validation.py
+-rw-r--r--   0 vivaan     (501) staff       (20)    14458 2023-04-30 22:56:45.000000 unisci-1.7.0/unisci/formulas/chemistry.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1881 2023-05-09 23:31:16.000000 unisci-1.7.0/unisci/metric.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-11 03:47:55.982168 unisci-1.7.0/unisci/periodic/
+-rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.7.0/unisci/periodic/periodic-table-lookup.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-05-03 23:47:40.000000 unisci-1.7.0/unisci/periodic/periodic-table-numbers.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.7.0/unisci/periodic/periodic-table-symbols.json
+-rw-r--r--   0 vivaan     (501) staff       (20)    41095 2023-05-11 03:45:54.000000 unisci-1.7.0/unisci/types.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-11 03:47:55.980121 unisci-1.7.0/unisci.egg-info/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-11 03:47:55.000000 unisci-1.7.0/unisci.egg-info/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)      525 2023-05-11 03:47:55.000000 unisci-1.7.0/unisci.egg-info/SOURCES.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-11 03:47:55.000000 unisci-1.7.0/unisci.egg-info/dependency_links.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-05-11 03:47:55.000000 unisci-1.7.0/unisci.egg-info/requires.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-05-11 03:47:55.000000 unisci-1.7.0/unisci.egg-info/top_level.txt
```

### Comparing `unisci-1.6.0/LICENSE` & `unisci-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unisci-1.6.0/PKG-INFO` & `unisci-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.6.0
+Version: 1.7.0
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `unisci-1.6.0/README.md` & `unisci-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `unisci-1.6.0/setup.py` & `unisci-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.readlines()
 
 setup(
     name='unisci',
-    version='1.6.0',
+    version='1.7.0',
     author='Vivaan Singhvi',
     author_email='singhvi.vivaan@gmail.com',
     description='Units Conversions, and Science Package',
     long_description=description,
     long_description_content_type="text/markdown",
     license='MIT',
     packages=find_packages(),
```

### Comparing `unisci-1.6.0/unisci/_conversion_factors.py` & `unisci-1.7.0/unisci/_conversion_factors.py`

 * *Files identical despite different names*

### Comparing `unisci-1.6.0/unisci/_error.py` & `unisci-1.7.0/unisci/_error.py`

 * *Files identical despite different names*

### Comparing `unisci-1.6.0/unisci/formulas/_validation.py` & `unisci-1.7.0/unisci/formulas/_validation.py`

 * *Files identical despite different names*

### Comparing `unisci-1.6.0/unisci/formulas/chemistry.py` & `unisci-1.7.0/unisci/formulas/chemistry.py`

 * *Files identical despite different names*

### Comparing `unisci-1.6.0/unisci/metric.py` & `unisci-1.7.0/unisci/metric.py`

 * *Files identical despite different names*

### Comparing `unisci-1.6.0/unisci/periodic/periodic-table-lookup.json` & `unisci-1.7.0/unisci/periodic/periodic-table-lookup.json`

 * *Files identical despite different names*

### Comparing `unisci-1.6.0/unisci/periodic/periodic-table-numbers.json` & `unisci-1.7.0/unisci/periodic/periodic-table-numbers.json`

 * *Files identical despite different names*

### Comparing `unisci-1.6.0/unisci/periodic/periodic-table-symbols.json` & `unisci-1.7.0/unisci/periodic/periodic-table-symbols.json`

 * *Files identical despite different names*

### Comparing `unisci-1.6.0/unisci/types.py` & `unisci-1.7.0/unisci/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,14 +330,39 @@
         # performs <power> self multiplications
         output = self.__copy__()
         for _ in range(1, power):
             output = output * self
 
         return output
 
+    def __eq__(self, other: Quantity) -> bool:
+
+        """
+        Checks equality between one Quantity and another.
+
+        Arguments: The self and another Quantity.
+
+        Raises: UnsupportedError for anything other than a Quantity.
+
+        Returns: A boolean signifying equality to a certain precision.
+        """
+
+        if not isinstance(other, Quantity):
+            raise UnsupportedError("Quantities can only be tested for equality with other Quantities.")
+        
+        temp = Quantity.auto_format
+        Quantity.set_auto_format(False)
+        
+        try:
+            other = other.to_base_units().converted(list(self.unit_type.keys()))
+            self_temp = self.to_base_units()
+            return abs(other.number - self_temp.number) < 10**-(Quantity.precision*2) and other.unit_type == self_temp.unit_type
+        finally:
+            Quantity.set_auto_format(temp)
+
     def __rm_zeroes(self):
         
         """
         Removes all units that are to the power of 0.
         """
 
         for key in list(self.unit_type.keys()):
@@ -935,52 +960,52 @@
 
     # loads symbols and numbers
     with open(f"{Path(__file__).parent}/periodic/periodic-table-symbols.json", "r") as f:
         _SYMBOL_TO_NAME = json.load(f)
     with open(f"{Path(__file__).parent}/periodic/periodic-table-numbers.json") as f:
         _NUMBER_TO_NAME = json.load(f)
 
-    def __init__(self, element_symbol: str = None, element_name: str = None, element_number: int = None) -> Element:
+    def __init__(self, symbol: str = None, name: str = None, atomic_number: int = None) -> Element:
 
         """
         Arguments: EITHER a symbol OR a name for the element. 
 
         Raises: ArgumentError for when both or neither the symbol and name are given.
         NameError for incorrect symbol or name.
 
         Returns: a new Element
         """
 
-        if [element_symbol, element_name, element_number].count(None) != 2:
+        if [symbol, name, atomic_number].count(None) != 2:
             raise ArgumentError("You must enter only one of the folloing: a name, symbol, or number.")
 
         # obtain json data for the element
         with open(f"{Path(__file__).parent}/periodic/periodic-table-lookup.json", "r") as f:
             table = json.load(f)
             try:
-                if element_name:
-                    self.information = table[element_name.lower().replace('aluminum', 'aluminium')]  # format name to lowercase: "Hydrogen" -> "hydrogen"
-                elif element_number: 
-                    self.information = table[Element._NUMBER_TO_NAME[str(element_number)]]
-                elif element_symbol:
-                    self.information = table[Element._SYMBOL_TO_NAME[element_symbol]]
+                if name:
+                    self.information = table[name.lower().replace('aluminum', 'aluminium')]  # format name to lowercase: "Hydrogen" -> "hydrogen"
+                elif atomic_number: 
+                    self.information = table[Element._NUMBER_TO_NAME[str(atomic_number)]]
+                elif symbol:
+                    self.information = table[Element._SYMBOL_TO_NAME[symbol]]
             except:
                 raise ArgumentError("Invalid information given. Check your spelling.")
             
     def __str__(self) -> str:
         """
         Returns the element symbol.
         """
         return self.symbol
     
     def __repr__(self) -> str:
         """
         Returns the element as it would be constructed.
         """
-        return f"Element(element_symbol='{self.symbol}')"
+        return f"Element(symbol='{self.symbol}')"
 
     """
     Below are several properties of the element, returned via information lookup.
     """     
 
     @property
     def name(self) -> str:
@@ -1101,22 +1126,22 @@
         
         return configs
     
     @property
     def noble_gas_config(self) -> dict:
         """
         Returns a dictionary containing the noble gas and the configuration. 
-        Example: {'gas': Element(element_symbol="He"), 'configuration': {'2s': 2, '2p': 4}}
+        Example: {'gas': Element(symbol="He"), 'configuration': {'2s': 2, '2p': 4}}
         """
         config_split = self.noble_gas_config_str.split()
         configs = {}
 
         # gets the gas
         noble_symbol = config_split[0][1:-1]   # remove []
-        noble_gas = Element(element_symbol=noble_symbol)
+        noble_gas = Element(symbol=noble_symbol)
 
         # gets reset of configurations
         list_configs  = config_split[1::]
         for config in list_configs:
             configs[config[:2:]] = int(config[2::])
 
         return {'gas': noble_gas, 'configuration': configs}
```

### Comparing `unisci-1.6.0/unisci.egg-info/PKG-INFO` & `unisci-1.7.0/unisci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.6.0
+Version: 1.7.0
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `unisci-1.6.0/unisci.egg-info/SOURCES.txt` & `unisci-1.7.0/unisci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

