# Comparing `tmp/SmoobuExtractorFormatter-1.0.1.tar.gz` & `tmp/SmoobuExtractorFormatter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmoobuExtractorFormatter-1.0.1.tar", last modified: Thu May 11 18:38:56 2023, max compression
+gzip compressed data, was "SmoobuExtractorFormatter-1.0.2.tar", last modified: Thu May 11 18:46:14 2023, max compression
```

## Comparing `SmoobuExtractorFormatter-1.0.1.tar` & `SmoobuExtractorFormatter-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 18:38:56.623676 SmoobuExtractorFormatter-1.0.1/
--rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      751 2023-05-11 18:38:56.622642 SmoobuExtractorFormatter-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.0.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-11 18:38:56.619643 SmoobuExtractorFormatter-1.0.1/SmoobuExtractorFormatter.egg-info/
--rw-rw-rw-   0        0        0      751 2023-05-11 18:38:56.000000 SmoobuExtractorFormatter-1.0.1/SmoobuExtractorFormatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-11 18:38:56.000000 SmoobuExtractorFormatter-1.0.1/SmoobuExtractorFormatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 18:38:56.000000 SmoobuExtractorFormatter-1.0.1/SmoobuExtractorFormatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-11 18:38:56.000000 SmoobuExtractorFormatter-1.0.1/SmoobuExtractorFormatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 18:38:56.000000 SmoobuExtractorFormatter-1.0.1/SmoobuExtractorFormatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-05-11 18:20:16.000000 SmoobuExtractorFormatter-1.0.1/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-11 18:38:56.623676 SmoobuExtractorFormatter-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-05-11 18:38:51.000000 SmoobuExtractorFormatter-1.0.1/setup.py
--rw-rw-rw-   0        0        0     6659 2023-05-11 17:15:32.000000 SmoobuExtractorFormatter-1.0.1/smoobuOutput.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:46:14.273644 SmoobuExtractorFormatter-1.0.2/
+-rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      751 2023-05-11 18:46:14.272644 SmoobuExtractorFormatter-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 18:46:14.270640 SmoobuExtractorFormatter-1.0.2/SmoobuExtractorFormatter.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-05-11 18:46:14.000000 SmoobuExtractorFormatter-1.0.2/SmoobuExtractorFormatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-11 18:46:14.000000 SmoobuExtractorFormatter-1.0.2/SmoobuExtractorFormatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 18:46:14.000000 SmoobuExtractorFormatter-1.0.2/SmoobuExtractorFormatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-11 18:46:14.000000 SmoobuExtractorFormatter-1.0.2/SmoobuExtractorFormatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 18:46:14.000000 SmoobuExtractorFormatter-1.0.2/SmoobuExtractorFormatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6659 2023-05-11 18:45:15.000000 SmoobuExtractorFormatter-1.0.2/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-11 18:46:14.274648 SmoobuExtractorFormatter-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-05-11 18:46:08.000000 SmoobuExtractorFormatter-1.0.2/setup.py
+-rw-rw-rw-   0        0        0     6659 2023-05-11 17:15:32.000000 SmoobuExtractorFormatter-1.0.2/smoobuOutput.py
```

### Comparing `SmoobuExtractorFormatter-1.0.1/LICENSE.txt` & `SmoobuExtractorFormatter-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SmoobuExtractorFormatter-1.0.1/PKG-INFO` & `SmoobuExtractorFormatter-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.0.1/SmoobuExtractorFormatter.egg-info/PKG-INFO` & `SmoobuExtractorFormatter-1.0.2/SmoobuExtractorFormatter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.0.1/setup.py` & `SmoobuExtractorFormatter-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='SmoobuExtractorFormatter',
-    version='1.0.1',
+    version='1.0.2',
     description='A library to format the output of the Smoobu application',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     uri='',
     author='Badji Rayane',
     author_email='rayanebadji.freelance@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

### Comparing `SmoobuExtractorFormatter-1.0.1/smoobuOutput.py` & `SmoobuExtractorFormatter-1.0.2/__init__.py`

 * *Files identical despite different names*

