# Comparing `tmp/MHTMLconverter-0.3.tar.gz` & `tmp/MHTMLconverter-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MHTMLconverter-0.3.tar", last modified: Wed May  3 11:29:32 2023, max compression
+gzip compressed data, was "MHTMLconverter-0.4.tar", last modified: Thu May 11 13:28:42 2023, max compression
```

## Comparing `MHTMLconverter-0.3.tar` & `MHTMLconverter-0.4.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:29:32.336892 MHTMLconverter-0.3/
-drwxrwxrwx   0        0        0        0 2023-05-03 11:29:32.319806 MHTMLconverter-0.3/MHTMLconverter.egg-info/
--rw-rw-rw-   0        0        0     1081 2023-05-03 11:29:32.000000 MHTMLconverter-0.3/MHTMLconverter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      663 2023-05-03 11:29:32.000000 MHTMLconverter-0.3/MHTMLconverter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:29:32.000000 MHTMLconverter-0.3/MHTMLconverter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-05-03 11:29:32.000000 MHTMLconverter-0.3/MHTMLconverter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-03 11:29:32.000000 MHTMLconverter-0.3/MHTMLconverter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1081 2023-05-03 11:29:32.337912 MHTMLconverter-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      734 2023-05-03 11:20:43.000000 MHTMLconverter-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 11:29:32.328360 MHTMLconverter-0.3/mhtmlconverter/
--rw-rw-rw-   0        0        0        0 2023-04-30 14:14:46.000000 MHTMLconverter-0.3/mhtmlconverter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:29:32.333372 MHTMLconverter-0.3/mhtmlconverter/cli/
--rw-rw-rw-   0        0        0        0 2023-04-30 14:14:46.000000 MHTMLconverter-0.3/mhtmlconverter/cli/__init__.py
--rw-rw-rw-   0        0        0      845 2023-05-02 17:55:24.000000 MHTMLconverter-0.3/mhtmlconverter/cli/html2mhtml.py
--rw-rw-rw-   0        0        0      945 2023-05-02 17:57:20.000000 MHTMLconverter-0.3/mhtmlconverter/cli/md2mhtml.py
--rw-rw-rw-   0        0        0     1033 2023-05-03 11:20:43.000000 MHTMLconverter-0.3/mhtmlconverter/fileutility.py
--rw-rw-rw-   0        0        0     5029 2023-05-03 11:20:43.000000 MHTMLconverter-0.3/mhtmlconverter/htmlutility.py
--rw-rw-rw-   0        0        0     5260 2023-05-03 11:20:43.000000 MHTMLconverter-0.3/mhtmlconverter/mhtml.py
--rw-rw-rw-   0        0        0       92 2023-04-30 14:53:31.000000 MHTMLconverter-0.3/pyproject.toml
--rw-rw-rw-   0        0        0      515 2023-05-03 11:29:32.338904 MHTMLconverter-0.3/setup.cfg
--rw-rw-rw-   0        0        0      293 2023-04-30 16:01:35.000000 MHTMLconverter-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:29:32.336892 MHTMLconverter-0.3/tests/
--rw-rw-rw-   0        0        0     1036 2023-05-03 11:20:43.000000 MHTMLconverter-0.3/tests/test_html.py
--rw-rw-rw-   0        0        0      988 2023-05-02 19:55:58.000000 MHTMLconverter-0.3/tests/test_md.py
+drwxrwxrwx   0        0        0        0 2023-05-11 13:28:42.293826 MHTMLconverter-0.4/
+drwxrwxrwx   0        0        0        0 2023-05-11 13:28:42.273753 MHTMLconverter-0.4/MHTMLconverter.egg-info/
+-rw-rw-rw-   0        0        0     1566 2023-05-11 13:28:42.000000 MHTMLconverter-0.4/MHTMLconverter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      783 2023-05-11 13:28:42.000000 MHTMLconverter-0.4/MHTMLconverter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 13:28:42.000000 MHTMLconverter-0.4/MHTMLconverter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-05-11 13:28:42.000000 MHTMLconverter-0.4/MHTMLconverter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       85 2023-05-11 13:28:42.000000 MHTMLconverter-0.4/MHTMLconverter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-11 13:28:42.000000 MHTMLconverter-0.4/MHTMLconverter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1566 2023-05-11 13:28:42.293826 MHTMLconverter-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1219 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 13:28:42.278759 MHTMLconverter-0.4/mhtmlconverter/
+-rw-rw-rw-   0        0        0        0 2023-04-30 14:14:46.000000 MHTMLconverter-0.4/mhtmlconverter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 13:28:42.286294 MHTMLconverter-0.4/mhtmlconverter/cli/
+-rw-rw-rw-   0        0        0        0 2023-04-30 14:14:46.000000 MHTMLconverter-0.4/mhtmlconverter/cli/__init__.py
+-rw-rw-rw-   0        0        0      845 2023-05-02 17:55:24.000000 MHTMLconverter-0.4/mhtmlconverter/cli/html2mhtml.py
+-rw-rw-rw-   0        0        0      945 2023-05-02 17:57:20.000000 MHTMLconverter-0.4/mhtmlconverter/cli/md2mhtml.py
+-rw-rw-rw-   0        0        0      960 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/mhtmlconverter/cli/mhtml2html.py
+-rw-rw-rw-   0        0        0     3458 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/mhtmlconverter/fileutility.py
+-rw-rw-rw-   0        0        0     5141 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/mhtmlconverter/htmlutility.py
+-rw-rw-rw-   0        0        0     6835 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/mhtmlconverter/mhtml.py
+-rw-rw-rw-   0        0        0       92 2023-04-30 14:53:31.000000 MHTMLconverter-0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      707 2023-05-11 13:28:42.294824 MHTMLconverter-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      293 2023-04-30 16:01:35.000000 MHTMLconverter-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 13:28:42.291807 MHTMLconverter-0.4/tests/
+-rw-rw-rw-   0        0        0     1414 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/tests/test_fileutility.py
+-rw-rw-rw-   0        0        0     1084 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/tests/test_html.py
+-rw-rw-rw-   0        0        0     1020 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/tests/test_md.py
+-rw-rw-rw-   0        0        0     2129 2023-05-11 13:08:21.000000 MHTMLconverter-0.4/tests/test_mhtml.py
```

### Comparing `MHTMLconverter-0.3/MHTMLconverter.egg-info/SOURCES.txt` & `MHTMLconverter-0.4/MHTMLconverter.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 MHTMLconverter.egg-info/PKG-INFO
 MHTMLconverter.egg-info/SOURCES.txt
 MHTMLconverter.egg-info/dependency_links.txt
