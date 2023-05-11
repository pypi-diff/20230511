# Comparing `tmp/safetypes-0.1rc2.post2.tar.gz` & `tmp/safetypes-0.1rc2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safetypes-0.1rc2.post2.tar", last modified: Sun Feb 26 19:04:39 2023, max compression
+gzip compressed data, was "safetypes-0.1rc2.post3.tar", last modified: Thu May 11 19:01:32 2023, max compression
```

## Comparing `safetypes-0.1rc2.post2.tar` & `safetypes-0.1rc2.post3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rafaelgutierrezmartinez   (501) staff       (20)        0 2023-02-26 19:04:39.842453 safetypes-0.1rc2.post2/
--rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)     1106 2022-09-08 13:36:14.000000 safetypes-0.1rc2.post2/LICENSE
--rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)     4515 2023-02-26 19:04:39.842070 safetypes-0.1rc2.post2/PKG-INFO
--rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)     1944 2023-01-28 17:21:28.000000 safetypes-0.1rc2.post2/README.md
--rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)     1264 2023-02-26 19:03:05.000000 safetypes-0.1rc2.post2/pyproject.toml
-drwxr-xr-x   0 rafaelgutierrezmartinez   (501) staff       (20)        0 2023-02-26 19:04:39.836842 safetypes-0.1rc2.post2/safetypes/
--rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)     1257 2023-01-28 13:52:31.000000 safetypes-0.1rc2.post2/safetypes/__init__.py
-drwxr-xr-x   0 rafaelgutierrezmartinez   (501) staff       (20)        0 2023-02-26 19:04:39.841603 safetypes-0.1rc2.post2/safetypes/base/
--rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)    10416 2023-02-26 18:53:39.000000 safetypes-0.1rc2.post2/safetypes/base/SafeFiles.py
--rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)      171 2022-09-07 19:35:13.000000 safetypes-0.1rc2.post2/safetypes/base/SafeFunctionTypes.py
--rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)        0 2022-09-07 19:31:44.000000 safetypes-0.1rc2.post2/safetypes/base/__init__.py
-drwxr-xr-x   0 rafaelgutierrezmartinez   (501) staff       (20)        0 2023-02-26 19:04:39.839416 safetypes-0.1rc2.post2/safetypes.egg-info/
--rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)     4515 2023-02-26 19:04:39.000000 safetypes-0.1rc2.post2/safetypes.egg-info/PKG-INFO
--rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)      286 2023-02-26 19:04:39.000000 safetypes-0.1rc2.post2/safetypes.egg-info/SOURCES.txt
--rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)        1 2023-02-26 19:04:39.000000 safetypes-0.1rc2.post2/safetypes.egg-info/dependency_links.txt
--rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)       25 2023-02-26 19:04:39.000000 safetypes-0.1rc2.post2/safetypes.egg-info/top_level.txt
--rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)       38 2023-02-26 19:04:39.842571 safetypes-0.1rc2.post2/setup.cfg
--rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)      708 2023-02-26 18:53:39.000000 safetypes-0.1rc2.post2/setup.py
+drwxr-xr-x   0 rafaelgutierrezmartinez   (501) staff       (20)        0 2023-05-11 19:01:32.667907 safetypes-0.1rc2.post3/
+-rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)     1106 2022-09-08 13:36:14.000000 safetypes-0.1rc2.post3/LICENSE
+-rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)     4515 2023-05-11 19:01:32.667499 safetypes-0.1rc2.post3/PKG-INFO
+-rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)     1944 2023-01-28 17:21:28.000000 safetypes-0.1rc2.post3/README.md
+-rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)     1264 2023-05-11 19:00:30.000000 safetypes-0.1rc2.post3/pyproject.toml
+drwxr-xr-x   0 rafaelgutierrezmartinez   (501) staff       (20)        0 2023-05-11 19:01:32.663711 safetypes-0.1rc2.post3/safetypes/
+-rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)     1257 2023-01-28 13:52:31.000000 safetypes-0.1rc2.post3/safetypes/__init__.py
+drwxr-xr-x   0 rafaelgutierrezmartinez   (501) staff       (20)        0 2023-05-11 19:01:32.667008 safetypes-0.1rc2.post3/safetypes/base/
+-rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)    10726 2023-05-11 19:00:30.000000 safetypes-0.1rc2.post3/safetypes/base/SafeFiles.py
+-rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)      171 2022-09-07 19:35:13.000000 safetypes-0.1rc2.post3/safetypes/base/SafeFunctionTypes.py
+-rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)        0 2022-09-07 19:31:44.000000 safetypes-0.1rc2.post3/safetypes/base/__init__.py
+drwxr-xr-x   0 rafaelgutierrezmartinez   (501) staff       (20)        0 2023-05-11 19:01:32.665550 safetypes-0.1rc2.post3/safetypes.egg-info/
+-rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)     4515 2023-05-11 19:01:32.000000 safetypes-0.1rc2.post3/safetypes.egg-info/PKG-INFO
+-rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)      286 2023-05-11 19:01:32.000000 safetypes-0.1rc2.post3/safetypes.egg-info/SOURCES.txt
+-rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)        1 2023-05-11 19:01:32.000000 safetypes-0.1rc2.post3/safetypes.egg-info/dependency_links.txt
+-rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)       25 2023-05-11 19:01:32.000000 safetypes-0.1rc2.post3/safetypes.egg-info/top_level.txt
+-rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)       38 2023-05-11 19:01:32.668031 safetypes-0.1rc2.post3/setup.cfg
+-rw-r--r--   0 rafaelgutierrezmartinez   (501) staff       (20)      708 2023-05-11 19:00:30.000000 safetypes-0.1rc2.post3/setup.py
```

### Comparing `safetypes-0.1rc2.post2/LICENSE` & `safetypes-0.1rc2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `safetypes-0.1rc2.post2/PKG-INFO` & `safetypes-0.1rc2.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safetypes
-Version: 0.1rc2.post2
+Version: 0.1rc2.post3
 Summary: Python is a not typed language, and runs under the paradigm of first try and then it success or fails. This package allows you to have the capability of apply typing features in last versions of Python, allowing to the developer to have a transparent mechanism to grant that typing annotations are satisfied in the execution time of their programs.
 Home-page: https://github.com/wiscot/safetypes
 Author: Rafael Gutiérrez Martínez
 Author-email: Rafael Gutiérrez Martínez <ragutimar@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Rafael Gutiérrez Martínez - ragutimar@gmail.com
```

