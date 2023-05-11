# Comparing `tmp/edman-2023.5.10.1.tar.gz` & `tmp/edman-2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman-2023.5.10.1.tar", last modified: Wed May 10 01:26:59 2023, max compression
+gzip compressed data, was "edman-2023.5.8.tar", last modified: Mon May  8 02:04:22 2023, max compression
```

## Comparing `edman-2023.5.10.1.tar` & `edman-2023.5.8.tar`

### file list

```diff
@@ -1,44 +1,30 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-10 01:26:59.625815 edman-2023.5.10.1/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-02-17 05:03:50.000000 edman-2023.5.10.1/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7615 2023-05-10 01:26:59.625815 edman-2023.5.10.1/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)     6049 2023-01-20 03:28:32.000000 edman-2023.5.10.1/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-10 01:26:59.615815 edman-2023.5.10.1/edman/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      167 2023-05-09 07:38:50.000000 edman-2023.5.10.1/edman/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1373 2023-03-15 05:16:00.000000 edman-2023.5.10.1/edman/config.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    16457 2023-03-15 05:16:00.000000 edman-2023.5.10.1/edman/convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    47757 2023-04-05 05:00:36.000000 edman-2023.5.10.1/edman/db.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)      644 2022-04-13 07:00:02.000000 edman-2023.5.10.1/edman/exceptions.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    21800 2023-05-08 02:02:11.000000 edman-2023.5.10.1/edman/file.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1520 2023-03-09 05:51:32.000000 edman-2023.5.10.1/edman/json_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     9907 2023-04-10 07:58:11.000000 edman-2023.5.10.1/edman/search.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    10958 2023-03-09 05:51:32.000000 edman-2023.5.10.1/edman/utils.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-10 01:26:59.615815 edman-2023.5.10.1/edman.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7615 2023-05-10 01:26:59.000000 edman-2023.5.10.1/edman.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      738 2023-05-10 01:26:59.000000 edman-2023.5.10.1/edman.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-10 01:26:59.000000 edman-2023.5.10.1/edman.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       54 2023-05-10 01:26:59.000000 edman-2023.5.10.1/edman.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       34 2023-05-10 01:26:59.000000 edman-2023.5.10.1/edman.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)      853 2023-05-10 01:24:33.000000 edman-2023.5.10.1/pyproject.toml
--rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2023-05-10 01:26:59.625815 edman-2023.5.10.1/setup.cfg
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-10 01:26:59.615815 edman-2023.5.10.1/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    12303 2022-04-13 07:00:02.000000 edman-2023.5.10.1/tests/test_convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    86854 2023-04-20 03:03:49.000000 edman-2023.5.10.1/tests/test_db.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    36850 2023-05-08 02:02:11.000000 edman-2023.5.10.1/tests/test_file.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     5837 2023-03-09 05:51:32.000000 edman-2023.5.10.1/tests/test_multiuser.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    19062 2023-04-05 05:00:36.000000 edman-2023.5.10.1/tests/test_search.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7898 2022-04-13 07:00:02.000000 edman-2023.5.10.1/tests/test_utils.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-10 01:26:59.615815 edman-2023.5.10.1/venv/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-10 01:26:59.625815 edman-2023.5.10.1/venv/bin/
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1725 2023-04-07 00:37:51.000000 edman-2023.5.10.1/venv/bin/jp.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      632 2023-05-10 00:30:10.000000 edman-2023.5.10.1/venv/bin/rst2html.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      754 2023-05-10 00:30:10.000000 edman-2023.5.10.1/venv/bin/rst2html4.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1089 2023-05-10 00:30:10.000000 edman-2023.5.10.1/venv/bin/rst2html5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      831 2023-05-10 00:30:10.000000 edman-2023.5.10.1/venv/bin/rst2latex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      654 2023-05-10 00:30:10.000000 edman-2023.5.10.1/venv/bin/rst2man.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      820 2023-05-10 00:30:10.000000 edman-2023.5.10.1/venv/bin/rst2odt.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     2176 2023-05-10 00:30:10.000000 edman-2023.5.10.1/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      639 2023-05-10 00:30:10.000000 edman-2023.5.10.1/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      675 2023-05-10 00:30:10.000000 edman-2023.5.10.1/venv/bin/rst2s5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      911 2023-05-10 00:30:10.000000 edman-2023.5.10.1/venv/bin/rst2xetex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      640 2023-05-10 00:30:10.000000 edman-2023.5.10.1/venv/bin/rst2xml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      708 2023-05-10 00:30:10.000000 edman-2023.5.10.1/venv/bin/rstpep2html.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-02-17 05:03:50.000000 edman-2023.5.8/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       19 2022-04-13 07:00:02.000000 edman-2023.5.8/MANIFEST.in
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6379 2023-05-08 02:04:22.028113 edman-2023.5.8/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6049 2023-01-20 03:28:32.000000 edman-2023.5.8/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/edman/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      167 2022-04-13 07:00:02.000000 edman-2023.5.8/edman/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1373 2023-03-15 05:16:00.000000 edman-2023.5.8/edman/config.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    16457 2023-03-15 05:16:00.000000 edman-2023.5.8/edman/convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    47757 2023-04-05 05:00:36.000000 edman-2023.5.8/edman/db.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      644 2022-04-13 07:00:02.000000 edman-2023.5.8/edman/exceptions.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    21800 2023-05-08 02:02:11.000000 edman-2023.5.8/edman/file.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1520 2023-03-09 05:51:32.000000 edman-2023.5.8/edman/json_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     9907 2023-04-10 07:58:11.000000 edman-2023.5.8/edman/search.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    10958 2023-03-09 05:51:32.000000 edman-2023.5.8/edman/utils.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/edman.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6379 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      470 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       54 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        6 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      707 2023-05-08 02:04:22.028113 edman-2023.5.8/setup.cfg
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       41 2022-04-13 07:00:02.000000 edman-2023.5.8/setup.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    12303 2022-04-13 07:00:02.000000 edman-2023.5.8/tests/test_convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    86854 2023-04-20 03:03:49.000000 edman-2023.5.8/tests/test_db.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    36850 2023-05-08 02:02:11.000000 edman-2023.5.8/tests/test_file.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     5837 2023-03-09 05:51:32.000000 edman-2023.5.8/tests/test_multiuser.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    19062 2023-04-05 05:00:36.000000 edman-2023.5.8/tests/test_search.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     7898 2022-04-13 07:00:02.000000 edman-2023.5.8/tests/test_utils.py
```

### Comparing `edman-2023.5.10.1/LICENSE.txt` & `edman-2023.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman-2023.5.10.1/PKG-INFO` & `edman-2023.5.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 Metadata-Version: 2.1
 Name: edman
