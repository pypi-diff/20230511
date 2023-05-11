# Comparing `tmp/lmppl-0.2.5.tar.gz` & `tmp/lmppl-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmppl-0.2.5.tar", last modified: Mon May  1 11:09:17 2023, max compression
+gzip compressed data, was "lmppl-0.2.6.tar", last modified: Thu May 11 15:34:30 2023, max compression
```

## Comparing `lmppl-0.2.5.tar` & `lmppl-0.2.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-01 11:09:17.368382 lmppl-0.2.5/
--rw-r--r--   0 asahi      (501) staff       (20)     1064 2023-02-07 11:28:13.000000 lmppl-0.2.5/LICENSE.txt
--rw-r--r--   0 asahi      (501) staff       (20)     5200 2023-05-01 11:09:17.368560 lmppl-0.2.5/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)     4437 2023-02-09 18:23:49.000000 lmppl-0.2.5/README.md
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-01 11:09:17.363180 lmppl-0.2.5/lmppl/
--rw-r--r--   0 asahi      (501) staff       (20)      150 2023-04-05 16:38:19.000000 lmppl-0.2.5/lmppl/__init__.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-01 11:09:17.365769 lmppl-0.2.5/lmppl/lmppl_cl/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2023-02-07 11:25:50.000000 lmppl-0.2.5/lmppl/lmppl_cl/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     2643 2023-05-01 10:57:17.000000 lmppl-0.2.5/lmppl/openai_models.py
--rw-r--r--   0 asahi      (501) staff       (20)     8597 2023-04-01 16:15:20.000000 lmppl-0.2.5/lmppl/ppl_encoder_decoder_lm.py
--rw-r--r--   0 asahi      (501) staff       (20)     6883 2023-03-10 20:47:02.000000 lmppl-0.2.5/lmppl/ppl_mlm.py
--rw-r--r--   0 asahi      (501) staff       (20)     5709 2023-05-01 10:56:55.000000 lmppl-0.2.5/lmppl/ppl_recurrent_lm.py
--rw-r--r--   0 asahi      (501) staff       (20)      227 2023-02-07 13:19:37.000000 lmppl-0.2.5/lmppl/util.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-01 11:09:17.365413 lmppl-0.2.5/lmppl.egg-info/
--rw-r--r--   0 asahi      (501) staff       (20)     5200 2023-05-01 11:09:17.000000 lmppl-0.2.5/lmppl.egg-info/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)      399 2023-05-01 11:09:17.000000 lmppl-0.2.5/lmppl.egg-info/SOURCES.txt
--rw-r--r--   0 asahi      (501) staff       (20)        1 2023-05-01 11:09:17.000000 lmppl-0.2.5/lmppl.egg-info/dependency_links.txt
--rw-r--r--   0 asahi      (501) staff       (20)       79 2023-05-01 11:09:17.000000 lmppl-0.2.5/lmppl.egg-info/requires.txt
--rw-r--r--   0 asahi      (501) staff       (20)        6 2023-05-01 11:09:17.000000 lmppl-0.2.5/lmppl.egg-info/top_level.txt
--rw-r--r--   0 asahi      (501) staff       (20)       38 2023-05-01 11:09:17.369015 lmppl-0.2.5/setup.cfg
--rw-r--r--   0 asahi      (501) staff       (20)     1760 2023-05-01 11:08:58.000000 lmppl-0.2.5/setup.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-01 11:09:17.367475 lmppl-0.2.5/test/
--rw-r--r--   0 asahi      (501) staff       (20)     1249 2023-02-09 19:14:51.000000 lmppl-0.2.5/test/test_analogy.py
--rw-r--r--   0 asahi      (501) staff       (20)     2261 2023-02-12 13:50:45.000000 lmppl-0.2.5/test/test_model_with_simple_input.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-11 15:34:30.673125 lmppl-0.2.6/
+-rw-r--r--   0 asahi      (501) staff       (20)     1064 2023-02-07 11:28:13.000000 lmppl-0.2.6/LICENSE.txt
+-rw-r--r--   0 asahi      (501) staff       (20)     5200 2023-05-11 15:34:30.673284 lmppl-0.2.6/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)     4437 2023-02-09 18:23:49.000000 lmppl-0.2.6/README.md
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-11 15:34:30.668231 lmppl-0.2.6/lmppl/
+-rw-r--r--   0 asahi      (501) staff       (20)      150 2023-04-05 16:38:19.000000 lmppl-0.2.6/lmppl/__init__.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-11 15:34:30.671017 lmppl-0.2.6/lmppl/lmppl_cl/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2023-02-07 11:25:50.000000 lmppl-0.2.6/lmppl/lmppl_cl/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2660 2023-05-11 15:34:08.000000 lmppl-0.2.6/lmppl/openai_models.py
+-rw-r--r--   0 asahi      (501) staff       (20)     8597 2023-04-01 16:15:20.000000 lmppl-0.2.6/lmppl/ppl_encoder_decoder_lm.py
+-rw-r--r--   0 asahi      (501) staff       (20)     6883 2023-03-10 20:47:02.000000 lmppl-0.2.6/lmppl/ppl_mlm.py
+-rw-r--r--   0 asahi      (501) staff       (20)     5709 2023-05-01 10:56:55.000000 lmppl-0.2.6/lmppl/ppl_recurrent_lm.py
+-rw-r--r--   0 asahi      (501) staff       (20)      227 2023-02-07 13:19:37.000000 lmppl-0.2.6/lmppl/util.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-11 15:34:30.670557 lmppl-0.2.6/lmppl.egg-info/
+-rw-r--r--   0 asahi      (501) staff       (20)     5200 2023-05-11 15:34:30.000000 lmppl-0.2.6/lmppl.egg-info/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)      399 2023-05-11 15:34:30.000000 lmppl-0.2.6/lmppl.egg-info/SOURCES.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        1 2023-05-11 15:34:30.000000 lmppl-0.2.6/lmppl.egg-info/dependency_links.txt
+-rw-r--r--   0 asahi      (501) staff       (20)       79 2023-05-11 15:34:30.000000 lmppl-0.2.6/lmppl.egg-info/requires.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        6 2023-05-11 15:34:30.000000 lmppl-0.2.6/lmppl.egg-info/top_level.txt
+-rw-r--r--   0 asahi      (501) staff       (20)       38 2023-05-11 15:34:30.673738 lmppl-0.2.6/setup.cfg
+-rw-r--r--   0 asahi      (501) staff       (20)     1760 2023-05-11 15:34:13.000000 lmppl-0.2.6/setup.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-11 15:34:30.672253 lmppl-0.2.6/test/
+-rw-r--r--   0 asahi      (501) staff       (20)     1249 2023-02-09 19:14:51.000000 lmppl-0.2.6/test/test_analogy.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2261 2023-02-12 13:50:45.000000 lmppl-0.2.6/test/test_model_with_simple_input.py
```

### Comparing `lmppl-0.2.5/LICENSE.txt` & `lmppl-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.5/PKG-INFO` & `lmppl-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lmppl
-Version: 0.2.5
+Version: 0.2.6
 Summary: Calculate perplexity on the text with pre-trained language models.
 Home-page: https://github.com/asahi417/lmppl
 Author: Asahi Ushio
 Author-email: asahi1992ushio@gmail.com
 License: MIT License
