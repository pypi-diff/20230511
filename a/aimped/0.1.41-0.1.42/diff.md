# Comparing `tmp/aimped-0.1.41.tar.gz` & `tmp/aimped-0.1.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimped-0.1.41.tar", last modified: Fri May  5 13:54:48 2023, max compression
+gzip compressed data, was "aimped-0.1.42.tar", last modified: Thu May 11 09:15:00 2023, max compression
```

## Comparing `aimped-0.1.41.tar` & `aimped-0.1.42.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-05 13:54:48.751413 aimped-0.1.41/
--rw-rw-r--   0 forest    (1000) forest    (1000)     1063 2023-05-05 13:49:40.000000 aimped-0.1.41/LICENSE
--rw-rw-r--   0 forest    (1000) forest    (1000)     1740 2023-05-05 13:54:48.751413 aimped-0.1.41/PKG-INFO
--rw-rw-r--   0 forest    (1000) forest    (1000)     1170 2023-05-05 13:52:11.000000 aimped-0.1.41/README.md
-drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-05 13:54:48.743413 aimped-0.1.41/aimped/
--rw-rw-r--   0 forest    (1000) forest    (1000)      165 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/__init__.py
-drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-05 13:54:48.747413 aimped-0.1.41/aimped/model/
--rw-rw-r--   0 forest    (1000) forest    (1000)        0 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/model/__init__.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     2338 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/model/load.py
--rw-rw-r--   0 forest    (1000) forest    (1000)      502 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/models.py
-drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-05 13:54:48.747413 aimped-0.1.41/aimped/nitro/
--rw-rw-r--   0 forest    (1000) forest    (1000)        0 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/nitro/__init__.py
-drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-05 13:54:48.747413 aimped-0.1.41/aimped/nlp/
--rw-rw-r--   0 forest    (1000) forest    (1000)      353 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/nlp/__init__.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     2228 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/nlp/assertion.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     3917 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/nlp/chunker.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     2825 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/nlp/deid.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     4521 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/nlp/ner.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     2629 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/nlp/ner_cls_report.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     7231 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/nlp/pipeline.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     3899 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/nlp/regex_parser.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     4592 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/nlp/relation.py
--rw-rw-r--   0 forest    (1000) forest    (1000)    19853 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/nlp/relation_visualizer.py
--rw-rw-r--   0 forest    (1000) forest    (1000)      803 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/nlp/tokenizer.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     2251 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/nlp/tools.py
--rwxrwxrwx   0 forest    (1000) forest    (1000)     2524 2023-05-01 20:16:49.000000 aimped-0.1.41/aimped/nlp/translation.py
-drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-05 13:54:48.747413 aimped-0.1.41/aimped/test/
--rw-rw-r--   0 forest    (1000) forest    (1000)        0 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/test/__init__.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     2748 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/test/test_assertion.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     1313 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/test/test_chunk_merger.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     1866 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/test/test_deid_pipeline.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     1297 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/test/test_ner_results.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     1592 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/test/test_regex_parser.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     3320 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/test/test_relation_pipeline.py
--rw-rw-r--   0 forest    (1000) forest    (1000)      610 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/test/test_tokenizer.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     5585 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/test/test_translation_pipeline.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     2056 2023-05-05 13:49:40.000000 aimped-0.1.41/aimped/utils.py
--rw-rw-r--   0 forest    (1000) forest    (1000)      123 2023-05-05 13:52:32.000000 aimped-0.1.41/aimped/version.py
-drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-05 13:54:48.747413 aimped-0.1.41/aimped.egg-info/
--rw-rw-r--   0 forest    (1000) forest    (1000)     1740 2023-05-05 13:54:48.000000 aimped-0.1.41/aimped.egg-info/PKG-INFO
--rw-rw-r--   0 forest    (1000) forest    (1000)      933 2023-05-05 13:54:48.000000 aimped-0.1.41/aimped.egg-info/SOURCES.txt
--rw-rw-r--   0 forest    (1000) forest    (1000)        1 2023-05-05 13:54:48.000000 aimped-0.1.41/aimped.egg-info/dependency_links.txt
--rw-rw-r--   0 forest    (1000) forest    (1000)       39 2023-05-05 13:54:48.000000 aimped-0.1.41/aimped.egg-info/requires.txt
--rw-rw-r--   0 forest    (1000) forest    (1000)        7 2023-05-05 13:54:48.000000 aimped-0.1.41/aimped.egg-info/top_level.txt
--rw-rw-r--   0 forest    (1000) forest    (1000)      103 2023-05-05 13:54:48.751413 aimped-0.1.41/setup.cfg
--rw-rw-r--   0 forest    (1000) forest    (1000)     1139 2023-05-05 13:49:40.000000 aimped-0.1.41/setup.py
+drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-11 09:15:00.684665 aimped-0.1.42/
+-rw-rw-r--   0 forest    (1000) forest    (1000)     1063 2023-05-05 13:49:40.000000 aimped-0.1.42/LICENSE
+-rw-rw-r--   0 forest    (1000) forest    (1000)     1740 2023-05-11 09:15:00.684665 aimped-0.1.42/PKG-INFO
+-rw-rw-r--   0 forest    (1000) forest    (1000)     1170 2023-05-05 13:52:11.000000 aimped-0.1.42/README.md
+drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-11 09:15:00.680665 aimped-0.1.42/aimped/
+-rw-rw-r--   0 forest    (1000) forest    (1000)      165 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/__init__.py
+drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-11 09:15:00.684665 aimped-0.1.42/aimped/model/
+-rw-rw-r--   0 forest    (1000) forest    (1000)        0 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/model/__init__.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     2338 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/model/load.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)      502 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/models.py
+drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-11 09:15:00.684665 aimped-0.1.42/aimped/nitro/
+-rw-rw-r--   0 forest    (1000) forest    (1000)        0 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nitro/__init__.py
+drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-11 09:15:00.684665 aimped-0.1.42/aimped/nlp/
+-rw-rw-r--   0 forest    (1000) forest    (1000)      353 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/__init__.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     2228 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/assertion.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     3917 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/chunker.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     2825 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/deid.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     4521 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/ner.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     2629 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/ner_cls_report.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     7231 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/pipeline.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     3899 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/regex_parser.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     4592 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/relation.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)    19853 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/relation_visualizer.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)      803 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/tokenizer.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     2251 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/tools.py
+-rwxrwxrwx   0 forest    (1000) forest    (1000)     2524 2023-05-11 09:11:50.000000 aimped-0.1.42/aimped/nlp/translation.py
+drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-11 09:15:00.684665 aimped-0.1.42/aimped/test/
+-rw-rw-r--   0 forest    (1000) forest    (1000)        0 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/__init__.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     2748 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/test_assertion.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     1313 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/test_chunk_merger.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     1866 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/test_deid_pipeline.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     1297 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/test_ner_results.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     1592 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/test_regex_parser.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     3320 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/test_relation_pipeline.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)      610 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/test_tokenizer.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     5585 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/test_translation_pipeline.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)     2056 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/utils.py
+-rw-rw-r--   0 forest    (1000) forest    (1000)      123 2023-05-11 09:13:14.000000 aimped-0.1.42/aimped/version.py
+drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-11 09:15:00.684665 aimped-0.1.42/aimped.egg-info/
+-rw-rw-r--   0 forest    (1000) forest    (1000)     1740 2023-05-11 09:15:00.000000 aimped-0.1.42/aimped.egg-info/PKG-INFO
+-rw-rw-r--   0 forest    (1000) forest    (1000)      933 2023-05-11 09:15:00.000000 aimped-0.1.42/aimped.egg-info/SOURCES.txt
+-rw-rw-r--   0 forest    (1000) forest    (1000)        1 2023-05-11 09:15:00.000000 aimped-0.1.42/aimped.egg-info/dependency_links.txt
+-rw-rw-r--   0 forest    (1000) forest    (1000)       39 2023-05-11 09:15:00.000000 aimped-0.1.42/aimped.egg-info/requires.txt
+-rw-rw-r--   0 forest    (1000) forest    (1000)        7 2023-05-11 09:15:00.000000 aimped-0.1.42/aimped.egg-info/top_level.txt
+-rw-rw-r--   0 forest    (1000) forest    (1000)      103 2023-05-11 09:15:00.684665 aimped-0.1.42/setup.cfg
+-rw-rw-r--   0 forest    (1000) forest    (1000)     1139 2023-05-05 13:49:40.000000 aimped-0.1.42/setup.py
```

### Comparing `aimped-0.1.41/LICENSE` & `aimped-0.1.42/LICENSE`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/PKG-INFO` & `aimped-0.1.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimped
-Version: 0.1.41
+Version: 0.1.42
 Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
 Home-page: https://dev.ml-hub.nioyatechai.com/
 Author: Russell C.
 Author-email: russell@aimped.com
 Maintainer: aimped
 Maintainer-email: contact@aimped.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aimped-0.1.41/README.md` & `aimped-0.1.42/README.md`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/model/load.py` & `aimped-0.1.42/aimped/model/load.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/nlp/assertion.py` & `aimped-0.1.42/aimped/nlp/assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/nlp/chunker.py` & `aimped-0.1.42/aimped/nlp/chunker.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/nlp/deid.py` & `aimped-0.1.42/aimped/nlp/deid.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/nlp/ner.py` & `aimped-0.1.42/aimped/nlp/ner.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/nlp/ner_cls_report.py` & `aimped-0.1.42/aimped/nlp/ner_cls_report.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/nlp/pipeline.py` & `aimped-0.1.42/aimped/nlp/pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/nlp/regex_parser.py` & `aimped-0.1.42/aimped/nlp/regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/nlp/relation.py` & `aimped-0.1.42/aimped/nlp/relation.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/nlp/relation_visualizer.py` & `aimped-0.1.42/aimped/nlp/relation_visualizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/nlp/tokenizer.py` & `aimped-0.1.42/aimped/nlp/tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/nlp/tools.py` & `aimped-0.1.42/aimped/nlp/tools.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/nlp/translation.py` & `aimped-0.1.42/aimped/nlp/translation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def translate_text(input_texts, source_lang, pipeline):
