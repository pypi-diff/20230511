# Comparing `tmp/widelearning-0.7.5.tar.gz` & `tmp/widelearning-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widelearning-0.7.5.tar", max compression
+gzip compressed data, was "widelearning-0.7.6.tar", max compression
```

## Comparing `widelearning-0.7.5.tar` & `widelearning-0.7.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      354 2023-05-07 04:44:44.856843 widelearning-0.7.5/pyproject.toml
--rw-r--r--   0        0        0    78935 2023-05-07 04:41:00.260607 widelearning-0.7.5/widelearning.py
--rw-r--r--   0        0        0      505 2023-05-07 04:45:09.419025 widelearning-0.7.5/setup.py
--rw-r--r--   0        0        0      514 2023-05-07 04:45:09.419279 widelearning-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0      354 2023-05-11 16:39:33.911395 widelearning-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0    78951 2023-05-11 16:37:44.468704 widelearning-0.7.6/widelearning.py
+-rw-r--r--   0        0        0      505 2023-05-11 16:39:42.287555 widelearning-0.7.6/setup.py
+-rw-r--r--   0        0        0      514 2023-05-11 16:39:42.287791 widelearning-0.7.6/PKG-INFO
```

### Comparing `widelearning-0.7.5/widelearning.py` & `widelearning-0.7.6/widelearning.py`

 * *Files 0% similar despite different names*

```diff
@@ -2130,16 +2130,16 @@
         with open(file_path, 'r') as file:
             lines = file.readlines()
             w.append(lines[0])           
 
     weights = []
 
     for i in range(len(w)):
-    string = w[i].replace("'", "").replace("\n", "")
-    string1 = string.split(',')
+        string = w[i].replace("'", "").replace("\n", "")
+        string1 = string.split(',')
 
     ww = []
 
     for j in range(len(string1)):
         z = string1[j].replace("'", "").replace("\n", "").replace("[", "").replace("]", "")
         ww.append(float(z))
 
@@ -2238,16 +2238,16 @@
         with open(file_path, 'r') as file:
             lines = file.readlines()
             w.append(lines[0])           
 
     weights = []
 
     for i in range(len(w)):
-    string = w[i].replace("'", "").replace("\n", "")
-    string1 = string.split(',')
+        string = w[i].replace("'", "").replace("\n", "")
+        string1 = string.split(',')
 
     ww = []
 
     for j in range(len(string1)):
         z = string1[j].replace("'", "").replace("\n", "").replace("[", "").replace("]", "")
         ww.append(float(z))
```

### Comparing `widelearning-0.7.5/PKG-INFO` & `widelearning-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widelearning
-Version: 0.7.5
+Version: 0.7.6
 Summary: Library for searching the optimal neural network architecture
 Author: Brinkinvision
 Author-email: brinkinvision@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
```

