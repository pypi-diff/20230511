# Comparing `tmp/unigui-1.4.3.tar.gz` & `tmp/unigui-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.4.3.tar", last modified: Sun May  7 23:44:05 2023, max compression
+gzip compressed data, was "dist/unigui-1.4.4.tar", last modified: Thu May 11 15:37:46 2023, max compression
```

## Comparing `unigui-1.4.3.tar` & `unigui-1.4.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 23:44:05.000000 unigui-1.4.3/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui/
--rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.4.3/unigui/manager.py
--rw-rw-r--   0 george    (1000) george    (1000)     7695 2023-05-03 16:32:01.000000 unigui-1.4.3/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.4.3/unigui/userset.py
--rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:39.000000 unigui-1.4.3/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.4.3/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.4.3/unigui/utils.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/css/748.d94da9c0.css
--rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/css/vendor.49a52e8f.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)   847622 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/js/vendor.c0de6c67.js
--rw-rw-r--   0 george    (1000) george    (1000)    39996 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/js/748.67c1fce8.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/js/193.b4cc3ffe.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/js/430.4be6e8a8.js
--rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/js/app.73e4276f.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-05-07 23:39:56.000000 unigui-1.4.3/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.4.3/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      585 2023-05-07 23:43:23.000000 unigui-1.4.3/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19428 2023-05-07 23:44:05.000000 unigui-1.4.3/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-07 23:44:05.000000 unigui-1.4.3/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    19138 2023-05-03 16:32:01.000000 unigui-1.4.3/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.4.3/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       30 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19428 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.4.3/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1223 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-05-07 23:44:05.000000 unigui-1.4.3/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 15:37:46.000000 unigui-1.4.4/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui/
+-rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.4.4/unigui/manager.py
+-rw-rw-r--   0 george    (1000) george    (1000)     7831 2023-05-11 09:43:13.000000 unigui-1.4.4/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.4.4/unigui/userset.py
+-rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:39.000000 unigui-1.4.4/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.4.4/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.4.4/unigui/utils.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/css/603.d94da9c0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/css/vendor.49a52e8f.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)   847622 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/js/vendor.c0de6c67.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/js/193.b4cc3ffe.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/js/430.4be6e8a8.js
+-rw-rw-r--   0 george    (1000) george    (1000)    40010 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/js/603.baf52338.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/js/app.a12bb431.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.4.4/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      585 2023-05-11 15:37:06.000000 unigui-1.4.4/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19428 2023-05-11 15:37:46.000000 unigui-1.4.4/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-11 15:37:46.000000 unigui-1.4.4/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    19138 2023-05-08 23:39:42.000000 unigui-1.4.4/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.4.4/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       30 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19428 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.4.4/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1223 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.4.3/unigui/manager.py` & `unigui-1.4.4/unigui/manager.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/guielements.py` & `unigui-1.4.4/unigui/guielements.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,37 +125,40 @@
         super().__init__(*args, **kwargs)         
         self.type = 'tree' 
         if not hasattr(self,'options'):
             self.options = {}        
         if not hasattr(self,'value'):
             self.value = None
 
-def accept_cell_value( _, val):
+def accept_cell_value( _, val):    
     value, position = val
+    try:
+        value = float(value)        
+    except ValueError:
+        pass
     _.rows[position[0]][position[1]] = value    
 
-def standart_table_delete(t, _):
-    if len(t.rows) == 0:
-        return
-    keyed = len(t.headers) < len(t.rows[0])
-    value = t.value    
-    if isinstance(value, list):        
-        if keyed:
-            t.rows = [row for row in t.rows if row[-1] not in value]
+def standart_table_delete(t, value):
+    if t.rows:        
+        keyed = len(t.headers) < len(t.rows[0])
+        t.value = value   
+        if isinstance(value, list):        
+            if keyed:
+                t.rows = [row for row in t.rows if row[-1] not in value]
+            else:
+                value.sort(reverse=True)
+                for v in value:            
+                    del t.rows[v]
+            t.value = []
         else:
-            value.sort(reverse=True)
-            for v in value:            
-                del t.rows[v]
-        t.value = []
-    else:
-        if keyed:            
-            t.rows = [row for row in t.rows if row[-1] != value]
-        else:
-            del t.rows[value]  
-        t.value = None    
+            if keyed:            
+                t.rows = [row for row in t.rows if row[-1] != value]
+            else:
+                del t.rows[value]  
+            t.value = None    
 
 class Table(Gui):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)             
         self.check('rows', 'headers','value')
         if not hasattr(self,'edit') or self.edit:
             if not hasattr(self,'modify'):
