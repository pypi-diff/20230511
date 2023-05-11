# Comparing `tmp/slashml-0.0.5.tar.gz` & `tmp/slashml-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/faizank/workspace/experiments/live_projects/slashml/sdk_tests/slashml/dist/.tmp-o1v63c_a/slashml-0.0.5.tar", last modified: Mon May  8 22:45:10 2023, max compression
+gzip compressed data, was "/Users/faizank/workspace/experiments/live_projects/slashml/sdk_tests/slashml/dist/.tmp-d_ea_6v9/slashml-0.0.6.tar", last modified: Thu May 11 05:12:50 2023, max compression
```

## Comparing `slashml-0.0.5.tar` & `slashml-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-08 22:45:10.277303 slashml-0.0.5/
--rw-r--r--   0 faizank    (501) staff       (20)     1064 2023-04-24 05:35:14.000000 slashml-0.0.5/LICENSE.txt
--rw-r--r--   0 faizank    (501) staff       (20)     6379 2023-05-08 22:45:10.277092 slashml-0.0.5/PKG-INFO
--rw-r--r--   0 faizank    (501) staff       (20)     6059 2023-05-08 22:40:33.000000 slashml-0.0.5/README.md
--rw-r--r--   0 faizank    (501) staff       (20)       38 2023-05-08 22:45:10.277362 slashml-0.0.5/setup.cfg
--rw-r--r--   0 faizank    (501) staff       (20)     1022 2023-05-08 22:44:55.000000 slashml-0.0.5/setup.py
-drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-08 22:45:10.275987 slashml-0.0.5/slashml/
--rw-r--r--   0 faizank    (501) staff       (20)      190 2023-05-08 20:59:11.000000 slashml-0.0.5/slashml/__init__.py
--rw-r--r--   0 faizank    (501) staff       (20)     1354 2023-05-08 22:40:33.000000 slashml-0.0.5/slashml/speech_to_text.py
--rw-r--r--   0 faizank    (501) staff       (20)      979 2023-05-08 22:40:33.000000 slashml-0.0.5/slashml/text_summarization.py
--rw-r--r--   0 faizank    (501) staff       (20)      956 2023-05-08 22:40:33.000000 slashml-0.0.5/slashml/text_to_speech.py
--rw-r--r--   0 faizank    (501) staff       (20)     1257 2023-05-08 22:40:33.000000 slashml-0.0.5/slashml/utils.py
-drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-08 22:45:10.276869 slashml-0.0.5/slashml.egg-info/
--rw-r--r--   0 faizank    (501) staff       (20)     6379 2023-05-08 22:45:10.000000 slashml-0.0.5/slashml.egg-info/PKG-INFO
--rw-r--r--   0 faizank    (501) staff       (20)      313 2023-05-08 22:45:10.000000 slashml-0.0.5/slashml.egg-info/SOURCES.txt
--rw-r--r--   0 faizank    (501) staff       (20)        1 2023-05-08 22:45:10.000000 slashml-0.0.5/slashml.egg-info/dependency_links.txt
--rw-r--r--   0 faizank    (501) staff       (20)       31 2023-05-08 22:45:10.000000 slashml-0.0.5/slashml.egg-info/requires.txt
--rw-r--r--   0 faizank    (501) staff       (20)        8 2023-05-08 22:45:10.000000 slashml-0.0.5/slashml.egg-info/top_level.txt
+drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-11 05:12:50.756911 slashml-0.0.6/
+-rw-r--r--   0 faizank    (501) staff       (20)     1064 2023-04-24 05:35:14.000000 slashml-0.0.6/LICENSE.txt
+-rw-r--r--   0 faizank    (501) staff       (20)     5452 2023-05-11 05:12:50.756733 slashml-0.0.6/PKG-INFO
+-rw-r--r--   0 faizank    (501) staff       (20)     5132 2023-05-11 05:12:25.000000 slashml-0.0.6/README.md
+-rw-r--r--   0 faizank    (501) staff       (20)       38 2023-05-11 05:12:50.756969 slashml-0.0.6/setup.cfg
+-rw-r--r--   0 faizank    (501) staff       (20)     1022 2023-05-11 05:12:25.000000 slashml-0.0.6/setup.py
+drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-11 05:12:50.755482 slashml-0.0.6/slashml/
+-rw-r--r--   0 faizank    (501) staff       (20)      190 2023-05-08 20:59:11.000000 slashml-0.0.6/slashml/__init__.py
+-rw-r--r--   0 faizank    (501) staff       (20)     2219 2023-05-11 05:12:25.000000 slashml-0.0.6/slashml/speech_to_text.py
+-rw-r--r--   0 faizank    (501) staff       (20)     1780 2023-05-11 05:12:25.000000 slashml-0.0.6/slashml/text_summarization.py
+-rw-r--r--   0 faizank    (501) staff       (20)     1759 2023-05-11 05:12:25.000000 slashml-0.0.6/slashml/text_to_speech.py
+-rw-r--r--   0 faizank    (501) staff       (20)     1257 2023-05-08 22:40:33.000000 slashml-0.0.6/slashml/utils.py
+drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-11 05:12:50.756525 slashml-0.0.6/slashml.egg-info/
+-rw-r--r--   0 faizank    (501) staff       (20)     5452 2023-05-11 05:12:50.000000 slashml-0.0.6/slashml.egg-info/PKG-INFO
+-rw-r--r--   0 faizank    (501) staff       (20)      313 2023-05-11 05:12:50.000000 slashml-0.0.6/slashml.egg-info/SOURCES.txt
+-rw-r--r--   0 faizank    (501) staff       (20)        1 2023-05-11 05:12:50.000000 slashml-0.0.6/slashml.egg-info/dependency_links.txt
+-rw-r--r--   0 faizank    (501) staff       (20)       31 2023-05-11 05:12:50.000000 slashml-0.0.6/slashml.egg-info/requires.txt
+-rw-r--r--   0 faizank    (501) staff       (20)        8 2023-05-11 05:12:50.000000 slashml-0.0.6/slashml.egg-info/top_level.txt
```

### Comparing `slashml-0.0.5/LICENSE.txt` & `slashml-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slashml-0.0.5/setup.py` & `slashml-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Read the contents of the README file
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="slashml",
-    version="0.0.5",
+    version="0.0.6",
     url="https://slashml.com/",
     author="eff-kay",
     author_email="faiizan14@gmail.com",
     description=(
         "A Python client for interacting with SlashML services" "Developed by SlashML."
     ),
     long_description=long_description,  # Use the contents of the README file
