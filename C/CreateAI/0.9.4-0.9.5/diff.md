# Comparing `tmp/CreateAI-0.9.4.tar.gz` & `tmp/CreateAI-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CreateAI-0.9.4.tar", last modified: Tue May  9 11:48:56 2023, max compression
+gzip compressed data, was "CreateAI-0.9.5.tar", last modified: Tue May  9 11:51:59 2023, max compression
```

## Comparing `CreateAI-0.9.4.tar` & `CreateAI-0.9.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 11:48:56.375935 CreateAI-0.9.4/
-drwxrwxrwx   0        0        0        0 2023-05-09 11:48:56.372927 CreateAI-0.9.4/CreateAI.egg-info/
--rw-rw-rw-   0        0        0     2251 2023-05-09 11:48:56.000000 CreateAI-0.9.4/CreateAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-05-09 11:48:56.000000 CreateAI-0.9.4/CreateAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 11:48:56.000000 CreateAI-0.9.4/CreateAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-09 11:48:56.000000 CreateAI-0.9.4/CreateAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1097 2023-05-05 14:50:25.000000 CreateAI-0.9.4/LICENCE
--rw-rw-rw-   0        0        0       48 2023-05-09 11:48:55.000000 CreateAI-0.9.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2251 2023-05-09 11:48:56.375935 CreateAI-0.9.4/PKG-INFO
--rw-rw-rw-   0        0        0     1806 2023-05-09 11:48:20.000000 CreateAI-0.9.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 11:48:56.377925 CreateAI-0.9.4/setup.cfg
--rw-rw-rw-   0        0        0      671 2023-05-09 11:48:55.000000 CreateAI-0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 11:51:59.966826 CreateAI-0.9.5/
+drwxrwxrwx   0        0        0        0 2023-05-09 11:51:59.965826 CreateAI-0.9.5/CreateAI.egg-info/
+-rw-rw-rw-   0        0        0     2296 2023-05-09 11:51:59.000000 CreateAI-0.9.5/CreateAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-05-09 11:51:59.000000 CreateAI-0.9.5/CreateAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 11:51:59.000000 CreateAI-0.9.5/CreateAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-09 11:51:59.000000 CreateAI-0.9.5/CreateAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1097 2023-05-05 14:50:25.000000 CreateAI-0.9.5/LICENCE
+-rw-rw-rw-   0        0        0       48 2023-05-09 11:51:58.000000 CreateAI-0.9.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2296 2023-05-09 11:51:59.967827 CreateAI-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1851 2023-05-09 11:51:24.000000 CreateAI-0.9.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 11:51:59.968830 CreateAI-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0      671 2023-05-09 11:51:58.000000 CreateAI-0.9.5/setup.py
```

### Comparing `CreateAI-0.9.4/CreateAI.egg-info/PKG-INFO` & `CreateAI-0.9.5/CreateAI.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: CreateAI
-Version: 0.9.4
+Version: 0.9.5
 Summary: Easy tool for creating AI in python
 Home-page: https://github.com/R0fael/CreateAI
 Author: R0fael
 Author-email: roslobodchikov@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 
-# CreateAI v0.9.3
+# CreateAI v0.9.5
 It's easy tool to create ai in python easy and fast.
 You can edit source code of CreateAI on [Create AI's github](https://github.com/R0fael/CreateAI)
 
 ## Dependencies
  - numpy
  - knowledge of python
  - our documentation
@@ -94,13 +94,15 @@
 print(n.process([0, 1, 0])) # test
 ```
 
 ## Change log
 0.8 - First version
 0.8.1 - Little bug fix
 0.9.2 - Speed up
-0.9.4 - convertors
+0.9.3 - Bug Fix
+0.9.4 - Bug Fix of bug fix
+0.9.5 - convertors
 
 ## Plans
 0.10.0 - Saving system
 0.10.1 - Fixing custom functions activation
 0.10.2 - Multi neurons update
```

### Comparing `CreateAI-0.9.4/LICENCE` & `CreateAI-0.9.5/LICENCE`

 * *Files identical despite different names*

### Comparing `CreateAI-0.9.4/PKG-INFO` & `CreateAI-0.9.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: CreateAI
-Version: 0.9.4
+Version: 0.9.5
 Summary: Easy tool for creating AI in python
 Home-page: https://github.com/R0fael/CreateAI
 Author: R0fael
 Author-email: roslobodchikov@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 
-# CreateAI v0.9.3
+# CreateAI v0.9.5
 It's easy tool to create ai in python easy and fast.
 You can edit source code of CreateAI on [Create AI's github](https://github.com/R0fael/CreateAI)
 
 ## Dependencies
  - numpy
  - knowledge of python
  - our documentation
@@ -94,13 +94,15 @@
 print(n.process([0, 1, 0])) # test
 ```
 
 ## Change log
 0.8 - First version
 0.8.1 - Little bug fix
 0.9.2 - Speed up
-0.9.4 - convertors
+0.9.3 - Bug Fix
+0.9.4 - Bug Fix of bug fix
+0.9.5 - convertors
 
 ## Plans
 0.10.0 - Saving system
 0.10.1 - Fixing custom functions activation
 0.10.2 - Multi neurons update
```

### Comparing `CreateAI-0.9.4/README.md` & `CreateAI-0.9.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# CreateAI v0.9.3
+# CreateAI v0.9.5
 It's easy tool to create ai in python easy and fast.
 You can edit source code of CreateAI on [Create AI's github](https://github.com/R0fael/CreateAI)
 
 ## Dependencies
  - numpy
  - knowledge of python
  - our documentation
@@ -80,13 +80,15 @@
 print(n.process([0, 1, 0])) # test
 ```
 
 ## Change log
 0.8 - First version
 0.8.1 - Little bug fix
 0.9.2 - Speed up
-0.9.4 - convertors
+0.9.3 - Bug Fix
+0.9.4 - Bug Fix of bug fix
+0.9.5 - convertors
 
 ## Plans
 0.10.0 - Saving system
 0.10.1 - Fixing custom functions activation
 0.10.2 - Multi neurons update
```

### Comparing `CreateAI-0.9.4/setup.py` & `CreateAI-0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open(r'C:\MyUse\code\python\EasyPack\README.md', 'r', encoding='utf-8') as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name='CreateAI',
-	version='0.9.4',
+	version='0.9.5',
 	author='R0fael',
 	author_email='roslobodchikov@gmail.com',
 	description='Easy tool for creating AI in python',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://github.com/R0fael/CreateAI',
 	packages=['C:\MyUse\code\python\EasyPack\CreateAI'],
```

