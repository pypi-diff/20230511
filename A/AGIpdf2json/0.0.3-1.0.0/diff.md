# Comparing `tmp/AGIpdf2json-0.0.3.tar.gz` & `tmp/AGIpdf2json-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AGIpdf2json-0.0.3.tar", last modified: Thu May 11 07:30:24 2023, max compression
+gzip compressed data, was "AGIpdf2json-1.0.0.tar", last modified: Thu May 11 08:09:42 2023, max compression
```

## Comparing `AGIpdf2json-0.0.3.tar` & `AGIpdf2json-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 07:30:24.649087 AGIpdf2json-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-05-11 07:30:24.636623 AGIpdf2json-0.0.3/AGIpdf2json.egg-info/
--rw-rw-rw-   0        0        0     1941 2023-05-11 07:30:24.000000 AGIpdf2json-0.0.3/AGIpdf2json.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-05-11 07:30:24.000000 AGIpdf2json-0.0.3/AGIpdf2json.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 07:30:24.000000 AGIpdf2json-0.0.3/AGIpdf2json.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-11 07:30:24.000000 AGIpdf2json-0.0.3/AGIpdf2json.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-05-11 07:30:24.000000 AGIpdf2json-0.0.3/AGIpdf2json.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 07:30:24.000000 AGIpdf2json-0.0.3/AGIpdf2json.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1941 2023-05-11 07:30:24.640552 AGIpdf2json-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1558 2023-05-11 07:12:16.000000 AGIpdf2json-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-11 07:30:24.657376 AGIpdf2json-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-05-11 07:29:57.000000 AGIpdf2json-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:09:42.773624 AGIpdf2json-1.0.0/
+drwxrwxrwx   0        0        0        0 2023-05-11 08:09:42.706990 AGIpdf2json-1.0.0/AGIPDF2JSON/
+-rw-rw-rw-   0        0        0       19 2023-05-11 07:55:37.000000 AGIpdf2json-1.0.0/AGIPDF2JSON/__init__.py
+-rw-rw-rw-   0        0        0     1502 2023-05-11 08:08:26.000000 AGIpdf2json-1.0.0/AGIPDF2JSON/main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:09:42.753522 AGIpdf2json-1.0.0/AGIpdf2json.egg-info/
+-rw-rw-rw-   0        0        0     1941 2023-05-11 08:09:42.000000 AGIpdf2json-1.0.0/AGIpdf2json.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-05-11 08:09:42.000000 AGIpdf2json-1.0.0/AGIpdf2json.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 08:09:42.000000 AGIpdf2json-1.0.0/AGIpdf2json.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-11 08:09:42.000000 AGIpdf2json-1.0.0/AGIpdf2json.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-05-11 08:09:42.000000 AGIpdf2json-1.0.0/AGIpdf2json.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-11 08:09:42.000000 AGIpdf2json-1.0.0/AGIpdf2json.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1941 2023-05-11 08:09:42.757599 AGIpdf2json-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1558 2023-05-11 07:12:16.000000 AGIpdf2json-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-11 08:09:42.776119 AGIpdf2json-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      809 2023-05-11 08:09:32.000000 AGIpdf2json-1.0.0/setup.py
```

### Comparing `AGIpdf2json-0.0.3/AGIpdf2json.egg-info/PKG-INFO` & `AGIpdf2json-1.0.0/AGIpdf2json.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AGIpdf2json
-Version: 0.0.3
+Version: 1.0.0
 Summary: This package can help user parse PDF files into text file and JSON file. Additionally, it can help user parse question-answer pairs into a JSONL document in prompt-completion format, that is supported by OpenAI
 Author: Mayank Monu
 Author-email: mayankmono29@gmail.com
 Description-Content-Type: text/markdown
 
 # Multi-purpose PDF parser
```

### Comparing `AGIpdf2json-0.0.3/PKG-INFO` & `AGIpdf2json-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AGIpdf2json
-Version: 0.0.3
+Version: 1.0.0
 Summary: This package can help user parse PDF files into text file and JSON file. Additionally, it can help user parse question-answer pairs into a JSONL document in prompt-completion format, that is supported by OpenAI
 Author: Mayank Monu
 Author-email: mayankmono29@gmail.com
 Description-Content-Type: text/markdown
 
 # Multi-purpose PDF parser
```

### Comparing `AGIpdf2json-0.0.3/README.md` & `AGIpdf2json-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `AGIpdf2json-0.0.3/setup.py` & `AGIpdf2json-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='AGIpdf2json',
-    version='0.0.3',
+    version='1.0.0',
     packages=find_packages(),
     install_requires=[
         'pdfplumber',
         'click'
     ],
     description='This package can help user parse PDF files into text file and JSON file. Additionally, it can help user parse question-answer pairs into a JSONL document in prompt-completion format, that is supported by OpenAI',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Mayank Monu',
     author_email='mayankmono29@gmail.com',
     entry_points={
         'console_scripts': [
-            'AGIpdf2json=main:cli',
+            'AGIpdf2json=AGIPDF2JSON.main:cli',
         ],
     },
 )
```

