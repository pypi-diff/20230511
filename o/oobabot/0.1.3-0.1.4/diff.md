# Comparing `tmp/oobabot-0.1.3.tar.gz` & `tmp/oobabot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oobabot-0.1.3.tar", max compression
+gzip compressed data, was "oobabot-0.1.4.tar", max compression
```

## Comparing `oobabot-0.1.3.tar` & `oobabot-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1067 2023-05-03 00:11:59.534663 oobabot-0.1.3/LICENSE
--rw-r--r--   0        0        0     8513 2023-05-07 08:27:31.575186 oobabot-0.1.3/README.md
--rw-r--r--   0        0        0      967 2023-05-07 08:29:52.158852 oobabot-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       80 2023-05-07 08:29:39.308544 oobabot-0.1.3/src/oobabot/__init__.py
--rw-r--r--   0        0        0       69 2023-05-05 00:57:20.206747 oobabot-0.1.3/src/oobabot/__main__.py
--rw-r--r--   0        0        0    13698 2023-05-07 08:22:57.238237 oobabot-0.1.3/src/oobabot/discord_bot.py
--rw-r--r--   0        0        0     1572 2023-05-05 00:57:22.929461 oobabot-0.1.3/src/oobabot/fancy_logging.py
--rw-r--r--   0        0        0     3296 2023-05-05 00:57:24.331138 oobabot-0.1.3/src/oobabot/ooba_client.py
--rwxr-xr-x   0        0        0     2157 2023-05-05 00:57:25.553393 oobabot-0.1.3/src/oobabot/oobabot.py
--rw-r--r--   0        0        0     6586 2023-05-05 00:57:26.704654 oobabot-0.1.3/src/oobabot/response_stats.py
--rw-r--r--   0        0        0     2695 2023-05-05 00:57:27.771786 oobabot-0.1.3/src/oobabot/sentence_splitter.py
--rw-r--r--   0        0        0     3981 2023-05-05 00:57:28.849070 oobabot-0.1.3/src/oobabot/settings.py
--rw-r--r--   0        0        0     9346 1970-01-01 00:00:00.000000 oobabot-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-04 00:39:46.200078 oobabot-0.1.4/LICENSE
+-rw-r--r--   0        0        0    11382 2023-05-10 23:17:09.014151 oobabot-0.1.4/README.md
+-rw-r--r--   0        0        0      967 2023-05-10 23:13:03.004218 oobabot-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-05-10 23:21:59.614073 oobabot-0.1.4/src/oobabot/__init__.py
+-rw-r--r--   0        0        0       69 2023-05-09 03:46:59.468832 oobabot-0.1.4/src/oobabot/__main__.py
+-rw-r--r--   0        0        0    27234 2023-05-10 02:23:25.013734 oobabot-0.1.4/src/oobabot/discord_bot.py
+-rw-r--r--   0        0        0     1572 2023-05-09 03:46:59.468832 oobabot-0.1.4/src/oobabot/fancy_logging.py
+-rw-r--r--   0        0        0     4989 2023-05-10 00:01:52.945718 oobabot-0.1.4/src/oobabot/ooba_client.py
+-rwxr-xr-x   0        0        0     2645 2023-05-10 01:43:04.854299 oobabot-0.1.4/src/oobabot/oobabot.py
+-rw-r--r--   0        0        0     6586 2023-05-09 03:46:59.468832 oobabot-0.1.4/src/oobabot/response_stats.py
+-rw-r--r--   0        0        0    10818 2023-05-10 00:01:52.945718 oobabot-0.1.4/src/oobabot/sd_client.py
+-rw-r--r--   0        0        0     2695 2023-05-09 03:46:59.468832 oobabot-0.1.4/src/oobabot/sentence_splitter.py
+-rw-r--r--   0        0        0     6656 2023-05-10 01:39:31.894349 oobabot-0.1.4/src/oobabot/settings.py
+-rw-r--r--   0        0        0    12218 1970-01-01 00:00:00.000000 oobabot-0.1.4/PKG-INFO
```

### Comparing `oobabot-0.1.3/LICENSE` & `oobabot-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.3/README.md` & `oobabot-0.1.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 | **multiple converations** | can track multiple conversational threads, and reply to each in a contextually appropriate way |
 | **watchwords** | can monitor all channels in a server for one or more wakewords or @-mentions |
 | **private conversations** | can chat with you 1:1 in a DM |
 | **good Discord hygiene** | splits messages into independent sentences, pings the author in the first one |
 | **low-latency** | streams the reply live, sentence by sentence.  Provides lower latency, especially on longer responses. |
 | **stats** | track token generation speed, latency, failures and usage |
 | **easy networking** | connects to discord from your machine using websockets, so no need to expose a server to the internet |
