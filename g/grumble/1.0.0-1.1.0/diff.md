# Comparing `tmp/grumble-1.0.0.tar.gz` & `tmp/grumble-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grumble-1.0.0.tar", last modified: Sun Oct 16 22:10:14 2022, max compression
+gzip compressed data, was "grumble-1.1.0.tar", last modified: Thu May 11 01:43:16 2023, max compression
```

## Comparing `grumble-1.0.0.tar` & `grumble-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-16 22:10:14.120104 grumble-1.0.0/
--rw-r--r--   0 chipx86    (501) staff       (20)       40 2022-10-16 22:09:07.000000 grumble-1.0.0/AUTHORS
--rw-r--r--   0 chipx86    (501) staff       (20)     1061 2022-10-16 22:08:31.000000 grumble-1.0.0/LICENSE
--rw-r--r--   0 chipx86    (501) staff       (20)     9601 2022-10-16 22:10:14.119875 grumble-1.0.0/PKG-INFO
--rw-r--r--   0 chipx86    (501) staff       (20)     7177 2022-10-16 21:36:54.000000 grumble-1.0.0/README.md
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-16 22:10:14.119030 grumble-1.0.0/grumble/
--rw-r--r--   0 chipx86    (501) staff       (20)    11407 2022-10-16 22:06:06.000000 grumble-1.0.0/grumble/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-16 22:10:14.119652 grumble-1.0.0/grumble.egg-info/
--rw-r--r--   0 chipx86    (501) staff       (20)     9601 2022-10-16 22:10:14.000000 grumble-1.0.0/grumble.egg-info/PKG-INFO
--rw-r--r--   0 chipx86    (501) staff       (20)      184 2022-10-16 22:10:14.000000 grumble-1.0.0/grumble.egg-info/SOURCES.txt
--rw-r--r--   0 chipx86    (501) staff       (20)        1 2022-10-16 22:10:14.000000 grumble-1.0.0/grumble.egg-info/dependency_links.txt
--rw-r--r--   0 chipx86    (501) staff       (20)        8 2022-10-16 22:10:14.000000 grumble-1.0.0/grumble.egg-info/top_level.txt
--rw-r--r--   0 chipx86    (501) staff       (20)     1151 2022-10-16 20:59:27.000000 grumble-1.0.0/pyproject.toml
--rw-r--r--   0 chipx86    (501) staff       (20)       38 2022-10-16 22:10:14.120151 grumble-1.0.0/setup.cfg
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-11 01:43:16.110323 grumble-1.1.0/
+-rw-r--r--   0 chipx86    (501) staff       (20)       40 2022-10-16 22:09:07.000000 grumble-1.1.0/AUTHORS
+-rw-r--r--   0 chipx86    (501) staff       (20)     1061 2022-10-16 22:08:31.000000 grumble-1.1.0/LICENSE
+-rw-r--r--   0 chipx86    (501) staff       (20)     8494 2023-05-11 01:43:16.110161 grumble-1.1.0/PKG-INFO
+-rw-r--r--   0 chipx86    (501) staff       (20)     7271 2023-05-11 01:37:01.000000 grumble-1.1.0/README.md
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-11 01:43:16.109520 grumble-1.1.0/grumble/
+-rw-r--r--   0 chipx86    (501) staff       (20)    11858 2023-05-11 01:37:01.000000 grumble-1.1.0/grumble/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-11 01:43:16.109987 grumble-1.1.0/grumble.egg-info/
+-rw-r--r--   0 chipx86    (501) staff       (20)     8494 2023-05-11 01:43:16.000000 grumble-1.1.0/grumble.egg-info/PKG-INFO
+-rw-r--r--   0 chipx86    (501) staff       (20)      184 2023-05-11 01:43:16.000000 grumble-1.1.0/grumble.egg-info/SOURCES.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)        1 2023-05-11 01:43:16.000000 grumble-1.1.0/grumble.egg-info/dependency_links.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)        8 2023-05-11 01:43:16.000000 grumble-1.1.0/grumble.egg-info/top_level.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)     1158 2023-05-11 01:41:06.000000 grumble-1.1.0/pyproject.toml
+-rw-r--r--   0 chipx86    (501) staff       (20)       38 2023-05-11 01:43:16.110363 grumble-1.1.0/setup.cfg
```

### Comparing `grumble-1.0.0/LICENSE` & `grumble-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grumble-1.0.0/PKG-INFO` & `grumble-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,16 @@
 Metadata-Version: 2.1
 Name: grumble
-Version: 1.0.0
+Version: 1.1.0
 Summary: For print debuggers drowning in print statements.
 Author-email: Christian Hammond <christian@beanbaginc.com>
-License: Copyright (c) 2022 Christian Hammond
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of
-        this software and associated documentation files (the "Software"), to deal in
-        the Software without restriction, including without limitation the rights to
-        use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-        of the Software, and to permit persons to whom the Software is furnished to do
-        so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: homepage, https://github.com/chipx86/grumble
-Project-URL: documentation, https://github.com/chipx86/grumble
-Project-URL: repository, https://github.com/chipx86/grumble
+License: MIT
+Project-URL: homepage, https://github.com/beanbaginc/grumble
+Project-URL: documentation, https://github.com/beanbaginc/grumble
+Project-URL: repository, https://github.com/beanbaginc/grumble
 Keywords: debugging,console,logs
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -43,15 +24,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-Grumble...
+Grumble 🤨
 ==========
 
 Grumble is a Python library for print debuggers who are drowning in `print()`
 statements..
 
 It's for developers who need to capture lots of data between runs.
 
