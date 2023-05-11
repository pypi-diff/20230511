# Comparing `tmp/KaggleToDatabricks-0.1.tar.gz` & `tmp/KaggleToDatabricks-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\KaggleToDatabricks-0.1.tar", last modified: Thu May 11 16:41:11 2023, max compression
+gzip compressed data, was "dist\KaggleToDatabricks-0.2.tar", last modified: Thu May 11 16:49:21 2023, max compression
```

## Comparing `KaggleToDatabricks-0.1.tar` & `KaggleToDatabricks-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 16:41:11.047366 KaggleToDatabricks-0.1/
-drwxrwxrwx   0        0        0        0 2023-05-11 16:41:11.041364 KaggleToDatabricks-0.1/KaggleToDatabricks/
--rw-rw-rw-   0        0        0       26 2023-05-11 16:39:05.000000 KaggleToDatabricks-0.1/KaggleToDatabricks/XD.py
--rw-rw-rw-   0        0        0       36 2023-05-11 16:38:34.000000 KaggleToDatabricks-0.1/KaggleToDatabricks/__innit__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:41:11.046365 KaggleToDatabricks-0.1/KaggleToDatabricks.egg-info/
--rw-rw-rw-   0        0        0      930 2023-05-11 16:41:10.000000 KaggleToDatabricks-0.1/KaggleToDatabricks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-05-11 16:41:10.000000 KaggleToDatabricks-0.1/KaggleToDatabricks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 16:41:10.000000 KaggleToDatabricks-0.1/KaggleToDatabricks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-05-11 16:41:10.000000 KaggleToDatabricks-0.1/KaggleToDatabricks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-11 16:41:10.000000 KaggleToDatabricks-0.1/KaggleToDatabricks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1077 2023-05-11 16:29:58.000000 KaggleToDatabricks-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      930 2023-05-11 16:41:11.048365 KaggleToDatabricks-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-11 16:15:46.000000 KaggleToDatabricks-0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-05-11 16:41:11.048365 KaggleToDatabricks-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1930 2023-05-11 16:41:06.000000 KaggleToDatabricks-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:49:21.398071 KaggleToDatabricks-0.2/
+drwxrwxrwx   0        0        0        0 2023-05-11 16:49:21.392071 KaggleToDatabricks-0.2/KaggleToDatabricks/
+-rw-rw-rw-   0        0        0       26 2023-05-11 16:39:05.000000 KaggleToDatabricks-0.2/KaggleToDatabricks/XD.py
+-rw-rw-rw-   0        0        0       36 2023-05-11 16:38:34.000000 KaggleToDatabricks-0.2/KaggleToDatabricks/__innit__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:49:21.397070 KaggleToDatabricks-0.2/KaggleToDatabricks.egg-info/
+-rw-rw-rw-   0        0        0      898 2023-05-11 16:49:21.000000 KaggleToDatabricks-0.2/KaggleToDatabricks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-05-11 16:49:21.000000 KaggleToDatabricks-0.2/KaggleToDatabricks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 16:49:21.000000 KaggleToDatabricks-0.2/KaggleToDatabricks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-11 16:49:21.000000 KaggleToDatabricks-0.2/KaggleToDatabricks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-11 16:49:21.000000 KaggleToDatabricks-0.2/KaggleToDatabricks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1077 2023-05-11 16:29:58.000000 KaggleToDatabricks-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      898 2023-05-11 16:49:21.399071 KaggleToDatabricks-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-11 16:15:46.000000 KaggleToDatabricks-0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-11 16:49:21.399071 KaggleToDatabricks-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1870 2023-05-11 16:49:18.000000 KaggleToDatabricks-0.2/setup.py
```

### Comparing `KaggleToDatabricks-0.1/KaggleToDatabricks.egg-info/PKG-INFO` & `KaggleToDatabricks-0.2/KaggleToDatabricks.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: KaggleToDatabricks
-Version: 0.1
+Version: 0.2
 Summary: Package created for recruitment task
 Home-page: https://github.com/Teneb/kaggle_to_databricks
+Download-URL: https://github.com/Teneb/kaggle_to_databricks/archive/refs/tags/v0.1.tar.gz
 Author: Artur Woźniak
 Author-email: arturwn39@gmail.com
 License: MIT
-Download-URL: https://github.com/Teneb/kaggle_to_databricks/archive/refs/tags/v0.1.tar.gz
 Keywords: pls,hire,me
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE.txt
-
-UNKNOWN
-
```

### Comparing `KaggleToDatabricks-0.1/LICENSE.txt` & `KaggleToDatabricks-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `KaggleToDatabricks-0.1/PKG-INFO` & `KaggleToDatabricks-0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: KaggleToDatabricks
-Version: 0.1
+Version: 0.2
 Summary: Package created for recruitment task
 Home-page: https://github.com/Teneb/kaggle_to_databricks
+Download-URL: https://github.com/Teneb/kaggle_to_databricks/archive/refs/tags/v0.1.tar.gz
 Author: Artur Woźniak
 Author-email: arturwn39@gmail.com
 License: MIT
-Download-URL: https://github.com/Teneb/kaggle_to_databricks/archive/refs/tags/v0.1.tar.gz
 Keywords: pls,hire,me
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE.txt
-
-UNKNOWN
-
```

### Comparing `KaggleToDatabricks-0.1/setup.py` & `KaggleToDatabricks-0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from distutils.core import setup
 setup(
   name = 'KaggleToDatabricks',         # How you named your package folder (MyLib)
   packages = ['KaggleToDatabricks'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Package created for recruitment task',   # Give a short description about your library
   author = 'Artur Woźniak',                   # Type in your name
   author_email = 'arturwn39@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/Teneb/kaggle_to_databricks',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/Teneb/kaggle_to_databricks/archive/refs/tags/v0.1.tar.gz',    # I explain this later on
   keywords = ['pls', 'hire', 'me'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
-          'os',
           'kaggle.api.kaggle_api_extended',
-          'sys',
-          'subprocess',
           'pandas',
           'pyspark.sql'          
       ],
   classifiers=[
     'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
```

