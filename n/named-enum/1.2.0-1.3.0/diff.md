# Comparing `tmp/named_enum-1.2.0.tar.gz` & `tmp/named_enum-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "named_enum-1.2.0.tar", last modified: Sun Apr 10 22:20:02 2022, max compression
+gzip compressed data, was "named_enum-1.3.0.tar", last modified: Wed May 10 22:04:28 2023, max compression
```

## Comparing `named_enum-1.2.0.tar` & `named_enum-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 22:20:02.750352 named_enum-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-04-10 22:19:54.000000 named_enum-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-10 22:19:54.000000 named_enum-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14314 2022-04-10 22:20:02.750352 named_enum-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13322 2022-04-10 22:19:54.000000 named_enum-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 22:20:02.750352 named_enum-1.2.0/named_enum/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-04-10 22:19:54.000000 named_enum-1.2.0/named_enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20249 2022-04-10 22:19:54.000000 named_enum-1.2.0/named_enum/enum.py
--rw-r--r--   0 runner    (1001) docker     (121)    24113 2022-04-10 22:19:54.000000 named_enum-1.2.0/named_enum/meta.py
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-04-10 22:19:54.000000 named_enum-1.2.0/named_enum/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 22:20:02.750352 named_enum-1.2.0/named_enum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14314 2022-04-10 22:20:02.000000 named_enum-1.2.0/named_enum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-04-10 22:20:02.000000 named_enum-1.2.0/named_enum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-10 22:20:02.000000 named_enum-1.2.0/named_enum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-10 22:20:02.000000 named_enum-1.2.0/named_enum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-04-10 22:20:02.000000 named_enum-1.2.0/named_enum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-04-10 22:20:02.000000 named_enum-1.2.0/named_enum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-04-10 22:20:02.750352 named_enum-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2870 2022-04-10 22:19:54.000000 named_enum-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:04:28.316132 named_enum-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-10 22:04:17.000000 named_enum-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:04:17.000000 named_enum-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-05-10 22:04:28.316132 named_enum-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-05-10 22:04:17.000000 named_enum-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:04:28.316132 named_enum-1.3.0/named_enum/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-10 22:04:17.000000 named_enum-1.3.0/named_enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20249 2023-05-10 22:04:17.000000 named_enum-1.3.0/named_enum/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24232 2023-05-10 22:04:17.000000 named_enum-1.3.0/named_enum/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 22:04:17.000000 named_enum-1.3.0/named_enum/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:04:28.316132 named_enum-1.3.0/named_enum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-05-10 22:04:28.000000 named_enum-1.3.0/named_enum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-10 22:04:28.000000 named_enum-1.3.0/named_enum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 22:04:28.000000 named_enum-1.3.0/named_enum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 22:04:28.000000 named_enum-1.3.0/named_enum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 22:04:28.000000 named_enum-1.3.0/named_enum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 22:04:28.000000 named_enum-1.3.0/named_enum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-10 22:04:28.316132 named_enum-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-10 22:04:17.000000 named_enum-1.3.0/setup.py
```

### Comparing `named_enum-1.2.0/LICENSE` & `named_enum-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `named_enum-1.2.0/PKG-INFO` & `named_enum-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: named_enum
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python named enumeration, which extends the built-in Enum class with extra features.
 Home-page: https://github.com/zhiwei2017/named_enum
 Author: Zhiwei Zhang
 Author-email: zhiwei2017@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 License-File: LICENSE
@@ -47,15 +48,15 @@
 .. development status from pypi
 .. image:: https://img.shields.io/pypi/status/named-enum.svg
     :target: https://pypi.python.org/pypi/named-enum/
 
 .. python version badge from PyPI
 .. image:: https://img.shields.io/pypi/pyversions/named-enum.svg
     :target: https://pypi.python.org/pypi/named-enum/
-    :alt: Python 3.7 | Python 3.8 | Python3.9 | Python3.10
+    :alt: Python 3.7 | Python 3.8 | Python3.9 | Python3.10 | Python3.11
 
 .. pypi format
 .. image:: https://img.shields.io/pypi/format/named-enum.svg
     :target: https://badge.fury.io/py/named-enum
 
 .. codecov badge
 .. image:: https://codecov.io/gh/zhiwei2017/named_enum/branch/master/graph/badge.svg
```

### Comparing `named_enum-1.2.0/README.rst` & `named_enum-1.3.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 .. development status from pypi
 .. image:: https://img.shields.io/pypi/status/named-enum.svg
     :target: https://pypi.python.org/pypi/named-enum/
 
 .. python version badge from PyPI
 .. image:: https://img.shields.io/pypi/pyversions/named-enum.svg
     :target: https://pypi.python.org/pypi/named-enum/
