# Comparing `tmp/PySciMath-1.2.1.tar.gz` & `tmp/PySciMath-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySciMath-1.2.1.tar", last modified: Wed May 10 13:27:39 2023, max compression
+gzip compressed data, was "PySciMath-1.2.2.tar", last modified: Wed May 10 14:50:58 2023, max compression
```

## Comparing `PySciMath-1.2.1.tar` & `PySciMath-1.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 13:27:39.878052 PySciMath-1.2.1/
--rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2649 2023-05-10 13:27:39.877056 PySciMath-1.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 13:27:39.850127 PySciMath-1.2.1/PySciMath/
--rw-rw-rw-   0        0        0      431 2023-05-10 10:33:22.000000 PySciMath-1.2.1/PySciMath/Arithmetic.py
--rw-rw-rw-   0        0        0      591 2023-05-10 10:37:49.000000 PySciMath-1.2.1/PySciMath/ComplexNumbers.py
--rw-rw-rw-   0        0        0     4281 2023-05-10 10:38:03.000000 PySciMath-1.2.1/PySciMath/CoordinateGeometry.py
--rw-rw-rw-   0        0        0     2818 2023-05-10 09:50:00.000000 PySciMath-1.2.1/PySciMath/Geometry.py
--rw-rw-rw-   0        0        0     1350 2023-05-10 13:24:34.000000 PySciMath-1.2.1/PySciMath/Numbers.py
--rw-rw-rw-   0        0        0      568 2023-05-10 10:26:42.000000 PySciMath-1.2.1/PySciMath/Quadratic.py
--rw-rw-rw-   0        0        0     1392 2023-05-10 09:43:22.000000 PySciMath-1.2.1/PySciMath/Statistics.py
--rw-rw-rw-   0        0        0      558 2023-05-10 09:51:46.000000 PySciMath-1.2.1/PySciMath/Trigonometry.py
--rw-rw-rw-   0        0        0      637 2023-05-10 09:41:19.000000 PySciMath-1.2.1/PySciMath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:27:39.873066 PySciMath-1.2.1/PySciMath.egg-info/
--rw-rw-rw-   0        0        0     2649 2023-05-10 13:27:39.000000 PySciMath-1.2.1/PySciMath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-05-10 13:27:39.000000 PySciMath-1.2.1/PySciMath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 13:27:39.000000 PySciMath-1.2.1/PySciMath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 13:27:39.000000 PySciMath-1.2.1/PySciMath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2134 2023-05-10 13:24:03.000000 PySciMath-1.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 13:27:39.879048 PySciMath-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-05-10 13:23:30.000000 PySciMath-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:50:58.061936 PySciMath-1.2.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2643 2023-05-10 14:50:58.060938 PySciMath-1.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-10 14:50:58.040994 PySciMath-1.2.2/PySciMath/
+-rw-rw-rw-   0        0        0      431 2023-05-10 10:33:22.000000 PySciMath-1.2.2/PySciMath/Arithmetic.py
+-rw-rw-rw-   0        0        0      677 2023-05-10 14:22:10.000000 PySciMath-1.2.2/PySciMath/ComplexNumbers.py
+-rw-rw-rw-   0        0        0     4286 2023-05-10 14:05:32.000000 PySciMath-1.2.2/PySciMath/CoordinateGeometry.py
+-rw-rw-rw-   0        0        0     2870 2023-05-10 14:48:59.000000 PySciMath-1.2.2/PySciMath/Geometry.py
+-rw-rw-rw-   0        0        0     1350 2023-05-10 13:24:34.000000 PySciMath-1.2.2/PySciMath/Numbers.py
+-rw-rw-rw-   0        0        0      568 2023-05-10 10:26:42.000000 PySciMath-1.2.2/PySciMath/Quadratic.py
+-rw-rw-rw-   0        0        0     1392 2023-05-10 09:43:22.000000 PySciMath-1.2.2/PySciMath/Statistics.py
+-rw-rw-rw-   0        0        0      558 2023-05-10 09:51:46.000000 PySciMath-1.2.2/PySciMath/Trigonometry.py
+-rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.2.2/PySciMath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:50:58.055952 PySciMath-1.2.2/PySciMath.egg-info/
+-rw-rw-rw-   0        0        0     2643 2023-05-10 14:50:57.000000 PySciMath-1.2.2/PySciMath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-05-10 14:50:57.000000 PySciMath-1.2.2/PySciMath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 14:50:57.000000 PySciMath-1.2.2/PySciMath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 14:50:57.000000 PySciMath-1.2.2/PySciMath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2128 2023-05-10 14:24:31.000000 PySciMath-1.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 14:50:58.061936 PySciMath-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      903 2023-05-10 14:23:55.000000 PySciMath-1.2.2/setup.py
```

### Comparing `PySciMath-1.2.1/LICENSE.txt` & `PySciMath-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.1/PKG-INFO` & `PySciMath-1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.2.1
+Version: 1.2.2
 Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/pyscimath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Calculations
