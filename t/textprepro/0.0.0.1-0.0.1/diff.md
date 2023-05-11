# Comparing `tmp/textprepro-0.0.0.1.tar.gz` & `tmp/textprepro-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textprepro-0.0.0.1.tar", last modified: Thu May 11 08:39:52 2023, max compression
+gzip compressed data, was "textprepro-0.0.1.tar", last modified: Thu May 11 11:39:16 2023, max compression
```

## Comparing `textprepro-0.0.0.1.tar` & `textprepro-0.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 08:39:52.624005 textprepro-0.0.0.1/
--rw-rw-rw-   0        0        0     1101 2023-05-09 15:11:42.000000 textprepro-0.0.0.1/LICENSE
--rw-rw-rw-   0        0        0       17 2023-05-09 08:41:05.000000 textprepro-0.0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0    17223 2023-05-11 08:39:52.622006 textprepro-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    16042 2023-05-11 07:37:38.000000 textprepro-0.0.0.1/README.md
--rw-rw-rw-   0        0        0     1479 2023-05-11 08:38:34.000000 textprepro-0.0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 08:39:52.624005 textprepro-0.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-05-09 07:05:32.000000 textprepro-0.0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:39:52.440381 textprepro-0.0.0.1/tests/
--rw-rw-rw-   0        0        0     7368 2023-05-11 07:33:54.000000 textprepro-0.0.0.1/tests/test_textprepro.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:39:52.521580 textprepro-0.0.0.1/textprepro/
--rw-rw-rw-   0        0        0       80 2023-05-09 02:31:24.000000 textprepro-0.0.0.1/textprepro/__init__.py
--rw-rw-rw-   0        0        0    22975 2023-05-11 07:27:43.000000 textprepro-0.0.0.1/textprepro/preprocess.py
--rw-rw-rw-   0        0        0     7491 2023-05-09 11:00:09.000000 textprepro-0.0.0.1/textprepro/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:39:52.609590 textprepro-0.0.0.1/textprepro.egg-info/
--rw-rw-rw-   0        0        0    17223 2023-05-11 08:39:52.000000 textprepro-0.0.0.1/textprepro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-05-11 08:39:52.000000 textprepro-0.0.0.1/textprepro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 08:39:52.000000 textprepro-0.0.0.1/textprepro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-05-11 08:39:52.000000 textprepro-0.0.0.1/textprepro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-11 08:39:52.000000 textprepro-0.0.0.1/textprepro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 11:39:16.146659 textprepro-0.0.1/
+-rw-rw-rw-   0        0        0     1101 2023-05-09 15:11:42.000000 textprepro-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0       17 2023-05-09 08:41:05.000000 textprepro-0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    17225 2023-05-11 11:39:16.144696 textprepro-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    16046 2023-05-11 09:17:30.000000 textprepro-0.0.1/README.md
+-rw-rw-rw-   0        0        0     1477 2023-05-11 11:30:26.000000 textprepro-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 11:39:16.146659 textprepro-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-05-09 07:05:32.000000 textprepro-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:39:15.734590 textprepro-0.0.1/tests/
+-rw-rw-rw-   0        0        0     7437 2023-05-11 09:38:22.000000 textprepro-0.0.1/tests/test_textprepro.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:39:16.095971 textprepro-0.0.1/textprepro/
+-rw-rw-rw-   0        0        0       80 2023-05-09 02:31:24.000000 textprepro-0.0.1/textprepro/__init__.py
+-rw-rw-rw-   0        0        0    22975 2023-05-11 07:27:43.000000 textprepro-0.0.1/textprepro/preprocess.py
+-rw-rw-rw-   0        0        0     7491 2023-05-09 11:00:09.000000 textprepro-0.0.1/textprepro/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:39:16.140698 textprepro-0.0.1/textprepro.egg-info/
+-rw-rw-rw-   0        0        0    17225 2023-05-11 11:39:15.000000 textprepro-0.0.1/textprepro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-05-11 11:39:15.000000 textprepro-0.0.1/textprepro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 11:39:15.000000 textprepro-0.0.1/textprepro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-05-11 11:39:15.000000 textprepro-0.0.1/textprepro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-11 11:39:15.000000 textprepro-0.0.1/textprepro.egg-info/top_level.txt
```

### Comparing `textprepro-0.0.0.1/LICENSE` & `textprepro-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `textprepro-0.0.0.1/PKG-INFO` & `textprepro-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textprepro
-Version: 0.0.0.1
+Version: 0.0.1
 Summary: Everything Everyway All At Once Text Preprocessing.
 Author-email: Umaporn Padungkiatwattana <umaploy@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/umapornp/textprepro
 Project-URL: Documentation, https://github.com/umapornp/textprepro/blob/master/README.md
 Project-URL: Source, https://github.com/umapornp/textprepro
 Keywords: text preprocessing,text mining,NLP,Natural Language Processing
@@ -30,15 +30,15 @@
 
 <p align="center">
     <a href="https://pypi.org/project/textprepro">
         <img src="https://img.shields.io/pypi/v/textprepro.svg?logo=pypi&logoColor=white"
             alt="PyPI">
     </a>
     <a href="https://pypi.org/project/textprepro">
-        <img src="https://img.shields.io/pypi/pyversions/textprepro?logo=python&logoColor=white"
+        <img src="https://img.shields.io/pypi/pyversions/textprepro.svg?logo=python&logoColor=white"
             alt="Python">
     </a>    
     <a href="https://codecov.io/gh/umapornp/textprepro">
         <img src="https://img.shields.io/codecov/c/github/umapornp/textprepro?logo=codecov"
             alt="Codecov">
     </a>    
     <a href="https://github.com/umapornp/textprepro/blob/master/LICENSE">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: textprepro Version: 0.0.0.1 Summary: Everything
+Metadata-Version: 2.1 Name: textprepro Version: 0.0.1 Summary: Everything
 Everyway All At Once Text Preprocessing. Author-email: Umaporn
 Padungkiatwattana
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/umapornp/
 textprepro Project-URL: Documentation, https://github.com/umapornp/textprepro/
 blob/master/README.md Project-URL: Source, https://github.com/umapornp/
 textprepro Keywords: text preprocessing,text mining,NLP,Natural Language
 Processing Classifier: Intended Audience :: Developers Classifier: Intended
```

