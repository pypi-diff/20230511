# Comparing `tmp/tts_arranger-0.3.4.tar.gz` & `tmp/tts_arranger-0.3.5.tar.gz`

## Comparing `tts_arranger-0.3.4.tar` & `tts_arranger-0.3.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/requirements.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/__init__.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/tts_abstract_writer.py
--rw-r--r--   0        0        0    12785 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/tts_html_converter.py
--rw-r--r--   0        0        0    24654 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/tts_processor.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/tts_simple_writer.py
--rw-r--r--   0        0        0    17440 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/tts_writer.py
--rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/data/checkers_default.json
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/data/exclude_ids.json
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/data/replace.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/data/replace_de.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/data/replace_en.json
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/examples/tts_project_example.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/examples/tts_simple_example.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/items/__init__.py
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/items/tts_chapter.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/items/tts_item.py
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/items/tts_project.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/tts_reader/__init__.py
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/tts_reader/checker.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/tts_reader/tts_abstract_reader.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/tts_reader/tts_epub_reader.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/tts_reader/tts_html_based_reader.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/tts_reader/tts_html_reader.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/tts_reader/tts_srt_reader.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/tts_reader/tts_text_reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/utils/__init__.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/src/tts_arranger/utils/log.py
--rw-r--r--   0        0        0    11217 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/tests/reader_test.py
--rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/tests/tts_arranger_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/LICENSE
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/README.md
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 tts_arranger-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/requirements.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/__init__.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/tts_abstract_writer.py
+-rw-r--r--   0        0        0    12785 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/tts_html_converter.py
+-rw-r--r--   0        0        0    24654 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/tts_processor.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/tts_simple_writer.py
+-rw-r--r--   0        0        0    17525 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/tts_writer.py
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/data/checkers_default.json
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/data/exclude_ids.json
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/data/replace.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/data/replace_de.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/data/replace_en.json
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/examples/tts_project_example.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/examples/tts_simple_example.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/items/__init__.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/items/tts_chapter.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/items/tts_item.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/items/tts_project.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/tts_reader/__init__.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/tts_reader/checker.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/tts_reader/tts_abstract_reader.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/tts_reader/tts_epub_reader.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/tts_reader/tts_html_based_reader.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/tts_reader/tts_html_reader.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/tts_reader/tts_srt_reader.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/tts_reader/tts_text_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/utils/__init__.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/src/tts_arranger/utils/log.py
+-rw-r--r--   0        0        0    11217 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/tests/reader_test.py
+-rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/tests/tts_arranger_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/LICENSE
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/README.md
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 tts_arranger-0.3.5/PKG-INFO
```

### Comparing `tts_arranger-0.3.4/src/tts_arranger/tts_abstract_writer.py` & `tts_arranger-0.3.5/src/tts_arranger/tts_abstract_writer.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/src/tts_arranger/tts_html_converter.py` & `tts_arranger-0.3.5/src/tts_arranger/tts_html_converter.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/src/tts_arranger/tts_processor.py` & `tts_arranger-0.3.5/src/tts_arranger/tts_processor.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/src/tts_arranger/tts_simple_writer.py` & `tts_arranger-0.3.5/src/tts_arranger/tts_simple_writer.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/src/tts_arranger/tts_writer.py` & `tts_arranger-0.3.5/src/tts_arranger/tts_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,17 +265,19 @@
         """
 
         if not self.project.tts_chapters:
             log(LOG_TYPE.ERROR, f'No chapters to synthesize, exiting.')
             return
 
         # Make sure the prefix exists
-        os.makedirs(temp_dir_prefix)
+        if temp_dir_prefix:
+            if not os.path.exists(temp_dir_prefix):
+                os.makedirs(temp_dir_prefix)
 
-        with tempfile.TemporaryDirectory(prefix=temp_dir_prefix) as temp_dir:
+        with tempfile.TemporaryDirectory(dir=temp_dir_prefix) as temp_dir:
             try:
                 log(LOG_TYPE.INFO, f'Synthesizing project "{self.project.title}".')
 
                 if self.model and self.vocoder:
                     t = TTS_Processor(self.model, self.vocoder, self.preferred_speakers)
                 else:
                     match self.project.lang_code:
```

### Comparing `tts_arranger-0.3.4/src/tts_arranger/data/checkers_default.json` & `tts_arranger-0.3.5/src/tts_arranger/data/checkers_default.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/src/tts_arranger/examples/tts_project_example.py` & `tts_arranger-0.3.5/src/tts_arranger/examples/tts_project_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 # Prepare the project file
 project = TTS_Project(chapter, 'Project title', 'This is a subtitle', author='Some author')
 project.add_image_from_url('https://coqui.ai/static/38a06ec53309f617be3eb3b8b9367abf/598c3/logo-wordmark.png')  # Add a cover image
 
 # Finally synthesize and write the project as a m4b audiobook using our preferred speakers
 writer = TTS_Writer(project, os.path.join(user_dir, 'tts_arranger_example_output/'), preferred_speakers=preferred_speakers)
-writer.synthesize_and_write(project.author + ' - ' + project.title)
+writer.synthesize_and_write(project.author + ' - ' + project.title, temp_dir_prefix='/tmp/the_test')
 
 # German example using Thorsten voice (no multispeaker support), output as mp3, writing one mp3 file per chapter
 
 items1 = []
 items1.append(TTS_Item('Dies ist ein Test.'))
 items1.append(TTS_Item('Noch ein Test.'))
```

### Comparing `tts_arranger-0.3.4/src/tts_arranger/examples/tts_simple_example.py` & `tts_arranger-0.3.5/src/tts_arranger/examples/tts_simple_example.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/src/tts_arranger/items/tts_chapter.py` & `tts_arranger-0.3.5/src/tts_arranger/items/tts_chapter.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/src/tts_arranger/items/tts_item.py` & `tts_arranger-0.3.5/src/tts_arranger/items/tts_item.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/src/tts_arranger/items/tts_project.py` & `tts_arranger-0.3.5/src/tts_arranger/items/tts_project.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/src/tts_arranger/tts_reader/checker.py` & `tts_arranger-0.3.5/src/tts_arranger/tts_reader/checker.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/src/tts_arranger/tts_reader/tts_abstract_reader.py` & `tts_arranger-0.3.5/src/tts_arranger/tts_reader/tts_abstract_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/src/tts_arranger/tts_reader/tts_epub_reader.py` & `tts_arranger-0.3.5/src/tts_arranger/tts_reader/tts_epub_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/src/tts_arranger/tts_reader/tts_html_based_reader.py` & `tts_arranger-0.3.5/src/tts_arranger/tts_reader/tts_html_based_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/src/tts_arranger/tts_reader/tts_html_reader.py` & `tts_arranger-0.3.5/src/tts_arranger/tts_reader/tts_html_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/src/tts_arranger/tts_reader/tts_srt_reader.py` & `tts_arranger-0.3.5/src/tts_arranger/tts_reader/tts_srt_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/src/tts_arranger/tts_reader/tts_text_reader.py` & `tts_arranger-0.3.5/src/tts_arranger/tts_reader/tts_text_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/src/tts_arranger/utils/log.py` & `tts_arranger-0.3.5/src/tts_arranger/utils/log.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/tests/reader_test.py` & `tts_arranger-0.3.5/tests/reader_test.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/tests/tts_arranger_test.py` & `tts_arranger-0.3.5/tests/tts_arranger_test.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/LICENSE` & `tts_arranger-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/README.md` & `tts_arranger-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.4/pyproject.toml` & `tts_arranger-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   "Operating System :: OS Independent",
 ]
 description = "Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS"
 dynamic = ["dependencies"]
 name = "tts_arranger"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.3.4"
+version = "0.3.5"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/knochenhans/tts_arranger/issues"
 "Homepage" = "https://github.com/knochenhans/tts_arranger"
 
 [tool.hatch.build]
 exclude = [
```

### Comparing `tts_arranger-0.3.4/PKG-INFO` & `tts_arranger-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tts_arranger
-Version: 0.3.4
+Version: 0.3.5
 Summary: Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS
 Project-URL: Bug Tracker, https://github.com/knochenhans/tts_arranger/issues
 Project-URL: Homepage, https://github.com/knochenhans/tts_arranger
 Author-email: Andre Jonas <nipsky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

