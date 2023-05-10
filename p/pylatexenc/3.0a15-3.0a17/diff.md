# Comparing `tmp/pylatexenc-3.0a15.tar.gz` & `tmp/pylatexenc-3.0a17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylatexenc-3.0a15.tar", max compression
+gzip compressed data, was "pylatexenc-3.0a17.tar", max compression
```

## Comparing `pylatexenc-3.0a15.tar` & `pylatexenc-3.0a17.tar`

### file list

```diff
@@ -1,58 +1,60 @@
--rw-r--r--   0        0        0     1086 2023-04-15 13:24:30.143033 pylatexenc-3.0a15/LICENSE.txt
--rw-r--r--   0        0        0     3572 2023-04-18 07:57:57.261013 pylatexenc-3.0a15/README.rst
--rw-r--r--   0        0        0     1326 2019-07-25 20:20:56.000000 pylatexenc-3.0a15/pylatexenc/__init__.py
--rw-r--r--   0        0        0     5162 2023-04-15 11:29:53.841130 pylatexenc-3.0a15/pylatexenc/_util.py
--rw-r--r--   0        0        0     3766 2023-04-15 11:29:53.841423 pylatexenc-3.0a15/pylatexenc/_util_support.py
--rw-r--r--   0        0        0    59269 2023-04-15 11:57:13.282343 pylatexenc-3.0a15/pylatexenc/latex2text/__init__.py
--rw-r--r--   0        0        0    10011 2023-04-15 11:55:00.471421 pylatexenc-3.0a15/pylatexenc/latex2text/__main__.py
--rw-r--r--   0        0        0    94342 2023-04-15 11:29:53.843500 pylatexenc-3.0a15/pylatexenc/latex2text/_defaultspecs.py
--rw-r--r--   0        0        0     2526 2021-12-17 19:22:56.000000 pylatexenc-3.0a15/pylatexenc/latex2text/_inputlatexfile.py
--rw-r--r--   0        0        0    12944 2021-03-31 23:28:40.000000 pylatexenc-3.0a15/pylatexenc/latexencode/__init__.py
--rw-r--r--   0        0        0     4426 2019-08-25 13:06:29.000000 pylatexenc-3.0a15/pylatexenc/latexencode/__main__.py
--rw-r--r--   0        0        0     4404 2023-04-15 12:03:11.103995 pylatexenc-3.0a15/pylatexenc/latexencode/_partial_latex_encoder.py
--rw-r--r--   0        0        0    99833 2021-09-15 19:08:59.000000 pylatexenc-3.0a15/pylatexenc/latexencode/_uni2latexmap.py
--rw-r--r--   0        0        0    55947 2019-07-27 15:08:32.000000 pylatexenc-3.0a15/pylatexenc/latexencode/_uni2latexmap_xml.py
--rw-r--r--   0        0        0    26209 2021-04-01 11:51:30.000000 pylatexenc-3.0a15/pylatexenc/latexencode/_unicode_to_latex_encoder.py
--rw-r--r--   0        0        0     2179 2023-04-15 11:29:53.843788 pylatexenc-3.0a15/pylatexenc/latexnodes/__init__.py
--rw-r--r--   0        0        0     2197 2023-04-15 17:44:53.955715 pylatexenc-3.0a15/pylatexenc/latexnodes/_callablespecbase.py
--rw-r--r--   0        0        0    11001 2023-04-15 17:53:09.732071 pylatexenc-3.0a15/pylatexenc/latexnodes/_exctypes.py
--rw-r--r--   0        0        0     6315 2023-04-15 17:52:07.518222 pylatexenc-3.0a15/pylatexenc/latexnodes/_latexcontextdbbase.py
--rw-r--r--   0        0        0    36489 2023-04-15 19:46:24.921466 pylatexenc-3.0a15/pylatexenc/latexnodes/_nodescollector.py
--rw-r--r--   0        0        0    10124 2023-04-15 11:29:53.845301 pylatexenc-3.0a15/pylatexenc/latexnodes/_parsedargs.py
--rw-r--r--   0        0        0    11877 2023-04-15 11:29:53.845584 pylatexenc-3.0a15/pylatexenc/latexnodes/_parsedargsinfo.py
--rw-r--r--   0        0        0    17020 2023-04-15 17:51:09.423753 pylatexenc-3.0a15/pylatexenc/latexnodes/_parsingstate.py
--rw-r--r--   0        0        0     7109 2023-04-15 11:29:53.846228 pylatexenc-3.0a15/pylatexenc/latexnodes/_parsingstatedelta.py
--rw-r--r--   0        0        0     8446 2023-04-15 17:12:48.503604 pylatexenc-3.0a15/pylatexenc/latexnodes/_token.py
--rw-r--r--   0        0        0    27524 2023-04-26 15:32:16.345591 pylatexenc-3.0a15/pylatexenc/latexnodes/_tokenreader.py
--rw-r--r--   0        0        0    10098 2023-04-15 17:13:31.159345 pylatexenc-3.0a15/pylatexenc/latexnodes/_tokenreaderbase.py
--rw-r--r--   0        0        0     4841 2023-04-15 17:50:19.637390 pylatexenc-3.0a15/pylatexenc/latexnodes/_walkerbase.py
--rw-r--r--   0        0        0    42174 2023-04-15 16:56:19.119357 pylatexenc-3.0a15/pylatexenc/latexnodes/nodes.py
--rw-r--r--   0        0        0     2141 2023-04-15 11:29:53.848262 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/__init__.py
--rw-r--r--   0        0        0     5285 2023-04-15 11:29:53.848639 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_base.py
--rw-r--r--   0        0        0    41024 2023-04-15 16:46:03.019064 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_delimited.py
--rw-r--r--   0        0        0    18288 2023-04-15 11:29:53.849524 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_expression.py
--rw-r--r--   0        0        0    12896 2023-04-15 11:29:53.849773 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_generalnodes.py
--rw-r--r--   0        0        0     5658 2023-04-15 11:29:53.849985 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_math.py
--rw-r--r--   0        0        0     6180 2023-04-15 11:29:53.850252 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_optionals.py
--rw-r--r--   0        0        0    22370 2023-04-15 16:46:34.476752 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_stdarg.py
--rw-r--r--   0        0        0    11551 2023-04-18 07:57:57.274724 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_verbatim.py
--rw-r--r--   0        0        0     4520 2023-04-15 11:29:53.851132 pylatexenc-3.0a15/pylatexenc/latexwalker/__init__.py
--rw-r--r--   0        0        0     6214 2023-04-15 11:29:53.851406 pylatexenc-3.0a15/pylatexenc/latexwalker/__main__.py
--rw-r--r--   0        0        0    17597 2023-04-26 15:29:33.456920 pylatexenc-3.0a15/pylatexenc/latexwalker/_defaultspecs.py
--rw-r--r--   0        0        0     2937 2023-04-15 11:29:53.852111 pylatexenc-3.0a15/pylatexenc/latexwalker/_get_defaultspecs.py
--rw-r--r--   0        0        0     7833 2023-04-15 11:29:53.852354 pylatexenc-3.0a15/pylatexenc/latexwalker/_helpers.py
--rw-r--r--   0        0        0     7487 2023-04-15 11:29:53.852626 pylatexenc-3.0a15/pylatexenc/latexwalker/_legacy_py1x.py
--rw-r--r--   0        0        0    52642 2023-04-15 11:37:07.707893 pylatexenc-3.0a15/pylatexenc/latexwalker/_walker.py
--rw-r--r--   0        0        0     2414 2023-04-18 07:57:57.275029 pylatexenc-3.0a15/pylatexenc/macrospec/__init__.py
--rw-r--r--   0        0        0     8819 2023-04-18 07:57:57.275339 pylatexenc-3.0a15/pylatexenc/macrospec/_argumentsparser.py
--rw-r--r--   0        0        0     7372 2023-04-15 11:29:53.853904 pylatexenc-3.0a15/pylatexenc/macrospec/_environmentbodyparser.py
--rw-r--r--   0        0        0    29706 2023-04-15 11:29:53.854223 pylatexenc-3.0a15/pylatexenc/macrospec/_latexcontextdb.py
--rw-r--r--   0        0        0    10046 2023-04-15 20:38:58.126785 pylatexenc-3.0a15/pylatexenc/macrospec/_macrocallparser.py
--rw-r--r--   0        0        0     1535 2023-04-15 11:29:53.854841 pylatexenc-3.0a15/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py
--rw-r--r--   0        0        0     9488 2023-04-18 07:57:57.275664 pylatexenc-3.0a15/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py
--rw-r--r--   0        0        0    16735 2023-04-18 07:57:57.276084 pylatexenc-3.0a15/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py
--rw-r--r--   0        0        0    15650 2023-04-15 11:29:53.855594 pylatexenc-3.0a15/pylatexenc/macrospec/_specclasses.py
--rw-r--r--   0        0        0     8951 2023-04-15 11:29:53.855874 pylatexenc-3.0a15/pylatexenc/macrospec/_spechelpers.py
--rw-r--r--   0        0        0     2115 2023-04-26 18:27:44.170514 pylatexenc-3.0a15/pylatexenc/version.py
--rw-r--r--   0        0        0     1091 2023-04-26 18:27:38.171969 pylatexenc-3.0a15/pyproject.toml
--rw-r--r--   0        0        0     4209 1970-01-01 00:00:00.000000 pylatexenc-3.0a15/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-04-15 13:24:30.143033 pylatexenc-3.0a17/LICENSE.txt
+-rw-r--r--   0        0        0     3572 2023-04-18 07:57:57.261013 pylatexenc-3.0a17/README.rst
+-rw-r--r--   0        0        0     1326 2019-07-25 20:20:56.000000 pylatexenc-3.0a17/pylatexenc/__init__.py
+-rw-r--r--   0        0        0     5083 2023-05-10 17:45:32.190520 pylatexenc-3.0a17/pylatexenc/_util.py
+-rw-r--r--   0        0        0     3766 2023-04-15 11:29:53.841423 pylatexenc-3.0a17/pylatexenc/_util_support.py
+-rw-r--r--   0        0        0    59269 2023-04-15 11:57:13.282343 pylatexenc-3.0a17/pylatexenc/latex2text/__init__.py
+-rw-r--r--   0        0        0    10011 2023-04-15 11:55:00.471421 pylatexenc-3.0a17/pylatexenc/latex2text/__main__.py
+-rw-r--r--   0        0        0    94342 2023-04-15 11:29:53.843500 pylatexenc-3.0a17/pylatexenc/latex2text/_defaultspecs.py
+-rw-r--r--   0        0        0     2526 2021-12-17 19:22:56.000000 pylatexenc-3.0a17/pylatexenc/latex2text/_inputlatexfile.py
+-rw-r--r--   0        0        0    12910 2023-05-10 22:25:03.185982 pylatexenc-3.0a17/pylatexenc/latexencode/__init__.py
+-rw-r--r--   0        0        0     4426 2019-08-25 13:06:29.000000 pylatexenc-3.0a17/pylatexenc/latexencode/__main__.py
+-rw-r--r--   0        0        0     4344 2023-05-10 22:44:33.867148 pylatexenc-3.0a17/pylatexenc/latexencode/_partial_latex_encoder.py
+-rw-r--r--   0        0        0     7516 2023-05-10 22:31:54.454547 pylatexenc-3.0a17/pylatexenc/latexencode/_rule.py
+-rw-r--r--   0        0        0    99833 2021-09-15 19:08:59.000000 pylatexenc-3.0a17/pylatexenc/latexencode/_uni2latexmap.py
+-rw-r--r--   0        0        0    55947 2019-07-27 15:08:32.000000 pylatexenc-3.0a17/pylatexenc/latexencode/_uni2latexmap_xml.py
+-rw-r--r--   0        0        0    20901 2023-05-10 22:39:39.968571 pylatexenc-3.0a17/pylatexenc/latexencode/_unicode_to_latex_encoder.py
+-rw-r--r--   0        0        0     3748 2023-05-10 22:33:06.225330 pylatexenc-3.0a17/pylatexenc/latexencode/get_builtin_rules.py
+-rw-r--r--   0        0        0     2179 2023-04-15 11:29:53.843788 pylatexenc-3.0a17/pylatexenc/latexnodes/__init__.py
+-rw-r--r--   0        0        0     2197 2023-04-15 17:44:53.955715 pylatexenc-3.0a17/pylatexenc/latexnodes/_callablespecbase.py
+-rw-r--r--   0        0        0    11001 2023-04-15 17:53:09.732071 pylatexenc-3.0a17/pylatexenc/latexnodes/_exctypes.py
+-rw-r--r--   0        0        0     6315 2023-04-15 17:52:07.518222 pylatexenc-3.0a17/pylatexenc/latexnodes/_latexcontextdbbase.py
+-rw-r--r--   0        0        0    36523 2023-04-27 21:55:57.200105 pylatexenc-3.0a17/pylatexenc/latexnodes/_nodescollector.py
+-rw-r--r--   0        0        0    10100 2023-04-27 21:53:07.906038 pylatexenc-3.0a17/pylatexenc/latexnodes/_parsedargs.py
+-rw-r--r--   0        0        0    11877 2023-04-15 11:29:53.845584 pylatexenc-3.0a17/pylatexenc/latexnodes/_parsedargsinfo.py
+-rw-r--r--   0        0        0    17020 2023-04-15 17:51:09.423753 pylatexenc-3.0a17/pylatexenc/latexnodes/_parsingstate.py
+-rw-r--r--   0        0        0     6625 2023-04-27 21:47:43.535760 pylatexenc-3.0a17/pylatexenc/latexnodes/_parsingstatedelta.py
+-rw-r--r--   0        0        0     8446 2023-04-15 17:12:48.503604 pylatexenc-3.0a17/pylatexenc/latexnodes/_token.py
+-rw-r--r--   0        0        0    27524 2023-04-27 21:49:33.263808 pylatexenc-3.0a17/pylatexenc/latexnodes/_tokenreader.py
+-rw-r--r--   0        0        0    10098 2023-04-15 17:13:31.159345 pylatexenc-3.0a17/pylatexenc/latexnodes/_tokenreaderbase.py
+-rw-r--r--   0        0        0     4841 2023-04-15 17:50:19.637390 pylatexenc-3.0a17/pylatexenc/latexnodes/_walkerbase.py
+-rw-r--r--   0        0        0    42458 2023-04-27 21:51:03.724446 pylatexenc-3.0a17/pylatexenc/latexnodes/nodes.py
+-rw-r--r--   0        0        0     2141 2023-04-15 11:29:53.848262 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/__init__.py
+-rw-r--r--   0        0        0     5285 2023-04-15 11:29:53.848639 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_base.py
+-rw-r--r--   0        0        0    41228 2023-04-27 21:59:01.687959 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_delimited.py
+-rw-r--r--   0        0        0    18288 2023-04-15 11:29:53.849524 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_expression.py
+-rw-r--r--   0        0        0    12896 2023-04-15 11:29:53.849773 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_generalnodes.py
+-rw-r--r--   0        0        0     5658 2023-04-15 11:29:53.849985 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_math.py
+-rw-r--r--   0        0        0     6180 2023-04-15 11:29:53.850252 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_optionals.py
+-rw-r--r--   0        0        0    22370 2023-04-15 16:46:34.476752 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_stdarg.py
+-rw-r--r--   0        0        0    11551 2023-04-18 07:57:57.274724 pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_verbatim.py
+-rw-r--r--   0        0        0     4520 2023-04-15 11:29:53.851132 pylatexenc-3.0a17/pylatexenc/latexwalker/__init__.py
+-rw-r--r--   0        0        0     6214 2023-04-15 11:29:53.851406 pylatexenc-3.0a17/pylatexenc/latexwalker/__main__.py
+-rw-r--r--   0        0        0    17597 2023-04-26 15:29:33.456920 pylatexenc-3.0a17/pylatexenc/latexwalker/_defaultspecs.py
+-rw-r--r--   0        0        0     2937 2023-04-15 11:29:53.852111 pylatexenc-3.0a17/pylatexenc/latexwalker/_get_defaultspecs.py
+-rw-r--r--   0        0        0     7833 2023-04-15 11:29:53.852354 pylatexenc-3.0a17/pylatexenc/latexwalker/_helpers.py
+-rw-r--r--   0        0        0     7487 2023-04-15 11:29:53.852626 pylatexenc-3.0a17/pylatexenc/latexwalker/_legacy_py1x.py
+-rw-r--r--   0        0        0    52642 2023-04-15 11:37:07.707893 pylatexenc-3.0a17/pylatexenc/latexwalker/_walker.py
+-rw-r--r--   0        0        0     2449 2023-05-01 13:36:34.698244 pylatexenc-3.0a17/pylatexenc/macrospec/__init__.py
+-rw-r--r--   0        0        0     8819 2023-04-18 07:57:57.275339 pylatexenc-3.0a17/pylatexenc/macrospec/_argumentsparser.py
+-rw-r--r--   0        0        0     7372 2023-04-15 11:29:53.853904 pylatexenc-3.0a17/pylatexenc/macrospec/_environmentbodyparser.py
+-rw-r--r--   0        0        0    29928 2023-04-27 08:01:22.265622 pylatexenc-3.0a17/pylatexenc/macrospec/_latexcontextdb.py
+-rw-r--r--   0        0        0    10046 2023-04-15 20:38:58.126785 pylatexenc-3.0a17/pylatexenc/macrospec/_macrocallparser.py
+-rw-r--r--   0        0        0     1535 2023-04-15 11:29:53.854841 pylatexenc-3.0a17/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py
+-rw-r--r--   0        0        0     9488 2023-04-18 07:57:57.275664 pylatexenc-3.0a17/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py
+-rw-r--r--   0        0        0    16735 2023-04-18 07:57:57.276084 pylatexenc-3.0a17/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py
+-rw-r--r--   0        0        0    21655 2023-05-01 13:56:41.086895 pylatexenc-3.0a17/pylatexenc/macrospec/_specclasses.py
+-rw-r--r--   0        0        0     8951 2023-04-15 11:29:53.855874 pylatexenc-3.0a17/pylatexenc/macrospec/_spechelpers.py
+-rw-r--r--   0        0        0     2115 2023-05-10 22:59:12.276101 pylatexenc-3.0a17/pylatexenc/version.py
+-rw-r--r--   0        0        0     1091 2023-05-10 22:59:04.979992 pylatexenc-3.0a17/pyproject.toml
+-rw-r--r--   0        0        0     4209 1970-01-01 00:00:00.000000 pylatexenc-3.0a17/PKG-INFO
```

### Comparing `pylatexenc-3.0a15/LICENSE.txt` & `pylatexenc-3.0a17/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/README.rst` & `pylatexenc-3.0a17/README.rst`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/__init__.py` & `pylatexenc-3.0a17/pylatexenc/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/_util.py` & `pylatexenc-3.0a17/pylatexenc/_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,19 +121,19 @@
             setattr(self.obj, self.propname, self.initval)
 
 
 # ------------------------------------------------------------------------------
 
 
 try:
-    from collections import ChainMap #lgtm [py/unused-import]
+    from collections import ChainMap
 except ImportError:
-    pass  #lgtm [py/unnecessary-pass]
+    pass
 ### BEGIN_PYTHON2_SUPPORT_CODE
-    from chainmap import ChainMap #lgtm [py/unused-import]
+    from chainmap import ChainMap
 ### END_PYTHON2_SUPPORT_CODE
 
 
 
 # ------------------------------------------------------------------------------
```