+MHTMLconverter.egg-info/entry_points.txt
 MHTMLconverter.egg-info/requires.txt
 MHTMLconverter.egg-info/top_level.txt
 mhtmlconverter/__init__.py
 mhtmlconverter/fileutility.py
 mhtmlconverter/htmlutility.py
 mhtmlconverter/mhtml.py
 mhtmlconverter.egg-info/PKG-INFO
 mhtmlconverter.egg-info/SOURCES.txt
 mhtmlconverter.egg-info/dependency_links.txt
 mhtmlconverter.egg-info/requires.txt
 mhtmlconverter.egg-info/top_level.txt
 mhtmlconverter/cli/__init__.py
 mhtmlconverter/cli/html2mhtml.py
 mhtmlconverter/cli/md2mhtml.py
+mhtmlconverter/cli/mhtml2html.py
+tests/test_fileutility.py
 tests/test_html.py
-tests/test_md.py
+tests/test_md.py
+tests/test_mhtml.py
```

### Comparing `MHTMLconverter-0.3/mhtmlconverter/cli/html2mhtml.py` & `MHTMLconverter-0.4/mhtmlconverter/cli/html2mhtml.py`

 * *Files identical despite different names*

### Comparing `MHTMLconverter-0.3/mhtmlconverter/cli/md2mhtml.py` & `MHTMLconverter-0.4/mhtmlconverter/cli/md2mhtml.py`

 * *Files identical despite different names*

### Comparing `MHTMLconverter-0.3/mhtmlconverter/htmlutility.py` & `MHTMLconverter-0.4/mhtmlconverter/htmlutility.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     - rewrite the references into the HTML Dom in for consistance with renamed references
                 `rewrite_reference_in_html()`
 """
 import logging
 import urllib.parse
 import pathlib
 import bs4  # For HTML easy parsing and management
+import typing
 
 URL = str
 
 def turn_relative_into_absolute(htmlcontent: str, sourcefilepath: str,
                                 tag: str = "img", att: str = "src") -> str:
     """
         Transform relative references into global
