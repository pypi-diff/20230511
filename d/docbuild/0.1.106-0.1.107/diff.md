# Comparing `tmp/docbuild-0.1.106.tar.gz` & `tmp/docbuild-0.1.107.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docbuild-0.1.106.tar", last modified: Mon May  8 09:08:18 2023, max compression
+gzip compressed data, was "docbuild-0.1.107.tar", last modified: Thu May 11 14:33:03 2023, max compression
```

## Comparing `docbuild-0.1.106.tar` & `docbuild-0.1.107.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-08 09:08:18.401326 docbuild-0.1.106/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-05-08 09:08:18.401112 docbuild-0.1.106/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.106/README.md
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-08 09:08:18.394006 docbuild-0.1.106/docbuild/
--rw-r--r--   0 moran      (501) staff       (20)       63 2023-05-08 09:07:48.000000 docbuild-0.1.106/docbuild/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      439 2023-04-20 11:04:19.000000 docbuild-0.1.106/docbuild/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     5392 2023-04-19 07:35:54.000000 docbuild-0.1.106/docbuild/graph.py
--rw-r--r--   0 moran      (501) staff       (20)     4478 2023-04-19 09:10:05.000000 docbuild-0.1.106/docbuild/hocr_parser.py
--rw-r--r--   0 moran      (501) staff       (20)     7054 2023-04-29 18:09:32.000000 docbuild-0.1.106/docbuild/page_creator.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-08 09:08:18.398018 docbuild-0.1.106/docbuild/paragraph_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.106/docbuild/paragraph_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.106/docbuild/paragraph_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     6831 2023-04-20 11:03:50.000000 docbuild-0.1.106/docbuild/paragraph_detection/paragraph_extractor.py
--rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.106/docbuild/paragraph_detection/paragraph_sorter.py
--rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.106/docbuild/paragraph_detection/two_columns.py
--rw-r--r--   0 moran      (501) staff       (20)     6087 2023-05-08 09:07:21.000000 docbuild-0.1.106/docbuild/textract_parser.py
--rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.106/docbuild/utils.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-08 09:08:18.400138 docbuild-0.1.106/docbuild/visual_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.106/docbuild/visual_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)    12923 2023-04-30 11:56:34.000000 docbuild-0.1.106/docbuild/visual_detection/bordered_table_extraction.py
--rw-r--r--   0 moran      (501) staff       (20)      218 2023-04-30 11:54:41.000000 docbuild-0.1.106/docbuild/visual_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)    16325 2023-04-30 05:58:58.000000 docbuild-0.1.106/docbuild/visual_detection/vis_line_detection.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-08 09:08:18.396395 docbuild-0.1.106/docbuild.egg-info/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-05-08 09:08:18.000000 docbuild-0.1.106/docbuild.egg-info/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)      741 2023-05-08 09:08:18.000000 docbuild-0.1.106/docbuild.egg-info/SOURCES.txt
--rw-r--r--   0 moran      (501) staff       (20)        1 2023-05-08 09:08:18.000000 docbuild-0.1.106/docbuild.egg-info/dependency_links.txt
--rw-r--r--   0 moran      (501) staff       (20)       83 2023-05-08 09:08:18.000000 docbuild-0.1.106/docbuild.egg-info/requires.txt
--rw-r--r--   0 moran      (501) staff       (20)        9 2023-05-08 09:08:18.000000 docbuild-0.1.106/docbuild.egg-info/top_level.txt
--rw-r--r--   0 moran      (501) staff       (20)       38 2023-05-08 09:08:18.401377 docbuild-0.1.106/setup.cfg
--rw-r--r--   0 moran      (501) staff       (20)      832 2023-05-08 09:08:02.000000 docbuild-0.1.106/setup.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-11 14:33:03.684638 docbuild-0.1.107/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-05-11 14:33:03.684442 docbuild-0.1.107/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.107/README.md
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-11 14:33:03.680322 docbuild-0.1.107/docbuild/
+-rw-r--r--   0 moran      (501) staff       (20)       63 2023-05-11 14:32:02.000000 docbuild-0.1.107/docbuild/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      439 2023-04-20 11:04:19.000000 docbuild-0.1.107/docbuild/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     5392 2023-04-19 07:35:54.000000 docbuild-0.1.107/docbuild/graph.py
+-rw-r--r--   0 moran      (501) staff       (20)     4478 2023-04-19 09:10:05.000000 docbuild-0.1.107/docbuild/hocr_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)     7055 2023-05-11 14:28:20.000000 docbuild-0.1.107/docbuild/page_creator.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-11 14:33:03.682676 docbuild-0.1.107/docbuild/paragraph_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.107/docbuild/paragraph_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.107/docbuild/paragraph_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     6831 2023-04-20 11:03:50.000000 docbuild-0.1.107/docbuild/paragraph_detection/paragraph_extractor.py
+-rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.107/docbuild/paragraph_detection/paragraph_sorter.py
+-rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.107/docbuild/paragraph_detection/two_columns.py
+-rw-r--r--   0 moran      (501) staff       (20)     6087 2023-05-08 09:07:21.000000 docbuild-0.1.107/docbuild/textract_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.107/docbuild/utils.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-11 14:33:03.683932 docbuild-0.1.107/docbuild/visual_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.107/docbuild/visual_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)    12923 2023-05-09 11:47:03.000000 docbuild-0.1.107/docbuild/visual_detection/bordered_table_extraction.py
+-rw-r--r--   0 moran      (501) staff       (20)      218 2023-04-30 11:54:41.000000 docbuild-0.1.107/docbuild/visual_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)    16349 2023-05-11 14:30:30.000000 docbuild-0.1.107/docbuild/visual_detection/vis_line_detection.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-11 14:33:03.681321 docbuild-0.1.107/docbuild.egg-info/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-05-11 14:33:03.000000 docbuild-0.1.107/docbuild.egg-info/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)      741 2023-05-11 14:33:03.000000 docbuild-0.1.107/docbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 moran      (501) staff       (20)        1 2023-05-11 14:33:03.000000 docbuild-0.1.107/docbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 moran      (501) staff       (20)       97 2023-05-11 14:33:03.000000 docbuild-0.1.107/docbuild.egg-info/requires.txt
+-rw-r--r--   0 moran      (501) staff       (20)        9 2023-05-11 14:33:03.000000 docbuild-0.1.107/docbuild.egg-info/top_level.txt
+-rw-r--r--   0 moran      (501) staff       (20)       38 2023-05-11 14:33:03.684687 docbuild-0.1.107/setup.cfg
+-rw-r--r--   0 moran      (501) staff       (20)      856 2023-05-11 14:31:56.000000 docbuild-0.1.107/setup.py
```

### Comparing `docbuild-0.1.106/PKG-INFO` & `docbuild-0.1.107/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.106
+Version: 0.1.107
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.106/docbuild/graph.py` & `docbuild-0.1.107/docbuild/graph.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.106/docbuild/hocr_parser.py` & `docbuild-0.1.107/docbuild/hocr_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.106/docbuild/page_creator.py` & `docbuild-0.1.107/docbuild/page_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             group_words.append(words[start : i + 1])
             start = i + 1
         group_words.append(words[start:])
         return [Line(children=group) for group in group_words]
 
     def get_tables(self, words: list[Word]) -> list[Table]:
         try:
