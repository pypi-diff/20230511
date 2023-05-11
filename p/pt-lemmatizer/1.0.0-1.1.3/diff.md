# Comparing `tmp/pt_lemmatizer-1.0.0.tar.gz` & `tmp/pt_lemmatizer-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pt_lemmatizer-1.0.0.tar", last modified: Thu May 11 20:56:34 2023, max compression
+gzip compressed data, was "pt_lemmatizer-1.1.3.tar", last modified: Thu May 11 21:01:43 2023, max compression
```

## Comparing `pt_lemmatizer-1.0.0.tar` & `pt_lemmatizer-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 naomilago  (1000) naomilago  (1000)        0 2023-05-11 20:56:34.423430 pt_lemmatizer-1.0.0/
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)     1086 2023-05-11 02:37:11.000000 pt_lemmatizer-1.0.0/LICENSE
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)     2021 2023-05-11 20:56:34.423430 pt_lemmatizer-1.0.0/PKG-INFO
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)      718 2023-05-11 14:35:44.000000 pt_lemmatizer-1.0.0/README.md
-drwxr-xr-x   0 naomilago  (1000) naomilago  (1000)        0 2023-05-11 20:56:34.423430 pt_lemmatizer-1.0.0/pt_lemmatizer/
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)       20 2023-05-11 15:08:35.000000 pt_lemmatizer-1.0.0/pt_lemmatizer/__init__.py
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)     1709 2023-05-11 20:51:05.000000 pt_lemmatizer-1.0.0/pt_lemmatizer/lemma.py
-drwxr-xr-x   0 naomilago  (1000) naomilago  (1000)        0 2023-05-11 20:56:34.423430 pt_lemmatizer-1.0.0/pt_lemmatizer.egg-info/
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)     2021 2023-05-11 20:56:34.000000 pt_lemmatizer-1.0.0/pt_lemmatizer.egg-info/PKG-INFO
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)      259 2023-05-11 20:56:34.000000 pt_lemmatizer-1.0.0/pt_lemmatizer.egg-info/SOURCES.txt
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)        1 2023-05-11 20:56:34.000000 pt_lemmatizer-1.0.0/pt_lemmatizer.egg-info/dependency_links.txt
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)       10 2023-05-11 20:56:34.000000 pt_lemmatizer-1.0.0/pt_lemmatizer.egg-info/requires.txt
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)       14 2023-05-11 20:56:34.000000 pt_lemmatizer-1.0.0/pt_lemmatizer.egg-info/top_level.txt
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)       38 2023-05-11 20:56:34.423430 pt_lemmatizer-1.0.0/setup.cfg
--rw-r--r--   0 naomilago  (1000) naomilago  (1000)     2288 2023-05-11 20:56:16.000000 pt_lemmatizer-1.0.0/setup.py
+drwxr-xr-x   0 naomilago  (1000) naomilago  (1000)        0 2023-05-11 21:01:43.863786 pt_lemmatizer-1.1.3/
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)     1086 2023-05-11 02:37:11.000000 pt_lemmatizer-1.1.3/LICENSE
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)     2021 2023-05-11 21:01:43.863786 pt_lemmatizer-1.1.3/PKG-INFO
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)      718 2023-05-11 14:35:44.000000 pt_lemmatizer-1.1.3/README.md
+drwxr-xr-x   0 naomilago  (1000) naomilago  (1000)        0 2023-05-11 21:01:43.863786 pt_lemmatizer-1.1.3/pt_lemmatizer/
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)       20 2023-05-11 15:08:35.000000 pt_lemmatizer-1.1.3/pt_lemmatizer/__init__.py
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)     1625 2023-05-11 21:00:59.000000 pt_lemmatizer-1.1.3/pt_lemmatizer/lemma.py
+drwxr-xr-x   0 naomilago  (1000) naomilago  (1000)        0 2023-05-11 21:01:43.863786 pt_lemmatizer-1.1.3/pt_lemmatizer.egg-info/
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)     2021 2023-05-11 21:01:43.000000 pt_lemmatizer-1.1.3/pt_lemmatizer.egg-info/PKG-INFO
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)      259 2023-05-11 21:01:43.000000 pt_lemmatizer-1.1.3/pt_lemmatizer.egg-info/SOURCES.txt
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)        1 2023-05-11 21:01:43.000000 pt_lemmatizer-1.1.3/pt_lemmatizer.egg-info/dependency_links.txt
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)       10 2023-05-11 21:01:43.000000 pt_lemmatizer-1.1.3/pt_lemmatizer.egg-info/requires.txt
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)       14 2023-05-11 21:01:43.000000 pt_lemmatizer-1.1.3/pt_lemmatizer.egg-info/top_level.txt
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)       38 2023-05-11 21:01:43.863786 pt_lemmatizer-1.1.3/setup.cfg
+-rw-r--r--   0 naomilago  (1000) naomilago  (1000)     2288 2023-05-11 21:01:23.000000 pt_lemmatizer-1.1.3/setup.py
```

### Comparing `pt_lemmatizer-1.0.0/LICENSE` & `pt_lemmatizer-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pt_lemmatizer-1.0.0/PKG-INFO` & `pt_lemmatizer-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pt_lemmatizer
-Version: 1.0.0
+Version: 1.1.3
 Summary: A NLP package for Portuguese Lemmatization.
 Home-page: UNKNOWN
 Author: Naomi Lago
 Author-email: <info@naomilago.com>
 License: UNKNOWN
 Keywords: python,portuguese,lemmatizer,nlp
 Platform: UNKNOWN
