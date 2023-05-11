# Comparing `tmp/betby-0.2.2.tar.gz` & `tmp/betby-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betby-0.2.2.tar", last modified: Wed May 10 23:17:21 2023, max compression
+gzip compressed data, was "betby-0.2.3.tar", last modified: Thu May 11 09:55:12 2023, max compression
```

## Comparing `betby-0.2.2.tar` & `betby-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 23:17:21.786810 betby-0.2.2/
--rw-rw-rw-   0        0        0      539 2023-05-10 23:17:21.784814 betby-0.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 23:17:21.752900 betby-0.2.2/betby/
--rw-rw-rw-   0        0        0       21 2023-05-09 23:44:47.000000 betby-0.2.2/betby/__init__.py
--rw-rw-rw-   0        0        0     5962 2023-05-10 23:16:03.000000 betby-0.2.2/betby/markets.py
-drwxrwxrwx   0        0        0        0 2023-05-10 23:17:21.779827 betby-0.2.2/betby.egg-info/
--rw-rw-rw-   0        0        0      539 2023-05-10 23:17:19.000000 betby-0.2.2/betby.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-05-10 23:17:20.000000 betby-0.2.2/betby.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 23:17:19.000000 betby-0.2.2/betby.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 23:17:19.000000 betby-0.2.2/betby.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 23:17:21.787807 betby-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      637 2023-05-10 23:16:24.000000 betby-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:55:12.354224 betby-0.2.3/
+-rw-rw-rw-   0        0        0      539 2023-05-11 09:55:12.352101 betby-0.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-11 09:55:12.332157 betby-0.2.3/betby/
+-rw-rw-rw-   0        0        0       21 2023-05-09 23:44:47.000000 betby-0.2.3/betby/__init__.py
+-rw-rw-rw-   0        0        0     6238 2023-05-11 09:53:02.000000 betby-0.2.3/betby/markets.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:55:12.349110 betby-0.2.3/betby.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-05-11 09:55:10.000000 betby-0.2.3/betby.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-05-11 09:55:11.000000 betby-0.2.3/betby.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 09:55:10.000000 betby-0.2.3/betby.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-11 09:55:10.000000 betby-0.2.3/betby.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 09:55:12.354224 betby-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      637 2023-05-11 09:53:28.000000 betby-0.2.3/setup.py
```

### Comparing `betby-0.2.2/PKG-INFO` & `betby-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betby
-Version: 0.2.2
+Version: 0.2.3
 Summary: Betby libraries
 Author: Ayrat Badrutdinov
 Author-email: a.badrutdinov@betby.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betby-0.2.2/betby.egg-info/PKG-INFO` & `betby-0.2.3/betby.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betby
-Version: 0.2.2
+Version: 0.2.3
 Summary: Betby libraries
 Author: Ayrat Badrutdinov
 Author-email: a.badrutdinov@betby.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betby-0.2.2/setup.py` & `betby-0.2.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="betby",
-    version="0.2.2",
+    version="0.2.3",
     author="Ayrat Badrutdinov",
     author_email="a.badrutdinov@betby.com",
     description="Betby libraries",
     packages=["betby"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