### Comparing `textprepro-0.0.0.1/README.md` & `textprepro-0.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 <p align="center">
     <a href="https://pypi.org/project/textprepro">
         <img src="https://img.shields.io/pypi/v/textprepro.svg?logo=pypi&logoColor=white"
             alt="PyPI">
     </a>
     <a href="https://pypi.org/project/textprepro">
-        <img src="https://img.shields.io/pypi/pyversions/textprepro?logo=python&logoColor=white"
+        <img src="https://img.shields.io/pypi/pyversions/textprepro.svg?logo=python&logoColor=white"
             alt="Python">
     </a>    
     <a href="https://codecov.io/gh/umapornp/textprepro">
         <img src="https://img.shields.io/codecov/c/github/umapornp/textprepro?logo=codecov"
             alt="Codecov">
     </a>    
     <a href="https://github.com/umapornp/textprepro/blob/master/LICENSE">
```

### Comparing `textprepro-0.0.0.1/pyproject.toml` & `textprepro-0.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "textprepro"
-version = "0.0.0.1"
+version = "0.0.1"
 description = "Everything Everyway All At Once Text Preprocessing."
 readme = "README.md"
 authors = [{name = "Umaporn Padungkiatwattana", email = "umaploy@gmail.com"}]
 license = {text = "MIT"}
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
```

### Comparing `textprepro-0.0.0.1/tests/test_textprepro.py` & `textprepro-0.0.1/tests/test_textprepro.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import textprepro as pre
+import unittest
 
 from collections import Counter
-from unittest import TestCase, mock
+from unittest import mock
 
 
-class Test_Preprocess(TestCase):
+class Test_Preprocess(unittest.TestCase):
 
     def test_tokenize(self):
         self.assertEqual(pre.tokenize("hello world @user #hashtag", "tweet"), list(["hello", "world", "@user", "#hashtag"]))
         self.assertEqual(pre.tokenize("hello world @user #hashtag", "word"), list(["hello", "world", "@", "user", "#", "hashtag"]))
         
         with self.assertRaises(ValueError):
             pre.tokenize("hello world @user #hashtag", "")
@@ -184,8 +185,12 @@
     
     
     def test_preprocess_text(self):
         self.assertEqual(pre.preprocess_text("hello world @user #hashtag"), "hello world hashtag")
     
         
     def test_preprocess_document(self):
-        self.assertEqual(pre.preprocess_document(["hello world @user", "world hello @user"]), ["hello world", "world hello"])
+        self.assertEqual(pre.preprocess_document(["hello world @user", "world hello @user"]), ["hello world", "world hello"])
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `textprepro-0.0.0.1/textprepro/preprocess.py` & `textprepro-0.0.1/textprepro/preprocess.py`

 * *Files identical despite different names*

### Comparing `textprepro-0.0.0.1/textprepro/utils.py` & `textprepro-0.0.1/textprepro/utils.py`

 * *Files identical despite different names*

### Comparing `textprepro-0.0.0.1/textprepro.egg-info/PKG-INFO` & `textprepro-0.0.1/textprepro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textprepro
-Version: 0.0.0.1
+Version: 0.0.1
 Summary: Everything Everyway All At Once Text Preprocessing.
 Author-email: Umaporn Padungkiatwattana <umaploy@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/umapornp/textprepro
 Project-URL: Documentation, https://github.com/umapornp/textprepro/blob/master/README.md
 Project-URL: Source, https://github.com/umapornp/textprepro
 Keywords: text preprocessing,text mining,NLP,Natural Language Processing
@@ -30,15 +30,15 @@
 
 <p align="center">
     <a href="https://pypi.org/project/textprepro">
         <img src="https://img.shields.io/pypi/v/textprepro.svg?logo=pypi&logoColor=white"
             alt="PyPI">
     </a>
     <a href="https://pypi.org/project/textprepro">
-        <img src="https://img.shields.io/pypi/pyversions/textprepro?logo=python&logoColor=white"
+        <img src="https://img.shields.io/pypi/pyversions/textprepro.svg?logo=python&logoColor=white"
             alt="Python">
     </a>    
     <a href="https://codecov.io/gh/umapornp/textprepro">
         <img src="https://img.shields.io/codecov/c/github/umapornp/textprepro?logo=codecov"
             alt="Codecov">
     </a>    
     <a href="https://github.com/umapornp/textprepro/blob/master/LICENSE">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: textprepro Version: 0.0.0.1 Summary: Everything
+Metadata-Version: 2.1 Name: textprepro Version: 0.0.1 Summary: Everything
 Everyway All At Once Text Preprocessing. Author-email: Umaporn
 Padungkiatwattana
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/umapornp/
 textprepro Project-URL: Documentation, https://github.com/umapornp/textprepro/
 blob/master/README.md Project-URL: Source, https://github.com/umapornp/
 textprepro Keywords: text preprocessing,text mining,NLP,Natural Language
 Processing Classifier: Intended Audience :: Developers Classifier: Intended
```