@@ -103,39 +104,40 @@
     listhrefdata = [str(u.get('data-href')) for u in soup.find_all("link")]
 
     if listhrefdata: listhref.append(listhrefdata)
     
     return listhref
 
 
-def rewrite_reference(localurl: str) -> str:
+def rewrite_reference_fake_http(localurl: str) -> str:
     """
         Transform a local reference into a fake http reference
 
         Don't know why but mime related do not work with file:// or local names
 
         Simply add a fake "http://" protocol in front of the actual name
 
         TODO: check if it works even with file:// protocol
 
-        >>> rewrite_reference("img.jpg")
+        >>> rewrite_reference_fake_http("img.jpg")
         'http://img.jpg'
     """
     return f"http://{localurl}"
 
 
-def rewrite_reference_in_html(htmlcontent: str, reference: str) -> str:
+def rewrite_reference_in_html(htmlcontent: str, reference: str, 
+        rewrite_func: typing.Callable[[str],str] = rewrite_reference_fake_http) -> str:
     """
         rewrite the references into the HTML Dom for consistancy with renamed references
                 `rewrite_reference_in_html()`
         
         >>> rewrite_reference_in_html('<!DOCTYPE html><img src="img.jpg">', "img.jpg")
         '<!DOCTYPE html>\\n<img src="http://img.jpg"/>'
 
     """
     soup = bs4.BeautifulSoup(htmlcontent, 'html.parser')
     for i in soup.find_all('img'):
         if i.get('src') == reference:   # If the found img is the one referenced
             im = soup.new_tag('img')
-            im['src'] = rewrite_reference(reference)
+            im['src'] = rewrite_func(reference)
             i.replace_with(im)
     return str(soup)
```

### Comparing `MHTMLconverter-0.3/setup.cfg` & `MHTMLconverter-0.4/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6874 6d6c 636f 6e76 6572 7465   = mhtmlconverte
 00000020: 720d 0a61 7574 686f 7220 3d20 4172 6e61  r..author = Arna
 00000030: 7564 2052 6576 656c 0d0a 6175 7468 6f72  ud Revel..author
 00000040: 5f65 6d61 696c 203d 2072 6576 656c 2e61  _email = revel.a
 00000050: 726e 6175 6440 676d 6169 6c2e 636f 6d0d  rnaud@gmail.com.
-00000060: 0a76 6572 7369 6f6e 203d 2030 2e33 0d0a  .version = 0.3..
+00000060: 0a76 6572 7369 6f6e 203d 2030 2e34 0d0a  .version = 0.4..
 00000070: 6c69 6365 6e73 655f 6669 6c65 7320 3d20  license_files = 
 00000080: 4c49 4345 4e43 450d 0a75 726c 203d 2068  LICENCE..url = h
 00000090: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 000000a0: 6d2f 6172 6e61 7564 7265 7665 6c2f 4d48  m/arnaudrevel/MH
 000000b0: 544d 4c63 6f6e 7665 7274 6572 0d0a 6465  TMLconverter..de
 000000c0: 7363 7269 7074 696f 6e20 3d20 546f 6f6c  scription = Tool
 000000d0: 7320 746f 2063 6f6e 7665 7274 206d 6172  s to convert mar
