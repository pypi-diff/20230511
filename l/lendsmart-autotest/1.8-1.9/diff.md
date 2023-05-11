# Comparing `tmp/lendsmart_autotest-1.8.tar.gz` & `tmp/lendsmart_autotest-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lendsmart_autotest-1.8.tar", last modified: Thu May 11 13:08:32 2023, max compression
+gzip compressed data, was "lendsmart_autotest-1.9.tar", last modified: Thu May 11 13:14:06 2023, max compression
```

## Comparing `lendsmart_autotest-1.8.tar` & `lendsmart_autotest-1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 13:08:32.388840 lendsmart_autotest-1.8/
--rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-11 13:08:32.388840 lendsmart_autotest-1.8/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 13:08:32.388840 lendsmart_autotest-1.8/lendsmart_autotest.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-11 13:08:32.000000 lendsmart_autotest-1.8/lendsmart_autotest.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-11 13:08:32.000000 lendsmart_autotest-1.8/lendsmart_autotest.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-11 13:08:32.000000 lendsmart_autotest-1.8/lendsmart_autotest.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      200 2023-05-11 13:08:32.000000 lendsmart_autotest-1.8/lendsmart_autotest.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-11 13:08:32.000000 lendsmart_autotest-1.8/lendsmart_autotest.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-11 13:08:32.388840 lendsmart_autotest-1.8/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1193 2023-05-11 13:08:08.000000 lendsmart_autotest-1.8/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 13:14:06.723255 lendsmart_autotest-1.9/
+-rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-11 13:14:06.723255 lendsmart_autotest-1.9/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 13:14:06.723255 lendsmart_autotest-1.9/lendsmart_autotest.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-11 13:14:06.000000 lendsmart_autotest-1.9/lendsmart_autotest.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-11 13:14:06.000000 lendsmart_autotest-1.9/lendsmart_autotest.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-11 13:14:06.000000 lendsmart_autotest-1.9/lendsmart_autotest.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      200 2023-05-11 13:14:06.000000 lendsmart_autotest-1.9/lendsmart_autotest.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-11 13:14:06.000000 lendsmart_autotest-1.9/lendsmart_autotest.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-11 13:14:06.723255 lendsmart_autotest-1.9/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1193 2023-05-11 13:13:35.000000 lendsmart_autotest-1.9/setup.py
```

### Comparing `lendsmart_autotest-1.8/setup.py` & `lendsmart_autotest-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import find_packages, setup
 
 here = path.abspath(path.dirname(__file__))
 
 setup(
     name="lendsmart_autotest",
-    version="1.8",
+    version="1.9",
     description="The internal SDK for lendsmart autotest",
     url="https://bitbucket.org/lendsmartlabs/lendsmart_py/",
     # Author details
     author="Lendsmart",
     author_email="infos@lendsmart.ai",
     license="MIT",
     classifiers=[
```

