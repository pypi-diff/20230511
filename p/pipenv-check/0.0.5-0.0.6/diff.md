# Comparing `tmp/pipenv-check-0.0.5.tar.gz` & `tmp/pipenv-check-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipenv-check-0.0.5.tar", last modified: Mon Dec 26 21:35:51 2022, max compression
+gzip compressed data, was "pipenv-check-0.0.6.tar", last modified: Thu May 11 09:01:05 2023, max compression
```

## Comparing `pipenv-check-0.0.5.tar` & `pipenv-check-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ayse       (501) staff       (20)        0 2022-12-26 21:35:51.413804 pipenv-check-0.0.5/
--rw-r--r--   0 ayse       (501) staff       (20)     1061 2022-12-23 10:49:03.000000 pipenv-check-0.0.5/LICENSE
--rw-r--r--   0 ayse       (501) staff       (20)      284 2022-12-26 21:35:51.412944 pipenv-check-0.0.5/PKG-INFO
--rw-r--r--   0 ayse       (501) staff       (20)       15 2022-12-23 10:49:03.000000 pipenv-check-0.0.5/README.md
-drwxr-xr-x   0 ayse       (501) staff       (20)        0 2022-12-26 21:35:51.408856 pipenv-check-0.0.5/pipenv_check/
--rw-r--r--   0 ayse       (501) staff       (20)        0 2022-12-23 10:50:36.000000 pipenv-check-0.0.5/pipenv_check/__init__.py
--rw-r--r--   0 ayse       (501) staff       (20)     5584 2022-12-26 21:32:02.000000 pipenv-check-0.0.5/pipenv_check/check.py
-drwxr-xr-x   0 ayse       (501) staff       (20)        0 2022-12-26 21:35:51.410855 pipenv-check-0.0.5/pipenv_check.egg-info/
--rw-r--r--   0 ayse       (501) staff       (20)      284 2022-12-26 21:35:51.000000 pipenv-check-0.0.5/pipenv_check.egg-info/PKG-INFO
--rw-r--r--   0 ayse       (501) staff       (20)      256 2022-12-26 21:35:51.000000 pipenv-check-0.0.5/pipenv_check.egg-info/SOURCES.txt
--rw-r--r--   0 ayse       (501) staff       (20)        1 2022-12-26 21:35:51.000000 pipenv-check-0.0.5/pipenv_check.egg-info/dependency_links.txt
--rw-r--r--   0 ayse       (501) staff       (20)       57 2022-12-26 21:35:51.000000 pipenv-check-0.0.5/pipenv_check.egg-info/entry_points.txt
--rw-r--r--   0 ayse       (501) staff       (20)       13 2022-12-26 21:35:51.000000 pipenv-check-0.0.5/pipenv_check.egg-info/top_level.txt
--rw-r--r--   0 ayse       (501) staff       (20)       38 2022-12-26 21:35:51.414200 pipenv-check-0.0.5/setup.cfg
--rw-r--r--   0 ayse       (501) staff       (20)      692 2022-12-26 21:34:11.000000 pipenv-check-0.0.5/setup.py
+drwxr-xr-x   0 ayse       (501) staff       (20)        0 2023-05-11 09:01:05.365694 pipenv-check-0.0.6/
+-rw-r--r--   0 ayse       (501) staff       (20)     1061 2023-05-10 13:32:16.000000 pipenv-check-0.0.6/LICENSE
+-rw-r--r--   0 ayse       (501) staff       (20)     1117 2023-05-11 09:01:05.365273 pipenv-check-0.0.6/PKG-INFO
+-rw-r--r--   0 ayse       (501) staff       (20)      847 2023-05-11 08:04:38.000000 pipenv-check-0.0.6/README.md
+drwxr-xr-x   0 ayse       (501) staff       (20)        0 2023-05-11 09:01:05.358666 pipenv-check-0.0.6/pipenv_check/
+-rw-r--r--   0 ayse       (501) staff       (20)        0 2023-05-10 13:32:16.000000 pipenv-check-0.0.6/pipenv_check/__init__.py
+-rw-r--r--   0 ayse       (501) staff       (20)     5697 2023-05-11 08:58:32.000000 pipenv-check-0.0.6/pipenv_check/check.py
+drwxr-xr-x   0 ayse       (501) staff       (20)        0 2023-05-11 09:01:05.364695 pipenv-check-0.0.6/pipenv_check.egg-info/
+-rw-r--r--   0 ayse       (501) staff       (20)     1117 2023-05-11 09:01:05.000000 pipenv-check-0.0.6/pipenv_check.egg-info/PKG-INFO
+-rw-r--r--   0 ayse       (501) staff       (20)      256 2023-05-11 09:01:05.000000 pipenv-check-0.0.6/pipenv_check.egg-info/SOURCES.txt
+-rw-r--r--   0 ayse       (501) staff       (20)        1 2023-05-11 09:01:05.000000 pipenv-check-0.0.6/pipenv_check.egg-info/dependency_links.txt
+-rw-r--r--   0 ayse       (501) staff       (20)       57 2023-05-11 09:01:05.000000 pipenv-check-0.0.6/pipenv_check.egg-info/entry_points.txt
+-rw-r--r--   0 ayse       (501) staff       (20)       13 2023-05-11 09:01:05.000000 pipenv-check-0.0.6/pipenv_check.egg-info/top_level.txt
+-rw-r--r--   0 ayse       (501) staff       (20)       38 2023-05-11 09:01:05.365828 pipenv-check-0.0.6/setup.cfg
+-rw-r--r--   0 ayse       (501) staff       (20)      692 2023-05-10 13:43:50.000000 pipenv-check-0.0.6/setup.py
```

### Comparing `pipenv-check-0.0.5/LICENSE` & `pipenv-check-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pipenv-check-0.0.5/pipenv_check/check.py` & `pipenv-check-0.0.6/pipenv_check/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,33 @@
 import subprocess
 from multiprocessing.pool import ThreadPool
 from urllib.request import urlopen
 import ssl
 import os
 
 