@@ -70,15 +51,15 @@
 
 
 It's a Friday evening, and everything you wrote is busted
 ---------------------------------------------------------
 
 You spent all week trying to get your code work. And it should work, but it's
 not. You're furiously trying to debug it as you get increasingly exhausted,
-your brain begining to melt into a pile of goo.
+your brain beginning to melt into a pile of goo.
 
 The hours are ticking away with nothing to show for it. Your console is full
 of print output, and it's beginning to blur together into some kind of blended
 soup of green Matrix code nonsense.
 
 Log messages mixed with tracebacks, mixed with variable dumps, all coming from
 different classes, threads, processes. Screens full of it.
@@ -275,14 +256,17 @@
 
 Works with threads and multiple processes!
 ------------------------------------------
 
 Logs are differentiated by thread and process IDs. Lock files ensure that
 logs don't get jumbled together. Because that would be annoying to deal with.
 
+If you want to collapse everything into a single log file, set
+`GRUMBLE_MERGE_THREADS=1`.
+
 
 Emojis and hashes are deterministic
 -----------------------------------
 
 Grumble will cycle through emojis in the following order, every time:
 
 😶 🧐 🤨 😬 🙄 😑 😕 ☹️ 😯 😧 😵 😠 😣 😖 😫 😤 😡 🤬 😒 😪
```

### Comparing `grumble-1.0.0/README.md` & `grumble-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Grumble...
+Grumble 🤨
 ==========
 
 Grumble is a Python library for print debuggers who are drowning in `print()`
 statements..
 
 It's for developers who need to capture lots of data between runs.
 
@@ -21,15 +21,15 @@
 
 
 It's a Friday evening, and everything you wrote is busted
 ---------------------------------------------------------
 
 You spent all week trying to get your code work. And it should work, but it's
 not. You're furiously trying to debug it as you get increasingly exhausted,
-your brain begining to melt into a pile of goo.
+your brain beginning to melt into a pile of goo.
 
 The hours are ticking away with nothing to show for it. Your console is full
 of print output, and it's beginning to blur together into some kind of blended
 soup of green Matrix code nonsense.
 
 Log messages mixed with tracebacks, mixed with variable dumps, all coming from
 different classes, threads, processes. Screens full of it.
@@ -226,14 +226,17 @@
 
 Works with threads and multiple processes!
 ------------------------------------------
 
 Logs are differentiated by thread and process IDs. Lock files ensure that
 logs don't get jumbled together. Because that would be annoying to deal with.
 
+If you want to collapse everything into a single log file, set
+`GRUMBLE_MERGE_THREADS=1`.
+
 
 Emojis and hashes are deterministic
 -----------------------------------
 
 Grumble will cycle through emojis in the following order, every time:
 
 😶 🧐 🤨 😬 🙄 😑 😕 ☹️ 😯 😧 😵 😠 😣 😖 😫 😤 😡 🤬 😒 😪
```

### Comparing `grumble-1.0.0/grumble/__init__.py` & `grumble-1.1.0/grumble/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,17 +61,14 @@
     '🕙',  # 10:00 / 22:00
     '🕥',  # 10:30 / 22:30
     '🕚',  # 11:00 / 23:00
     '🕦',  # 11:30 / 23:30
 ]
 
 _thread_state = threading.local()
-_thread_state.grumble_emoji_i = 0
-_thread_state.log_i = 0
-
 _cur_dir = os.getcwd()
 
 
 def _get_log_dir() -> str:
     """Return the directory where logs will be stored.
 
     By default, this will be the current directory stored when the module
@@ -105,19 +102,20 @@
     proc_name = sys.argv[0]
     pid = os.getpid()
     thread = threading.current_thread()
     thread_name = thread.name
 
     filename_parts = [
         'grumble',
-        proc_name or os.path.basename(sys.executable),
+        os.path.basename(proc_name or sys.executable),
         str(pid),
     ]
 
-    if thread_name != 'MainThread':
+    if (thread_name != 'MainThread' and
+        os.environ.get('GRUMBLE_MERGE_THREADS') != '1'):
         filename_parts += [thread_name, str(thread.ident)]
 
     if log_tag:
         filename_parts.append(log_tag)
 
     filename = '%s.log' % '-'.join(filename_parts)
 
@@ -312,27 +310,38 @@
         category (str, optional):
             A category for the log output, to help identify what the output
             pertains to.
 
         log_tag (str, optional):
             A custom tag to include in the generated log filename.
     """
+    try:
+        log_i = _thread_state.log_i
+    except AttributeError:
+        _thread_state.log_i = 0
+        log_i = 0
+
+    try:
+        emoji_i = _thread_state.grumble_emoji_i
+    except AttributeError:
+        _thread_state.grumble_emoji_i = 0
+        emoji_i = 0
+
     # Set up some identifying information.
     log_path = _get_log_file_path(log_tag=log_tag)
