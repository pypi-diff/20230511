# Comparing `tmp/solscan-0.1.4.tar.gz` & `tmp/solscan-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solscan-0.1.4.tar", last modified: Thu May 11 10:21:21 2023, max compression
+gzip compressed data, was "solscan-0.1.5.tar", last modified: Thu May 11 10:28:09 2023, max compression
```

## Comparing `solscan-0.1.4.tar` & `solscan-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 10:21:21.992681 solscan-0.1.4/
--rw-r--r--   0 manosriram   (501) staff       (20)      986 2023-05-11 10:21:21.992559 solscan-0.1.4/PKG-INFO
--rw-r--r--   0 manosriram   (501) staff       (20)      798 2023-05-11 06:27:08.000000 solscan-0.1.4/README.md
--rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-05-11 10:21:21.992718 solscan-0.1.4/setup.cfg
--rw-r--r--   0 manosriram   (501) staff       (20)      771 2023-05-11 10:21:10.000000 solscan-0.1.4/setup.py
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 10:21:21.991623 solscan-0.1.4/solscan/
--rw-r--r--   0 manosriram   (501) staff       (20)     3505 2023-05-11 10:11:37.000000 solscan-0.1.4/solscan/__init__.py
--rw-r--r--   0 manosriram   (501) staff       (20)     1792 2023-05-11 10:11:41.000000 solscan-0.1.4/solscan/config.py
--rw-r--r--   0 manosriram   (501) staff       (20)      158 2023-05-11 10:11:21.000000 solscan-0.1.4/solscan/constants.py
--rw-r--r--   0 manosriram   (501) staff       (20)     1345 2023-05-11 10:11:44.000000 solscan-0.1.4/solscan/exceptions.py
--rw-r--r--   0 manosriram   (501) staff       (20)      905 2023-05-11 10:11:46.000000 solscan-0.1.4/solscan/lang.py
--rw-r--r--   0 manosriram   (501) staff       (20)     2899 2023-05-11 10:11:31.000000 solscan-0.1.4/solscan/scan.py
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 10:21:21.992407 solscan-0.1.4/solscan.egg-info/
--rw-r--r--   0 manosriram   (501) staff       (20)      986 2023-05-11 10:21:21.000000 solscan-0.1.4/solscan.egg-info/PKG-INFO
--rw-r--r--   0 manosriram   (501) staff       (20)      319 2023-05-11 10:21:21.000000 solscan-0.1.4/solscan.egg-info/SOURCES.txt
--rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-05-11 10:21:21.000000 solscan-0.1.4/solscan.egg-info/dependency_links.txt
--rw-r--r--   0 manosriram   (501) staff       (20)       53 2023-05-11 10:21:21.000000 solscan-0.1.4/solscan.egg-info/entry_points.txt
--rw-r--r--   0 manosriram   (501) staff       (20)      113 2023-05-11 10:21:21.000000 solscan-0.1.4/solscan.egg-info/requires.txt
--rw-r--r--   0 manosriram   (501) staff       (20)        8 2023-05-11 10:21:21.000000 solscan-0.1.4/solscan.egg-info/top_level.txt
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 10:28:09.613265 solscan-0.1.5/
+-rw-r--r--   0 manosriram   (501) staff       (20)      986 2023-05-11 10:28:09.613153 solscan-0.1.5/PKG-INFO
+-rw-r--r--   0 manosriram   (501) staff       (20)      798 2023-05-11 06:27:08.000000 solscan-0.1.5/README.md
+-rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-05-11 10:28:09.613299 solscan-0.1.5/setup.cfg
+-rw-r--r--   0 manosriram   (501) staff       (20)     1257 2023-05-11 10:28:03.000000 solscan-0.1.5/setup.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 10:28:09.612289 solscan-0.1.5/solscan/
+-rw-r--r--   0 manosriram   (501) staff       (20)     3505 2023-05-11 10:11:37.000000 solscan-0.1.5/solscan/__init__.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     1792 2023-05-11 10:11:41.000000 solscan-0.1.5/solscan/config.py
+-rw-r--r--   0 manosriram   (501) staff       (20)      158 2023-05-11 10:11:21.000000 solscan-0.1.5/solscan/constants.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     1345 2023-05-11 10:11:44.000000 solscan-0.1.5/solscan/exceptions.py
+-rw-r--r--   0 manosriram   (501) staff       (20)      905 2023-05-11 10:11:46.000000 solscan-0.1.5/solscan/lang.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     2899 2023-05-11 10:11:31.000000 solscan-0.1.5/solscan/scan.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 10:28:09.613005 solscan-0.1.5/solscan.egg-info/
+-rw-r--r--   0 manosriram   (501) staff       (20)      986 2023-05-11 10:28:09.000000 solscan-0.1.5/solscan.egg-info/PKG-INFO
+-rw-r--r--   0 manosriram   (501) staff       (20)      319 2023-05-11 10:28:09.000000 solscan-0.1.5/solscan.egg-info/SOURCES.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-05-11 10:28:09.000000 solscan-0.1.5/solscan.egg-info/dependency_links.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)       53 2023-05-11 10:28:09.000000 solscan-0.1.5/solscan.egg-info/entry_points.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)      401 2023-05-11 10:28:09.000000 solscan-0.1.5/solscan.egg-info/requires.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)        8 2023-05-11 10:28:09.000000 solscan-0.1.5/solscan.egg-info/top_level.txt
```

### Comparing `solscan-0.1.4/PKG-INFO` & `solscan-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solscan
-Version: 0.1.4
+Version: 0.1.5
 Summary: Get your smart contracts audited by a smarter tool
 Home-page: https://solidityscan.com
 Description-Content-Type: text/markdown
 
 ## solscan
 
 ## Installation
