# Comparing `tmp/botcity-ms365-credentials-plugin-0.1.0.tar.gz` & `tmp/botcity-ms365-credentials-plugin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/bot-ms365-credentials-plugin-python/bot-ms365-credentials-plugin-python/dist/.tmp-ccewnd4n/botcity-ms365-cred", last modified: Thu Mar  2 17:59:23 2023, max compression
+gzip compressed data, was "/home/runner/work/bot-ms365-credentials-plugin-python/bot-ms365-credentials-plugin-python/dist/.tmp-_v7v3m9y/botcity-ms365-cred", last modified: Thu May 11 12:18:22 2023, max compression
```

## Comparing `botcity-ms365-credentials-plugin-0.1.0.tar` & `botcity-ms365-credentials-plugin-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:59:23.000000 botcity-ms365-credentials-plugin-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-02 17:59:14.000000 botcity-ms365-credentials-plugin-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-03-02 17:59:23.000000 botcity-ms365-credentials-plugin-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-03-02 17:59:14.000000 botcity-ms365-credentials-plugin-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:59:23.000000 botcity-ms365-credentials-plugin-0.1.0/botcity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:59:23.000000 botcity-ms365-credentials-plugin-0.1.0/botcity/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:59:23.000000 botcity-ms365-credentials-plugin-0.1.0/botcity/plugins/ms365/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:59:23.000000 botcity-ms365-credentials-plugin-0.1.0/botcity/plugins/ms365/credentials/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-02 17:59:14.000000 botcity-ms365-credentials-plugin-0.1.0/botcity/plugins/ms365/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-02 17:59:23.000000 botcity-ms365-credentials-plugin-0.1.0/botcity/plugins/ms365/credentials/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-03-02 17:59:14.000000 botcity-ms365-credentials-plugin-0.1.0/botcity/plugins/ms365/credentials/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:59:23.000000 botcity-ms365-credentials-plugin-0.1.0/botcity_ms365_credentials_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-03-02 17:59:23.000000 botcity-ms365-credentials-plugin-0.1.0/botcity_ms365_credentials_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-02 17:59:23.000000 botcity-ms365-credentials-plugin-0.1.0/botcity_ms365_credentials_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 17:59:23.000000 botcity-ms365-credentials-plugin-0.1.0/botcity_ms365_credentials_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-02 17:59:23.000000 botcity-ms365-credentials-plugin-0.1.0/botcity_ms365_credentials_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-02 17:59:23.000000 botcity-ms365-credentials-plugin-0.1.0/botcity_ms365_credentials_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-02 17:59:14.000000 botcity-ms365-credentials-plugin-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-02 17:59:23.000000 botcity-ms365-credentials-plugin-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-02 17:59:14.000000 botcity-ms365-credentials-plugin-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:59:23.000000 botcity-ms365-credentials-plugin-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-02 17:59:14.000000 botcity-ms365-credentials-plugin-0.1.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-02 17:59:14.000000 botcity-ms365-credentials-plugin-0.1.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-03-02 17:59:14.000000 botcity-ms365-credentials-plugin-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:18:22.000000 botcity-ms365-credentials-plugin-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-11 12:18:11.000000 botcity-ms365-credentials-plugin-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-11 12:18:22.000000 botcity-ms365-credentials-plugin-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-05-11 12:18:11.000000 botcity-ms365-credentials-plugin-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:18:22.000000 botcity-ms365-credentials-plugin-0.2.0/botcity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:18:22.000000 botcity-ms365-credentials-plugin-0.2.0/botcity/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:18:22.000000 botcity-ms365-credentials-plugin-0.2.0/botcity/plugins/ms365/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:18:22.000000 botcity-ms365-credentials-plugin-0.2.0/botcity/plugins/ms365/credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-11 12:18:11.000000 botcity-ms365-credentials-plugin-0.2.0/botcity/plugins/ms365/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-11 12:18:22.000000 botcity-ms365-credentials-plugin-0.2.0/botcity/plugins/ms365/credentials/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-11 12:18:11.000000 botcity-ms365-credentials-plugin-0.2.0/botcity/plugins/ms365/credentials/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:18:22.000000 botcity-ms365-credentials-plugin-0.2.0/botcity_ms365_credentials_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-11 12:18:22.000000 botcity-ms365-credentials-plugin-0.2.0/botcity_ms365_credentials_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-11 12:18:22.000000 botcity-ms365-credentials-plugin-0.2.0/botcity_ms365_credentials_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:18:22.000000 botcity-ms365-credentials-plugin-0.2.0/botcity_ms365_credentials_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 12:18:22.000000 botcity-ms365-credentials-plugin-0.2.0/botcity_ms365_credentials_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 12:18:22.000000 botcity-ms365-credentials-plugin-0.2.0/botcity_ms365_credentials_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-11 12:18:11.000000 botcity-ms365-credentials-plugin-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-11 12:18:22.000000 botcity-ms365-credentials-plugin-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-11 12:18:11.000000 botcity-ms365-credentials-plugin-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:18:22.000000 botcity-ms365-credentials-plugin-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-11 12:18:11.000000 botcity-ms365-credentials-plugin-0.2.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-11 12:18:11.000000 botcity-ms365-credentials-plugin-0.2.0/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-11 12:18:11.000000 botcity-ms365-credentials-plugin-0.2.0/versioneer.py
```

### Comparing `botcity-ms365-credentials-plugin-0.1.0/PKG-INFO` & `botcity-ms365-credentials-plugin-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botcity-ms365-credentials-plugin
-Version: 0.1.0
+Version: 0.2.0
 Home-page: https://github.com/botcity-dev/bot-ms365-credentials-plugin-python.git
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # BotCity Microsoft 365 Credentials Plugin - Python
 
 ## 🤖 Computer-vision based UI Automation
