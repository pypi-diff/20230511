# Comparing `tmp/boolrule-0.3.3.tar.gz` & `tmp/boolrule-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boolrule-0.3.3.tar", last modified: Thu Jul 15 11:57:07 2021, max compression
+gzip compressed data, was "boolrule-0.3.4.tar", last modified: Fri Sep 24 07:09:24 2021, max compression
```

## Comparing `boolrule-0.3.3.tar` & `boolrule-0.3.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-15 11:57:07.405202 boolrule-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-07-15 11:56:57.000000 boolrule-0.3.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3163 2021-07-15 11:56:57.000000 boolrule-0.3.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      847 2021-07-15 11:56:57.000000 boolrule-0.3.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-07-15 11:56:57.000000 boolrule-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      290 2021-07-15 11:56:57.000000 boolrule-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3377 2021-07-15 11:57:07.405202 boolrule-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2021-07-15 11:56:57.000000 boolrule-0.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-15 11:57:07.401202 boolrule-0.3.3/boolrule/
--rw-r--r--   0 runner    (1001) docker     (121)      203 2021-07-15 11:56:57.000000 boolrule-0.3.3/boolrule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7339 2021-07-15 11:56:57.000000 boolrule-0.3.3/boolrule/boolrule.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-15 11:56:57.000000 boolrule-0.3.3/boolrule/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-15 11:57:07.401202 boolrule-0.3.3/boolrule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3377 2021-07-15 11:57:07.000000 boolrule-0.3.3/boolrule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      580 2021-07-15 11:57:07.000000 boolrule-0.3.3/boolrule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-15 11:57:07.000000 boolrule-0.3.3/boolrule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-15 11:57:06.000000 boolrule-0.3.3/boolrule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-07-15 11:57:07.000000 boolrule-0.3.3/boolrule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-07-15 11:57:07.000000 boolrule-0.3.3/boolrule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-15 11:57:07.405202 boolrule-0.3.3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6770 2021-07-15 11:56:57.000000 boolrule-0.3.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      229 2021-07-15 11:56:57.000000 boolrule-0.3.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-07-15 11:56:57.000000 boolrule-0.3.3/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     8463 2021-07-15 11:56:57.000000 boolrule-0.3.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-07-15 11:56:57.000000 boolrule-0.3.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3253 2021-07-15 11:56:57.000000 boolrule-0.3.3/docs/expressions.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-07-15 11:56:57.000000 boolrule-0.3.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      777 2021-07-15 11:56:57.000000 boolrule-0.3.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2021-07-15 11:56:57.000000 boolrule-0.3.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6463 2021-07-15 11:56:57.000000 boolrule-0.3.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-07-15 11:56:57.000000 boolrule-0.3.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2021-07-15 11:56:57.000000 boolrule-0.3.3/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)      405 2021-07-15 11:57:07.405202 boolrule-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2021-07-15 11:56:57.000000 boolrule-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-15 11:57:07.405202 boolrule-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-07-15 11:56:57.000000 boolrule-0.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3709 2021-07-15 11:56:57.000000 boolrule-0.3.3/tests/test_boolrule.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-24 07:09:24.308197 boolrule-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-09-24 07:09:16.000000 boolrule-0.3.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3163 2021-09-24 07:09:16.000000 boolrule-0.3.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2021-09-24 07:09:16.000000 boolrule-0.3.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-09-24 07:09:16.000000 boolrule-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2021-09-24 07:09:16.000000 boolrule-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3547 2021-09-24 07:09:24.308197 boolrule-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1665 2021-09-24 07:09:16.000000 boolrule-0.3.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-24 07:09:24.308197 boolrule-0.3.4/boolrule/
+-rw-r--r--   0 runner    (1001) docker     (121)      203 2021-09-24 07:09:16.000000 boolrule-0.3.4/boolrule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7366 2021-09-24 07:09:16.000000 boolrule-0.3.4/boolrule/boolrule.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-24 07:09:16.000000 boolrule-0.3.4/boolrule/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-24 07:09:24.308197 boolrule-0.3.4/boolrule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3547 2021-09-24 07:09:24.000000 boolrule-0.3.4/boolrule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      580 2021-09-24 07:09:24.000000 boolrule-0.3.4/boolrule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-24 07:09:24.000000 boolrule-0.3.4/boolrule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-24 07:09:24.000000 boolrule-0.3.4/boolrule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-09-24 07:09:24.000000 boolrule-0.3.4/boolrule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-09-24 07:09:24.000000 boolrule-0.3.4/boolrule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-24 07:09:24.308197 boolrule-0.3.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     6770 2021-09-24 07:09:16.000000 boolrule-0.3.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2021-09-24 07:09:16.000000 boolrule-0.3.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-09-24 07:09:16.000000 boolrule-0.3.4/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8463 2021-09-24 07:09:16.000000 boolrule-0.3.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-09-24 07:09:16.000000 boolrule-0.3.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3253 2021-09-24 07:09:16.000000 boolrule-0.3.4/docs/expressions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-09-24 07:09:16.000000 boolrule-0.3.4/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2021-09-24 07:09:16.000000 boolrule-0.3.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1134 2021-09-24 07:09:16.000000 boolrule-0.3.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6463 2021-09-24 07:09:16.000000 boolrule-0.3.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-09-24 07:09:16.000000 boolrule-0.3.4/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1545 2021-09-24 07:09:16.000000 boolrule-0.3.4/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2021-09-24 07:09:24.308197 boolrule-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1378 2021-09-24 07:09:16.000000 boolrule-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-24 07:09:24.308197 boolrule-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-09-24 07:09:16.000000 boolrule-0.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3961 2021-09-24 07:09:16.000000 boolrule-0.3.4/tests/test_boolrule.py
```

### Comparing `boolrule-0.3.3/CONTRIBUTING.rst` & `boolrule-0.3.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `boolrule-0.3.3/HISTORY.rst` & `boolrule-0.3.4/HISTORY.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 =======
 History
 =======
 
+0.3.4 (2021-09-24)
+==================
+
+* Fixed error caused by early return when evaluating nested expressions.
+
+
 0.3.3 (2021-07-15)
+==================
 
 * Upgrade dependencies.
 
 
 0.3.2 (2020-09-23)
 ==================
```

