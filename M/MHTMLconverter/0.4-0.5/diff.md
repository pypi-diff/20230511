# Comparing `tmp/MHTMLconverter-0.4.tar.gz` & `tmp/MHTMLconverter-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MHTMLconverter-0.4.tar", last modified: Thu May 11 13:28:42 2023, max compression
+gzip compressed data, was "MHTMLconverter-0.5.tar", last modified: Thu May 11 13:37:54 2023, max compression
```

## Comparing `MHTMLconverter-0.4.tar` & `MHTMLconverter-0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 13:28:42.293826 MHTMLconverter-0.4/
-drwxrwxrwx   0        0        0        0 2023-05-11 13:28:42.273753 MHTMLconverter-0.4/MHTMLconverter.egg-info/
--rw-rw-rw-   0        0        0     1566 2023-05-11 13:28:42.000000 MHTMLconverter-0.4/MHTMLconverter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      783 2023-05-11 13:28:42.000000 MHTMLconverter-0.4/MHTMLconverter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 13:28:42.000000 MHTMLconverter-0.4/MHTMLconverter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-05-11 13:28:42.000000 MHTMLconverter-0.4/MHTMLconverter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       85 2023-05-11 13:28:42.000000 MHTMLconverter-0.4/MHTMLconverter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-11 13:28:42.000000 MHTMLconverter-0.4/MHTMLconverter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1566 2023-05-11 13:28:42.293826 MHTMLconverter-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1219 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 13:28:42.278759 MHTMLconverter-0.4/mhtmlconverter/
--rw-rw-rw-   0        0        0        0 2023-04-30 14:14:46.000000 MHTMLconverter-0.4/mhtmlconverter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 13:28:42.286294 MHTMLconverter-0.4/mhtmlconverter/cli/
--rw-rw-rw-   0        0        0        0 2023-04-30 14:14:46.000000 MHTMLconverter-0.4/mhtmlconverter/cli/__init__.py
--rw-rw-rw-   0        0        0      845 2023-05-02 17:55:24.000000 MHTMLconverter-0.4/mhtmlconverter/cli/html2mhtml.py
--rw-rw-rw-   0        0        0      945 2023-05-02 17:57:20.000000 MHTMLconverter-0.4/mhtmlconverter/cli/md2mhtml.py
--rw-rw-rw-   0        0        0      960 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/mhtmlconverter/cli/mhtml2html.py
--rw-rw-rw-   0        0        0     3458 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/mhtmlconverter/fileutility.py
--rw-rw-rw-   0        0        0     5141 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/mhtmlconverter/htmlutility.py
--rw-rw-rw-   0        0        0     6835 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/mhtmlconverter/mhtml.py
--rw-rw-rw-   0        0        0       92 2023-04-30 14:53:31.000000 MHTMLconverter-0.4/pyproject.toml
--rw-rw-rw-   0        0        0      707 2023-05-11 13:28:42.294824 MHTMLconverter-0.4/setup.cfg
--rw-rw-rw-   0        0        0      293 2023-04-30 16:01:35.000000 MHTMLconverter-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 13:28:42.291807 MHTMLconverter-0.4/tests/
--rw-rw-rw-   0        0        0     1414 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/tests/test_fileutility.py
--rw-rw-rw-   0        0        0     1084 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/tests/test_html.py
--rw-rw-rw-   0        0        0     1020 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/tests/test_md.py
--rw-rw-rw-   0        0        0     2129 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/tests/test_mhtml.py
+drwxrwxrwx   0        0        0        0 2023-05-11 13:37:54.006512 MHTMLconverter-0.5/
+drwxrwxrwx   0        0        0        0 2023-05-11 13:37:53.988340 MHTMLconverter-0.5/MHTMLconverter.egg-info/
+-rw-rw-rw-   0        0        0     1727 2023-05-11 13:37:53.000000 MHTMLconverter-0.5/MHTMLconverter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      783 2023-05-11 13:37:53.000000 MHTMLconverter-0.5/MHTMLconverter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 13:37:53.000000 MHTMLconverter-0.5/MHTMLconverter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-05-11 13:37:53.000000 MHTMLconverter-0.5/MHTMLconverter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       85 2023-05-11 13:37:53.000000 MHTMLconverter-0.5/MHTMLconverter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-11 13:37:53.000000 MHTMLconverter-0.5/MHTMLconverter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1727 2023-05-11 13:37:54.006512 MHTMLconverter-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1378 2023-05-11 13:33:20.000000 MHTMLconverter-0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 13:37:53.993635 MHTMLconverter-0.5/mhtmlconverter/
+-rw-rw-rw-   0        0        0        0 2023-04-30 14:14:46.000000 MHTMLconverter-0.5/mhtmlconverter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 13:37:54.000161 MHTMLconverter-0.5/mhtmlconverter/cli/
+-rw-rw-rw-   0        0        0        0 2023-04-30 14:14:46.000000 MHTMLconverter-0.5/mhtmlconverter/cli/__init__.py
+-rw-rw-rw-   0        0        0      845 2023-05-02 17:55:24.000000 MHTMLconverter-0.5/mhtmlconverter/cli/html2mhtml.py
+-rw-rw-rw-   0        0        0      945 2023-05-02 17:57:20.000000 MHTMLconverter-0.5/mhtmlconverter/cli/md2mhtml.py
+-rw-rw-rw-   0        0        0      960 2023-05-11 13:08:21.000000 MHTMLconverter-0.5/mhtmlconverter/cli/mhtml2html.py
+-rw-rw-rw-   0        0        0     3458 2023-05-11 13:08:21.000000 MHTMLconverter-0.5/mhtmlconverter/fileutility.py
+-rw-rw-rw-   0        0        0     5141 2023-05-11 13:08:21.000000 MHTMLconverter-0.5/mhtmlconverter/htmlutility.py
+-rw-rw-rw-   0        0        0     6835 2023-05-11 13:08:21.000000 MHTMLconverter-0.5/mhtmlconverter/mhtml.py
+-rw-rw-rw-   0        0        0       92 2023-04-30 14:53:31.000000 MHTMLconverter-0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      707 2023-05-11 13:37:54.008076 MHTMLconverter-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      293 2023-04-30 16:01:35.000000 MHTMLconverter-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 13:37:54.005511 MHTMLconverter-0.5/tests/
+-rw-rw-rw-   0        0        0     1414 2023-05-11 13:08:21.000000 MHTMLconverter-0.5/tests/test_fileutility.py
+-rw-rw-rw-   0        0        0     1084 2023-05-11 13:08:21.000000 MHTMLconverter-0.5/tests/test_html.py
+-rw-rw-rw-   0        0        0     1020 2023-05-11 13:08:21.000000 MHTMLconverter-0.5/tests/test_md.py
+-rw-rw-rw-   0        0        0     2129 2023-05-11 13:08:21.000000 MHTMLconverter-0.5/tests/test_mhtml.py
```

### Comparing `MHTMLconverter-0.4/MHTMLconverter.egg-info/PKG-INFO` & `MHTMLconverter-0.5/MHTMLconverter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MHTMLconverter
-Version: 0.4
+Version: 0.5
 Summary: Tools to convert markdown or html files including images to a single MHTML self-content file
 Home-page: https://github.com/arnaudrevel/MHTMLconverter
 Author: Arnaud Revel
 Author-email: revel.arnaud@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