+def color_print(message, text_type, bold=False):
+    if bold:
+        print(text_type + "\033[1m" + message + "\033[0m")  # noqa T201
+    else:
+        print(text_type + message + "\033[0m")  # noqa T201
+
+
+class BColors:
+    HEADER = "\033[95m"
+    OKBLUE = "\033[94m"
+    OKGREEN = "\033[92m"
+    WARNING = "\033[93m"
+    FAIL = "\033[91m"
+    # - ENDC = "\033[0m"
+
+
 def main():
     ssl._create_default_https_context = ssl._create_unverified_context
 
-    def color_print(message, text_type, bold=False):
-        if bold:
-            print(text_type + "\033[1m" + message + "\033[0m")  # noqa T201
-        else:
-            print(text_type + message + "\033[0m")  # noqa T201
-
-    class BColors:
-        HEADER = "\033[95m"
-        OKBLUE = "\033[94m"
-        OKGREEN = "\033[92m"
-        WARNING = "\033[93m"
-        FAIL = "\033[91m"
-        # - ENDC = "\033[0m"
-
     color_print(
         'Checking for outdated packages in your "Pipfile"...', BColors.OKBLUE, True
     )
 
     pipfile = os.path.join(os.getcwd(), "Pipfile")
     pipfile_packages = []
 
@@ -46,15 +48,20 @@
     pipfile_packages = [x.strip(' ') for x in pipfile_packages]
     # get package names max len
     package_name_len = (
             max([len(package) for package in pipfile_packages]) + 1
     )
 
     # get the list of installed packages
-    installed_packages = json.loads(subprocess.check_output(["pip", "list", "--format=json"]).lower())
+    try:
+        installed_packages = json.loads(subprocess.check_output(["pip", "list", "--format=json"]).decode('utf-8').lower())
+    except Exception as e:
+        print("Error occurred while fetching installed packages:", e)
+        exit(1)
+
     # installed_packages_in_pipfile with current version
     installed_packages_in_pipfile = {
         package["name"]: {"current": package["version"]}
         for package in installed_packages
         if package["name"] in pipfile_packages
     }
 
@@ -78,14 +85,15 @@
         r = json.loads(data.decode("utf-8"))
         version = r["info"]["version"]
         return version
 
     pool = ThreadPool()
     latest_versions = pool.map(get_latest_version, installed_packages_in_pipfile)
     pool.close()
+    pool.join()
 
     for package_name, latest_version in zip(installed_packages_in_pipfile.keys(), latest_versions):
         installed_packages_in_pipfile[package_name]["latest"] = latest_version
 
     # group packages by major, minor and bug fix update
     packages_by_update = {
         "not installed": [],
```

### Comparing `pipenv-check-0.0.5/setup.py` & `pipenv-check-0.0.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages, setup
 
 long_description = u"\n\n".join((open("README.md").read(),))
 
 setup(
     name="pipenv-check",
-    version="0.0.5",
+    version="0.0.6",
     description="View installed pip packages and their update status.",
     long_description=long_description,
     author="3bfab",
     author_email="info@3bfab.com",
     license="MIT",
     url="https://github.com/3bfab/pipenv-check",
     classifiers=[],
```