```

### Comparing `unigui-1.4.3/unigui/server.py` & `unigui-1.4.4/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/utils.py` & `unigui-1.4.4/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/favicon.ico` & `unigui-1.4.4/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/css/748.d94da9c0.css` & `unigui-1.4.4/unigui/web/css/603.d94da9c0.css`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.4.4/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/icons/favicon-96x96.png` & `unigui-1.4.4/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/icons/favicon-16x16.png` & `unigui-1.4.4/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/icons/favicon-32x32.png` & `unigui-1.4.4/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/icons/favicon-128x128.png` & `unigui-1.4.4/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.4.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.4.4/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.4.4/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.4.4/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.4.4/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.4.4/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.4.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.4.4/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/js/vendor.c0de6c67.js` & `unigui-1.4.4/unigui/web/js/vendor.c0de6c67.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/js/748.67c1fce8.js` & `unigui-1.4.4/unigui/web/js/603.baf52338.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [748], {
-        9748: (e, t, a) => {
+    [603], {
+        7603: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => Qt
             });
             var l = a(3673),
                 s = a(2323);
             const i = (0, l._)("div", {
                 class: "q-pa-lg"
@@ -1078,15 +1078,15 @@
                             let a = this.rows;
                             a[t][this.data.headers[this.cedit]] = e, this.sendMessage("#", [e, [t, this.cedit]])
                         }
                     },
                     keyInput(e) {
                         if ("Control" != e.key) switch (g && console.log("keypress", e), e.key) {
                             case "Enter":
-                                "update" in this.data && this.sendMessage("->", [this.data.rows[this.redit][this.cedit],
+                                "update" in this.data && this.sendMessage("->", [this.rows[this.redit][this.data.headers[this.cedit]],
                                     [this.redit, this.cedit]
                                 ]);
                                 break;
                             case "Escape":
                                 this.switchEdit();
                                 break;
                             case "ArrowLeft":
```

### Comparing `unigui-1.4.3/unigui/web/js/193.b4cc3ffe.js` & `unigui-1.4.4/unigui/web/js/193.b4cc3ffe.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/js/430.4be6e8a8.js` & `unigui-1.4.4/unigui/web/js/430.4be6e8a8.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui/web/js/app.73e4276f.js` & `unigui-1.4.4/unigui/web/js/app.a12bb431.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(748)]).then(r.bind(r, 9748)),
+                        component: () => Promise.all([r.e(736), r.e(603)]).then(r.bind(r, 7603)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -44,30 +44,30 @@
                                     top: 0
                                 }),
                                 routes: v,
                                 history: e("")
                             });
                         return t
                     }));
-                async function g(e, t) {
+                async function b(e, t) {
                     const r = "function" === typeof m ? await m({}) : m,
                         n = e(d);
                     return n.use(o.Z, t), {
                         app: n,
                         router: r
                     }
                 }
-                var b = r(6417),
+                var g = r(6417),
                     y = r(5597);
                 const w = {
                         config: {
                             notify: {}
                         },
                         plugins: {
-                            Notify: b.Z,
+                            Notify: g.Z,
                             Dialog: y.Z
                         }
                     },
                     O = "";
                 async function k({
                     app: e,
                     router: t
@@ -94,15 +94,15 @@
                             urlPath: i,
                             publicPath: O
                         })
                     } catch (l) {
                         return l && l.url ? void a(l.url) : void console.error("[Quasar] boot error:", l)
                     }!0 !== n && (e.use(t), e.mount("#q-app"))
                 }
-                g(n.ri, w).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
+                b(n.ri, w).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
                     const r = t.map((e => e.default)).filter((e => "function" === typeof e));
                     k(e, r)
                 }))))
             },
             2390: (e, t, r) => {
                 r.r(t), r.d(t, {
                     default: () => o
@@ -160,24 +160,24 @@
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "b4cc3ffe",
             430: "4be6e8a8",
-            748: "67c1fce8"
+            603: "baf52338"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            736: "49a52e8f",
-            748: "d94da9c0"
+            603: "d94da9c0",
+            736: "49a52e8f"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
             } catch (e) {
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                748: 1
+                603: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
```

### Comparing `unigui-1.4.3/unigui/web/index.html` & `unigui-1.4.4/unigui/web/index.html`

 * *Files 11% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.c0de6c67.js></script><script defer src=js/app.73e4276f.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.c0de6c67.js></script><script defer src=js/app.a12bb431.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.4.3/LICENSE` & `unigui-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/setup.py` & `unigui-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.4.3',      
+      version='1.4.4',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal app browser',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.4.3/PKG-INFO` & `unigui-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.4.3
+Version: 1.4.4
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.4.3/README.md` & `unigui-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `unigui-1.4.3/unigui.egg-info/PKG-INFO` & `unigui-1.4.4/unigui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.4.3
+Version: 1.4.4
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.4.3/unigui.egg-info/SOURCES.txt` & `unigui-1.4.4/unigui.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/748.d94da9c0.css
+unigui/web/css/603.d94da9c0.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.49a52e8f.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -29,10 +29,10 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.b4cc3ffe.js
 unigui/web/js/430.4be6e8a8.js
-unigui/web/js/748.67c1fce8.js
-unigui/web/js/app.73e4276f.js
+unigui/web/js/603.baf52338.js
+unigui/web/js/app.a12bb431.js
 unigui/web/js/vendor.c0de6c67.js
```

