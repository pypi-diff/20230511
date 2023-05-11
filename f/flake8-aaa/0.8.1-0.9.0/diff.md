# Comparing `tmp/flake8-aaa-0.8.1.tar.gz` & `tmp/flake8-aaa-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flake8-aaa-0.8.1.tar", last modified: Sun Mar  1 18:34:46 2020, max compression
+gzip compressed data, was "dist/flake8-aaa-0.9.0.tar", last modified: Sat Mar  7 18:31:44 2020, max compression
```

## Comparing `flake8-aaa-0.8.1.tar` & `flake8-aaa-0.9.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2020-03-01 18:34:46.000000 flake8-aaa-0.8.1/
--rw-rw-r--   0 james     (1000) james     (1000)     5103 2020-03-01 18:34:46.000000 flake8-aaa-0.8.1/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)      415 2020-03-01 18:34:46.000000 flake8-aaa-0.8.1/setup.cfg
--rw-rw-r--   0 james     (1000) james     (1000)     1068 2018-02-22 22:42:33.000000 flake8-aaa-0.8.1/LICENSE
--rw-rw-r--   0 james     (1000) james     (1000)     1408 2020-02-27 12:50:56.000000 flake8-aaa-0.8.1/setup.py
--rw-rw-r--   0 james     (1000) james     (1000)       35 2018-04-20 18:13:45.000000 flake8-aaa-0.8.1/MANIFEST.in
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2020-03-01 18:34:46.000000 flake8-aaa-0.8.1/src/
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2020-03-01 18:34:46.000000 flake8-aaa-0.8.1/src/flake8_aaa.egg-info/
--rw-rw-r--   0 james     (1000) james     (1000)        1 2020-03-01 18:34:45.000000 flake8-aaa-0.8.1/src/flake8_aaa.egg-info/dependency_links.txt
--rw-rw-r--   0 james     (1000) james     (1000)      678 2020-03-01 18:34:45.000000 flake8-aaa-0.8.1/src/flake8_aaa.egg-info/SOURCES.txt
--rw-rw-r--   0 james     (1000) james     (1000)     5103 2020-03-01 18:34:45.000000 flake8-aaa-0.8.1/src/flake8_aaa.egg-info/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)       45 2020-03-01 18:34:45.000000 flake8-aaa-0.8.1/src/flake8_aaa.egg-info/entry_points.txt
--rw-rw-r--   0 james     (1000) james     (1000)        1 2019-01-14 22:14:52.000000 flake8-aaa-0.8.1/src/flake8_aaa.egg-info/not-zip-safe
--rw-rw-r--   0 james     (1000) james     (1000)       11 2020-03-01 18:34:45.000000 flake8-aaa-0.8.1/src/flake8_aaa.egg-info/top_level.txt
--rw-rw-r--   0 james     (1000) james     (1000)       13 2020-03-01 18:34:45.000000 flake8-aaa-0.8.1/src/flake8_aaa.egg-info/requires.txt
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2020-03-01 18:34:46.000000 flake8-aaa-0.8.1/src/flake8_aaa/
--rw-rw-r--   0 james     (1000) james     (1000)     7116 2020-02-28 16:59:15.000000 flake8-aaa-0.8.1/src/flake8_aaa/helpers.py
--rw-rw-r--   0 james     (1000) james     (1000)      674 2019-04-19 15:49:49.000000 flake8-aaa-0.8.1/src/flake8_aaa/__main__.py
--rw-rw-r--   0 james     (1000) james     (1000)     1259 2019-07-13 12:22:04.000000 flake8-aaa-0.8.1/src/flake8_aaa/exceptions.py
--rw-rw-r--   0 james     (1000) james     (1000)     2598 2019-07-13 12:22:04.000000 flake8-aaa-0.8.1/src/flake8_aaa/block.py
--rw-rw-r--   0 james     (1000) james     (1000)       59 2019-02-01 23:53:13.000000 flake8-aaa-0.8.1/src/flake8_aaa/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)      399 2020-02-28 16:59:15.000000 flake8-aaa-0.8.1/src/flake8_aaa/multi_node_block.py
--rw-rw-r--   0 james     (1000) james     (1000)     1823 2020-02-28 16:59:15.000000 flake8-aaa-0.8.1/src/flake8_aaa/act_node.py
--rw-rw-r--   0 james     (1000) james     (1000)      694 2020-02-27 12:50:56.000000 flake8-aaa-0.8.1/src/flake8_aaa/types.py
--rw-rw-r--   0 james     (1000) james     (1000)     1697 2019-04-21 17:26:05.000000 flake8-aaa-0.8.1/src/flake8_aaa/checker.py
--rw-rw-r--   0 james     (1000) james     (1000)      255 2020-03-01 18:22:53.000000 flake8-aaa-0.8.1/src/flake8_aaa/__about__.py
--rw-rw-r--   0 james     (1000) james     (1000)     5815 2020-02-28 16:59:15.000000 flake8-aaa-0.8.1/src/flake8_aaa/line_markers.py
--rw-rw-r--   0 james     (1000) james     (1000)     7034 2020-02-28 16:59:15.000000 flake8-aaa-0.8.1/src/flake8_aaa/function.py
--rw-rw-r--   0 james     (1000) james     (1000)     1081 2019-05-25 22:46:52.000000 flake8-aaa-0.8.1/src/flake8_aaa/command_line.py
--rw-rw-r--   0 james     (1000) james     (1000)     3414 2020-02-27 12:50:56.000000 flake8-aaa-0.8.1/README.rst
+drwxr-xr-x   0 james     (1000) james     (1000)        0 2020-03-07 18:31:44.000000 flake8-aaa-0.9.0/
+-rw-r--r--   0 james     (1000) james     (1000)     1068 2020-02-13 10:22:50.000000 flake8-aaa-0.9.0/LICENSE
+-rw-r--r--   0 james     (1000) james     (1000)       35 2020-02-13 10:22:50.000000 flake8-aaa-0.9.0/MANIFEST.in
+-rw-r--r--   0 james     (1000) james     (1000)     5103 2020-03-07 18:31:44.000000 flake8-aaa-0.9.0/PKG-INFO
+-rw-r--r--   0 james     (1000) james     (1000)     3414 2020-03-06 19:19:00.000000 flake8-aaa-0.9.0/README.rst
+-rw-r--r--   0 james     (1000) james     (1000)      397 2020-03-07 18:31:44.000000 flake8-aaa-0.9.0/setup.cfg
+-rw-r--r--   0 james     (1000) james     (1000)     1408 2020-03-06 19:19:00.000000 flake8-aaa-0.9.0/setup.py
+drwxr-xr-x   0 james     (1000) james     (1000)        0 2020-03-07 18:31:44.000000 flake8-aaa-0.9.0/src/
+drwxr-xr-x   0 james     (1000) james     (1000)        0 2020-03-07 18:31:44.000000 flake8-aaa-0.9.0/src/flake8_aaa/
+-rw-r--r--   0 james     (1000) james     (1000)      255 2020-03-07 18:24:47.000000 flake8-aaa-0.9.0/src/flake8_aaa/__about__.py
+-rw-r--r--   0 james     (1000) james     (1000)       59 2020-02-13 10:22:50.000000 flake8-aaa-0.9.0/src/flake8_aaa/__init__.py
+-rw-r--r--   0 james     (1000) james     (1000)      674 2020-02-13 10:22:50.000000 flake8-aaa-0.9.0/src/flake8_aaa/__main__.py
+-rw-r--r--   0 james     (1000) james     (1000)     1823 2020-03-06 19:19:00.000000 flake8-aaa-0.9.0/src/flake8_aaa/act_node.py
+-rw-r--r--   0 james     (1000) james     (1000)     2598 2020-02-13 10:22:50.000000 flake8-aaa-0.9.0/src/flake8_aaa/block.py
+-rw-r--r--   0 james     (1000) james     (1000)     1697 2020-02-13 10:22:50.000000 flake8-aaa-0.9.0/src/flake8_aaa/checker.py
+-rw-r--r--   0 james     (1000) james     (1000)     1081 2020-02-13 10:22:50.000000 flake8-aaa-0.9.0/src/flake8_aaa/command_line.py
+-rw-r--r--   0 james     (1000) james     (1000)     1259 2020-02-13 10:22:50.000000 flake8-aaa-0.9.0/src/flake8_aaa/exceptions.py
+-rw-r--r--   0 james     (1000) james     (1000)     7034 2020-03-06 19:19:00.000000 flake8-aaa-0.9.0/src/flake8_aaa/function.py
+-rw-r--r--   0 james     (1000) james     (1000)     6545 2020-03-06 20:11:53.000000 flake8-aaa-0.9.0/src/flake8_aaa/helpers.py
+-rw-r--r--   0 james     (1000) james     (1000)     5815 2020-03-06 19:19:00.000000 flake8-aaa-0.9.0/src/flake8_aaa/line_markers.py
+-rw-r--r--   0 james     (1000) james     (1000)      399 2020-03-06 19:19:00.000000 flake8-aaa-0.9.0/src/flake8_aaa/multi_node_block.py
+-rw-r--r--   0 james     (1000) james     (1000)      694 2020-03-06 19:19:00.000000 flake8-aaa-0.9.0/src/flake8_aaa/types.py
+drwxr-xr-x   0 james     (1000) james     (1000)        0 2020-03-07 18:31:44.000000 flake8-aaa-0.9.0/src/flake8_aaa.egg-info/
+-rw-r--r--   0 james     (1000) james     (1000)     5103 2020-03-07 18:31:44.000000 flake8-aaa-0.9.0/src/flake8_aaa.egg-info/PKG-INFO
+-rw-r--r--   0 james     (1000) james     (1000)      678 2020-03-07 18:31:44.000000 flake8-aaa-0.9.0/src/flake8_aaa.egg-info/SOURCES.txt
+-rw-r--r--   0 james     (1000) james     (1000)        1 2020-03-07 18:31:44.000000 flake8-aaa-0.9.0/src/flake8_aaa.egg-info/dependency_links.txt
+-rw-r--r--   0 james     (1000) james     (1000)       45 2020-03-07 18:31:44.000000 flake8-aaa-0.9.0/src/flake8_aaa.egg-info/entry_points.txt
+-rw-r--r--   0 james     (1000) james     (1000)        1 2020-02-24 09:59:12.000000 flake8-aaa-0.9.0/src/flake8_aaa.egg-info/not-zip-safe
+-rw-r--r--   0 james     (1000) james     (1000)       13 2020-03-07 18:31:44.000000 flake8-aaa-0.9.0/src/flake8_aaa.egg-info/requires.txt
+-rw-r--r--   0 james     (1000) james     (1000)       11 2020-03-07 18:31:44.000000 flake8-aaa-0.9.0/src/flake8_aaa.egg-info/top_level.txt
```

### Comparing `flake8-aaa-0.8.1/PKG-INFO` & `flake8-aaa-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: flake8-aaa
-Version: 0.8.1
+Version: 0.9.0
 Summary: A linter for Python tests
 Home-page: https://github.com/jamescooke/flake8-aaa
 Author: James Cooke
 Author-email: github@jamescooke.info
 License: MIT
 Description: .. image:: https://img.shields.io/travis/jamescooke/flake8-aaa/master.svg
             :target: https://travis-ci.org/jamescooke/flake8-aaa/branches
