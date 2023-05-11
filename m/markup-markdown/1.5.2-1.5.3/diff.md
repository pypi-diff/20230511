# Comparing `tmp/markup-markdown-1.5.2.tar.gz` & `tmp/markup-markdown-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/markup-markdown-1.5.2.tar", last modified: Tue Mar 28 07:23:59 2023, max compression
+gzip compressed data, was "dist/markup-markdown-1.5.3.tar", last modified: Thu May 11 01:27:16 2023, max compression
```

## Comparing `markup-markdown-1.5.2.tar` & `markup-markdown-1.5.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 hai       (1000) hai       (1000)        0 2023-03-28 07:23:59.000000 markup-markdown-1.5.2/
--rwxrwxrwx   0 hai       (1000) hai       (1000)     1078 2023-03-03 10:00:42.000000 markup-markdown-1.5.2/LICENSE
--rwxrwxrwx   0 hai       (1000) hai       (1000)       24 2023-03-03 10:00:42.000000 markup-markdown-1.5.2/MANIFEST.in
--rw-r--r--   0 hai       (1000) hai       (1000)      757 2023-03-28 07:23:59.000000 markup-markdown-1.5.2/PKG-INFO
--rwxrwxrwx   0 hai       (1000) hai       (1000)    15023 2023-03-28 07:12:45.000000 markup-markdown-1.5.2/README.md
-drwxr-xr-x   0 hai       (1000) hai       (1000)        0 2023-03-28 07:23:59.000000 markup-markdown-1.5.2/markup/
--rwxr-xr-x   0 hai       (1000) hai       (1000)     4237 2023-03-27 01:06:24.000000 markup-markdown-1.5.2/markup/Headings.py
--rwxrwxrwx   0 hai       (1000) hai       (1000)     1097 2023-03-03 10:05:06.000000 markup-markdown-1.5.2/markup/MarkdownPP.py
--rwxrwxrwx   0 hai       (1000) hai       (1000)      362 2023-03-03 10:30:10.000000 markup-markdown-1.5.2/markup/Markers.py
--rwxrwxrwx   0 hai       (1000) hai       (1000)      906 2023-03-03 10:05:06.000000 markup-markdown-1.5.2/markup/Module.py
-drwxr-xr-x   0 hai       (1000) hai       (1000)        0 2023-03-28 07:23:59.000000 markup-markdown-1.5.2/markup/Modules/
--rwxrwxrwx   0 hai       (1000) hai       (1000)      798 2023-03-03 10:05:06.000000 markup-markdown-1.5.2/markup/Modules/BlankLine.py
--rwxr-xr-x   0 hai       (1000) hai       (1000)     2483 2023-03-28 07:16:49.000000 markup-markdown-1.5.2/markup/Modules/EnvVariableReplacements.py
--rwxrwxrwx   0 hai       (1000) hai       (1000)    10716 2023-03-04 11:36:46.000000 markup-markdown-1.5.2/markup/Modules/Include.py
--rwxrwxrwx   0 hai       (1000) hai       (1000)     2302 2023-03-03 10:00:42.000000 markup-markdown-1.5.2/markup/Modules/IncludeCode.py
--rwxrwxrwx   0 hai       (1000) hai       (1000)     1821 2023-03-03 10:05:07.000000 markup-markdown-1.5.2/markup/Modules/IncludeURL.py
--rwxr-xr-x   0 hai       (1000) hai       (1000)     1801 2023-03-28 04:54:10.000000 markup-markdown-1.5.2/markup/Modules/IncludeWikilinkImage.py
--rwxrwxrwx   0 hai       (1000) hai       (1000)     1812 2023-03-03 10:00:42.000000 markup-markdown-1.5.2/markup/Modules/Reference.py
--rwxrwxrwx   0 hai       (1000) hai       (1000)     1318 2023-03-03 10:00:42.000000 markup-markdown-1.5.2/markup/Modules/SkipBlocks.py
--rwxr-xr-x   0 hai       (1000) hai       (1000)     1874 2023-03-03 11:05:48.000000 markup-markdown-1.5.2/markup/Modules/SkipHeaderMetadata.py
--rwxrwxrwx   0 hai       (1000) hai       (1000)      856 2023-03-03 10:05:07.000000 markup-markdown-1.5.2/markup/Modules/SkipLine.py
--rwxr-xr-x   0 hai       (1000) hai       (1000)     1136 2023-03-05 05:56:26.000000 markup-markdown-1.5.2/markup/Modules/SkipObsidianComments.py
--rwxrwxrwx   0 hai       (1000) hai       (1000)    14688 2023-03-13 08:25:14.000000 markup-markdown-1.5.2/markup/Modules/TableOfContents.py
--rwxrwxrwx   0 hai       (1000) hai       (1000)     1009 2023-03-03 10:05:08.000000 markup-markdown-1.5.2/markup/Modules/WordPageBreak.py
--rwxrwxrwx   0 hai       (1000) hai       (1000)     4095 2023-03-03 10:00:42.000000 markup-markdown-1.5.2/markup/Modules/YoutubeEmbed.py
--rwxrwxrwx   0 hai       (1000) hai       (1000)      864 2023-03-03 10:00:42.000000 markup-markdown-1.5.2/markup/Modules/__init__.py
--rw-r--r--   0 hai       (1000) hai       (1000)     9182 2023-03-27 07:09:21.000000 markup-markdown-1.5.2/markup/ObCanvas.py
--rwxrwxrwx   0 hai       (1000) hai       (1000)     2682 2023-03-03 10:37:36.000000 markup-markdown-1.5.2/markup/Processor.py
--rwxrwxrwx   0 hai       (1000) hai       (1000)      847 2023-03-03 10:00:42.000000 markup-markdown-1.5.2/markup/Transform.py
--rwxrwxrwx   0 hai       (1000) hai       (1000)      343 2023-03-03 10:00:42.000000 markup-markdown-1.5.2/markup/__init__.py
--rwxrwxrwx   0 hai       (1000) hai       (1000)     7217 2023-03-27 06:10:49.000000 markup-markdown-1.5.2/markup/main.py
-drwxr-xr-x   0 hai       (1000) hai       (1000)        0 2023-03-28 07:23:59.000000 markup-markdown-1.5.2/markup_markdown.egg-info/
--rw-r--r--   0 hai       (1000) hai       (1000)      757 2023-03-28 07:23:58.000000 markup-markdown-1.5.2/markup_markdown.egg-info/PKG-INFO
--rw-r--r--   0 hai       (1000) hai       (1000)      952 2023-03-28 07:23:58.000000 markup-markdown-1.5.2/markup_markdown.egg-info/SOURCES.txt
--rw-r--r--   0 hai       (1000) hai       (1000)        1 2023-03-28 07:23:58.000000 markup-markdown-1.5.2/markup_markdown.egg-info/dependency_links.txt
--rw-r--r--   0 hai       (1000) hai       (1000)      151 2023-03-28 07:23:58.000000 markup-markdown-1.5.2/markup_markdown.egg-info/entry_points.txt
--rw-r--r--   0 hai       (1000) hai       (1000)       30 2023-03-28 07:23:58.000000 markup-markdown-1.5.2/markup_markdown.egg-info/requires.txt
--rw-r--r--   0 hai       (1000) hai       (1000)       22 2023-03-28 07:23:58.000000 markup-markdown-1.5.2/markup_markdown.egg-info/top_level.txt
--rw-r--r--   0 hai       (1000) hai       (1000)       38 2023-03-28 07:23:59.000000 markup-markdown-1.5.2/setup.cfg
--rwxrwxrwx   0 hai       (1000) hai       (1000)     1263 2023-03-28 07:17:20.000000 markup-markdown-1.5.2/setup.py
-drwxr-xr-x   0 hai       (1000) hai       (1000)        0 2023-03-28 07:23:59.000000 markup-markdown-1.5.2/test/
--rwxrwxrwx   0 hai       (1000) hai       (1000)    13382 2023-03-03 10:16:24.000000 markup-markdown-1.5.2/test/test.py
+drwxr-xr-x   0 hai       (1000) hai       (1000)        0 2023-05-11 01:27:16.000000 markup-markdown-1.5.3/
+-rwxrwxrwx   0 hai       (1000) hai       (1000)     1078 2023-03-03 10:00:42.000000 markup-markdown-1.5.3/LICENSE
+-rwxrwxrwx   0 hai       (1000) hai       (1000)       24 2023-03-03 10:00:42.000000 markup-markdown-1.5.3/MANIFEST.in
+-rw-r--r--   0 hai       (1000) hai       (1000)      757 2023-05-11 01:27:16.000000 markup-markdown-1.5.3/PKG-INFO
+-rwxrwxrwx   0 hai       (1000) hai       (1000)    15023 2023-03-28 07:12:45.000000 markup-markdown-1.5.3/README.md
+drwxr-xr-x   0 hai       (1000) hai       (1000)        0 2023-05-11 01:27:15.000000 markup-markdown-1.5.3/markup/
+-rwxr-xr-x   0 hai       (1000) hai       (1000)     4237 2023-03-27 01:06:24.000000 markup-markdown-1.5.3/markup/Headings.py
+-rwxrwxrwx   0 hai       (1000) hai       (1000)     1097 2023-03-03 10:05:06.000000 markup-markdown-1.5.3/markup/MarkdownPP.py
+-rwxrwxrwx   0 hai       (1000) hai       (1000)      362 2023-03-03 10:30:10.000000 markup-markdown-1.5.3/markup/Markers.py
+-rwxrwxrwx   0 hai       (1000) hai       (1000)      906 2023-03-03 10:05:06.000000 markup-markdown-1.5.3/markup/Module.py
+drwxr-xr-x   0 hai       (1000) hai       (1000)        0 2023-05-11 01:27:16.000000 markup-markdown-1.5.3/markup/Modules/
+-rwxrwxrwx   0 hai       (1000) hai       (1000)      798 2023-03-03 10:05:06.000000 markup-markdown-1.5.3/markup/Modules/BlankLine.py
+-rwxr-xr-x   0 hai       (1000) hai       (1000)     2483 2023-03-28 07:16:49.000000 markup-markdown-1.5.3/markup/Modules/EnvVariableReplacements.py
+-rwxrwxrwx   0 hai       (1000) hai       (1000)    10716 2023-03-04 11:36:46.000000 markup-markdown-1.5.3/markup/Modules/Include.py
+-rwxrwxrwx   0 hai       (1000) hai       (1000)     2302 2023-03-03 10:00:42.000000 markup-markdown-1.5.3/markup/Modules/IncludeCode.py
+-rwxrwxrwx   0 hai       (1000) hai       (1000)     1821 2023-03-03 10:05:07.000000 markup-markdown-1.5.3/markup/Modules/IncludeURL.py
+-rwxr-xr-x   0 hai       (1000) hai       (1000)     1801 2023-03-28 04:54:10.000000 markup-markdown-1.5.3/markup/Modules/IncludeWikilinkImage.py
+-rwxrwxrwx   0 hai       (1000) hai       (1000)     1812 2023-03-03 10:00:42.000000 markup-markdown-1.5.3/markup/Modules/Reference.py
+-rwxrwxrwx   0 hai       (1000) hai       (1000)     1318 2023-03-03 10:00:42.000000 markup-markdown-1.5.3/markup/Modules/SkipBlocks.py
+-rwxr-xr-x   0 hai       (1000) hai       (1000)     1874 2023-03-03 11:05:48.000000 markup-markdown-1.5.3/markup/Modules/SkipHeaderMetadata.py
+-rwxrwxrwx   0 hai       (1000) hai       (1000)      856 2023-03-03 10:05:07.000000 markup-markdown-1.5.3/markup/Modules/SkipLine.py
+-rwxr-xr-x   0 hai       (1000) hai       (1000)     1136 2023-03-05 05:56:26.000000 markup-markdown-1.5.3/markup/Modules/SkipObsidianComments.py
+-rwxrwxrwx   0 hai       (1000) hai       (1000)    14688 2023-03-13 08:25:14.000000 markup-markdown-1.5.3/markup/Modules/TableOfContents.py
+-rwxrwxrwx   0 hai       (1000) hai       (1000)     1009 2023-03-03 10:05:08.000000 markup-markdown-1.5.3/markup/Modules/WordPageBreak.py
+-rwxrwxrwx   0 hai       (1000) hai       (1000)     4095 2023-03-03 10:00:42.000000 markup-markdown-1.5.3/markup/Modules/YoutubeEmbed.py
+-rwxrwxrwx   0 hai       (1000) hai       (1000)      864 2023-03-03 10:00:42.000000 markup-markdown-1.5.3/markup/Modules/__init__.py
+-rw-r--r--   0 hai       (1000) hai       (1000)     9214 2023-05-11 01:26:11.000000 markup-markdown-1.5.3/markup/ObCanvas.py
+-rwxrwxrwx   0 hai       (1000) hai       (1000)     2682 2023-03-03 10:37:36.000000 markup-markdown-1.5.3/markup/Processor.py
+-rwxrwxrwx   0 hai       (1000) hai       (1000)      847 2023-03-03 10:00:42.000000 markup-markdown-1.5.3/markup/Transform.py
+-rwxrwxrwx   0 hai       (1000) hai       (1000)      343 2023-03-03 10:00:42.000000 markup-markdown-1.5.3/markup/__init__.py
+-rwxrwxrwx   0 hai       (1000) hai       (1000)     7217 2023-03-27 06:10:49.000000 markup-markdown-1.5.3/markup/main.py
+drwxr-xr-x   0 hai       (1000) hai       (1000)        0 2023-05-11 01:27:16.000000 markup-markdown-1.5.3/markup_markdown.egg-info/
+-rw-r--r--   0 hai       (1000) hai       (1000)      757 2023-05-11 01:27:14.000000 markup-markdown-1.5.3/markup_markdown.egg-info/PKG-INFO
+-rw-r--r--   0 hai       (1000) hai       (1000)      952 2023-05-11 01:27:15.000000 markup-markdown-1.5.3/markup_markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 hai       (1000) hai       (1000)        1 2023-05-11 01:27:15.000000 markup-markdown-1.5.3/markup_markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 hai       (1000) hai       (1000)      151 2023-05-11 01:27:15.000000 markup-markdown-1.5.3/markup_markdown.egg-info/entry_points.txt
+-rw-r--r--   0 hai       (1000) hai       (1000)       30 2023-05-11 01:27:15.000000 markup-markdown-1.5.3/markup_markdown.egg-info/requires.txt
+-rw-r--r--   0 hai       (1000) hai       (1000)       22 2023-05-11 01:27:15.000000 markup-markdown-1.5.3/markup_markdown.egg-info/top_level.txt
+-rw-r--r--   0 hai       (1000) hai       (1000)       38 2023-05-11 01:27:16.000000 markup-markdown-1.5.3/setup.cfg
+-rwxrwxrwx   0 hai       (1000) hai       (1000)     1263 2023-05-11 01:26:31.000000 markup-markdown-1.5.3/setup.py
+drwxr-xr-x   0 hai       (1000) hai       (1000)        0 2023-05-11 01:27:16.000000 markup-markdown-1.5.3/test/
+-rwxrwxrwx   0 hai       (1000) hai       (1000)    13382 2023-03-03 10:16:24.000000 markup-markdown-1.5.3/test/test.py
```

### Comparing `markup-markdown-1.5.2/LICENSE` & `markup-markdown-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/PKG-INFO` & `markup-markdown-1.5.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: markup-markdown
-Version: 1.5.2
+Version: 1.5.3
 Summary: Markup Markdown, Stack up markdown files with `!INCLUDE` directives.
 Home-page: https://github.com/hailiang-wang/markup-markdown
 Author: John Reese, Hai Liang W.
 Author-email: hailiang.hl.wang@gmail.com
 License: MIT License
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `markup-markdown-1.5.2/README.md` & `markup-markdown-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Headings.py` & `markup-markdown-1.5.3/markup/Headings.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/MarkdownPP.py` & `markup-markdown-1.5.3/markup/MarkdownPP.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Module.py` & `markup-markdown-1.5.3/markup/Module.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Modules/BlankLine.py` & `markup-markdown-1.5.3/markup/Modules/BlankLine.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Modules/EnvVariableReplacements.py` & `markup-markdown-1.5.3/markup/Modules/EnvVariableReplacements.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Modules/Include.py` & `markup-markdown-1.5.3/markup/Modules/Include.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Modules/IncludeCode.py` & `markup-markdown-1.5.3/markup/Modules/IncludeCode.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Modules/IncludeURL.py` & `markup-markdown-1.5.3/markup/Modules/IncludeURL.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Modules/IncludeWikilinkImage.py` & `markup-markdown-1.5.3/markup/Modules/IncludeWikilinkImage.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Modules/Reference.py` & `markup-markdown-1.5.3/markup/Modules/Reference.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Modules/SkipBlocks.py` & `markup-markdown-1.5.3/markup/Modules/SkipBlocks.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Modules/SkipHeaderMetadata.py` & `markup-markdown-1.5.3/markup/Modules/SkipHeaderMetadata.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Modules/SkipLine.py` & `markup-markdown-1.5.3/markup/Modules/SkipLine.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Modules/SkipObsidianComments.py` & `markup-markdown-1.5.3/markup/Modules/SkipObsidianComments.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Modules/TableOfContents.py` & `markup-markdown-1.5.3/markup/Modules/TableOfContents.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Modules/WordPageBreak.py` & `markup-markdown-1.5.3/markup/Modules/WordPageBreak.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Modules/YoutubeEmbed.py` & `markup-markdown-1.5.3/markup/Modules/YoutubeEmbed.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Modules/__init__.py` & `markup-markdown-1.5.3/markup/Modules/__init__.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/ObCanvas.py` & `markup-markdown-1.5.3/markup/ObCanvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 
 import json
 from copy import deepcopy
 from datetime import datetime
 
 # Get ENV
 ENVIRON = os.environ.copy()
-EXCERPT_PAGE_TITLE = ENVIRON.get("EXCERPT_PAGE_TITLE", "")
-EXCERPT_URL = ENVIRON.get("EXCERPT_URL", "")
-EXCERPT_LANG = ENVIRON.get("EXCERPT_LANG", "cn")
-EXCERPT_TAGS = ENVIRON.get("EXCERPT_TAGS", "pipeline,index")
+EXCERPT_PAGE_TITLE = ENVIRON.get("EXCERPT_PAGE_TITLE", "").strip()
+EXCERPT_URL = ENVIRON.get("EXCERPT_URL", "").strip()
+EXCERPT_LANG = ENVIRON.get("EXCERPT_LANG", "cn").strip()
+EXCERPT_TAGS = ENVIRON.get("EXCERPT_TAGS", "pipeline,index").strip()
 
 
 def get_tags_from_env():
     '''
     Get tags from ENV
     '''
     tags = set()
```

