# Comparing `tmp/pyrc-python-utils-1.0.8.tar.gz` & `tmp/pyrc-python-utils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrc-python-utils-1.0.8.tar", last modified: Wed May 10 00:22:53 2023, max compression
+gzip compressed data, was "pyrc-python-utils-1.0.9.tar", last modified: Wed May 10 18:35:58 2023, max compression
```

## Comparing `pyrc-python-utils-1.0.8.tar` & `pyrc-python-utils-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 00:22:53.318598 pyrc-python-utils-1.0.8/
--rw-rw-rw-   0        0        0     1085 2023-05-08 22:51:52.000000 pyrc-python-utils-1.0.8/LICENSE
--rw-rw-rw-   0        0        0       57 2023-05-08 23:01:23.000000 pyrc-python-utils-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      456 2023-05-10 00:22:53.318598 pyrc-python-utils-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.8/README.md
--rw-rw-rw-   0        0        0      519 2023-05-10 00:22:33.000000 pyrc-python-utils-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 00:22:53.318598 pyrc-python-utils-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 00:22:53.311598 pyrc-python-utils-1.0.8/src/
--rw-rw-rw-   0        0        0      171 2023-05-10 00:20:57.000000 pyrc-python-utils-1.0.8/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 00:22:53.317597 pyrc-python-utils-1.0.8/src/pyrc_python_utils.egg-info/
--rw-rw-rw-   0        0        0      456 2023-05-10 00:22:53.000000 pyrc-python-utils-1.0.8/src/pyrc_python_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2023-05-10 00:22:53.000000 pyrc-python-utils-1.0.8/src/pyrc_python_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 00:22:53.000000 pyrc-python-utils-1.0.8/src/pyrc_python_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-10 00:22:53.000000 pyrc-python-utils-1.0.8/src/pyrc_python_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       98 2023-05-10 00:22:53.000000 pyrc-python-utils-1.0.8/src/pyrc_python_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      503 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.8/src/pyrc_util_datetime.py
--rw-rw-rw-   0        0        0     3409 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.8/src/pyrc_util_exchange.py
--rw-rw-rw-   0        0        0      229 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.8/src/pyrc_util_file.py
--rw-rw-rw-   0        0        0     9937 2023-05-10 00:22:16.000000 pyrc-python-utils-1.0.8/src/pyrc_util_sftp.py
--rw-rw-rw-   0        0        0     4408 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.8/src/pyrc_util_sharepoint.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:35:58.494730 pyrc-python-utils-1.0.9/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 22:51:52.000000 pyrc-python-utils-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-05-08 23:01:23.000000 pyrc-python-utils-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      456 2023-05-10 18:35:58.494730 pyrc-python-utils-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.9/README.md
+-rw-rw-rw-   0        0        0      540 2023-05-10 18:35:40.000000 pyrc-python-utils-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 18:35:58.495731 pyrc-python-utils-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 18:35:58.487213 pyrc-python-utils-1.0.9/src/
+-rw-rw-rw-   0        0        0      171 2023-05-10 00:20:57.000000 pyrc-python-utils-1.0.9/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:35:58.493732 pyrc-python-utils-1.0.9/src/pyrc_python_utils.egg-info/
+-rw-rw-rw-   0        0        0      456 2023-05-10 18:35:58.000000 pyrc-python-utils-1.0.9/src/pyrc_python_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2023-05-10 18:35:58.000000 pyrc-python-utils-1.0.9/src/pyrc_python_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 18:35:58.000000 pyrc-python-utils-1.0.9/src/pyrc_python_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-10 18:35:58.000000 pyrc-python-utils-1.0.9/src/pyrc_python_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       98 2023-05-10 18:35:58.000000 pyrc-python-utils-1.0.9/src/pyrc_python_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      503 2023-05-10 13:29:21.000000 pyrc-python-utils-1.0.9/src/pyrc_util_datetime.py
+-rw-rw-rw-   0        0        0     3409 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.9/src/pyrc_util_exchange.py
+-rw-rw-rw-   0        0        0      229 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.9/src/pyrc_util_file.py
+-rw-rw-rw-   0        0        0     9941 2023-05-10 18:32:42.000000 pyrc-python-utils-1.0.9/src/pyrc_util_sftp.py
+-rw-rw-rw-   0        0        0     4408 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.9/src/pyrc_util_sharepoint.py
```

### Comparing `pyrc-python-utils-1.0.8/LICENSE` & `pyrc-python-utils-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrc-python-utils-1.0.8/src/pyrc_util_exchange.py` & `pyrc-python-utils-1.0.9/src/pyrc_util_exchange.py`

 * *Files identical despite different names*

### Comparing `pyrc-python-utils-1.0.8/src/pyrc_util_sftp.py` & `pyrc-python-utils-1.0.9/src/pyrc_util_sftp.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import re
 import stat
 from io import BytesIO
 
 import paramiko
 
-import pyrc_util_file as util_file
+import src.pyrc_util_file as util_file
 
 
 def create_client(host: str, username: str, password: str) -> paramiko.SFTPClient:
     transport = paramiko.Transport((host, 22))
     transport.connect(None, username, password)
 
     return paramiko.SFTPClient.from_transport(transport)
```

### Comparing `pyrc-python-utils-1.0.8/src/pyrc_util_sharepoint.py` & `pyrc-python-utils-1.0.9/src/pyrc_util_sharepoint.py`

 * *Files identical despite different names*

