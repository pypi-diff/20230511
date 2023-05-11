# Comparing `tmp/solscan-0.1.2.tar.gz` & `tmp/solscan-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solscan-0.1.2.tar", last modified: Thu May 11 06:54:10 2023, max compression
+gzip compressed data, was "solscan-0.1.3.tar", last modified: Thu May 11 10:12:17 2023, max compression
```

## Comparing `solscan-0.1.2.tar` & `solscan-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 06:54:10.182411 solscan-0.1.2/
--rw-r--r--   0 manosriram   (501) staff       (20)      986 2023-05-11 06:54:10.182241 solscan-0.1.2/PKG-INFO
--rw-r--r--   0 manosriram   (501) staff       (20)      798 2023-05-11 06:27:08.000000 solscan-0.1.2/README.md
--rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-05-11 06:54:10.182455 solscan-0.1.2/setup.cfg
--rw-r--r--   0 manosriram   (501) staff       (20)     1209 2023-05-11 06:53:58.000000 solscan-0.1.2/setup.py
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 06:54:10.181462 solscan-0.1.2/solscan/
--rw-r--r--   0 manosriram   (501) staff       (20)     3505 2023-05-11 06:48:21.000000 solscan-0.1.2/solscan/__init__.py
--rw-r--r--   0 manosriram   (501) staff       (20)     1792 2023-05-11 06:48:12.000000 solscan-0.1.2/solscan/config.py
--rw-r--r--   0 manosriram   (501) staff       (20)       57 2023-05-11 05:17:41.000000 solscan-0.1.2/solscan/constants.py
--rw-r--r--   0 manosriram   (501) staff       (20)     1345 2023-05-11 06:48:28.000000 solscan-0.1.2/solscan/exceptions.py
--rw-r--r--   0 manosriram   (501) staff       (20)      905 2023-05-11 06:48:31.000000 solscan-0.1.2/solscan/lang.py
--rw-r--r--   0 manosriram   (501) staff       (20)     2899 2023-05-11 06:48:06.000000 solscan-0.1.2/solscan/scan.py
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 06:54:10.182086 solscan-0.1.2/solscan.egg-info/
--rw-r--r--   0 manosriram   (501) staff       (20)      986 2023-05-11 06:54:10.000000 solscan-0.1.2/solscan.egg-info/PKG-INFO
--rw-r--r--   0 manosriram   (501) staff       (20)      319 2023-05-11 06:54:10.000000 solscan-0.1.2/solscan.egg-info/SOURCES.txt
--rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-05-11 06:54:10.000000 solscan-0.1.2/solscan.egg-info/dependency_links.txt
--rw-r--r--   0 manosriram   (501) staff       (20)       53 2023-05-11 06:54:10.000000 solscan-0.1.2/solscan.egg-info/entry_points.txt
--rw-r--r--   0 manosriram   (501) staff       (20)      375 2023-05-11 06:54:10.000000 solscan-0.1.2/solscan.egg-info/requires.txt
--rw-r--r--   0 manosriram   (501) staff       (20)        8 2023-05-11 06:54:10.000000 solscan-0.1.2/solscan.egg-info/top_level.txt
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 10:12:17.497073 solscan-0.1.3/
+-rw-r--r--   0 manosriram   (501) staff       (20)      986 2023-05-11 10:12:17.496974 solscan-0.1.3/PKG-INFO
+-rw-r--r--   0 manosriram   (501) staff       (20)      798 2023-05-11 06:27:08.000000 solscan-0.1.3/README.md
+-rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-05-11 10:12:17.497107 solscan-0.1.3/setup.cfg
+-rw-r--r--   0 manosriram   (501) staff       (20)     1209 2023-05-11 10:11:56.000000 solscan-0.1.3/setup.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 10:12:17.496241 solscan-0.1.3/solscan/
+-rw-r--r--   0 manosriram   (501) staff       (20)     3505 2023-05-11 10:11:37.000000 solscan-0.1.3/solscan/__init__.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     1792 2023-05-11 10:11:41.000000 solscan-0.1.3/solscan/config.py
+-rw-r--r--   0 manosriram   (501) staff       (20)      158 2023-05-11 10:11:21.000000 solscan-0.1.3/solscan/constants.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     1345 2023-05-11 10:11:44.000000 solscan-0.1.3/solscan/exceptions.py
+-rw-r--r--   0 manosriram   (501) staff       (20)      905 2023-05-11 10:11:46.000000 solscan-0.1.3/solscan/lang.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     2899 2023-05-11 10:11:31.000000 solscan-0.1.3/solscan/scan.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 10:12:17.496840 solscan-0.1.3/solscan.egg-info/
+-rw-r--r--   0 manosriram   (501) staff       (20)      986 2023-05-11 10:12:17.000000 solscan-0.1.3/solscan.egg-info/PKG-INFO
+-rw-r--r--   0 manosriram   (501) staff       (20)      319 2023-05-11 10:12:17.000000 solscan-0.1.3/solscan.egg-info/SOURCES.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-05-11 10:12:17.000000 solscan-0.1.3/solscan.egg-info/dependency_links.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)       53 2023-05-11 10:12:17.000000 solscan-0.1.3/solscan.egg-info/entry_points.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)      375 2023-05-11 10:12:17.000000 solscan-0.1.3/solscan.egg-info/requires.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)        8 2023-05-11 10:12:17.000000 solscan-0.1.3/solscan.egg-info/top_level.txt
```

### Comparing `solscan-0.1.2/PKG-INFO` & `solscan-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solscan
-Version: 0.1.2
+Version: 0.1.3
 Summary: Get your smart contracts audited by a smarter tool
 Home-page: https://solidityscan.com
 Description-Content-Type: text/markdown
 
 ## solscan
 
 ## Installation
```

### Comparing `solscan-0.1.2/README.md` & `solscan-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `solscan-0.1.2/setup.py` & `solscan-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 def readme():
     with open(os.path.join(os.path.dirname(__file__), 'README.md')) as f:
         return f.read()
 
 setup(name="solscan",
-      version="0.1.2",
+      version="0.1.3",
       description="Get your smart contracts audited by a smarter tool",
       long_description=readme(),
       long_description_content_type='text/markdown',
       url="https://solidityscan.com",
       entry_points={
         'console_scripts': [
             'solscan=solscan.__init__:solscan',
```

### Comparing `solscan-0.1.2/solscan/__init__.py` & `solscan-0.1.3/solscan/__init__.py`

 * *Files identical despite different names*

### Comparing `solscan-0.1.2/solscan/config.py` & `solscan-0.1.3/solscan/config.py`

 * *Files identical despite different names*

### Comparing `solscan-0.1.2/solscan/exceptions.py` & `solscan-0.1.3/solscan/exceptions.py`

 * *Files identical despite different names*

### Comparing `solscan-0.1.2/solscan/lang.py` & `solscan-0.1.3/solscan/lang.py`

 * *Files identical despite different names*

### Comparing `solscan-0.1.2/solscan/scan.py` & `solscan-0.1.3/solscan/scan.py`

 * *Files identical despite different names*

### Comparing `solscan-0.1.2/solscan.egg-info/PKG-INFO` & `solscan-0.1.3/solscan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solscan
-Version: 0.1.2
+Version: 0.1.3
 Summary: Get your smart contracts audited by a smarter tool
 Home-page: https://solidityscan.com
 Description-Content-Type: text/markdown
 
 ## solscan
 
 ## Installation
```

