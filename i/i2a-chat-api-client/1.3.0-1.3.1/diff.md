# Comparing `tmp/i2a_chat_api_client-1.3.0.tar.gz` & `tmp/i2a_chat_api_client-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i2a_chat_api_client-1.3.0.tar", last modified: Wed Apr 12 11:33:35 2023, max compression
+gzip compressed data, was "i2a_chat_api_client-1.3.1.tar", last modified: Thu May 11 09:03:22 2023, max compression
```

## Comparing `i2a_chat_api_client-1.3.0.tar` & `i2a_chat_api_client-1.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 adn       (1000) adn       (1000)        0 2023-04-12 11:33:35.268773 i2a_chat_api_client-1.3.0/
--rw-rw-r--   0 adn       (1000) adn       (1000)     1061 2023-04-12 09:16:02.000000 i2a_chat_api_client-1.3.0/LICENSE.txt
--rw-rw-r--   0 adn       (1000) adn       (1000)      579 2023-04-12 11:33:35.268773 i2a_chat_api_client-1.3.0/PKG-INFO
--rw-rw-r--   0 adn       (1000) adn       (1000)      203 2023-04-12 09:16:02.000000 i2a_chat_api_client-1.3.0/README.md
-drwxrwxr-x   0 adn       (1000) adn       (1000)        0 2023-04-12 11:33:35.268773 i2a_chat_api_client-1.3.0/i2a_chat_api_client/
--rw-rw-r--   0 adn       (1000) adn       (1000)       49 2023-04-12 09:16:02.000000 i2a_chat_api_client-1.3.0/i2a_chat_api_client/__init__.py
--rw-rw-r--   0 adn       (1000) adn       (1000)    13004 2023-04-12 11:33:20.000000 i2a_chat_api_client-1.3.0/i2a_chat_api_client/client.py
--rw-rw-r--   0 adn       (1000) adn       (1000)      480 2023-04-12 09:16:02.000000 i2a_chat_api_client-1.3.0/i2a_chat_api_client/exceptions.py
-drwxrwxr-x   0 adn       (1000) adn       (1000)        0 2023-04-12 11:33:35.268773 i2a_chat_api_client-1.3.0/i2a_chat_api_client.egg-info/
--rw-rw-r--   0 adn       (1000) adn       (1000)      579 2023-04-12 11:33:35.000000 i2a_chat_api_client-1.3.0/i2a_chat_api_client.egg-info/PKG-INFO
--rw-rw-r--   0 adn       (1000) adn       (1000)      340 2023-04-12 11:33:35.000000 i2a_chat_api_client-1.3.0/i2a_chat_api_client.egg-info/SOURCES.txt
--rw-rw-r--   0 adn       (1000) adn       (1000)        1 2023-04-12 11:33:35.000000 i2a_chat_api_client-1.3.0/i2a_chat_api_client.egg-info/dependency_links.txt
--rw-rw-r--   0 adn       (1000) adn       (1000)       17 2023-04-12 11:33:35.000000 i2a_chat_api_client-1.3.0/i2a_chat_api_client.egg-info/requires.txt
--rw-rw-r--   0 adn       (1000) adn       (1000)       20 2023-04-12 11:33:35.000000 i2a_chat_api_client-1.3.0/i2a_chat_api_client.egg-info/top_level.txt
--rw-rw-r--   0 adn       (1000) adn       (1000)       38 2023-04-12 11:33:35.268773 i2a_chat_api_client-1.3.0/setup.cfg
--rw-rw-r--   0 adn       (1000) adn       (1000)      786 2023-04-12 11:33:20.000000 i2a_chat_api_client-1.3.0/setup.py
+drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-05-11 09:03:22.589735 i2a_chat_api_client-1.3.1/
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1061 2023-05-11 08:43:46.000000 i2a_chat_api_client-1.3.1/LICENSE.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      579 2023-05-11 09:03:22.589735 i2a_chat_api_client-1.3.1/PKG-INFO
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      203 2023-05-11 08:43:46.000000 i2a_chat_api_client-1.3.1/README.md
+drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-05-11 09:03:22.589735 i2a_chat_api_client-1.3.1/i2a_chat_api_client/
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       49 2023-05-11 08:43:46.000000 i2a_chat_api_client-1.3.1/i2a_chat_api_client/__init__.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)    13003 2023-05-11 08:56:10.000000 i2a_chat_api_client-1.3.1/i2a_chat_api_client/client.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      480 2023-05-11 08:43:46.000000 i2a_chat_api_client-1.3.1/i2a_chat_api_client/exceptions.py
+drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-05-11 09:03:22.589735 i2a_chat_api_client-1.3.1/i2a_chat_api_client.egg-info/
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      579 2023-05-11 09:03:22.000000 i2a_chat_api_client-1.3.1/i2a_chat_api_client.egg-info/PKG-INFO
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      340 2023-05-11 09:03:22.000000 i2a_chat_api_client-1.3.1/i2a_chat_api_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        1 2023-05-11 09:03:22.000000 i2a_chat_api_client-1.3.1/i2a_chat_api_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       17 2023-05-11 09:03:22.000000 i2a_chat_api_client-1.3.1/i2a_chat_api_client.egg-info/requires.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       20 2023-05-11 09:03:22.000000 i2a_chat_api_client-1.3.1/i2a_chat_api_client.egg-info/top_level.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       38 2023-05-11 09:03:22.589735 i2a_chat_api_client-1.3.1/setup.cfg
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      786 2023-05-11 09:03:15.000000 i2a_chat_api_client-1.3.1/setup.py
```

### Comparing `i2a_chat_api_client-1.3.0/LICENSE.txt` & `i2a_chat_api_client-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i2a_chat_api_client-1.3.0/PKG-INFO` & `i2a_chat_api_client-1.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2a_chat_api_client
-Version: 1.3.0
+Version: 1.3.1
 Summary: Sdk for i2a chat api
 Download-URL: https://pypi.org/project/i2a_chat_api_client/
 Author: i2a Solutions Inc.
 Author-email: msyta@i2asolutions.com
 License: MIT
 Keywords: I2A Chat Api Client,I2A Chat Api,I2A Chat,Python 3,I2A Chat Api SDK
 Description-Content-Type: text/markdown
