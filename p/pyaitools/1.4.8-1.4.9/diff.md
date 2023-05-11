# Comparing `tmp/pyaitools-1.4.8-py3-none-any.whl.zip` & `tmp/pyaitools-1.4.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9019 bytes, number of entries: 11
+Zip file size: 9027 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 22-Mar-21 09:12 pyaitools/__init__.py
 -rw-r--r--  2.0 unx     2263 b- defN 23-Mar-02 06:34 pyaitools/detect.py
 -rw-r--r--  2.0 unx     1353 b- defN 23-Mar-02 05:44 pyaitools/loss.py
--rw-r--r--  2.0 unx      902 b- defN 23-Mar-15 06:20 pyaitools/similar.py
+-rw-r--r--  2.0 unx      910 b- defN 23-Mar-15 06:50 pyaitools/similar.py
 -rw-r--r--  2.0 unx    12212 b- defN 23-Mar-15 06:05 pyaitools/theT.py
 -rw-r--r--  2.0 unx     1277 b- defN 23-Mar-02 06:33 pyaitools/weight_pooled_output.py
--rw-r--r--  2.0 unx     1096 b- defN 23-Mar-15 06:22 pyaitools-1.4.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      698 b- defN 23-Mar-15 06:22 pyaitools-1.4.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-15 06:22 pyaitools-1.4.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Mar-15 06:22 pyaitools-1.4.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      861 b- defN 23-Mar-15 06:22 pyaitools-1.4.8.dist-info/RECORD
-11 files, 20764 bytes uncompressed, 7569 bytes compressed:  63.5%
+-rw-r--r--  2.0 unx     1096 b- defN 23-Mar-15 06:56 pyaitools-1.4.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      698 b- defN 23-Mar-15 06:56 pyaitools-1.4.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-15 06:56 pyaitools-1.4.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Mar-15 06:56 pyaitools-1.4.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      861 b- defN 23-Mar-15 06:56 pyaitools-1.4.9.dist-info/RECORD
+11 files, 20772 bytes uncompressed, 7577 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: pyaitools/theT.py
 Comment: 
 
 Filename: pyaitools/weight_pooled_output.py
 Comment: 
 
-Filename: pyaitools-1.4.8.dist-info/LICENSE
+Filename: pyaitools-1.4.9.dist-info/LICENSE
 Comment: 
 
-Filename: pyaitools-1.4.8.dist-info/METADATA
+Filename: pyaitools-1.4.9.dist-info/METADATA
 Comment: 
 
-Filename: pyaitools-1.4.8.dist-info/WHEEL
+Filename: pyaitools-1.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: pyaitools-1.4.8.dist-info/top_level.txt
+Filename: pyaitools-1.4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pyaitools-1.4.8.dist-info/RECORD
+Filename: pyaitools-1.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyaitools/similar.py

```diff
@@ -21,12 +21,12 @@
             c_list.append(c_set)
     return c_list 
 
 
 
 
 if __name__ == "__main__":
-    input_list = ["A","B","C"]
-    similar_input_list = ["a","b","c"]
+    input_list = ["A","B","C","A"]
+    similar_input_list = ["a","b","c","b"]
     c_list = find_connected_area(input_list, similar_input_list)
     print(c_list)
     # [{'A', 'a'}, {'B', 'b'}, {'c', 'C'}]
```

## Comparing `pyaitools-1.4.8.dist-info/LICENSE` & `pyaitools-1.4.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyaitools-1.4.8.dist-info/METADATA` & `pyaitools-1.4.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaitools
-Version: 1.4.8
+Version: 1.4.9
 Summary: AI tools-code!
 Home-page: https://github.com/AITutorials/aitools/
 Author: Stephen.Z
 Author-email: 15242200221@163.com
 License: MIT
 Keywords: python ai tools
 Platform: UNKNOWN
```

