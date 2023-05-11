# Comparing `tmp/selfcord.py-0.1.3.tar.gz` & `tmp/selfcord.py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfcord.py-0.1.3.tar", last modified: Sat May  6 21:57:31 2023, max compression
+gzip compressed data, was "selfcord.py-0.1.4.tar", last modified: Thu May 11 15:32:31 2023, max compression
```

## Comparing `selfcord.py-0.1.3.tar` & `selfcord.py-0.1.4.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-06 21:57:31.341505 selfcord.py-0.1.3/
--rw-r--r--   0 shell     (1000) shell     (1001)     2546 2023-05-06 21:57:31.338171 selfcord.py-0.1.3/PKG-INFO
--rw-r--r--   0 shell     (1000) shell     (1001)     2259 2023-04-24 19:11:53.000000 selfcord.py-0.1.3/README.md
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-06 21:57:31.288169 selfcord.py-0.1.3/selfcord/
--rw-r--r--   0 shell     (1000) shell     (1001)       80 2023-05-01 21:22:28.000000 selfcord.py-0.1.3/selfcord/__init__.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-06 21:57:31.308170 selfcord.py-0.1.3/selfcord/api/
--rw-r--r--   0 shell     (1000) shell     (1001)       86 2023-05-04 18:44:24.000000 selfcord.py-0.1.3/selfcord/api/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)      562 2023-05-01 21:29:31.000000 selfcord.py-0.1.3/selfcord/api/errors.py
--rw-r--r--   0 shell     (1000) shell     (1001)    11532 2023-05-05 15:18:43.000000 selfcord.py-0.1.3/selfcord/api/events.py
--rw-r--r--   0 shell     (1000) shell     (1001)    18766 2023-05-04 18:21:11.000000 selfcord.py-0.1.3/selfcord/api/gateway.py
--rw-r--r--   0 shell     (1000) shell     (1001)     8009 2023-05-02 22:11:22.000000 selfcord.py-0.1.3/selfcord/api/http.py
--rw-r--r--   0 shell     (1000) shell     (1001)      496 2023-05-05 15:18:26.000000 selfcord.py-0.1.3/selfcord/api/voice.py
--rw-r--r--   0 shell     (1000) shell     (1001)    17999 2023-05-04 23:52:27.000000 selfcord.py-0.1.3/selfcord/bot.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-06 21:57:31.331504 selfcord.py-0.1.3/selfcord/models/
--rw-r--r--   0 shell     (1000) shell     (1001)      353 2023-05-01 18:43:46.000000 selfcord.py-0.1.3/selfcord/models/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)    17143 2023-05-04 23:13:01.000000 selfcord.py-0.1.3/selfcord/models/channel.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1086 2023-05-01 21:28:53.000000 selfcord.py-0.1.3/selfcord/models/client.py
--rw-r--r--   0 shell     (1000) shell     (1001)      935 2023-05-01 21:28:45.000000 selfcord.py-0.1.3/selfcord/models/emoji.py
--rw-r--r--   0 shell     (1000) shell     (1001)     7587 2023-05-04 18:10:43.000000 selfcord.py-0.1.3/selfcord/models/guild.py
--rw-r--r--   0 shell     (1000) shell     (1001)      967 2023-05-01 21:28:32.000000 selfcord.py-0.1.3/selfcord/models/member.py
--rw-r--r--   0 shell     (1000) shell     (1001)     2733 2023-05-01 21:28:28.000000 selfcord.py-0.1.3/selfcord/models/message.py
--rw-r--r--   0 shell     (1000) shell     (1001)     2164 2023-05-01 21:28:21.000000 selfcord.py-0.1.3/selfcord/models/permission.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1591 2023-05-01 21:28:16.000000 selfcord.py-0.1.3/selfcord/models/role.py
--rw-r--r--   0 shell     (1000) shell     (1001)     3933 2023-05-01 21:28:11.000000 selfcord.py-0.1.3/selfcord/models/user.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1367 2023-05-01 21:28:06.000000 selfcord.py-0.1.3/selfcord/models/webhook.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-06 21:57:31.334838 selfcord.py-0.1.3/selfcord/utils/
--rw-r--r--   0 shell     (1000) shell     (1001)      106 2023-05-01 18:43:35.000000 selfcord.py-0.1.3/selfcord/utils/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)    15665 2023-05-04 23:46:51.000000 selfcord.py-0.1.3/selfcord/utils/command.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-06 21:57:31.291502 selfcord.py-0.1.3/selfcord.py.egg-info/
--rw-r--r--   0 shell     (1000) shell     (1001)     2546 2023-05-06 21:57:31.000000 selfcord.py-0.1.3/selfcord.py.egg-info/PKG-INFO
--rw-r--r--   0 shell     (1000) shell     (1001)      732 2023-05-06 21:57:31.000000 selfcord.py-0.1.3/selfcord.py.egg-info/SOURCES.txt
--rw-r--r--   0 shell     (1000) shell     (1001)        1 2023-05-06 21:57:31.000000 selfcord.py-0.1.3/selfcord.py.egg-info/dependency_links.txt
--rw-r--r--   0 shell     (1000) shell     (1001)       65 2023-05-06 21:57:31.000000 selfcord.py-0.1.3/selfcord.py.egg-info/requires.txt
--rw-r--r--   0 shell     (1000) shell     (1001)        9 2023-05-06 21:57:31.000000 selfcord.py-0.1.3/selfcord.py.egg-info/top_level.txt
--rw-r--r--   0 shell     (1000) shell     (1001)       38 2023-05-06 21:57:31.341505 selfcord.py-0.1.3/setup.cfg
--rw-r--r--   0 shell     (1000) shell     (1001)     1004 2023-05-06 21:57:14.000000 selfcord.py-0.1.3/setup.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-06 21:57:31.334838 selfcord.py-0.1.3/tests/
--rw-r--r--   0 shell     (1000) shell     (1001)      455 2023-04-27 00:48:03.000000 selfcord.py-0.1.3/tests/test_commands.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-11 15:32:31.036249 selfcord.py-0.1.4/
+-rw-r--r--   0 shell     (1000) shell     (1001)     4285 2023-05-11 15:32:31.032916 selfcord.py-0.1.4/PKG-INFO
+-rw-r--r--   0 shell     (1000) shell     (1001)     3998 2023-05-09 17:58:36.000000 selfcord.py-0.1.4/README.md
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-11 15:32:30.989581 selfcord.py-0.1.4/selfcord/
+-rw-r--r--   0 shell     (1000) shell     (1001)       80 2023-05-01 21:22:28.000000 selfcord.py-0.1.4/selfcord/__init__.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-11 15:32:31.006248 selfcord.py-0.1.4/selfcord/api/
+-rw-r--r--   0 shell     (1000) shell     (1001)       83 2023-05-09 17:08:02.000000 selfcord.py-0.1.4/selfcord/api/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      562 2023-05-01 21:29:31.000000 selfcord.py-0.1.4/selfcord/api/errors.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    11818 2023-05-09 13:56:43.000000 selfcord.py-0.1.4/selfcord/api/events.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    18766 2023-05-04 18:21:11.000000 selfcord.py-0.1.4/selfcord/api/gateway.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     8009 2023-05-02 22:11:22.000000 selfcord.py-0.1.4/selfcord/api/http.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-11 15:32:31.009582 selfcord.py-0.1.4/selfcord/api/voice/
+-rw-r--r--   0 shell     (1000) shell     (1001)       24 2023-05-07 01:54:34.000000 selfcord.py-0.1.4/selfcord/api/voice/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     7223 2023-05-11 15:29:35.000000 selfcord.py-0.1.4/selfcord/api/voice/voice.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    17994 2023-05-09 17:08:02.000000 selfcord.py-0.1.4/selfcord/bot.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-11 15:32:31.022915 selfcord.py-0.1.4/selfcord/models/
+-rw-r--r--   0 shell     (1000) shell     (1001)      353 2023-05-01 18:43:46.000000 selfcord.py-0.1.4/selfcord/models/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    17143 2023-05-06 22:19:39.000000 selfcord.py-0.1.4/selfcord/models/channel.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     1086 2023-05-01 21:28:53.000000 selfcord.py-0.1.4/selfcord/models/client.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      935 2023-05-01 21:28:45.000000 selfcord.py-0.1.4/selfcord/models/emoji.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     7587 2023-05-04 18:10:43.000000 selfcord.py-0.1.4/selfcord/models/guild.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      967 2023-05-01 21:28:32.000000 selfcord.py-0.1.4/selfcord/models/member.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     2733 2023-05-01 21:28:28.000000 selfcord.py-0.1.4/selfcord/models/message.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     2164 2023-05-01 21:28:21.000000 selfcord.py-0.1.4/selfcord/models/permission.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     1591 2023-05-01 21:28:16.000000 selfcord.py-0.1.4/selfcord/models/role.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     4328 2023-05-11 15:15:00.000000 selfcord.py-0.1.4/selfcord/models/user.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     1367 2023-05-01 21:28:06.000000 selfcord.py-0.1.4/selfcord/models/webhook.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-11 15:32:31.029582 selfcord.py-0.1.4/selfcord/utils/
+-rw-r--r--   0 shell     (1000) shell     (1001)      106 2023-05-01 18:43:35.000000 selfcord.py-0.1.4/selfcord/utils/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    15665 2023-05-09 16:55:24.000000 selfcord.py-0.1.4/selfcord/utils/command.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-11 15:32:30.996248 selfcord.py-0.1.4/selfcord.py.egg-info/
+-rw-r--r--   0 shell     (1000) shell     (1001)     4285 2023-05-11 15:32:30.000000 selfcord.py-0.1.4/selfcord.py.egg-info/PKG-INFO
+-rw-r--r--   0 shell     (1000) shell     (1001)      769 2023-05-11 15:32:30.000000 selfcord.py-0.1.4/selfcord.py.egg-info/SOURCES.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)        1 2023-05-11 15:32:30.000000 selfcord.py-0.1.4/selfcord.py.egg-info/dependency_links.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)       65 2023-05-11 15:32:30.000000 selfcord.py-0.1.4/selfcord.py.egg-info/requires.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)        9 2023-05-11 15:32:30.000000 selfcord.py-0.1.4/selfcord.py.egg-info/top_level.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)       38 2023-05-11 15:32:31.036249 selfcord.py-0.1.4/setup.cfg
+-rw-r--r--   0 shell     (1000) shell     (1001)     1026 2023-05-11 15:31:53.000000 selfcord.py-0.1.4/setup.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-11 15:32:31.029582 selfcord.py-0.1.4/tests/
+-rw-r--r--   0 shell     (1000) shell     (1001)      455 2023-04-27 00:48:03.000000 selfcord.py-0.1.4/tests/test_commands.py
```

### Comparing `selfcord.py-0.1.3/selfcord/api/errors.py` & `selfcord.py-0.1.4/selfcord/api/errors.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.3/selfcord/api/events.py` & `selfcord.py-0.1.4/selfcord/api/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,33 +267,38 @@
         """Handles the voice state updating
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
-        if data['channel'] != None:
+        if data['channel_id'] != None:
             self.session_id = data['session_id']
 
     async def handle_voice_server_update(self, data: dict, user: Client, http):
         """Handles the voice server updating
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
         self.token = data['token']
         self.endpoint = data['endpoint']