-Download-URL: https://github.com/asahi417/lmppl/archive/v0.2.5.tar.gz
+Download-URL: https://github.com/asahi417/lmppl/archive/v0.2.6.tar.gz
 Keywords: language model,t5,gpt3,bert,perplexity,nlp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lmppl-0.2.5/README.md` & `lmppl-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.5/lmppl/openai_models.py` & `lmppl-0.2.6/lmppl/openai_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         @param model: OpenAI model.
         """
         logging.info(f'Loading Model: `{model}`')
         openai.api_key = api_key
         self.model = model
         self.sleep_time = sleep_time
 
-    def get_perplexity(self, input_texts: str or List):
+    def get_perplexity(self, input_texts: str or List, *args, **kwargs):
         """ Compute the perplexity on recurrent LM.
 
         :param input_texts: A string or list of input texts for the encoder.
         :return: A value or list of perplexity.
         """
         single_input = type(input_texts) == str
         input_texts = [input_texts] if single_input else input_texts
```

### Comparing `lmppl-0.2.5/lmppl/ppl_encoder_decoder_lm.py` & `lmppl-0.2.6/lmppl/ppl_encoder_decoder_lm.py`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.5/lmppl/ppl_mlm.py` & `lmppl-0.2.6/lmppl/ppl_mlm.py`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.5/lmppl/ppl_recurrent_lm.py` & `lmppl-0.2.6/lmppl/ppl_recurrent_lm.py`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.5/lmppl.egg-info/PKG-INFO` & `lmppl-0.2.6/lmppl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lmppl
-Version: 0.2.5
+Version: 0.2.6
 Summary: Calculate perplexity on the text with pre-trained language models.
 Home-page: https://github.com/asahi417/lmppl
 Author: Asahi Ushio
 Author-email: asahi1992ushio@gmail.com
 License: MIT License
-Download-URL: https://github.com/asahi417/lmppl/archive/v0.2.5.tar.gz
+Download-URL: https://github.com/asahi417/lmppl/archive/v0.2.6.tar.gz
 Keywords: language model,t5,gpt3,bert,perplexity,nlp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lmppl-0.2.5/setup.py` & `lmppl-0.2.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     readme = f.read()
-VERSION = '0.2.5'
+VERSION = '0.2.6'
 NAME = 'lmppl'
 LICENSE = 'MIT License'
 setup(
     name=NAME,
     packages=find_packages(exclude=['tests', 'misc', 'asset']),
     version=VERSION,
     license=LICENSE,
```

### Comparing `lmppl-0.2.5/test/test_analogy.py` & `lmppl-0.2.6/test/test_analogy.py`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.5/test/test_model_with_simple_input.py` & `lmppl-0.2.6/test/test_model_with_simple_input.py`

 * *Files identical despite different names*