### Comparing `boolrule-0.3.3/LICENSE` & `boolrule-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `boolrule-0.3.3/PKG-INFO` & `boolrule-0.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boolrule
-Version: 0.3.3
+Version: 0.3.4
 Summary: Simple boolean expression evaluation engine
 Home-page: https://github.com/tailsdotcom/boolrule
 Author: Steve Webster
 Author-email: spjwebster@gmail.com
 License: MIT license
 Keywords: boolrule boolean expression
 Platform: UNKNOWN
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Text Processing :: General
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ========
 boolrule
 ========
 
@@ -87,15 +88,22 @@
 
 
 
 =======
 History
 =======
 
+0.3.4 (2021-09-24)
+==================
+
+* Fixed error caused by early return when evaluating nested expressions.
+
+
 0.3.3 (2021-07-15)
+==================
 
 * Upgrade dependencies.
 
 
 0.3.2 (2020-09-23)
 ==================
```

### Comparing `boolrule-0.3.3/README.rst` & `boolrule-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `boolrule-0.3.3/boolrule/boolrule.py` & `boolrule-0.3.4/boolrule/boolrule.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,16 @@
                 if token == 'or' and passed:
                     return True
                 elif token == 'and' and not passed:
                     return False
                 continue
 
             if not token.getName():
-                return self._test_tokens(token, context)
+                passed = self._test_tokens(token, context)
+                continue
 
             items = token.asDict()
 
             operator = items['operator']
             lval = self._expand_val(items['lval'][0], context)
             rval = self._expand_val(items['rval'][0], context)
```

### Comparing `boolrule-0.3.3/boolrule.egg-info/PKG-INFO` & `boolrule-0.3.4/boolrule.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boolrule
-Version: 0.3.3
+Version: 0.3.4
 Summary: Simple boolean expression evaluation engine
 Home-page: https://github.com/tailsdotcom/boolrule
 Author: Steve Webster
 Author-email: spjwebster@gmail.com
 License: MIT license
 Keywords: boolrule boolean expression
 Platform: UNKNOWN
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Text Processing :: General
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ========
 boolrule
 ========
 
@@ -87,15 +88,22 @@
 
 
 
 =======
 History
 =======
 
+0.3.4 (2021-09-24)
+==================
+
+* Fixed error caused by early return when evaluating nested expressions.
+
+
 0.3.3 (2021-07-15)
+==================
 
 * Upgrade dependencies.
 
 
 0.3.2 (2020-09-23)
 ==================
```

### Comparing `boolrule-0.3.3/boolrule.egg-info/SOURCES.txt` & `boolrule-0.3.4/boolrule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boolrule-0.3.3/docs/Makefile` & `boolrule-0.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `boolrule-0.3.3/docs/conf.py` & `boolrule-0.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `boolrule-0.3.3/docs/expressions.rst` & `boolrule-0.3.4/docs/expressions.rst`

 * *Files identical despite different names*

### Comparing `boolrule-0.3.3/docs/index.rst` & `boolrule-0.3.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `boolrule-0.3.3/docs/installation.rst` & `boolrule-0.3.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `boolrule-0.3.3/docs/make.bat` & `boolrule-0.3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `boolrule-0.3.3/docs/usage.rst` & `boolrule-0.3.4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `boolrule-0.3.3/setup.py` & `boolrule-0.3.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 
 test_requirements = [
     'pytest'
 ]
 
 setup(
     name='boolrule',
-    version='0.3.3',
+    version='0.3.4',
     description="Simple boolean expression evaluation engine",
     long_description=readme + '\n\n' + history,
+    long_description_content_type='text/x-rst',
     author="Steve Webster",
     author_email='spjwebster@gmail.com',
     url='https://github.com/tailsdotcom/boolrule',
     packages=[
         'boolrule',
     ],
     package_dir={'boolrule':
```

### Comparing `boolrule-0.3.3/tests/test_boolrule.py` & `boolrule-0.3.4/tests/test_boolrule.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,21 @@
     ('5 > 3 and (3 > 5 or 3 > 1)', True),
     ('5 > 3 and (3 > 5 and 3 < 1)', False),
 ])
 def test_nested_logical_combinations(s, expected):
     boolrule = BoolRule(s)
     assert boolrule.test() == expected
 
+@pytest.mark.parametrize('s,expected', [
+    ('(1=1 or 2=2) and (3 = 3)', True),
+    ('(1=1 or 2=2) and (3 = 4)', False),
+])
+def test_nested_logical_combinations_and_error(s, expected):
+    boolrule = BoolRule(s)
+    assert boolrule.test() == expected
 
 @pytest.mark.parametrize('s,context,expected', [
     ('foo = "bar" AND baz > 10', {'foo': 'bar', 'baz': 20}, True),
     ('foo = "bar" AND baz > 10', {'foo': 'bar', 'baz': 9}, False),
     (
         'foo = "bar" AND ("a" = "b" OR baz > 10)',
         {'foo': 'bar', 'baz': 11}, True
```

