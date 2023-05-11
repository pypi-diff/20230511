# Comparing `tmp/solscan-0.1.8.tar.gz` & `tmp/solscan-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solscan-0.1.8.tar", last modified: Thu May 11 10:31:55 2023, max compression
+gzip compressed data, was "solscan-0.1.9.tar", last modified: Thu May 11 10:33:29 2023, max compression
```

## Comparing `solscan-0.1.8.tar` & `solscan-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 10:31:55.274721 solscan-0.1.8/
--rw-r--r--   0 manosriram   (501) staff       (20)      986 2023-05-11 10:31:55.274582 solscan-0.1.8/PKG-INFO
--rw-r--r--   0 manosriram   (501) staff       (20)      798 2023-05-11 06:27:08.000000 solscan-0.1.8/README.md
--rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-05-11 10:31:55.274760 solscan-0.1.8/setup.cfg
--rw-r--r--   0 manosriram   (501) staff       (20)     1230 2023-05-11 10:31:52.000000 solscan-0.1.8/setup.py
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 10:31:55.273384 solscan-0.1.8/solscan/
--rw-r--r--   0 manosriram   (501) staff       (20)     3505 2023-05-11 10:11:37.000000 solscan-0.1.8/solscan/__init__.py
--rw-r--r--   0 manosriram   (501) staff       (20)     1792 2023-05-11 10:11:41.000000 solscan-0.1.8/solscan/config.py
--rw-r--r--   0 manosriram   (501) staff       (20)      158 2023-05-11 10:11:21.000000 solscan-0.1.8/solscan/constants.py
--rw-r--r--   0 manosriram   (501) staff       (20)     1345 2023-05-11 10:11:44.000000 solscan-0.1.8/solscan/exceptions.py
--rw-r--r--   0 manosriram   (501) staff       (20)      905 2023-05-11 10:11:46.000000 solscan-0.1.8/solscan/lang.py
--rw-r--r--   0 manosriram   (501) staff       (20)     2899 2023-05-11 10:11:31.000000 solscan-0.1.8/solscan/scan.py
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 10:31:55.274407 solscan-0.1.8/solscan.egg-info/
--rw-r--r--   0 manosriram   (501) staff       (20)      986 2023-05-11 10:31:55.000000 solscan-0.1.8/solscan.egg-info/PKG-INFO
--rw-r--r--   0 manosriram   (501) staff       (20)      319 2023-05-11 10:31:55.000000 solscan-0.1.8/solscan.egg-info/SOURCES.txt
--rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-05-11 10:31:55.000000 solscan-0.1.8/solscan.egg-info/dependency_links.txt
--rw-r--r--   0 manosriram   (501) staff       (20)       53 2023-05-11 10:31:55.000000 solscan-0.1.8/solscan.egg-info/entry_points.txt
--rw-r--r--   0 manosriram   (501) staff       (20)      385 2023-05-11 10:31:55.000000 solscan-0.1.8/solscan.egg-info/requires.txt
--rw-r--r--   0 manosriram   (501) staff       (20)        8 2023-05-11 10:31:55.000000 solscan-0.1.8/solscan.egg-info/top_level.txt
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 10:33:29.584599 solscan-0.1.9/
+-rw-r--r--   0 manosriram   (501) staff       (20)      986 2023-05-11 10:33:29.584483 solscan-0.1.9/PKG-INFO
+-rw-r--r--   0 manosriram   (501) staff       (20)      798 2023-05-11 06:27:08.000000 solscan-0.1.9/README.md
+-rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-05-11 10:33:29.584630 solscan-0.1.9/setup.cfg
+-rw-r--r--   0 manosriram   (501) staff       (20)     1232 2023-05-11 10:33:26.000000 solscan-0.1.9/setup.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 10:33:29.583632 solscan-0.1.9/solscan/
+-rw-r--r--   0 manosriram   (501) staff       (20)     3505 2023-05-11 10:11:37.000000 solscan-0.1.9/solscan/__init__.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     1792 2023-05-11 10:11:41.000000 solscan-0.1.9/solscan/config.py
+-rw-r--r--   0 manosriram   (501) staff       (20)      158 2023-05-11 10:11:21.000000 solscan-0.1.9/solscan/constants.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     1345 2023-05-11 10:11:44.000000 solscan-0.1.9/solscan/exceptions.py
+-rw-r--r--   0 manosriram   (501) staff       (20)      905 2023-05-11 10:11:46.000000 solscan-0.1.9/solscan/lang.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     2899 2023-05-11 10:11:31.000000 solscan-0.1.9/solscan/scan.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 10:33:29.584327 solscan-0.1.9/solscan.egg-info/
+-rw-r--r--   0 manosriram   (501) staff       (20)      986 2023-05-11 10:33:29.000000 solscan-0.1.9/solscan.egg-info/PKG-INFO
+-rw-r--r--   0 manosriram   (501) staff       (20)      319 2023-05-11 10:33:29.000000 solscan-0.1.9/solscan.egg-info/SOURCES.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-05-11 10:33:29.000000 solscan-0.1.9/solscan.egg-info/dependency_links.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)       53 2023-05-11 10:33:29.000000 solscan-0.1.9/solscan.egg-info/entry_points.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)      387 2023-05-11 10:33:29.000000 solscan-0.1.9/solscan.egg-info/requires.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)        8 2023-05-11 10:33:29.000000 solscan-0.1.9/solscan.egg-info/top_level.txt
```

### Comparing `solscan-0.1.8/PKG-INFO` & `solscan-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solscan
-Version: 0.1.8
+Version: 0.1.9
 Summary: Get your smart contracts audited by a smarter tool
 Home-page: https://solidityscan.com
 Description-Content-Type: text/markdown
 
 ## solscan
 
 ## Installation