```

### Comparing `flake8-aaa-0.8.1/LICENSE` & `flake8-aaa-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-aaa-0.8.1/setup.py` & `flake8-aaa-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `flake8-aaa-0.8.1/src/flake8_aaa.egg-info/SOURCES.txt` & `flake8-aaa-0.9.0/src/flake8_aaa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flake8-aaa-0.8.1/src/flake8_aaa.egg-info/PKG-INFO` & `flake8-aaa-0.9.0/src/flake8_aaa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: flake8-aaa
-Version: 0.8.1
+Version: 0.9.0
 Summary: A linter for Python tests
 Home-page: https://github.com/jamescooke/flake8-aaa
 Author: James Cooke
 Author-email: github@jamescooke.info
 License: MIT
 Description: .. image:: https://img.shields.io/travis/jamescooke/flake8-aaa/master.svg
             :target: https://travis-ci.org/jamescooke/flake8-aaa/branches
```

### Comparing `flake8-aaa-0.8.1/src/flake8_aaa/helpers.py` & `flake8-aaa-0.9.0/src/flake8_aaa/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,26 @@
 import ast
 import os
+import re
 from typing import List, Set
 
 from asttokens.util import Token
 
+test_file_pattern = re.compile(r'test(_.*|s)?\.py$')
+
 
 def is_test_file(filename: str) -> bool:
     """
     Check that path to file being checked passed by flake8 looks like a pytest
     test file.
-
-    Examples:
-        1.  Non-test files give False.
-        >>> is_test_file('./test.py')
-        False
-        >>> is_test_file('./helper.py')
-        False
-        >>> is_test_file('tests/conftest.py')
-        False
-
-        2.  Finds files that start with 'test_' to be test files.
-        >>> is_test_file('./test_helpers.py')
-        True
     """
