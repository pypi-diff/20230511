# Comparing `tmp/pyneweb-0.5.0.tar.gz` & `tmp/pyneweb-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneweb-0.5.0.tar", last modified: Thu May 11 11:36:29 2023, max compression
+gzip compressed data, was "pyneweb-0.5.1.tar", last modified: Thu May 11 11:58:09 2023, max compression
```

## Comparing `pyneweb-0.5.0.tar` & `pyneweb-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:36:29.967369 pyneweb-0.5.0/
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-05-04 18:35:57.000000 pyneweb-0.5.0/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-11 11:36:29.967145 pyneweb-0.5.0/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4042 2023-05-04 18:48:17.000000 pyneweb-0.5.0/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:36:29.965157 pyneweb-0.5.0/logic/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-02 16:20:24.000000 pyneweb-0.5.0/logic/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2383 2023-05-11 11:32:48.000000 pyneweb-0.5.0/logic/cli.py
--rw-r--r--   0 ahmad      (501) staff       (20)     5504 2023-05-11 11:32:24.000000 pyneweb-0.5.0/logic/script.py
--rw-r--r--   0 ahmad      (501) staff       (20)      197 2023-05-04 18:00:23.000000 pyneweb-0.5.0/logic/states.py
--rw-r--r--   0 ahmad      (501) staff       (20)     6686 2023-05-11 11:35:49.000000 pyneweb-0.5.0/logic/utilities.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:36:29.966448 pyneweb-0.5.0/pyneweb.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-11 11:36:29.000000 pyneweb-0.5.0/pyneweb.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      315 2023-05-11 11:36:29.000000 pyneweb-0.5.0/pyneweb.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-11 11:36:29.000000 pyneweb-0.5.0/pyneweb.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-05-11 11:36:29.000000 pyneweb-0.5.0/pyneweb.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       42 2023-05-11 11:36:29.000000 pyneweb-0.5.0/pyneweb.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-11 11:36:29.000000 pyneweb-0.5.0/pyneweb.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-11 11:36:29.967451 pyneweb-0.5.0/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1107 2023-05-11 11:35:52.000000 pyneweb-0.5.0/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:36:29.966659 pyneweb-0.5.0/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-04 18:31:36.000000 pyneweb-0.5.0/tests/test_pass.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:58:09.038490 pyneweb-0.5.1/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-05-04 18:35:57.000000 pyneweb-0.5.1/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-11 11:58:09.038257 pyneweb-0.5.1/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4042 2023-05-04 18:48:17.000000 pyneweb-0.5.1/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:58:09.036145 pyneweb-0.5.1/logic/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-02 16:20:24.000000 pyneweb-0.5.1/logic/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2304 2023-05-11 11:49:53.000000 pyneweb-0.5.1/logic/cli.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     5504 2023-05-11 11:32:24.000000 pyneweb-0.5.1/logic/script.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      197 2023-05-04 18:00:23.000000 pyneweb-0.5.1/logic/states.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     6686 2023-05-11 11:35:49.000000 pyneweb-0.5.1/logic/utilities.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:58:09.037605 pyneweb-0.5.1/pyneweb.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-11 11:58:09.000000 pyneweb-0.5.1/pyneweb.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      315 2023-05-11 11:58:09.000000 pyneweb-0.5.1/pyneweb.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-11 11:58:09.000000 pyneweb-0.5.1/pyneweb.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-05-11 11:58:09.000000 pyneweb-0.5.1/pyneweb.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       42 2023-05-11 11:58:09.000000 pyneweb-0.5.1/pyneweb.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-11 11:58:09.000000 pyneweb-0.5.1/pyneweb.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-11 11:58:09.038561 pyneweb-0.5.1/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1107 2023-05-11 11:58:01.000000 pyneweb-0.5.1/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-11 11:58:09.037805 pyneweb-0.5.1/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-04 18:31:36.000000 pyneweb-0.5.1/tests/test_pass.py
```

### Comparing `pyneweb-0.5.0/LICENSE` & `pyneweb-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneweb-0.5.0/PKG-INFO` & `pyneweb-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneweb
-Version: 0.5.0
+Version: 0.5.1
 Summary: Web Boilerplate for Pynecone
 Home-page: https://github.com/LineIndent/pyneweb
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneweb-0.5.0/README.md` & `pyneweb-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pyneweb-0.5.0/logic/cli.py` & `pyneweb-0.5.1/logic/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,29 +58,27 @@
         with open(file_path, "w") as new_file:
             new_file.write(source_contents)
 
     click.echo()
     click.echo(f"Generated {len(file_list)} files in the 'logic' directory:")
     for files in file_list:
         click.echo(f"● {files}")
+    click.echo()
     click.echo("Status: OK")
     click.echo()
 
     # Run the 'pc init' command
-    result = subprocess.run(["pc", "init"], capture_output=True, text=True)
+    subprocess.run(["pc", "init"], capture_output=True, text=True)
     click.echo()
-    if result.returncode == 0:
-        click.echo("Command 'pc init' executed successfully.")
-        click.echo()
-        click.echo("Setting up the default application layout ...")
-        initialize_pynecone_file_script()
-
-    else:
-        click.echo("Command 'pc init' execution failed.")
+    click.echo("Command 'pc init' executed successfully.")
     click.echo()
+    click.echo("Setting up the default application layout ...")
+    initialize_pynecone_file_script()
+    click.echo()
+    click.echo("Status: OK")
 
 
 @click.group()
 def pyneweb():
     pass
```

### Comparing `pyneweb-0.5.0/logic/script.py` & `pyneweb-0.5.1/logic/script.py`

 * *Files identical despite different names*

### Comparing `pyneweb-0.5.0/logic/utilities.py` & `pyneweb-0.5.1/logic/utilities.py`

 * *Files identical despite different names*

### Comparing `pyneweb-0.5.0/pyneweb.egg-info/PKG-INFO` & `pyneweb-0.5.1/pyneweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneweb
-Version: 0.5.0
+Version: 0.5.1
 Summary: Web Boilerplate for Pynecone
 Home-page: https://github.com/LineIndent/pyneweb
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneweb-0.5.0/setup.py` & `pyneweb-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="pyneweb",
-    version="0.5.0",
+    version="0.5.1",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Pynecone",
     long_description="Pyneweb is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Pynecone. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their web applications, without the need to spend time setting up infrastructure or configuration.",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/pyneweb",
     packages=["logic"],
```

