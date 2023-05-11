# Comparing `tmp/ion-numworks.0.0.1.tar.gz` & `tmp/ion-Numworks-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ion.0.0.1.tar", last modified: Thu May 11 18:18:57 2023, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
+gzip compressed data, was "ion-Numworks-1.2.3.tar", last modified: Sun Oct 17 16:07:29 2021, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
```

## Comparing `ion-numworks.0.0.1.tar` & `ion-Numworks-1.2.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2021-10-17 16:06:52.000000 ion.0.0.1/
--rwxrwxrwx   0        0        0      545 2023-05-11 18:18:24.000000 ion.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 1970-01-01 00:00:00.000000 ion.0.0.1/setup.cfg
--rwxrwxrwx   0        0        0      784 2023-05-11 18:18:37.000000 ion.0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 1970-01-01 00:00:00.000000 ion.0.0.1/src/
-drwxrwxrwx   0        0        0        0 2021-10-17 15:58:27.000000 ion.0.0.1/src/ion/
-drwxrwxrwx   0        0        0        0 2021-10-17 16:07:28.000000 ion.0.0.1/src/ion.egg-info/
--rwxrwxrwx   0        0        0        1 2021-10-17 16:07:28.000000 ion.0.0.1/src/ion.egg-info/dependency_links.txt
--rwxrwxrwx   0        0        0      545 2023-05-11 18:18:55.000000 ion.0.0.1/src/ion.egg-info/PKG-INFO
--rwxrwxrwx   0        0        0        1 2023-05-11 18:14:29.000000 ion.0.0.1/src/ion.egg-info/requires.txt
--rwxrwxrwx   0        0        0      217 2021-10-17 16:07:28.000000 ion.0.0.1/src/ion.egg-info/SOURCES.txt
--rwxrwxrwx   0        0        0        3 2021-10-17 15:59:11.000000 ion.0.0.1/src/ion.egg-info/top_level.txt
--rwxrwxrwx   0        0        0       37 2023-05-11 18:13:24.000000 ion.0.0.1/src/ion/__init__.py
+drwxrwxrwx   0        0        0        0 2021-10-17 16:06:52.000000 ion-Numworks-1.2.3/
+-rw-rw-rw-   0        0        0      935 1970-01-01 00:00:00.000000 ion-Numworks-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      273 1970-01-01 00:00:00.000000 ion-Numworks-1.2.3/README.md
+-rw-rw-rw-   0        0        0       42 1970-01-01 00:00:00.000000 ion-Numworks-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1004 1970-01-01 00:00:00.000000 ion-Numworks-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 1970-01-01 00:00:00.000000 ion-Numworks-1.2.3/src/
+drwxrwxrwx   0        0        0        0 2021-10-17 15:58:27.000000 ion-Numworks-1.2.3/src/ion/
+drwxrwxrwx   0        0        0        0 2021-10-17 16:07:28.000000 ion-Numworks-1.2.3/src/ion.egg-info/
+-rwxrwxrwx   0        0        0        1 2021-10-17 16:07:28.000000 ion-Numworks-1.2.3/src/ion.egg-info/dependency_links.txt
+-rwxrwxrwx   0        0        0      935 2021-10-17 16:07:28.000000 ion-Numworks-1.2.3/src/ion.egg-info/PKG-INFO
+-rwxrwxrwx   0        0        0        9 2021-10-17 16:07:28.000000 ion-Numworks-1.2.3/src/ion.egg-info/requires.txt
+-rwxrwxrwx   0        0        0      217 2021-10-17 16:07:28.000000 ion-Numworks-1.2.3/src/ion.egg-info/SOURCES.txt
+-rwxrwxrwx   0        0        0        3 2021-10-17 15:59:11.000000 ion-Numworks-1.2.3/src/ion.egg-info/top_level.txt
+-rwxrwxrwx   0        0        0     1460 2021-08-23 15:19:29.000000 ion-Numworks-1.2.3/src/ion/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ion.0.0.1/PKG-INFO` & `ion-Numworks-1.2.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
-Name: ion-numworks
-Version: 0.01
-Summary: 
+Name: ion-Numworks
+Version: 1.2.3
+Summary: Permet de faire la liason entre les modules ion (de la Numworks) et keyboard.
 Home-page: https://github.com/ZetaMap/Ion-numworks
 Author: ZetaMap
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ZetaMap/Ion-numworks/issues
 Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
 
-no content
+# Ion-numworks
+Un petit module python vous permettant de faire la liason entre les modules ion (de la Numworks) et keyboard. (modules permettant les détections d'appuis de touches)
+
+### Plus
+[Kandinsky module of Numworks](https://github.com/ZetaMap/Kandinsky-Numworks)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ion.0.0.1/setup.py` & `ion-Numworks-1.2.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from setuptools import setup, find_packages
 
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
 setup(
-    name="ion-numworks",
-    version="0.0.1",
+    name="ion-Numworks",
+    version="1.2.3",
     author="ZetaMap",
-    description="",
+    description="Permet de faire la liason entre les modules ion (de la Numworks) et keyboard.",
     license='MIT',
-    long_description="no content,
+    long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/ZetaMap/Ion-numworks",
     project_urls={
         "Bug Tracker": "https://github.com/ZetaMap/Ion-numworks/issues",
     },
     classifiers=[
+        'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: Unix',
         'Operating System :: MacOS :: MacOS X',
     ],
     package_dir={"": "src"},
```

