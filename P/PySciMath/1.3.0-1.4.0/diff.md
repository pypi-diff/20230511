# Comparing `tmp/PySciMath-1.3.0.tar.gz` & `tmp/PySciMath-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySciMath-1.3.0.tar", last modified: Thu May 11 07:39:58 2023, max compression
+gzip compressed data, was "PySciMath-1.4.0.tar", last modified: Thu May 11 15:16:27 2023, max compression
```

## Comparing `PySciMath-1.3.0.tar` & `PySciMath-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 07:39:58.373470 PySciMath-1.3.0/
--rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2643 2023-05-11 07:39:58.363495 PySciMath-1.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-11 07:39:58.297670 PySciMath-1.3.0/PySciMath/
--rw-rw-rw-   0        0        0      431 2023-05-10 10:33:22.000000 PySciMath-1.3.0/PySciMath/Arithmetic.py
--rw-rw-rw-   0        0        0      677 2023-05-10 14:22:10.000000 PySciMath-1.3.0/PySciMath/ComplexNumbers.py
--rw-rw-rw-   0        0        0     4286 2023-05-10 14:05:32.000000 PySciMath-1.3.0/PySciMath/CoordinateGeometry.py
--rw-rw-rw-   0        0        0    17238 2023-05-11 07:37:25.000000 PySciMath-1.3.0/PySciMath/Geometry.py
--rw-rw-rw-   0        0        0     1350 2023-05-10 13:24:34.000000 PySciMath-1.3.0/PySciMath/Numbers.py
--rw-rw-rw-   0        0        0      568 2023-05-10 10:26:42.000000 PySciMath-1.3.0/PySciMath/Quadratic.py
--rw-rw-rw-   0        0        0     1392 2023-05-10 09:43:22.000000 PySciMath-1.3.0/PySciMath/Statistics.py
--rw-rw-rw-   0        0        0      558 2023-05-10 09:51:46.000000 PySciMath-1.3.0/PySciMath/Trigonometry.py
--rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.3.0/PySciMath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 07:39:58.332578 PySciMath-1.3.0/PySciMath.egg-info/
--rw-rw-rw-   0        0        0     2643 2023-05-11 07:39:57.000000 PySciMath-1.3.0/PySciMath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-05-11 07:39:57.000000 PySciMath-1.3.0/PySciMath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 07:39:57.000000 PySciMath-1.3.0/PySciMath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-11 07:39:57.000000 PySciMath-1.3.0/PySciMath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2128 2023-05-11 07:38:28.000000 PySciMath-1.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-11 07:39:58.373470 PySciMath-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-05-11 07:38:16.000000 PySciMath-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:16:27.752609 PySciMath-1.4.0/
+-rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2643 2023-05-11 15:16:27.751612 PySciMath-1.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-11 15:16:27.735654 PySciMath-1.4.0/PySciMath/
+-rw-rw-rw-   0        0        0     1720 2023-05-11 15:05:50.000000 PySciMath-1.4.0/PySciMath/Arithmetic.py
+-rw-rw-rw-   0        0        0      677 2023-05-10 14:22:10.000000 PySciMath-1.4.0/PySciMath/ComplexNumbers.py
+-rw-rw-rw-   0        0        0     4286 2023-05-10 14:05:32.000000 PySciMath-1.4.0/PySciMath/CoordinateGeometry.py
+-rw-rw-rw-   0        0        0    17742 2023-05-11 15:13:15.000000 PySciMath-1.4.0/PySciMath/Geometry.py
+-rw-rw-rw-   0        0        0      568 2023-05-10 10:26:42.000000 PySciMath-1.4.0/PySciMath/Quadratic.py
+-rw-rw-rw-   0        0        0     1272 2023-05-11 15:14:07.000000 PySciMath-1.4.0/PySciMath/Statistics.py
+-rw-rw-rw-   0        0        0      558 2023-05-10 09:51:46.000000 PySciMath-1.4.0/PySciMath/Trigonometry.py
+-rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.4.0/PySciMath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:16:27.747622 PySciMath-1.4.0/PySciMath.egg-info/
+-rw-rw-rw-   0        0        0     2643 2023-05-11 15:16:27.000000 PySciMath-1.4.0/PySciMath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2023-05-11 15:16:27.000000 PySciMath-1.4.0/PySciMath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 15:16:27.000000 PySciMath-1.4.0/PySciMath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 15:16:27.000000 PySciMath-1.4.0/PySciMath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2128 2023-05-11 15:14:59.000000 PySciMath-1.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-11 15:16:27.752609 PySciMath-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      903 2023-05-11 15:14:54.000000 PySciMath-1.4.0/setup.py
```

### Comparing `PySciMath-1.3.0/LICENSE.txt` & `PySciMath-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySciMath-1.3.0/PKG-INFO` & `PySciMath-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.3.0
+Version: 1.4.0
 Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/pyscimath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Calculations