```

### Comparing `slashml-0.0.5/slashml/speech_to_text.py` & `slashml-0.0.6/slashml/text_summarization.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 import requests
+import time
 from enum import Enum
 from .utils import generateURL, baseUrl, generateHeaders, formatResponse, getTaskStatus
 
-
-class SpeechToText:
+class TextSummarization:
     class ServiceProvider(Enum):
-        ASSEMBLY = "assembly"
-        AWS = "aws"
-        WHISPER = "whisper"
+        OPENAI = "openai"
+        HUGGING_FACE = "hugging-face"
 
         @classmethod
         def choices(cls):
             return [key.value for key in cls]
 
-    _base_url = baseUrl("speech-to-text", "v1")
+    _base_url = baseUrl("summarization", "v1")
     _headers = None
 
     def __init__(self, api_key: str = None):
         self._headers = generateHeaders(api_key)
 
-    def upload_audio(self, file_location: str):
-        url = generateURL(self._base_url, "upload")
-        files = [("audio", ("test_audio.mp3", open(file_location, "rb"), "audio/mpeg"))]
-        response = requests.post(url, headers=self._headers, files=files)
-        return formatResponse(response)
-
-    def transcribe(self, upload_url: str, service_provider: ServiceProvider):
+    def submit_job(self, text: str, service_provider: ServiceProvider):
         url = generateURL(self._base_url, "jobs")
-        payload = {
-            "uploaded_audio_url": upload_url,
-            "service_provider": service_provider.value,
-        }
+        payload = {"text": [text], "service_provider": service_provider.value}
         response = requests.post(url, headers=self._headers, data=payload)
         return formatResponse(response)
 
     def status(self, job_id: str, service_provider: ServiceProvider):
         return getTaskStatus(self._base_url, self._headers, job_id, service_provider)
+
+    def execute(self, text: str, service_provider: ServiceProvider):
+        url = generateURL(self._base_url, "jobs")
+        payload = {"text": [text], "service_provider": service_provider.value}
+        response = requests.post(url, headers=self._headers, data=payload)
+        job = formatResponse(response)
+
+        assert job.status != "ERROR", f"{job}"
+        print(f"Got Job ID: {job.id}")
+
+        # check job status
+        response = getTaskStatus(self._base_url, self._headers, job.id, service_provider)
+
+        while response.status == "IN_PROGRESS":
+            time.sleep(5)
+            response = getTaskStatus(self._base_url, self._headers, job.id, service_provider)
+            print(f"Response = {response}. Retrying in 5 seconds")
+        
+        return response
+
```

### Comparing `slashml-0.0.5/slashml/utils.py` & `slashml-0.0.6/slashml/utils.py`

 * *Files identical despite different names*

