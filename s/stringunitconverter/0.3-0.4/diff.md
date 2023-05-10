# Comparing `tmp/stringunitconverter-0.3.tar.gz` & `tmp/stringunitconverter-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringunitconverter-0.3.tar", last modified: Sun Apr 30 23:46:12 2023, max compression
+gzip compressed data, was "stringunitconverter-0.4.tar", last modified: Wed May 10 22:30:42 2023, max compression
```

## Comparing `stringunitconverter-0.3.tar` & `stringunitconverter-0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-30 23:46:12.326774 stringunitconverter-0.3/
--rw-rw-r--   0 arend     (1000) arend     (1000)     1112 2023-02-07 21:57:17.000000 stringunitconverter-0.3/LICENSE.txt
--rw-rw-r--   0 arend     (1000) arend     (1000)     6011 2023-04-30 23:46:12.326774 stringunitconverter-0.3/PKG-INFO
--rw-rw-r--   0 arend     (1000) arend     (1000)     5157 2023-04-30 23:33:33.000000 stringunitconverter-0.3/README.md
--rw-rw-r--   0 arend     (1000) arend     (1000)       86 2022-03-13 18:39:33.000000 stringunitconverter-0.3/pyproject.toml
--rw-rw-r--   0 arend     (1000) arend     (1000)       38 2023-04-30 23:46:12.326774 stringunitconverter-0.3/setup.cfg
--rw-rw-r--   0 arend     (1000) arend     (1000)     1212 2023-04-30 23:43:42.000000 stringunitconverter-0.3/setup.py
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-30 23:46:12.322775 stringunitconverter-0.3/src/
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-30 23:46:12.322775 stringunitconverter-0.3/src/stringunitconverter/
--rw-rw-r--   0 arend     (1000) arend     (1000)       76 2022-03-13 20:47:38.000000 stringunitconverter-0.3/src/stringunitconverter/__init__.py
--rw-rw-r--   0 arend     (1000) arend     (1000)     3941 2023-02-07 21:46:45.000000 stringunitconverter-0.3/src/stringunitconverter/core.py
--rw-rw-r--   0 arend     (1000) arend     (1000)      273 2022-04-04 23:30:44.000000 stringunitconverter-0.3/src/stringunitconverter/prefixes.json
--rw-rw-r--   0 arend     (1000) arend     (1000)      608 2023-02-07 21:40:49.000000 stringunitconverter-0.3/src/stringunitconverter/units.json
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-30 23:46:12.326774 stringunitconverter-0.3/src/stringunitconverter.egg-info/
--rw-rw-r--   0 arend     (1000) arend     (1000)     6011 2023-04-30 23:46:12.000000 stringunitconverter-0.3/src/stringunitconverter.egg-info/PKG-INFO
--rw-rw-r--   0 arend     (1000) arend     (1000)      438 2023-04-30 23:46:12.000000 stringunitconverter-0.3/src/stringunitconverter.egg-info/SOURCES.txt
--rw-rw-r--   0 arend     (1000) arend     (1000)        1 2023-04-30 23:46:12.000000 stringunitconverter-0.3/src/stringunitconverter.egg-info/dependency_links.txt
--rw-rw-r--   0 arend     (1000) arend     (1000)       20 2023-04-30 23:46:12.000000 stringunitconverter-0.3/src/stringunitconverter.egg-info/requires.txt
--rw-rw-r--   0 arend     (1000) arend     (1000)       20 2023-04-30 23:46:12.000000 stringunitconverter-0.3/src/stringunitconverter.egg-info/top_level.txt
-drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-04-30 23:46:12.326774 stringunitconverter-0.3/tests/
--rw-rw-r--   0 arend     (1000) arend     (1000)     1718 2022-05-23 20:58:17.000000 stringunitconverter-0.3/tests/test_all.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-10 22:30:42.064736 stringunitconverter-0.4/
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1109 2023-05-10 21:18:11.000000 stringunitconverter-0.4/LICENSE.txt
+-rw-rw-r--   0 arend     (1000) arend     (1000)     5418 2023-05-10 22:30:42.064736 stringunitconverter-0.4/PKG-INFO
+-rw-rw-r--   0 arend     (1000) arend     (1000)     4520 2023-05-10 22:27:49.000000 stringunitconverter-0.4/README.md
+-rw-rw-r--   0 arend     (1000) arend     (1000)       86 2022-03-13 18:39:33.000000 stringunitconverter-0.4/pyproject.toml
+-rw-rw-r--   0 arend     (1000) arend     (1000)       38 2023-05-10 22:30:42.064736 stringunitconverter-0.4/setup.cfg
+-rw-rw-r--   0 arend     (1000) arend     (1000)     1255 2023-05-10 22:29:55.000000 stringunitconverter-0.4/setup.py
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-10 22:30:42.060736 stringunitconverter-0.4/src/
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-10 22:30:42.064736 stringunitconverter-0.4/src/stringunitconverter/
+-rw-rw-r--   0 arend     (1000) arend     (1000)       76 2022-03-13 20:47:38.000000 stringunitconverter-0.4/src/stringunitconverter/__init__.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)     6398 2023-05-10 22:18:52.000000 stringunitconverter-0.4/src/stringunitconverter/core.py
+-rw-rw-r--   0 arend     (1000) arend     (1000)      273 2022-04-04 23:30:44.000000 stringunitconverter-0.4/src/stringunitconverter/prefixes.json
+-rw-rw-r--   0 arend     (1000) arend     (1000)      608 2023-02-07 21:40:49.000000 stringunitconverter-0.4/src/stringunitconverter/units.json
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-10 22:30:42.064736 stringunitconverter-0.4/src/stringunitconverter.egg-info/
+-rw-rw-r--   0 arend     (1000) arend     (1000)     5418 2023-05-10 22:30:42.000000 stringunitconverter-0.4/src/stringunitconverter.egg-info/PKG-INFO
+-rw-rw-r--   0 arend     (1000) arend     (1000)      438 2023-05-10 22:30:42.000000 stringunitconverter-0.4/src/stringunitconverter.egg-info/SOURCES.txt
+-rw-rw-r--   0 arend     (1000) arend     (1000)        1 2023-05-10 22:30:42.000000 stringunitconverter-0.4/src/stringunitconverter.egg-info/dependency_links.txt
+-rw-rw-r--   0 arend     (1000) arend     (1000)       20 2023-05-10 22:30:42.000000 stringunitconverter-0.4/src/stringunitconverter.egg-info/requires.txt
+-rw-rw-r--   0 arend     (1000) arend     (1000)       20 2023-05-10 22:30:42.000000 stringunitconverter-0.4/src/stringunitconverter.egg-info/top_level.txt
+drwxrwxr-x   0 arend     (1000) arend     (1000)        0 2023-05-10 22:30:42.064736 stringunitconverter-0.4/tests/
+-rw-rw-r--   0 arend     (1000) arend     (1000)     2437 2023-05-10 22:11:09.000000 stringunitconverter-0.4/tests/test_all.py
```

### Comparing `stringunitconverter-0.3/LICENSE.txt` & `stringunitconverter-0.4/LICENSE.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright © 2023 Arne Baeyens <2arne.baeyens@gmail.com>
+Copyright © 2023 Arne Baeyens <mail@arnebaeyens.com>
 
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the “Software”), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
```

### Comparing `stringunitconverter-0.3/PKG-INFO` & `stringunitconverter-0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: stringunitconverter
-Version: 0.3
+Version: 0.4
 Summary: Unit converter: Returns multiplier for unit conversion, with units defined as strings.
 Home-page: https://gitlab.com/abaeyens/stringunitconverter
 Author: Arne Baeyens
 Author-email: mail@arnebaeyens.com
 Keywords: unit conversion,conversion
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
+Classifier: Topic :: Utilities
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # stringunitconverter
 [![PyPI version](https://badge.fury.io/py/stringunitconverter.svg)](https://badge.fury.io/py/stringunitconverter)
 ![coverage](https://gitlab.com/abaeyens/stringunitconverter/badges/master/coverage.svg)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![downloads](https://img.shields.io/pypi/dm/stringunitconverter)
 
 ## Goal
 Get the multiplication factor
 required to convert from one unit to another,
 with the units being given as strings.
 In short:
 make it easy to convert between units.
@@ -84,18 +87,31 @@
 - SI: g, N, s, Pa, bar, A, K, mol, Hz, J, W, C, V, Ohm, S, F, L, rad
 - Imperial: oz, psi, mi, ft, in, mil, mph
 - Nautical: (NM, nmi), (kn, kt)
 - other: mmHg, gf, (°, deg, degree)
 - also supported: %
 
 
-Functionality to easily add prefixes will be added in the future.
+## Functions and examples
+```python
+def add_unit(unit: str, multiplier: str)
 
+def add_json(filename: str, add_to_existing=False)
 
-## Examples
+def multiplier(a: str, b: str) -> float)
+
+def get_factor(a: str, unsafe=False) -> float)
+
+def unit_to_factor_string(a: str) -> str
+```
+
+For documentation of these functions:
+please see their help strings.
+
+Two usage examples:
 ```python3
 >>> import stringunitconverter as suc
 >>>
 >>> suc.multiplier('N/m^2', 'kN/cm^2')
 10.0
 >>> suc.multiplier('1/kPa', '1/(N/m^2)')
 0.001
@@ -130,43 +146,15 @@
     ```
 2. Navigate to the created directory.
     ```
     $ cd stringunitconverter
     ```
 
 
-### Create a local install
-A local install allows to try out the library locally.
-This can be useful during development.
-First, ensure that the project root directory is named `stringunitconverter`.
-Second, run in the project root directory:
-```
-$ python -m pip install -e .
-```
-This installs the package such that it is accessible
-like all other Python packages, e.g. using `import stringunitconverter`.
-The `-e` option denotes that it uses a symbolic link:
-code changes in the project directory (including branch switching)
-take effect at the first following `import`.
-No re-installation is required.
-
-Notes
-- `python` in the instruction above 
-should refer to Python 3.
-One may have to write `python3` to avoid using Python 2. 
-- There appear to be problems with this method on some Windows machines.
-- If it is desired to install several versions
-of the same package on a single system,
-for example a stable version from PyPi
-and a development version from a local install,
-it may be useful to use
-[Python virtual environments](https://docs.python.org/3/tutorial/venv.html).
-
-
 ## Contact
 Have a question, suggestion, ... ?
 Your feedback on this project is always appreciated!
-Send an email to
-[2arne.baeyens@gmail.com](mailto:2arne.baeyens@gmail.com).
+Send an e-mail to
+[mail@arnebaeyens.com](mailto:mail@arnebaeyens.com).
 
 It is also possible to use the [GitLab issues webpage](
   https://gitlab.com/abaeyens/stringunitconverter/-/issues).
```

### Comparing `stringunitconverter-0.3/README.md` & `stringunitconverter-0.4/src/stringunitconverter.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,34 @@
+Metadata-Version: 2.1
+Name: stringunitconverter
+Version: 0.4
+Summary: Unit converter: Returns multiplier for unit conversion, with units defined as strings.
+Home-page: https://gitlab.com/abaeyens/stringunitconverter
+Author: Arne Baeyens
+Author-email: mail@arnebaeyens.com
+Keywords: unit conversion,conversion
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Manufacturing
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
+Classifier: Topic :: Utilities
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # stringunitconverter
 [![PyPI version](https://badge.fury.io/py/stringunitconverter.svg)](https://badge.fury.io/py/stringunitconverter)
 ![coverage](https://gitlab.com/abaeyens/stringunitconverter/badges/master/coverage.svg)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![downloads](https://img.shields.io/pypi/dm/stringunitconverter)
 
 ## Goal
 Get the multiplication factor
 required to convert from one unit to another,
 with the units being given as strings.
 In short:
 make it easy to convert between units.
@@ -63,18 +87,31 @@
 - SI: g, N, s, Pa, bar, A, K, mol, Hz, J, W, C, V, Ohm, S, F, L, rad
 - Imperial: oz, psi, mi, ft, in, mil, mph
 - Nautical: (NM, nmi), (kn, kt)
 - other: mmHg, gf, (°, deg, degree)
 - also supported: %
 
 
-Functionality to easily add prefixes will be added in the future.
+## Functions and examples
+```python
+def add_unit(unit: str, multiplier: str)
+
+def add_json(filename: str, add_to_existing=False)
+
+def multiplier(a: str, b: str) -> float)
+
+def get_factor(a: str, unsafe=False) -> float)
+
+def unit_to_factor_string(a: str) -> str
+```
 
+For documentation of these functions:
+please see their help strings.
 
-## Examples
+Two usage examples:
 ```python3
 >>> import stringunitconverter as suc
 >>>
 >>> suc.multiplier('N/m^2', 'kN/cm^2')
 10.0
 >>> suc.multiplier('1/kPa', '1/(N/m^2)')
 0.001
@@ -109,43 +146,15 @@
     ```
 2. Navigate to the created directory.
     ```
     $ cd stringunitconverter
     ```
 
 
-### Create a local install
-A local install allows to try out the library locally.
-This can be useful during development.
-First, ensure that the project root directory is named `stringunitconverter`.
-Second, run in the project root directory:
-```
-$ python -m pip install -e .
-```
-This installs the package such that it is accessible
-like all other Python packages, e.g. using `import stringunitconverter`.
-The `-e` option denotes that it uses a symbolic link:
-code changes in the project directory (including branch switching)
-take effect at the first following `import`.
-No re-installation is required.
-
-Notes
-- `python` in the instruction above 
-should refer to Python 3.
-One may have to write `python3` to avoid using Python 2. 
-- There appear to be problems with this method on some Windows machines.
-- If it is desired to install several versions
-of the same package on a single system,
-for example a stable version from PyPi
-and a development version from a local install,
-it may be useful to use
-[Python virtual environments](https://docs.python.org/3/tutorial/venv.html).
-
-
 ## Contact
 Have a question, suggestion, ... ?
 Your feedback on this project is always appreciated!
-Send an email to
-[2arne.baeyens@gmail.com](mailto:2arne.baeyens@gmail.com).
+Send an e-mail to
+[mail@arnebaeyens.com](mailto:mail@arnebaeyens.com).
 
 It is also possible to use the [GitLab issues webpage](
   https://gitlab.com/abaeyens/stringunitconverter/-/issues).
```

### Comparing `stringunitconverter-0.3/setup.py` & `stringunitconverter-0.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="stringunitconverter",
-    version="0.3",
+    version="0.4",
     author="Arne Baeyens",
     author_email="mail@arnebaeyens.com",
     description="Unit converter: Returns multiplier for unit conversion, with units defined as strings.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/abaeyens/stringunitconverter",
     keywords='unit conversion, conversion',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     package_data={'': ['*.json']},
     install_requires=['importlib_resources',
                       ],
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Education",
         "Intended Audience :: Manufacturing",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)",
+        "Topic :: Utilities",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

### Comparing `stringunitconverter-0.3/src/stringunitconverter/core.py` & `stringunitconverter-0.4/src/stringunitconverter/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 2022, March 12
 """
 
 import importlib_resources as ir
 import json
+import math
+import warnings
 
 
 # Load JSON files in dictionaries for fast access
 # see https://importlib-resources.readthedocs.io/en/latest/using.html
 def getdict(filename: str) -> dict:
     source = ir.files('stringunitconverter').joinpath(filename)
     with ir.as_file(source) as filepath:
@@ -21,25 +23,90 @@
 
 operators_and_brackets = frozenset(('*', '/', '^', '-', '+', '(', ')', ' ',
                                     '·', '.'))
 digits = frozenset(('0', '1', '2', '3', '4', '5', '6', '7', '8', '9'))
 nonunits = operators_and_brackets.union(digits)
 
 
+def add_unit(unit: str, multiplier: str):
+    """Add a unit and its multiplier
+
+    For the parameter 'multiplier',
+    We want a string here because we substitute strings
+    and don't care about the actual mathematical value.
+
+    :param unit: base unit string, e.g. 'ft'
+    :param multiplier: corresponding multiplier, e.g. '0.3048'
+    """
+    # Check multiplier of correct type
+    if not isinstance(multiplier, str):
+        msg = f"The argument for parameter 'multiplier' must be " + \
+              f"of type str, not {type(multiplier)}."
+        raise ValueError(msg)
+    # Check whether unit isn't registered yet
+    if unit in units:
+        if units[unit] == multiplier:
+            msg = f'The unit {unit} is already present with the same multiplier.'
+            warnings.warn(msg, UserWarning, stacklevel=2)
+            return None
+        else:
+            msg = f'The unit {unit} is already present ' + \
+                  f'with the multiplier {units[unit]}, which differs from ' + \
+                  f'the given multiplier {multiplier}.'
+            raise Exception(msg)
+    # Ok, unit not yet preset => add it
+    else:
+        units[unit] = multiplier
+
+
+def add_json(filename: str, add_to_existing=False):
+    """Add JSON file with units and multipliers
+
+    Example of the used formatting:
+    ```
+    {
+      "oz": "0.02834952",
+      "gf": "9.80665e-6",
+      "ft": "0.3048"
+    }
+    ```
+
+    :param filename: filepath of the JSON file
+    :param add_to_existing: Whether to add the units to the already present
+                            ones (common ones will be overwritten), or to
+                            let them replace the already present ones.
+    """
+    units_new = getdict(filename)
+    units = units.update(units_new) if add_to_existing \
+        else units_new
+
+
 def multiplier(a: str, b: str, *args, **kwargs) -> float:
-    """
-    :param a: input unit
-    :param b: output unit
+    """Get float multiplier from two unitstrings
+
+    Multiplying the returned value with
+    a value of a quantity expressed in unit 'a'
+    gives the value of that quantity expressed in unit 'b'.
+    Any additional parameters are passed to ``get_factor``.
+
+    :param a: input unitstring
+    :param b: output unitstring
     :return: multiplier
     """
     return get_factor(a, *args, **kwargs) / get_factor(b, *args, **kwargs)
 
 
 def get_factor(a: str, unsafe=False) -> float:
-    """
+    """Get float multiplier to convert to base SI
+
+    Multiplying the returned value with
+    a value of a quantity expressed in unit 'a'
+    gives the value of that quantity expressed in
+    (a combinatione of) base SI units, i.e. g, N, m/s etc.
+
     :param a: input unit
     :param unsafe: set to 'True' to disable protection against malicious code
     :return: multiplier
     """
     # Replace each hat with two asterisks
     # and replace multiplication dot with asterisk
     # and replace ² and ³ with **2 and **3 respectively
@@ -85,24 +152,26 @@
             a = a[:ks] + '*' + a[ks+1:]
         # Move end index to start index
         ke = ks
     # Before evaluating the string, search for suspicious code,
     # unless unsafe mode has been enabled
     if unsafe is False:
         if 'import' in a or 'eval' in a:
-            raise Exception('The string may not contain "import" or "eval". ' +
-                            'Add argument "unsafe=True" to circumvent protection.')
+            msg = 'The string may not contain "import" or "eval". ' + \
+                  'Add argument "unsafe=True" to circumvent protection.'
+            raise Exception(msg)
     # Evaluate string
     a = eval(a)
     # Return outcome
     return a
 
 
 def unit_to_factor_string(a: str) -> str:
-    """
+    """single unit with prefix => multiplier string
+
     Convert string with a single unit and prefix, e.g. 'kPa',
     to its multiplier string, e.g. '(1e3*1)'.
 
     :param a: single unit
     :return: multiplier
     """
     # assume no prefix
@@ -111,12 +180,13 @@
     # doesn't work, so assume prefix and split it
     p = a[0]
     u = a[1:]
     if p in prefixes and u in units:
         return '(' + prefixes[p] + '*' + units[u] + ')'
     # neither of the two worked, so error out
     print('Failed to decode string: <' + a + '>')
+    # doesn't work either, so it's not a known unitstring
     return a
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `stringunitconverter-0.3/src/stringunitconverter/units.json` & `stringunitconverter-0.4/src/stringunitconverter/units.json`

 * *Files identical despite different names*

### Comparing `stringunitconverter-0.3/tests/test_all.py` & `stringunitconverter-0.4/tests/test_all.py`

 * *Files 25% similar despite different names*

```diff
@@ -49,16 +49,18 @@
 
 
 @pytest.mark.parametrize('test_input', [
     'import',
     'eval("10 + 10")',
 ])
 def test_get_factor_input_protection_01(test_input):
-    with pytest.raises(Exception):
+    with pytest.raises(Exception) as msg:
         _ = get_factor(test_input)
+    msg = str(msg.value)
+    assert 'unsafe=True' in msg
 
 
 @pytest.mark.parametrize('test_input, expected', [
     ('eval("10 + 10")', 20),
 ])
 def test_get_factor_input_protection_02(test_input, expected):
     assert get_factor(test_input, unsafe=True) == approx(expected)
@@ -69,7 +71,35 @@
     (('Pa', 'N/m^2'), 1),
     (('1/kPa', '1/(N/m^2)'), 1e-3),
     (('25 N·m', 'N·mm'), 25 * 1e3),
 ])
 def test_multiplier(test_input, expected):
     a, b = test_input
     assert multiplier(a, b) == approx(expected)
+
+
+def test_add_unit_01():
+    add_unit('foo', '123.456')
+    assert unit_to_factor_string('foo') == '123.456'
+
+
+def test_add_unit_02():
+    with pytest.raises(Exception) as msg:
+        add_unit('foo', 123.456)
+    msg = str(msg.value).lower()
+    assert 'parameter' in msg
+    assert 'multiplier' in msg
+    assert 'float' in msg
+    assert 'str' in msg
+
+
+def test_add_unit_03():
+    with pytest.raises(Exception) as msg:
+        add_unit('ft', '123')
+    msg = str(msg.value).lower()
+    assert 'unit' in msg
+    assert 'already present' in msg
+
+
+def test_add_unit_04():
+    with pytest.warns(match=r'same multiplier'):
+        add_unit('ft', '0.3048')
```