@@ -44,7 +44,18 @@
 If the resource dir is different, the references in the html file are rewritten according to
 this location
 
 ```
 >> python -m mhtmlconverter.cli.mhtml2html -i index.mhtml -o index.html -r resources_dir
 
 ```
+
+### html2mtml, md2mtml, mhtml2html
+
+Those scripts should work...
+
+```
+    >>> html2mtml --help
+    >>> md2mtml --help
+    >>> mhtml2html --help
+
+```
```

### Comparing `MHTMLconverter-0.4/MHTMLconverter.egg-info/SOURCES.txt` & `MHTMLconverter-0.5/MHTMLconverter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MHTMLconverter-0.4/PKG-INFO` & `MHTMLconverter-0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MHTMLconverter
-Version: 0.4
+Version: 0.5
 Summary: Tools to convert markdown or html files including images to a single MHTML self-content file
 Home-page: https://github.com/arnaudrevel/MHTMLconverter
 Author: Arnaud Revel
 Author-email: revel.arnaud@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
@@ -44,7 +44,18 @@
 If the resource dir is different, the references in the html file are rewritten according to
 this location
 
 ```
 >> python -m mhtmlconverter.cli.mhtml2html -i index.mhtml -o index.html -r resources_dir
 
 ```
+
+### html2mtml, md2mtml, mhtml2html
+
+Those scripts should work...
+
+```
+    >>> html2mtml --help
+    >>> md2mtml --help
+    >>> mhtml2html --help
+
+```
```

### Comparing `MHTMLconverter-0.4/README.md` & `MHTMLconverter-0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,7 +34,18 @@
 If the resource dir is different, the references in the html file are rewritten according to
 this location
 
 ```
 >> python -m mhtmlconverter.cli.mhtml2html -i index.mhtml -o index.html -r resources_dir
 
 ```