@@ -18,15 +18,15 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.3.0</br>
+**Version** - 1.4.0</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **Author's Email** - anikethchavare@gmail.com</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
```

### Comparing `PySciMath-1.3.0/PySciMath/ComplexNumbers.py` & `PySciMath-1.4.0/PySciMath/ComplexNumbers.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.3.0/PySciMath/CoordinateGeometry.py` & `PySciMath-1.4.0/PySciMath/CoordinateGeometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.3.0/PySciMath/Geometry.py` & `PySciMath-1.4.0/PySciMath/Geometry.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,66 +19,66 @@
 
     if ("shape" in keyList):
         if (kwargs["shape"] in shapeList):
             shape = kwargs["shape"]
 
             if (shape == "square"): # Square
                 if ("side" in keyList):
-                    if (isinstance(kwargs["side"], int)):
+                    if (isinstance(kwargs["side"], (int, float))):
                         return kwargs["side"] * kwargs["side"]
                     else:
-                        raise Exception("The 'side' argument should be an integer.")
+                        raise Exception("The 'side' argument should be an integer or float.")
                 else:
                     raise Exception("To check the area of a square, the 'side' argument should be present.")
             elif (shape == "rectangle"): # Rectangle
                 if ("length" in keyList and "width" in keyList):
-                    if (isinstance(kwargs["length"], int) and isinstance(kwargs["width"], int)):
+                    if (isinstance(kwargs["length"], (int, float)) and isinstance(kwargs["width"], (int, float))):
                         return kwargs["length"] * kwargs["width"]
                     else:
-                        raise Exception("The 'length' and 'width' arguments should be an integer.")
+                        raise Exception("The 'length' and 'width' arguments should be an integer or float.")
                 else:
                     raise Exception("To check the area of a rectangle, the 'length' and 'width' arguments should be present.")
             elif (shape == "triangle"): # Triangle
                 if ("base" in keyList and "height" in keyList):
