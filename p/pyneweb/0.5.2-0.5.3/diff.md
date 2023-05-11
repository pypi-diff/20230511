# Comparing `tmp/pyneweb-0.5.2.tar.gz` & `tmp/pyneweb-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneweb-0.5.2.tar", last modified: Thu May 11 12:17:21 2023, max compression
+gzip compressed data, was "pyneweb-0.5.3.tar", last modified: Thu May 11 12:52:57 2023, max compression
```

## Comparing `pyneweb-0.5.2.tar` & `pyneweb-0.5.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 12:17:21.803646 pyneweb-0.5.2/
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-05-04 18:35:57.000000 pyneweb-0.5.2/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-11 12:17:21.803406 pyneweb-0.5.2/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4042 2023-05-04 18:48:17.000000 pyneweb-0.5.2/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 12:17:21.801247 pyneweb-0.5.2/logic/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-02 16:20:24.000000 pyneweb-0.5.2/logic/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2431 2023-05-11 12:16:26.000000 pyneweb-0.5.2/logic/cli.py
--rw-r--r--   0 ahmad      (501) staff       (20)     5504 2023-05-11 11:32:24.000000 pyneweb-0.5.2/logic/script.py
--rw-r--r--   0 ahmad      (501) staff       (20)      197 2023-05-04 18:00:23.000000 pyneweb-0.5.2/logic/states.py
--rw-r--r--   0 ahmad      (501) staff       (20)     6741 2023-05-11 12:16:23.000000 pyneweb-0.5.2/logic/utilities.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 12:17:21.802699 pyneweb-0.5.2/pyneweb.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-11 12:17:21.000000 pyneweb-0.5.2/pyneweb.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      315 2023-05-11 12:17:21.000000 pyneweb-0.5.2/pyneweb.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-11 12:17:21.000000 pyneweb-0.5.2/pyneweb.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-05-11 12:17:21.000000 pyneweb-0.5.2/pyneweb.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       42 2023-05-11 12:17:21.000000 pyneweb-0.5.2/pyneweb.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-11 12:17:21.000000 pyneweb-0.5.2/pyneweb.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-11 12:17:21.803727 pyneweb-0.5.2/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1107 2023-05-11 12:17:01.000000 pyneweb-0.5.2/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 12:17:21.802902 pyneweb-0.5.2/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-04 18:31:36.000000 pyneweb-0.5.2/tests/test_pass.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 12:52:57.465523 pyneweb-0.5.3/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-05-04 18:35:57.000000 pyneweb-0.5.3/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-11 12:52:57.465309 pyneweb-0.5.3/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4042 2023-05-04 18:48:17.000000 pyneweb-0.5.3/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 12:52:57.463303 pyneweb-0.5.3/logic/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-02 16:20:24.000000 pyneweb-0.5.3/logic/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2348 2023-05-11 12:52:13.000000 pyneweb-0.5.3/logic/cli.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     5504 2023-05-11 11:32:24.000000 pyneweb-0.5.3/logic/script.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      197 2023-05-04 18:00:23.000000 pyneweb-0.5.3/logic/states.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     6741 2023-05-11 12:16:23.000000 pyneweb-0.5.3/logic/utilities.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 12:52:57.464660 pyneweb-0.5.3/pyneweb.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-11 12:52:57.000000 pyneweb-0.5.3/pyneweb.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      315 2023-05-11 12:52:57.000000 pyneweb-0.5.3/pyneweb.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-11 12:52:57.000000 pyneweb-0.5.3/pyneweb.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-05-11 12:52:57.000000 pyneweb-0.5.3/pyneweb.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       42 2023-05-11 12:52:57.000000 pyneweb-0.5.3/pyneweb.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-11 12:52:57.000000 pyneweb-0.5.3/pyneweb.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-11 12:52:57.465594 pyneweb-0.5.3/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1107 2023-05-11 12:52:18.000000 pyneweb-0.5.3/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 12:52:57.464861 pyneweb-0.5.3/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-04 18:31:36.000000 pyneweb-0.5.3/tests/test_pass.py
```

### Comparing `pyneweb-0.5.2/LICENSE` & `pyneweb-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneweb-0.5.2/PKG-INFO` & `pyneweb-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneweb
-Version: 0.5.2
+Version: 0.5.3
 Summary: Web Boilerplate for Pynecone
 Home-page: https://github.com/LineIndent/pyneweb
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneweb-0.5.2/README.md` & `pyneweb-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pyneweb-0.5.2/logic/cli.py` & `pyneweb-0.5.3/logic/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,33 +5,31 @@
 import os
 
 
 def initialize_pynecone_file_script():
     target_dir = None
     target_file = None
 
-    base = os.path.basename(os.path.dirname(os.path.abspath(__file__)))
+    base = os.path.basename(os.getcwd())
 
     for dir in os.listdir():
         if dir == base:
             target_dir = dir
 
     if target_dir:
         for file in os.listdir(target_dir):
             file_path = os.path.join(target_dir, file)
             if os.path.isfile(file_path) and file != "__init__.py":
                 target_file = file
-                print(target_file)
 
     if target_file:
         target_file_path = os.path.join(target_dir, target_file)
         string = set_up_pynecone_file()
         with open(target_file_path, "w") as f:
             f.write(string)
-            pass
 
     else:
         pass
 
 
 @click.command()
 def init():
```

### Comparing `pyneweb-0.5.2/logic/script.py` & `pyneweb-0.5.3/logic/script.py`

 * *Files identical despite different names*

### Comparing `pyneweb-0.5.2/logic/utilities.py` & `pyneweb-0.5.3/logic/utilities.py`

 * *Files identical despite different names*

### Comparing `pyneweb-0.5.2/pyneweb.egg-info/PKG-INFO` & `pyneweb-0.5.3/pyneweb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneweb
-Version: 0.5.2
+Version: 0.5.3
 Summary: Web Boilerplate for Pynecone
 Home-page: https://github.com/LineIndent/pyneweb
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneweb-0.5.2/setup.py` & `pyneweb-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="pyneweb",
-    version="0.5.2",
+    version="0.5.3",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Pynecone",
     long_description="Pyneweb is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Pynecone. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their web applications, without the need to spend time setting up infrastructure or configuration.",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/pyneweb",
     packages=["logic"],
```

