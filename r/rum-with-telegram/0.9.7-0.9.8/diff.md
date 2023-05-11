# Comparing `tmp/rum_with_telegram-0.9.7.tar.gz` & `tmp/rum_with_telegram-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-0.9.7.tar", last modified: Thu May 11 05:03:32 2023, max compression
+gzip compressed data, was "rum_with_telegram-0.9.8.tar", last modified: Thu May 11 05:37:34 2023, max compression
```

## Comparing `rum_with_telegram-0.9.7.tar` & `rum_with_telegram-0.9.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 05:03:32.746887 rum_with_telegram-0.9.7/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.7/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-05-11 05:03:32.745889 rum_with_telegram-0.9.7/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.7/README.md
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.9.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-11 05:03:32.731927 rum_with_telegram-0.9.7/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-05-11 04:58:55.000000 rum_with_telegram-0.9.7/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0     1955 2023-05-04 04:53:43.000000 rum_with_telegram-0.9.7/rum_with_telegram/config.py
--rw-rw-rw-   0        0        0    25871 2023-05-11 04:59:43.000000 rum_with_telegram-0.9.7/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     3345 2023-05-04 04:27:01.000000 rum_with_telegram-0.9.7/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1850 2023-05-04 04:25:42.000000 rum_with_telegram-0.9.7/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-05-11 05:03:32.742897 rum_with_telegram-0.9.7/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-05-11 05:03:32.000000 rum_with_telegram-0.9.7/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-11 05:03:32.000000 rum_with_telegram-0.9.7/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 05:03:32.000000 rum_with_telegram-0.9.7/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-11 05:03:32.000000 rum_with_telegram-0.9.7/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-11 05:03:32.000000 rum_with_telegram-0.9.7/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 05:03:32.746887 rum_with_telegram-0.9.7/setup.cfg
--rw-rw-rw-   0        0        0     1430 2023-05-11 04:58:55.000000 rum_with_telegram-0.9.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:37:34.522055 rum_with_telegram-0.9.8/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.8/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-05-11 05:37:34.520060 rum_with_telegram-0.9.8/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.8/README.md
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.9.8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-11 05:37:34.506133 rum_with_telegram-0.9.8/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-05-11 05:37:08.000000 rum_with_telegram-0.9.8/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0     1955 2023-05-04 04:53:43.000000 rum_with_telegram-0.9.8/rum_with_telegram/config.py
+-rw-rw-rw-   0        0        0    25867 2023-05-11 05:36:27.000000 rum_with_telegram-0.9.8/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     3478 2023-05-11 05:36:45.000000 rum_with_telegram-0.9.8/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1850 2023-05-04 04:25:42.000000 rum_with_telegram-0.9.8/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:37:34.518066 rum_with_telegram-0.9.8/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-05-11 05:37:34.000000 rum_with_telegram-0.9.8/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-11 05:37:34.000000 rum_with_telegram-0.9.8/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 05:37:34.000000 rum_with_telegram-0.9.8/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-11 05:37:34.000000 rum_with_telegram-0.9.8/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-11 05:37:34.000000 rum_with_telegram-0.9.8/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 05:37:34.522055 rum_with_telegram-0.9.8/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2023-05-11 05:37:08.000000 rum_with_telegram-0.9.8/setup.py
```

### Comparing `rum_with_telegram-0.9.7/LICENSE` & `rum_with_telegram-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.7/PKG-INFO` & `rum_with_telegram-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum_with_telegram
-Version: 0.9.7
+Version: 0.9.8
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.9.7/rum_with_telegram/config.py` & `rum_with_telegram-0.9.8/rum_with_telegram/config.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.7/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-0.9.8/rum_with_telegram/data_exchanger.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,15 @@
                 channel_message_id = obj.channel_message_id
                 logger.info(
                     "reply %s to chat_message_id %s channel_message_id %s",
                     reply_id,
                     reply_chat_message_id,
                     channel_message_id,
                 )
-                if reply_id is None and obj.channel_message_id:
+                if reply_id is None and channel_message_id:
                     obj = self.db.get_trx_sent(channel_message_id)
                     reply_id = obj.rum_post_id
                     logger.info("reply_id reset %s", reply_id)
 
         if reply_id is None:
             bot = Bot(token=context.bot.token)
             _pinned = await bot.get_chat(self.config.TG_GROUP_ID)
```

### Comparing `rum_with_telegram-0.9.7/rum_with_telegram/db_handle.py` & `rum_with_telegram-0.9.8/rum_with_telegram/db_handle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
 from quorum_mininode_py import RumAccount
-from sqlalchemy import create_engine
+from sqlalchemy import create_engine, not_
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.sql import func
 
 from rum_with_telegram.module import Base, Relation, UsedKey, User
 
 logger = logging.getLogger(__name__)
 
@@ -44,23 +44,27 @@
 
     def get_all(self, table, payload: dict, pk: str):
         with self.Session() as session:
             return session.query(table).filter_by(**{pk: payload[pk]}).all()
 
     def get_trx_sent(self, channel_message_id):
         with self.Session() as session:
-            relation = (
+            relations = (
                 session.query(Relation)
-                .filter_by(channel_message_id=channel_message_id, chat_type="private")
-                .first()
+                .filter_by(channel_message_id=channel_message_id)
+                .fiter(not_(chat_type="supergroup"))
+                .all()
             )
-            if relation and relation.trx_id:
-                return relation
+            for relation in relations:
+                if relation.trx_id:
+                    return relation
             relations = (
-                session.query(Relation).filter_by(channel_message_id=channel_message_id).all()
+                session.query(Relation)
+                .filter_by(channel_message_id=channel_message_id, chat_type="supergroup")
+                .all()
             )
             for relation in relations:
                 if relation.trx_id:
                     return relation
         return None
 
     def is_exist(self, table, payload: dict, pk: str):
```

### Comparing `rum_with_telegram-0.9.7/rum_with_telegram/module.py` & `rum_with_telegram-0.9.8/rum_with_telegram/module.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.7/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-0.9.8/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum-with-telegram
-Version: 0.9.7
+Version: 0.9.8
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.9.7/setup.py` & `rum_with_telegram-0.9.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="0.9.7",
+    version="0.9.8",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
```

