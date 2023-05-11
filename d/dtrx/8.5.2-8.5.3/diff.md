# Comparing `tmp/dtrx-8.5.2.tar.gz` & `tmp/dtrx-8.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtrx-8.5.2.tar", last modified: Fri Apr 28 20:52:20 2023, max compression
+gzip compressed data, was "dtrx-8.5.3.tar", last modified: Thu May 11 18:56:02 2023, max compression
```

## Comparing `dtrx-8.5.2.tar` & `dtrx-8.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2023-04-28 20:52:20.144792 dtrx-8.5.2/
--rw-rw-r--   0 noah      (1000) noah      (1000)    35147 2021-11-24 20:34:36.000000 dtrx-8.5.2/COPYING
--rw-rw-r--   0 noah      (1000) noah      (1000)     6729 2023-04-28 20:52:20.144792 dtrx-8.5.2/PKG-INFO
--rw-rw-r--   0 noah      (1000) noah      (1000)     5611 2023-04-28 20:50:11.000000 dtrx-8.5.2/README.md
-drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2023-04-28 20:52:20.144792 dtrx-8.5.2/dtrx/
--rw-rw-r--   0 noah      (1000) noah      (1000)        0 2022-03-29 02:05:22.000000 dtrx-8.5.2/dtrx/__init__.py
--rwxrwxr-x   0 noah      (1000) noah      (1000)    61917 2023-04-28 20:51:17.000000 dtrx-8.5.2/dtrx/dtrx.py
-drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2023-04-28 20:52:20.144792 dtrx-8.5.2/dtrx.egg-info/
--rw-rw-r--   0 noah      (1000) noah      (1000)     6729 2023-04-28 20:52:20.000000 dtrx-8.5.2/dtrx.egg-info/PKG-INFO
--rw-rw-r--   0 noah      (1000) noah      (1000)      251 2023-04-28 20:52:20.000000 dtrx-8.5.2/dtrx.egg-info/SOURCES.txt
--rw-rw-r--   0 noah      (1000) noah      (1000)        1 2023-04-28 20:52:20.000000 dtrx-8.5.2/dtrx.egg-info/dependency_links.txt
--rw-rw-r--   0 noah      (1000) noah      (1000)       40 2023-04-28 20:52:20.000000 dtrx-8.5.2/dtrx.egg-info/entry_points.txt
--rw-rw-r--   0 noah      (1000) noah      (1000)       99 2023-04-28 20:52:20.000000 dtrx-8.5.2/dtrx.egg-info/requires.txt
--rw-rw-r--   0 noah      (1000) noah      (1000)        5 2023-04-28 20:52:20.000000 dtrx-8.5.2/dtrx.egg-info/top_level.txt
--rw-rw-r--   0 noah      (1000) noah      (1000)      240 2022-03-29 02:05:22.000000 dtrx-8.5.2/pyproject.toml
--rw-rw-r--   0 noah      (1000) noah      (1000)     1311 2023-04-28 20:52:20.144792 dtrx-8.5.2/setup.cfg
--rw-rw-r--   0 noah      (1000) noah      (1000)       88 2022-11-16 14:51:03.000000 dtrx-8.5.2/setup.py
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2023-05-11 18:56:02.714164 dtrx-8.5.3/
+-rw-rw-r--   0 noah      (1000) noah      (1000)    35147 2021-11-24 20:34:36.000000 dtrx-8.5.3/COPYING
+-rw-rw-r--   0 noah      (1000) noah      (1000)     6729 2023-05-11 18:56:02.714164 dtrx-8.5.3/PKG-INFO
+-rw-rw-r--   0 noah      (1000) noah      (1000)     5611 2023-04-28 20:50:11.000000 dtrx-8.5.3/README.md
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2023-05-11 18:56:02.714164 dtrx-8.5.3/dtrx/
+-rw-rw-r--   0 noah      (1000) noah      (1000)        0 2022-03-29 02:05:22.000000 dtrx-8.5.3/dtrx/__init__.py
+-rwxrwxr-x   0 noah      (1000) noah      (1000)    62096 2023-05-11 18:55:13.000000 dtrx-8.5.3/dtrx/dtrx.py
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2023-05-11 18:56:02.714164 dtrx-8.5.3/dtrx.egg-info/
+-rw-rw-r--   0 noah      (1000) noah      (1000)     6729 2023-05-11 18:56:02.000000 dtrx-8.5.3/dtrx.egg-info/PKG-INFO
+-rw-rw-r--   0 noah      (1000) noah      (1000)      251 2023-05-11 18:56:02.000000 dtrx-8.5.3/dtrx.egg-info/SOURCES.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)        1 2023-05-11 18:56:02.000000 dtrx-8.5.3/dtrx.egg-info/dependency_links.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)       40 2023-05-11 18:56:02.000000 dtrx-8.5.3/dtrx.egg-info/entry_points.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)       99 2023-05-11 18:56:02.000000 dtrx-8.5.3/dtrx.egg-info/requires.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)        5 2023-05-11 18:56:02.000000 dtrx-8.5.3/dtrx.egg-info/top_level.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)      240 2022-03-29 02:05:22.000000 dtrx-8.5.3/pyproject.toml
+-rw-rw-r--   0 noah      (1000) noah      (1000)     1311 2023-05-11 18:56:02.714164 dtrx-8.5.3/setup.cfg
+-rw-rw-r--   0 noah      (1000) noah      (1000)       88 2022-11-16 14:51:03.000000 dtrx-8.5.3/setup.py
```

### Comparing `dtrx-8.5.2/COPYING` & `dtrx-8.5.3/COPYING`

 * *Files identical despite different names*

### Comparing `dtrx-8.5.2/PKG-INFO` & `dtrx-8.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtrx
-Version: 8.5.2
+Version: 8.5.3
 Summary: Script to intelligently extract multiple archive types
 Download-URL: https://github.com/dtrx-py/dtrx
 Author: Brett Smith
 Author-email: brettcsmith@brettcsmith.org
 License: GNU General Public License version 3 or later
 Project-URL: homepage, http://www.brettcsmith.org/2007/dtrx/
 Project-URL: code, https://github.com/dtrx-py/dtrx