-            avg_word_size_ver = get_average_character_height(words)
+            avg_word_size_ver = get_average_character_height(words) 
             avg_word_size_hor = (
                 avg_word_size_ver * self.image_height / self.image_width
             )
             image_length_threshold = int(avg_word_size_ver * self.image_height)
             
             ver_threshold = avg_word_size_ver
             hor_threshold = avg_word_size_hor
```

### Comparing `docbuild-0.1.106/docbuild/paragraph_detection/paragraph_extractor.py` & `docbuild-0.1.107/docbuild/paragraph_detection/paragraph_extractor.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.106/docbuild/paragraph_detection/paragraph_sorter.py` & `docbuild-0.1.107/docbuild/paragraph_detection/paragraph_sorter.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.106/docbuild/paragraph_detection/two_columns.py` & `docbuild-0.1.107/docbuild/paragraph_detection/two_columns.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.106/docbuild/textract_parser.py` & `docbuild-0.1.107/docbuild/textract_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.106/docbuild/utils.py` & `docbuild-0.1.107/docbuild/utils.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.106/docbuild/visual_detection/bordered_table_extraction.py` & `docbuild-0.1.107/docbuild/visual_detection/bordered_table_extraction.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.106/docbuild/visual_detection/vis_line_detection.py` & `docbuild-0.1.107/docbuild/visual_detection/vis_line_detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,28 +421,28 @@
         line_remover = VisLineRemover(lines=hor_lines + ver_lines, words=self.words)
 
         hor_lines, ver_lines = line_remover.remove_lines()
         if self.debug:
             self.remover_drawer.draw_vis_lines(hor_lines + ver_lines, random_color=True)
             self.remover_drawer.save(os.path.join(self.folder, "remover_lines.jpg"))
 
-        hor_line_merger = VisLineMerger(hor_lines, hor_threshold)
+        hor_line_merger = VisLineMerger(hor_lines, hor_threshold / 2)
         merged_hor_lines = hor_line_merger.merge_lines()
-        ver_line_merger = VisLineMerger(ver_lines, ver_threshold)
+        ver_line_merger = VisLineMerger(ver_lines, ver_threshold / 2)
         merged_ver_lines = ver_line_merger.merge_lines()
-
+        
         if self.debug:
             self.merge_drawer.draw_vis_lines(
                 merged_hor_lines + merged_ver_lines, random_color=True
             )
             self.merge_drawer.save(os.path.join(self.folder, "merge_lines.jpg"))
 
-        line_extension = VisLineExtension(merged_hor_lines, hor_threshold)
+        line_extension = VisLineExtension(merged_hor_lines, hor_threshold / 2)
         line_extension.extend_lines()
-        line_extension = VisLineExtension(merged_ver_lines, ver_threshold)
+        line_extension = VisLineExtension(merged_ver_lines, ver_threshold / 2)
 
         hor_ver_vis_lines = HorVerVisLines(merged_hor_lines, merged_ver_lines)
         return hor_ver_vis_lines
 
     def hor_preprocess(self, image: np.ndarray) -> np.ndarray:
         image = cv2.filter2D(image, -1, self.hor_kernel)
         return image
```

### Comparing `docbuild-0.1.106/docbuild.egg-info/PKG-INFO` & `docbuild-0.1.107/docbuild.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.106
+Version: 0.1.107
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.106/docbuild.egg-info/SOURCES.txt` & `docbuild-0.1.107/docbuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.106/setup.py` & `docbuild-0.1.107/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name="docbuild",
-    version="0.1.106",
+    version="0.1.107",
     description="A package for building a document from a textract response, for more information see the docstruct package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Moran Nechushtan, Serah Tapia, Shlomo Agishtein",
     author_email="moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com",
     url="https://github.com/smrt-co/docbuild",
     packages=setuptools.find_packages(),
     install_requires=[
         "attrs>=22.0.0",
         "numpy==1.23.2",
         "beautifulsoup4>=4.11.1",
         "opencv-contrib-python==4.6.0.66",
+        "python-dotenv"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
 )
```