+| ✨**Stable Diffusion** | new in v0.1.4!  Optional image generation with AUTOMATIC1111 |
 
 ## Getting Started with **`oobabot`**
 
 ### See the [Installation Guide](./docs/INSTALL.md) for step-by-step instructions
 
 ## Installation tl;dr
 
@@ -67,40 +68,62 @@
 
 ~: oobabot --base-url ws://oobabooga-hostname:5005/ --ai-name YourBotsName --persona "You are a cat named YourBotsName"
 ```
 
 You should now be able to run oobabot from wherever pip installed it.
 
 ```none
-usage: oobabot [-h] [--base-url BASE_URL] [--ai-name AI_NAME] [--wakewords [WAKEWORDS ...]]
-               [--persona PERSONA] [--local-repl] [--log-all-the-things LOG_ALL_THE_THINGS]
+usage: oobabot [-h] [--ai-name AI_NAME] [--wakewords [WAKEWORDS ...]] [--ignore-dms]
+               [--base-url BASE_URL] [--persona PERSONA] [--log-all-the-things]
+               [--stable-diffusion-url STABLE_DIFFUSION_URL]
+               [--stable-diffusion-sampler STABLE_DIFFUSION_SAMPLER]
+               [--stable-diffusion-negative-prompt STABLE_DIFFUSION_NEGATIVE_PROMPT]
+               [--stable-diffusion-negative-prompt-nsfw STABLE_DIFFUSION_NEGATIVE_PROMPT_NSFW]
 
 Discord bot for oobabooga's text-generation-webui
 
 options:
   -h, --help            show this help message and exit
-  --base-url BASE_URL   Base URL for the oobabooga instance. This should be ws://hostname[:port] for
-                        plain websocket connections, or wss://hostname[:port] for websocket
-                        connections over TLS.
-  --ai-name AI_NAME     Name of the AI to use for requests. This can be whatever you want, but might
-                        make sense to be the name of the bot in Discord.
+
+Discord Settings:
+  --ai-name AI_NAME     Name of the AI to use for requests. This can be whatever you want, but
+                        might make sense to be the name of the bot in Discord.
   --wakewords [WAKEWORDS ...]
                         One or more words that the bot will listen for. The bot will listen in all
                         discord channels can access for one of these words to be mentioned, then
-                        reply to any messages it sees with a matching word. The bot will always reply
-                        to @-mentions and direct messages, even if no wakewords are supplied.
+                        reply to any messages it sees with a matching word. The bot will always
+                        reply to @-mentions and direct messages, even if no wakewords are supplied.
+  --ignore-dms          If set, the bot will ignore direct messages.
+
+Oobabooga Seetings:
+  --base-url BASE_URL   Base URL for the oobabooga instance. This should be ws://hostname[:port]
+                        for plain websocket connections, or wss://hostname[:port] for websocket
+                        connections over TLS.
   --persona PERSONA     This prefix will be added in front of every user-supplied request. This is
-                        useful for setting up a 'character' for the bot to play. Alternatively, this
-                        can be set with the OOBABOT_PERSONA environment variable.
-  --local-repl          start a local REPL, instead of connecting to Discord
-  --log-all-the-things LOG_ALL_THE_THINGS
-                        prints all oobabooga requests and responses in their entirety to STDOUT
+                        useful for setting up a 'character' for the bot to play. Alternatively,
+                        this can be set with the OOBABOT_PERSONA environment variable.
+  --log-all-the-things  Prints all oobabooga requests and responses in their entirety to STDOUT
+
+Stable Diffusion Settings:
+  --stable-diffusion-url STABLE_DIFFUSION_URL
+                        URL for an AUTOMATIC1111 Stable Diffusion server
+  --stable-diffusion-sampler STABLE_DIFFUSION_SAMPLER
+                        Sampler to use when generating images. If not specified, the one set on the
+                        AUTOMATIC1111 server will be used.
+  --stable-diffusion-negative-prompt STABLE_DIFFUSION_NEGATIVE_PROMPT
+                        Negative prompt to use when generating images. This will discourage Stable
+                        Diffusion from generating images with the specified content. By default,
+                        this is set to follow Discord's TOS.
+  --stable-diffusion-negative-prompt-nsfw STABLE_DIFFUSION_NEGATIVE_PROMPT_NSFW
+                        Negative prompt to use when generating images in a channel marked as'Age-
+                        Restricted'. By default, this follows the Discord TOS by allowing some
+                        sexual content forbidden in non-age-restricted channels.
 