```

### Comparing `dtrx-8.5.2/README.md` & `dtrx-8.5.3/README.md`

 * *Files identical despite different names*

### Comparing `dtrx-8.5.2/dtrx/dtrx.py` & `dtrx-8.5.3/dtrx/dtrx.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     get_input = raw_input  # noqa: F821
 
 try:
     set
 except NameError:
     from sets import Set as set
 
-VERSION = "8.5.2"
+VERSION = "8.5.3"
 VERSION_BANNER = """dtrx version %s
 Copyright © 2006-2011 Brett Smith <brettcsmith@brettcsmith.org>
 Copyright © 2008 Peter Kelemen <Peter.Kelemen@gmail.com>
 Copyright © 2011 Ville Skyttä <ville.skytta@iki.fi>
 
 This program is free software; you can redistribute it and/or modify it
 under the terms of the GNU General Public License as published by the
@@ -291,16 +291,21 @@
                     # Clean up the error output
                     self.stderr = ""
                     raise ExtractorError(
                         "cannot extract encrypted archive '%s' in non-interactive mode"
                         % (self.filename)
                     )
 
+    def send_stdout_to_dev_null(self):
+        return True
+
     def run_pipes(self, final_stdout=None):
-        has_output_target = True if final_stdout else False
+        has_output_target = (
+            True if final_stdout or self.send_stdout_to_dev_null() else False
+        )
         if not self.pipes:
             return
         elif final_stdout is None:
             final_stdout = open("/dev/null", "w")
         num_pipes = len(self.pipes)
         last_pipe = num_pipes - 1
         processes = []
@@ -709,14 +714,17 @@
                     break
                 else:
                     fn_index = string.rindex(line, " ") + 1
             elif fn_index is not None:
                 yield line[fn_index:]
         self.archive.close()
 
+    def send_stdout_to_dev_null(self):
+        return False
+
     def timeout_check(self, pipe):
         nbs = NonblockingRead(pipe.stdout)
         errs = nbs.readlines()
 
         self.stderr += "".join(errs)
 
         # pass through the password prompt, if 7z sent one
```

### Comparing `dtrx-8.5.2/dtrx.egg-info/PKG-INFO` & `dtrx-8.5.3/dtrx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtrx
-Version: 8.5.2
+Version: 8.5.3
 Summary: Script to intelligently extract multiple archive types
 Download-URL: https://github.com/dtrx-py/dtrx
 Author: Brett Smith
 Author-email: brettcsmith@brettcsmith.org
 License: GNU General Public License version 3 or later
 Project-URL: homepage, http://www.brettcsmith.org/2007/dtrx/
 Project-URL: code, https://github.com/dtrx-py/dtrx
```

### Comparing `dtrx-8.5.2/setup.cfg` & `dtrx-8.5.3/setup.cfg`

 * *Files identical despite different names*