-        self.guild_id = data['guild_id']
+        if data['guild_id'] != None:
+            self.server_id = data['guild_id']
+        else:
+            self.server_id = data['channel_id']
         await asyncio.sleep(1)
-        self.voice = Voice(self.session_id, self.token, self.endpoint, self.guild_id, self.bot)
-
-
+        self.voice = Voice(self.session_id, self.token, self.endpoint, self.server_id, self.bot)
+        await self.voice_start(self.voice)
 
+    async def voice_start(self, voice: Voice):
+        asyncio.create_task(voice.start())
+        setattr(self.bot, "voice", self.voice)
```

### Comparing `selfcord.py-0.1.3/selfcord/api/gateway.py` & `selfcord.py-0.1.4/selfcord/api/gateway.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.3/selfcord/api/http.py` & `selfcord.py-0.1.4/selfcord/api/http.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.3/selfcord/bot.py` & `selfcord.py-0.1.4/selfcord/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
             def clean_code(content):
                 if content.startswith("```") and content.endswith("```"):
                     return "\n".join(content.split("\n")[1:])[:-3]
                 else:
                     return content
 
             @self.cmd(description="Executes and runs code", aliases=['exec'])
-            async def eval(ctx, *, code: str):
+            async def eval(ctx, *, code):
                 """Runs python code via exec, intended for experienced usage. This can be DANGEROUS if you do not know what you are doing, use with caution.
                 """
                 code = clean_code(code)
 
                 try:
                     with contextlib.redirect_stdout(io.StringIO()) as f:
                         await aexec(code)