### Comparing `pylatexenc-3.0a15/pylatexenc/_util_support.py` & `pylatexenc-3.0a17/pylatexenc/_util_support.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latex2text/__init__.py` & `pylatexenc-3.0a17/pylatexenc/latex2text/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latex2text/__main__.py` & `pylatexenc-3.0a17/pylatexenc/latex2text/__main__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latex2text/_defaultspecs.py` & `pylatexenc-3.0a17/pylatexenc/latex2text/_defaultspecs.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latex2text/_inputlatexfile.py` & `pylatexenc-3.0a17/pylatexenc/latex2text/_inputlatexfile.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexencode/__init__.py` & `pylatexenc-3.0a17/pylatexenc/latexencode/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,59 +88,61 @@
 
 import unicodedata
 import logging
 import sys
 import functools
 import itertools
 
+### BEGIN_PYTHON2_SUPPORT_CODE
 if sys.version_info.major > 2:
     unicode = str # need to support unicode() w/ no arguments
     basestring = str
-    # use MappingProxyType for keeping
-    from types import MappingProxyType as _MappingProxyType
-    # inspect function argument names
-    from inspect import getfullargspec
-else:
-    _MappingProxyType = dict
-    # inspect function argument names -- simulate getfullargspec with getargspec (argh...)
-    from inspect import getargspec as getfullargspec
 
