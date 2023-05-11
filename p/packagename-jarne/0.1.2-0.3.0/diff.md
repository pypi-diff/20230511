# Comparing `tmp/packagename_jarne-0.1.2.tar.gz` & `tmp/packagename_jarne-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packagename_jarne-0.1.2.tar", last modified: Tue Apr 18 07:41:26 2023, max compression
+gzip compressed data, was "packagename_jarne-0.3.0.tar", last modified: Thu May 11 15:16:12 2023, max compression
```

## Comparing `packagename_jarne-0.1.2.tar` & `packagename_jarne-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:41:26.904733 packagename_jarne-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-18 07:41:05.000000 packagename_jarne-0.1.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-18 07:41:26.904733 packagename_jarne-0.1.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-04-18 07:41:05.000000 packagename_jarne-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:41:26.904733 packagename_jarne-0.1.2/packagename_jarne.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-18 07:41:26.000000 packagename_jarne-0.1.2/packagename_jarne.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-18 07:41:26.000000 packagename_jarne-0.1.2/packagename_jarne.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:41:26.000000 packagename_jarne-0.1.2/packagename_jarne.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-18 07:41:26.000000 packagename_jarne-0.1.2/packagename_jarne.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-18 07:41:26.000000 packagename_jarne-0.1.2/packagename_jarne.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 07:41:26.904733 packagename_jarne-0.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3611 2023-04-18 07:41:05.000000 packagename_jarne-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:41:26.904733 packagename_jarne-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-18 07:41:05.000000 packagename_jarne-0.1.2/tests/test_PID.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-18 07:41:05.000000 packagename_jarne-0.1.2/tests/test_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:12.538192 packagename_jarne-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-11 15:15:27.000000 packagename_jarne-0.3.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-11 15:16:12.538192 packagename_jarne-0.3.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-05-11 15:15:27.000000 packagename_jarne-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:12.538192 packagename_jarne-0.3.0/packagename_jarne.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-11 15:16:12.000000 packagename_jarne-0.3.0/packagename_jarne.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-11 15:16:12.000000 packagename_jarne-0.3.0/packagename_jarne.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:16:12.000000 packagename_jarne-0.3.0/packagename_jarne.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-11 15:16:12.000000 packagename_jarne-0.3.0/packagename_jarne.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-11 15:16:12.000000 packagename_jarne-0.3.0/packagename_jarne.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:16:12.538192 packagename_jarne-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3714 2023-05-11 15:15:27.000000 packagename_jarne-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:12.538192 packagename_jarne-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-11 15:15:27.000000 packagename_jarne-0.3.0/tests/test_PID.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-11 15:15:27.000000 packagename_jarne-0.3.0/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-11 15:15:27.000000 packagename_jarne-0.3.0/tests/test_submodule.py
```

### Comparing `packagename_jarne-0.1.2/LICENCE` & `packagename_jarne-0.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `packagename_jarne-0.1.2/PKG-INFO` & `packagename_jarne-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: packagename_jarne
-Version: 0.1.2
+Version: 0.3.0
 Summary: Example project for sphinx python.
 Home-page: https://github.com/jarneamerlinck/python-sphinx-documentation
 Author: Jarne Amerlinck
 Author-email: jarneamerlinck@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENCE
```

### Comparing `packagename_jarne-0.1.2/README.md` & `packagename_jarne-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `packagename_jarne-0.1.2/packagename_jarne.egg-info/PKG-INFO` & `packagename_jarne-0.3.0/packagename_jarne.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: packagename-jarne
-Version: 0.1.2
+Version: 0.3.0
 Summary: Example project for sphinx python.
 Home-page: https://github.com/jarneamerlinck/python-sphinx-documentation
 Author: Jarne Amerlinck
 Author-email: jarneamerlinck@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENCE
```

### Comparing `packagename_jarne-0.1.2/setup.py` & `packagename_jarne-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 	'psutil'
 ]
 
 
 
 # What packages are optional?
 EXTRAS = {
-	'docs': [ 'Sphinx==6.1.3', 'sphinx-markdown-builder==0.5.5','sphinx-press-theme', 'twine',
-          'pytest']
+	'docs': ['Sphinx>=6.1.3', 'sphinx-markdown-builder>=0.5.5', 'sphinx_autodoc_typehints>=1.22', 
+			 'sphinx-press-theme>=0.8.0', 'sphinx_favicon', 'twine', 'graphviz']
 }
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License, remember to change the Trove Classifier for that!
 
@@ -118,16 +118,17 @@
 	include_package_data=True,
 	license='MIT',
 	classifiers=[
 		# Trove classifiers
 		# Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
 		'License :: OSI Approved :: MIT License',
 		'Programming Language :: Python',
-		'Programming Language :: Python :: 3',
-		'Programming Language :: Python :: 3.6',
+		'Programming Language :: Python :: 3.9',
+		'Programming Language :: Python :: 3.10',
+		'Programming Language :: Python :: 3.11',
 		'Programming Language :: Python :: Implementation :: CPython',
 		'Programming Language :: Python :: Implementation :: PyPy'
 	],
 	# $ setup.py publish support.
 	cmdclass={
 		'upload': UploadCommand,
 	},
```

