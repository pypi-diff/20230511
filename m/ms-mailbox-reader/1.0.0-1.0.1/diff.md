# Comparing `tmp/ms_mailbox_reader-1.0.0.tar.gz` & `tmp/ms_mailbox_reader-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_mailbox_reader-1.0.0.tar", last modified: Fri May  5 21:41:25 2023, max compression
+gzip compressed data, was "ms_mailbox_reader-1.0.1.tar", last modified: Thu May 11 15:09:07 2023, max compression
```

## Comparing `ms_mailbox_reader-1.0.0.tar` & `ms_mailbox_reader-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:41:25.681637 ms_mailbox_reader-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-05 21:41:12.000000 ms_mailbox_reader-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-05 21:41:25.681637 ms_mailbox_reader-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-05 21:41:12.000000 ms_mailbox_reader-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:41:25.677637 ms_mailbox_reader-1.0.0/ms_mailbox_reader/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 21:41:12.000000 ms_mailbox_reader-1.0.0/ms_mailbox_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-05 21:41:12.000000 ms_mailbox_reader-1.0.0/ms_mailbox_reader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:41:25.681637 ms_mailbox_reader-1.0.0/ms_mailbox_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-05 21:41:25.000000 ms_mailbox_reader-1.0.0/ms_mailbox_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-05 21:41:25.000000 ms_mailbox_reader-1.0.0/ms_mailbox_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:41:25.000000 ms_mailbox_reader-1.0.0/ms_mailbox_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 21:41:25.000000 ms_mailbox_reader-1.0.0/ms_mailbox_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 21:41:25.000000 ms_mailbox_reader-1.0.0/ms_mailbox_reader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:41:25.681637 ms_mailbox_reader-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-05 21:41:12.000000 ms_mailbox_reader-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:09:07.589939 ms_mailbox_reader-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-11 15:08:53.000000 ms_mailbox_reader-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-11 15:09:07.589939 ms_mailbox_reader-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-11 15:08:53.000000 ms_mailbox_reader-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:09:07.585939 ms_mailbox_reader-1.0.1/ms_mailbox_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-11 15:08:53.000000 ms_mailbox_reader-1.0.1/ms_mailbox_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-11 15:08:53.000000 ms_mailbox_reader-1.0.1/ms_mailbox_reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:09:07.589939 ms_mailbox_reader-1.0.1/ms_mailbox_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-11 15:09:07.000000 ms_mailbox_reader-1.0.1/ms_mailbox_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-11 15:09:07.000000 ms_mailbox_reader-1.0.1/ms_mailbox_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:09:07.000000 ms_mailbox_reader-1.0.1/ms_mailbox_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 15:09:07.000000 ms_mailbox_reader-1.0.1/ms_mailbox_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 15:09:07.000000 ms_mailbox_reader-1.0.1/ms_mailbox_reader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:09:07.589939 ms_mailbox_reader-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-11 15:08:53.000000 ms_mailbox_reader-1.0.1/setup.py
```

### Comparing `ms_mailbox_reader-1.0.0/LICENSE` & `ms_mailbox_reader-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_mailbox_reader-1.0.0/README.md` & `ms_mailbox_reader-1.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # ms-mailbox-reader
 A python package for windows which allows easy reading of email 
 messages from a local mailbox. Tested with Outlook + Microsoft Exchange on a Windows 11 PC. 
 
 
 ### Basic Usage
 ```python
-from ms_mailbox_reader.client import MsExchangeClient, MessageFilter
+from datetime import datetime, timedelta
+from ms_mailbox_reader.reader import MsOutlookMessageReader, MessageFilter
 
 # Create the message reader
 message_reader = MsOutlookMessageReader()
 
-# Timedelta representing the last two hours
-last_n_hours = datetime.now() - timedelta(hours=2)
-
 # Create a filter to limit returned messages to a max of 25, 
 # those which were sent from @mydomain.com and 
 # received in the last two hours
-filter_params = MessageFilter(sender_email="@mydomain.com",
-                              received_since = last_n_hours,
+# ---
+# The sender email param may not be what you expect. Sometimes it'll be a
+# long OU type string. 
+filter_params = MessageFilter(sender_email="@mydomain.com", 
+                              received_since = (datetime.now() - timedelta(hours=2)),
                               limit=25)
 
 # Get the message list
 messages = message_reader.get_outlook_messages(filter_params)
 
 # Do stuff with the messages
 for message in messages:
```

### Comparing `ms_mailbox_reader-1.0.0/ms_mailbox_reader/reader.py` & `ms_mailbox_reader-1.0.1/ms_mailbox_reader/reader.py`

 * *Files identical despite different names*