-logger = logging.getLogger(__name__)
+### END_PYTHON2_SUPPORT_CODE
+
 
+logger = logging.getLogger(__name__)
 
 
 from .. import _util
 
 
 # ------------------------------------------------
 
 
 from ._unicode_to_latex_encoder import (
-    get_builtin_uni2latex_dict,
     RULE_DICT,
     RULE_REGEX,
     RULE_CALLABLE,
     UnicodeToLatexConversionRule,
-    get_builtin_conversion_rules,
     UnicodeToLatexEncoder,
 )
+#    get_builtin_uni2latex_dict,
+#    get_builtin_conversion_rules,
+
+### BEGIN_PYLATEXENC_GET_DEFAULT_SPECS_FN
+from .get_builtin_rules import (
+    get_builtin_uni2latex_dict, get_builtin_conversion_rules
+)
+### END_PYLATEXENC_GET_DEFAULT_SPECS_FN
 
 
 
 # ------------------------------------------------
 
 from ._partial_latex_encoder import (
     PartialLatexToLatexEncoder,
 )
 
 
 
 # ------------------------------------------------
 
 
+### BEGIN_PYLATEXENC1_LEGACY_SUPPORT_CODE
 
 _u2l_obj_cache = {}
 
 
 def unicode_to_latex(s, non_ascii_only=False, replacement_latex_protection='braces',
                      unknown_char_policy='keep', unknown_char_warning=True):
     r"""
@@ -323,10 +325,8 @@
                 else:
                     # keep unescaped char
                     result += ch
 
     return result
 
 
-
-
-
+### END_PYLATEXENC1_LEGACY_SUPPORT_CODE
```

### Comparing `pylatexenc-3.0a15/pylatexenc/latexencode/__main__.py` & `pylatexenc-3.0a17/pylatexenc/latexencode/__main__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexencode/_partial_latex_encoder.py` & `pylatexenc-3.0a17/pylatexenc/latexencode/_partial_latex_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,16 @@
 
 from ._unicode_to_latex_encoder import (
     RULE_CALLABLE,
     UnicodeToLatexConversionRule,
     UnicodeToLatexEncoder
 )
 
-# if sys.version_info.major == 2:
-#     bytes = str
-#     str = unicode
 
+from ..latexwalker import _walker
 
 
 class PartialLatexToLatexEncoder(UnicodeToLatexEncoder):
     r"""
     Encode a string while preserving some (fuzzily detected) LaTeX constructs
     that the input string already has (e.g. accent macros or inline math modes).
 
