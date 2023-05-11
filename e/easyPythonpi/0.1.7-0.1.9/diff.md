# Comparing `tmp/easyPythonpi-0.1.7.tar.gz` & `tmp/easyPythonpi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyPythonpi-0.1.7.tar", last modified: Sun Feb 12 14:57:28 2023, max compression
+gzip compressed data, was "easyPythonpi-0.1.9.tar", last modified: Thu May 11 10:09:10 2023, max compression
```

## Comparing `easyPythonpi-0.1.7.tar` & `easyPythonpi-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-12 14:57:28.036140 easyPythonpi-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (116)      499 2023-02-12 14:57:28.036140 easyPythonpi-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2257 2023-02-12 14:57:19.000000 easyPythonpi-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-12 14:57:28.032140 easyPythonpi-0.1.7/easyPythonpi/
--rw-r--r--   0 runner    (1001) docker     (116)     4986 2023-02-12 14:57:19.000000 easyPythonpi-0.1.7/easyPythonpi/TestBin2Hex.py
--rw-r--r--   0 runner    (1001) docker     (116)       40 2023-02-12 14:57:19.000000 easyPythonpi-0.1.7/easyPythonpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12871 2023-02-12 14:57:19.000000 easyPythonpi-0.1.7/easyPythonpi/easyPythonpi.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-12 14:57:28.036140 easyPythonpi-0.1.7/easyPythonpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      499 2023-02-12 14:57:28.000000 easyPythonpi-0.1.7/easyPythonpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      279 2023-02-12 14:57:28.000000 easyPythonpi-0.1.7/easyPythonpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-12 14:57:28.000000 easyPythonpi-0.1.7/easyPythonpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2023-02-12 14:57:28.000000 easyPythonpi-0.1.7/easyPythonpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2023-02-12 14:57:28.000000 easyPythonpi-0.1.7/easyPythonpi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-02-12 14:57:28.036140 easyPythonpi-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1554 2023-02-12 14:57:19.000000 easyPythonpi-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:09:10.655319 easyPythonpi-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-11 10:09:10.655319 easyPythonpi-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-11 10:08:59.000000 easyPythonpi-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:09:10.655319 easyPythonpi-0.1.9/easyPythonpi/
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-05-11 10:08:59.000000 easyPythonpi-0.1.9/easyPythonpi/TestBin2Hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-11 10:08:59.000000 easyPythonpi-0.1.9/easyPythonpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-05-11 10:08:59.000000 easyPythonpi-0.1.9/easyPythonpi/easyPythonpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:09:10.655319 easyPythonpi-0.1.9/easyPythonpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-11 10:09:10.000000 easyPythonpi-0.1.9/easyPythonpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-11 10:09:10.000000 easyPythonpi-0.1.9/easyPythonpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:09:10.000000 easyPythonpi-0.1.9/easyPythonpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 10:09:10.000000 easyPythonpi-0.1.9/easyPythonpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 10:09:10.000000 easyPythonpi-0.1.9/easyPythonpi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 10:09:10.655319 easyPythonpi-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-11 10:08:59.000000 easyPythonpi-0.1.9/setup.py
```

### Comparing `easyPythonpi-0.1.7/README.md` & `easyPythonpi-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `easyPythonpi-0.1.7/easyPythonpi/easyPythonpi.py` & `easyPythonpi-0.1.9/easyPythonpi/easyPythonpi.py`

 * *Files 9% similar despite different names*

```diff
@@ -204,16 +204,58 @@
             h = 'C' + h
         elif substring == '1101':
             h = 'D' + h
         elif substring == '1110':
             h = 'E' + h
         elif substring == '1111':
             h = 'F' + h
+            
+    return h 
 
-    return h        
+
+def bin2oct(x:'bin')->'oct':  
+    o = ''  # hexadecimal number converted from binary and to be returned
+
+    x=str(x)
+    
+    # Determine if the string has invalid characters
+    if re.search('[^(0-1)]', x):
+        raise InvalidBinaryException 
+
+    # Get the length of the string
+    l=len(x)
+
+    # Begin the process of converting x to its hexadecimal number
+
+    # If the length is not a multiple of 3, prepend 0's before converting
+    if l % 3 != 0:
+        numZerosPrepended = 3 - ( l % 3 ) # number of zeros to prepend 
+        x = (numZerosPrepended * '0') + x # concatenate numZerosPrepended to x
+
+    for i in range(len(x), 0, -3):
+        substring = x[i-3:i]
+
+        if substring == '000':
+            o = '0' + o
+        elif substring == '001':
+            o = '1' + o
+        elif substring == '010':
+            o = '2' + o
+        elif substring == '011':
+            o = '3' + o
+        elif substring == '100':
+            o = '4' + o                        
+        elif substring == '101':
+            o = '5' + o        
+        elif substring == '110':
+            o = '6' + o
+        elif substring == '111':
+            o = '7' + o    
+
+    return o
 
 def createarray(length:'int',dtype='int')->'array':   # To create an array of entered length and entered data type(interger data type is a default data type)
     import numpy as np 
     a=[]  #empty list
     for i in range(length):
         # if entered dtype is an interger
             if dtype=='int':
```

### Comparing `easyPythonpi-0.1.7/setup.py` & `easyPythonpi-0.1.9/setup.py`

 * *Files identical despite different names*