@@ -17,21 +17,21 @@
 
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
-**Name** - PySciMath </br>
-**Version** - 1.2.1 </br>
+**Name** - PySciMath</br>
+**Version** - 1.2.2</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
-**Author** - Aniketh Chavare </br>
-**Author's Email** - anikethchavare@gmail.com </br>
-**GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath) </br>
-**Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath) </br>
+**Author** - Aniketh Chavare</br>
+**Author's Email** - anikethchavare@gmail.com</br>
+**GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
+**Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
 
 MIT License
 
 Copyright (c) 2023 Aniketh Chavare
```

### Comparing `PySciMath-1.2.1/PySciMath/CoordinateGeometry.py` & `PySciMath-1.2.2/PySciMath/CoordinateGeometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 
             return distance
         else:
             raise Exception("Both tuples should be in the form (x₁, y₁) and (x₂, y₂) or (x₁, y₁, z₁) and (x₂, y₂, z₂).")
     else:
         raise TypeError("Both Point 1 and Point 2 should be in the form of a tuple.")
 
-# Function 2 - Collinear
-def collinear(point1, point2, point3):
+# Function 2 - Is Collinear
+def isCollinear(point1, point2, point3):
     isCollinear = False
 
     if (isinstance(point1, tuple) and isinstance(point2, tuple) and isinstance(point2, tuple)):
         if (len(point1) == 2 and len(point2) == 2 or len(point1) == 3 and len(point2) == 3):
             point1point2 = distance(point1, point2)
             point2point3 = distance(point2, point3)
             point1point3 = distance(point1, point3)
```

### Comparing `PySciMath-1.2.1/PySciMath/Geometry.py` & `PySciMath-1.2.2/PySciMath/Geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # PySciMath - Geometry
 
 ''' This is the "Geometry" sub-module. '''
 
 # Imports
 import math
 
+# Constants
+pi = 3.14159
+goldenRatio = 1.61803
+
 # Functions - Area
 def squareArea(side): return side * side
 def rectangleArea(length, width): return length * width
 def triangleArea(base, height): return 0.5 * base * height
 def circleArea(radius): return 3.14 * math.pow(radius, 2)
 def parallelogramArea(base, height): return base * height
 def trapeziumArea(base1, base2, height): return 0.5 * height * (base1 + base2)
```

### Comparing `PySciMath-1.2.1/PySciMath/Numbers.py` & `PySciMath-1.2.2/PySciMath/Numbers.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.1/PySciMath/Quadratic.py` & `PySciMath-1.2.2/PySciMath/Quadratic.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.1/PySciMath/Statistics.py` & `PySciMath-1.2.2/PySciMath/Statistics.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.1/PySciMath/Trigonometry.py` & `PySciMath-1.2.2/PySciMath/Trigonometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.1/PySciMath.egg-info/PKG-INFO` & `PySciMath-1.2.2/PySciMath.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.2.1
+Version: 1.2.2
 Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/pyscimath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Calculations
@@ -17,21 +17,21 @@
 
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
-**Name** - PySciMath </br>
-**Version** - 1.2.1 </br>
+**Name** - PySciMath</br>
+**Version** - 1.2.2</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
-**Author** - Aniketh Chavare </br>
-**Author's Email** - anikethchavare@gmail.com </br>
-**GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath) </br>
-**Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath) </br>
+**Author** - Aniketh Chavare</br>
+**Author's Email** - anikethchavare@gmail.com</br>
+**GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
+**Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
 
 MIT License
 
 Copyright (c) 2023 Aniketh Chavare
```

### Comparing `PySciMath-1.2.1/README.md` & `PySciMath-1.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
-**Name** - PySciMath </br>
-**Version** - 1.2.1 </br>
+**Name** - PySciMath</br>
+**Version** - 1.2.2</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
-**Author** - Aniketh Chavare </br>
-**Author's Email** - anikethchavare@gmail.com </br>
-**GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath) </br>
-**Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath) </br>
+**Author** - Aniketh Chavare</br>
+**Author's Email** - anikethchavare@gmail.com</br>
+**GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
+**Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
 
 MIT License
 
 Copyright (c) 2023 Aniketh Chavare
```

### Comparing `PySciMath-1.2.1/setup.py` & `PySciMath-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PySciMath",
-    version="1.2.1",
+    version="1.2.2",
     description="PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
```