### Comparing `markup-markdown-1.5.2/markup/Processor.py` & `markup-markdown-1.5.3/markup/Processor.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/Transform.py` & `markup-markdown-1.5.3/markup/Transform.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup/main.py` & `markup-markdown-1.5.3/markup/main.py`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/markup_markdown.egg-info/PKG-INFO` & `markup-markdown-1.5.3/markup_markdown.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: markup-markdown
-Version: 1.5.2
+Version: 1.5.3
 Summary: Markup Markdown, Stack up markdown files with `!INCLUDE` directives.
 Home-page: https://github.com/hailiang-wang/markup-markdown
 Author: John Reese, Hai Liang W.
 Author-email: hailiang.hl.wang@gmail.com
 License: MIT License
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `markup-markdown-1.5.2/markup_markdown.egg-info/SOURCES.txt` & `markup-markdown-1.5.3/markup_markdown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `markup-markdown-1.5.2/setup.py` & `markup-markdown-1.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
 setup(
     name='markup-markdown',
     description='Markup Markdown, Stack up markdown files with `!INCLUDE` directives.',
-    version='1.5.2',
+    version='1.5.3',
     author='John Reese, Hai Liang W.',
     author_email='hailiang.hl.wang@gmail.com',
     url='https://github.com/hailiang-wang/markup-markdown',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
```

### Comparing `markup-markdown-1.5.2/test/test.py` & `markup-markdown-1.5.3/test/test.py`

 * *Files identical despite different names*

