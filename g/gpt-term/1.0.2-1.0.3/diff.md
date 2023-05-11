# Comparing `tmp/gpt-term-1.0.2.tar.gz` & `tmp/gpt-term-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-term-1.0.2.tar", last modified: Thu May 11 09:05:29 2023, max compression
+gzip compressed data, was "gpt-term-1.0.3.tar", last modified: Thu May 11 11:02:21 2023, max compression
```

## Comparing `gpt-term-1.0.2.tar` & `gpt-term-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:05:29.847288 gpt-term-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-11 09:05:16.000000 gpt-term-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 09:05:16.000000 gpt-term-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-05-11 09:05:29.847288 gpt-term-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13525 2023-05-11 09:05:16.000000 gpt-term-1.0.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-05-11 09:05:16.000000 gpt-term-1.0.2/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:05:29.847288 gpt-term-1.0.2/gpt_term/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 09:05:16.000000 gpt-term-1.0.2/gpt_term/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-11 09:05:16.000000 gpt-term-1.0.2/gpt_term/config.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)    48427 2023-05-11 09:05:16.000000 gpt-term-1.0.2/gpt_term/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:05:29.847288 gpt-term-1.0.2/gpt_term.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-05-11 09:05:29.000000 gpt-term-1.0.2/gpt_term.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-11 09:05:29.000000 gpt-term-1.0.2/gpt_term.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:05:29.000000 gpt-term-1.0.2/gpt_term.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 09:05:29.000000 gpt-term-1.0.2/gpt_term.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 09:05:29.000000 gpt-term-1.0.2/gpt_term.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 09:05:29.000000 gpt-term-1.0.2/gpt_term.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 09:05:29.847288 gpt-term-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-11 09:05:16.000000 gpt-term-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:02:21.032970 gpt-term-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-11 11:02:09.000000 gpt-term-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 11:02:09.000000 gpt-term-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-05-11 11:02:21.032970 gpt-term-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13525 2023-05-11 11:02:09.000000 gpt-term-1.0.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-05-11 11:02:09.000000 gpt-term-1.0.3/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:02:21.032970 gpt-term-1.0.3/gpt_term/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 11:02:09.000000 gpt-term-1.0.3/gpt_term/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-11 11:02:09.000000 gpt-term-1.0.3/gpt_term/config.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48428 2023-05-11 11:02:09.000000 gpt-term-1.0.3/gpt_term/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:02:21.032970 gpt-term-1.0.3/gpt_term.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-05-11 11:02:21.000000 gpt-term-1.0.3/gpt_term.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-11 11:02:21.000000 gpt-term-1.0.3/gpt_term.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:02:21.000000 gpt-term-1.0.3/gpt_term.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 11:02:21.000000 gpt-term-1.0.3/gpt_term.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 11:02:21.000000 gpt-term-1.0.3/gpt_term.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 11:02:21.000000 gpt-term-1.0.3/gpt_term.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 11:02:21.032970 gpt-term-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-11 11:02:09.000000 gpt-term-1.0.3/setup.py
```

### Comparing `gpt-term-1.0.2/LICENSE` & `gpt-term-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-term-1.0.2/PKG-INFO` & `gpt-term-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-term
-Version: 1.0.2
+Version: 1.0.3
 Summary: Use ChatGPT in terminal
 Home-page: https://github.com/xiaoxx970/chatgpt-in-terminal
 Author: xiaoxx970
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gpt-term-1.0.2/README.md` & `gpt-term-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gpt-term-1.0.2/gpt_term/config.ini` & `gpt-term-1.0.3/gpt_term/config.ini`

 * *Files identical despite different names*

### Comparing `gpt-term-1.0.2/gpt_term/main.py` & `gpt-term-1.0.3/gpt_term/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -911,15 +911,15 @@
     /help                    - Show this help message
     /exit                    - Exit the application''')
         
     else:
         set_command = set(command)
         min_levenshtein_distance = len(command)
         most_similar_command = ""
-        for slash_command in CustomCompleter.commands:
+        for slash_command in CommandCompleter.commands:
             this_levenshtein_distance = get_levenshtein_distance(command, slash_command)
             if this_levenshtein_distance < min_levenshtein_distance:
                 set_slash_command = set(slash_command)
                 if len(set_command & set_slash_command) / len(set_command | set_slash_command) >= 0.75:
                     most_similar_command = slash_command
                     min_levenshtein_distance = this_levenshtein_distance
```

### Comparing `gpt-term-1.0.2/gpt_term.egg-info/PKG-INFO` & `gpt-term-1.0.3/gpt_term.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-term
-Version: 1.0.2
+Version: 1.0.3
 Summary: Use ChatGPT in terminal
 Home-page: https://github.com/xiaoxx970/chatgpt-in-terminal
 Author: xiaoxx970
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gpt-term-1.0.2/setup.py` & `gpt-term-1.0.3/setup.py`

 * *Files identical despite different names*

