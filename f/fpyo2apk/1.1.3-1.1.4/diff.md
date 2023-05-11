# Comparing `tmp/fpyo2apk-1.1.3.tar.gz` & `tmp/fpyo2apk-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpyo2apk-1.1.3.tar", last modified: Mon May  8 15:02:04 2023, max compression
+gzip compressed data, was "fpyo2apk-1.1.4.tar", last modified: Thu May 11 17:38:53 2023, max compression
```

## Comparing `fpyo2apk-1.1.3.tar` & `fpyo2apk-1.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:02:04.199349 fpyo2apk-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 15:01:47.000000 fpyo2apk-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 15:01:47.000000 fpyo2apk-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-08 15:02:04.199349 fpyo2apk-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:01:47.000000 fpyo2apk-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:02:04.195349 fpyo2apk-1.1.3/fpyo2apk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:02:04.195349 fpyo2apk-1.1.3/fpyo2apk/Tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:01:47.000000 fpyo2apk-1.1.3/fpyo2apk/Tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-08 15:01:47.000000 fpyo2apk-1.1.3/fpyo2apk/Tools/check_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-08 15:01:47.000000 fpyo2apk-1.1.3/fpyo2apk/Tools/check_venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-08 15:01:47.000000 fpyo2apk-1.1.3/fpyo2apk/Tools/unzip_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:01:47.000000 fpyo2apk-1.1.3/fpyo2apk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:02:04.195349 fpyo2apk-1.1.3/fpyo2apk/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:01:47.000000 fpyo2apk-1.1.3/fpyo2apk/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   495603 2023-05-08 15:01:47.000000 fpyo2apk-1.1.3/fpyo2apk/assets/fpyo2apkdist.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:02:04.199349 fpyo2apk-1.1.3/fpyo2apk/beeware_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:01:47.000000 fpyo2apk-1.1.3/fpyo2apk/beeware_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-08 15:01:47.000000 fpyo2apk-1.1.3/fpyo2apk/beeware_tools/edit_beeware_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-08 15:01:47.000000 fpyo2apk-1.1.3/fpyo2apk/beeware_tools/the_app_py.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-08 15:01:47.000000 fpyo2apk-1.1.3/fpyo2apk/beeware_tools/the_localhost_py.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-08 15:01:47.000000 fpyo2apk-1.1.3/fpyo2apk/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:02:04.195349 fpyo2apk-1.1.3/fpyo2apk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-08 15:02:04.000000 fpyo2apk-1.1.3/fpyo2apk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-08 15:02:04.000000 fpyo2apk-1.1.3/fpyo2apk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:02:04.000000 fpyo2apk-1.1.3/fpyo2apk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 15:02:04.000000 fpyo2apk-1.1.3/fpyo2apk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 15:02:04.000000 fpyo2apk-1.1.3/fpyo2apk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 15:01:47.000000 fpyo2apk-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:02:04.199349 fpyo2apk-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-08 15:01:47.000000 fpyo2apk-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:38:53.793618 fpyo2apk-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-11 17:38:41.000000 fpyo2apk-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-11 17:38:41.000000 fpyo2apk-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-11 17:38:53.793618 fpyo2apk-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-11 17:38:41.000000 fpyo2apk-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:38:53.789617 fpyo2apk-1.1.4/fpyo2apk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:38:53.789617 fpyo2apk-1.1.4/fpyo2apk/Tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 17:38:41.000000 fpyo2apk-1.1.4/fpyo2apk/Tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-11 17:38:41.000000 fpyo2apk-1.1.4/fpyo2apk/Tools/check_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-11 17:38:41.000000 fpyo2apk-1.1.4/fpyo2apk/Tools/check_venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-11 17:38:41.000000 fpyo2apk-1.1.4/fpyo2apk/Tools/unzip_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 17:38:41.000000 fpyo2apk-1.1.4/fpyo2apk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:38:53.789617 fpyo2apk-1.1.4/fpyo2apk/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 17:38:41.000000 fpyo2apk-1.1.4/fpyo2apk/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   495603 2023-05-11 17:38:41.000000 fpyo2apk-1.1.4/fpyo2apk/assets/fpyo2apkdist.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:38:53.793618 fpyo2apk-1.1.4/fpyo2apk/beeware_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 17:38:41.000000 fpyo2apk-1.1.4/fpyo2apk/beeware_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-11 17:38:41.000000 fpyo2apk-1.1.4/fpyo2apk/beeware_tools/edit_beeware_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-11 17:38:41.000000 fpyo2apk-1.1.4/fpyo2apk/beeware_tools/the_app_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-11 17:38:41.000000 fpyo2apk-1.1.4/fpyo2apk/beeware_tools/the_localhost_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-11 17:38:41.000000 fpyo2apk-1.1.4/fpyo2apk/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:38:53.789617 fpyo2apk-1.1.4/fpyo2apk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-11 17:38:53.000000 fpyo2apk-1.1.4/fpyo2apk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-11 17:38:53.000000 fpyo2apk-1.1.4/fpyo2apk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 17:38:53.000000 fpyo2apk-1.1.4/fpyo2apk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 17:38:53.000000 fpyo2apk-1.1.4/fpyo2apk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 17:38:53.000000 fpyo2apk-1.1.4/fpyo2apk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-11 17:38:41.000000 fpyo2apk-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 17:38:53.793618 fpyo2apk-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-11 17:38:41.000000 fpyo2apk-1.1.4/setup.py
```

### Comparing `fpyo2apk-1.1.3/LICENSE` & `fpyo2apk-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.1.3/fpyo2apk/Tools/unzip_assets.py` & `fpyo2apk-1.1.4/fpyo2apk/Tools/unzip_assets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import os
 import zipfile
 import shutil
 
 def Unzip_asset ():
     asset_path = str(__file__).replace("Tools/unzip_assets.py", "assets/fpyo2apkdist.zip")