@@ -64,15 +62,16 @@
     `keep_latex_chars` are to be interpreted as LaTeX and are not to be further
     encoded.
 
     .. versionadded: 2.10
     """
     def __init__(self,
                  # keyword arguments:
-                 keep_latex_chars=r'\${}^_', conversion_rules=None,
+                 keep_latex_chars=r'\${}^_',
+                 conversion_rules=None,
                  **kwargs):
 
         base_conversion_rules = conversion_rules
         if base_conversion_rules is None:
             base_conversion_rules = ['defaults']
 
         super(PartialLatexToLatexEncoder, self).__init__(
@@ -95,19 +94,17 @@
         :py:class:`UnicodeToLatexEncoder` object.
 
         The strategy is to see if we have something that looks like a LaTeX char
         we want to keep.  If so, keep it as is; if not, return `None` so that
         further rules can be considered by the base unicode encoder.
         """
 
-        from ..latexwalker import LatexWalker
-
         if s[pos] in self.keep_latex_chars:
             # Read a token and if it is a macro, keep the full macro!
-            lw = LatexWalker(s, tolerant_parsing=False)
+            lw = _walker.LatexWalker(s, tolerant_parsing=False)
             ps = lw.make_parsing_state()
             tok = lw.make_token_reader(pos=pos).peek_token(parsing_state=ps)
 
             tok_as_latex = tok.pre_space + s[tok.pos : tok.pos+tok.len]
 
             # keep the LaTeX token as-is
             return (tok.pos+tok.len - pos, tok_as_latex)
```

### Comparing `pylatexenc-3.0a15/pylatexenc/latexencode/_uni2latexmap.py` & `pylatexenc-3.0a17/pylatexenc/latexencode/_uni2latexmap.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexencode/_uni2latexmap_xml.py` & `pylatexenc-3.0a17/pylatexenc/latexencode/_uni2latexmap_xml.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/__init__.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/_callablespecbase.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/_callablespecbase.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/_exctypes.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/_exctypes.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/_latexcontextdbbase.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/_latexcontextdbbase.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/_nodescollector.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/_nodescollector.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,22 +44,22 @@
 
 
 class LatexNodesCollector(object):
     r"""
     Process a stream of LaTeX tokens and convert them into a list of nodes.
 
     The `LatexNodesCollector` class functions hand-in-hand with parsers to
-    transform tokens into nodes.  The parser sets up the parsing state
-    correctly, checks the input against errors such as missing mandatory
-    arguments, and then typically defers to a `LatexNodesCollector` instance to
-    actually parse a bulk of contents.  The `LatexNodesCollector` instance, on
-    the other hand, recurses down to calling parsers when we encounter new
-    macros, environments, specials, etc. in the bulk that is being parsed.  The
-    result is a node list containing a full tree of child nodes that represents
-    the logical structure of the tokens that were encountered.
+    transform tokens into nodes.  A parser such as
+    :py:class:`~pylatexenc.latexnodes.parsers.LatexGeneralNodesParser` might set
+    up the parsing state correctly and then defer to a `LatexNodesCollector`
+    instance to actually parse a bulk of contents.  The `LatexNodesCollector`
+    instance, on the other hand, recurses down to calling parsers when we
+    encounter new macros, environments, specials, etc. in the bulk that is being
+    parsed.  The result is a node list containing a full tree of child nodes
+    that represents the logical structure of the tokens that were encountered.
     
     The public API of this class resides essentially in the
     :py:meth:`process_tokens()`, as well as the :py:meth:`get_final_nodelist()`
     (and some other friends, see docs below).
 
 
     .. versionadded:: 3.0
@@ -143,15 +143,16 @@
 
 
 
     def get_final_nodelist(self):
         r"""
         Returns the final nodelist collected from the processed tokens.
 
-        The return value is a :py:class:`LatexNodeList` instance.
+        The return value is a
+        :py:class:`~pylatexenc.latexnodes.nodes.LatexNodeList` instance.
         """
         if not self._finalized:
             raise RuntimeError("Call to get_final_nodelist() before finalize()")
 
         return self.latex_walker.make_nodelist(
             nodelist=self._nodelist,
             parsing_state=self.start_parsing_state,
```

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/_parsedargs.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/_parsedargs.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,16 +263,14 @@
         Called when we export the node structure to JSON when running latexwalker in
         command-line.
 
         Return a representation of the current parsed arguments in an object,
         typically a dictionary, that can easily be exported to JSON.  The object
         may contain latex nodes and other parsed-argument objects, as we use a
         custom JSON encoder that understands these types.
-
-        Subclasses may
         """
 
         return dict(
             arguments_spec_list=self.arguments_spec_list,
             argnlist=self.argnlist,
         )
```

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/_parsedargsinfo.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/_parsedargsinfo.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/_parsingstate.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/_parsingstate.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/_parsingstatedelta.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/_parsingstatedelta.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,22 +42,14 @@
     mode; the definition of a new macro causing the latex context to change;
     etc. etc.
 
     There are many ways in which the parsing state can change, and this is
     reflected in the many different subclasses of `ParsingStateDelta` (e.g.,
     :py:class:`ParsingStateDeltaEnterMathMode`).
 
-    It is the :py:class:`LatexWalkerBase` class that is being used that is
-    responsible for actually updating a parsing state according to a
-    `ParsingStateDelta` object.  Of course, `ParsingStateDelta` objects offer a
-    `get_updated_parsing_state()` method that should minimally implement this
-    parsing state change.  Yet the walker instance may take additional
-    initiatives, for instance, changing the latex context as a consequence of a
-    change to/from math mode.
-
     This class serves both as a base class for general parsing state changes, as
     well as a simple implementation of a parsing state change based on parsing
     state attributes that are to be changed.
     """
     def __init__(self, set_attributes=None, _fields=None, **kwargs):
         super(ParsingStateDelta, self).__init__(**kwargs)
         self.set_attributes = dict(set_attributes) if set_attributes else None
```

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/_token.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/_token.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/_tokenreader.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/_tokenreader.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/_tokenreaderbase.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/_tokenreaderbase.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/_walkerbase.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/_walkerbase.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/nodes.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,22 @@
 
     Use :py:meth:`nodeType()` to figure out what type of node this is, and
     :py:meth:`isNodeType()` to test whether it is of a given type.
 
     You should use :py:meth:`LatexWalker.make_node()` to create nodes, so that
     the latex walker has the opportunity to do some additional setting up.
 