```

### Comparing `solscan-0.1.8/README.md` & `solscan-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `solscan-0.1.8/setup.py` & `solscan-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 def readme():
     with open(os.path.join(os.path.dirname(__file__), 'README.md')) as f:
         return f.read()
 
 setup(name="solscan",
-      version="0.1.8",
+      version="0.1.9",
       description="Get your smart contracts audited by a smarter tool",
       long_description=readme(),
       long_description_content_type='text/markdown',
       url="https://solidityscan.com",
       entry_points={
         'console_scripts': [
             'solscan=solscan.__init__:solscan',
@@ -18,15 +18,15 @@
       },
       packages=find_packages(),
       install_requires=[
         "anyio==3.6.2",
         "beautifulsoup4==4.12.2",
         "certifi==2023.5.7",
         "chardet==5.1.0",
-        "charset-normalizer==2.9",
+        "charset-normalizer==2.1.1",
         "click==8.1.3",
         "deep-translator==1.10.1",
         "h11==0.14.0",
         "h2==4.1.0",
         "hpack==4.0.0",
         "hstspreload==2023.1.1",
         "httpcore==0.17.0",
```

### Comparing `solscan-0.1.8/solscan/__init__.py` & `solscan-0.1.9/solscan/__init__.py`

 * *Files identical despite different names*

### Comparing `solscan-0.1.8/solscan/config.py` & `solscan-0.1.9/solscan/config.py`

 * *Files identical despite different names*

### Comparing `solscan-0.1.8/solscan/exceptions.py` & `solscan-0.1.9/solscan/exceptions.py`

 * *Files identical despite different names*

### Comparing `solscan-0.1.8/solscan/lang.py` & `solscan-0.1.9/solscan/lang.py`

 * *Files identical despite different names*

### Comparing `solscan-0.1.8/solscan/scan.py` & `solscan-0.1.9/solscan/scan.py`

 * *Files identical despite different names*

### Comparing `solscan-0.1.8/solscan.egg-info/PKG-INFO` & `solscan-0.1.9/solscan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solscan
-Version: 0.1.8
+Version: 0.1.9
 Summary: Get your smart contracts audited by a smarter tool
 Home-page: https://solidityscan.com
 Description-Content-Type: text/markdown
 
 ## solscan
 
 ## Installation
```

