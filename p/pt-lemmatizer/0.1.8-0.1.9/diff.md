# Comparing `tmp/pt_lemmatizer-0.1.8.tar.gz` & `tmp/pt_lemmatizer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pt_lemmatizer-0.1.8.tar", last modified: Thu May 11 14:25:10 2023, max compression
+gzip compressed data, was "pt_lemmatizer-0.1.9.tar", last modified: Thu May 11 14:28:23 2023, max compression
```

## Comparing `pt_lemmatizer-0.1.8.tar` & `pt_lemmatizer-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 naomilago  (1000) naomilago  (1000)        0 2023-05-11 14:25:10.838084 pt_lemmatizer-0.1.8/
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)     1086 2023-05-11 02:37:11.000000 pt_lemmatizer-0.1.8/LICENSE
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)     2015 2023-05-11 14:25:10.838084 pt_lemmatizer-0.1.8/PKG-INFO
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)      718 2023-05-11 14:15:00.000000 pt_lemmatizer-0.1.8/README.md
-drwxr-xr-x   0 naomilago  (1000) naomilago  (1000)        0 2023-05-11 14:25:10.838084 pt_lemmatizer-0.1.8/pt_lemmatizer/
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)       31 2023-05-11 13:44:59.000000 pt_lemmatizer-0.1.8/pt_lemmatizer/__init__.py
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)     1709 2023-05-11 13:43:19.000000 pt_lemmatizer-0.1.8/pt_lemmatizer/pt_lemmatizer.py
-drwxr-xr-x   0 naomilago  (1000) naomilago  (1000)        0 2023-05-11 14:25:10.838084 pt_lemmatizer-0.1.8/pt_lemmatizer.egg-info/
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)     2015 2023-05-11 14:25:10.000000 pt_lemmatizer-0.1.8/pt_lemmatizer.egg-info/PKG-INFO
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)      267 2023-05-11 14:25:10.000000 pt_lemmatizer-0.1.8/pt_lemmatizer.egg-info/SOURCES.txt
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)        1 2023-05-11 14:25:10.000000 pt_lemmatizer-0.1.8/pt_lemmatizer.egg-info/dependency_links.txt
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)       17 2023-05-11 14:25:10.000000 pt_lemmatizer-0.1.8/pt_lemmatizer.egg-info/requires.txt
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)       14 2023-05-11 14:25:10.000000 pt_lemmatizer-0.1.8/pt_lemmatizer.egg-info/top_level.txt
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)       38 2023-05-11 14:25:10.838084 pt_lemmatizer-0.1.8/setup.cfg
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)     2291 2023-05-11 14:24:59.000000 pt_lemmatizer-0.1.8/setup.py
+drwxr-xr-x   0 naomilago  (1000) naomilago  (1000)        0 2023-05-11 14:28:23.913683 pt_lemmatizer-0.1.9/
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)     1086 2023-05-11 02:37:11.000000 pt_lemmatizer-0.1.9/LICENSE
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)     2015 2023-05-11 14:28:23.913683 pt_lemmatizer-0.1.9/PKG-INFO
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)      718 2023-05-11 14:15:00.000000 pt_lemmatizer-0.1.9/README.md
+drwxr-xr-x   0 naomilago  (1000) naomilago  (1000)        0 2023-05-11 14:28:23.913683 pt_lemmatizer-0.1.9/pt_lemmatizer/
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)       36 2023-05-11 14:28:22.000000 pt_lemmatizer-0.1.9/pt_lemmatizer/__init__.py
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)     1709 2023-05-11 13:43:19.000000 pt_lemmatizer-0.1.9/pt_lemmatizer/pt_lemmatizer.py
+drwxr-xr-x   0 naomilago  (1000) naomilago  (1000)        0 2023-05-11 14:28:23.913683 pt_lemmatizer-0.1.9/pt_lemmatizer.egg-info/
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)     2015 2023-05-11 14:28:23.000000 pt_lemmatizer-0.1.9/pt_lemmatizer.egg-info/PKG-INFO
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)      267 2023-05-11 14:28:23.000000 pt_lemmatizer-0.1.9/pt_lemmatizer.egg-info/SOURCES.txt
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)        1 2023-05-11 14:28:23.000000 pt_lemmatizer-0.1.9/pt_lemmatizer.egg-info/dependency_links.txt
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)       10 2023-05-11 14:28:23.000000 pt_lemmatizer-0.1.9/pt_lemmatizer.egg-info/requires.txt
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)       14 2023-05-11 14:28:23.000000 pt_lemmatizer-0.1.9/pt_lemmatizer.egg-info/top_level.txt
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)       38 2023-05-11 14:28:23.913683 pt_lemmatizer-0.1.9/setup.cfg
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)     2281 2023-05-11 14:28:01.000000 pt_lemmatizer-0.1.9/setup.py
```

### Comparing `pt_lemmatizer-0.1.8/LICENSE` & `pt_lemmatizer-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pt_lemmatizer-0.1.8/PKG-INFO` & `pt_lemmatizer-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pt_lemmatizer
-Version: 0.1.8
+Version: 0.1.9
 Summary: A NLP package for Portuguese Lemmatization.
 Home-page: UNKNOWN
 Author: Naomi Lago
 Author-email: <info@naomilago.com>
 License: UNKNOWN
 Keywords: python,portuguese,lemmatizer,nlp
 Platform: UNKNOWN