+    .. versionchanged: 3.0
+    
+       This class (along with its canonical subclasses) is located in the module
+       :py:mod:`pylatexenc.latexnodes.nodes` starting in `pylatexenc 3.0`.  It
+       is aliased in :py:mod:`pylatexenc.latexwalker` for backwards
+       compatibility.
+
+
     All nodes have the following attributes:
 
     .. py:attribute:: parsing_state
 
        The parsing state at the time this node was created.  This object stores
        additional context information for this node, such as whether or not this
        node was parsed in a math mode block of LaTeX code.
```

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/__init__.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_base.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_base.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_delimited.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_delimited.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,16 +75,17 @@
 
 
 # LatexDelimitedGroupContentsParserInfo
 
 
 class LatexDelimitedExpressionParserInfo(object):
     r"""
-    Class that specifies how to parse a LaTeX chunk of code that is delimited by
-    specific delimiters (a "delimited group").
+    Class that specifies how to parse a LaTeX chunk of code that is
+    delimited by specific delimiters (a "delimited group").  Helper class for
+    :py:class:`LatexDelimitedExpressionParser`.
 
     This class determines specific aspects of what type of delimited LaTeX code
     we should be reading, such as whether the delimiters are actual LaTeX group
     delimiters, or if they are math mode delimiters, or if they are verbatim
     delimiters, etc.
 
     Some static/class methods are crucial for determining how the beginning of
@@ -805,15 +806,18 @@
 
 
 
 
 # ------------------------------------------------
 
 class LatexDelimitedGroupParserInfo(LatexDelimitedExpressionParserInfo):
-
+    r"""
+    Helper class for :py:class:`LatexDelimitedGroupParser`.  See also
+    :py:class:`LatexDelimitedExpressionParserInfo`.
+    """
 
     @classmethod
     def get_group_parsing_state(cls, parsing_state, delimiters, delimited_expression_parser,
                                 latex_walker, **kwargs):
         r"""
         Return the parsing state object to use for the overall group.  This is the
         parsing state that will be attached to the resulting
```

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_expression.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_expression.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_generalnodes.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_generalnodes.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_math.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_math.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_optionals.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_optionals.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_stdarg.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_stdarg.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_verbatim.py` & `pylatexenc-3.0a17/pylatexenc/latexnodes/parsers/_verbatim.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexwalker/__init__.py` & `pylatexenc-3.0a17/pylatexenc/latexwalker/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexwalker/__main__.py` & `pylatexenc-3.0a17/pylatexenc/latexwalker/__main__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexwalker/_defaultspecs.py` & `pylatexenc-3.0a17/pylatexenc/latexwalker/_defaultspecs.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexwalker/_get_defaultspecs.py` & `pylatexenc-3.0a17/pylatexenc/latexwalker/_get_defaultspecs.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexwalker/_helpers.py` & `pylatexenc-3.0a17/pylatexenc/latexwalker/_helpers.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexwalker/_legacy_py1x.py` & `pylatexenc-3.0a17/pylatexenc/latexwalker/_legacy_py1x.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/latexwalker/_walker.py` & `pylatexenc-3.0a17/pylatexenc/latexwalker/_walker.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/macrospec/__init__.py` & `pylatexenc-3.0a17/pylatexenc/macrospec/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,20 @@
 .. versionadded:: 2.0
 
    The entire module :py:mod:`pylatexenc.macrospec` was introduced in
    `pylatexenc 2.0`.
 """
 
 
-from ._specclasses import MacroSpec, EnvironmentSpec, SpecialsSpec
+from ._specclasses import (
+    CallableSpec,
+    MacroSpec,
+    EnvironmentSpec,
+    SpecialsSpec,
+)
 
 ### BEGIN_PYLATEXENC2_LEGACY_SUPPORT_CODE
 from ._spechelpers import std_macro, std_environment, std_specials
 ### END_PYLATEXENC2_LEGACY_SUPPORT_CODE
 
 
 from ._latexcontextdb import (
```

### Comparing `pylatexenc-3.0a15/pylatexenc/macrospec/_argumentsparser.py` & `pylatexenc-3.0a17/pylatexenc/macrospec/_argumentsparser.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/macrospec/_environmentbodyparser.py` & `pylatexenc-3.0a17/pylatexenc/macrospec/_environmentbodyparser.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/macrospec/_latexcontextdb.py` & `pylatexenc-3.0a17/pylatexenc/macrospec/_latexcontextdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -435,25 +435,29 @@
                     "Invalid latex environment spec db category: {!r} (Expected one of {!r})"
                     .format(c, self.category_list)
                 )
             for spec in self.d[c]['specials'].values():
                 yield spec
 
 
+### BEGIN_PYLATEXENC2_LEGACY_SUPPORT_CODE
+
     def filter_context(self, *args, **kwargs):
         r"""
         .. deprecated:: 3.0
 
            The `filter_context()` method was renamed `filtered_context()`.  The
            method signature is unchanged.
         """
         _util.pylatexenc_deprecated_3("`LatexContextDb.filter_context()` was renamed to "
                                       "`filtered_context()`.")
         return self.filtered_context(*args, **kwargs)
 
+### END_PYLATEXENC2_LEGACY_SUPPORT_CODE
+
 
     def filtered_context(self, keep_categories=[], exclude_categories=[],
                          keep_which=[], create_class=None):
         r"""
         Return a new :py:class:`LatexContextDb` instance where we only keep
         certain categories of macro and environment specifications.
         
@@ -473,14 +477,19 @@
         keep.  It should be a subset of the list ['macros', 'environments',
         'specials'].
         
         The returned context will make a copy of the dictionaries that store the
         macro and environment specifications, but the specification classes (and
         corresponding argument parsers) might correspond to the same instances.
         I.e., the returned context is not a full deep copy.
