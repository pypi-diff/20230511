# Comparing `tmp/SDTcloud-0.1.8.tar.gz` & `tmp/SDTcloud-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SDTcloud-0.1.8.tar", last modified: Thu May  4 08:06:20 2023, max compression
+gzip compressed data, was "SDTcloud-0.1.9.tar", last modified: Thu May  4 08:18:33 2023, max compression
```

## Comparing `SDTcloud-0.1.8.tar` & `SDTcloud-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 08:06:20.198544 SDTcloud-0.1.8/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 08:06:20.198356 SDTcloud-0.1.8/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)       12 2023-05-04 01:12:59.000000 SDTcloud-0.1.8/README.md
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 08:06:20.196930 SDTcloud-0.1.8/SDTcloud/
--rw-r--r--   0 june       (501) staff       (20)       75 2023-05-04 01:12:59.000000 SDTcloud-0.1.8/SDTcloud/__init__.py
--rw-r--r--   0 june       (501) staff       (20)    10861 2023-05-04 08:06:09.000000 SDTcloud-0.1.8/SDTcloud/sdtcloud.py
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 08:06:20.198063 SDTcloud-0.1.8/SDTcloud.egg-info/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 08:06:20.000000 SDTcloud-0.1.8/SDTcloud.egg-info/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)      188 2023-05-04 08:06:20.000000 SDTcloud-0.1.8/SDTcloud.egg-info/SOURCES.txt
--rw-r--r--   0 june       (501) staff       (20)        1 2023-05-04 08:06:20.000000 SDTcloud-0.1.8/SDTcloud.egg-info/dependency_links.txt
--rw-r--r--   0 june       (501) staff       (20)        9 2023-05-04 08:06:20.000000 SDTcloud-0.1.8/SDTcloud.egg-info/top_level.txt
--rw-r--r--   0 june       (501) staff       (20)       38 2023-05-04 08:06:20.198588 SDTcloud-0.1.8/setup.cfg
--rw-r--r--   0 june       (501) staff       (20)      656 2023-05-04 08:06:16.000000 SDTcloud-0.1.8/setup.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 08:18:33.388619 SDTcloud-0.1.9/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 08:18:33.388480 SDTcloud-0.1.9/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)       12 2023-05-04 01:12:59.000000 SDTcloud-0.1.9/README.md
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 08:18:33.387395 SDTcloud-0.1.9/SDTcloud/
+-rw-r--r--   0 june       (501) staff       (20)       75 2023-05-04 01:12:59.000000 SDTcloud-0.1.9/SDTcloud/__init__.py
+-rw-r--r--   0 june       (501) staff       (20)    10839 2023-05-04 08:18:20.000000 SDTcloud-0.1.9/SDTcloud/sdtcloud.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 08:18:33.388284 SDTcloud-0.1.9/SDTcloud.egg-info/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 08:18:33.000000 SDTcloud-0.1.9/SDTcloud.egg-info/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)      188 2023-05-04 08:18:33.000000 SDTcloud-0.1.9/SDTcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 june       (501) staff       (20)        1 2023-05-04 08:18:33.000000 SDTcloud-0.1.9/SDTcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 june       (501) staff       (20)        9 2023-05-04 08:18:33.000000 SDTcloud-0.1.9/SDTcloud.egg-info/top_level.txt
+-rw-r--r--   0 june       (501) staff       (20)       38 2023-05-04 08:18:33.388653 SDTcloud-0.1.9/setup.cfg
+-rw-r--r--   0 june       (501) staff       (20)      656 2023-05-04 08:18:28.000000 SDTcloud-0.1.9/setup.py
```

### Comparing `SDTcloud-0.1.8/SDTcloud/sdtcloud.py` & `SDTcloud-0.1.9/SDTcloud/sdtcloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,9 +347,8 @@
         if respStatus == 0:
             self.exceptionHandle(response, returnMessage)
 
         result = json.loads(response.content)
         result['createdAt'] = datetime.fromtimestamp(int(result['createdAt']/1000), timezone(timedelta(hours=9)))
         result['modifiedAt'] = datetime.fromtimestamp(int(result['modifiedAt']/1000), timezone(timedelta(hours=9)))
         
-        print(returnMessage)
-        return result
+        print(returnMessage)
```

### Comparing `SDTcloud-0.1.8/setup.py` & `SDTcloud-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SDTcloud", # Replace with your own username
-    version="0.1.8",
+    version="0.1.9",
     author="sujune",
     author_email="hoakw@sdt.inc",
     description="SDT cloud API Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

