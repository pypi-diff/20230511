# Comparing `tmp/KaggleToDatabricks-0.3.tar.gz` & `tmp/KaggleToDatabricks-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\KaggleToDatabricks-0.3.tar", last modified: Thu May 11 16:51:19 2023, max compression
+gzip compressed data, was "dist\KaggleToDatabricks-0.4.tar", last modified: Thu May 11 17:00:18 2023, max compression
```

## Comparing `KaggleToDatabricks-0.3.tar` & `KaggleToDatabricks-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 16:51:19.067495 KaggleToDatabricks-0.3/
-drwxrwxrwx   0        0        0        0 2023-05-11 16:51:19.061492 KaggleToDatabricks-0.3/KaggleToDatabricks/
--rw-rw-rw-   0        0        0       26 2023-05-11 16:39:05.000000 KaggleToDatabricks-0.3/KaggleToDatabricks/XD.py
--rw-rw-rw-   0        0        0       36 2023-05-11 16:38:34.000000 KaggleToDatabricks-0.3/KaggleToDatabricks/__innit__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:51:19.066494 KaggleToDatabricks-0.3/KaggleToDatabricks.egg-info/
--rw-rw-rw-   0        0        0      898 2023-05-11 16:51:18.000000 KaggleToDatabricks-0.3/KaggleToDatabricks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-05-11 16:51:19.000000 KaggleToDatabricks-0.3/KaggleToDatabricks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 16:51:18.000000 KaggleToDatabricks-0.3/KaggleToDatabricks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-11 16:51:18.000000 KaggleToDatabricks-0.3/KaggleToDatabricks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-11 16:51:18.000000 KaggleToDatabricks-0.3/KaggleToDatabricks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1077 2023-05-11 16:29:58.000000 KaggleToDatabricks-0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      898 2023-05-11 16:51:19.067495 KaggleToDatabricks-0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-11 16:15:46.000000 KaggleToDatabricks-0.3/README.md
--rw-rw-rw-   0        0        0       86 2023-05-11 16:51:19.068494 KaggleToDatabricks-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1842 2023-05-11 16:51:09.000000 KaggleToDatabricks-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 17:00:18.714480 KaggleToDatabricks-0.4/
+drwxrwxrwx   0        0        0        0 2023-05-11 17:00:18.708086 KaggleToDatabricks-0.4/KaggleToDatabricks/
+-rw-rw-rw-   0        0        0       26 2023-05-11 16:59:04.000000 KaggleToDatabricks-0.4/KaggleToDatabricks/XD.py
+-rw-rw-rw-   0        0        0       36 2023-05-11 16:38:34.000000 KaggleToDatabricks-0.4/KaggleToDatabricks/__innit__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 17:00:18.713480 KaggleToDatabricks-0.4/KaggleToDatabricks.egg-info/
+-rw-rw-rw-   0        0        0      898 2023-05-11 17:00:18.000000 KaggleToDatabricks-0.4/KaggleToDatabricks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-05-11 17:00:18.000000 KaggleToDatabricks-0.4/KaggleToDatabricks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 17:00:18.000000 KaggleToDatabricks-0.4/KaggleToDatabricks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-11 17:00:18.000000 KaggleToDatabricks-0.4/KaggleToDatabricks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-11 17:00:18.000000 KaggleToDatabricks-0.4/KaggleToDatabricks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1077 2023-05-11 16:29:58.000000 KaggleToDatabricks-0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      898 2023-05-11 17:00:18.714480 KaggleToDatabricks-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-11 16:15:46.000000 KaggleToDatabricks-0.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-11 17:00:18.714480 KaggleToDatabricks-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1842 2023-05-11 17:00:01.000000 KaggleToDatabricks-0.4/setup.py
```

### Comparing `KaggleToDatabricks-0.3/KaggleToDatabricks.egg-info/PKG-INFO` & `KaggleToDatabricks-0.4/KaggleToDatabricks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KaggleToDatabricks
-Version: 0.3
+Version: 0.4
 Summary: Package created for recruitment task
 Home-page: https://github.com/Teneb/kaggle_to_databricks
 Download-URL: https://github.com/Teneb/kaggle_to_databricks/archive/refs/tags/v0.1.tar.gz
 Author: Artur Woźniak
 Author-email: arturwn39@gmail.com
 License: MIT
 Keywords: pls,hire,me
```

### Comparing `KaggleToDatabricks-0.3/LICENSE.txt` & `KaggleToDatabricks-0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `KaggleToDatabricks-0.3/PKG-INFO` & `KaggleToDatabricks-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KaggleToDatabricks
-Version: 0.3
+Version: 0.4
 Summary: Package created for recruitment task
 Home-page: https://github.com/Teneb/kaggle_to_databricks
 Download-URL: https://github.com/Teneb/kaggle_to_databricks/archive/refs/tags/v0.1.tar.gz
 Author: Artur Woźniak
 Author-email: arturwn39@gmail.com
 License: MIT
 Keywords: pls,hire,me
```

### Comparing `KaggleToDatabricks-0.3/setup.py` & `KaggleToDatabricks-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'KaggleToDatabricks',         # How you named your package folder (MyLib)
   packages = ['KaggleToDatabricks'],   # Chose the same as "name"
-  version = '0.3',      # Start with a small number and increase it with every change you make
+  version = '0.4',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Package created for recruitment task',   # Give a short description about your library
   author = 'Artur Woźniak',                   # Type in your name
   author_email = 'arturwn39@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/Teneb/kaggle_to_databricks',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/Teneb/kaggle_to_databricks/archive/refs/tags/v0.1.tar.gz',    # I explain this later on
   keywords = ['pls', 'hire', 'me'],   # Keywords that define your package best
```

