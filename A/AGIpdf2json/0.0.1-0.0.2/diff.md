# Comparing `tmp/AGIpdf2json-0.0.1.tar.gz` & `tmp/AGIpdf2json-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AGIpdf2json-0.0.1.tar", last modified: Thu May 11 07:17:48 2023, max compression
+gzip compressed data, was "AGIpdf2json-0.0.2.tar", last modified: Thu May 11 07:26:01 2023, max compression
```

## Comparing `AGIpdf2json-0.0.1.tar` & `AGIpdf2json-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 07:17:48.089411 AGIpdf2json-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-11 07:17:48.085940 AGIpdf2json-0.0.1/AGIpdf2json.egg-info/
--rw-rw-rw-   0        0        0      338 2023-05-11 07:17:47.000000 AGIpdf2json-0.0.1/AGIpdf2json.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-05-11 07:17:47.000000 AGIpdf2json-0.0.1/AGIpdf2json.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 07:17:47.000000 AGIpdf2json-0.0.1/AGIpdf2json.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-11 07:17:47.000000 AGIpdf2json-0.0.1/AGIpdf2json.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-05-11 07:17:47.000000 AGIpdf2json-0.0.1/AGIpdf2json.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 07:17:47.000000 AGIpdf2json-0.0.1/AGIpdf2json.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      338 2023-05-11 07:17:48.087832 AGIpdf2json-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1558 2023-05-11 07:12:16.000000 AGIpdf2json-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-11 07:17:48.094656 AGIpdf2json-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      615 2023-05-11 07:17:39.000000 AGIpdf2json-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 07:26:01.067685 AGIpdf2json-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-11 07:26:01.054656 AGIpdf2json-0.0.2/AGIpdf2json.egg-info/
+-rw-rw-rw-   0        0        0     1941 2023-05-11 07:26:00.000000 AGIpdf2json-0.0.2/AGIpdf2json.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-05-11 07:26:00.000000 AGIpdf2json-0.0.2/AGIpdf2json.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 07:26:00.000000 AGIpdf2json-0.0.2/AGIpdf2json.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-11 07:26:00.000000 AGIpdf2json-0.0.2/AGIpdf2json.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-05-11 07:26:00.000000 AGIpdf2json-0.0.2/AGIpdf2json.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 07:26:00.000000 AGIpdf2json-0.0.2/AGIpdf2json.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1941 2023-05-11 07:26:01.058094 AGIpdf2json-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1558 2023-05-11 07:12:16.000000 AGIpdf2json-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-11 07:26:01.067685 AGIpdf2json-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      795 2023-05-11 07:25:57.000000 AGIpdf2json-0.0.2/setup.py
```

### Comparing `AGIpdf2json-0.0.1/README.md` & `AGIpdf2json-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `AGIpdf2json-0.0.1/setup.py` & `AGIpdf2json-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from setuptools import setup, find_packages
 
+with open('README.md', 'r', encoding='utf-8') as f:
+    long_description = f.read()
+
 setup(
     name='AGIpdf2json',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=[
         'pdfplumber',
         'click'
     ],
     description='This package can help user parse PDF files into text file and JSON file. Additionally, it can help user parse question-answer pairs into a JSONL document in prompt-completion format, that is supported by OpenAI',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     author='Mayank Monu',
     author_email='mayankmono29@gmail.com',
     entry_points={
         'console_scripts': [
             'PDFparser=main:cli',
         ],
     },
```