```

### Comparing `i2a_chat_api_client-1.3.0/i2a_chat_api_client/client.py` & `i2a_chat_api_client-1.3.1/i2a_chat_api_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,15 @@
         """
         Queuing system message to be saved and send on websocket in provided chat room
         :param chat_room_identifier: str, None
         :param message_timestamp_from: str, None
         :param limit: int
         :return: response - [messages]
        """
-        url = self._get_full_url(f'/chat-room/{chat_room_identifier}/messages/')
+        url = self._get_full_url(f'chat-room/{chat_room_identifier}/messages/')
         params = {}
         if message_timestamp_from:
             params['timestamp_from'] = message_timestamp_from
         if limit:
             params['limit'] = limit
         response = requests.get(url, headers=self._required_headers(), params=params)
         if response.status_code == 200:
```

### Comparing `i2a_chat_api_client-1.3.0/i2a_chat_api_client.egg-info/PKG-INFO` & `i2a_chat_api_client-1.3.1/i2a_chat_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2a-chat-api-client
-Version: 1.3.0
+Version: 1.3.1
 Summary: Sdk for i2a chat api
 Download-URL: https://pypi.org/project/i2a_chat_api_client/
 Author: i2a Solutions Inc.
 Author-email: msyta@i2asolutions.com
 License: MIT
 Keywords: I2A Chat Api Client,I2A Chat Api,I2A Chat,Python 3,I2A Chat Api SDK
 Description-Content-Type: text/markdown
```

### Comparing `i2a_chat_api_client-1.3.0/setup.py` & `i2a_chat_api_client-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='i2a_chat_api_client',
-    version='1.3.0',
+    version='1.3.1',
     description='Sdk for i2a chat api',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='i2a Solutions Inc.',
     author_email='msyta@i2asolutions.com',
```