```

### Comparing `selfcord.py-0.1.3/selfcord/models/channel.py` & `selfcord.py-0.1.4/selfcord/models/channel.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.3/selfcord/models/client.py` & `selfcord.py-0.1.4/selfcord/models/client.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.3/selfcord/models/emoji.py` & `selfcord.py-0.1.4/selfcord/models/emoji.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.3/selfcord/models/guild.py` & `selfcord.py-0.1.4/selfcord/models/guild.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.3/selfcord/models/member.py` & `selfcord.py-0.1.4/selfcord/models/member.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.3/selfcord/models/message.py` & `selfcord.py-0.1.4/selfcord/models/message.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.3/selfcord/models/permission.py` & `selfcord.py-0.1.4/selfcord/models/permission.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.3/selfcord/models/role.py` & `selfcord.py-0.1.4/selfcord/models/role.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.3/selfcord/models/user.py` & `selfcord.py-0.1.4/selfcord/models/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,7 +124,21 @@
         """
         data = await self.http.request(method="get", endpoint=f"/users/{self.id}/profile?with_mutual_guilds=true")
 
         if data != None:
             data = Profile(data, self.bot, self.http)
 
         return data
+
+    async def get_mutual_friends(self) -> list[User]:
+        """Get the User mutual friends
+
+        Returns:
+            list[User]: Mutual friends
+        """
+        data = await self.http.request(method="get", endpoint=f"/users/{self.id}/relationships")
+
+        if len(data) != 0:
+            return [User(user, self.bot, self.http) for user in data]
+        else:
+            return []
+
```

### Comparing `selfcord.py-0.1.3/selfcord/models/webhook.py` & `selfcord.py-0.1.4/selfcord/models/webhook.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.3/selfcord/utils/command.py` & `selfcord.py-0.1.4/selfcord/utils/command.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.3/selfcord.py.egg-info/SOURCES.txt` & `selfcord.py-0.1.4/selfcord.py.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 selfcord.py.egg-info/requires.txt
 selfcord.py.egg-info/top_level.txt
 selfcord/api/__init__.py
 selfcord/api/errors.py
 selfcord/api/events.py
 selfcord/api/gateway.py
 selfcord/api/http.py
-selfcord/api/voice.py
+selfcord/api/voice/__init__.py
+selfcord/api/voice/voice.py
 selfcord/models/__init__.py
 selfcord/models/channel.py
 selfcord/models/client.py
 selfcord/models/emoji.py
 selfcord/models/guild.py
 selfcord/models/member.py
 selfcord/models/message.py
```

### Comparing `selfcord.py-0.1.3/setup.py` & `selfcord.py-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 if __name__ == "__main__":
     this_directory = Path(__file__).parent
     long_description = ( this_directory /"README.md").read_text()
     setup(
         name="selfcord.py",
-        packages=find_packages(include=['selfcord', 'selfcord.api', 'selfcord.utils', 'selfcord.models']),
-        version="0.1.3",
+        packages=find_packages(include=['selfcord', 'selfcord.api', 'selfcord.utils', 'selfcord.models', 'selfcord.api.voice']),
+        version="0.1.4",
         description="A Discord API wrapper designed for selfbots!",
         readme="README.md",
         author="Shell of OMEGA",
         license="MIT",
         install_requires=["aiohttp==3.7.4.post0","aioconsole==0.3.3", "websockets==10.1", "requests"],
         setup_requires=['pytest-runner'],
         tests_require=['pytest'],
```