```

### Comparing `solscan-0.1.4/README.md` & `solscan-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `solscan-0.1.4/setup.py` & `solscan-0.1.5/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,27 +2,45 @@
 import os
 
 def readme():
     with open(os.path.join(os.path.dirname(__file__), 'README.md')) as f:
         return f.read()
 
 setup(name="solscan",
-      version="0.1.4",
+      version="0.1.5",
       description="Get your smart contracts audited by a smarter tool",
       long_description=readme(),
       long_description_content_type='text/markdown',
       url="https://solidityscan.com",
       entry_points={
         'console_scripts': [
             'solscan=solscan.__init__:solscan',
         ],
       },
       packages=find_packages(),
       install_requires=[
+        "anyio==3.6.2",
+        "beautifulsoup4==4.12.2",
+        "certifi==2023.5.7",
+        "chardet==5.1.0",
+        "charset-normalizer==3.1.0",
         "click==8.1.3",
         "deep-translator==1.10.1",
+        "h11==0.14.0",
+        "h2==4.1.0",
+        "hpack==4.0.0",
+        "hstspreload==2023.1.1",
+        "httpcore==0.17.0",
+        "httpx==0.24.0",
+        "hyperframe==6.0.1",
+        "idna==3.4",
         "loguru==0.7.0",
-        "requests==2.29.0",
-        "ruamel.yaml==0.17.22",
+        "requests==2.30.0",
+        "rfc3986==2.0.0",
+        "ruamel.yaml==0.17.26",
         "ruamel.yaml.clib==0.2.7",
+        "sniffio==1.3.0",
+        "solscan==0.1.4",
+        "soupsieve==2.4.1",
+        "urllib3==2.0.2",
     ]
 )
```

### Comparing `solscan-0.1.4/solscan/__init__.py` & `solscan-0.1.5/solscan/__init__.py`

 * *Files identical despite different names*

### Comparing `solscan-0.1.4/solscan/config.py` & `solscan-0.1.5/solscan/config.py`

 * *Files identical despite different names*

### Comparing `solscan-0.1.4/solscan/exceptions.py` & `solscan-0.1.5/solscan/exceptions.py`

 * *Files identical despite different names*

### Comparing `solscan-0.1.4/solscan/lang.py` & `solscan-0.1.5/solscan/lang.py`

 * *Files identical despite different names*

### Comparing `solscan-0.1.4/solscan/scan.py` & `solscan-0.1.5/solscan/scan.py`

 * *Files identical despite different names*

### Comparing `solscan-0.1.4/solscan.egg-info/PKG-INFO` & `solscan-0.1.5/solscan.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solscan
-Version: 0.1.4
+Version: 0.1.5
 Summary: Get your smart contracts audited by a smarter tool
 Home-page: https://solidityscan.com
 Description-Content-Type: text/markdown
 
 ## solscan
 
 ## Installation
```

