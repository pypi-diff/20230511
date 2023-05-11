# Comparing `tmp/scripture-0.2.tar.gz` & `tmp/scripture-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scripture-0.2.tar", last modified: Thu May 11 20:26:34 2023, max compression
+gzip compressed data, was "scripture-0.3.tar", last modified: Thu May 11 20:31:02 2023, max compression
```

## Comparing `scripture-0.2.tar` & `scripture-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 20:26:34.061832 scripture-0.2/
--rw-rw-rw-   0        0        0     1088 2023-05-11 19:59:13.000000 scripture-0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      380 2023-05-11 20:26:34.060604 scripture-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      948 2023-05-11 20:21:29.000000 scripture-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 20:26:34.057319 scripture-0.2/scripture.egg-info/
--rw-rw-rw-   0        0        0      380 2023-05-11 20:26:33.000000 scripture-0.2/scripture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-05-11 20:26:33.000000 scripture-0.2/scripture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 20:26:33.000000 scripture-0.2/scripture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-05-11 20:26:33.000000 scripture-0.2/scripture.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 20:26:33.000000 scripture-0.2/scripture.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 20:26:34.061832 scripture-0.2/setup.cfg
--rw-rw-rw-   0        0        0      544 2023-05-11 20:26:20.000000 scripture-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:31:02.637938 scripture-0.3/
+-rw-rw-rw-   0        0        0     1088 2023-05-11 19:59:13.000000 scripture-0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      380 2023-05-11 20:31:02.637938 scripture-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      948 2023-05-11 20:21:29.000000 scripture-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 20:31:02.636429 scripture-0.3/scripture.egg-info/
+-rw-rw-rw-   0        0        0      380 2023-05-11 20:31:02.000000 scripture-0.3/scripture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-05-11 20:31:02.000000 scripture-0.3/scripture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 20:31:02.000000 scripture-0.3/scripture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-05-11 20:31:02.000000 scripture-0.3/scripture.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 20:31:02.000000 scripture-0.3/scripture.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 20:31:02.637938 scripture-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      544 2023-05-11 20:30:32.000000 scripture-0.3/setup.py
```

### Comparing `scripture-0.2/LICENSE.txt` & `scripture-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scripture-0.2/README.md` & `scripture-0.3/README.md`

 * *Files identical despite different names*

### Comparing `scripture-0.2/setup.py` & `scripture-0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='scripture',
-    version='0.2',
+    version='0.3',
     author='Isaac L.B Richardson',
     author_email='isaaclindenbarrierichardson@gmail.com',
     description='A simplistic rule-based AI that is easy to train and use',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