-Also, to authenticate to Discord, you must set the environment variable: DISCORD_TOKEN = <your bot's
-discord token>
+Also, to authenticate to Discord, you must set the environment variable: DISCORD_TOKEN = <your
+bot's discord token>
 ```
 
 ## Required settings
 
 - **`DISCORD_TOKEN`** environment variable
 
    Set your shell environment's **`DISCORD_TOKEN`** to token Discord provided when you set up the bot account.  It should be something like a 72-character-long random-looking string.
@@ -138,18 +161,14 @@
 
    the name the AI will be instructed to call itself.  Note that this technically doesn't need to be the same as the bot in your discord, but it would likely make sense to your users if they are at least similar.
 
 - **`--wakewords`**
 
    one or more words that the bot will look for.  It will reply to any message which contains one of these words, in any channel.
 
-- **`--local-repl`**
-
-    instead of connecting to discord, just start up a local REPL and send these prompts directly to the oobabooga server.  Useful if you want to test if that part is working in isolation.  Note that in this mode you will be sending the oobabooga server raw input, and so the persona or AI name settings will be ignored.
-
 ## Persona: the fun setting
 
 - **`--persona`**
 
     is a short few sentences describing the role your bot should act as.  For instance, this is the setting I'm using for my cat-bot, whose name is "Rosie".
 
 ```console
@@ -173,14 +192,52 @@
 
 You should see something like this if everything worked:
 
 ![oobabot running!](./docs/oobabot-cli.png "textually interesting image")
 
 ---
 