+
+        .. versionadded:: 3.0
+
+           The `filter_context()` method was renamed `filtered_context()` in
+           `pylatexenc 3.0`.
         """
         
         if create_class is None:
             create_class = self.__class__
 
         new_context = create_class()
```

### Comparing `pylatexenc-3.0a15/pylatexenc/macrospec/_macrocallparser.py` & `pylatexenc-3.0a17/pylatexenc/macrospec/_macrocallparser.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py` & `pylatexenc-3.0a17/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py` & `pylatexenc-3.0a17/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py` & `pylatexenc-3.0a17/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/macrospec/_specclasses.py` & `pylatexenc-3.0a17/pylatexenc/macrospec/_specclasses.py`

 * *Files 20% similar despite different names*

```diff
@@ -54,150 +54,269 @@
     _basestring = basestring
 ### END_PYTHON2_SUPPORT_CODE
 
 
 _legacy_pyltxenc2_do = lambda *args: None
 
 
-class _SpecBase(CallableSpecBase):
+class _NotSpecified:
+    pass
+
+
+class CallableSpec(CallableSpecBase):
+    r"""
+    Base class for :py:class:`MacroSpec`, :py:class:`EnvironmentSpec` and
+    :py:class:`SpecialsSpec` classes regrouping common functionality.
+
+    Doc. ................
+
+    One of the main reasons for bringing all the default functionality of the
+    :py:class:`MacroSpec`, :py:class:`EnvironmentSpec`, and
+    :py:class:`SpecialsSpec` classes together in the same base class is to
+    facilitate creating richer derived spec classes.  For instance, the `flm
+    <https://github.com/phfaist/flm>`_ project needs to supplement spec classes
+    with additional information, e.g., about how to render the node in
+    appropriate output formats.  In such cases, it suffices to inherit
+    `CallableSpec` to implement the desired functionality, and instantiate such
+    classes directly (or recreate lightweight derived versions for macros,
+    environments, and specials), rather than have to play around with multiple
+    inheritance or other such tricks to simultaneously implement new base
+    functionality that is common to macro, environment, and specials parsing.
+    """
+
     def __init__(self,
-                 arguments_spec_list=None,
+                 arguments_spec_list,
+                 #*,
+                 spec_node_parser_type,
+                 macroname=_NotSpecified,
+                 environmentname=_NotSpecified,
+                 specials_chars=_NotSpecified,
                  make_arguments_parsing_state_delta=None,
                  make_body_parsing_state_delta=None,
                  make_after_parsing_state_delta=None,
-                 finalize_node=None, **kwargs):
+                 make_body_parser=None,
+                 finalize_node=None,
+                 **kwargs):
 
         self.arguments_spec_list = arguments_spec_list
 
-        self._fn_make_arguments_parsing_state_delta = make_arguments_parsing_state_delta
-        self._fn_make_body_parsing_state_delta = make_body_parsing_state_delta
-        self._fn_make_after_parsing_state_delta = make_after_parsing_state_delta
-        self._fn_finalize_node = finalize_node
+        self.spec_node_parser_type = spec_node_parser_type
+        if macroname is not _NotSpecified:
+            self.macroname = macroname
+        if environmentname is not _NotSpecified:
+            self.environmentname = environmentname
+        if specials_chars is not _NotSpecified:
+            self.specials_chars = specials_chars
+
+        # Internal convention: if any of the _fn_*** attributes are set, they
+        # should NOT be set to None.  They should simply not be set.  We're
+        # testing for their presence with hasattr(self, '_fn_***').
+
+        if make_arguments_parsing_state_delta is not None:
+            self._fn_make_arguments_parsing_state_delta = make_arguments_parsing_state_delta
+        if make_body_parsing_state_delta is not None:
+            self._fn_make_body_parsing_state_delta = make_body_parsing_state_delta
+        if make_after_parsing_state_delta is not None:
+            self._fn_make_after_parsing_state_delta = make_after_parsing_state_delta
+        if make_body_parser is not None:
+            self._fn_make_body_parser = make_body_parser
+        if finalize_node is not None:
+            self._fn_finalize_node = finalize_node
 
         # note, the following might set self._fn_make_***_parsing_state_delta:
         use_legacy_args_parser = _legacy_pyltxenc2_do(
-            'SpecBase_init_from_args_parser', self, arguments_spec_list, kwargs
+            'CallableSpec_init_from_args_parser', self, arguments_spec_list, kwargs
         )
 
-        super(_SpecBase, self).__init__(**kwargs)
+        # for environments---
+        # body_parsing_state_delta is the default delta object if no
+        # "make_body_parsing_state_delta" function is provided or overridden
+        body_parsing_state_delta = kwargs.pop('body_parsing_state_delta', None)
+
+### BEGIN_PYLATEXENC2_LEGACY_SUPPORT_CODE
+        self.is_math_mode = kwargs.pop('is_math_mode', None) # obsolete !
+        if self.is_math_mode:
+            if body_parsing_state_delta is None:
+                body_parsing_state_delta = ParsingStateDeltaEnterMathMode()
+            else:
+                raise ValueError("You cannot specify both is_math_mode= and "
+                                 "body_parsing_state_delta=")
+### END_PYLATEXENC2_LEGACY_SUPPORT_CODE
+
+        self.body_parsing_state_delta = body_parsing_state_delta
+
+        super(CallableSpec, self).__init__(**kwargs)
 
         if not use_legacy_args_parser:
             if self.arguments_spec_list:
                 self.arguments_parser = LatexArgumentsParser(arguments_spec_list)
             else:
                 self.arguments_parser = LatexNoArgumentsParser()
 
 
+    def get_node_parser(self, token):
+        r"""
+        Return a parser instance that is capable of parsing this node
+        construct.
+
+        This base class instantiates and returns an object of the type
+        `spec_node_parser_type` that was specified to the constructor.  (This
+        type is set to :py:class:`LatexMacroCallParser`,
+        :py:class:`LatexEnvironmentCallParser`, or
+        :py:class:`LatexSpecialsCallParser` by the corresponding subclasses
+        :py:class:`MacroSpec`, :py:class:`EnvironmentSpec`, or
+        :py:class:`SpecialsSpec`.)  The given type's constructor is assumed to
+        accept to positional arguments to which the token object `token` and the
+        present spec instance (`self`) are passed.
+        """
+        return self.spec_node_parser_type(token, self)
+
 ### BEGIN_PYLATEXENC2_LEGACY_SUPPORT_CODE
 
     @property
     def args_parser(self):
         return self.arguments_parser
 
 ### END_PYLATEXENC2_LEGACY_SUPPORT_CODE
 
 
     def finalize_node(self, node):
         r"""
-        ................
+        Doc ................
 
         MUST RETURN the new node instance.
 
         This is called from the LatexMacroCallParser instance, i.e., this
         function won't be called by default if you override get_node_parser()
         and return a different parser instance.
         """
 
-        if self._fn_finalize_node is not None:
+        # Transcrypt doesn't seem to like getattr(obj, attrname, default) with
+        # default arg, so use hasattr() test
+        if hasattr(self, '_fn_finalize_node'): # and self._fn_finalize_node is not None:
             return self._fn_finalize_node(node)
 
         return node
 
 
     def make_arguments_parsing_state_delta(self, token, latex_walker):
-        if self._fn_make_arguments_parsing_state_delta is not None:
+        r"""
+        Doc ................
+        """
+        # Transcrypt doesn't seem to like getattr(obj, attrname, default) with
+        # default arg, so use hasattr() test
+        if (
+                hasattr(self, '_fn_make_arguments_parsing_state_delta')
+                #and self._fn_make_arguments_parsing_state_delta is not None
+        ):
             return self._fn_make_arguments_parsing_state_delta(
                 token=token,
                 latex_walker=latex_walker
             )
         return None
 
     def make_body_parsing_state_delta(self,
                                       token,
                                       nodeargd,
                                       arg_parsing_state_delta,
                                       latex_walker):
         r"""
-        ...........
+        Doc ................
 
         This method only makes sense for LaTeX environments.  It's defined in
-        the base class :py:class:`_SpecBase` for consistency with the other
+        the base class :py:class:`CallableSpec` for consistency with the other
         `make_**_parsing_state_delta()` methods.  This base class
         implementation, if no custom body parsing state delta function is set in
         the constructor, relies on `self.body_parsing_state_delta` being available!
 
         Note: `arg_parsing_state_delta` is always `None` (unless you actually
         went ahead and replaced the the `arguments_parser` attribute, which is a
-        `LatexArgumentsParser` or `LatexNoArgumentsParser` instance, by a custom
-        parser).
+        :py:class:`LatexArgumentsParser` or :py:class:`LatexNoArgumentsParser`
+        instance, by a custom parser).
         """
-        if self._fn_make_body_parsing_state_delta is not None:
+        if (
+                hasattr(self, '_fn_make_body_parsing_state_delta')
+                #and self._fn_make_body_parsing_state_delta is not None
+        ):
             return self._fn_make_body_parsing_state_delta(
                 token=token,
                 nodeargd=nodeargd,
                 arg_parsing_state_delta=arg_parsing_state_delta,
                 latex_walker=latex_walker,
             )
 
         # default implementation checks the body_parsing_state_delta attribute
         return self.body_parsing_state_delta
 
 
     def make_after_parsing_state_delta(self, parsed_node, latex_walker):
         r"""
