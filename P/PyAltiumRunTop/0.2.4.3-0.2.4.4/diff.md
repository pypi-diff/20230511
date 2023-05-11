# Comparing `tmp/PyAltiumRunTop-0.2.4.3.tar.gz` & `tmp/PyAltiumRunTop-0.2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAltiumRunTop-0.2.4.3.tar", last modified: Mon Mar  6 02:08:38 2023, max compression
+gzip compressed data, was "PyAltiumRunTop-0.2.4.4.tar", last modified: Mon Mar  6 02:14:23 2023, max compression
```

## Comparing `PyAltiumRunTop-0.2.4.3.tar` & `PyAltiumRunTop-0.2.4.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-03-06 02:08:38.657683 PyAltiumRunTop-0.2.4.3/
--rw-rw-rw-   0        0        0     1051 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.3/LICENSE
--rw-rw-rw-   0        0        0       33 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2735 2023-03-06 02:08:38.657683 PyAltiumRunTop-0.2.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     1879 2023-03-02 09:07:41.000000 PyAltiumRunTop-0.2.4.3/README.md
--rw-rw-rw-   0        0        0      819 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.3/pyproject.toml
--rw-rw-rw-   0        0        0     1228 2023-03-06 02:08:38.658681 PyAltiumRunTop-0.2.4.3/setup.cfg
--rw-rw-rw-   0        0        0       69 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-06 02:08:38.638894 PyAltiumRunTop-0.2.4.3/src/
-drwxrwxrwx   0        0        0        0 2023-03-06 02:08:38.646903 PyAltiumRunTop-0.2.4.3/src/PyAltiumRun.egg-info/
--rw-rw-rw-   0        0        0     2672 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      575 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 09:14:50.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRun.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       73 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRun.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRun.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-06 02:08:38.648898 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop/
--rw-rw-rw-   0        0        0    14566 2023-03-03 06:17:54.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop/AltiumRun.py
--rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 02:08:38.654692 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop/helpers/
--rw-rw-rw-   0        0        0     1987 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop/helpers/AltiumHelper.py
--rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop/helpers/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop/py.typed
-drwxrwxrwx   0        0        0        0 2023-03-06 02:08:38.656686 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop/scriptingbase/
--rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop/scriptingbase/__init__.py
--rw-rw-rw-   0        0        0      525 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop/scriptingbase/logger.pas
--rw-rw-rw-   0        0        0      478 2023-02-27 09:06:28.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop/scriptingbase/main.pas
--rw-rw-rw-   0        0        0     7285 2023-03-06 02:08:36.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop/scriptingbase/updateSitNum0302.pas
-drwxrwxrwx   0        0        0        0 2023-03-06 02:08:38.653691 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop.egg-info/
--rw-rw-rw-   0        0        0     2735 2023-03-06 02:08:38.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      903 2023-03-06 02:08:38.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-06 02:08:38.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 09:40:41.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       73 2023-03-06 02:08:38.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-06 02:08:38.000000 PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-06 02:14:23.707089 PyAltiumRunTop-0.2.4.4/
+-rw-rw-rw-   0        0        0     1051 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2735 2023-03-06 02:14:23.707089 PyAltiumRunTop-0.2.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1879 2023-03-02 09:07:41.000000 PyAltiumRunTop-0.2.4.4/README.md
+-rw-rw-rw-   0        0        0      819 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1228 2023-03-06 02:14:23.708086 PyAltiumRunTop-0.2.4.4/setup.cfg
+-rw-rw-rw-   0        0        0       69 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-06 02:14:23.687668 PyAltiumRunTop-0.2.4.4/src/
+drwxrwxrwx   0        0        0        0 2023-03-06 02:14:23.697113 PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/
+-rw-rw-rw-   0        0        0     2672 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      575 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-27 09:14:50.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       73 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-06 02:14:23.698113 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/
+-rw-rw-rw-   0        0        0    14566 2023-03-03 06:17:54.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/AltiumRun.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-06 02:14:23.704097 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/helpers/
+-rw-rw-rw-   0        0        0     1987 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/helpers/AltiumHelper.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/helpers/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/py.typed
+drwxrwxrwx   0        0        0        0 2023-03-06 02:14:23.706091 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/scriptingbase/
+-rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/scriptingbase/__init__.py
+-rw-rw-rw-   0        0        0      525 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/scriptingbase/logger.pas
+-rw-rw-rw-   0        0        0      478 2023-02-27 09:06:28.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/scriptingbase/main.pas
+-rw-rw-rw-   0        0        0     7285 2023-03-06 02:14:13.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/scriptingbase/updateSitNum0302.pas
+drwxrwxrwx   0        0        0        0 2023-03-06 02:14:23.702102 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/
+-rw-rw-rw-   0        0        0     2735 2023-03-06 02:14:23.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      903 2023-03-06 02:14:23.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-06 02:14:23.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-27 09:40:41.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       73 2023-03-06 02:14:23.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-03-06 02:14:23.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/top_level.txt
```

### Comparing `PyAltiumRunTop-0.2.4.3/LICENSE` & `PyAltiumRunTop-0.2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.3/PKG-INFO` & `PyAltiumRunTop-0.2.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAltiumRunTop
-Version: 0.2.4.3
+Version: 0.2.4.4
 Summary: A library that can run scripts in altium designer
 Home-page: https://github.com/wqh0109663/PyAltiumRun
 Author: Dylan Gybels,wqh0109663
 Author-email: dylangybels@gmail.com,wqh0109663@gmail.com
 License: MIT
 Keywords: Altium,Scripting,Runner
 Platform: win32