+## Stable Diffusion via AUTOMATIC1111
+
+- **`--stable-diffusion-url`**
+
+  is the URL to a server running [AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui)
+
+  With it, users can ask **`oobabot`** to generate images and post the
+  results to the channel.  The user who made the original request can
+  choose to regenerate the image as they like.  If they either don't
+  find one they like, or don't do anything within 3 minutes, the image
+  will be removed.
+
+  ![oobabot running!](./docs/zombietaytay.png "textually interesting image")
+
+  Currently, detection of photo requests is very crude, and is only looking
+  for messages which match this regex:
+
+  ```python
+        photowords = ["drawing", "photo", "pic", "picture", "image", "sketch"]
+        self.photo_patterns = [
+            re.compile(
+                r"^.*\b" + photoword + r"\b[\s]*(of|with)?[\s]*[:]?(.*)$", re.IGNORECASE
+            )
+            for photoword in photowords
+        ]
+  ```
+
+  Note that depending on the checkpoint loaded in Stable Diffusion, it may not be appropriate
+  for your server's community.  I suggest reviewing [Discord's Terms of Service](https://discord.com/terms) and
+  [Community Guidelines](https://discord.com/guidelines) before deciding what checkpoint to run.
+
+  **`oobabot`** supports two different negative prompts, depending on whether the channel
+  is marked as "Age-Restricted" or not.  This is to allow for more explicit content in
+  channels which are marked as such.  While the negative prompt will discourage Stable
+  Diffusion from generating an image which matches the prompt, but is not foolproof.
+
+---
+
 ## Interacting with **`oobabot`**
 
 By default, **`oobabot`** will listen for three types of messages in the servers it's connected to:
 
  1. any message in which **`oobabot`**'s account is @-mentioned
  1. any direct message
  1. any message containing a provided wakeword (see Optional Settings)
@@ -188,10 +245,12 @@
 Also, the bot has a random chance of sending follow-up messages within the
 same channel if others reply within 120 seconds of its last post.  The exact
 parameters for this are in flux, but is meant to simulate a natural conversation
 flow, without forcing others to always post a wakeword.
 
 ## Known Issues
 
-- ooba's text generation can error with OOM when more than one request comes in at once.
+- detection of requests for photos is very crude, and will likely be improved in the future.
+- some of the default settings are very specific to my use case, and will likely be made
+  configurable in the future
 - sometimes the bot wants to continue conversations on behalf of other members of the chatroom.  I have some hacks in place to notice and truncate this behavior, but it can lead to terse responses on occasion.
-- found one not listed here?  [Create an issue](https://github.com/chrisrude/oobabot/issues) on github!
+- found one not listed here?  Have an idea?  [Create an issue](https://github.com/chrisrude/oobabot/issues) on github!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `oobabot-0.1.3/pyproject.toml` & `oobabot-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "oobabot"
-version = "0.1.3"
+version = "0.1.4"
 description = "A Discord bot which talks to Large Language Model AIs running on oobabooga's text-generation-webui"
 authors = ["Christopher Rude <chris@rudesoftware.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/chrisrude/oobabot"
 
 [tool.poetry.dependencies]
+aiohttp = "^3.8.4"
 python = "^3.8"
 "discord.py" = "^2.2.2"
 pysbd = "^0.3.4"
-websockets = "^11"
 
 [tool.poetry.scripts]
 oobabot = 'oobabot.oobabot:main'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `oobabot-0.1.3/src/oobabot/fancy_logging.py` & `oobabot-0.1.4/src/oobabot/fancy_logging.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.3/src/oobabot/oobabot.py` & `oobabot-0.1.4/src/oobabot/oobabot.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 #
 
 import asyncio
 import signal
 import sys
 
 from oobabot.discord_bot import DiscordBot
+from oobabot.fancy_logging import get_logger
 from oobabot.fancy_logging import init_logging
 from oobabot.ooba_client import OobaClient
 from oobabot.ooba_client import OobaClientError
+from oobabot.sd_client import StableDiffusionClient
 from oobabot.settings import Settings
 
 
-class LocalREPL:
-    # local REPL for testing
-    def __init__(self, ooba_client):
-        self.ooba_client = ooba_client
-
-    def show_prompt(self) -> None:
-        print("\n>>> ", end="", flush=True)
-
-    async def start(self) -> None:
-        self.show_prompt()
-        for user_prompt in sys.stdin:
-            async for token in self.ooba_client.request_by_token(user_prompt):
-                if token:
-                    print(token, end="", flush=True)
-                else:
-                    # end of response
-                    print("")
-            self.show_prompt()
+def verify_client(client, service_name, url):
+    async def try_setup(client):
+        assert client is not None
+        async with client:
+            await client.setup()
+
+    logger = get_logger()
+    logger.info(f"{service_name} is at {url}")
+    try:
+        asyncio.run(try_setup(client))
+    except OobaClientError as e:
+        logger.error(f"Could not connect to {service_name} server: [{url}]")
+        logger.error("Please check the URL and try again.")
+        logger.error(f"Reason: {e}")
+        sys.exit(1)
+    logger.info(f"Connected to {service_name}!")
 
 
 def main():
     logger = init_logging()
     settings = Settings()
 
     bot = None
@@ -43,35 +43,46 @@
         logger.info("Received SIGINT, exiting...")
         if bot:
             bot.log_stats()
         exit(1)
 
     signal.signal(signal.SIGINT, sigint_handler)
 
-    ooba_client = OobaClient(settings.base_url)
+    ########################################################
+    # Connect to Oobabooga
 
-    logger.debug(f"Oobabooga base URL: {settings.base_url}")
-    try:
-        asyncio.run(ooba_client.try_connect())
-    except OobaClientError as e:
-        logger.error(f"Could not connect to ooba server: [{ooba_client.api_url}]")
-        logger.error("Please check the URL and try again.")
-        logger.error(f"Reason: {e}")
-        sys.exit(1)
+    ooba_client = OobaClient(settings.base_url)
+    verify_client(ooba_client, "Oobabooga", settings.base_url)
 
-    logger.info("Connected to Oobabooga!")
+    ########################################################
+    # Connect to Stable Diffusion, if configured
 
-    if settings.local_repl:
-        logger.debug("Using local REPL, not connecting to Discord")
-        coroutine = LocalREPL(ooba_client).start()
-    else:
-        logger.debug("Connecting to Discord... ")
-        bot = DiscordBot(
-            ooba_client,
-            ai_name=settings.ai_name,
-            ai_persona=settings.persona,
-            wakewords=settings.wakewords,
-            log_all_the_things=settings.log_all_the_things,
+    stable_diffusion_client = None
+    if settings.stable_diffusion_url:
+        stable_diffusion_client = StableDiffusionClient(
+            settings.stable_diffusion_url,
+            negative_prompt=settings.stable_diffusion_negative_prompt,
+            negative_prompt_nsfw=settings.stable_diffusion_negative_prompt_nsfw,
+            desired_sampler=settings.stable_diffusion_sampler,
+        )
+        verify_client(
+            stable_diffusion_client,
+            "Stable Diffusion",
+            settings.stable_diffusion_url,
         )
-        coroutine = bot.start(settings.DISCORD_TOKEN)
+
+    ########################################################
+    # Connect to Discord
+
+    logger.info("Connecting to Discord... ")
+    bot = DiscordBot(
+        ooba_client,
+        ai_name=settings.ai_name,
+        ai_persona=settings.persona,
+        wakewords=settings.wakewords,
+        log_all_the_things=settings.log_all_the_things,
+        ignore_dms=settings.ignore_dms,
+        stable_diffusion_client=stable_diffusion_client,
+    )
+    coroutine = bot.start(settings.DISCORD_TOKEN)
 
     asyncio.run(coroutine)
```

### Comparing `oobabot-0.1.3/src/oobabot/response_stats.py` & `oobabot-0.1.4/src/oobabot/response_stats.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.3/src/oobabot/sentence_splitter.py` & `oobabot-0.1.4/src/oobabot/sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.3/src/oobabot/settings.py` & `oobabot-0.1.4/src/oobabot/settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,84 +11,149 @@
 
     OOBABOT_PERSONA_ENV_VAR = "OOBABOT_PERSONA"
     OOBABOT_PERSONA = os.environ.get(OOBABOT_PERSONA_ENV_VAR, "")
 
     DEFAULT_WAKEWORDS = ["oobabot"]
     DEFAULT_URL = "ws://localhost:5005"
 
+    # use this prompt for "age_restricted" Dsicord channels
+    #  i.e. channel.nsfw is true
+    DEFAULT_SD_NEGATIVE_PROMPT_NSFW = (
+        "animal harm, "
+        + "suicide, self-harm, "
+        + "excessive violence, "
+        + "naked children, child sexualization, lolicon"
+    )
+
+    # use this prompt for non-age-restricted channels
+    DEFAULT_SD_NEGATIVE_PROMPT = (
+        DEFAULT_SD_NEGATIVE_PROMPT_NSFW + ", sexually explicit content"
+    )
+
     def __init__(self):
         self._settings = None
         self.wakewords = []
 
         super().__init__(
             description="Discord bot for oobabooga's text-generation-webui",
             epilog="Also, to authenticate to Discord, you must set the "
             + "environment variable:\n"
             f"\t{self.DISCORD_TOKEN_ENV_VAR} = <your bot's discord token>",
         )
-        self.add_argument(
-            "--base-url",
-            type=str,
-            default=self.DEFAULT_URL,
-            help="Base URL for the oobabooga instance.  "
-            + "This should be ws://hostname[:port] for plain websocket "
-            + "connections, or wss://hostname[:port] for websocket "
-            + "connections over TLS.",
-        )
-        self.add_argument(
+
+        ###########################################################
+        # Discord Settings
+
+        discord_group = self.add_argument_group("Discord Settings")
+        discord_group.add_argument(
             "--ai-name",
             type=str,
             default="oobabot",
             help="Name of the AI to use for requests.  "
             + "This can be whatever you want, but might make sense "
             + "to be the name of the bot in Discord.",
         )
-        self.add_argument(
+        discord_group.add_argument(
             "--wakewords",
             type=str,
             nargs="*",
             default=self.DEFAULT_WAKEWORDS,
             help="One or more words that the bot will listen for.\n "
             + "The bot will listen in all discord channels can "
             + "access for one of these words to be mentioned, then reply "
             + "to any messages it sees with a matching word.  "
             + "The bot will always reply to @-mentions and "
             + "direct messages, even if no wakewords are supplied.",
         )
-        self.add_argument(
+        discord_group.add_argument(
+            "--ignore-dms",
+            default=False,
+            help="If set, the bot will ignore direct messages.",
+            action="store_true",
+        )
+
+        ###########################################################
+        # Oobabooga Settings
+
+        oobabooga_group = self.add_argument_group("Oobabooga Seetings")
+        oobabooga_group.add_argument(
+            "--base-url",
+            type=str,
+            default=self.DEFAULT_URL,
+            help="Base URL for the oobabooga instance.  "
+            + "This should be ws://hostname[:port] for plain websocket "
+            + "connections, or wss://hostname[:port] for websocket "
+            + "connections over TLS.",
+        )
+
+        oobabooga_group.add_argument(
             "--persona",
             type=str,
             default=self.OOBABOT_PERSONA,
             help="This prefix will be added in front of every user-supplied "
             + "request.  This is useful for setting up a 'character' for the "
             + "bot to play.  Alternatively, this can be set with the "
             + f"{self.OOBABOT_PERSONA_ENV_VAR} environment variable.",
         )
-        self.add_argument(
-            "--local-repl",
-            default=False,
-            help="start a local REPL, instead of connecting to Discord",
-            action="store_true",
-        )
-        self.add_argument(
+
+        oobabooga_group.add_argument(
             "--log-all-the-things",
             default=False,
-            help="prints all oobabooga requests and responses in their "
+            help="Prints all oobabooga requests and responses in their "
             + "entirety to STDOUT",
             action="store_true",
         )
 
+        ###########################################################
+        # Stable Diffusion Settings
+
+        stable_diffusion_group = self.add_argument_group("Stable Diffusion Settings")
+        stable_diffusion_group.add_argument(
+            "--stable-diffusion-url",
+            type=str,
+            default=None,
+            help="URL for an AUTOMATIC1111 Stable Diffusion server",
+        )
+        stable_diffusion_group.add_argument(
+            "--stable-diffusion-sampler",
+            type=str,
+            default=None,
+            help="Sampler to use when generating images.  If not specified, the one "
+            + "set on the AUTOMATIC1111 server will be used.",
+        )
+        stable_diffusion_group.add_argument(
+            "--stable-diffusion-negative-prompt",
+            type=str,
+            default=self.DEFAULT_SD_NEGATIVE_PROMPT,
+            help="Negative prompt to use when generating images.  This will discourage"
+            + " Stable Diffusion from generating images with the specified content.  "
+            + "By default, this is set to follow Discord's TOS.",
+        )
+        stable_diffusion_group.add_argument(
+            "--stable-diffusion-negative-prompt-nsfw",
+            type=str,
+            default=self.DEFAULT_SD_NEGATIVE_PROMPT_NSFW,
+            help="Negative prompt to use when generating images in a channel marked as"
+            + "'Age-Restricted'.  By default, this follows the Discord TOS by allowing "
+            + "some sexual content forbidden in non-age-restricted channels.",
+        )
+
     def settings(self) -> dict[str, str]:
         if self._settings is None:
             self._settings = self.parse_args().__dict__
 
             # this is a bit of a hack, but by doing this with
             # non-str settings, we can add stronger type hints
             self.wakewords = self._settings.pop("wakewords")
             self.log_all_the_things = self._settings.pop("log_all_the_things")
+            self.stable_diffusion_url = self._settings.pop("stable_diffusion_url")
+            self.stable_diffusion_sampler = self._settings.pop(
+                "stable_diffusion_sampler"
+            )
+            self.ignore_dms = self._settings.pop("ignore_dms")
 
             # either we're using a local REPL, or we're connecting to Discord.
             # assume the user wants to connect to Discord
             if not (self.local_repl or self.DISCORD_TOKEN):
                 msg = (
                     f"Please set the '{Settings.DISCORD_TOKEN_ENV_VAR}' "
                     + "environment variable to your bot's discord token."
```

### Comparing `oobabot-0.1.3/PKG-INFO` & `oobabot-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: oobabot
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Discord bot which talks to Large Language Model AIs running on oobabooga's text-generation-webui
 Home-page: https://github.com/chrisrude/oobabot
 License: MIT
 Author: Christopher Rude
 Author-email: chris@rudesoftware.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: discord.py (>=2.2.2,<3.0.0)
 Requires-Dist: pysbd (>=0.3.4,<0.4.0)
-Requires-Dist: websockets (>=11,<12)
 Project-URL: Repository, https://github.com/chrisrude/oobabot
 Description-Content-Type: text/markdown
 
 # `oobabot`
 
 **`oobabot`** is a Discord bot which talks to a Large Language Model AIs (like LLaMA, llama.cpp, etc...), running on [oobabooga's text-generation-webui](https://github.com/oobabooga/text-generation-webui).
 
@@ -66,14 +66,15 @@
 | **multiple converations** | can track multiple conversational threads, and reply to each in a contextually appropriate way |
 | **watchwords** | can monitor all channels in a server for one or more wakewords or @-mentions |
 | **private conversations** | can chat with you 1:1 in a DM |
 | **good Discord hygiene** | splits messages into independent sentences, pings the author in the first one |
 | **low-latency** | streams the reply live, sentence by sentence.  Provides lower latency, especially on longer responses. |
 | **stats** | track token generation speed, latency, failures and usage |
 | **easy networking** | connects to discord from your machine using websockets, so no need to expose a server to the internet |
+| ✨**Stable Diffusion** | new in v0.1.4!  Optional image generation with AUTOMATIC1111 |
 
 ## Getting Started with **`oobabot`**
 
 ### See the [Installation Guide](./docs/INSTALL.md) for step-by-step instructions
 
 ## Installation tl;dr
 
@@ -88,40 +89,62 @@
 
 ~: oobabot --base-url ws://oobabooga-hostname:5005/ --ai-name YourBotsName --persona "You are a cat named YourBotsName"
 ```
 
 You should now be able to run oobabot from wherever pip installed it.
 
 ```none
-usage: oobabot [-h] [--base-url BASE_URL] [--ai-name AI_NAME] [--wakewords [WAKEWORDS ...]]
-               [--persona PERSONA] [--local-repl] [--log-all-the-things LOG_ALL_THE_THINGS]
+usage: oobabot [-h] [--ai-name AI_NAME] [--wakewords [WAKEWORDS ...]] [--ignore-dms]
+               [--base-url BASE_URL] [--persona PERSONA] [--log-all-the-things]
+               [--stable-diffusion-url STABLE_DIFFUSION_URL]
+               [--stable-diffusion-sampler STABLE_DIFFUSION_SAMPLER]
+               [--stable-diffusion-negative-prompt STABLE_DIFFUSION_NEGATIVE_PROMPT]
+               [--stable-diffusion-negative-prompt-nsfw STABLE_DIFFUSION_NEGATIVE_PROMPT_NSFW]
 
 Discord bot for oobabooga's text-generation-webui
 
 options:
   -h, --help            show this help message and exit
-  --base-url BASE_URL   Base URL for the oobabooga instance. This should be ws://hostname[:port] for
-                        plain websocket connections, or wss://hostname[:port] for websocket
-                        connections over TLS.
-  --ai-name AI_NAME     Name of the AI to use for requests. This can be whatever you want, but might
-                        make sense to be the name of the bot in Discord.
+
+Discord Settings:
+  --ai-name AI_NAME     Name of the AI to use for requests. This can be whatever you want, but
+                        might make sense to be the name of the bot in Discord.
   --wakewords [WAKEWORDS ...]
                         One or more words that the bot will listen for. The bot will listen in all
                         discord channels can access for one of these words to be mentioned, then
-                        reply to any messages it sees with a matching word. The bot will always reply
-                        to @-mentions and direct messages, even if no wakewords are supplied.
+                        reply to any messages it sees with a matching word. The bot will always
+                        reply to @-mentions and direct messages, even if no wakewords are supplied.
+  --ignore-dms          If set, the bot will ignore direct messages.
+
+Oobabooga Seetings:
+  --base-url BASE_URL   Base URL for the oobabooga instance. This should be ws://hostname[:port]
+                        for plain websocket connections, or wss://hostname[:port] for websocket
+                        connections over TLS.
   --persona PERSONA     This prefix will be added in front of every user-supplied request. This is
-                        useful for setting up a 'character' for the bot to play. Alternatively, this
-                        can be set with the OOBABOT_PERSONA environment variable.
-  --local-repl          start a local REPL, instead of connecting to Discord
-  --log-all-the-things LOG_ALL_THE_THINGS
-                        prints all oobabooga requests and responses in their entirety to STDOUT
+                        useful for setting up a 'character' for the bot to play. Alternatively,
+                        this can be set with the OOBABOT_PERSONA environment variable.
+  --log-all-the-things  Prints all oobabooga requests and responses in their entirety to STDOUT
+
+Stable Diffusion Settings:
+  --stable-diffusion-url STABLE_DIFFUSION_URL
+                        URL for an AUTOMATIC1111 Stable Diffusion server
+  --stable-diffusion-sampler STABLE_DIFFUSION_SAMPLER
+                        Sampler to use when generating images. If not specified, the one set on the
+                        AUTOMATIC1111 server will be used.
+  --stable-diffusion-negative-prompt STABLE_DIFFUSION_NEGATIVE_PROMPT
+                        Negative prompt to use when generating images. This will discourage Stable
+                        Diffusion from generating images with the specified content. By default,
+                        this is set to follow Discord's TOS.
+  --stable-diffusion-negative-prompt-nsfw STABLE_DIFFUSION_NEGATIVE_PROMPT_NSFW
+                        Negative prompt to use when generating images in a channel marked as'Age-
+                        Restricted'. By default, this follows the Discord TOS by allowing some
+                        sexual content forbidden in non-age-restricted channels.
 
-Also, to authenticate to Discord, you must set the environment variable: DISCORD_TOKEN = <your bot's
-discord token>
+Also, to authenticate to Discord, you must set the environment variable: DISCORD_TOKEN = <your
+bot's discord token>
 ```
 
 ## Required settings
 
 - **`DISCORD_TOKEN`** environment variable
 
    Set your shell environment's **`DISCORD_TOKEN`** to token Discord provided when you set up the bot account.  It should be something like a 72-character-long random-looking string.
@@ -159,18 +182,14 @@
 
    the name the AI will be instructed to call itself.  Note that this technically doesn't need to be the same as the bot in your discord, but it would likely make sense to your users if they are at least similar.
 
 - **`--wakewords`**
 
    one or more words that the bot will look for.  It will reply to any message which contains one of these words, in any channel.
 
-- **`--local-repl`**
-
-    instead of connecting to discord, just start up a local REPL and send these prompts directly to the oobabooga server.  Useful if you want to test if that part is working in isolation.  Note that in this mode you will be sending the oobabooga server raw input, and so the persona or AI name settings will be ignored.
-
 ## Persona: the fun setting
 
 - **`--persona`**
 
     is a short few sentences describing the role your bot should act as.  For instance, this is the setting I'm using for my cat-bot, whose name is "Rosie".
 
 ```console
@@ -194,14 +213,52 @@
 
 You should see something like this if everything worked:
 
 ![oobabot running!](./docs/oobabot-cli.png "textually interesting image")
 
 ---
 
+## Stable Diffusion via AUTOMATIC1111
+
+- **`--stable-diffusion-url`**
+
+  is the URL to a server running [AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui)
+
+  With it, users can ask **`oobabot`** to generate images and post the
+  results to the channel.  The user who made the original request can
+  choose to regenerate the image as they like.  If they either don't
+  find one they like, or don't do anything within 3 minutes, the image
+  will be removed.
+
+  ![oobabot running!](./docs/zombietaytay.png "textually interesting image")
+
+  Currently, detection of photo requests is very crude, and is only looking
+  for messages which match this regex:
+
+  ```python
+        photowords = ["drawing", "photo", "pic", "picture", "image", "sketch"]
+        self.photo_patterns = [
+            re.compile(
+                r"^.*\b" + photoword + r"\b[\s]*(of|with)?[\s]*[:]?(.*)$", re.IGNORECASE
+            )
+            for photoword in photowords
+        ]
+  ```
+
+  Note that depending on the checkpoint loaded in Stable Diffusion, it may not be appropriate
+  for your server's community.  I suggest reviewing [Discord's Terms of Service](https://discord.com/terms) and
+  [Community Guidelines](https://discord.com/guidelines) before deciding what checkpoint to run.
+
+  **`oobabot`** supports two different negative prompts, depending on whether the channel
+  is marked as "Age-Restricted" or not.  This is to allow for more explicit content in
+  channels which are marked as such.  While the negative prompt will discourage Stable
+  Diffusion from generating an image which matches the prompt, but is not foolproof.
+
+---
+
 ## Interacting with **`oobabot`**
 
 By default, **`oobabot`** will listen for three types of messages in the servers it's connected to:
 
  1. any message in which **`oobabot`**'s account is @-mentioned
  1. any direct message
  1. any message containing a provided wakeword (see Optional Settings)
@@ -209,11 +266,13 @@
 Also, the bot has a random chance of sending follow-up messages within the
 same channel if others reply within 120 seconds of its last post.  The exact
 parameters for this are in flux, but is meant to simulate a natural conversation
 flow, without forcing others to always post a wakeword.
 
 ## Known Issues
 
-- ooba's text generation can error with OOM when more than one request comes in at once.
+- detection of requests for photos is very crude, and will likely be improved in the future.
+- some of the default settings are very specific to my use case, and will likely be made
+  configurable in the future
 - sometimes the bot wants to continue conversations on behalf of other members of the chatroom.  I have some hacks in place to notice and truncate this behavior, but it can lead to terse responses on occasion.
-- found one not listed here?  [Create an issue](https://github.com/chrisrude/oobabot/issues) on github!
+- found one not listed here?  Have an idea?  [Create an issue](https://github.com/chrisrude/oobabot/issues) on github!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