-        If applicable, create a :py:class:`ParsingStateDelta` class to convey any
+        If applicable, create a
+        :py:class:`~pylatexenc.latexnodes.ParsingStateDelta` class to convey any
         changes in the parsing state after completing this callable node.
         
         The default implementation returns `None`.  You may, but do not have to,
         override this method to customize its behavior.  You can specify a
         custom callable to `make_after_parsing_state_delta=...` in the
-        constructor, and the constructor will reassign the attribute
-        `spec.make_after_parsing_state_delta` to that callable.
-
+        constructor which will be invoked in this method.
 
-        This is called from the LatexMacroCallParser instance, i.e., this
-        function won't be called by default if you override get_node_parser()
-        and return a different parser instance.
+        This method is called from the :py:class:`LatexMacroCallParser`
+        instance, i.e., this function won't be called by default if you override
+        :py:meth:`get_node_parser()` and return a different parser instance.
         """
-        if self._fn_make_after_parsing_state_delta is not None:
+        if (
+                hasattr(self, '_fn_make_after_parsing_state_delta')
+                #and self._fn_make_after_parsing_state_delta is not None
+        ):
             return self._fn_make_after_parsing_state_delta(
                 parsed_node=parsed_node,
                 latex_walker=latex_walker,
             )
         return None
 
 
     def needs_arguments(self):
+        r"""
+        Doc ................
+        """
         for arg in self.arguments_spec_list:
             if arg.spec.is_required():
                 return True
         return False
 
+
+    def make_body_parser(self, token, nodeargd, arg_parsing_state_delta):
+        r"""
+        Doc. ................
+
+        For environment specs only. ........
+        """
+        if hasattr(self, '_fn_make_body_parser'): # and self._fn_make_body_parser is not None:
+            return self._fn_make_body_parser(token, nodeargd, arg_parsing_state_delta)
+        return LatexEnvironmentBodyContentsParser(
+            environmentname=token.arg,
+        )
+
+
     def __repr__(self):
         return (
             self.__class__.__name__ + "(" +
-            ", ".join([ "{}={!r}".format(k,v)
-                        for (k,v) in self.__dict__.items()
-                        if not k.startswith("_") ])
+            ", ".join([
+                "{}={!r}".format(k,v)
+                for (k,v) in self.__dict__.items()
+                if (not k.startswith("_")
+                    and v is not None
+                    and k not in ('spec_node_parser_type', ))
+            ])
             + ")"
         )
     
 
 
-class MacroSpec(_SpecBase):
+class MacroSpec(CallableSpec):
     r"""
     Stores the specification of a macro.
 
     This stores the macro name and instructions on how to parse the macro
     arguments.
 
     .. py:attribute:: macroname
@@ -209,118 +328,127 @@
        The parser instance that can understand this macro's arguments.  For
        standard LaTeX macros this is usually a
        :py:class:`MacroStandardArgsParser` instance.
 
        If you specify a string, then for convenience this is interpreted as an
        argspec argument for :py:class:`MacroStandardArgsParser` and such an
        instance is automatically created.
+
+       .. deprecated:: 3.0
+
+           The `args_parser` attribute is deprecated since `pylatexenc 3.0`.  Macro,
+           environment, and specials specification classes now return more general
+           parsers meant to handle the entire macro/environment/specials invocation,
+           not only their arguments, via the :meth:`get_node_parser()` method.
     """
     def __init__(self, macroname, arguments_spec_list=None, **kwargs):
-        super(MacroSpec, self).__init__(arguments_spec_list=arguments_spec_list,
-                                        **kwargs)
-
-        self.macroname = macroname
+        super(MacroSpec, self).__init__(
+            arguments_spec_list=arguments_spec_list,
+            spec_node_parser_type=LatexMacroCallParser,
+            macroname=macroname,
+            **kwargs
+        )
+        #self.macroname = macroname
 
-    def get_node_parser(self, token):
-        return LatexMacroCallParser(token, self)
+    # def get_node_parser(self, token):
+    #     r"""
+    #     Doc.........
+    #     """
+    #     return LatexMacroCallParser(token, self)
 
 
 
 
-class EnvironmentSpec(_SpecBase):
+class EnvironmentSpec(CallableSpec):
     r"""
     Stores the specification of a LaTeX environment.
 
     This stores the environment name and instructions on how to parse any
     arguments provided after ``\begin{environment}<args>``.
 
+    .. note::
+
+       Starred variants of environments (as in ``\begin{equation*}``) must not
+       be specified using an argspec as for macros (e.g., `argspec='*'`).
+       Rather, we need to define a separate environment spec for the starred
+       variant with the star in the name itself (``EnvironmentSpec('equation*',
+       None)``) because the star really is part of the environment name.  If you
+       happened to use ``EnvironmentSpec('equation', '*')``, then the parser
+       would recognize the expression ``\begin{equation}*`` but not
+       ``\begin{equation*}``.
+
     .. py:attribute:: environmentname
 
        The name of the environment, i.e., the argument of ``\begin{...}`` and
        ``\end{...}``.
 
+    .. py:attribute:: body_parsing_state_delta
+
+       The parsing state changes that are set in order to parse the body
+       contents of the environment.
+
+
     .. py:attribute:: args_parser
 
        The parser instance that can understand this environment's arguments.
        For standard LaTeX environment this is usually a
        :py:class:`MacroStandardArgsParser` instance.
 
        If you specify a string, then for convenience this is interpreted as an
        argspec argument for :py:class:`MacroStandardArgsParser` and such an
        instance is automatically created.
 
+       .. deprecated:: 3.0
+
+           The `args_parser` attribute is deprecated since `pylatexenc 3.0`.  Macro,
+           environment, and specials specification classes now return more general
+           parsers meant to handle the entire macro/environment/specials invocation,
+           not only their arguments, via the :meth:`get_node_parser()` method.
+
     .. py:attribute:: is_math_mode
 
        Indicates if the contents is to be interpreted in Math Mode.  This would
        be `True` for environments like ``\begin{equation}``, ``\begin{align}``,
        etc., but is left to `None` for ``\begin{figure}``, etc.
 
        .. deprecated:: 3.0
 
           The field `is_math_mode` was deprecated in `pylatexenc 3` in favor of
           the field `body_parsing_state_delta`.  Instead of `is_math_mode=True`,
           use `body_parsing_state_delta=ParsingStateDeltaEnterMathMode()`.
-
-    .. py:attribute:: body_parsing_state_delta
-
-       The parsing state changes that are set in order to parse the body
-       contents of the environment.
-
-    .. note::
-
-       Starred variants of environments (as in ``\begin{equation*}``) must not
-       be specified using an argspec as for macros (e.g., `argspec='*'`).
-       Rather, we need to define a separate environment spec for the starred
-       variant with the star in the name itself (``EnvironmentSpec('equation*',
-       None)``) because the star really is part of the environment name.  If you
-       happened to use ``EnvironmentSpec('equation', '*')``, then the parser
-       would recognize the expression ``\begin{equation}*`` but not
-       ``\begin{equation*}``.
     """
     def __init__(self, environmentname, arguments_spec_list=None, **kwargs):
 
-        make_body_parser = kwargs.pop('make_body_parser', None)
-        body_parsing_state_delta = kwargs.pop('body_parsing_state_delta', None)
-
-### BEGIN_PYLATEXENC2_LEGACY_SUPPORT_CODE
-        is_math_mode = kwargs.pop('is_math_mode', None) # obsolete !
-### END_PYLATEXENC2_LEGACY_SUPPORT_CODE
-
         super(EnvironmentSpec, self).__init__(
             arguments_spec_list=arguments_spec_list,
+            spec_node_parser_type=LatexEnvironmentCallParser,
+            environmentname=environmentname,
             **kwargs
         )
