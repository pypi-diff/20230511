# Comparing `tmp/rum_with_telegram-0.9.4.tar.gz` & `tmp/rum_with_telegram-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-0.9.4.tar", last modified: Thu May  4 05:07:42 2023, max compression
+gzip compressed data, was "rum_with_telegram-0.9.5.tar", last modified: Thu May 11 03:44:29 2023, max compression
```

## Comparing `rum_with_telegram-0.9.4.tar` & `rum_with_telegram-0.9.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 05:07:42.920520 rum_with_telegram-0.9.4/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.4/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-05-04 05:07:42.919514 rum_with_telegram-0.9.4/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.4/README.md
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.9.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-04 05:07:42.904555 rum_with_telegram-0.9.4/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-05-04 05:01:32.000000 rum_with_telegram-0.9.4/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0     1955 2023-05-04 04:53:43.000000 rum_with_telegram-0.9.4/rum_with_telegram/config.py
--rw-rw-rw-   0        0        0    25343 2023-05-04 05:03:28.000000 rum_with_telegram-0.9.4/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     3345 2023-05-04 04:27:01.000000 rum_with_telegram-0.9.4/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1850 2023-05-04 04:25:42.000000 rum_with_telegram-0.9.4/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:07:42.917518 rum_with_telegram-0.9.4/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-05-04 05:07:42.000000 rum_with_telegram-0.9.4/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-04 05:07:42.000000 rum_with_telegram-0.9.4/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 05:07:42.000000 rum_with_telegram-0.9.4/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-04 05:07:42.000000 rum_with_telegram-0.9.4/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-04 05:07:42.000000 rum_with_telegram-0.9.4/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 05:07:42.921510 rum_with_telegram-0.9.4/setup.cfg
--rw-rw-rw-   0        0        0     1430 2023-05-04 05:01:32.000000 rum_with_telegram-0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 03:44:29.858099 rum_with_telegram-0.9.5/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.5/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-05-11 03:44:29.857102 rum_with_telegram-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.5/README.md
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.9.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-11 03:44:29.842141 rum_with_telegram-0.9.5/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-05-11 03:38:44.000000 rum_with_telegram-0.9.5/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0     1955 2023-05-04 04:53:43.000000 rum_with_telegram-0.9.5/rum_with_telegram/config.py
+-rw-rw-rw-   0        0        0    25467 2023-05-11 03:41:18.000000 rum_with_telegram-0.9.5/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     3345 2023-05-04 04:27:01.000000 rum_with_telegram-0.9.5/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1850 2023-05-04 04:25:42.000000 rum_with_telegram-0.9.5/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-05-11 03:44:29.855108 rum_with_telegram-0.9.5/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-05-11 03:44:29.000000 rum_with_telegram-0.9.5/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-11 03:44:29.000000 rum_with_telegram-0.9.5/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 03:44:29.000000 rum_with_telegram-0.9.5/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-11 03:44:29.000000 rum_with_telegram-0.9.5/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-11 03:44:29.000000 rum_with_telegram-0.9.5/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 03:44:29.859096 rum_with_telegram-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2023-05-11 03:38:44.000000 rum_with_telegram-0.9.5/setup.py
```

### Comparing `rum_with_telegram-0.9.4/LICENSE` & `rum_with_telegram-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.4/PKG-INFO` & `rum_with_telegram-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum_with_telegram
-Version: 0.9.4
+Version: 0.9.5
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.9.4/rum_with_telegram/config.py` & `rum_with_telegram-0.9.5/rum_with_telegram/config.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.4/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-0.9.5/rum_with_telegram/data_exchanger.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,28 +310,31 @@
         logger.info("start handle_reply_message %s", update.message.message_id)
         username = update.message.from_user.username
         userid = update.message.from_user.id
         reply_msg = update.message.reply_to_message
         channel_message_id = reply_msg.forward_from_message_id
         reply_chat_message_id = reply_msg.message_id
         reply_id = None
-        if channel_message_id:
+        if channel_message_id and reply_id is None:
             obj = self.db.get_trx_sent(channel_message_id)
             reply_id = obj.rum_post_id if obj else None
-        elif reply_chat_message_id:
+        if reply_chat_message_id and reply_id is None:
             obj = self.db.get_first(
                 Relation,
                 {"chat_message_id": reply_chat_message_id},
                 "chat_message_id",
             )
             reply_id = obj.rum_post_id if obj else None
             if obj and not channel_message_id:
                 channel_message_id = obj.channel_message_id
+                if reply_id is None:
+                    obj = self.db.get_trx_sent(channel_message_id)
+                    reply_id = obj.rum_post_id if obj else None
 
-        if not channel_message_id and not reply_chat_message_id:
+        if reply_id is None:
             bot = Bot(token=context.bot.token)
             _pinned = await bot.get_chat(self.config.TG_GROUP_ID)
             _pinned = _pinned.pinned_message
             channel_message_id = _pinned.forward_from_message_id
             logger.info("get channel_message_id from pinned %s", channel_message_id)
             reply_id = self.db.get_trx_sent(channel_message_id).rum_post_id
             logger.info("channel_message_id to reply_id %s", reply_id)
@@ -539,15 +542,14 @@
             return
         # TODO
 
     def run(self):
         self.app.add_handler(CommandHandler("start", self.command_start))
         self.app.add_handler(CommandHandler("profile", self.command_profile))
         self.app.add_handler(CommandHandler("show_pvtkey", self.command_show_pvtkey))
-        # TODO: add logs to map userid and pvtkey
         self.app.add_handler(CommandHandler("new_pvtkey", self.command_new_pvtkey))
         self.app.add_handler(CommandHandler("import_pvtkey", self.command_import_pvtkey))
         self.app.add_handler(CommandHandler("export_data", self.command_export_data))
         # TODO:
         self.app.add_handler(CommandHandler("my_nft", self.command_my_nft))
         self.app.add_handler(CommandHandler("grant_nft", self.command_grant_nft))
```

### Comparing `rum_with_telegram-0.9.4/rum_with_telegram/db_handle.py` & `rum_with_telegram-0.9.5/rum_with_telegram/db_handle.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.4/rum_with_telegram/module.py` & `rum_with_telegram-0.9.5/rum_with_telegram/module.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.4/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-0.9.5/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum-with-telegram
-Version: 0.9.4
+Version: 0.9.5
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.9.4/setup.py` & `rum_with_telegram-0.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="0.9.4",
+    version="0.9.5",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
```

