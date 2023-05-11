# Comparing `tmp/hyt-gpt-0.3.4.tar.gz` & `tmp/hyt-gpt-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyt-gpt-0.3.4.tar", last modified: Sat May  6 03:33:35 2023, max compression
+gzip compressed data, was "hyt-gpt-0.3.5.tar", last modified: Thu May 11 04:23:31 2023, max compression
```

## Comparing `hyt-gpt-0.3.4.tar` & `hyt-gpt-0.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:33:35.786681 hyt-gpt-0.3.4/
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      702 2023-05-06 03:33:35.786681 hyt-gpt-0.3.4/PKG-INFO
-drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:33:35.786681 hyt-gpt-0.3.4/hyt_gpt/
--rw-r-----   0 haibinzh (778454) primarygroup (89939)        0 2023-04-19 01:16:56.000000 hyt-gpt-0.3.4/hyt_gpt/__init__.py
--rw-r-----   0 haibinzh (778454) primarygroup (89939)     4000 2023-05-06 03:19:55.000000 hyt-gpt-0.3.4/hyt_gpt/gpt.py
--rw-r-----   0 haibinzh (778454) primarygroup (89939)     2886 2023-04-19 01:16:56.000000 hyt-gpt-0.3.4/hyt_gpt/notion.py
--rw-r-----   0 haibinzh (778454) primarygroup (89939)     7325 2023-05-06 03:33:18.000000 hyt-gpt-0.3.4/hyt_gpt/youtube.py
-drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:33:35.786681 hyt-gpt-0.3.4/hyt_gpt.egg-info/
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      702 2023-05-06 03:33:35.000000 hyt-gpt-0.3.4/hyt_gpt.egg-info/PKG-INFO
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      204 2023-05-06 03:33:35.000000 hyt-gpt-0.3.4/hyt_gpt.egg-info/SOURCES.txt
--rw-r-----   0 haibinzh (778454) primarygroup (89939)        1 2023-05-06 03:33:35.000000 hyt-gpt-0.3.4/hyt_gpt.egg-info/dependency_links.txt
--rw-r-----   0 haibinzh (778454) primarygroup (89939)        8 2023-05-06 03:33:35.000000 hyt-gpt-0.3.4/hyt_gpt.egg-info/top_level.txt
--rw-r-----   0 haibinzh (778454) primarygroup (89939)       38 2023-05-06 03:33:35.786681 hyt-gpt-0.3.4/setup.cfg
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      837 2023-05-06 03:33:29.000000 hyt-gpt-0.3.4/setup.py
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 04:23:31.958724 hyt-gpt-0.3.5/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-05-11 04:23:31.958724 hyt-gpt-0.3.5/PKG-INFO
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 04:23:31.958724 hyt-gpt-0.3.5/hyt_gpt/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        0 2023-03-26 03:01:59.000000 hyt-gpt-0.3.5/hyt_gpt/__init__.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     4000 2023-05-06 17:04:43.000000 hyt-gpt-0.3.5/hyt_gpt/gpt.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     2886 2023-03-26 03:01:59.000000 hyt-gpt-0.3.5/hyt_gpt/notion.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     8126 2023-05-11 04:20:21.000000 hyt-gpt-0.3.5/hyt_gpt/youtube.py
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 04:23:31.958724 hyt-gpt-0.3.5/hyt_gpt.egg-info/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-05-11 04:23:31.000000 hyt-gpt-0.3.5/hyt_gpt.egg-info/PKG-INFO
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      204 2023-05-11 04:23:31.000000 hyt-gpt-0.3.5/hyt_gpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        1 2023-05-11 04:23:31.000000 hyt-gpt-0.3.5/hyt_gpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        8 2023-05-11 04:23:31.000000 hyt-gpt-0.3.5/hyt_gpt.egg-info/top_level.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)       38 2023-05-11 04:23:31.958724 hyt-gpt-0.3.5/setup.cfg
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      837 2023-05-11 04:23:22.000000 hyt-gpt-0.3.5/setup.py
```

### Comparing `hyt-gpt-0.3.4/PKG-INFO` & `hyt-gpt-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.3.4
+Version: 0.3.5
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.3.4/hyt_gpt/gpt.py` & `hyt-gpt-0.3.5/hyt_gpt/gpt.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.3.4/hyt_gpt/notion.py` & `hyt-gpt-0.3.5/hyt_gpt/notion.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.3.4/hyt_gpt/youtube.py` & `hyt-gpt-0.3.5/hyt_gpt/youtube.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,20 +86,40 @@
     @staticmethod
     def get_timestamp_diff(start_time, end_time):
         start_time = datetime.strptime(start_time, "%H:%M:%S.%f")
         end_time = datetime.strptime(end_time, "%H:%M:%S.%f")
         diff = (end_time - start_time).total_seconds()
         return diff
 
+    @staticmethod    
+    def parse_text_from_start_duration(subtitles: List[Dict[str, str]]) -> List[str]:
+        combined_texts = []
+        current_text = subtitles[0]['text']
+        current_end_time = subtitles[0]['start'] + subtitles[0]['duration']
+
+        for i in range(1, len(subtitles)):
+            next_start_time = subtitles[i]['start']
+            if current_end_time + 0.5 > next_start_time: # if the next subtitle is within 1 second of the current subtitle # type: ignore
+                current_text += " " + subtitles[i]['text']
+            else:
+                combined_texts.append(current_text)
+                current_text = subtitles[i]['text']
+
+            current_end_time = next_start_time + subtitles[i]['duration']
+
+        combined_texts.append(current_text)
+        return combined_texts
+
+
     def __youtube_subtitle(
         self, url: str
     ) -> Tuple[Union[List[Dict[str, str]], None], str]:
         video_id = self.get_youtube_id(url)
         list = YouTubeTranscriptApi.list_transcripts(video_id)
-        logging.debug("transcript_lists: ", list)
+        logging.debug(list)
         
         for transcript in list:
             if transcript.language_code in ["en", "zh", "zh-Hans", "zh-Hant"]:
                 return transcript.fetch(), transcript.language
         # if 'zh-Hans' in transicript.translation_languages:
         #     translated = transicript.translate('zh-Hans').fetch()
         #     return translated
```

### Comparing `hyt-gpt-0.3.4/hyt_gpt.egg-info/PKG-INFO` & `hyt-gpt-0.3.5/hyt_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.3.4
+Version: 0.3.5
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.3.4/setup.py` & `hyt-gpt-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name='hyt-gpt',
-    version='0.3.4',
+    version='0.3.5',
     description='A library for GPT and Youtube',
     author='Harbin',
     author_email='harbinfate@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