+def text_translate(input_texts, source_lang, pipeline):
     """
     Splits the input text into sentences and creates batches of sentences to be fed into the model.
 
     Args:
         text (str): The input text to be split into sentences.
         source_lang (str): The language of the input text.
         language_codes (dict): A dictionary mapping language names to their corresponding language codes.
```

### Comparing `aimped-0.1.41/aimped/test/test_assertion.py` & `aimped-0.1.42/aimped/test/test_assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/test/test_chunk_merger.py` & `aimped-0.1.42/aimped/test/test_chunk_merger.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/test/test_deid_pipeline.py` & `aimped-0.1.42/aimped/test/test_deid_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/test/test_ner_results.py` & `aimped-0.1.42/aimped/test/test_ner_results.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/test/test_regex_parser.py` & `aimped-0.1.42/aimped/test/test_regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/test/test_relation_pipeline.py` & `aimped-0.1.42/aimped/test/test_relation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/test/test_tokenizer.py` & `aimped-0.1.42/aimped/test/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/test/test_translation_pipeline.py` & `aimped-0.1.42/aimped/test/test_translation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped/utils.py` & `aimped-0.1.42/aimped/utils.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/aimped.egg-info/PKG-INFO` & `aimped-0.1.42/aimped.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimped
-Version: 0.1.41
+Version: 0.1.42
 Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
 Home-page: https://dev.ml-hub.nioyatechai.com/
 Author: Russell C.
 Author-email: russell@aimped.com
 Maintainer: aimped
 Maintainer-email: contact@aimped.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aimped-0.1.41/aimped.egg-info/SOURCES.txt` & `aimped-0.1.42/aimped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aimped-0.1.41/setup.py` & `aimped-0.1.42/setup.py`

 * *Files identical despite different names*

