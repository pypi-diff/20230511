# Comparing `tmp/KaggleToDatabricks-0.2.tar.gz` & `tmp/KaggleToDatabricks-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\KaggleToDatabricks-0.2.tar", last modified: Thu May 11 16:49:21 2023, max compression
+gzip compressed data, was "dist\KaggleToDatabricks-0.3.tar", last modified: Thu May 11 16:51:19 2023, max compression
```

## Comparing `KaggleToDatabricks-0.2.tar` & `KaggleToDatabricks-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 16:49:21.398071 KaggleToDatabricks-0.2/
-drwxrwxrwx   0        0        0        0 2023-05-11 16:49:21.392071 KaggleToDatabricks-0.2/KaggleToDatabricks/
--rw-rw-rw-   0        0        0       26 2023-05-11 16:39:05.000000 KaggleToDatabricks-0.2/KaggleToDatabricks/XD.py
--rw-rw-rw-   0        0        0       36 2023-05-11 16:38:34.000000 KaggleToDatabricks-0.2/KaggleToDatabricks/__innit__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:49:21.397070 KaggleToDatabricks-0.2/KaggleToDatabricks.egg-info/
--rw-rw-rw-   0        0        0      898 2023-05-11 16:49:21.000000 KaggleToDatabricks-0.2/KaggleToDatabricks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-05-11 16:49:21.000000 KaggleToDatabricks-0.2/KaggleToDatabricks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 16:49:21.000000 KaggleToDatabricks-0.2/KaggleToDatabricks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-11 16:49:21.000000 KaggleToDatabricks-0.2/KaggleToDatabricks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-11 16:49:21.000000 KaggleToDatabricks-0.2/KaggleToDatabricks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1077 2023-05-11 16:29:58.000000 KaggleToDatabricks-0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      898 2023-05-11 16:49:21.399071 KaggleToDatabricks-0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-11 16:15:46.000000 KaggleToDatabricks-0.2/README.md
--rw-rw-rw-   0        0        0       86 2023-05-11 16:49:21.399071 KaggleToDatabricks-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1870 2023-05-11 16:49:18.000000 KaggleToDatabricks-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:51:19.067495 KaggleToDatabricks-0.3/
+drwxrwxrwx   0        0        0        0 2023-05-11 16:51:19.061492 KaggleToDatabricks-0.3/KaggleToDatabricks/
+-rw-rw-rw-   0        0        0       26 2023-05-11 16:39:05.000000 KaggleToDatabricks-0.3/KaggleToDatabricks/XD.py
+-rw-rw-rw-   0        0        0       36 2023-05-11 16:38:34.000000 KaggleToDatabricks-0.3/KaggleToDatabricks/__innit__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:51:19.066494 KaggleToDatabricks-0.3/KaggleToDatabricks.egg-info/
+-rw-rw-rw-   0        0        0      898 2023-05-11 16:51:18.000000 KaggleToDatabricks-0.3/KaggleToDatabricks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-05-11 16:51:19.000000 KaggleToDatabricks-0.3/KaggleToDatabricks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 16:51:18.000000 KaggleToDatabricks-0.3/KaggleToDatabricks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-11 16:51:18.000000 KaggleToDatabricks-0.3/KaggleToDatabricks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-11 16:51:18.000000 KaggleToDatabricks-0.3/KaggleToDatabricks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1077 2023-05-11 16:29:58.000000 KaggleToDatabricks-0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      898 2023-05-11 16:51:19.067495 KaggleToDatabricks-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-11 16:15:46.000000 KaggleToDatabricks-0.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-11 16:51:19.068494 KaggleToDatabricks-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1842 2023-05-11 16:51:09.000000 KaggleToDatabricks-0.3/setup.py
```

### Comparing `KaggleToDatabricks-0.2/KaggleToDatabricks.egg-info/PKG-INFO` & `KaggleToDatabricks-0.3/KaggleToDatabricks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KaggleToDatabricks
-Version: 0.2
+Version: 0.3
 Summary: Package created for recruitment task
 Home-page: https://github.com/Teneb/kaggle_to_databricks
 Download-URL: https://github.com/Teneb/kaggle_to_databricks/archive/refs/tags/v0.1.tar.gz
 Author: Artur Woźniak
 Author-email: arturwn39@gmail.com
 License: MIT
 Keywords: pls,hire,me
```

### Comparing `KaggleToDatabricks-0.2/LICENSE.txt` & `KaggleToDatabricks-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `KaggleToDatabricks-0.2/PKG-INFO` & `KaggleToDatabricks-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KaggleToDatabricks
-Version: 0.2
+Version: 0.3
 Summary: Package created for recruitment task
 Home-page: https://github.com/Teneb/kaggle_to_databricks
 Download-URL: https://github.com/Teneb/kaggle_to_databricks/archive/refs/tags/v0.1.tar.gz
 Author: Artur Woźniak
 Author-email: arturwn39@gmail.com
 License: MIT
 Keywords: pls,hire,me
```

### Comparing `KaggleToDatabricks-0.2/setup.py` & `KaggleToDatabricks-0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from distutils.core import setup
 setup(
   name = 'KaggleToDatabricks',         # How you named your package folder (MyLib)
   packages = ['KaggleToDatabricks'],   # Chose the same as "name"
-  version = '0.2',      # Start with a small number and increase it with every change you make
+  version = '0.3',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Package created for recruitment task',   # Give a short description about your library
   author = 'Artur Woźniak',                   # Type in your name
   author_email = 'arturwn39@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/Teneb/kaggle_to_databricks',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/Teneb/kaggle_to_databricks/archive/refs/tags/v0.1.tar.gz',    # I explain this later on
   keywords = ['pls', 'hire', 'me'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
-          'kaggle.api.kaggle_api_extended',
+          'kaggle',
           'pandas',
-          'pyspark.sql'          
+          'pyspark'          
       ],
   classifiers=[
     'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
```