-    return os.path.basename(filename).startswith('test_')
+    return bool(test_file_pattern.match(os.path.basename(filename)))
 
 
 def first_non_blank_char(line: str) -> int:
-    """
-    Examples:
-        1.  Empty string has no non-blank chars.
-        >>> first_non_blank_char('')
-        0
-
-        2.  First char after whitespace or tabs works.
-        >>> first_non_blank_char('    return')
-        4
-        >>> first_non_blank_char('        return')
-        8
-    """
     for pos, char in enumerate(line):
         if not char.isspace():
             return pos
     return 0
 
 
 class TestFuncLister(ast.NodeVisitor):
```

### Comparing `flake8-aaa-0.8.1/src/flake8_aaa/__main__.py` & `flake8-aaa-0.9.0/src/flake8_aaa/__main__.py`

 * *Files identical despite different names*

### Comparing `flake8-aaa-0.8.1/src/flake8_aaa/exceptions.py` & `flake8-aaa-0.9.0/src/flake8_aaa/exceptions.py`

 * *Files identical despite different names*

### Comparing `flake8-aaa-0.8.1/src/flake8_aaa/block.py` & `flake8-aaa-0.9.0/src/flake8_aaa/block.py`

 * *Files identical despite different names*

### Comparing `flake8-aaa-0.8.1/src/flake8_aaa/act_node.py` & `flake8-aaa-0.9.0/src/flake8_aaa/act_node.py`

 * *Files identical despite different names*

### Comparing `flake8-aaa-0.8.1/src/flake8_aaa/types.py` & `flake8-aaa-0.9.0/src/flake8_aaa/types.py`

 * *Files identical despite different names*

### Comparing `flake8-aaa-0.8.1/src/flake8_aaa/checker.py` & `flake8-aaa-0.9.0/src/flake8_aaa/checker.py`

 * *Files identical despite different names*

### Comparing `flake8-aaa-0.8.1/src/flake8_aaa/line_markers.py` & `flake8-aaa-0.9.0/src/flake8_aaa/line_markers.py`

 * *Files identical despite different names*

### Comparing `flake8-aaa-0.8.1/src/flake8_aaa/function.py` & `flake8-aaa-0.9.0/src/flake8_aaa/function.py`

 * *Files identical despite different names*

### Comparing `flake8-aaa-0.8.1/src/flake8_aaa/command_line.py` & `flake8-aaa-0.9.0/src/flake8_aaa/command_line.py`

 * *Files identical despite different names*

### Comparing `flake8-aaa-0.8.1/README.rst` & `flake8-aaa-0.9.0/README.rst`

 * *Files identical despite different names*