```

### Comparing `PyAltiumRunTop-0.2.4.3/README.md` & `PyAltiumRunTop-0.2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.3/pyproject.toml` & `PyAltiumRunTop-0.2.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.3/setup.cfg` & `PyAltiumRunTop-0.2.4.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 7941 6c74 6975 6d52 756e 546f   = PyAltiumRunTo
 00000020: 700d 0a76 6572 7369 6f6e 203d 2030 2e32  p..version = 0.2
-00000030: 2e34 2e33 0d0a 6465 7363 7269 7074 696f  .4.3..descriptio
+00000030: 2e34 2e34 0d0a 6465 7363 7269 7074 696f  .4.4..descriptio
 00000040: 6e20 3d20 4120 6c69 6272 6172 7920 7468  n = A library th
 00000050: 6174 2063 616e 2072 756e 2073 6372 6970  at can run scrip
 00000060: 7473 2069 6e20 616c 7469 756d 2064 6573  ts in altium des
 00000070: 6967 6e65 720d 0a6c 6f6e 675f 6465 7363  igner..long_desc
 00000080: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000090: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
 000000a0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
```

### Comparing `PyAltiumRunTop-0.2.4.3/src/PyAltiumRun.egg-info/PKG-INFO` & `PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.3/src/PyAltiumRun.egg-info/SOURCES.txt` & `PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop/AltiumRun.py` & `PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/AltiumRun.py`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop/helpers/AltiumHelper.py` & `PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/helpers/AltiumHelper.py`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop/scriptingbase/logger.pas` & `PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/scriptingbase/logger.pas`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop/scriptingbase/updateSitNum0302.pas` & `PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/scriptingbase/updateSitNum0302.pas`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 //          ShowMessage(ObjectList[I]);
           FlagStr := 'T';
           currentTime := Now;
           Splitted1 := TStringList.Create;
           Splitted1.LineBreak := '!!!!!';
           Splitted1.Text := ObjectList[I];
 //      Model := AComponent.AddPart;
-          for G1 := 1 to Splitted1.Count - 1 do
+          for G1 := 0 to Splitted1.Count - 1 do
           begin
             if G1 = 0 Then
             begin
               Sdy := Sdy+ 'Designator:'+Splitted1[G1]+' ';
             end;
             if G1 = 1 Then
             begin
```

### Comparing `PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop.egg-info/PKG-INFO` & `PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAltiumRunTop
-Version: 0.2.4.3
+Version: 0.2.4.4
 Summary: A library that can run scripts in altium designer
 Home-page: https://github.com/wqh0109663/PyAltiumRun
 Author: Dylan Gybels,wqh0109663
 Author-email: dylangybels@gmail.com,wqh0109663@gmail.com
 License: MIT
 Keywords: Altium,Scripting,Runner
 Platform: win32
```

### Comparing `PyAltiumRunTop-0.2.4.3/src/PyAltiumRunTop.egg-info/SOURCES.txt` & `PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