```

### Comparing `botcity-ms365-credentials-plugin-0.1.0/README.md` & `botcity-ms365-credentials-plugin-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `botcity-ms365-credentials-plugin-0.1.0/botcity/plugins/ms365/credentials/plugin.py` & `botcity-ms365-credentials-plugin-0.2.0/botcity/plugins/ms365/credentials/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,19 +8,21 @@
     """
     The class with the enumerated scopes that can be used in the authentication.
 
     Usage: Scopes.<SCOPE_NAME>
     """
 
     BASIC = "basic"
-    MS365_FILES_READ = "onedrive"
-    MS365_FILES_ALL = "onedrive_all"
-    MS365_OUTLOOK_READ = "mailbox"
-    MS365_OUTLOOK_SEND = "message_send"
-    MS365_OUTLOOK_ALL = "message_all"
+    FILES_READ = "onedrive"
+    FILES_READ_WRITE_ALL = "onedrive_all"
+    SITES_READ_ALL = "sharepoint"
+    SITES_READ_WRITE_ALL = "sharepoint_dl"
+    MAIL_READ = "mailbox"
+    MAIL_SEND = "message_send"
+    MAIL_READ_WRITE = "message_all"
 
 
 class MS365CredentialsPlugin:
     def __init__(self, client_id: str, client_secret: str, token_path: str = '') -> None:
         """
         MS365CredentialsPlugin.
 
@@ -48,19 +50,17 @@
         """
         return self._account
 
     def authenticate(self, scopes: List[Scopes] = []) -> None:
         """
         Authenticate the Microsoft365 account with the credentials of the created application.
 
+        Scopes must match permissions added to the project in the Azure portal.
+
         Args:
             scopes (List[Scopes]): The permission scopes defined in the Scopes class that will
-                be used for authentication. Defaults to:
-
-                - BASIC: basic configuration.
-                - MS365_FILES_ALL: scope to use OneDrive, Excel.
-                - MS365_OUTLOOK_ALL: scope to use Outlook mail.
+                be used for authentication.
         """
         if not self.ms365_account.is_authenticated:
-            if not scopes:
-                scopes = [Scopes.BASIC, Scopes.MS365_FILES_ALL, Scopes.MS365_OUTLOOK_ALL]
+            if Scopes.BASIC not in scopes:
+                scopes.append(Scopes.BASIC)
             self.ms365_account.authenticate(scopes=scopes)
```

### Comparing `botcity-ms365-credentials-plugin-0.1.0/botcity_ms365_credentials_plugin.egg-info/PKG-INFO` & `botcity-ms365-credentials-plugin-0.2.0/botcity_ms365_credentials_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botcity-ms365-credentials-plugin
-Version: 0.1.0
+Version: 0.2.0
 Home-page: https://github.com/botcity-dev/bot-ms365-credentials-plugin-python.git
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # BotCity Microsoft 365 Credentials Plugin - Python
 
 ## 🤖 Computer-vision based UI Automation
```

### Comparing `botcity-ms365-credentials-plugin-0.1.0/botcity_ms365_credentials_plugin.egg-info/SOURCES.txt` & `botcity-ms365-credentials-plugin-0.2.0/botcity_ms365_credentials_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botcity-ms365-credentials-plugin-0.1.0/setup.py` & `botcity-ms365-credentials-plugin-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `botcity-ms365-credentials-plugin-0.1.0/versioneer.py` & `botcity-ms365-credentials-plugin-0.2.0/versioneer.py`

 * *Files identical despite different names*

