# Comparing `tmp/bardapi-0.1.1.tar.gz` & `tmp/bardapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bardapi-0.1.1.tar", last modified: Thu May 11 17:40:49 2023, max compression
+gzip compressed data, was "bardapi-0.1.2.tar", last modified: Thu May 11 19:19:55 2023, max compression
```

## Comparing `bardapi-0.1.1.tar` & `bardapi-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 17:40:49.826256 bardapi-0.1.1/
--rw-rw-rw-   0        0        0     2352 2023-05-11 17:40:49.824757 bardapi-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1451 2023-05-11 17:40:13.000000 bardapi-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 17:40:49.807428 bardapi-0.1.1/bardapi/
--rw-rw-rw-   0        0        0      194 2023-05-11 17:40:43.000000 bardapi-0.1.1/bardapi/__init__.py
--rw-rw-rw-   0        0        0     2807 2023-05-11 17:07:14.000000 bardapi-0.1.1/bardapi/core.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:40:49.822239 bardapi-0.1.1/bardapi.egg-info/
--rw-rw-rw-   0        0        0     2352 2023-05-11 17:40:49.000000 bardapi-0.1.1/bardapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-05-11 17:40:49.000000 bardapi-0.1.1/bardapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 17:40:49.000000 bardapi-0.1.1/bardapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-11 17:40:49.000000 bardapi-0.1.1/bardapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-05-11 17:40:49.000000 bardapi-0.1.1/bardapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 17:40:49.826256 bardapi-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1753 2023-05-11 17:40:30.000000 bardapi-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 19:19:55.149331 bardapi-0.1.2/
+-rw-rw-rw-   0        0        0     3538 2023-05-11 19:19:55.147848 bardapi-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2637 2023-05-11 19:19:14.000000 bardapi-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 19:19:55.126198 bardapi-0.1.2/bardapi/
+-rw-rw-rw-   0        0        0      198 2023-05-11 19:19:42.000000 bardapi-0.1.2/bardapi/__init__.py
+-rw-rw-rw-   0        0        0     2809 2023-05-11 19:18:58.000000 bardapi-0.1.2/bardapi/core.py
+drwxrwxrwx   0        0        0        0 2023-05-11 19:19:55.144693 bardapi-0.1.2/bardapi.egg-info/
+-rw-rw-rw-   0        0        0     3538 2023-05-11 19:19:55.000000 bardapi-0.1.2/bardapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-05-11 19:19:55.000000 bardapi-0.1.2/bardapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 19:19:55.000000 bardapi-0.1.2/bardapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-11 19:19:55.000000 bardapi-0.1.2/bardapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-05-11 19:19:55.000000 bardapi-0.1.2/bardapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 19:19:55.149331 bardapi-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1747 2023-05-11 19:19:39.000000 bardapi-0.1.2/setup.py
```

### Comparing `bardapi-0.1.1/bardapi/core.py` & `bardapi-0.1.2/bardapi/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,27 +27,27 @@
 
     def _get_snim0e(self):
         resp = self.session.get(url="https://bard.google.com/", timeout=5)
         if resp.status_code != 200:
             raise Exception(f"Response Status: {resp.status_code}")
         return re.search(r"SNlM0e\":\"(.*?)\"", resp.text).group(1)
 
-    def get_answer(self, question: str) -> dict:
+    def get_answer(self, input_text: str) -> dict:
         params = {
             "bl": "boq_assistant-bard-web-server_20230419.00_p1",
             "_reqid": str(self._reqid),
             "rt": "c",
         }
-        question_struct = [
-            [question],
+        input_text_struct = [
+            [input_text],
             None,
             [self.conversation_id, self.response_id, self.choice_id],
         ]
         data = {
-            "f.req": json.dumps([None, json.dumps(question_struct)]),
+            "f.req": json.dumps([None, json.dumps(input_text_struct)]),
             "at": self.SNlM0e,
         }
         resp = self.session.post(
             "https://bard.google.com/_/BardChatUi/data/assistant.lamda.BardFrontendService/StreamGenerate",
             params=params,
             data=data,
             timeout=100,
@@ -67,8 +67,7 @@
         }
         self.conversation_id = bard_answer["conversation_id"]
         self.response_id = bard_answer["response_id"]
         self.choice_id = bard_answer["choices"][0]["id"]
         self._reqid += 100000
 
         return bard_answer
-
```

### Comparing `bardapi-0.1.1/setup.py` & `bardapi-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,25 +21,24 @@
 
 
 version = get_version()
 
 
 setup(
     name="bardapi",
-    version="0.1.1",
+    version="0.1.2",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="A package that returns Response of Google BARD through API.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/BARD_API",
     packages=find_packages(exclude=[]),
     python_requires=">=3.6",
-    install_requires=[
-    ],
+    install_requires=[],
     keywords="BARD, Python, Google Bard, Large Language Model, Chatbot API, Google API, Chatbot",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
```

