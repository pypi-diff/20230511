# Comparing `tmp/fazy-0.0.4.tar.gz` & `tmp/fazy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fazy-0.0.4.tar", last modified: Tue Apr 25 09:42:26 2023, max compression
+gzip compressed data, was "fazy-0.0.5.tar", last modified: Thu May 11 04:31:15 2023, max compression
```

## Comparing `fazy-0.0.4.tar` & `fazy-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-25 09:42:26.057125 fazy-0.0.4/
--rw-r--r--   0 pomponchik   (501) staff       (20)     1067 2023-04-12 12:31:37.000000 fazy-0.0.4/LICENSE
--rw-r--r--   0 pomponchik   (501) staff       (20)    14426 2023-04-25 09:42:26.056899 fazy-0.0.4/PKG-INFO
--rw-r--r--   0 pomponchik   (501) staff       (20)    13874 2023-04-25 09:34:57.000000 fazy-0.0.4/README.md
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-25 09:42:26.055685 fazy-0.0.4/f/
--rw-r--r--   0 pomponchik   (501) staff       (20)       98 2023-04-20 12:08:45.000000 fazy-0.0.4/f/__init__.py
--rw-r--r--   0 pomponchik   (501) staff       (20)      286 2023-04-20 12:02:43.000000 fazy-0.0.4/f/chain_unit.py
--rw-r--r--   0 pomponchik   (501) staff       (20)     6839 2023-04-20 12:04:13.000000 fazy-0.0.4/f/lazy_string.py
--rw-r--r--   0 pomponchik   (501) staff       (20)     5166 2023-04-25 09:22:32.000000 fazy-0.0.4/f/proxy_module.py
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-25 09:42:26.056641 fazy-0.0.4/fazy.egg-info/
--rw-r--r--   0 pomponchik   (501) staff       (20)    14426 2023-04-25 09:42:25.000000 fazy-0.0.4/fazy.egg-info/PKG-INFO
--rw-r--r--   0 pomponchik   (501) staff       (20)      203 2023-04-25 09:42:26.000000 fazy-0.0.4/fazy.egg-info/SOURCES.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)        1 2023-04-25 09:42:25.000000 fazy-0.0.4/fazy.egg-info/dependency_links.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)        2 2023-04-25 09:42:25.000000 fazy-0.0.4/fazy.egg-info/top_level.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)       38 2023-04-25 09:42:26.057179 fazy-0.0.4/setup.cfg
--rw-r--r--   0 pomponchik   (501) staff       (20)      833 2023-04-21 18:39:23.000000 fazy-0.0.4/setup.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-11 04:31:15.826790 fazy-0.0.5/
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1067 2023-04-12 12:31:37.000000 fazy-0.0.5/LICENSE
+-rw-r--r--   0 pomponchik   (501) staff       (20)    14426 2023-05-11 04:31:15.826570 fazy-0.0.5/PKG-INFO
+-rw-r--r--   0 pomponchik   (501) staff       (20)    13874 2023-04-25 09:34:57.000000 fazy-0.0.5/README.md
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-11 04:31:15.825200 fazy-0.0.5/f/
+-rw-r--r--   0 pomponchik   (501) staff       (20)       98 2023-04-20 12:08:45.000000 fazy-0.0.5/f/__init__.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)      286 2023-04-20 12:02:43.000000 fazy-0.0.5/f/chain_unit.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     6839 2023-04-20 12:04:13.000000 fazy-0.0.5/f/lazy_string.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     5202 2023-05-11 04:10:37.000000 fazy-0.0.5/f/proxy_module.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-11 04:31:15.826267 fazy-0.0.5/fazy.egg-info/
+-rw-r--r--   0 pomponchik   (501) staff       (20)    14426 2023-05-11 04:31:15.000000 fazy-0.0.5/fazy.egg-info/PKG-INFO
+-rw-r--r--   0 pomponchik   (501) staff       (20)      203 2023-05-11 04:31:15.000000 fazy-0.0.5/fazy.egg-info/SOURCES.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)        1 2023-05-11 04:31:15.000000 fazy-0.0.5/fazy.egg-info/dependency_links.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)        2 2023-05-11 04:31:15.000000 fazy-0.0.5/fazy.egg-info/top_level.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)       38 2023-05-11 04:31:15.826846 fazy-0.0.5/setup.cfg
+-rw-r--r--   0 pomponchik   (501) staff       (20)      833 2023-05-11 04:29:26.000000 fazy-0.0.5/setup.py
```

### Comparing `fazy-0.0.4/LICENSE` & `fazy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fazy-0.0.4/PKG-INFO` & `fazy-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fazy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Lazy f-strings for everyone
 Home-page: https://github.com/pomponchik/fazy
 Author: Evgeniy Blinov
 Author-email: zheni-b@yandex.ru
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `fazy-0.0.4/README.md` & `fazy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fazy-0.0.4/f/lazy_string.py` & `fazy-0.0.5/f/lazy_string.py`

 * *Files identical despite different names*

### Comparing `fazy-0.0.4/f/proxy_module.py` & `fazy-0.0.5/f/proxy_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
                         for arg in node.args:
                             ConstantVisitor().visit(arg)
                         for keyword in node.keywords:
                             ConstantVisitor().visit(keyword.value)
 
         ConstantVisitor().visit(ast_of_code)
 
-        if not flag:
+        if not flag and not (sys.version_info < (3, 8)):
             raise SyntaxError('Unsafe use of a variable as a template.')
 
 
     @staticmethod
     def startswith(iterable, second_iterable):
         if len(iterable) < len(second_iterable):
             return False
```

### Comparing `fazy-0.0.4/fazy.egg-info/PKG-INFO` & `fazy-0.0.5/fazy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fazy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Lazy f-strings for everyone
 Home-page: https://github.com/pomponchik/fazy
 Author: Evgeniy Blinov
 Author-email: zheni-b@yandex.ru
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `fazy-0.0.4/setup.py` & `fazy-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md', 'r') as readme_file:
     readme = readme_file.read()
 
 requirements = []
 
 setup(
     name='fazy',
-    version='0.0.4',
+    version='0.0.5',
     author='Evgeniy Blinov',
     author_email='zheni-b@yandex.ru',
     description='Lazy f-strings for everyone',
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://github.com/pomponchik/fazy',
     packages=find_packages(exclude=('tests',)),
```

