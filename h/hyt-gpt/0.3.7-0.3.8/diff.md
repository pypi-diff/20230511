# Comparing `tmp/hyt-gpt-0.3.7.tar.gz` & `tmp/hyt-gpt-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyt-gpt-0.3.7.tar", last modified: Thu May 11 06:19:59 2023, max compression
+gzip compressed data, was "hyt-gpt-0.3.8.tar", last modified: Thu May 11 06:43:02 2023, max compression
```

## Comparing `hyt-gpt-0.3.7.tar` & `hyt-gpt-0.3.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 06:19:59.351512 hyt-gpt-0.3.7/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-05-11 06:19:59.351512 hyt-gpt-0.3.7/PKG-INFO
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 06:19:59.351512 hyt-gpt-0.3.7/hyt_gpt/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        0 2023-03-26 03:01:59.000000 hyt-gpt-0.3.7/hyt_gpt/__init__.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     4038 2023-05-11 05:46:57.000000 hyt-gpt-0.3.7/hyt_gpt/gpt.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     2886 2023-03-26 03:01:59.000000 hyt-gpt-0.3.7/hyt_gpt/notion.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)    12445 2023-05-11 06:05:50.000000 hyt-gpt-0.3.7/hyt_gpt/youtube.py
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 06:19:59.351512 hyt-gpt-0.3.7/hyt_gpt.egg-info/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-05-11 06:19:59.000000 hyt-gpt-0.3.7/hyt_gpt.egg-info/PKG-INFO
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      204 2023-05-11 06:19:59.000000 hyt-gpt-0.3.7/hyt_gpt.egg-info/SOURCES.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        1 2023-05-11 06:19:59.000000 hyt-gpt-0.3.7/hyt_gpt.egg-info/dependency_links.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        8 2023-05-11 06:19:59.000000 hyt-gpt-0.3.7/hyt_gpt.egg-info/top_level.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)       38 2023-05-11 06:19:59.351512 hyt-gpt-0.3.7/setup.cfg
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      837 2023-05-11 06:19:50.000000 hyt-gpt-0.3.7/setup.py
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 06:43:02.432431 hyt-gpt-0.3.8/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-05-11 06:43:02.432431 hyt-gpt-0.3.8/PKG-INFO
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 06:43:02.432431 hyt-gpt-0.3.8/hyt_gpt/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        0 2023-03-26 03:01:59.000000 hyt-gpt-0.3.8/hyt_gpt/__init__.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     4038 2023-05-11 05:46:57.000000 hyt-gpt-0.3.8/hyt_gpt/gpt.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     2886 2023-03-26 03:01:59.000000 hyt-gpt-0.3.8/hyt_gpt/notion.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)    12461 2023-05-11 06:42:30.000000 hyt-gpt-0.3.8/hyt_gpt/youtube.py
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 06:43:02.432431 hyt-gpt-0.3.8/hyt_gpt.egg-info/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-05-11 06:43:02.000000 hyt-gpt-0.3.8/hyt_gpt.egg-info/PKG-INFO
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      204 2023-05-11 06:43:02.000000 hyt-gpt-0.3.8/hyt_gpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        1 2023-05-11 06:43:02.000000 hyt-gpt-0.3.8/hyt_gpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        8 2023-05-11 06:43:02.000000 hyt-gpt-0.3.8/hyt_gpt.egg-info/top_level.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)       38 2023-05-11 06:43:02.432431 hyt-gpt-0.3.8/setup.cfg
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      837 2023-05-11 06:42:53.000000 hyt-gpt-0.3.8/setup.py
```

### Comparing `hyt-gpt-0.3.7/PKG-INFO` & `hyt-gpt-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.3.7
+Version: 0.3.8
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.3.7/hyt_gpt/gpt.py` & `hyt-gpt-0.3.8/hyt_gpt/gpt.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.3.7/hyt_gpt/notion.py` & `hyt-gpt-0.3.8/hyt_gpt/notion.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.3.7/hyt_gpt/youtube.py` & `hyt-gpt-0.3.8/hyt_gpt/youtube.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import re
 import os
 import subprocess
 import io
 import sys
-from typing import Dict, Any, List, Union, Tuple
+from typing import Dict, Any, List, Union, Tuple, Optional
 from .gpt import seg_transcript, chat_gpt
 from datetime import datetime
 from youtube_transcript_api import YouTubeTranscriptApi
 from pydub import AudioSegment
 from pydub.utils import make_chunks
 
 # TODO: Use google.cloud.speech_v2 instead of google.cloud.speech_v1p1beta1
@@ -88,15 +88,15 @@
         # Check if the URL matches the pattern
         if youtube_url_pattern.match(url):
             return True
         else:
             return False
 
     @staticmethod
-    def get_youtube_id(url: str) -> str | None:
+    def get_youtube_id(url: str) -> Optional[str]:
         youtube_id_match = re.search(r"(?<=v=)[^&#]+", url)
         youtube_id_match = youtube_id_match or re.search(r"(?<=be/)[^&#]+", url)
         return youtube_id_match.group(0) if youtube_id_match else None
 
     @staticmethod
     def build_youtube_url(youtube_id: str) -> str:
         return f"https://www.youtube.com/watch?v={youtube_id}"
@@ -223,15 +223,15 @@
             chunk.export(chunk_name, format="mp3")
             chunk_files.append(chunk_name)
 
         return chunk_files
 
     def __youtube_subtitle(
         self, url: str
-    ) -> Tuple[start_duration_transcript_t | None, str]:
+    ) -> Tuple[Optional[start_duration_transcript_t], str]:
         """Get the subtitle of the youtube video
         Args:
             url (str): The url of the youtube video
         Returns:
             Tuple[Union[List[Dict[str, str]], None], str]: The subtitle of the youtube video
         """
         video_id = self.get_youtube_id(url)
```

### Comparing `hyt-gpt-0.3.7/hyt_gpt.egg-info/PKG-INFO` & `hyt-gpt-0.3.8/hyt_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.3.7
+Version: 0.3.8
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.3.7/setup.py` & `hyt-gpt-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name='hyt-gpt',
-    version='0.3.7',
+    version='0.3.8',
     description='A library for GPT and Youtube',
     author='Harbin',
     author_email='harbinfate@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

