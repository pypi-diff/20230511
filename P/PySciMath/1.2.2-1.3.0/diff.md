# Comparing `tmp/PySciMath-1.2.2.tar.gz` & `tmp/PySciMath-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySciMath-1.2.2.tar", last modified: Wed May 10 14:50:58 2023, max compression
+gzip compressed data, was "PySciMath-1.3.0.tar", last modified: Thu May 11 07:39:58 2023, max compression
```

## Comparing `PySciMath-1.2.2.tar` & `PySciMath-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 14:50:58.061936 PySciMath-1.2.2/
--rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2643 2023-05-10 14:50:58.060938 PySciMath-1.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 14:50:58.040994 PySciMath-1.2.2/PySciMath/
--rw-rw-rw-   0        0        0      431 2023-05-10 10:33:22.000000 PySciMath-1.2.2/PySciMath/Arithmetic.py
--rw-rw-rw-   0        0        0      677 2023-05-10 14:22:10.000000 PySciMath-1.2.2/PySciMath/ComplexNumbers.py
--rw-rw-rw-   0        0        0     4286 2023-05-10 14:05:32.000000 PySciMath-1.2.2/PySciMath/CoordinateGeometry.py
--rw-rw-rw-   0        0        0     2870 2023-05-10 14:48:59.000000 PySciMath-1.2.2/PySciMath/Geometry.py
--rw-rw-rw-   0        0        0     1350 2023-05-10 13:24:34.000000 PySciMath-1.2.2/PySciMath/Numbers.py
--rw-rw-rw-   0        0        0      568 2023-05-10 10:26:42.000000 PySciMath-1.2.2/PySciMath/Quadratic.py
--rw-rw-rw-   0        0        0     1392 2023-05-10 09:43:22.000000 PySciMath-1.2.2/PySciMath/Statistics.py
--rw-rw-rw-   0        0        0      558 2023-05-10 09:51:46.000000 PySciMath-1.2.2/PySciMath/Trigonometry.py
--rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.2.2/PySciMath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:50:58.055952 PySciMath-1.2.2/PySciMath.egg-info/
--rw-rw-rw-   0        0        0     2643 2023-05-10 14:50:57.000000 PySciMath-1.2.2/PySciMath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-05-10 14:50:57.000000 PySciMath-1.2.2/PySciMath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 14:50:57.000000 PySciMath-1.2.2/PySciMath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 14:50:57.000000 PySciMath-1.2.2/PySciMath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2128 2023-05-10 14:24:31.000000 PySciMath-1.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 14:50:58.061936 PySciMath-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-05-10 14:23:55.000000 PySciMath-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 07:39:58.373470 PySciMath-1.3.0/
+-rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2643 2023-05-11 07:39:58.363495 PySciMath-1.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-11 07:39:58.297670 PySciMath-1.3.0/PySciMath/
+-rw-rw-rw-   0        0        0      431 2023-05-10 10:33:22.000000 PySciMath-1.3.0/PySciMath/Arithmetic.py
+-rw-rw-rw-   0        0        0      677 2023-05-10 14:22:10.000000 PySciMath-1.3.0/PySciMath/ComplexNumbers.py
+-rw-rw-rw-   0        0        0     4286 2023-05-10 14:05:32.000000 PySciMath-1.3.0/PySciMath/CoordinateGeometry.py
+-rw-rw-rw-   0        0        0    17238 2023-05-11 07:37:25.000000 PySciMath-1.3.0/PySciMath/Geometry.py
+-rw-rw-rw-   0        0        0     1350 2023-05-10 13:24:34.000000 PySciMath-1.3.0/PySciMath/Numbers.py
+-rw-rw-rw-   0        0        0      568 2023-05-10 10:26:42.000000 PySciMath-1.3.0/PySciMath/Quadratic.py
+-rw-rw-rw-   0        0        0     1392 2023-05-10 09:43:22.000000 PySciMath-1.3.0/PySciMath/Statistics.py
+-rw-rw-rw-   0        0        0      558 2023-05-10 09:51:46.000000 PySciMath-1.3.0/PySciMath/Trigonometry.py
+-rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.3.0/PySciMath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 07:39:58.332578 PySciMath-1.3.0/PySciMath.egg-info/
+-rw-rw-rw-   0        0        0     2643 2023-05-11 07:39:57.000000 PySciMath-1.3.0/PySciMath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-05-11 07:39:57.000000 PySciMath-1.3.0/PySciMath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 07:39:57.000000 PySciMath-1.3.0/PySciMath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 07:39:57.000000 PySciMath-1.3.0/PySciMath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2128 2023-05-11 07:38:28.000000 PySciMath-1.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-11 07:39:58.373470 PySciMath-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      903 2023-05-11 07:38:16.000000 PySciMath-1.3.0/setup.py
```

### Comparing `PySciMath-1.2.2/LICENSE.txt` & `PySciMath-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.2/PKG-INFO` & `PySciMath-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.2.2
+Version: 1.3.0
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
-**Version** - 1.2.2</br>
+**Version** - 1.3.0</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **Author's Email** - anikethchavare@gmail.com</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
```

### Comparing `PySciMath-1.2.2/PySciMath/ComplexNumbers.py` & `PySciMath-1.3.0/PySciMath/ComplexNumbers.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.2/PySciMath/CoordinateGeometry.py` & `PySciMath-1.3.0/PySciMath/CoordinateGeometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.2/PySciMath/Numbers.py` & `PySciMath-1.3.0/PySciMath/Numbers.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.2/PySciMath/Quadratic.py` & `PySciMath-1.3.0/PySciMath/Quadratic.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.2/PySciMath/Statistics.py` & `PySciMath-1.3.0/PySciMath/Statistics.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.2/PySciMath/Trigonometry.py` & `PySciMath-1.3.0/PySciMath/Trigonometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.2/PySciMath.egg-info/PKG-INFO` & `PySciMath-1.3.0/PySciMath.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.2.2
+Version: 1.3.0
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
-**Version** - 1.2.2</br>
+**Version** - 1.3.0</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **Author's Email** - anikethchavare@gmail.com</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
```

### Comparing `PySciMath-1.2.2/README.md` & `PySciMath-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.2.2</br>
+**Version** - 1.3.0</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **Author's Email** - anikethchavare@gmail.com</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
```

### Comparing `PySciMath-1.2.2/setup.py` & `PySciMath-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PySciMath",
-    version="1.2.2",
+    version="1.3.0",
     description="PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
```