-Version: 2023.5.10.1
+Version: 2023.5.8
 Summary: KEK IMSS SBRC/PF Experimental Data Management System
-Author-email: Masaki Ohno <masakio@post.kek.jp>
+Home-page: https://github.com/ryde/edman
+Author: Masaki Ohno
+Author-email: masakio@post.kek.jp
 License: MIT License
-        
-        Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Yusuke Yamada, Masaki Ohno
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: documentation, https://ryde.github.io/edman/
-Project-URL: repository, https://github.com/ryde/edman
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 edman
 =====
```

### Comparing `edman-2023.5.10.1/README.rst` & `edman-2023.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `edman-2023.5.10.1/edman/config.py` & `edman-2023.5.8/edman/config.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.10.1/edman/convert.py` & `edman-2023.5.8/edman/convert.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.10.1/edman/db.py` & `edman-2023.5.8/edman/db.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.10.1/edman/exceptions.py` & `edman-2023.5.8/edman/exceptions.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.10.1/edman/file.py` & `edman-2023.5.8/edman/file.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.10.1/edman/json_manager.py` & `edman-2023.5.8/edman/json_manager.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.10.1/edman/search.py` & `edman-2023.5.8/edman/search.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.10.1/edman/utils.py` & `edman-2023.5.8/edman/utils.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.10.1/edman.egg-info/PKG-INFO` & `edman-2023.5.8/edman.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 Metadata-Version: 2.1
 Name: edman
-Version: 2023.5.10.1
+Version: 2023.5.8
 Summary: KEK IMSS SBRC/PF Experimental Data Management System
-Author-email: Masaki Ohno <masakio@post.kek.jp>
+Home-page: https://github.com/ryde/edman
+Author: Masaki Ohno
+Author-email: masakio@post.kek.jp
 License: MIT License
-        
-        Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Yusuke Yamada, Masaki Ohno
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: documentation, https://ryde.github.io/edman/
-Project-URL: repository, https://github.com/ryde/edman
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 edman
 =====
```

### Comparing `edman-2023.5.10.1/tests/test_convert.py` & `edman-2023.5.8/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.10.1/tests/test_db.py` & `edman-2023.5.8/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.10.1/tests/test_file.py` & `edman-2023.5.8/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.10.1/tests/test_multiuser.py` & `edman-2023.5.8/tests/test_multiuser.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.10.1/tests/test_search.py` & `edman-2023.5.8/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.10.1/tests/test_utils.py` & `edman-2023.5.8/tests/test_utils.py`

 * *Files identical despite different names*

