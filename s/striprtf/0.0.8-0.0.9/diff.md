# Comparing `tmp/striprtf-0.0.8.tar.gz` & `tmp/striprtf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/striprtf-0.0.8.tar", last modified: Fri Feb 21 08:32:38 2020, max compression
+gzip compressed data, was "dist/striprtf-0.0.9.tar", last modified: Thu Mar 12 09:38:45 2020, max compression
```

## Comparing `striprtf-0.0.8.tar` & `striprtf-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 joshy     (1000) joshy     (1000)        0 2020-02-21 08:32:38.000000 striprtf-0.0.8/
-drwxrwxr-x   0 joshy     (1000) joshy     (1000)        0 2020-02-21 08:32:38.000000 striprtf-0.0.8/striprtf.egg-info/
--rw-rw-r--   0 joshy     (1000) joshy     (1000)        9 2020-02-21 08:32:38.000000 striprtf-0.0.8/striprtf.egg-info/top_level.txt
--rw-rw-r--   0 joshy     (1000) joshy     (1000)        1 2020-02-21 08:32:38.000000 striprtf-0.0.8/striprtf.egg-info/dependency_links.txt
--rw-rw-r--   0 joshy     (1000) joshy     (1000)     1582 2020-02-21 08:32:38.000000 striprtf-0.0.8/striprtf.egg-info/PKG-INFO
--rw-rw-r--   0 joshy     (1000) joshy     (1000)      237 2020-02-21 08:32:38.000000 striprtf-0.0.8/striprtf.egg-info/SOURCES.txt
--rw-rw-r--   0 joshy     (1000) joshy     (1000)       79 2020-02-21 08:32:38.000000 striprtf-0.0.8/setup.cfg
-drwxrwxr-x   0 joshy     (1000) joshy     (1000)        0 2020-02-21 08:32:38.000000 striprtf-0.0.8/striprtf/
--rw-rw-r--   0 joshy     (1000) joshy     (1000)      403 2019-02-15 10:00:30.000000 striprtf-0.0.8/striprtf/striprtf
--rw-rw-r--   0 joshy     (1000) joshy     (1000)       34 2020-02-21 08:25:44.000000 striprtf-0.0.8/striprtf/__init__.py
--rw-rw-r--   0 joshy     (1000) joshy     (1000)     6546 2020-02-21 08:25:44.000000 striprtf-0.0.8/striprtf/striprtf.py
--rw-rw-r--   0 joshy     (1000) joshy     (1000)       21 2020-02-21 08:29:49.000000 striprtf-0.0.8/striprtf/_version.py
--rw-rw-r--   0 joshy     (1000) joshy     (1000)      890 2020-02-21 08:29:25.000000 striprtf-0.0.8/setup.py
--rw-r--r--   0 joshy     (1000) joshy     (1000)      953 2019-06-26 08:19:15.000000 striprtf-0.0.8/README.md
--rw-rw-r--   0 joshy     (1000) joshy     (1000)     1582 2020-02-21 08:32:38.000000 striprtf-0.0.8/PKG-INFO
+drwxr-xr-x   0 irrwitz    (501) staff       (20)        0 2020-03-12 09:38:45.000000 striprtf-0.0.9/
+-rw-r--r--   0 irrwitz    (501) staff       (20)     1625 2020-03-12 09:38:45.000000 striprtf-0.0.9/PKG-INFO
+drwxr-xr-x   0 irrwitz    (501) staff       (20)        0 2020-03-12 09:38:45.000000 striprtf-0.0.9/striprtf.egg-info/
+-rw-r--r--   0 irrwitz    (501) staff       (20)     1625 2020-03-12 09:38:45.000000 striprtf-0.0.9/striprtf.egg-info/PKG-INFO
+-rw-r--r--   0 irrwitz    (501) staff       (20)      246 2020-03-12 09:38:45.000000 striprtf-0.0.9/striprtf.egg-info/SOURCES.txt
+-rw-r--r--   0 irrwitz    (501) staff       (20)        9 2020-03-12 09:38:45.000000 striprtf-0.0.9/striprtf.egg-info/top_level.txt
+-rw-r--r--   0 irrwitz    (501) staff       (20)        1 2020-03-12 09:38:45.000000 striprtf-0.0.9/striprtf.egg-info/dependency_links.txt
+-rw-r--r--   0 irrwitz    (501) staff       (20)      988 2020-01-27 23:29:17.000000 striprtf-0.0.9/README.md
+-rw-r--r--   0 irrwitz    (501) staff       (20)      890 2020-03-12 08:49:48.000000 striprtf-0.0.9/setup.py
+drwxr-xr-x   0 irrwitz    (501) staff       (20)        0 2020-03-12 09:38:45.000000 striprtf-0.0.9/striprtf/
+-rw-r--r--   0 irrwitz    (501) staff       (20)       21 2020-03-12 09:37:19.000000 striprtf-0.0.9/striprtf/_version.py
+-rw-r--r--   0 irrwitz    (501) staff       (20)     7783 2020-03-12 09:24:40.000000 striprtf-0.0.9/striprtf/striprtf.py
+-rw-r--r--   0 irrwitz    (501) staff       (20)       34 2020-01-27 23:29:17.000000 striprtf-0.0.9/striprtf/__init__.py
+-rw-r--r--   0 irrwitz    (501) staff       (20)      622 2020-03-12 09:33:48.000000 striprtf-0.0.9/striprtf/striprtf
+-rw-r--r--   0 irrwitz    (501) staff       (20)       79 2020-03-12 09:38:45.000000 striprtf-0.0.9/setup.cfg
```

### Comparing `striprtf-0.0.8/striprtf.egg-info/PKG-INFO` & `striprtf-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: striprtf
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple library to convert rtf to text
 Home-page: https://github.com/joshy/striprtf
 Author: Joshy Cyriac
 Author-email: j.cyriac@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/joshy/striprtf/archive/v0.0.8.tar.gz