@@ -23,11 +23,23 @@
 00000160: 390d 0a69 6e73 7461 6c6c 5f72 6571 7569  9..install_requi
 00000170: 7265 7320 3d20 0d0a 0962 6561 7574 6966  res = ...beautif
 00000180: 756c 736f 7570 343d 3d34 2e31 322e 320d  ulsoup4==4.12.2.
 00000190: 0a09 636c 6963 6b3d 3d38 2e31 2e33 0d0a  ..click==8.1.3..
 000001a0: 0963 6f6c 6f72 616d 613d 3d30 2e34 2e36  .colorama==0.4.6
 000001b0: 0d0a 094d 6172 6b64 6f77 6e3d 3d33 2e34  ...Markdown==3.4
 000001c0: 2e33 0d0a 0973 6f75 7073 6965 7665 3d3d  .3...soupsieve==
-000001d0: 322e 342e 310d 0a0d 0a5b 6567 675f 696e  2.4.1....[egg_in
-000001e0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-000001f0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-00000200: 0a0d 0a                                  ...
+000001d0: 322e 342e 310d 0a0d 0a5b 6f70 7469 6f6e  2.4.1....[option
+000001e0: 732e 656e 7472 795f 706f 696e 7473 5d0d  s.entry_points].
+000001f0: 0a63 6f6e 736f 6c65 5f73 6372 6970 7473  .console_scripts
+00000200: 203d 200d 0a09 6874 6d6c 326d 6874 6d6c   = ...html2mhtml
+00000210: 203d 206d 6874 6d6c 636f 6e76 6572 7465   = mhtmlconverte
+00000220: 722e 636c 692e 6874 6d6c 326d 6874 6d6c  r.cli.html2mhtml
+00000230: 3a6d 6169 6e0d 0a09 6d64 326d 6874 6d6c  :main...md2mhtml
+00000240: 203d 206d 6874 6d6c 636f 6e76 6572 7465   = mhtmlconverte
+00000250: 722e 636c 692e 6d64 326d 6874 6d6c 3a6d  r.cli.md2mhtml:m
+00000260: 6169 6e0d 0a09 6d68 746d 6c32 6874 6d6c  ain...mhtml2html
+00000270: 203d 206d 6874 6d6c 636f 6e76 6572 7465   = mhtmlconverte
+00000280: 722e 636c 692e 6d68 746d 6c32 6874 6d6c  r.cli.mhtml2html
+00000290: 3a6d 6169 6e0d 0a0d 0a5b 6567 675f 696e  :main....[egg_in
+000002a0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+000002b0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+000002c0: 0a0d 0a                                  ...
```

### Comparing `MHTMLconverter-0.3/tests/test_md.py` & `MHTMLconverter-0.4/tests/test_md.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 
 import markdown
 
 def test_md() -> None:
     """
         Test MD
     """
-    out = pathlib.Path("./tests/resources/test_md.mhtml")
+    out = pathlib.Path("./tests/resources/results/test_md.mhtml")
 
     if out.exists():    out.unlink()
 
     with open("./tests/resources/test.md","r") as md_file:
         htmlcontent = markdown.markdown(md_file.read())
-        mhtmlconverter.mhtml.html_content_to_mhtml(htmlcontent,"./tests/resources/test_md.mhtml", "./tests/resources/test_local.md")
+        mhtmlconverter.mhtml.html_content_to_mhtml(htmlcontent,"./tests/resources/results/test_md.mhtml", "./tests/resources/test_local.md")
 
     assert(out.exists())
 
 def test_local_md() -> None:
     """
         Test local MD
 
     """
-    out = pathlib.Path("./tests/resources/test_localmd.mhtml")
+    out = pathlib.Path("./tests/resources/results/test_localmd.mhtml")
 
     if out.exists():    out.unlink()
 
     with open("./tests/resources/test_local.md","r") as md_file:
         htmlcontent = markdown.markdown(md_file.read())
-        mhtmlconverter.mhtml.html_content_to_mhtml(htmlcontent,"./tests/resources/test_localmd.mhtml", "./tests/resources/test_local.md")
+        mhtmlconverter.mhtml.html_content_to_mhtml(htmlcontent,"./tests/resources/results/test_localmd.mhtml", "./tests/resources/test_local.md")
 
     assert(out.exists())
```