+
+    if r"Tools\unzip_assets.py" in str(asset_path):
+        asset_path = str(asset_path).replace(r"Tools\unzip_assets.py", r"assets\fpyo2apkdist.zip")
+    
     if not os.path.isfile(asset_path):
         raise FileNotFoundError("Cannot found the assets.")
     
     if os.path.isdir("fpyo2apkdist"):
         shutil.rmtree("fpyo2apkdist")
 
     with zipfile.ZipFile(asset_path, "r") as zip_ref:
```

### Comparing `fpyo2apk-1.1.3/fpyo2apk/assets/fpyo2apkdist.zip` & `fpyo2apk-1.1.4/fpyo2apk/assets/fpyo2apkdist.zip`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.1.3/fpyo2apk/beeware_tools/edit_beeware_project.py` & `fpyo2apk-1.1.4/fpyo2apk/beeware_tools/edit_beeware_project.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,28 +35,25 @@
     open("dist/index.html", "w+", encoding="utf-8").write(the_index_file)
 
     print("copy the dist..")
     if os.path.isdir(f"{project_name}/src/fpyo2apk/assets/dist"):
         shutil.rmtree(f"{project_name}/src/fpyo2apk/assets/dist")
     shutil.copytree("dist", f"{project_name}/src/fpyo2apk/assets/dist")
 
-    print("start edit the 'app.py' file")
+    print("start edit the 'app.py' file..")
     open(f"{project_name}/src/fpyo2apk/app.py", "w+", encoding="utf-8").write(The_app_py_script)
 
-    print("start creating/editing the 'localhost.py' file")
+    print("start creating/editing the 'localhost.py' file..")
     open(f"{project_name}/src/fpyo2apk/localhost.py", "w+", encoding="utf-8").write(The_localhost_py_script)
 
-    print("Your app is being built and then can open it on the android simulator..\nThis Usually take two minutes to finish, please wait..")
-    process = subprocess.Popen(["cd fpyo2apkdist\nbriefcase create Android\nbriefcase build Android\n"], stdin=subprocess.PIPE, stdout=subprocess.PIPE, shell=True)
-    output, error = process.communicate()
-    if error != None:
-        sys.exit(f"\nExit with Error: {error}")
-    
     print("""
 
-All work done!
-Your app is in the `fpyo2apkdist/build/fpyo2apkdist/android/`!
-To run a simulator, use:
+Your project has been created successfully!
+There are some problems with running brifcase commands automatically,
+so you will have to run them manually.
+
 $ cd fpyo2apkdist
+$ briefcase create Android
+$ briefcase build Android
 $ briefcase run Android
 
     """)
```

### Comparing `fpyo2apk-1.1.3/fpyo2apk/beeware_tools/the_app_py.py` & `fpyo2apk-1.1.4/fpyo2apk/beeware_tools/the_app_py.py`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.1.3/fpyo2apk/beeware_tools/the_localhost_py.py` & `fpyo2apk-1.1.4/fpyo2apk/beeware_tools/the_localhost_py.py`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.1.3/fpyo2apk/build.py` & `fpyo2apk-1.1.4/fpyo2apk/build.py`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.1.3/fpyo2apk.egg-info/SOURCES.txt` & `fpyo2apk-1.1.4/fpyo2apk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.1.3/setup.py` & `fpyo2apk-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fpyo2apk',
-    version='1.1.3',
+    version='1.1.4',
     author='SKbarbon',
     description='A package tool that allow you to built a python Android apps with flet-pyodide dist.',
     long_description="https://github.com/SKbarbon/fpyo2apk",
     url='https://github.com/SKbarbon/fpyo2apk',
     install_requires=["briefcase==0.3.14"],
     include_package_data=True,
     packages=find_packages(),
```