+        #self.environmentname = environmentname
 
-### BEGIN_PYLATEXENC2_LEGACY_SUPPORT_CODE
-        self.is_math_mode = is_math_mode
-        if is_math_mode:
-            if body_parsing_state_delta is None:
-                body_parsing_state_delta = ParsingStateDeltaEnterMathMode()
-            else:
-                raise ValueError("You cannot specify both is_math_mode= and "
-                                 "body_parsing_state_delta=")
-### END_PYLATEXENC2_LEGACY_SUPPORT_CODE
+    # def get_node_parser(self, token):
+    #     r"""
+    #     Doc.........
+    #     """
+    #     return LatexEnvironmentCallParser(token, self)
+
+    # def make_body_parser(self, token, nodeargd, arg_parsing_state_delta):
+    #     r"""
+    #     Doc. ................
+    #     """
+    #     if self._fn_make_body_parser is not None:
+    #         return self._fn_make_body_parser(token, nodeargd, arg_parsing_state_delta)
+    #     return LatexEnvironmentBodyContentsParser(
+    #         environmentname=token.arg,
+    #     )
 
-        self.environmentname = environmentname
-        self.body_parsing_state_delta = body_parsing_state_delta
-        self._fn_make_body_parser = make_body_parser
 
-    def get_node_parser(self, token):
-        return LatexEnvironmentCallParser(token, self)
 
-    def make_body_parser(self, token, nodeargd, arg_parsing_state_delta):
-        if self._fn_make_body_parser is not None:
-            return self._fn_make_body_parser(token, nodeargd, arg_parsing_state_delta)
-        return LatexEnvironmentBodyContentsParser(
-            environmentname=token.arg,
-        )
-
-
-
-class SpecialsSpec(_SpecBase):
+class SpecialsSpec(CallableSpec):
     r"""
     Specification of a LaTeX "special char sequence": an active char, a
     ligature, or some other non-macro char sequence that has a special meaning.
 
     For instance, '&', '~', and '``' are considered as "specials".
 
     .. py:attribute:: specials_chars
@@ -329,27 +457,41 @@
        '&', '~', '``', etc.
 
     .. py:attribute:: args_parser
     
        A parser (e.g. :py:class:`MacroStandardArgsParser`) that is invoked when
        the specials is encountered.  Can/should be set to `None` if the specials
        should not parse any arguments (e.g. '~').
-    """
-    def __init__(self, specials_chars, arguments_spec_list=None, **kwargs):
-        super(SpecialsSpec, self).__init__(arguments_spec_list=arguments_spec_list, **kwargs)
 
-        self.specials_chars = specials_chars
+       .. deprecated:: 3.0
 
-    def __repr__(self):
-        return 'SpecialsSpec(specials_chars={!r}, arguments_spec_list={!r})'.format(
-            self.specials_chars, self.arguments_spec_list
+           The `args_parser` attribute is deprecated since `pylatexenc 3.0`.  Macro,
+           environment, and specials specification classes now return more general
+           parsers meant to handle the entire macro/environment/specials invocation,
+           not only their arguments, via the :meth:`get_node_parser()` method.
+    """
+    def __init__(self, specials_chars, arguments_spec_list=None, **kwargs):
+        super(SpecialsSpec, self).__init__(
+            arguments_spec_list=arguments_spec_list,
+            spec_node_parser_type=LatexSpecialsCallParser,
+            specials_chars=specials_chars,
+            **kwargs
         )
+        #self.specials_chars = specials_chars
 
-    def get_node_parser(self, token):
-        return LatexSpecialsCallParser(token, self)
+    # def __repr__(self):
+    #     return 'SpecialsSpec(specials_chars={!r}, arguments_spec_list={!r})'.format(
+    #         self.specials_chars, self.arguments_spec_list
+    #     )
+
+    # def get_node_parser(self, token):
+    #     r"""
+    #     Doc.........
+    #     """
+    #     return LatexSpecialsCallParser(token, self)
 
 
 
 
 
 ### BEGIN_PYLATEXENC2_LEGACY_SUPPORT_CODE
 
@@ -357,15 +499,15 @@
 
 from ..latexnodes import ParsingStateDeltaReplaceParsingState
 
 _legacy_pyltxenc2_do = \
     lambda what, *args: globals()['_legacy_pyltxenc2_'+what](*args)
 
 
-def _legacy_pyltxenc2_SpecBase_init_from_args_parser(spec, arguments_spec_list, kwargs):
+def _legacy_pyltxenc2_CallableSpec_init_from_args_parser(spec, arguments_spec_list, kwargs):
 
     def _make_after_parsing_state_delta(parsed_node, spec=spec, **kwargs):
         new_parsing_state = getattr(parsed_node.nodeargd,
                                     '_legacy_pyltxenc2_new_parsing_state',
                                     None)
         return ParsingStateDeltaReplaceParsingState(set_parsing_state=new_parsing_state)
 
@@ -402,15 +544,15 @@
     else:
         return _init_with_legacy_wrapper(args_parser)
 
     return False
 
 
 
-def _legacy_pyltxenc2_SpecBase_parse_args(spec, w, pos, parsing_state=None):
+def _legacy_pyltxenc2_CallableSpec_parse_args(spec, w, pos, parsing_state=None):
     r"""
     .. deprecated:: 3.0
 
         This method is not recommented starting from `pylatexenc 3`.  You can
         use parser stored as the `arguments_parser` attribute instead.
     """
 
@@ -421,11 +563,11 @@
     )
 
     if parsing_state_delta is not None:
         return parsed, parsed.pos, parsed.len, parsing_state_delta._to_legacy_pyltxenc2_dict()
 
     return parsed, parsed.pos, parsed.len
 
-_SpecBase.parse_args = _legacy_pyltxenc2_SpecBase_parse_args
+CallableSpec.parse_args = _legacy_pyltxenc2_CallableSpec_parse_args
 
 
 ### END_PYLATEXENC2_LEGACY_SUPPORT_CODE
```

### Comparing `pylatexenc-3.0a15/pylatexenc/macrospec/_spechelpers.py` & `pylatexenc-3.0a17/pylatexenc/macrospec/_spechelpers.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a15/pylatexenc/version.py` & `pylatexenc-3.0a17/pylatexenc/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 #   7) on github.com, fill in release details with a summary of changes etc.
 #
 #   8) create the source package for PyPI (" python3 setup.py sdist ")
 #   
 #   8) upload package to PyPI (twine upload dist/pylatexenc-X.X.tar.gz -r realpypi)
 #
 
-version_str = "3.0alpha000015"
+version_str = "3.0alpha000017"
```

### Comparing `pylatexenc-3.0a15/pyproject.toml` & `pylatexenc-3.0a17/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylatexenc"
-version = "3.0alpha000015" # ALSO BUMP IN pylatexenc/version.py
+version = "3.0alpha000017" # ALSO BUMP IN pylatexenc/version.py
 description = "Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion"
 authors = ["Philippe Faist <philippe.faist@bluewin.ch>"]
 license = "MIT"
 readme = "README.rst"
 
 [tool.poetry.scripts]
 latexwalker = 'pylatexenc.latexwalker.__main__:main'
```

### Comparing `pylatexenc-3.0a15/PKG-INFO` & `pylatexenc-3.0a17/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylatexenc
-Version: 3.0a15
+Version: 3.0a17
 Summary: Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion
 License: MIT
 Author: Philippe Faist
 Author-email: philippe.faist@bluewin.ch
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

