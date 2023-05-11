# Comparing `tmp/gpt-convo-reader-0.1.1.tar.gz` & `tmp/gpt-convo-reader-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-convo-reader-0.1.1.tar", last modified: Mon May  8 13:33:32 2023, max compression
+gzip compressed data, was "gpt-convo-reader-0.1.2.tar", last modified: Thu May 11 06:29:24 2023, max compression
```

## Comparing `gpt-convo-reader-0.1.1.tar` & `gpt-convo-reader-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-08 13:33:32.873408 gpt-convo-reader-0.1.1/
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     1072 2023-05-07 14:42:35.000000 gpt-convo-reader-0.1.1/LICENSE
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     2164 2023-05-08 13:33:32.873408 gpt-convo-reader-0.1.1/PKG-INFO
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     1574 2023-05-08 13:33:05.000000 gpt-convo-reader-0.1.1/README.md
--rw-rw-r--   0 romilly   (1000) romilly   (1000)      828 2023-05-08 13:33:32.873408 gpt-convo-reader-0.1.1/setup.cfg
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     1067 2023-05-08 13:33:05.000000 gpt-convo-reader-0.1.1/setup.py
-drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-08 13:33:32.873408 gpt-convo-reader-0.1.1/src/
-drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-08 13:33:32.873408 gpt-convo-reader-0.1.1/src/converter/
--rw-rw-r--   0 romilly   (1000) romilly   (1000)      343 2023-05-08 12:59:31.000000 gpt-convo-reader-0.1.1/src/converter/__init__.py
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     2078 2023-05-07 10:27:12.000000 gpt-convo-reader-0.1.1/src/converter/convert.py
--rwxrwxr-x   0 romilly   (1000) romilly   (1000)     3130 2023-05-08 13:12:58.000000 gpt-convo-reader-0.1.1/src/converter/gui.py
-drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-08 13:33:32.873408 gpt-convo-reader-0.1.1/src/gpt_convo_reader.egg-info/
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     2164 2023-05-08 13:33:32.000000 gpt-convo-reader-0.1.1/src/gpt_convo_reader.egg-info/PKG-INFO
--rw-rw-r--   0 romilly   (1000) romilly   (1000)      374 2023-05-08 13:33:32.000000 gpt-convo-reader-0.1.1/src/gpt_convo_reader.egg-info/SOURCES.txt
--rw-rw-r--   0 romilly   (1000) romilly   (1000)        1 2023-05-08 13:33:32.000000 gpt-convo-reader-0.1.1/src/gpt_convo_reader.egg-info/dependency_links.txt
--rw-rw-r--   0 romilly   (1000) romilly   (1000)       51 2023-05-08 13:33:32.000000 gpt-convo-reader-0.1.1/src/gpt_convo_reader.egg-info/entry_points.txt
--rw-rw-r--   0 romilly   (1000) romilly   (1000)       15 2023-05-08 13:33:32.000000 gpt-convo-reader-0.1.1/src/gpt_convo_reader.egg-info/requires.txt
--rw-rw-r--   0 romilly   (1000) romilly   (1000)       10 2023-05-08 13:33:32.000000 gpt-convo-reader-0.1.1/src/gpt_convo_reader.egg-info/top_level.txt
+drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-11 06:29:24.739875 gpt-convo-reader-0.1.2/
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     1072 2023-05-07 14:42:35.000000 gpt-convo-reader-0.1.2/LICENSE
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     2164 2023-05-11 06:29:24.739875 gpt-convo-reader-0.1.2/PKG-INFO
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     1574 2023-05-08 13:33:05.000000 gpt-convo-reader-0.1.2/README.md
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)      828 2023-05-11 06:29:24.739875 gpt-convo-reader-0.1.2/setup.cfg
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     1067 2023-05-11 06:29:05.000000 gpt-convo-reader-0.1.2/setup.py
+drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-11 06:29:24.667876 gpt-convo-reader-0.1.2/src/
+drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-11 06:29:24.719875 gpt-convo-reader-0.1.2/src/converter/
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)      343 2023-05-08 12:59:31.000000 gpt-convo-reader-0.1.2/src/converter/__init__.py
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     2078 2023-05-07 10:27:12.000000 gpt-convo-reader-0.1.2/src/converter/convert.py
+-rwxrwxr-x   0 romilly   (1000) romilly   (1000)     3328 2023-05-11 06:28:24.000000 gpt-convo-reader-0.1.2/src/converter/gui.py
+drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-11 06:29:24.739875 gpt-convo-reader-0.1.2/src/gpt_convo_reader.egg-info/
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     2164 2023-05-11 06:29:24.000000 gpt-convo-reader-0.1.2/src/gpt_convo_reader.egg-info/PKG-INFO
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)      374 2023-05-11 06:29:24.000000 gpt-convo-reader-0.1.2/src/gpt_convo_reader.egg-info/SOURCES.txt
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)        1 2023-05-11 06:29:24.000000 gpt-convo-reader-0.1.2/src/gpt_convo_reader.egg-info/dependency_links.txt
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)       51 2023-05-11 06:29:24.000000 gpt-convo-reader-0.1.2/src/gpt_convo_reader.egg-info/entry_points.txt
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)       15 2023-05-11 06:29:24.000000 gpt-convo-reader-0.1.2/src/gpt_convo_reader.egg-info/requires.txt
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)       10 2023-05-11 06:29:24.000000 gpt-convo-reader-0.1.2/src/gpt_convo_reader.egg-info/top_level.txt
```

### Comparing `gpt-convo-reader-0.1.1/LICENSE` & `gpt-convo-reader-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-convo-reader-0.1.1/PKG-INFO` & `gpt-convo-reader-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-convo-reader
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lets you find, view and format the conversations you've had with ChatGPT in the playground.
 Home-page: https://github.com/romilly/gpt-convo-reader
 Author: Romilly Cocking
 Author-email: romilly.cocking@gmail.com
 Project-URL: Bug Tracker, https://github.com/romilly/gpt-convo-reader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gpt-convo-reader-0.1.1/README.md` & `gpt-convo-reader-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gpt-convo-reader-0.1.1/setup.cfg` & `gpt-convo-reader-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `gpt-convo-reader-0.1.1/setup.py` & `gpt-convo-reader-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gpt-convo-reader",
