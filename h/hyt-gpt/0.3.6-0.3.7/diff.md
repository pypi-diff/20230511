# Comparing `tmp/hyt-gpt-0.3.6.tar.gz` & `tmp/hyt-gpt-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyt-gpt-0.3.6.tar", last modified: Thu May 11 04:40:07 2023, max compression
+gzip compressed data, was "hyt-gpt-0.3.7.tar", last modified: Thu May 11 06:19:59 2023, max compression
```

## Comparing `hyt-gpt-0.3.6.tar` & `hyt-gpt-0.3.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 04:40:07.196667 hyt-gpt-0.3.6/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-05-11 04:40:07.196667 hyt-gpt-0.3.6/PKG-INFO
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 04:40:07.196667 hyt-gpt-0.3.6/hyt_gpt/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        0 2023-03-26 03:01:59.000000 hyt-gpt-0.3.6/hyt_gpt/__init__.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     4000 2023-05-06 17:04:43.000000 hyt-gpt-0.3.6/hyt_gpt/gpt.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     2886 2023-03-26 03:01:59.000000 hyt-gpt-0.3.6/hyt_gpt/notion.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     8502 2023-05-11 04:39:48.000000 hyt-gpt-0.3.6/hyt_gpt/youtube.py
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 04:40:07.196667 hyt-gpt-0.3.6/hyt_gpt.egg-info/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-05-11 04:40:07.000000 hyt-gpt-0.3.6/hyt_gpt.egg-info/PKG-INFO
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      204 2023-05-11 04:40:07.000000 hyt-gpt-0.3.6/hyt_gpt.egg-info/SOURCES.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        1 2023-05-11 04:40:07.000000 hyt-gpt-0.3.6/hyt_gpt.egg-info/dependency_links.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        8 2023-05-11 04:40:07.000000 hyt-gpt-0.3.6/hyt_gpt.egg-info/top_level.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)       38 2023-05-11 04:40:07.196667 hyt-gpt-0.3.6/setup.cfg
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      837 2023-05-11 04:40:01.000000 hyt-gpt-0.3.6/setup.py
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 06:19:59.351512 hyt-gpt-0.3.7/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-05-11 06:19:59.351512 hyt-gpt-0.3.7/PKG-INFO
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 06:19:59.351512 hyt-gpt-0.3.7/hyt_gpt/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        0 2023-03-26 03:01:59.000000 hyt-gpt-0.3.7/hyt_gpt/__init__.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     4038 2023-05-11 05:46:57.000000 hyt-gpt-0.3.7/hyt_gpt/gpt.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     2886 2023-03-26 03:01:59.000000 hyt-gpt-0.3.7/hyt_gpt/notion.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)    12445 2023-05-11 06:05:50.000000 hyt-gpt-0.3.7/hyt_gpt/youtube.py
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 06:19:59.351512 hyt-gpt-0.3.7/hyt_gpt.egg-info/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-05-11 06:19:59.000000 hyt-gpt-0.3.7/hyt_gpt.egg-info/PKG-INFO
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      204 2023-05-11 06:19:59.000000 hyt-gpt-0.3.7/hyt_gpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        1 2023-05-11 06:19:59.000000 hyt-gpt-0.3.7/hyt_gpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        8 2023-05-11 06:19:59.000000 hyt-gpt-0.3.7/hyt_gpt.egg-info/top_level.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)       38 2023-05-11 06:19:59.351512 hyt-gpt-0.3.7/setup.cfg
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      837 2023-05-11 06:19:50.000000 hyt-gpt-0.3.7/setup.py
```

### Comparing `hyt-gpt-0.3.6/PKG-INFO` & `hyt-gpt-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.3.6
+Version: 0.3.7
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.3.6/hyt_gpt/gpt.py` & `hyt-gpt-0.3.7/hyt_gpt/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-from typing import List
+from typing import List, Dict, Union
 import logging
 import tiktoken
 
 
 def chat_gpt(key, prompt, text):
     API_KEY = key
     headers = {
@@ -23,15 +23,15 @@
     if response.status_code != 200:
         logging.info('response:', response.content)
         return str(response.json()['error'])
 
     return response.json()['choices'][0]['message']['content']
 
 
-def seg_transcript(transcript: List[str]) -> List[str]:
+def seg_transcript(transcript: List[Dict[str, Union[str, float]]]) -> List[str]:
     transcript = [{"text": item["text"], "index": index,
                    "timestamp": item["start"]} for index, item in enumerate(transcript)]
     text = " ".join([x["text"]
                     for x in sorted(transcript, key=lambda x: x["index"])])
     enc = tiktoken.get_encoding("cl100k_base")
     len_original = len(enc.encode(text))
     seg_length = 3500
```

### Comparing `hyt-gpt-0.3.6/hyt_gpt/notion.py` & `hyt-gpt-0.3.7/hyt_gpt/notion.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.3.6/hyt_gpt.egg-info/PKG-INFO` & `hyt-gpt-0.3.7/hyt_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.3.6
+Version: 0.3.7
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.3.6/setup.py` & `hyt-gpt-0.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name='hyt-gpt',
-    version='0.3.6',
+    version='0.3.7',
     description='A library for GPT and Youtube',
     author='Harbin',
     author_email='harbinfate@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