+
+### html2mtml, md2mtml, mhtml2html
+
+Those scripts should work...
+
+```
+    >>> html2mtml --help
+    >>> md2mtml --help
+    >>> mhtml2html --help
+
+```
```

### Comparing `MHTMLconverter-0.4/mhtmlconverter/cli/html2mhtml.py` & `MHTMLconverter-0.5/mhtmlconverter/cli/html2mhtml.py`

 * *Files identical despite different names*

### Comparing `MHTMLconverter-0.4/mhtmlconverter/cli/md2mhtml.py` & `MHTMLconverter-0.5/mhtmlconverter/cli/md2mhtml.py`

 * *Files identical despite different names*

### Comparing `MHTMLconverter-0.4/mhtmlconverter/cli/mhtml2html.py` & `MHTMLconverter-0.5/mhtmlconverter/cli/mhtml2html.py`

 * *Files identical despite different names*

### Comparing `MHTMLconverter-0.4/mhtmlconverter/fileutility.py` & `MHTMLconverter-0.5/mhtmlconverter/fileutility.py`

 * *Files identical despite different names*

### Comparing `MHTMLconverter-0.4/mhtmlconverter/htmlutility.py` & `MHTMLconverter-0.5/mhtmlconverter/htmlutility.py`

 * *Files identical despite different names*

### Comparing `MHTMLconverter-0.4/mhtmlconverter/mhtml.py` & `MHTMLconverter-0.5/mhtmlconverter/mhtml.py`

 * *Files identical despite different names*

### Comparing `MHTMLconverter-0.4/setup.cfg` & `MHTMLconverter-0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6874 6d6c 636f 6e76 6572 7465   = mhtmlconverte
 00000020: 720d 0a61 7574 686f 7220 3d20 4172 6e61  r..author = Arna
 00000030: 7564 2052 6576 656c 0d0a 6175 7468 6f72  ud Revel..author
 00000040: 5f65 6d61 696c 203d 2072 6576 656c 2e61  _email = revel.a
 00000050: 726e 6175 6440 676d 6169 6c2e 636f 6d0d  rnaud@gmail.com.
-00000060: 0a76 6572 7369 6f6e 203d 2030 2e34 0d0a  .version = 0.4..
+00000060: 0a76 6572 7369 6f6e 203d 2030 2e35 0d0a  .version = 0.5..
 00000070: 6c69 6365 6e73 655f 6669 6c65 7320 3d20  license_files = 
 00000080: 4c49 4345 4e43 450d 0a75 726c 203d 2068  LICENCE..url = h
 00000090: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 000000a0: 6d2f 6172 6e61 7564 7265 7665 6c2f 4d48  m/arnaudrevel/MH
 000000b0: 544d 4c63 6f6e 7665 7274 6572 0d0a 6465  TMLconverter..de
 000000c0: 7363 7269 7074 696f 6e20 3d20 546f 6f6c  scription = Tool
 000000d0: 7320 746f 2063 6f6e 7665 7274 206d 6172  s to convert mar
```

### Comparing `MHTMLconverter-0.4/tests/test_fileutility.py` & `MHTMLconverter-0.5/tests/test_fileutility.py`

 * *Files identical despite different names*

### Comparing `MHTMLconverter-0.4/tests/test_html.py` & `MHTMLconverter-0.5/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `MHTMLconverter-0.4/tests/test_md.py` & `MHTMLconverter-0.5/tests/test_md.py`

 * *Files identical despite different names*

### Comparing `MHTMLconverter-0.4/tests/test_mhtml.py` & `MHTMLconverter-0.5/tests/test_mhtml.py`

 * *Files identical despite different names*