### Comparing `safetypes-0.1rc2.post2/README.md` & `safetypes-0.1rc2.post3/README.md`

 * *Files identical despite different names*

### Comparing `safetypes-0.1rc2.post2/pyproject.toml` & `safetypes-0.1rc2.post3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "safetypes"
-version = "0.1rc2post2"
+version = "0.1rc2post3"
 authors = [
   { name="Rafael Gutiérrez Martínez", email="ragutimar@gmail.com" },
 ]
 description = "Python is a not typed language, and runs under the paradigm of first try and then it success or fails. This package allows you to have the capability of apply typing features in last versions of Python, allowing to the developer to have a transparent mechanism to grant that typing annotations are satisfied in the execution time of their programs."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.5"
```

### Comparing `safetypes-0.1rc2.post2/safetypes/__init__.py` & `safetypes-0.1rc2.post3/safetypes/__init__.py`

 * *Files identical despite different names*

### Comparing `safetypes-0.1rc2.post2/safetypes/base/SafeFiles.py` & `safetypes-0.1rc2.post3/safetypes/base/SafeFiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,18 +151,22 @@
             else:
                 err = False
                 try:
                     if not isinstance(argument, parameter_type.__args__):
                         err = True
                 except TypeError:
                     for arg in parameter_type.__args__:
-                        if not type(argument) in arg and not isinstance(argument, arg):
+                        if isinstance(arg, typing.ForwardRef):
+                            if argument.__class__.__qualname__ != arg.__forward_arg__ \
+                                    and SafeTypes._get_full_name(type(argument)) != arg.__forward_arg__:
+                                err = True
+                            break
+                        elif not type(argument) in arg and not isinstance(argument, arg):
                             err = True
                             break
-                    pass
                 if err:
                     SafeTypes._raise_error(argument, parameter_type, parameter_name)
         elif type(parameter_type) is str:
             if argument.__class__.__qualname__ != parameter_type and SafeTypes._get_full_name(type(argument)) != parameter_type:
                 SafeTypes._raise_error(argument, parameter_type, parameter_name)
         else:
             if not isinstance(argument, parameter_type):
```

### Comparing `safetypes-0.1rc2.post2/safetypes.egg-info/PKG-INFO` & `safetypes-0.1rc2.post3/safetypes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safetypes
-Version: 0.1rc2.post2
+Version: 0.1rc2.post3
 Summary: Python is a not typed language, and runs under the paradigm of first try and then it success or fails. This package allows you to have the capability of apply typing features in last versions of Python, allowing to the developer to have a transparent mechanism to grant that typing annotations are satisfied in the execution time of their programs.
 Home-page: https://github.com/wiscot/safetypes
 Author: Rafael Gutiérrez Martínez
 Author-email: Rafael Gutiérrez Martínez <ragutimar@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Rafael Gutiérrez Martínez - ragutimar@gmail.com
```

### Comparing `safetypes-0.1rc2.post2/setup.py` & `safetypes-0.1rc2.post3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='safetypes',
-    version='0.1rc2post2',
+    version='0.1rc2post3',
     packages=['safetypes', 'safetypes/base'],
     url='https://github.com/wiscot/safetypes',
     license='MIT',
     author='Rafael Gutiérrez Martínez',
     author_email='ragutimar@gmail.com',
     description='Python is a non typed language, and runs under the paradigm of first try and then '
                 'it success or fails. This package allows you to have the capability of apply typing features '
```

