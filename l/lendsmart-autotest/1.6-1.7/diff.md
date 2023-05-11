# Comparing `tmp/lendsmart_autotest-1.6.tar.gz` & `tmp/lendsmart_autotest-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lendsmart_autotest-1.6.tar", last modified: Thu May 11 12:55:26 2023, max compression
+gzip compressed data, was "lendsmart_autotest-1.7.tar", last modified: Thu May 11 13:05:54 2023, max compression
```

## Comparing `lendsmart_autotest-1.6.tar` & `lendsmart_autotest-1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:55:26.270805 lendsmart_autotest-1.6/
--rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-11 12:55:26.270805 lendsmart_autotest-1.6/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:55:26.270805 lendsmart_autotest-1.6/lendsmart_autotest.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-11 12:55:26.000000 lendsmart_autotest-1.6/lendsmart_autotest.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-11 12:55:26.000000 lendsmart_autotest-1.6/lendsmart_autotest.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-11 12:55:26.000000 lendsmart_autotest-1.6/lendsmart_autotest.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      200 2023-05-11 12:55:26.000000 lendsmart_autotest-1.6/lendsmart_autotest.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-11 12:55:26.000000 lendsmart_autotest-1.6/lendsmart_autotest.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-11 12:55:26.270805 lendsmart_autotest-1.6/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1193 2023-05-11 12:54:27.000000 lendsmart_autotest-1.6/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 13:05:54.758183 lendsmart_autotest-1.7/
+-rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-11 13:05:54.758183 lendsmart_autotest-1.7/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 13:05:54.758183 lendsmart_autotest-1.7/lendsmart_autotest.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-11 13:05:54.000000 lendsmart_autotest-1.7/lendsmart_autotest.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-11 13:05:54.000000 lendsmart_autotest-1.7/lendsmart_autotest.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-11 13:05:54.000000 lendsmart_autotest-1.7/lendsmart_autotest.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      200 2023-05-11 13:05:54.000000 lendsmart_autotest-1.7/lendsmart_autotest.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-11 13:05:54.000000 lendsmart_autotest-1.7/lendsmart_autotest.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-11 13:05:54.758183 lendsmart_autotest-1.7/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1193 2023-05-11 13:05:29.000000 lendsmart_autotest-1.7/setup.py
```

### Comparing `lendsmart_autotest-1.6/setup.py` & `lendsmart_autotest-1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import find_packages, setup
 
 here = path.abspath(path.dirname(__file__))
 
 setup(
     name="lendsmart_autotest",
-    version="1.6",
+    version="1.7",
     description="The internal SDK for lendsmart autotest",
     url="https://bitbucket.org/lendsmartlabs/lendsmart_py/",
     # Author details
     author="Lendsmart",
     author_email="infos@lendsmart.ai",
     license="MIT",
     classifiers=[
```

