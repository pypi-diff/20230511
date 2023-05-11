# Comparing `tmp/hyt-gpt-0.3.5.tar.gz` & `tmp/hyt-gpt-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyt-gpt-0.3.5.tar", last modified: Thu May 11 04:23:31 2023, max compression
+gzip compressed data, was "hyt-gpt-0.3.6.tar", last modified: Thu May 11 04:40:07 2023, max compression
```

## Comparing `hyt-gpt-0.3.5.tar` & `hyt-gpt-0.3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 04:23:31.958724 hyt-gpt-0.3.5/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-05-11 04:23:31.958724 hyt-gpt-0.3.5/PKG-INFO
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 04:23:31.958724 hyt-gpt-0.3.5/hyt_gpt/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        0 2023-03-26 03:01:59.000000 hyt-gpt-0.3.5/hyt_gpt/__init__.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     4000 2023-05-06 17:04:43.000000 hyt-gpt-0.3.5/hyt_gpt/gpt.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     2886 2023-03-26 03:01:59.000000 hyt-gpt-0.3.5/hyt_gpt/notion.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     8126 2023-05-11 04:20:21.000000 hyt-gpt-0.3.5/hyt_gpt/youtube.py
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 04:23:31.958724 hyt-gpt-0.3.5/hyt_gpt.egg-info/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-05-11 04:23:31.000000 hyt-gpt-0.3.5/hyt_gpt.egg-info/PKG-INFO
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      204 2023-05-11 04:23:31.000000 hyt-gpt-0.3.5/hyt_gpt.egg-info/SOURCES.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        1 2023-05-11 04:23:31.000000 hyt-gpt-0.3.5/hyt_gpt.egg-info/dependency_links.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        8 2023-05-11 04:23:31.000000 hyt-gpt-0.3.5/hyt_gpt.egg-info/top_level.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)       38 2023-05-11 04:23:31.958724 hyt-gpt-0.3.5/setup.cfg
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      837 2023-05-11 04:23:22.000000 hyt-gpt-0.3.5/setup.py
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 04:40:07.196667 hyt-gpt-0.3.6/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-05-11 04:40:07.196667 hyt-gpt-0.3.6/PKG-INFO
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 04:40:07.196667 hyt-gpt-0.3.6/hyt_gpt/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        0 2023-03-26 03:01:59.000000 hyt-gpt-0.3.6/hyt_gpt/__init__.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     4000 2023-05-06 17:04:43.000000 hyt-gpt-0.3.6/hyt_gpt/gpt.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     2886 2023-03-26 03:01:59.000000 hyt-gpt-0.3.6/hyt_gpt/notion.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     8502 2023-05-11 04:39:48.000000 hyt-gpt-0.3.6/hyt_gpt/youtube.py
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-05-11 04:40:07.196667 hyt-gpt-0.3.6/hyt_gpt.egg-info/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-05-11 04:40:07.000000 hyt-gpt-0.3.6/hyt_gpt.egg-info/PKG-INFO
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      204 2023-05-11 04:40:07.000000 hyt-gpt-0.3.6/hyt_gpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        1 2023-05-11 04:40:07.000000 hyt-gpt-0.3.6/hyt_gpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        8 2023-05-11 04:40:07.000000 hyt-gpt-0.3.6/hyt_gpt.egg-info/top_level.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)       38 2023-05-11 04:40:07.196667 hyt-gpt-0.3.6/setup.cfg
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      837 2023-05-11 04:40:01.000000 hyt-gpt-0.3.6/setup.py
```

### Comparing `hyt-gpt-0.3.5/PKG-INFO` & `hyt-gpt-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.3.5
+Version: 0.3.6
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.3.5/hyt_gpt/gpt.py` & `hyt-gpt-0.3.6/hyt_gpt/gpt.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.3.5/hyt_gpt/notion.py` & `hyt-gpt-0.3.6/hyt_gpt/notion.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.3.5/hyt_gpt/youtube.py` & `hyt-gpt-0.3.6/hyt_gpt/youtube.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,29 +33,30 @@
                 "status": "failed",
                 "url": ylink,
                 "subtitles": subtitles,
                 "summaries": "Subtitle retrieval failed",
             }
 
         seged_text = seg_transcript(subtitles)
+        print(len(HytGpt.parse_text_from_start_duration(subtitles)))
         summaried_text = ""
-        i = 1
+        # i = 1
 
-        for entry in seged_text:
-            try:
-                response = chat_gpt(
-                    self.gpt_key, self.prompt.format(language=language), entry
-                )
-                print(f"Completed the {str(i)} part summary")
-                i += 1
-            except Exception as e:
-                print(f"Exception occurred: {str(e)}")
-                traceback.print_exc()
-                response = "Summary failed"
-            summaried_text += response + "\n"
+        # for entry in seged_text:
+        #     try:
+        #         response = chat_gpt(
+        #             self.gpt_key, self.prompt.format(language=language), entry
+        #         )
+        #         print(f"Completed the {str(i)} part summary")
+        #         i += 1
+        #     except Exception as e:
+        #         print(f"Exception occurred: {str(e)}")
+        #         traceback.print_exc()
+        #         response = "Summary failed"
+        #     summaried_text += response + "\n"
         response_data = {
             "status": "success",
             "url": ylink,
             "subtitles": subtitles,
             "summaries": summaried_text,
         }
         return response_data
@@ -86,29 +87,38 @@
     @staticmethod
     def get_timestamp_diff(start_time, end_time):
         start_time = datetime.strptime(start_time, "%H:%M:%S.%f")
         end_time = datetime.strptime(end_time, "%H:%M:%S.%f")
         diff = (end_time - start_time).total_seconds()
         return diff
 
+    @staticmethod
+    def should_concatenate(segment1, segment2, max_time_difference=1.1): # seconds
+        current_end_time = segment1['start'] + segment1['duration']
+        next_start_time = segment2['start']
+        is_close = current_end_time + max_time_difference > next_start_time
+        no_punctuation = not segment1['text'].strip().endswith(('.', '?', '!'))
+        return is_close and no_punctuation
+
     @staticmethod    
     def parse_text_from_start_duration(subtitles: List[Dict[str, str]]) -> List[str]:
         combined_texts = []
         current_text = subtitles[0]['text']
-        current_end_time = subtitles[0]['start'] + subtitles[0]['duration']
+        current_segment = subtitles[0]
 
         for i in range(1, len(subtitles)):
-            next_start_time = subtitles[i]['start']
-            if current_end_time + 0.5 > next_start_time: # if the next subtitle is within 1 second of the current subtitle # type: ignore
-                current_text += " " + subtitles[i]['text']
+            next_segment = subtitles[i]
+            
+            if HytGpt.should_concatenate(current_segment, next_segment):
+                current_text += " " + next_segment['text']
             else:
                 combined_texts.append(current_text)
-                current_text = subtitles[i]['text']
+                current_text = next_segment['text']
 
-            current_end_time = next_start_time + subtitles[i]['duration']
+            current_segment = next_segment
 
         combined_texts.append(current_text)
         return combined_texts
 
 
     def __youtube_subtitle(
         self, url: str
```

### Comparing `hyt-gpt-0.3.5/hyt_gpt.egg-info/PKG-INFO` & `hyt-gpt-0.3.6/hyt_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.3.5
+Version: 0.3.6
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.3.5/setup.py` & `hyt-gpt-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name='hyt-gpt',
-    version='0.3.5',
+    version='0.3.6',
     description='A library for GPT and Youtube',
     author='Harbin',
     author_email='harbinfate@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