-    :alt: Python 3.7 | Python 3.8 | Python3.9 | Python3.10
+    :alt: Python 3.7 | Python 3.8 | Python3.9 | Python3.10 | Python3.11
 
 .. pypi format
 .. image:: https://img.shields.io/pypi/format/named-enum.svg
     :target: https://badge.fury.io/py/named-enum
 
 .. codecov badge
 .. image:: https://codecov.io/gh/zhiwei2017/named_enum/branch/master/graph/badge.svg
```

### Comparing `named_enum-1.2.0/named_enum/enum.py` & `named_enum-1.3.0/named_enum/enum.py`

 * *Files identical despite different names*

### Comparing `named_enum-1.2.0/named_enum/meta.py` & `named_enum-1.3.0/named_enum/meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,17 @@
     def _clean(self) -> None:
         """Removes all the items, and set the variables '_member_names' and
         '_last_values' to empty."""
         # for dictionary, that's the only way to _clean it
         for name in self._member_names:
             del self[name]
         # _clean the variables as well
-        self._member_names, self._last_values = [], []
+        tmp_dict = _EnumDict()
+        self._member_names = tmp_dict._member_names
+        self._last_values = tmp_dict._last_values
 
     def _convert(self, tuple_cls: Type[NamedTuple]) -> None:
         """Uses the given tuple class to _convert the items.
 
         Args:
             tuple_cls (Type[NamedTuple]): using namedtuple generated tuple class.
         """
@@ -57,18 +59,18 @@
         if feature_num == 1:
             # converting the type of the value in customized tuple
             for value in self._last_values:
                 _last_values.append(tuple_cls(value))
         else:
             # converting the type of the value in customized tuple
             for value in self._last_values:
-                if not isinstance(value, Sequence):
-                    raise ValueError("unable to unpack the value for the fields.")
-                elif isinstance(value, str):
-                    _last_values.append(tuple_cls(value))
+                if not isinstance(value, Sequence) or isinstance(value, str):
+                    err_msg = "Unable to unpack the value '{}' as {} " \
+                              "for the fields.".format(value, tuple_cls.__name__)
+                    raise ValueError(err_msg)
                 else:
                     _last_values.append(tuple_cls(*value))
         self._clean()
 
         # put the converted items back, the __setitem__ function in _EnumDict
         # will fill the variables, like '_member_names' and '_last_values'
         for i, name in enumerate(_member_names):
```

### Comparing `named_enum-1.2.0/named_enum.egg-info/PKG-INFO` & `named_enum-1.3.0/named_enum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: named-enum
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python named enumeration, which extends the built-in Enum class with extra features.
 Home-page: https://github.com/zhiwei2017/named_enum
 Author: Zhiwei Zhang
 Author-email: zhiwei2017@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 License-File: LICENSE
@@ -47,15 +48,15 @@
 .. development status from pypi
 .. image:: https://img.shields.io/pypi/status/named-enum.svg
     :target: https://pypi.python.org/pypi/named-enum/
 
 .. python version badge from PyPI
 .. image:: https://img.shields.io/pypi/pyversions/named-enum.svg
     :target: https://pypi.python.org/pypi/named-enum/
-    :alt: Python 3.7 | Python 3.8 | Python3.9 | Python3.10
+    :alt: Python 3.7 | Python 3.8 | Python3.9 | Python3.10 | Python3.11
 
 .. pypi format
 .. image:: https://img.shields.io/pypi/format/named-enum.svg
     :target: https://badge.fury.io/py/named-enum
 
 .. codecov badge
 .. image:: https://codecov.io/gh/zhiwei2017/named_enum/branch/master/graph/badge.svg
```

### Comparing `named_enum-1.2.0/setup.py` & `named_enum-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
           "Development Status :: 5 - Production/Stable",
           "Programming Language :: Python",
           "Programming Language :: Python :: 3",
           "Programming Language :: Python :: 3.7",
           "Programming Language :: Python :: 3.8",
           "Programming Language :: Python :: 3.9",
           "Programming Language :: Python :: 3.10",
+          "Programming Language :: Python :: 3.11",
           "Programming Language :: Python :: Implementation",
           "Topic :: Utilities",
           "Natural Language :: English",
           "Intended Audience :: Developers",
       ],
       install_requires=INSTALL_REQUIRED,
       tests_require=DEV_REQUIRED,
```