-    version="0.1.1",
+    version="0.1.2",
     author="Romilly Cocking",
     author_email="romilly.cocking@gmail.com",
     description="Lets you find, view and format the conversations you've had with ChatGPT in the playground.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/romilly/gpt-convo-reader",
     project_urls={
```

### Comparing `gpt-convo-reader-0.1.1/src/converter/convert.py` & `gpt-convo-reader-0.1.2/src/converter/convert.py`

 * *Files identical despite different names*

### Comparing `gpt-convo-reader-0.1.1/src/converter/gui.py` & `gpt-convo-reader-0.1.2/src/converter/gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # coding: utf-8
-
+import os.path
 from configparser import ConfigParser
 from guizero import App, ListBox, TextBox, TitleBox, MenuBar
 
 from converter.convert import convert
 
 
 class ConversationGUI(App):
@@ -23,19 +23,25 @@
         # Create a ListBox to display the conversation titles
         self.conversation_list = ListBox(self.conversation_box, command=self.show_conversation, width = 'fill')
         # Create a TextBox to display the conversation messages
         self.conversation_text = TextBox(self.conversation_box, multiline=True, scrollbar=True, width= 'fill', height='fill')
 
     def get_default_directories(self):
         config = ConfigParser()
-        config.read('convert.ini')
-        zip_folder = config['default directory locations']['zip directory']
-        save_folder = config['default directory locations']['save directory']
+        if os.path.exists('convert.ini'):
+            config.read('convert.ini')
+            zip_folder = config['default directory locations']['zip directory']
+            save_folder = config['default directory locations']['save directory']
+        else:
+            zip_folder = '.'
+            save_folder = '.'
+            print('using current directory as default')
         return zip_folder, save_folder
 
+
     def show_conversation(self):
         # Get the selected conversation from the ListBox
         title = self.conversation_list.value
         # Get the conversation object from the dictionary
         self.selected_conversation = self.conversations[title]
         # Clear the TextBox
         self.conversation_text.clear()
```

### Comparing `gpt-convo-reader-0.1.1/src/gpt_convo_reader.egg-info/PKG-INFO` & `gpt-convo-reader-0.1.2/src/gpt_convo_reader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-convo-reader
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lets you find, view and format the conversations you've had with ChatGPT in the playground.
 Home-page: https://github.com/romilly/gpt-convo-reader
 Author: Romilly Cocking
 Author-email: romilly.cocking@gmail.com
 Project-URL: Bug Tracker, https://github.com/romilly/gpt-convo-reader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

