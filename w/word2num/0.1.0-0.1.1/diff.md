# Comparing `tmp/word2num-0.1.0.tar.gz` & `tmp/word2num-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/bryson/projects/word2num/dist/.tmp-wyik2gwk/word2num-0.1.0.tar", last modified: Thu May 11 00:21:50 2023, max compression
+gzip compressed data, was "/Users/bryson/projects/word2num/dist/.tmp-sr23xrnu/word2num-0.1.1.tar", last modified: Thu May 11 00:29:31 2023, max compression
```

## Comparing `word2num-0.1.0.tar` & `word2num-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 bryson     (501) staff       (20)        0 2023-05-11 00:21:50.000000 word2num-0.1.0/
--rw-r--r--   0 bryson     (501) staff       (20)     1069 2023-05-11 00:06:30.000000 word2num-0.1.0/LICENSE.txt
--rw-r--r--   0 bryson     (501) staff       (20)      456 2023-05-11 00:21:50.000000 word2num-0.1.0/PKG-INFO
--rw-r--r--   0 bryson     (501) staff       (20)     3388 2023-05-11 00:17:28.000000 word2num-0.1.0/README.md
--rw-r--r--   0 bryson     (501) staff       (20)       38 2023-05-11 00:21:50.000000 word2num-0.1.0/setup.cfg
--rw-r--r--   0 bryson     (501) staff       (20)      647 2023-05-11 00:06:30.000000 word2num-0.1.0/setup.py
-drwxr-xr-x   0 bryson     (501) staff       (20)        0 2023-05-11 00:21:50.000000 word2num-0.1.0/tests/
--rw-r--r--   0 bryson     (501) staff       (20)     3111 2023-05-11 00:06:30.000000 word2num-0.1.0/tests/test_word2num.py
-drwxr-xr-x   0 bryson     (501) staff       (20)        0 2023-05-11 00:21:50.000000 word2num-0.1.0/word2num/
--rw-r--r--   0 bryson     (501) staff       (20)       76 2023-05-11 00:06:30.000000 word2num-0.1.0/word2num/__init__.py
-drwxr-xr-x   0 bryson     (501) staff       (20)        0 2023-05-11 00:21:50.000000 word2num-0.1.0/word2num/languages/
--rw-r--r--   0 bryson     (501) staff       (20)        0 2023-05-11 00:06:30.000000 word2num-0.1.0/word2num/languages/__init__.py
-drwxr-xr-x   0 bryson     (501) staff       (20)        0 2023-05-11 00:21:50.000000 word2num-0.1.0/word2num/languages/en/
--rw-r--r--   0 bryson     (501) staff       (20)       43 2023-05-11 00:06:30.000000 word2num-0.1.0/word2num/languages/en/__init__.py
--rw-r--r--   0 bryson     (501) staff       (20)     7563 2023-05-11 00:06:30.000000 word2num-0.1.0/word2num/languages/en/parser.py
--rw-r--r--   0 bryson     (501) staff       (20)     1692 2023-05-11 00:06:30.000000 word2num-0.1.0/word2num/languages/en/vocabulary.py
--rw-r--r--   0 bryson     (501) staff       (20)     6962 2023-05-11 00:06:30.000000 word2num-0.1.0/word2num/languages/en/word_matcher.py
--rw-r--r--   0 bryson     (501) staff       (20)      968 2023-05-11 00:06:30.000000 word2num-0.1.0/word2num/number_word_parser.py
--rw-r--r--   0 bryson     (501) staff       (20)     2250 2023-05-11 00:06:30.000000 word2num-0.1.0/word2num/word2num.py
-drwxr-xr-x   0 bryson     (501) staff       (20)        0 2023-05-11 00:21:50.000000 word2num-0.1.0/word2num.egg-info/
--rw-r--r--   0 bryson     (501) staff       (20)      456 2023-05-11 00:21:50.000000 word2num-0.1.0/word2num.egg-info/PKG-INFO
--rw-r--r--   0 bryson     (501) staff       (20)      456 2023-05-11 00:21:50.000000 word2num-0.1.0/word2num.egg-info/SOURCES.txt
--rw-r--r--   0 bryson     (501) staff       (20)        1 2023-05-11 00:21:50.000000 word2num-0.1.0/word2num.egg-info/dependency_links.txt
--rw-r--r--   0 bryson     (501) staff       (20)       43 2023-05-11 00:21:50.000000 word2num-0.1.0/word2num.egg-info/requires.txt
--rw-r--r--   0 bryson     (501) staff       (20)        9 2023-05-11 00:21:50.000000 word2num-0.1.0/word2num.egg-info/top_level.txt
+drwxr-xr-x   0 bryson     (501) staff       (20)        0 2023-05-11 00:29:31.000000 word2num-0.1.1/
+-rw-r--r--   0 bryson     (501) staff       (20)     1069 2023-05-11 00:06:30.000000 word2num-0.1.1/LICENSE.txt
+-rw-r--r--   0 bryson     (501) staff       (20)     3885 2023-05-11 00:29:31.000000 word2num-0.1.1/PKG-INFO
+-rw-r--r--   0 bryson     (501) staff       (20)     3388 2023-05-11 00:17:28.000000 word2num-0.1.1/README.md
+-rw-r--r--   0 bryson     (501) staff       (20)       38 2023-05-11 00:29:31.000000 word2num-0.1.1/setup.cfg
+-rw-r--r--   0 bryson     (501) staff       (20)      822 2023-05-11 00:29:13.000000 word2num-0.1.1/setup.py
+drwxr-xr-x   0 bryson     (501) staff       (20)        0 2023-05-11 00:29:31.000000 word2num-0.1.1/tests/
+-rw-r--r--   0 bryson     (501) staff       (20)     3111 2023-05-11 00:06:30.000000 word2num-0.1.1/tests/test_word2num.py
+drwxr-xr-x   0 bryson     (501) staff       (20)        0 2023-05-11 00:29:31.000000 word2num-0.1.1/word2num/
+-rw-r--r--   0 bryson     (501) staff       (20)       76 2023-05-11 00:06:30.000000 word2num-0.1.1/word2num/__init__.py
+drwxr-xr-x   0 bryson     (501) staff       (20)        0 2023-05-11 00:29:31.000000 word2num-0.1.1/word2num/languages/
+-rw-r--r--   0 bryson     (501) staff       (20)        0 2023-05-11 00:06:30.000000 word2num-0.1.1/word2num/languages/__init__.py
+drwxr-xr-x   0 bryson     (501) staff       (20)        0 2023-05-11 00:29:31.000000 word2num-0.1.1/word2num/languages/en/
+-rw-r--r--   0 bryson     (501) staff       (20)       43 2023-05-11 00:06:30.000000 word2num-0.1.1/word2num/languages/en/__init__.py
+-rw-r--r--   0 bryson     (501) staff       (20)     7563 2023-05-11 00:06:30.000000 word2num-0.1.1/word2num/languages/en/parser.py
+-rw-r--r--   0 bryson     (501) staff       (20)     1692 2023-05-11 00:06:30.000000 word2num-0.1.1/word2num/languages/en/vocabulary.py
+-rw-r--r--   0 bryson     (501) staff       (20)     6962 2023-05-11 00:06:30.000000 word2num-0.1.1/word2num/languages/en/word_matcher.py
+-rw-r--r--   0 bryson     (501) staff       (20)      968 2023-05-11 00:06:30.000000 word2num-0.1.1/word2num/number_word_parser.py
+-rw-r--r--   0 bryson     (501) staff       (20)     2250 2023-05-11 00:06:30.000000 word2num-0.1.1/word2num/word2num.py
+drwxr-xr-x   0 bryson     (501) staff       (20)        0 2023-05-11 00:29:31.000000 word2num-0.1.1/word2num.egg-info/
+-rw-r--r--   0 bryson     (501) staff       (20)     3885 2023-05-11 00:29:31.000000 word2num-0.1.1/word2num.egg-info/PKG-INFO
+-rw-r--r--   0 bryson     (501) staff       (20)      456 2023-05-11 00:29:31.000000 word2num-0.1.1/word2num.egg-info/SOURCES.txt
+-rw-r--r--   0 bryson     (501) staff       (20)        1 2023-05-11 00:29:31.000000 word2num-0.1.1/word2num.egg-info/dependency_links.txt
+-rw-r--r--   0 bryson     (501) staff       (20)       43 2023-05-11 00:29:31.000000 word2num-0.1.1/word2num.egg-info/requires.txt
+-rw-r--r--   0 bryson     (501) staff       (20)        9 2023-05-11 00:29:31.000000 word2num-0.1.1/word2num.egg-info/top_level.txt
```

### Comparing `word2num-0.1.0/LICENSE.txt` & `word2num-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `word2num-0.1.0/README.md` & `word2num-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `word2num-0.1.0/setup.py` & `word2num-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from setuptools import setup, find_packages
 
