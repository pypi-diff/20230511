# Comparing `tmp/rum_with_telegram-0.9.8.tar.gz` & `tmp/rum_with_telegram-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-0.9.8.tar", last modified: Thu May 11 05:37:34 2023, max compression
+gzip compressed data, was "rum_with_telegram-0.9.9.tar", last modified: Thu May 11 05:50:20 2023, max compression
```

## Comparing `rum_with_telegram-0.9.8.tar` & `rum_with_telegram-0.9.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 05:37:34.522055 rum_with_telegram-0.9.8/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.8/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-05-11 05:37:34.520060 rum_with_telegram-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.8/README.md
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.9.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-11 05:37:34.506133 rum_with_telegram-0.9.8/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-05-11 05:37:08.000000 rum_with_telegram-0.9.8/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0     1955 2023-05-04 04:53:43.000000 rum_with_telegram-0.9.8/rum_with_telegram/config.py
--rw-rw-rw-   0        0        0    25867 2023-05-11 05:36:27.000000 rum_with_telegram-0.9.8/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     3478 2023-05-11 05:36:45.000000 rum_with_telegram-0.9.8/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1850 2023-05-04 04:25:42.000000 rum_with_telegram-0.9.8/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-05-11 05:37:34.518066 rum_with_telegram-0.9.8/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-05-11 05:37:34.000000 rum_with_telegram-0.9.8/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-11 05:37:34.000000 rum_with_telegram-0.9.8/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 05:37:34.000000 rum_with_telegram-0.9.8/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-11 05:37:34.000000 rum_with_telegram-0.9.8/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-11 05:37:34.000000 rum_with_telegram-0.9.8/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 05:37:34.522055 rum_with_telegram-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1430 2023-05-11 05:37:08.000000 rum_with_telegram-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:50:20.006198 rum_with_telegram-0.9.9/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.9/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-05-11 05:50:20.005199 rum_with_telegram-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.9/README.md
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.9.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-11 05:50:19.944361 rum_with_telegram-0.9.9/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-05-11 05:49:31.000000 rum_with_telegram-0.9.9/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0     1955 2023-05-04 04:53:43.000000 rum_with_telegram-0.9.9/rum_with_telegram/config.py
+-rw-rw-rw-   0        0        0    25891 2023-05-11 05:49:36.000000 rum_with_telegram-0.9.9/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     3479 2023-05-11 05:48:50.000000 rum_with_telegram-0.9.9/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1850 2023-05-04 04:25:42.000000 rum_with_telegram-0.9.9/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:50:20.002206 rum_with_telegram-0.9.9/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-05-11 05:50:19.000000 rum_with_telegram-0.9.9/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-11 05:50:19.000000 rum_with_telegram-0.9.9/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 05:50:19.000000 rum_with_telegram-0.9.9/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-11 05:50:19.000000 rum_with_telegram-0.9.9/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-11 05:50:19.000000 rum_with_telegram-0.9.9/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 05:50:20.006198 rum_with_telegram-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2023-05-11 05:49:31.000000 rum_with_telegram-0.9.9/setup.py
```

### Comparing `rum_with_telegram-0.9.8/LICENSE` & `rum_with_telegram-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.8/PKG-INFO` & `rum_with_telegram-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum_with_telegram
-Version: 0.9.8
+Version: 0.9.9
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.9.8/rum_with_telegram/config.py` & `rum_with_telegram-0.9.9/rum_with_telegram/config.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.8/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-0.9.9/rum_with_telegram/data_exchanger.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,17 +273,18 @@
 
     async def handle_channel_message(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         """send message to rum group"""
         # channel post to rum group chain
         if update.channel_post:
             await self._handle_channel_post(update, context)
             return
-        logger.info("handle_channel_message %s", update.message.message_id)
-        channel_message_id = update.message.forward_from_message_id
-        chat_message_id = update.message.message_id
+        message = update.message or update.edited_message
+        logger.info("handle_channel_message %s", message.message_id)
+        channel_message_id = message.forward_from_message_id
+        chat_message_id = message.message_id
 
         # send reply to user in group chat
         for i in range(5):
             obj = self.db.get_trx_sent(channel_message_id)
             if not obj:
                 await asyncio.sleep(0.5)
                 continue
@@ -293,19 +294,19 @@
             else:
                 break
         if not rum_post_url:
             logger.warning("%s not found channel_message_id %s", i, channel_message_id)
             return
         logger.info("found rum_post_url %s", rum_post_url)
         await self._comment_with_feedurl(
-            context, "", update.message.chat.id, chat_message_id, rum_post_url
+            context, "", message.chat.id, chat_message_id, rum_post_url
         )
         payload = {
             "chat_message_id": chat_message_id,
-            "chat_type": update.message.chat.type,
+            "chat_type": message.chat.type,
             "channel_message_id": channel_message_id,
         }
         self.db.add_or_update(Relation, payload, "chat_message_id")
 
     async def _handle_reply_message(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         logger.info("start handle_reply_message %s", update.message.message_id)
         username = update.message.from_user.username
```

### Comparing `rum_with_telegram-0.9.8/rum_with_telegram/db_handle.py` & `rum_with_telegram-0.9.9/rum_with_telegram/db_handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             return session.query(table).filter_by(**{pk: payload[pk]}).all()
 
     def get_trx_sent(self, channel_message_id):
         with self.Session() as session:
             relations = (
                 session.query(Relation)
                 .filter_by(channel_message_id=channel_message_id)
-                .fiter(not_(chat_type="supergroup"))
+                .filter(not_(chat_type="supergroup"))
                 .all()
             )
             for relation in relations:
                 if relation.trx_id:
                     return relation
             relations = (
                 session.query(Relation)
```

### Comparing `rum_with_telegram-0.9.8/rum_with_telegram/module.py` & `rum_with_telegram-0.9.9/rum_with_telegram/module.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.8/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-0.9.9/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum-with-telegram
-Version: 0.9.8
+Version: 0.9.9
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.9.8/setup.py` & `rum_with_telegram-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="0.9.8",
+    version="0.9.9",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
```