```

### Comparing `pt_lemmatizer-1.0.0/README.md` & `pt_lemmatizer-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pt_lemmatizer-1.0.0/pt_lemmatizer/lemma.py` & `pt_lemmatizer-1.1.3/pt_lemmatizer/lemma.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import unidecode
 import pickle
 import os
 
 class Lemmatizer():
     def __init__(self):
-        if (os.path.exists('pt_lemmatizer/lemmatizer.pickle')):
-            print('loading lemmatizer dict (pt_lemmatizer/lemmatizer.pickle)')
+        if (os.path.exists('lemmatizer.pickle')):
+            print('loading lemmatizer dict (lemmatizer.pickle)')
             self.lemmatizer_dict = self.load_lemmatizer_dict()
         else:
-            print('generating lemmatizer dict (pt_lemmatizer/lemmatizer.pickle)')
+            print('generating lemmatizer dict (lemmatizer.pickle)')
             self.lemmatizer_dict = self.generate_lemmatizer_dict()
 
     def generate_lemmatizer_dict(self):
-        file_name = 'pt_lemmatizer/data/lemmatization-pt.txt'
+        file_name = 'data/lemmatization-pt.txt'
 
         with open(file_name, encoding="utf-8") as f:
             lemmatizer_dict = {}
             for l in list(f)[1:]:
                 words = l.rstrip().split("\t")
                 word = unidecode.unidecode(words[0]).strip().lower()
                 infl = unidecode.unidecode(words[1]).strip().lower()
@@ -26,19 +26,19 @@
                     else:
                         lemmatizer_dict[word].append(infl)
         inverse_lemmatizer_dict = {}
         for k, v in lemmatizer_dict.items():
             for w in v:
                 inverse_lemmatizer_dict[w] = k
 
-        pickle.dump(inverse_lemmatizer_dict, open("pt_lemmatizer/lemmatizer.pickle", "wb"))
+        pickle.dump(inverse_lemmatizer_dict, open("lemmatizer.pickle", "wb"))
         return inverse_lemmatizer_dict
 
     def load_lemmatizer_dict(self):
-        return pickle.load(open("pt_lemmatizer/lemmatizer.pickle", "rb"))
+        return pickle.load(open("lemmatizer.pickle", "rb"))
 
     def lemmatize(self, word):
         return self.lemmatizer_dict.get(word, word)
 
 if __name__ == '__main__':
     l = Lemmatizer()
     w = 'apagou'
```

### Comparing `pt_lemmatizer-1.0.0/pt_lemmatizer.egg-info/PKG-INFO` & `pt_lemmatizer-1.1.3/pt_lemmatizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pt-lemmatizer
-Version: 1.0.0
+Version: 1.1.3
 Summary: A NLP package for Portuguese Lemmatization.
 Home-page: UNKNOWN
 Author: Naomi Lago
 Author-email: <info@naomilago.com>
 License: UNKNOWN
 Keywords: python,portuguese,lemmatizer,nlp
 Platform: UNKNOWN
```

### Comparing `pt_lemmatizer-1.0.0/setup.py` & `pt_lemmatizer-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 l = Lemmatizer()
 l.lemmatize('apagou')  #all words must be unidecoded and lowercased
 >> 'apagar'
 l.lemmatize('nasalaram')
 >> 'nasalar'
 
 '''
-VERSION = '1.0.0' 
+VERSION = '1.1.3' 
 
 # Setting up 
 setup( 
     name="pt_lemmatizer",   
     version=VERSION, 
     author="Naomi Lago", 
     author_email="<info@naomilago.com>",
```