+Download-URL: https://github.com/joshy/striprtf/archive/v0.0.9.tar.gz
 Description: # striprtf
         [![Build Status](https://api.travis-ci.org/joshy/striprtf.svg?branch=master)](https://travis-ci.org/joshy/striprtf)
         
         ## Purpose
         This is a simple library to convert rtf files to python strings. A lot of
         medical documents are written in rtf format which is not ideal for parsing
         and further processing. This library converts it to plain old text.
@@ -31,15 +31,16 @@
         [Pyth](https://github.com/brendonh/pyth) was not working for the rtf files I
         had. The next best thing was this gist:
         https://gist.github.com/gilsondev/7c1d2d753ddb522e7bc22511cfb08676
         
         Very few additions where made, e.g. better formatting of tables.
         
         ## Pushing to PyPi
-        Run command
+        Run commands
         ```
+        python setup.py sdist bdist_wheel
         python setup.py sdist upload -r pypi
         ```
         
 Keywords: rtf
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `striprtf-0.0.8/setup.py` & `striprtf-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `striprtf-0.0.8/README.md` & `striprtf-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,11 +22,12 @@
 [Pyth](https://github.com/brendonh/pyth) was not working for the rtf files I
 had. The next best thing was this gist:
 https://gist.github.com/gilsondev/7c1d2d753ddb522e7bc22511cfb08676
 
 Very few additions where made, e.g. better formatting of tables.
 
 ## Pushing to PyPi
-Run command
+Run commands
 ```
+python setup.py sdist bdist_wheel
 python setup.py sdist upload -r pypi
 ```
```

### Comparing `striprtf-0.0.8/PKG-INFO` & `striprtf-0.0.9/striprtf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: striprtf
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple library to convert rtf to text
 Home-page: https://github.com/joshy/striprtf
 Author: Joshy Cyriac
 Author-email: j.cyriac@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/joshy/striprtf/archive/v0.0.8.tar.gz
+Download-URL: https://github.com/joshy/striprtf/archive/v0.0.9.tar.gz
 Description: # striprtf
         [![Build Status](https://api.travis-ci.org/joshy/striprtf.svg?branch=master)](https://travis-ci.org/joshy/striprtf)
         
         ## Purpose
         This is a simple library to convert rtf files to python strings. A lot of
         medical documents are written in rtf format which is not ideal for parsing
         and further processing. This library converts it to plain old text.
@@ -31,15 +31,16 @@
         [Pyth](https://github.com/brendonh/pyth) was not working for the rtf files I
         had. The next best thing was this gist:
         https://gist.github.com/gilsondev/7c1d2d753ddb522e7bc22511cfb08676
         
         Very few additions where made, e.g. better formatting of tables.
         
         ## Pushing to PyPi
-        Run command
+        Run commands
         ```
+        python setup.py sdist bdist_wheel
         python setup.py sdist upload -r pypi
         ```
         
 Keywords: rtf
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

