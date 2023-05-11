# Comparing `tmp/pyneweb-0.3.0.tar.gz` & `tmp/pyneweb-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneweb-0.3.0.tar", last modified: Thu May 11 11:18:50 2023, max compression
+gzip compressed data, was "pyneweb-0.4.0.tar", last modified: Thu May 11 11:33:32 2023, max compression
```

## Comparing `pyneweb-0.3.0.tar` & `pyneweb-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:18:50.481125 pyneweb-0.3.0/
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-05-04 18:35:57.000000 pyneweb-0.3.0/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-11 11:18:50.480890 pyneweb-0.3.0/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4042 2023-05-04 18:48:17.000000 pyneweb-0.3.0/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:18:50.478641 pyneweb-0.3.0/logic/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-02 16:20:24.000000 pyneweb-0.3.0/logic/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1559 2023-05-11 11:17:54.000000 pyneweb-0.3.0/logic/cli.py
--rw-r--r--   0 ahmad      (501) staff       (20)     6318 2023-05-11 11:10:58.000000 pyneweb-0.3.0/logic/script.py
--rw-r--r--   0 ahmad      (501) staff       (20)      197 2023-05-04 18:00:23.000000 pyneweb-0.3.0/logic/states.py
--rw-r--r--   0 ahmad      (501) staff       (20)     6651 2023-05-11 11:08:22.000000 pyneweb-0.3.0/logic/utilities.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:18:50.480143 pyneweb-0.3.0/pyneweb.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-11 11:18:50.000000 pyneweb-0.3.0/pyneweb.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      315 2023-05-11 11:18:50.000000 pyneweb-0.3.0/pyneweb.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-11 11:18:50.000000 pyneweb-0.3.0/pyneweb.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-05-11 11:18:50.000000 pyneweb-0.3.0/pyneweb.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       42 2023-05-11 11:18:50.000000 pyneweb-0.3.0/pyneweb.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-11 11:18:50.000000 pyneweb-0.3.0/pyneweb.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-11 11:18:50.481190 pyneweb-0.3.0/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1107 2023-05-11 11:17:59.000000 pyneweb-0.3.0/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:18:50.480334 pyneweb-0.3.0/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-04 18:31:36.000000 pyneweb-0.3.0/tests/test_pass.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:33:32.284693 pyneweb-0.4.0/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-05-04 18:35:57.000000 pyneweb-0.4.0/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-11 11:33:32.284464 pyneweb-0.4.0/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4042 2023-05-04 18:48:17.000000 pyneweb-0.4.0/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:33:32.282147 pyneweb-0.4.0/logic/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-02 16:20:24.000000 pyneweb-0.4.0/logic/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2383 2023-05-11 11:32:48.000000 pyneweb-0.4.0/logic/cli.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     5504 2023-05-11 11:32:24.000000 pyneweb-0.4.0/logic/script.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      197 2023-05-04 18:00:23.000000 pyneweb-0.4.0/logic/states.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     6651 2023-05-11 11:08:22.000000 pyneweb-0.4.0/logic/utilities.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:33:32.283760 pyneweb-0.4.0/pyneweb.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-11 11:33:32.000000 pyneweb-0.4.0/pyneweb.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      315 2023-05-11 11:33:32.000000 pyneweb-0.4.0/pyneweb.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-11 11:33:32.000000 pyneweb-0.4.0/pyneweb.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-05-11 11:33:32.000000 pyneweb-0.4.0/pyneweb.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       42 2023-05-11 11:33:32.000000 pyneweb-0.4.0/pyneweb.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-11 11:33:32.000000 pyneweb-0.4.0/pyneweb.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-11 11:33:32.284774 pyneweb-0.4.0/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1107 2023-05-11 11:33:22.000000 pyneweb-0.4.0/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:33:32.283970 pyneweb-0.4.0/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-04 18:31:36.000000 pyneweb-0.4.0/tests/test_pass.py
```

### Comparing `pyneweb-0.3.0/LICENSE` & `pyneweb-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneweb-0.3.0/PKG-INFO` & `pyneweb-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneweb
-Version: 0.3.0
+Version: 0.4.0
 Summary: Web Boilerplate for Pynecone
 Home-page: https://github.com/LineIndent/pyneweb
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneweb-0.3.0/README.md` & `pyneweb-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyneweb-0.3.0/logic/script.py` & `pyneweb-0.4.0/logic/script.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import yaml
 import os
 from logic.utilities import (
     navigation,
     navigation_list,
     side_navigation_list,
-    set_up_pynecone_file,
 )
 import pynecone as pc
 
 
 def get_yaml_object() -> dict:
     with open("config.yml", "r") as file:
         docs = yaml.safe_load(file)
@@ -137,40 +136,14 @@
             path = os.path.join("routes", file)
             if not os.path.isdir(path) and path != "routes/__init__.py":
                 file = os.path.splitext(file)[0]
                 string = f"from routes.{file} import {file}\n"
                 f.write(string)
 
 
-def initialize_pynecone_file_script():
-    target_dir = None
-    target_file = None
-
-    for dir in os.listdir():
-        if dir != "logic" and os.path.isdir(dir):
-            target_dir = dir
-            break
-
-    if target_dir:
-        for file in os.listdir(target_dir):
-            if file != "__init__.py":
-                target_file = file
-                break
-
-    if target_file:
-        target_file_path = os.path.join(target_dir, target_file)
-        string = set_up_pynecone_file()
-        with open(target_file_path, "w") as f:
-            f.write(string)
-            pass
-
-    else:
-        pass
-
-
 # Main automation script...
 def script(app: pc.Component):
     # 1. Store the YAML data as a python dict object
     try:
         docs: dict = get_yaml_object()
 
     except FileNotFoundError as err:
@@ -200,16 +173,8 @@
     # 5. Update the `__init__.py` file
     try:
         update_init_file()
 
     except Exception as err:
         print(err)
 
-    # 6. init pyencone files
-    try:
-        if not os.path.exists("logic"):
-            initialize_pynecone_file_script()
-
-    except Exception as err:
-        print(err)
-
     app.compile()
```

### Comparing `pyneweb-0.3.0/logic/utilities.py` & `pyneweb-0.4.0/logic/utilities.py`

 * *Files identical despite different names*

### Comparing `pyneweb-0.3.0/pyneweb.egg-info/PKG-INFO` & `pyneweb-0.4.0/pyneweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneweb
-Version: 0.3.0
+Version: 0.4.0
 Summary: Web Boilerplate for Pynecone
 Home-page: https://github.com/LineIndent/pyneweb
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneweb-0.3.0/setup.py` & `pyneweb-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="pyneweb",
-    version="0.3.0",
+    version="0.4.0",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Pynecone",
     long_description="Pyneweb is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Pynecone. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their web applications, without the need to spend time setting up infrastructure or configuration.",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/pyneweb",
     packages=["logic"],
```

