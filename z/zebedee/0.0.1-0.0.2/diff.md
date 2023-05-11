# Comparing `tmp/zebedee-0.0.1.tar.gz` & `tmp/zebedee-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zebedee-0.0.1.tar", last modified: Thu May 11 05:13:53 2023, max compression
+gzip compressed data, was "zebedee-0.0.2.tar", last modified: Thu May 11 05:56:20 2023, max compression
```

## Comparing `zebedee-0.0.1.tar` & `zebedee-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-11 05:13:53.142123 zebedee-0.0.1/
--rw-r--r--   0 santos     (501) staff       (20)     1065 2023-04-03 00:04:47.000000 zebedee-0.0.1/LICENSE
--rw-r--r--   0 santos     (501) staff       (20)     6912 2023-05-11 05:13:53.142005 zebedee-0.0.1/PKG-INFO
--rw-r--r--   0 santos     (501) staff       (20)     6324 2023-04-04 03:34:21.000000 zebedee-0.0.1/README.md
--rw-r--r--   0 santos     (501) staff       (20)       38 2023-05-11 05:13:53.142161 zebedee-0.0.1/setup.cfg
--rw-r--r--   0 santos     (501) staff       (20)     1171 2023-05-11 05:13:28.000000 zebedee-0.0.1/setup.py
-drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-11 05:13:53.141099 zebedee-0.0.1/zbd/
--rw-r--r--   0 santos     (501) staff       (20)       17 2023-05-11 05:00:30.000000 zebedee-0.0.1/zbd/__init__.py
--rw-r--r--   0 santos     (501) staff       (20)    10840 2023-05-07 00:47:26.000000 zebedee-0.0.1/zbd/zbd.py
-drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-11 05:13:53.141841 zebedee-0.0.1/zebedee.egg-info/
--rw-r--r--   0 santos     (501) staff       (20)     6912 2023-05-11 05:13:53.000000 zebedee-0.0.1/zebedee.egg-info/PKG-INFO
--rw-r--r--   0 santos     (501) staff       (20)      207 2023-05-11 05:13:53.000000 zebedee-0.0.1/zebedee.egg-info/SOURCES.txt
--rw-r--r--   0 santos     (501) staff       (20)        1 2023-05-11 05:13:53.000000 zebedee-0.0.1/zebedee.egg-info/dependency_links.txt
--rw-r--r--   0 santos     (501) staff       (20)       49 2023-05-11 05:13:53.000000 zebedee-0.0.1/zebedee.egg-info/requires.txt
--rw-r--r--   0 santos     (501) staff       (20)        4 2023-05-11 05:13:53.000000 zebedee-0.0.1/zebedee.egg-info/top_level.txt
+drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-11 05:56:20.574799 zebedee-0.0.2/
+-rw-r--r--   0 santos     (501) staff       (20)     1065 2023-04-03 00:04:47.000000 zebedee-0.0.2/LICENSE
+-rw-r--r--   0 santos     (501) staff       (20)     6912 2023-05-11 05:56:20.574554 zebedee-0.0.2/PKG-INFO
+-rw-r--r--   0 santos     (501) staff       (20)     6324 2023-04-04 03:34:21.000000 zebedee-0.0.2/README.md
+-rw-r--r--   0 santos     (501) staff       (20)       38 2023-05-11 05:56:20.574858 zebedee-0.0.2/setup.cfg
+-rw-r--r--   0 santos     (501) staff       (20)     1167 2023-05-11 05:54:38.000000 zebedee-0.0.2/setup.py
+drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-11 05:56:20.571457 zebedee-0.0.2/zebedee/
+-rw-r--r--   0 santos     (501) staff       (20)       19 2023-05-11 05:51:33.000000 zebedee-0.0.2/zebedee/__init__.py
+-rw-r--r--   0 santos     (501) staff       (20)    10852 2023-05-11 05:51:16.000000 zebedee-0.0.2/zebedee/main.py
+drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-11 05:56:20.572280 zebedee-0.0.2/zebedee.egg-info/
+-rw-r--r--   0 santos     (501) staff       (20)     6912 2023-05-11 05:56:20.000000 zebedee-0.0.2/zebedee.egg-info/PKG-INFO
+-rw-r--r--   0 santos     (501) staff       (20)      216 2023-05-11 05:56:20.000000 zebedee-0.0.2/zebedee.egg-info/SOURCES.txt
+-rw-r--r--   0 santos     (501) staff       (20)        1 2023-05-11 05:56:20.000000 zebedee-0.0.2/zebedee.egg-info/dependency_links.txt
+-rw-r--r--   0 santos     (501) staff       (20)       49 2023-05-11 05:56:20.000000 zebedee-0.0.2/zebedee.egg-info/requires.txt
+-rw-r--r--   0 santos     (501) staff       (20)        8 2023-05-11 05:56:20.000000 zebedee-0.0.2/zebedee.egg-info/top_level.txt
```

### Comparing `zebedee-0.0.1/LICENSE` & `zebedee-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zebedee-0.0.1/PKG-INFO` & `zebedee-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zebedee
-Version: 0.0.1
+Version: 0.0.2
 Summary: Move Money at the Speed of the Internet 
 Author: zantoshi (Santos Hernandez)
 Author-email: <santosdhernandez@gmail.com>
 Keywords: python,payments,bitcoin,lightning network,django,lightning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zebedee-0.0.1/README.md` & `zebedee-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `zebedee-0.0.1/setup.py` & `zebedee-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Move Money at the Speed of the Internet '
 LONG_DESCRIPTION = 'A package that allows for faster integration of the ZEBEDEE API.'
 
 # Setting up
 setup(
     name="zebedee",
     version=VERSION,
     author="zantoshi (Santos Hernandez)",
     author_email="<santosdhernandez@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
-    packages=find_packages(),
+    packages=["zebedee"],
     install_requires=['certifi', 'charset-normalizer', 'idna', 'requests', 'urllib3'],
     keywords=['python', 'payments', 'bitcoin', 'lightning network', 'django', 'lightning'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

### Comparing `zebedee-0.0.1/zbd/zbd.py` & `zebedee-0.0.2/zebedee/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     '''
 
     def __init__(self, apikey, callback_url = None):
         self.apikey = apikey
         self.callback_url = callback_url
 
     def __str__(self):
-        return "ZBD Object"
+        return "ZEBEDEE Project Object"
 
     '''
         Charge Actions
     '''
 
     def get_wallet_details(self):
         URL = 'https://api.zebedee.io/v0/wallet'
```

### Comparing `zebedee-0.0.1/zebedee.egg-info/PKG-INFO` & `zebedee-0.0.2/zebedee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zebedee
-Version: 0.0.1
+Version: 0.0.2
 Summary: Move Money at the Speed of the Internet 
 Author: zantoshi (Santos Hernandez)
 Author-email: <santosdhernandez@gmail.com>
 Keywords: python,payments,bitcoin,lightning network,django,lightning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