-    sha = hashlib.sha1(b'%d' % _thread_state.log_i).hexdigest()
+    sha = hashlib.sha1(b'%d' % log_i).hexdigest()
     now = datetime.now()
     now_str = now.strftime('%Y-%m-%d %H:%M:%S')
 
     _thread_state.log_i += 1
 
     # Select an emoji.
     #
     # We'll cycle through the list, wrapping around when we hit the last
     # one.
-    emoji_i = _thread_state.grumble_emoji_i
     emoji = _GRUMBLE_EMOJIS[emoji_i]
 
     if emoji_i < _NUM_GRUMBLE_EMOJIS:
         emoji_i += 1
     else:
         emoji_i = 0
 
@@ -357,14 +366,21 @@
     # Build the message for the log.
     log_header_lines = [
         emoji,
         '%s  Grumble ID:  %s' % (emoji, sha),
         '%s   Timestamp:  %s %s' % (emoji, clock_emoji, now_str),
     ]
 
+    thread = threading.current_thread()
+    thread_name = thread.name
+
+    if thread_name != 'MainThread':
+        log_header_lines.append('%s      Thread:  %s (%s)'
+                                % (emoji, thread_name, thread.ident))
+
     if category:
         log_header_lines.append('%s    Category:  %s' % (emoji, category))
 
     if msg:
         log_header_lines.append('%s     Message:  %s' % (emoji, msg))
 
     log_header_lines += [
```

### Comparing `grumble-1.0.0/grumble.egg-info/PKG-INFO` & `grumble-1.1.0/grumble.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,16 @@
 Metadata-Version: 2.1
 Name: grumble
-Version: 1.0.0
+Version: 1.1.0
 Summary: For print debuggers drowning in print statements.
 Author-email: Christian Hammond <christian@beanbaginc.com>
-License: Copyright (c) 2022 Christian Hammond
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of
-        this software and associated documentation files (the "Software"), to deal in
-        the Software without restriction, including without limitation the rights to
-        use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-        of the Software, and to permit persons to whom the Software is furnished to do
-        so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: homepage, https://github.com/chipx86/grumble
-Project-URL: documentation, https://github.com/chipx86/grumble
-Project-URL: repository, https://github.com/chipx86/grumble
+License: MIT
+Project-URL: homepage, https://github.com/beanbaginc/grumble
+Project-URL: documentation, https://github.com/beanbaginc/grumble
+Project-URL: repository, https://github.com/beanbaginc/grumble
 Keywords: debugging,console,logs
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -43,15 +24,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-Grumble...
+Grumble 🤨
 ==========
 
 Grumble is a Python library for print debuggers who are drowning in `print()`
 statements..
 
 It's for developers who need to capture lots of data between runs.
 
@@ -70,15 +51,15 @@
 
 
 It's a Friday evening, and everything you wrote is busted
 ---------------------------------------------------------
 
 You spent all week trying to get your code work. And it should work, but it's
 not. You're furiously trying to debug it as you get increasingly exhausted,
-your brain begining to melt into a pile of goo.
+your brain beginning to melt into a pile of goo.
 
 The hours are ticking away with nothing to show for it. Your console is full
 of print output, and it's beginning to blur together into some kind of blended
 soup of green Matrix code nonsense.
 
 Log messages mixed with tracebacks, mixed with variable dumps, all coming from
 different classes, threads, processes. Screens full of it.
@@ -275,14 +256,17 @@
 
 Works with threads and multiple processes!
 ------------------------------------------
 
 Logs are differentiated by thread and process IDs. Lock files ensure that
 logs don't get jumbled together. Because that would be annoying to deal with.
 
+If you want to collapse everything into a single log file, set
+`GRUMBLE_MERGE_THREADS=1`.
+
 
 Emojis and hashes are deterministic
 -----------------------------------
 
 Grumble will cycle through emojis in the following order, every time:
 
 😶 🧐 🤨 😬 🙄 😑 😕 ☹️ 😯 😧 😵 😠 😣 😖 😫 😤 😡 🤬 😒 😪
```

### Comparing `grumble-1.0.0/pyproject.toml` & `grumble-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "grumble"
-version = "1.0.0"
+version = "1.1.0"
 description = "For print debuggers drowning in print statements."
 authors = [
     {name = "Christian Hammond", email="christian@beanbaginc.com"},
 ]
-license = {file = "LICENSE"}
+license = { text = "MIT" }
 readme = "README.md"
 requires-python = ">=3.6"
 
 keywords = [
     "debugging",
     "console",
     "logs",
@@ -31,10 +31,10 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
 ]
 
 
 [project.urls]
-homepage = "https://github.com/chipx86/grumble"
-documentation = "https://github.com/chipx86/grumble"
-repository = "https://github.com/chipx86/grumble"
+homepage = "https://github.com/beanbaginc/grumble"
+documentation = "https://github.com/beanbaginc/grumble"
+repository = "https://github.com/beanbaginc/grumble"
```