```

### Comparing `pt_lemmatizer-0.1.8/README.md` & `pt_lemmatizer-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pt_lemmatizer-0.1.8/pt_lemmatizer/pt_lemmatizer.py` & `pt_lemmatizer-0.1.9/pt_lemmatizer/pt_lemmatizer.py`

 * *Files identical despite different names*

### Comparing `pt_lemmatizer-0.1.8/pt_lemmatizer.egg-info/PKG-INFO` & `pt_lemmatizer-0.1.9/pt_lemmatizer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pt-lemmatizer
-Version: 0.1.8
+Version: 0.1.9
 Summary: A NLP package for Portuguese Lemmatization.
 Home-page: UNKNOWN
 Author: Naomi Lago
 Author-email: <info@naomilago.com>
 License: UNKNOWN
 Keywords: python,portuguese,lemmatizer,nlp
 Platform: UNKNOWN
```

### Comparing `pt_lemmatizer-0.1.8/setup.py` & `pt_lemmatizer-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages 
 import codecs 
 import os
 
-VERSION = '0.1.8' 
+VERSION = '0.1.9' 
 DESCRIPTION = 'A NLP package for Portuguese Lemmatization.' 
 LONG_DESCRIPTION = '''
 This NLP package for Portuguese lemmatization is a powerful and advanced tool that can accurately transform words into their base forms or lemmas, taking into account the specific grammatical rules and variations of the Portuguese language. It is designed to handle various types of text input and supports multiple output formats, making it a versatile tool for applications such as information retrieval, machine translation, sentiment analysis, and text classification. Additionally, the package is customizable and user-friendly, allowing users to specify their own dictionaries and rules for lemmatization and providing features for error correction and word sense disambiguation.
 Whether you are a researcher, developer, or linguist working with Portuguese text data, this NLP package can help you save time and improve the accuracy and quality of your analyses. With its advanced algorithms and techniques in NLP, you can trust that this tool will provide high-quality results and make the lemmatization process more efficient.
 
 *_A lemma is a word that stands at the head of a definition in a dictionary._* [Wikipedia](https://simple.wikipedia.org/wiki/Lemma_(linguistics)#:~:text=A%20lemma%20is%20a%20word,you%20find%20in%20the%20dictionary.)
 ### Example
@@ -27,15 +27,15 @@
     version=VERSION, 
     author="Naomi Lago", 
     author_email="<info@naomilago.com>", 
     description=DESCRIPTION, 
     long_description_content_type="text/markdown", 
     long_description=LONG_DESCRIPTION, 
     packages=find_packages(), 
-    install_requires=['unidecode', 'pickle'], 
+    install_requires=['unidecode'], 
     keywords=['python', 'portuguese', 'lemmatizer', 'nlp'], 
     classifiers=[ 
         "Development Status :: 5 - Production/Stable", 
         "Intended Audience :: Developers", 
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