-                    if (isinstance(kwargs["base"], int) and isinstance(kwargs["height"], int)):
+                    if (isinstance(kwargs["base"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         return 0.5 * kwargs["base"] * kwargs["height"]
                     else:
-                        raise Exception("The 'base' and 'height' arguments should be an integer.")
+                        raise Exception("The 'base' and 'height' arguments should be an integer or float.")
                 else:
                     raise Exception("To check the area of a triangle, the 'base' and 'height' arguments should be present.")
             elif (shape == "circle"): # Circle
                 if ("radius" in keyList):
-                    if (isinstance(kwargs["radius"], int)):
+                    if (isinstance(kwargs["radius"], (int, float))):
                         return 3.14 * math.pow(kwargs["radius"], 2)
                     else:
-                        raise Exception("The 'radius' argument should be an integer.")
+                        raise Exception("The 'radius' argument should be an integer or float.")
                 else:
                     raise Exception("To check the area of a circle, the 'radius' argument should be present.")
             elif (shape == "parallelogram"): # Parallelogram
                 if ("base" in keyList and "height" in keyList):
-                    if (isinstance(kwargs["base"], int) and isinstance(kwargs["height"], int)):
+                    if (isinstance(kwargs["base"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         return kwargs["base"] * kwargs["height"]
                     else:
-                        raise Exception("The 'base' and 'height' arguments should be an integer.")
+                        raise Exception("The 'base' and 'height' arguments should be an integer or float.")
                 else:
                     raise Exception("To check the area of a parallelogram, the 'base' and 'height' arguments should be present.")
             elif (shape == "trapezium"): # Trapezium
                 if ("base1" in keyList and "base2" in keyList and "height" in keyList):
-                    if (isinstance(kwargs["base1"], int) and isinstance(kwargs["base2"], int) and isinstance(kwargs["height"], int)):
+                    if (isinstance(kwargs["base1"], (int, float)) and isinstance(kwargs["base2"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         return 0.5 * kwargs["height"] * (kwargs["base1"] + kwargs["base2"])
                     else:
-                        raise Exception("The 'base1', 'base2', and 'height' arguments should be an integer.")
+                        raise Exception("The 'base1', 'base2', and 'height' arguments should be an integer or float.")
                 else:
                     raise Exception("To check the area of a trapezium, the 'base1', 'base2', and 'height' arguments should be present.")
             elif (shape == "rhombus"): # Rhombus
                 if ("diagonal1" in keyList and "diagonal2" in keyList):
-                    if (isinstance(kwargs["diagonal1"], int) and isinstance(kwargs["diagonal2"], int)):
+                    if (isinstance(kwargs["diagonal1"], (int, float)) and isinstance(kwargs["diagonal2"], (int, float))):
                         return (kwargs["diagonal1"] * kwargs["diagonal2"]) / 2
                     else:
-                        raise Exception("The 'diagonal' and 'diagonal2' arguments should be an integer.")
+                        raise Exception("The 'diagonal' and 'diagonal2' arguments should be an integer or float.")
                 else:
                     raise Exception("To check the area of a rhombus, the 'diagonal1' and 'diagonal2' arguments should be present.")
         else:
             raise Exception("The 'shape' argument should be a square, rectangle, triangle, circle, parallelogram, trapezium, or rhombus.")
     else:
         raise Exception("The 'shape' argument should be present in this function.")
 
@@ -92,66 +92,66 @@
 
     if ("shape" in keyList):
         if (kwargs["shape"] in shapeList):
             shape = kwargs["shape"]
 
             if (shape == "cube"): # Cube
                 if ("side" in keyList):
-                    if (isinstance(kwargs["side"], int)):
+                    if (isinstance(kwargs["side"], (int, float))):
                         return math.pow(kwargs["side"], 3)
                     else:
-                        raise Exception("The 'side' argument should be an integer.")
+                        raise Exception("The 'side' argument should be an integer or float.")
                 else:
                     raise Exception("To check the volume of a cube, the 'side' argument should be present.")
             elif (shape == "cuboid"): # Cuboid
                 if ("length" in keyList and "width" in keyList and "height" in keyList):
-                    if (isinstance(kwargs["length"], int) and isinstance(kwargs["width"], int) and isinstance(kwargs["height"], int)):
+                    if (isinstance(kwargs["length"], (int, float)) and isinstance(kwargs["width"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         return kwargs["length"] * kwargs["width"] * kwargs["height"]
                     else:
-                        raise Exception("The 'length', 'width', and 'height' arguments should be an integer.")
+                        raise Exception("The 'length', 'width', and 'height' arguments should be an integer or float.")
                 else:
                     raise Exception("To check the volume of a cuboid, the 'length', 'width', and 'height' arguments should be present.")
             elif (shape == "cone"): # Cone
                 if ("raidus" in keyList and "height" in keyList):
-                    if (isinstance(kwargs["radius"], int) and isinstance(kwargs["height"], int)):
+                    if (isinstance(kwargs["radius"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         return (1/3) * 3.14 * math.pow(kwargs["radius"], 2) * kwargs["height"]
                     else:
-                        raise Exception("The 'radius' and 'height' arguments should be an integer.")
+                        raise Exception("The 'radius' and 'height' arguments should be an integer or float.")
                 else:
                     raise Exception("To check the volume of a cone, the 'radius' and 'height' arguments should be present.")
             elif (shape == "cylinder"): # Cylinder
                 if ("radius" in keyList and "height" in keyList):
-                    if (isinstance(kwargs["radius"], int) and isinstance(kwargs["height"], int)):
+                    if (isinstance(kwargs["radius"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         return 3.14 * math.pow(kwargs["radius"], 2) * kwargs["height"]
                     else:
-                        raise Exception("The 'radius' and 'height' arguments should be an integer.")
+                        raise Exception("The 'radius' and 'height' arguments should be an integer or float.")
                 else:
                     raise Exception("To check the volume of a cylinder, the 'radius' and 'height' arguments should be present.")
             elif (shape == "sphere"): # Sphere
                 if ("radius" in keyList):
-                    if (isinstance(kwargs["radius"], int)):
+                    if (isinstance(kwargs["radius"], (int, float))):
                         return (4/3) * 3.14 * math.pow(kwargs["radius"], 3)
                     else:
-                        raise Exception("The 'radius' argument should be an integer.")
+                        raise Exception("The 'radius' argument should be an integer or float.")
                 else:
                     raise Exception("To check the volume of a sphere, the 'radius' argument should be present.")
             elif (shape == "hemisphere"): # Hemisphere
                 if ("radius" in keyList):
-                    if (isinstance(kwargs["radius"], int)):
+                    if (isinstance(kwargs["radius"], (int, float))):
                         return (2/3) * 3.14 * math.pow(kwargs["radius"], 3)
                     else:
-                        raise Exception("The 'radius' argument should be an integer.")
+                        raise Exception("The 'radius' argument should be an integer or float.")
                 else:
                     raise Exception("To check the volume of a hemisphere, the 'radius' argument should be present.")
             elif (shape == "pyramid"): # Pyramid
                 if ("length" in keyList and "width" in keyList and "height" in keyList):
-                    if (isinstance(kwargs["length"], int) and isinstance(kwargs["width"], int) and isinstance(kwargs["height"], int)):
+                    if (isinstance(kwargs["length"], (int, float)) and isinstance(kwargs["width"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         return (length * width * height) / 3
                     else:
-                        raise Exception("The 'length', 'width', and 'height' arguments should be an integer.")
+                        raise Exception("The 'length', 'width', and 'height' arguments should be an integer or float.")
                 else:
                     raise Exception("To check the volume of a pyramid, the 'length', 'width', and 'height' arguments should be present.")
         else:
             raise Exception("The 'shape' argument should be a cube, cuboid, cone, cylinder, sphere, hemisphere, or pyramid.")
     else:
         raise Exception("The 'shape' argument should be present in this function.")
 
@@ -165,114 +165,114 @@
 
     if ("shape" in keyList):
         if (kwargs["shape"] in shapeList):
             shape = kwargs["shape"]
 
             if (shape == "cube"): # Cube
                 if ("side" in keyList):
-                    if (isinstance(kwargs["side"], int)):
+                    if (isinstance(kwargs["side"], (int, float))):
                         if ("lateral" in keyList):
                             if (isinstance(kwargs["lateral"], bool)):
                                 if (kwargs["lateral"] == True):
                                     return 4 * math.pow(side, 2)
                                 else:
                                     return 6 * math.pow(side, 2)
                             else:
                                 raise Exception("The 'lateral' argument should be either True or False.")
                         else:
                             return 6 * math.pow(kwargs["side"], 2)
                     else:
-                        raise Exception("The 'side' argument should be an integer.")
+                        raise Exception("The 'side' argument should be an integer or float.")
                 else:
                     raise Exception("To check the surface area of a cube, the 'side' argument should be present.")
             elif (shape == "cuboid"): # Cuboid
                 if ("length" in keyList and "width" in keyList and "height" in keyList):
-                    if (isinstance(kwargs["length"], int) and isinstance(kwargs["width"], int) and isinstance(kwargs["height"], int)):
+                    if (isinstance(kwargs["length"], (int, float)) and isinstance(kwargs["width"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         if ("lateral" in keyList):
                             if (isinstance(kwargs["lateral"], bool)):
                                 if (kwargs["lateral"] == True):
                                     return 2 * kwargs["height"] * (kwargs["length"] + kwargs["width"])
                                 else:
                                     return 2 * ((kwargs["length"] * kwargs["width"]) + (kwargs["width"] * kwargs["height"]) + (kwargs["length"] * kwargs["height"]))
                             else:
                                 raise Exception("The 'lateral' argument should be either True or False.")
                         else:
                             return 2 * ((kwargs["length"] * kwargs["width"]) + (kwargs["width"] * kwargs["height"]) + (kwargs["length"] * kwargs["height"]))
                     else:
-                        raise Exception("The 'length', 'width', and 'height' arguments should be an integer.")
+                        raise Exception("The 'length', 'width', and 'height' arguments should be an integer or float.")
                 else:
                     raise Exception("To check the surface area of a cuboid, the 'length', 'width', and 'height' arguments should be present.")
             elif (shape == "cone"): # Cone
                 if ("raidus" in keyList and "height" in keyList):
-                    if (isinstance(kwargs["radius"], int) and isinstance(kwargs["height"], int)):
+                    if (isinstance(kwargs["radius"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         slantHeight = math.sqrt(math.pow(kwargs["radius"], 2) + math.pow(kwargs["height"], 2))
 
                         if ("lateral" in keyList):
                             if (isinstance(kwargs["lateral"], bool)):
                                 if (kwargs["lateral"] == True):
                                     return 3.14 * kwargs["radius"] * slantHeight
                                 else:
                                     return 3.14 * kwargs["radius"] * (slantHeight + kwargs["radius"])
                             else:
                                 raise Exception("The 'lateral' argument should be either True or False.")
                         else:
                             return 3.14 * kwargs["radius"] * (slantHeight + kwargs["radius"])
                     else:
-                        raise Exception("The 'radius' and 'height' arguments should be an integer.")
+                        raise Exception("The 'radius' and 'height' arguments should be an integer or float.")
                 else:
                     raise Exception("To check the surface area of a cone, the 'radius' and 'height' arguments should be present.")
             elif (shape == "cylinder"): # Cylinder
                 if ("radius" in keyList and "height" in keyList):
-                    if (isinstance(kwargs["radius"], int) and isinstance(kwargs["height"], int)):
+                    if (isinstance(kwargs["radius"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         if ("lateral" in keyList):
                             if (isinstance(kwargs["lateral"], bool)):
                                 if (kwargs["lateral"] == True):
                                     return 2 * 3.14 * kwargs["radius"] * kwargs["height"]
                                 else:
                                     return 2 * 3.14 * kwargs["radius"] * (kwargs["radius"] + kwargs["height"])
                             else:
                                 raise Exception("The 'lateral' argument should be either True or False.")
                         else:
                             return 2 * 3.14 * kwargs["radius"] * (kwargs["radius"] + kwargs["height"])
                     else:
-                        raise Exception("The 'radius' and 'height' arguments should be an integer.")
+                        raise Exception("The 'radius' and 'height' arguments should be an integer or float.")
                 else:
                     raise Exception("To check the surface area of a cylinder, the 'radius' and 'height' arguments should be present.")
             elif (shape == "sphere"): # Sphere
                 if ("radius" in keyList):
-                    if (isinstance(kwargs["radius"], int)):
+                    if (isinstance(kwargs["radius"], (int, float))):
                         if ("lateral" in keyList):
                             if (isinstance(kwargs["lateral"], bool)):
                                 if (kwargs["lateral"] == True):
                                     return 4 * 3.14 * math.pow(kwargs["radius"], 2)
                                 else:
                                     return 4 * 3.14 * math.pow(kwargs["radius"], 2)
                             else:
                                 raise Exception("The 'lateral' argument should be either True or False.")
                         else:
                             return 4 * 3.14 * math.pow(kwargs["radius"], 2)
                     else:
-                        raise Exception("The 'radius' argument should be an integer.")
+                        raise Exception("The 'radius' argument should be an integer or float.")
                 else:
                     raise Exception("To check the surface area of a sphere, the 'radius' argument should be present.")
             elif (shape == "hemisphere"): # Hemisphere
                 if ("radius" in keyList):
-                    if (isinstance(kwargs["radius"], int)):
+                    if (isinstance(kwargs["radius"], (int, float))):
                         if ("lateral" in keyList):
                             if (isinstance(kwargs["lateral"], bool)):
                                 if (kwargs["lateral"] == True):
                                     return 2 * 3.14 * math.pow(kwargs["radius"], 2)
                                 else:
                                     return 3 * 3.14 * math.pow(kwargs["radius"], 2)
                             else:
                                 raise Exception("The 'lateral' argument should be either True or False.")
                         else:
                             return 3 * 3.14 * math.pow(kwargs["radius"], 2)
                     else:
-                        raise Exception("The 'radius' argument should be an integer.")
+                        raise Exception("The 'radius' argument should be an integer or float.")
                 else:
                     raise Exception("To check the surface area of a hemisphere, the 'radius' argument should be present.")
         else:
             raise Exception("The 'shape' argument should be a cube, cuboid, cone, cylinder, sphere, or hemisphere.")
     else:
         raise Exception("The 'shape' argument should be present in this function.")
```

### Comparing `PySciMath-1.3.0/PySciMath/Numbers.py` & `PySciMath-1.4.0/PySciMath/Arithmetic.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,72 @@
-# PySciMath - Numbers
+# PySciMath - Arithmetic
 
-''' This is the "Numbers" sub-module. '''
+''' This is the "Arithmetic" sub-module. '''
 
-# Function 1 - HCF
+# Functions - Simple Arithmetic Operations
+def add(num1, num2): return num1 + num2
+def subtract(num1, num2): return num1 - num2
+def multiply(num1, num2): return num1 * num2
+def divide(num1, num2): return num1 / num2
+def modulus(num1, num2): return num1 % num2
+def floorDivision(num1, num2): return num1 // num2
+def power(base, exponent): return base ** exponent
+
+# Functions - Squares and Cubes
+def square(number): return power(number, 2)
+def cube(number): return power(number, 3)
+def squareRoot(number): return number ** 0.5
+def cubeRoot(number): return number ** (1/3)
+
+# Functions - Odd and Even
+def isOdd(number): return number % 2 == 1
+def isEven(number): return number % 2 == 0
+
+# Function 1 - Factorial
+def factorial(number):
+    f = 1
+
+    for i in range(1, number + 1):
+        f = f * i
+
+    return f
+
+# Function 2 - HCF
 def hcf(num1, num2):
     hcf = 1
 
     for i in range(1, min(num1, num2)):
         if num1 % i == 0 and num2 % i == 0:
             hcf = i
 
     return hcf
 
-# Function 2 - LCM
+# Function 3 - LCM
 def lcm(num1, num2):
     if (num1 > num2):
         greater = num1
     else:
         greater = num2
 
     while True:
         if ((greater % num1 == 0) and (greater % num2 == 0)):
             lcm = greater
             break
         greater += 1
 
     return lcm
 
-# Function 3 - Prime
+# Function 4 - Prime
 def isPrime(number):
     isPrime = False
 
     if (number < 1):
         isPrime = False
     else:
         for i in range(2, int(number/2) + 1):
             if (number % i == 0):
                 isPrime = False
                 break
         else:
             isPrime = True
 
-    return isPrime
-
-# Function 4 - Power
-def power(base, exponent):
-    num = 1
-
-    for i in range(exponent, 0, -1):
-        num *= base
-
-    return num
-
-# Functions - Squares and Cubes
-def square(number): return power(number, 2)
-def cube(number): return power(number, 3)
-def squareRoot(number): return number ** 0.5
-def cubeRoot(number): return number ** (1/3)
-
-# Functions - Odd and Even
-def isOdd(number): return number % 2 == 1
-def isEven(number): return number % 2 == 0
+    return isPrime
```

### Comparing `PySciMath-1.3.0/PySciMath/Quadratic.py` & `PySciMath-1.4.0/PySciMath/Quadratic.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.3.0/PySciMath/Statistics.py` & `PySciMath-1.4.0/PySciMath/Statistics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # PySciMath - Statistics
 
 ''' This is the "Statistics" sub-module. '''
 
 # Function 1 - Mean
 def mean(data):
-    if (isinstance(data, list) or isinstance(data, tuple) or isinstance(data, set)):
+    if isinstance(data, (list, tuple, set)):
         if (data != None and sum(data) != 0):
             return sum(data) / len(data)
         else:
             raise Exception("The data can't be null and the sum of the data can't be zero.")
     else:
         raise TypeError("The data should be in the form of a list, tuple, or set.")
 
 # Function 2 - Mode
 def mode(data):
-    if (isinstance(data, list) or isinstance(data, tuple) or isinstance(data, set)):
+    if isinstance(data, (list, tuple, set)):
         if (data != None and sum(data) != 0):
             return max(data)
         else:
             raise Exception("The data can't be null and the sum of the data can't be zero.")
     else:
         raise TypeError("The data should be in the form of a list, tuple, or set.")
 
 # Function 3 - Median
 def median(data):
-    if (isinstance(data, list) or isinstance(data, tuple) or isinstance(data, set)):
+    if isinstance(data, (list, tuple, set)):
         if (data != None and sum(data) != 0):
             data.sort()
             mid = len(data) // 2
 
             return (data[mid] + data[~mid]) / 2
         else:
             raise Exception("The data can't be null and the sum of the data can't be zero.")
```

### Comparing `PySciMath-1.3.0/PySciMath/Trigonometry.py` & `PySciMath-1.4.0/PySciMath/Trigonometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.3.0/PySciMath.egg-info/PKG-INFO` & `PySciMath-1.4.0/PySciMath.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.3.0
+Version: 1.4.0
 Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/pyscimath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Calculations
@@ -18,15 +18,15 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.3.0</br>
+**Version** - 1.4.0</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **Author's Email** - anikethchavare@gmail.com</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
```

### Comparing `PySciMath-1.3.0/README.md` & `PySciMath-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.3.0</br>
+**Version** - 1.4.0</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **Author's Email** - anikethchavare@gmail.com</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
```

### Comparing `PySciMath-1.3.0/setup.py` & `PySciMath-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PySciMath",
-    version="1.3.0",
+    version="1.4.0",
     description="PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
```

