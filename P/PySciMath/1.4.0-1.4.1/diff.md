# Comparing `tmp/PySciMath-1.4.0.tar.gz` & `tmp/PySciMath-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySciMath-1.4.0.tar", last modified: Thu May 11 15:16:27 2023, max compression
+gzip compressed data, was "PySciMath-1.4.1.tar", last modified: Thu May 11 15:32:21 2023, max compression
```

## Comparing `PySciMath-1.4.0.tar` & `PySciMath-1.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 15:16:27.752609 PySciMath-1.4.0/
--rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2643 2023-05-11 15:16:27.751612 PySciMath-1.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-11 15:16:27.735654 PySciMath-1.4.0/PySciMath/
--rw-rw-rw-   0        0        0     1720 2023-05-11 15:05:50.000000 PySciMath-1.4.0/PySciMath/Arithmetic.py
--rw-rw-rw-   0        0        0      677 2023-05-10 14:22:10.000000 PySciMath-1.4.0/PySciMath/ComplexNumbers.py
--rw-rw-rw-   0        0        0     4286 2023-05-10 14:05:32.000000 PySciMath-1.4.0/PySciMath/CoordinateGeometry.py
--rw-rw-rw-   0        0        0    17742 2023-05-11 15:13:15.000000 PySciMath-1.4.0/PySciMath/Geometry.py
--rw-rw-rw-   0        0        0      568 2023-05-10 10:26:42.000000 PySciMath-1.4.0/PySciMath/Quadratic.py
--rw-rw-rw-   0        0        0     1272 2023-05-11 15:14:07.000000 PySciMath-1.4.0/PySciMath/Statistics.py
--rw-rw-rw-   0        0        0      558 2023-05-10 09:51:46.000000 PySciMath-1.4.0/PySciMath/Trigonometry.py
--rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.4.0/PySciMath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:16:27.747622 PySciMath-1.4.0/PySciMath.egg-info/
--rw-rw-rw-   0        0        0     2643 2023-05-11 15:16:27.000000 PySciMath-1.4.0/PySciMath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2023-05-11 15:16:27.000000 PySciMath-1.4.0/PySciMath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 15:16:27.000000 PySciMath-1.4.0/PySciMath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-11 15:16:27.000000 PySciMath-1.4.0/PySciMath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2128 2023-05-11 15:14:59.000000 PySciMath-1.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-11 15:16:27.752609 PySciMath-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-05-11 15:14:54.000000 PySciMath-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:32:21.231861 PySciMath-1.4.1/
+-rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2591 2023-05-11 15:32:21.230862 PySciMath-1.4.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-11 15:32:21.211923 PySciMath-1.4.1/PySciMath/
+-rw-rw-rw-   0        0        0     1720 2023-05-11 15:05:50.000000 PySciMath-1.4.1/PySciMath/Arithmetic.py
+-rw-rw-rw-   0        0        0      677 2023-05-10 14:22:10.000000 PySciMath-1.4.1/PySciMath/ComplexNumbers.py
+-rw-rw-rw-   0        0        0     4286 2023-05-10 14:05:32.000000 PySciMath-1.4.1/PySciMath/CoordinateGeometry.py
+-rw-rw-rw-   0        0        0    17742 2023-05-11 15:13:15.000000 PySciMath-1.4.1/PySciMath/Geometry.py
+-rw-rw-rw-   0        0        0      568 2023-05-10 10:26:42.000000 PySciMath-1.4.1/PySciMath/Quadratic.py
+-rw-rw-rw-   0        0        0     1272 2023-05-11 15:14:07.000000 PySciMath-1.4.1/PySciMath/Statistics.py
+-rw-rw-rw-   0        0        0      558 2023-05-10 09:51:46.000000 PySciMath-1.4.1/PySciMath/Trigonometry.py
+-rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.4.1/PySciMath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:32:21.226874 PySciMath-1.4.1/PySciMath.egg-info/
+-rw-rw-rw-   0        0        0     2591 2023-05-11 15:32:21.000000 PySciMath-1.4.1/PySciMath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2023-05-11 15:32:21.000000 PySciMath-1.4.1/PySciMath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 15:32:21.000000 PySciMath-1.4.1/PySciMath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 15:32:21.000000 PySciMath-1.4.1/PySciMath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2077 2023-05-11 15:31:15.000000 PySciMath-1.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-11 15:32:21.232857 PySciMath-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      903 2023-05-11 15:31:24.000000 PySciMath-1.4.1/setup.py
```

### Comparing `PySciMath-1.4.0/LICENSE.txt` & `PySciMath-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySciMath-1.4.0/PKG-INFO` & `PySciMath-1.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.4.0
+Version: 1.4.1
 Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/pyscimath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Calculations
@@ -18,18 +18,17 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.4.0</br>
+**Version** - 1.4.1</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
-**Author's Email** - anikethchavare@gmail.com</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
 
 MIT License
```

### Comparing `PySciMath-1.4.0/PySciMath/Arithmetic.py` & `PySciMath-1.4.1/PySciMath/Arithmetic.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.4.0/PySciMath/ComplexNumbers.py` & `PySciMath-1.4.1/PySciMath/ComplexNumbers.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.4.0/PySciMath/CoordinateGeometry.py` & `PySciMath-1.4.1/PySciMath/CoordinateGeometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.4.0/PySciMath/Geometry.py` & `PySciMath-1.4.1/PySciMath/Geometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.4.0/PySciMath/Quadratic.py` & `PySciMath-1.4.1/PySciMath/Quadratic.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.4.0/PySciMath/Statistics.py` & `PySciMath-1.4.1/PySciMath/Statistics.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.4.0/PySciMath/Trigonometry.py` & `PySciMath-1.4.1/PySciMath/Trigonometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.4.0/PySciMath.egg-info/PKG-INFO` & `PySciMath-1.4.1/PySciMath.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.4.0
+Version: 1.4.1
 Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/pyscimath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Calculations
@@ -18,18 +18,17 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.4.0</br>
+**Version** - 1.4.1</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
-**Author's Email** - anikethchavare@gmail.com</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
 
 MIT License
```

### Comparing `PySciMath-1.4.0/README.md` & `PySciMath-1.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.4.0</br>
+**Version** - 1.4.1</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
-**Author's Email** - anikethchavare@gmail.com</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
 
 MIT License
```

### Comparing `PySciMath-1.4.0/setup.py` & `PySciMath-1.4.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PySciMath",
-    version="1.4.0",
+    version="1.4.1",
     description="PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
```

