# Comparing `tmp/arabic2latin-1.1.2.tar.gz` & `tmp/arabic2latin-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabic2latin-1.1.2.tar", last modified: Sun May  7 20:25:09 2023, max compression
+gzip compressed data, was "arabic2latin-1.1.3.tar", last modified: Thu May 11 10:51:16 2023, max compression
```

## Comparing `arabic2latin-1.1.2.tar` & `arabic2latin-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 20:25:09.930472 arabic2latin-1.1.2/
--rw-rw-rw-   0        0        0     1083 2023-04-12 10:51:38.000000 arabic2latin-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     3219 2023-05-07 20:25:09.930472 arabic2latin-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1203 2023-05-07 20:22:58.000000 arabic2latin-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 20:25:09.905074 arabic2latin-1.1.2/arabic2latin/
--rw-rw-rw-   0        0        0       55 2023-04-10 05:39:27.000000 arabic2latin-1.1.2/arabic2latin/__init__.py
--rw-rw-rw-   0        0        0     3758 2023-05-07 20:20:43.000000 arabic2latin-1.1.2/arabic2latin/arabic2latin.py
--rw-rw-rw-   0        0        0       23 2023-05-07 20:20:43.000000 arabic2latin-1.1.2/arabic2latin/version.py
-drwxrwxrwx   0        0        0        0 2023-05-07 20:25:09.930472 arabic2latin-1.1.2/arabic2latin.egg-info/
--rw-rw-rw-   0        0        0     3219 2023-05-07 20:25:09.000000 arabic2latin-1.1.2/arabic2latin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-05-07 20:25:09.000000 arabic2latin-1.1.2/arabic2latin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 20:25:09.000000 arabic2latin-1.1.2/arabic2latin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-07 20:25:09.000000 arabic2latin-1.1.2/arabic2latin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      781 2023-05-07 20:20:43.000000 arabic2latin-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 20:25:09.930472 arabic2latin-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      563 2023-04-12 10:59:40.000000 arabic2latin-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:51:16.325616 arabic2latin-1.1.3/
+-rw-rw-rw-   0        0        0     1083 2023-04-12 10:51:38.000000 arabic2latin-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3219 2023-05-11 10:51:16.325616 arabic2latin-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1203 2023-05-07 20:26:17.000000 arabic2latin-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 10:51:16.294223 arabic2latin-1.1.3/arabic2latin/
+-rw-rw-rw-   0        0        0       55 2023-04-10 05:39:27.000000 arabic2latin-1.1.3/arabic2latin/__init__.py
+-rw-rw-rw-   0        0        0     3765 2023-05-09 12:22:36.000000 arabic2latin-1.1.3/arabic2latin/arabic2latin.py
+-rw-rw-rw-   0        0        0       23 2023-05-09 12:22:36.000000 arabic2latin-1.1.3/arabic2latin/version.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:51:16.325616 arabic2latin-1.1.3/arabic2latin.egg-info/
+-rw-rw-rw-   0        0        0     3219 2023-05-11 10:51:16.000000 arabic2latin-1.1.3/arabic2latin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-05-11 10:51:16.000000 arabic2latin-1.1.3/arabic2latin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 10:51:16.000000 arabic2latin-1.1.3/arabic2latin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-11 10:51:16.000000 arabic2latin-1.1.3/arabic2latin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      781 2023-05-09 12:22:36.000000 arabic2latin-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 10:51:16.325616 arabic2latin-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      563 2023-04-12 10:59:40.000000 arabic2latin-1.1.3/setup.py
```

### Comparing `arabic2latin-1.1.2/LICENSE` & `arabic2latin-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arabic2latin-1.1.2/PKG-INFO` & `arabic2latin-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabic2latin
-Version: 1.1.2
+Version: 1.1.3
 Summary: Convert Arabic characters to their Latin (English) homophones.
 Author: rexa222
 Author-email: rexa222@outlook.com
 License: MIT License
         
         Copyright (c) 2023 rexa222
```

### Comparing `arabic2latin-1.1.2/README.md` & `arabic2latin-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `arabic2latin-1.1.2/arabic2latin/arabic2latin.py` & `arabic2latin-1.1.3/arabic2latin/arabic2latin.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
                 else:
                     result += MAPPING[char]
 
             elif char == "ه" and (c == n-1 or (c != n-1 and text[c+1] == " ")):
                 result += "ah"
 
-            else:
+            elif result:
                 if result[-1] not in VOWELS and MAPPING[char][:1] not in VOWELS and result[-3:] not in " al" and MAPPING[char] != "y":
                     if not no_vowel:
                         result += "a"
                     else:
                         no_vowel = False
 
                 # prevent occurrence of a letter for more than two times
```

### Comparing `arabic2latin-1.1.2/arabic2latin.egg-info/PKG-INFO` & `arabic2latin-1.1.3/arabic2latin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabic2latin
-Version: 1.1.2
+Version: 1.1.3
 Summary: Convert Arabic characters to their Latin (English) homophones.
 Author: rexa222
 Author-email: rexa222@outlook.com
 License: MIT License
         
         Copyright (c) 2023 rexa222
```

### Comparing `arabic2latin-1.1.2/pyproject.toml` & `arabic2latin-1.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arabic2latin"
-version = "1.1.2"
+version = "1.1.3"
 description = "Convert Arabic characters to their Latin (English) homophones."
 readme = "README.md"
 requires-python = ">=3.6"
 license= {file = "LICENSE"}
 keywords=["arabic", "homophone", "arabic to english", "arabic to latin"]
 authors = [
   {email = "rexa222@outlook.com"},
```

### Comparing `arabic2latin-1.1.2/setup.py` & `arabic2latin-1.1.3/setup.py`

 * *Files identical despite different names*

