# Comparing `tmp/pyneweb-0.2.0.tar.gz` & `tmp/pyneweb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneweb-0.2.0.tar", last modified: Thu May  4 19:30:20 2023, max compression
+gzip compressed data, was "pyneweb-0.3.0.tar", last modified: Thu May 11 11:18:50 2023, max compression
```

## Comparing `pyneweb-0.2.0.tar` & `pyneweb-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-04 19:30:20.437101 pyneweb-0.2.0/
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-05-04 18:35:57.000000 pyneweb-0.2.0/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-04 19:30:20.436877 pyneweb-0.2.0/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4042 2023-05-04 18:48:17.000000 pyneweb-0.2.0/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-04 19:30:20.434897 pyneweb-0.2.0/logic/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-02 16:20:24.000000 pyneweb-0.2.0/logic/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1253 2023-05-04 18:56:48.000000 pyneweb-0.2.0/logic/cli.py
--rw-r--r--   0 ahmad      (501) staff       (20)     5504 2023-05-04 17:09:49.000000 pyneweb-0.2.0/logic/script.py
--rw-r--r--   0 ahmad      (501) staff       (20)      197 2023-05-04 18:00:23.000000 pyneweb-0.2.0/logic/states.py
--rw-r--r--   0 ahmad      (501) staff       (20)     6206 2023-05-04 18:29:03.000000 pyneweb-0.2.0/logic/utilities.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-04 19:30:20.436277 pyneweb-0.2.0/pyneweb.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-04 19:30:20.000000 pyneweb-0.2.0/pyneweb.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      315 2023-05-04 19:30:20.000000 pyneweb-0.2.0/pyneweb.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-04 19:30:20.000000 pyneweb-0.2.0/pyneweb.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-05-04 19:30:20.000000 pyneweb-0.2.0/pyneweb.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       42 2023-05-04 19:30:20.000000 pyneweb-0.2.0/pyneweb.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-04 19:30:20.000000 pyneweb-0.2.0/pyneweb.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-04 19:30:20.437166 pyneweb-0.2.0/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1107 2023-05-04 19:29:48.000000 pyneweb-0.2.0/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-04 19:30:20.436471 pyneweb-0.2.0/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-04 18:31:36.000000 pyneweb-0.2.0/tests/test_pass.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:18:50.481125 pyneweb-0.3.0/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-05-04 18:35:57.000000 pyneweb-0.3.0/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-11 11:18:50.480890 pyneweb-0.3.0/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4042 2023-05-04 18:48:17.000000 pyneweb-0.3.0/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:18:50.478641 pyneweb-0.3.0/logic/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-02 16:20:24.000000 pyneweb-0.3.0/logic/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1559 2023-05-11 11:17:54.000000 pyneweb-0.3.0/logic/cli.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     6318 2023-05-11 11:10:58.000000 pyneweb-0.3.0/logic/script.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      197 2023-05-04 18:00:23.000000 pyneweb-0.3.0/logic/states.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     6651 2023-05-11 11:08:22.000000 pyneweb-0.3.0/logic/utilities.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:18:50.480143 pyneweb-0.3.0/pyneweb.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-11 11:18:50.000000 pyneweb-0.3.0/pyneweb.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      315 2023-05-11 11:18:50.000000 pyneweb-0.3.0/pyneweb.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-11 11:18:50.000000 pyneweb-0.3.0/pyneweb.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-05-11 11:18:50.000000 pyneweb-0.3.0/pyneweb.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       42 2023-05-11 11:18:50.000000 pyneweb-0.3.0/pyneweb.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-11 11:18:50.000000 pyneweb-0.3.0/pyneweb.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-11 11:18:50.481190 pyneweb-0.3.0/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1107 2023-05-11 11:17:59.000000 pyneweb-0.3.0/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:18:50.480334 pyneweb-0.3.0/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-04 18:31:36.000000 pyneweb-0.3.0/tests/test_pass.py
```

### Comparing `pyneweb-0.2.0/LICENSE` & `pyneweb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneweb-0.2.0/PKG-INFO` & `pyneweb-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneweb
-Version: 0.2.0
+Version: 0.3.0
 Summary: Web Boilerplate for Pynecone
 Home-page: https://github.com/LineIndent/pyneweb
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneweb-0.2.0/README.md` & `pyneweb-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyneweb-0.2.0/logic/cli.py` & `pyneweb-0.3.0/logic/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import click
+import subprocess
 from logic.utilities import set_up_yaml_file
 from pathlib import Path
 
 
 @click.command()
 def init():
     # First, create the flet_config.yml file