+with open("README.md", "r", encoding="utf-8") as f:
+    long_description = f.read()
+
 setup(
     name="word2num",
-    version="0.1.0",
+    version="0.1.1",
     author="Bryson Thill",
     author_email="bryson@streamliners.dev",
     description="Converts numbers expressed in words to numerical values.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     url="https://github.com/doppio/word2num",
     license="MIT",
     packages=find_packages(),
     install_requires=[
         "thefuzz>=0.19.0",
         "python-Levenshtein>=0.20.4"
     ],
```

### Comparing `word2num-0.1.0/tests/test_word2num.py` & `word2num-0.1.1/tests/test_word2num.py`

 * *Files identical despite different names*

### Comparing `word2num-0.1.0/word2num/languages/en/parser.py` & `word2num-0.1.1/word2num/languages/en/parser.py`

 * *Files identical despite different names*

### Comparing `word2num-0.1.0/word2num/languages/en/vocabulary.py` & `word2num-0.1.1/word2num/languages/en/vocabulary.py`

 * *Files identical despite different names*

### Comparing `word2num-0.1.0/word2num/languages/en/word_matcher.py` & `word2num-0.1.1/word2num/languages/en/word_matcher.py`

 * *Files identical despite different names*

### Comparing `word2num-0.1.0/word2num/number_word_parser.py` & `word2num-0.1.1/word2num/number_word_parser.py`

 * *Files identical despite different names*

### Comparing `word2num-0.1.0/word2num/word2num.py` & `word2num-0.1.1/word2num/word2num.py`

 * *Files identical despite different names*