@@ -32,14 +33,22 @@
 
     click.echo()
     click.echo(f"Generated {len(file_list)} files in the 'logic' directory:")
     for files in file_list:
         click.echo(f"● {files}")
     click.echo()
 
+    # Run the 'pc init' command
+    result = subprocess.run(["pc", "init"], capture_output=True, text=True)
+    if result.returncode == 0:
+        click.echo("Command 'pc init' executed successfully.")
+    else:
+        click.echo("Command 'pc init' execution failed.")
+    click.echo()
+
 
 @click.group()
 def pyneweb():
     pass
 
 
 pyneweb.add_command(init)
```

### Comparing `pyneweb-0.2.0/logic/script.py` & `pyneweb-0.3.0/logic/script.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import yaml
 import os
 from logic.utilities import (
     navigation,
     navigation_list,
     side_navigation_list,
+    set_up_pynecone_file,
 )
 import pynecone as pc
 
 
 def get_yaml_object() -> dict:
     with open("config.yml", "r") as file:
         docs = yaml.safe_load(file)
@@ -136,14 +137,40 @@
             path = os.path.join("routes", file)
             if not os.path.isdir(path) and path != "routes/__init__.py":
                 file = os.path.splitext(file)[0]
                 string = f"from routes.{file} import {file}\n"
                 f.write(string)
 
 
+def initialize_pynecone_file_script():
+    target_dir = None
+    target_file = None
+
+    for dir in os.listdir():
+        if dir != "logic" and os.path.isdir(dir):
+            target_dir = dir
+            break
+
+    if target_dir:
+        for file in os.listdir(target_dir):
+            if file != "__init__.py":
+                target_file = file
+                break
+
+    if target_file:
+        target_file_path = os.path.join(target_dir, target_file)
+        string = set_up_pynecone_file()
+        with open(target_file_path, "w") as f:
+            f.write(string)
+            pass
+
+    else:
+        pass
+
+
 # Main automation script...
 def script(app: pc.Component):
     # 1. Store the YAML data as a python dict object
     try:
         docs: dict = get_yaml_object()
 
     except FileNotFoundError as err:
@@ -173,8 +200,16 @@
     # 5. Update the `__init__.py` file
     try:
         update_init_file()
 
     except Exception as err:
         print(err)
 
+    # 6. init pyencone files
+    try:
+        if not os.path.exists("logic"):
+            initialize_pynecone_file_script()
+
+    except Exception as err:
+        print(err)
+
     app.compile()
```

### Comparing `pyneweb-0.2.0/logic/utilities.py` & `pyneweb-0.3.0/logic/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Utiltities: Provides chunks of code as supplement to the main scrip inside `script.py`.
+Utilities: Provides chunks of code as supplement to the main scrip inside `script.py`.
 """
 
 import os
 
 
 def navigation(route, title, fn_name):
     string = f"""import pynecone as pc
@@ -206,7 +206,30 @@
 nav:
   - Home: "index.py"
   - About: "about.py"
   - Contact: "contact.py"
 
 """
     return string
+
+
+############################################
+######### Update pynecone init file ########
+############################################
+
+
+def set_up_pynecone_file():
+    string = """# Pynecone && Pyneweb modules
+import pynecone as pc
+from logic.script import script
+from logic.states import State
+
+# Import pages from routes dir
+from routes import *
+
+# Setup for script
+app = pc.App(state=State)
+app.compile()
+script(app)
+"""
+
+    return string
```

### Comparing `pyneweb-0.2.0/pyneweb.egg-info/PKG-INFO` & `pyneweb-0.3.0/pyneweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneweb
-Version: 0.2.0
+Version: 0.3.0
 Summary: Web Boilerplate for Pynecone
 Home-page: https://github.com/LineIndent/pyneweb
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneweb-0.2.0/setup.py` & `pyneweb-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="pyneweb",
-    version="0.2.0",
+    version="0.3.0",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Pynecone",
     long_description="Pyneweb is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Pynecone. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their web applications, without the need to spend time setting up infrastructure or configuration.",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/pyneweb",
     packages=["logic"],
```

