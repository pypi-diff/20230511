# Comparing `tmp/nonebot_plugin_spark_gpt-0.1.1.tar.gz` & `tmp/nonebot_plugin_spark_gpt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_spark_gpt-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_spark_gpt-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_spark_gpt-0.1.1.tar` & `nonebot_plugin_spark_gpt-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,41 @@
--rw-r--r--   0        0        0     1743 2023-05-09 13:58:29.200887 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/__init__.py
--rw-r--r--   0        0        0       14 2023-05-07 04:23:37.338492 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/__init__.py
--rw-r--r--   0        0        0     3919 2023-05-08 16:53:49.475522 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/chatgpt_web_func.py
--rw-r--r--   0        0        0     8227 2023-05-08 17:28:00.134982 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/config.py
--rw-r--r--   0        0        0    27202 2023-05-08 17:35:02.026220 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/main.py
--rw-r--r--   0        0        0     6129 2023-05-08 17:20:52.155727 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/web_api.py
--rw-r--r--   0        0        0       14 2023-05-07 04:37:03.529698 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/__init__.py
--rw-r--r--   0        0        0     2070 2023-05-07 16:21:14.595978 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/common_func.py
--rw-r--r--   0        0        0     6152 2023-05-08 15:02:15.181030 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/config.py
--rw-r--r--   0        0        0     4877 2023-05-09 05:04:52.272343 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/main.py
--rw-r--r--   0        0        0     3936 2023-05-09 11:11:17.903494 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/__pycache__/render.cpython-310.pyc
--rw-r--r--   0        0        0     4066 2023-05-09 11:11:11.036002 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/render.py
--rw-r--r--   0        0        0    18464 2023-05-09 08:51:42.987873 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/github-markdown-light.css
--rw-r--r--   0        0        0  1458204 2023-04-22 14:17:13.496635 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.b64_fonts.css
--rw-r--r--   0        0        0   270288 2023-04-22 14:17:13.497555 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.js
--rw-r--r--   0        0        0     1290 2023-04-22 14:17:13.498611 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/katex/mathtex-script-type.min.js
--rw-r--r--   0        0        0      670 2023-05-09 08:51:13.189256 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/markdown.html
--rw-r--r--   0        0        0     1253 2023-05-09 05:07:59.973080 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/markdown_.html
--rw-r--r--   0        0        0     4625 2023-05-09 09:23:49.857905 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/pygments-default.css
--rw-r--r--   0        0        0    86342 2023-04-22 05:34:37.774678 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/source/background.png
--rw-r--r--   0        0        0     1137 2023-04-22 05:34:37.774678 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/source/banner.png
--rw-r--r--   0        0        0    86342 2023-04-22 05:34:37.775678 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/source/mi_background.png
--rw-r--r--   0        0        0      125 2023-04-22 14:17:13.500554 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/text.css
--rw-r--r--   0        0        0      233 2023-04-22 14:17:13.500554 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/text.html
--rw-r--r--   0        0        0     4215 2023-05-08 15:55:10.287665 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/newbing/config.py
--rw-r--r--   0        0        0    18565 2023-05-08 16:56:38.171949 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/newbing/main.py
--rw-r--r--   0        0        0     3068 2023-05-08 16:16:37.378665 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/newbing/newbing_func.py
--rw-r--r--   0        0        0       16 2023-05-08 03:59:58.447201 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/__init__.py
--rw-r--r--   0        0        0     9719 2023-05-08 16:42:46.394179 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/config.py
--rw-r--r--   0        0        0    29776 2023-05-08 17:01:51.461667 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/main.py
--rw-r--r--   0        0        0    10706 2023-05-08 03:59:52.713874 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/poe_api.py
--rw-r--r--   0        0        0     7374 2023-05-08 03:59:50.889224 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/poe_func.py
--rw-r--r--   0        0        0     2147 2023-05-08 03:59:48.875662 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/pwframework.py
--rw-r--r--   0        0        0      897 2023-05-09 14:00:56.802173 nonebot_plugin_spark_gpt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2889 2023-05-09 14:04:08.408306 nonebot_plugin_spark_gpt-0.1.1/README.md
--rw-r--r--   0        0        0     3983 1970-01-01 00:00:00.000000 nonebot_plugin_spark_gpt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1894 2023-05-11 03:29:22.094362 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/__init__.py
+-rw-r--r--   0        0        0       16 2023-05-10 17:23:53.939876 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/__init__.py
+-rw-r--r--   0        0        0     3919 2023-05-08 16:53:49.475522 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/chatgpt_web_func.py
+-rw-r--r--   0        0        0     8228 2023-05-10 17:23:58.319737 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/config.py
+-rw-r--r--   0        0        0    28144 2023-05-10 17:24:00.050884 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/main.py
+-rw-r--r--   0        0        0     6131 2023-05-10 17:24:01.276809 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/web_api.py
+-rw-r--r--   0        0        0       16 2023-05-10 17:24:06.325142 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/claude_slack/__init__.py
+-rw-r--r--   0        0        0     3036 2023-05-10 17:24:07.826903 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/claude_slack/claude_func.py
+-rw-r--r--   0        0        0     8094 2023-05-10 17:24:09.084792 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/claude_slack/config.py
+-rw-r--r--   0        0        0    25921 2023-05-10 17:24:10.744126 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/claude_slack/main.py
+-rw-r--r--   0        0        0     4309 2023-05-10 17:24:12.141727 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/claude_slack/slack_api.py
+-rw-r--r--   0        0        0       16 2023-05-10 17:24:16.477844 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/__init__.py
+-rw-r--r--   0        0        0     2633 2023-05-10 17:24:17.515144 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/common_func.py
+-rw-r--r--   0        0        0     6158 2023-05-10 16:32:44.366675 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/config.py
+-rw-r--r--   0        0        0     5563 2023-05-11 03:26:38.959437 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/main.py
+-rw-r--r--   0        0        0     3936 2023-05-09 11:11:17.903494 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/__pycache__/render.cpython-310.pyc
+-rw-r--r--   0        0        0     4066 2023-05-09 11:11:11.036002 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/render.py
+-rw-r--r--   0        0        0    18464 2023-05-09 08:51:42.987873 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/github-markdown-light.css
+-rw-r--r--   0        0        0  1458204 2023-04-22 14:17:13.496635 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.b64_fonts.css
+-rw-r--r--   0        0        0   270288 2023-04-22 14:17:13.497555 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.js
+-rw-r--r--   0        0        0     1290 2023-04-22 14:17:13.498611 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/katex/mathtex-script-type.min.js
+-rw-r--r--   0        0        0      670 2023-05-09 08:51:13.189256 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/markdown.html
+-rw-r--r--   0        0        0     1253 2023-05-09 05:07:59.973080 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/markdown_.html
+-rw-r--r--   0        0        0     4625 2023-05-09 09:23:49.857905 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/pygments-default.css
+-rw-r--r--   0        0        0    86342 2023-04-22 05:34:37.774678 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/source/background.png
+-rw-r--r--   0        0        0     1137 2023-04-22 05:34:37.774678 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/source/banner.png
+-rw-r--r--   0        0        0    86342 2023-04-22 05:34:37.775678 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/source/mi_background.png
+-rw-r--r--   0        0        0      125 2023-04-22 14:17:13.500554 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/text.css
+-rw-r--r--   0        0        0      233 2023-04-22 14:17:13.500554 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/text.html
+-rw-r--r--   0        0        0     4244 2023-05-10 17:24:24.469959 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/newbing/config.py
+-rw-r--r--   0        0        0    18363 2023-05-10 17:24:26.071103 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/newbing/main.py
+-rw-r--r--   0        0        0     3068 2023-05-08 16:16:37.378665 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/newbing/newbing_func.py
+-rw-r--r--   0        0        0       16 2023-05-08 03:59:58.447201 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/__init__.py
+-rw-r--r--   0        0        0     9719 2023-05-10 14:13:15.440356 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/config.py
+-rw-r--r--   0        0        0    29872 2023-05-10 16:30:34.806983 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/main.py
+-rw-r--r--   0        0        0    10706 2023-05-08 03:59:52.713874 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/poe_api.py
+-rw-r--r--   0        0        0     6332 2023-05-10 17:24:38.505890 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/poe_func.py
+-rw-r--r--   0        0        0     2147 2023-05-08 03:59:48.875662 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/pwframework.py
+-rw-r--r--   0        0        0      920 2023-05-11 03:29:11.350702 nonebot_plugin_spark_gpt-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3042 2023-05-11 03:31:13.216645 nonebot_plugin_spark_gpt-0.1.2/README.md
+-rw-r--r--   0        0        0     4173 1970-01-01 00:00:00.000000 nonebot_plugin_spark_gpt-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/__init__.py` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import nonebot
 
 from .poe import main
 from .newbing import main
 from .chatgpt_web import main
 from .common import main
+from .claude_slack import main
 from nonebot.matcher import Matcher
 from nonebot.plugin import PluginMetadata
 from nonebot.adapters.onebot.v11 import (
     Event,
     Bot,
     MessageSegment,
 )
 
 from .common.render.render import md_to_pic
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __plugin_meta__ = PluginMetadata(
     "Spark-GPT",
     "将多来源的gpt接入qq及更多平台，使用便捷，管理完善，功能强大",
     "通过/help /帮助 /说明 /使用说明  命令来获取详细使用说明",
     {"Author": "canxin121"},
 )
 
@@ -50,14 +51,20 @@
 
 ## GPT_Web帮助命令
 
 | 命令 | 描述 |
 | --- | --- |
 | `/gwhelp / gwh` | 获取GPT_Web帮助说明。 |
 
+## Claude_Slack帮助命令
+
+| 命令 | 描述 |
+| --- | --- |
+| `/chelp / ch` | 获取GPT_Web帮助说明。 |
+
 # 通用命令
 
 - 所有用户均可使用
 
 | 命令 | 描述 |
 | --- | --- |
 | `/botlist / bl` | 获取你的所有机器人的列表。 |
```

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/chatgpt_web_func.py` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/chatgpt_web_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/config.py` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     session_token: str = ""
     pic_able: str = None
     url_able: str = "True"
     num_limit: int = 350
     model: str = "text-davinci-002-render-sha"
     mode: str = "black"
     api_url: str = "https://chat.loli.vet/"
-    proxy:str = None
+    proxy: str = None
     cookie_dict: dict = {}
     superusers = []
     blacklist = []
     whitelist = []
     # user_dict: Dict[UserInfo, Dict["all" or "now", Dict[nickname, BotInfo]]] = {}
     user_dict: Dict[UserInfo, Dict[str, Dict[str, BotInfo]]] = {}
     auto_prompt: str = "默认"
```

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/main.py` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 from .config import (
     BotInfo,
     GPT_webTemper,
     gptweb_persistor,
     get_user_info_and_data,
     set_userdata,
 )
-from .chatgpt_web_func import reply_out, delete_messages, sendmsg
+from .chatgpt_web_func import sendmsg
 from .web_api import gptweb_api
 from ..common.config import spark_persistor
+from ..common.common_func import delete_messages, reply_out
 from ..poe.config import poe_persistor
-from nonebot.rule import fullmatch
 from nonebot import logger
 
 # 初始化两个需要使用的实例
 temp_data = GPT_webTemper()
 user_data_dict = temp_data.user_data_dict
 msg_bot_bidict = temp_data.msg_bot_bidict
 prompts_dict = spark_persistor.prompts_dict
@@ -64,15 +64,15 @@
     event: Event,
     state: T_State,
     infos: str = ArgStr("model"),
 ):
     global gptweb_persistor
     create_msgs = state["create_msgs"]
     user_id = str(event.user_id)
-    infos = infos.split(" ", 2)
+    infos = infos.split(" ", 1)
     if infos[0] in ["取消", "算了"]:
         create_msgs.append(await matcher.send(reply_out(event, "取消创建")))
         await delete_messages(bot, str(event.user_id), create_msgs)
         await matcher.finish()
     if len(infos) != 2:
         create_msgs.append(await matcher.reject(reply_out(event, "你输入的信息有误，请重新输入")))
 
@@ -108,20 +108,24 @@
             await matcher.send(reply_out(event, "已经有同名的bot了，换一个名字重新输入吧"))
         )
         await matcher.reject()
     if creat_lock.locked():
         waitmsg = await matcher.send(reply_out(event, "有人正在创建中，稍后自动为你创建"))
     async with creat_lock:
         try:
+            current_userdata.is_waiting = True
             result = await gptweb_api.gpt_web_chat(truename, parentname, prompt)
+            current_userdata.is_waiting = False
         except:
+            current_userdata.is_waiting = False
             await matcher.send(reply_out(event, "出错了，多次出错请尝试换一个预设，还不行请联系机器人主人"))
             await delete_messages(bot, user_id, create_msgs)
         if isinstance(result, str):
             text_error = result
+            current_userdata.is_waiting = False
             await matcher.finish(reply_out(event, text_error))
         elif isinstance(result, tuple):
             answer, parentname, truename = result
             # 将更新后的字典写回到JSON文件中
             botinfo = BotInfo(
                 nickname=nickname,
                 truename=truename,
@@ -144,19 +148,21 @@
                 pass
             reply_msgid = await matcher.send(
                 reply_out(event, f"创建成功并切换到新建bot\n\n创建自动回复:{answer}")
             )
             msg_bot_bidict[reply_msgid["message_id"]] = botinfo
             current_userdata.last_reply_message_id[nickname] = reply_msgid["message_id"]
             await delete_messages(bot, user_id, create_msgs)
+            current_userdata.is_waiting = False
             await matcher.finish()
         else:
             await matcher.send(reply_out(event, "出错了，多次出错请联系机器人管理员"))
 
             await delete_messages(bot, user_id, create_msgs)
+            current_userdata.is_waiting = False
             await matcher.finish()
 
 
 #############################################################
 gptweb_switch = on_command("gwswitch", aliases={"gws"}, priority=4, block=False)
 
 
@@ -300,17 +306,15 @@
                     if str(event.message).startswith("/" + name)
                 ),
                 None,
             )
             if nickname:
                 if not is_useable(event):
                     return False
-                botinfo = gptweb_persistor.user_dict[current_userinfo]["all"][
-                    nickname
-                ]
+                botinfo = gptweb_persistor.user_dict[current_userinfo]["all"][nickname]
                 raw_message = (
                     str(event.message)
                     .replace("/" + nickname + " ", "")
                     .replace("/" + nickname, "")
                 )
                 if not raw_message:
                     return False
@@ -327,53 +331,58 @@
                 )
             else:
                 return False
         except:
             return False
 
 
-
 #############################################################
 chat_lock = asyncio.Semaphore(3)
 
 gw_chat_ = on_message(priority=1, block=False)
 
 
 @gw_chat_.handle()
 async def __chat_bot__(matcher: Matcher, event: MessageEvent, bot: Bot):
     temp = await _is_chat_(event, bot)
     if temp == False:
         await matcher.finish()
     if temp == "none":
+        current_userinfo, current_userdata = set_userdata(event, user_data_dict)
+        if current_userdata.is_waiting:
+            await matcher.finish(reply_out(event, "你已经有一个请求进行中了，请等结束后再发送"))
         nickname = "gwdefault"
         truename = None
         parentname = str(random_uuid4())
         prompt_nickname = gptweb_persistor.auto_prompt
         prompt = prompts_dict[prompt_nickname]
         raw_message = (
             str(event.message)
             .replace("/gwtalk ", "")
             .replace("/gwtalk", "")
             .replace("/gwt ", "")
             .replace("/gwt", "")
         )
         lastmsg_id = 0
-        current_userinfo, current_userdata = set_userdata(event, user_data_dict)
         if current_userinfo not in list(gptweb_persistor.user_dict.keys()):
             gptweb_persistor.user_dict.setdefault(
                 current_userinfo, {"all": {}, "now": {}}
             )
 
         if creat_lock.locked():
             waitmsg = await matcher.send(reply_out(event, "有人正在创建中，稍后自动为你创建"))
         async with creat_lock:
             try:
+                current_userdata.is_waiting = True
                 result = await gptweb_api.gpt_web_chat(truename, parentname, prompt)
+                current_userdata.is_waiting = False
             except:
+                current_userdata.is_waiting = False
                 await matcher.finish(reply_out(event, "出错了，多次出错请联系机器人管理员"))
+
             if isinstance(result, str):
                 text_error = result
             elif isinstance(result, tuple):
                 answer, parentname, truename = result
                 # 将更新后的字典写回到JSON文件中
                 botinfo = BotInfo(
                     nickname=nickname,
@@ -395,14 +404,15 @@
                     await bot.delete_msg(message_id=waitmsg["message_id"])
                 except:
                     pass
                 await matcher.send(
                     reply_out(event, f"自动创建成功并切换到新建bot:gwdefault\n自动创建回复:\n{answer}")
                 )
             else:
+                current_userdata.is_waiting = False
                 await matcher.finish(reply_out(event, "出错了，多次出错请联系机器人管理员"))
     else:
         lastmsg_id, raw_message, botinfo, current_userinfo, current_userdata = temp
     nickname = botinfo.nickname
     truename = botinfo.truename
     parentname = botinfo.parentname
     if current_userdata.is_waiting:
@@ -415,16 +425,14 @@
             "清除对话",
             "清空对话",
             "清除历史",
             "清空历史",
             "清除记录",
             "清空历史对话",
             "刷新对话",
-            "pd",
-            "gwdump",
         ]:
             truename = None
             parentname = str(random_uuid4())
             prompt_nickname = gptweb_persistor.auto_prompt
             prompt = prompts_dict[prompt_nickname]
 
             if current_userinfo not in list(gptweb_persistor.user_dict.keys()):
@@ -451,15 +459,20 @@
                         prompt_nickname=prompt_nickname,
                         prompt=prompt,
                         owner="qq-" + str(event.user_id),
                     )
                     gptweb_persistor.user_dict[current_userinfo]["all"][
                         nickname
                     ] = botinfo
-                    if botinfo.nickname == list(gptweb_persistor.user_dict[current_userinfo]["now"].values())[0].nickname:
+                    if (
+                        botinfo.nickname
+                        == list(
+                            gptweb_persistor.user_dict[current_userinfo]["now"].values()
+                        )[0].nickname
+                    ):
                         gptweb_persistor.user_dict[current_userinfo]["now"] = {
                             nickname: botinfo
                         }
                     gptweb_persistor.save()
                     msg_bot_bidict[lastmsg_id] = botinfo
                     try:
                         await bot.delete_msg(message_id=waitmsg["message_id"])
@@ -467,54 +480,60 @@
                         pass
                     reply_msgid = await matcher.send(
                         reply_out(event, f"刷新对话成功\n刷新回复:\n{answer}")
                     )
                     current_userdata.last_reply_message_id[nickname] = reply_msgid[
                         "message_id"
                     ]
-                    msg_bot_bidict.inv[botinfo] = reply_msgid[
-                        "message_id"
-                    ]
+                    msg_bot_bidict.inv[botinfo] = reply_msgid["message_id"]
+                    current_userdata.is_waiting = False
                     await matcher.finish()
                 else:
+                    current_userdata.is_waiting = False
                     await matcher.finish(reply_out(event, "出错了，多次出错请联系机器人管理员"))
         else:
             current_userdata.is_waiting = True
             try:
                 result = await gptweb_api.gpt_web_chat(
                     truename, parentname, raw_message
                 )
+                current_userdata.is_waiting = False
             except:
                 current_userdata.is_waiting = False
                 await matcher.finish(reply_out(event, "出错了，多次出错请联系机器人主人"))
-            current_userdata.is_waiting = False
             if isinstance(result, str):
                 text_error = result
                 logger.warning(text_error)
                 await matcher.send(reply_out(event, text_error))
             elif isinstance(result, tuple):
                 answer, parentname, truename = result
                 botinfo.truename = truename
                 botinfo.parentname = parentname
 
                 msg_bot_bidict[lastmsg_id] = botinfo
 
                 gptweb_persistor.user_dict[current_userinfo]["all"][nickname] = botinfo
-                if botinfo in gptweb_persistor.user_dict[current_userinfo]["now"]:
-                    gptweb_persistor.user_dict[current_userinfo]["now"] = { 
+                if (
+                    botinfo
+                    == list(
+                        gptweb_persistor.user_dict[current_userinfo]["now"].values()
+                    )[0]
+                ):
+                    gptweb_persistor.user_dict[current_userinfo]["now"] = {
                         nickname: botinfo
                     }
                 gptweb_persistor.save()
 
                 reply_msgid = await sendmsg(answer, matcher, event)
                 current_userdata.last_reply_message_id[nickname] = reply_msgid[
                     "message_id"
                 ]
 
                 msg_bot_bidict.inv[botinfo] = reply_msgid["message_id"]
+                current_userdata.is_waiting = False
                 await matcher.finish()
 
 
 # ######################################################
 gptweb_remove = on_command("gwremove", aliases={"gwr"}, priority=4, block=False)
 
 
@@ -601,15 +620,15 @@
 ######################################################
 gw_auto_change_prompt = on_command(
     "gwchangeprompt", aliases={"gwcp"}, priority=4, block=False
 )
 
 
 @gw_auto_change_prompt.handle()
-async def __poe_auto_change_prompt__(matcher:Matcher,event: Event):
+async def __poe_auto_change_prompt__(matcher: Matcher, event: Event):
     if not is_useable(event):
         await matcher.finish()
     global gptweb_persistor
     user_id = str(event.user_id)
     if user_id not in gptweb_persistor.superusers:
         await gw_auto_change_prompt.finish("你不是管理员哦")
     now_prompt = gptweb_persistor.auto_prompt
@@ -648,15 +667,15 @@
     if not is_useable(event):
         await matcher.finish()
     msg = """
 # spark-gpt GPT_web使用说明
 
 - !!! 以下命令前面全部要加 '/' !!!  
 
-- 问答功能均支持以下特性：可以通过回复机器人的最后一个回答来继续对话，而无需命令；可以回复 "(清除/清空)(对话/历史)"或 刷新对话，清除对话历史 或 "pd","poedump","pdump"来清空对话；可以通过建议回复的数字索引来使用建议回复。
+- 问答功能均支持以下特性：可以通过回复机器人的最后一个回答来继续对话，而无需命令；可以回复 "(清除/清空)(对话/历史)"或 "刷新对话" 或 "清除对话历史"来清空对话；可以通过建议回复的数字索引来使用建议回复。
 
 ## 对话命令
 
 | 命令 | 描述 |
 | --- | --- |
 | `/gwtalk / gwt + 你要询问的内容` | 对话功能，如果没创建机器人，对话将自动创建默认机器人。 |
```

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/web_api.py` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/web_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,8 +126,9 @@
                 )
                 self.authorization = response.json()["accessToken"]
             except Exception as e:
                 logger.opt(colors=True, exception=e).error(
                     f"刷新会话失败: <r>HTTP{response.status_code}</r> {response.text}"
                 )
 
+
 gptweb_api = ChatGPT_web()
```

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/common_func.py` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/common_func.py`

 * *Files 23% similar despite different names*

```diff
@@ -27,14 +27,29 @@
     if type(content) == bytes:
         return MessageSegment.reply(event.message_id) + MessageSegment.image(content)
     if content[0:9] == "base64://":
         return MessageSegment.reply(event.message_id) + MessageSegment.image(content)
     return MessageSegment.reply(event.message_id) + content
 
 
+async def delete_messages(bot, user_id: str, dict_list: dict):
+    await asyncio.sleep(1)
+    if user_id in dict_list:
+        if isinstance(dict_list[user_id], list):
+            for eachmsg in dict_list[user_id]:
+                await bot.delete_msg(message_id=eachmsg["message_id"])
+            del dict_list[user_id]
+        else:
+            await bot.delete_msg(message_id=dict_list[user_id]["message_id"])
+    else:
+        for eachmsg in dict_list:
+            await bot.delete_msg(message_id=eachmsg["message_id"])
+        del dict_list
+
+
 async def get_url(text):
     """将 Markdown 文本保存到 Mozilla Pastebin，并获得 URL"""
     async with aiohttp.ClientSession() as session:
         payload = {
             "expires": "86400",
             "format": "url",
             "lexer": "_markdown",
```

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/config.py` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     num_limit: int = 350
     superusers: List[str] = []
     blacklist: List[str] = []
     whitelist: List[str] = []
     mode: str = "black"
     prompts_dict: Dict[str, str] = {
         "猫娘": "现在你将模仿一只猫娘，与我对话每一句话后面都要加上“喵”，如果你能明白我的意思，请回复“喵~你好主人”",
-        "默认": "一个ai语言模型",
+        "默认": "你是一个ai语言模型",
     }
 
     def __init__(self, **data):
         super().__init__(**data)
         try:
             saved_data = self.load()
             self.__dict__.update(saved_data)
```

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/main.py` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from nonebot.plugin import on_command
 from nonebot.params import ArgStr
 from nonebot.typing import T_State
 from nonebot.matcher import Matcher
-from nonebot.adapters.onebot.v11 import Event,Message
+from nonebot.adapters.onebot.v11 import Event, Message,MessageSegment
 from nonebot.params import ArgStr, CommandArg
 from .render.render import md_to_pic
 from .common_func import reply_out
 from .config import spark_persistor, get_user_info_and_data
 from .common_func import is_auto_prompt
 from ..chatgpt_web.config import gptweb_persistor
 from ..poe.config import poe_persistor
+from ..claude_slack.config import claude_slack_persistor
 
 spark_addprompt = on_command("添加预设", aliases={"ap"}, priority=4, block=False)
 
 
 @spark_addprompt.handle()
 async def __spark_addprompt__(matcher: Matcher, event: Event):
     global spark_persistor
@@ -38,17 +39,16 @@
 @spark_addprompt.got("prompt", prompt="请输入预设\n输入取消 或 算了可以终止创建")
 async def __spark_addprompt____(
     event: Event, state: T_State, infos: str = ArgStr("prompt")
 ):
     global spark_persistor
     if infos in ["取消", "算了"]:
         await spark_addprompt.finish("终止添加")
-    infos = infos.split(" ")
     name = state["key"]
-    prompt = infos[0]
+    prompt = infos
     # # 将更新后的字典写回到JSON文件中
     spark_persistor.prompts_dict[name] = prompt
     spark_persistor.save()
     await spark_addprompt.finish("成功添加prompt")
 
 
 ######################################################
@@ -63,15 +63,20 @@
         await spark_removeprompt.finish("你不是管理员哦")
     else:
         str_prompts = str()
         i = 1
         for key, value in spark_persistor.prompts_dict.items():
             str_prompts += f"************************\n{i}:预设名称：{key}\n预设内容：{value}\n"
             i += 1
-        await spark_removeprompt.send(f"当前预设有：\n{str_prompts}")
+        if len(str_prompts)>600:
+            pic = await md_to_pic(f"当前预设有：\n{str_prompts}")
+            pic = MessageSegment.image(pic)
+            await spark_removeprompt.send(pic)
+        else:
+            await spark_removeprompt.send(f"当前预设有：\n{str_prompts}")
 
 
 @spark_removeprompt.got("name", prompt="请输入要删除的预设名称\n输入取消 或 算了可以终止创建")
 async def __spark_removeprompt____(event: Event, infos: str = ArgStr("name")):
     if infos in ["取消", "算了"]:
         await spark_removeprompt.finish("终止删除")
     infos = infos.split(" ")
@@ -99,22 +104,31 @@
     try:
         gw_bots = list(gptweb_persistor.user_dict[current_userinfo]["all"].keys())
         gw_bot_str = "gpt_web机器人有:\n"
         for i in range(len(gw_bots)):
             gw_bot_str += f"    {i+1}:{gw_bots[i]}\n"
     except:
         gw_bot_str = "没有可用的gpt_web机器人\n"
-    poe_bots = list(poe_persistor.user_dict[current_userinfo]["all"].keys())
     try:
+        poe_bots = list(poe_persistor.user_dict[current_userinfo]["all"].keys())
         poe_bot_str = "poe机器人有:\n"
         for i in range(len(poe_bots)):
             poe_bot_str += f"    {i+1}:{poe_bots[i]}\n"
     except:
         poe_bot_str = "没有可用的poe机器人\n"
-    msg = "所有机器人信息如下:\n\n" + gw_bot_str + poe_bot_str
+    try:
+        claude_slack_bots = list(
+            claude_slack_persistor.user_dict[current_userinfo]["all"].keys()
+        )
+        claude_slack_bot_str = "claude_slack机器人有:\n"
+        for i in range(len(claude_slack_bots)):
+            claude_slack_bot_str += f"    {i+1}:{claude_slack_bots[i]}\n"
+    except:
+        claude_slack_bot_str = "没有可用的poe机器人\n"
+    msg = "所有机器人信息如下:\n\n" + gw_bot_str + poe_bot_str + claude_slack_bot_str
     await matcher.finish(reply_out(event, msg))
 
 
 test = on_command("md2pic", priority=4, block=False)
 
 
 @test.handle()
@@ -122,8 +136,8 @@
     matcher: Matcher,
     event: Event,
     state: T_State,
     args: Message = CommandArg(),
 ):
     text = str(args[0])
     pic = await md_to_pic(text)
-    await matcher.finish(reply_out(event, pic))
+    await matcher.finish(reply_out(event, pic))
```

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/__pycache__/render.cpython-310.pyc` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/__pycache__/render.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/render.py` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/render.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/github-markdown-light.css` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.b64_fonts.css` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.b64_fonts.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.js` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/katex/mathtex-script-type.min.js` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/katex/mathtex-script-type.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/markdown.html` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/markdown.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/markdown_.html` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/markdown_.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/pygments-default.css` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/pygments-default.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/source/background.png` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/source/background.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/source/banner.png` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/source/banner.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/source/mi_background.png` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/source/mi_background.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/newbing/config.py` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/newbing/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Dict, List, Optional
 import nonebot
 from nonebot.adapters.onebot.v11 import MessageEvent
 from pathlib import Path
-from pydantic import BaseModel,Extra
+from pydantic import BaseModel, Extra
 from EdgeGPT import Chatbot
 from ..common.config import spark_persistor
 
+
 class UserInfo(BaseModel):
     platform: str
     user_id: int
 
     def to_dict(self) -> dict:
         return self.dict()
 
@@ -121,11 +122,14 @@
         )
         self.proxy = getattr(get_config, "newbing_proxy", self.proxy)
         self.pic_able = getattr(get_config, "newbing_picable", spark_persistor.pic_able)
         self.url_able = getattr(get_config, "newbing_urlable", spark_persistor.url_able)
         self.suggest_able = getattr(
             get_config, "newbing_suggestable", spark_persistor.suggest_able
         )
-        self.num_limit = int(getattr(get_config, "newbing_limit", spark_persistor.num_limit))
+        self.num_limit = int(
+            getattr(get_config, "newbing_limit", spark_persistor.num_limit)
+        )
+
 
 # 这里的配置即使在多平台，也应只初始化一次
 newbing_persistor = NerBingPersistor()
```

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/newbing/main.py` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/newbing/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,20 @@
     Message,
     Event,
     Bot,
     MessageEvent,
     MessageSegment,
 )
 from ImageGen import ImageGenAsync
-from .newbing_func import is_useable, reply_out, sendmsg
+from .newbing_func import is_useable, sendmsg
 from .config import newbing_persistor, NewBingTemper, set_userdata
 from EdgeGPT import Chatbot, ConversationStyle
 from ..common.render.render import md_to_pic
+from ..common.common_func import reply_out
+
 
 logger.info("开始加载Newbing")
 newbingtemper = NewBingTemper()
 user_data_dict = newbingtemper.user_data_dict
 
 
 #############################################################
@@ -140,56 +142,52 @@
     chatmode = current_userdata.chatmode
     if chatmode == "1":
         style = ConversationStyle.creative
     elif chatmode == "2":
         style = ConversationStyle.balanced
     else:
         style = ConversationStyle.precise
-    current_userdata.is_waiting = True
+
     try:
+        current_userdata.is_waiting = True
         raw_json = await chatbot.ask(
             prompt=raw_message,
             conversation_style=style,
             wss_link="wss://sydney.bing.com/sydney/ChatHub",
         )
+        current_userdata.is_waiting = False
     except:
         current_userdata.is_waiting = False
         await matcher.send(reply_out(event, "出错喽，多次重试都出错的话，联系机器人主人"))
         await matcher.finish()
     value = raw_json["item"]["result"]["value"]
     if value != "Success":
         if value == "Throttled":
-            current_userdata.is_waiting = False
             await matcher.finish(reply_out(event, "该账号cookie问答次数已达到今日上限捏"))
         elif value == "InvalidSession":
-            current_userdata.is_waiting = False
             await matcher.finish(reply_out(event, "无效会话捏"))
         else:
-            current_userdata.is_waiting = False
             await matcher.finish(reply_out(event, "出错喽，多次重试都出错的话，联系机器人主人"))
     try:
         is_offense = raw_json["item"]["messages"][0]["offense"]
 
         if is_offense == "Offensive":
-            current_userdata.is_waiting = False
             await matcher.finish(reply_out(event, "你的询问太冒犯了,newbing拒绝回答"))
         if "hiddenText" in raw_json["item"]["messages"][1]:
-            current_userdata.is_waiting = False
             await matcher.finish(reply_out(event, "你的询问太敏感了,newbing拒绝回答"))
     except:
         pass
 
     try:
         max_num = raw_json["item"]["throttling"]["maxNumUserMessagesInConversation"]
         now_num = raw_json["item"]["throttling"]["numUserMessagesInConversation"]
         reply = raw_json["item"]["messages"][1]["text"]
         reply = re.sub(r"\[\^(\d+)\^\]", r"[\1]", reply)
         reply = re.sub(r"\[?\^(\d+)\^\]?", r"[\1]", reply)
     except:
-        current_userdata.is_waiting = False
         await matcher.finish(reply_out(event, "出错喽，多次重试都出错的话，联系机器人主人"))
     msg_text = MessageSegment.text(reply + "  \n")
     if newbing_persistor.suggest_able == "True":
         try:
             suggests = [
                 raw_json["item"]["messages"][1]["suggestedResponses"][i]["text"]
                 for i in range(
@@ -287,14 +285,15 @@
     await matcher.finish()
 
 
 newbing_change_mode = on_command(
     "bc", aliases={"bingchange", "bing切换"}, priority=1, block=False
 )
 
+
 @newbing_change_mode.handle()
 async def __newbing_change_mode__(
     matcher: Matcher,
     state: T_State,
     event: MessageEvent,
     bot: Bot,
     args: Message = CommandArg(),
```

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/newbing/newbing_func.py` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/newbing/newbing_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/config.py` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/main.py` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,21 @@
     PoeTemper,
     poe_persistor,
     get_user_info_and_data,
     set_userdata,
 )
 from .poe_func import (
     generate_truename,
-    reply_out,
-    delete_messages,
     is_useable,
     send_msg,
     close_page,
     is_vip,
 )
 from .poe_api import poe_chat, poe_create, poe_clear
+from ..common.common_func import delete_messages, reply_out
 from ..common.config import spark_persistor
 from ..common.render.render import md_to_pic
 from ..chatgpt_web.config import gptweb_persistor
 from .pwframework import pwfw
 from nonebot import logger
 
 # 初始化两个需要使用的实例
@@ -115,15 +114,15 @@
     create_msgs = state["create_msgs"]
     user_id = str(event.user_id)
     if infos in ["取消", "算了"]:
         create_msgs.append(await matcher.send(reply_out(event, "取消创建")))
         await delete_messages(bot, str(event.user_id), create_msgs)
         await poe_create_.finish()
 
-    infos = infos.split(" ", 2)
+    infos = infos.split(" ", 1)
     if not (len(infos) == 3 and infos[1] in ["1", "2"]):
         create_msgs.append(await matcher.send(reply_out(event, "输入信息有误，请检查后重新输入")))
         await poe_create_.reject()
 
     # 获取创建所需信息
 
     nickname = str(infos[0])
@@ -390,17 +389,15 @@
                 if botinfo in list(base_botinfo_dict.values()):
                     mode = "public"
                 elif botinfo.nickname in current_userdata.last_reply_message_id:
                     mode = "private"
                 else:
                     return False
                 try:
-                    last_suggests = msg_bot_bidict[
-                        event.reply.message_id
-                    ].last_suggests
+                    last_suggests = msg_bot_bidict[event.reply.message_id].last_suggests
                 except:
                     last_suggests = []
                     #  mode,raw_message,last_msgid,last_suggests,nickname,truename,current_userinfo,current_userdata = temp
                 return (
                     mode,
                     raw_message,
                     event.reply.message_id,
@@ -424,17 +421,15 @@
             .replace("/pt ", "")
             .replace("/pt", "")
         )
         if not raw_message:
             return False
         mode = "private"
         try:
-            botinfo = list(
-                poe_persistor.user_dict[current_userinfo]["now"].values()
-            )[0]
+            botinfo = list(poe_persistor.user_dict[current_userinfo]["now"].values())[0]
             nickname = botinfo.nickname
             truename = botinfo.truename
         except:
             return "none"
         try:
             last_msgid = current_userdata.last_reply_message_id[nickname]
             last_suggests = msg_bot_bidict[last_msgid].last_suggests
@@ -515,17 +510,15 @@
                     )
                     if nickname in ["psg4", "psc+"] and not is_vip(event):
                         return False
                     if not raw_message:
                         return False
                     mode = "public"
                     try:
-                        last_msgid = current_userdata.last_reply_message_id[
-                            nickname
-                        ]
+                        last_msgid = current_userdata.last_reply_message_id[nickname]
                         last_suggests = msg_bot_bidict[last_msgid].last_suggests
                     except:
                         last_msgid = 0
                         last_suggests = []
                     return (
                         mode,
                         raw_message,
@@ -537,46 +530,51 @@
                         current_userdata,
                     )
                 else:
                     return False
         except:
             return False
 
+
 #############################################################
 chat_lock = asyncio.Semaphore(3)
 poe_base_lock = asyncio.Lock()
 poe_chat_ = on_message(priority=1, block=False)
 
 
 @poe_chat_.handle()
 async def __chat_bot__(matcher: Matcher, event: MessageEvent, bot: Bot):
     temp = await _is_chat_(event, bot)
     if temp == False:
         await matcher.finish()
     if temp == "none":
+        current_userinfo, current_userdata = set_userdata(
+            event=event, user_data_dict=user_data_dict
+        )
+        if current_userdata.is_waiting:
+            await matcher.finish(reply_out(event, "你已经有一个请求进行中了，请等结束后再发送"))
         mode = "private"
         user_id = str(event.user_id)
         raw_message = (
             str(event.message)
             .replace("/pchat ", "")
             .replace("/pchat", "")
             .replace("/pt ", "")
             .replace("/pt", "")
         )
         last_suggests = []
         nickname = "pdefault"
         truename = str(generate_truename(user_id, nickname))
         prompt_nickname = poe_persistor.auto_prompt
         prompt = spark_persistor.prompts_dict[prompt_nickname]
+        current_userdata.is_waiting = True
         page = await pwfw.new_page()
         is_created = await poe_create(page, truename, 1, prompt)
         await page.close()
-        current_userinfo, current_userdata = set_userdata(
-            event=event, user_data_dict=user_data_dict
-        )
+        current_userdata.is_waiting = False
         if is_created:
             # # 将更新后的字典写回到JSON文件中
             botinfo = BotInfo(
                 nickname=nickname,
                 truename=truename,
                 source="poe",
                 model="gpt3.5",
@@ -619,15 +617,15 @@
     if mode == "private":
         if current_userdata.is_waiting:
             await matcher.finish(reply_out(event, "你已经有一个对话进行中了，请等结束后再发送"))
         if chat_lock.locked():
             await matcher.send(reply_out(event, "请稍等,你前面已有3个用户,你的回答稍后就来"))
 
         async with chat_lock:
-            if text in ["清除对话", "清空对话", "清除历史", "清空历史", "清除记录", "清空历史对话", "刷新对话"]:
+            if text in ["清除对话", "清空对话", "清除历史", "清空历史", "清空历史对话", "刷新对话"]:
                 current_userdata.is_waiting = True
                 page = await pwfw.new_page()
                 is_cleared = await poe_clear(page=page, truename=truename)
                 await page.close()
                 if is_cleared:
                     msg = f"成功清除了{nickname}的历史消息"
                 else:
@@ -706,15 +704,15 @@
 - 共享的机器人供多人共同使用，而用户隔离的机器人每个人都是相互独立的。
 
 - 以下命令前面全部要加 '/' ！！！！！
 
 - 对话问答功能均支持以下特性：
 
 - 可以通过回复机器人的最后一个回答来继续对话，而无需命令。
-- 可以回复 "(清除/清空)(对话/历史)" 或 刷新对话, 清除对话历史 或 "pd", "poedump", "pdump" 来清空对话。
+- 可以回复 "(清除/清空)(对话/历史)" 或"刷新对话"或"清除对话历史"来清空对话。
 - 可以通过建议回复的数字索引来使用建议回复。
 
 ************************
 
 - 以下命令均支持用户隔离
 
 | 命令 | 描述 |
```

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/poe_api.py` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/poe_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/poe_func.py` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/poe_func.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,43 +50,14 @@
 
 
 def is_email(email) -> bool:
     pattern = r"^[\w\.-]+@[\w\.-]+\.[a-zA-Z]{2,}$"
     return bool(re.match(pattern, email))
 
 
-async def delete_messages(bot, user_id: str, dict_list: dict):
-    await asyncio.sleep(1)
-    if user_id in dict_list:
-        if isinstance(dict_list[user_id], list):
-            for eachmsg in dict_list[user_id]:
-                await bot.delete_msg(message_id=eachmsg["message_id"])
-            del dict_list[user_id]
-        else:
-            await bot.delete_msg(message_id=dict_list[user_id]["message_id"])
-    else:
-        for eachmsg in dict_list:
-            await bot.delete_msg(message_id=eachmsg["message_id"])
-        del dict_list
-
-
-async def mdlink_2_str(md_text):
-    result = []
-    pattern = r"\[([^\]]+)\]\(([^)]+)\)(\s*-\s*([^[]+))?"  # 匹配超链接及其描述
-    matches = re.findall(pattern, md_text)
-    for i, match in enumerate(matches):
-        # 提取标题
-        title = match[0].strip() if not match[3] else match[3].strip()
-        # 组合字符串
-        result.append(f"{i+1}. {title} - {match[1].strip()}")
-
-    output_str = "\n\n".join(result)
-    return output_str
-
-
 def is_useable(event, mode=poe_persistor.mode):
     if poe_persistor.poe_cookie:
         if mode == "black":
             try:
                 if str(event.user_id) in poe_persistor.blacklist:
                     logger.warning(f"黑名单用户:{str(event.user_id)},跳过")
                     return False
```

### Comparing `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/pwframework.py` & `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/pwframework.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.1/pyproject.toml` & `nonebot_plugin_spark_gpt-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_spark_gpt"
-version = "0.1.1"
+version = "0.1.2"
 description = "Spark-GPT,将多来源的gpt接入qq及更多平台,使用便捷,管理完善,功能强大"
 authors = ["canxin121 <1969730106@qq.com>"]
 readme = "README.md"
 packages = [{include = "nonebot_plugin_spark_gpt"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -19,14 +19,15 @@
 markdown = "^3.4.3"
 nonebot-plugin-guild-patch = "*"
 playwright = "^1.33.0"
 pydantic = "^1.10.7"
 nonebot-adapter-onebot = { version = "^2.0.0-beta.1", optional = true }
 pymdown-extensions = "^9.11"
 python-markdown-math = "^0.8"
+slack-sdk = "^3.21.3"
 
 [tool.poetry.extras]
 onebot = ["nonebot-adapter-onebot"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_spark_gpt-0.1.1/README.md` & `nonebot_plugin_spark_gpt-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 >
 ## [必看教程-残心小站-文档库](https://canxin121.github.io/docs/docs/Spark_GPT.html )
 
 > 用户交流群:[610948446](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=KHGqjjbiz6fpRr-W2X9SugTXThKFiprJ&authKey=LhpClaGtc4%2Ff3EL7f4IIIt7F94vLHJj4HSS8c2YCE55nRBRBtftzla%2Bgj7pa0fWX&noverify=0&group_code=610948446
 )
 ---
 
-- 目前支持将Poe,NewBing,Dalle,ChatGPT (session token)接入qq
+- 目前支持将Poe,NewBing,Dalle,ChatGPT (session token),Claude(slack)接入qq
 
 | Image 1 | Image 2 |
 |:-------:|:-------:|
 | ![1](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(1).png) | ![2](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(2).png) |
-| ![3](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png) | ![4](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(5).png) |
-| ![5](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(4).png) |                                   |
+| ![3](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png) | ![4](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(4).png) |
+| ![5](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(5).png) | ![6](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(6).png) |
+
+## 更新
+
+- 2023.5.11 0.1.2:  
+    1.增加claude_slack  
+    2.修复一些小bug
```

#### html2text {}

```diff
@@ -9,15 +9,17 @@
 ) > è¯¦ç»æç¨ï¼å¿çï¼å¦åä¸ä¼ä½¿ç¨ï¼ ç¹å»é¾æ¥è·³è½¬ð
 ç¹å»å¾çè·³è½¬âï¸ > è¯¦ç»æç¨ï¼å¿çï¼å¦åä¸ä¼ä½¿ç¨ï¼
 ç¹å»é¾æ¥è·³è½¬ð ç¹å»å¾çè·³è½¬âï¸ > ## [å¿çæç¨-
 æ®å¿å°ç«-ææ¡£åº](https://canxin121.github.io/docs/docs/Spark_GPT.html )
 > ç¨æ·äº¤æµç¾¤:[610948446](http://qm.qq.com/cgi-bin/qm/
 qr?_wv=1027&k=KHGqjjbiz6fpRr-
 W2X9SugTXThKFiprJ&authKey=LhpClaGtc4%2Ff3EL7f4IIIt7F94vLHJj4HSS8c2YCE55nRBRBtftzla%2Bgj7pa0fWX&noverify=0&group_code=610948446
-) --- - ç®åæ¯æå°Poe,NewBing,Dalle,ChatGPT (session token)æ¥å¥qq |
-Image 1 | Image 2 | |:-------:|:-------:| | ![1](https://github.com/canxin121/
-Spark-GPT/blob/main/source/spark/demo(1).png) | ![2](https://github.com/
-canxin121/Spark-GPT/blob/main/source/spark/demo(2).png) | | ![3](https://
-github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png) | ![4]
-(https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(5).png) | |
-![5](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(4).png)
-| |
+) --- - ç®åæ¯æå°Poe,NewBing,Dalle,ChatGPT (session token),Claude
+(slack)æ¥å¥qq | Image 1 | Image 2 | |:-------:|:-------:| | ![1](https://
+github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(1).png) | ![2]
+(https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(2).png) | |
+![3](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png)
+| ![4](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo
+(4).png) | | ![5](https://github.com/canxin121/Spark-GPT/blob/main/source/
+spark/demo(5).png) | ![6](https://github.com/canxin121/Spark-GPT/blob/main/
+source/spark/demo(6).png) | ## æ´æ° - 2023.5.11 0.1.2: 1.å¢å claude_slack
+2.ä¿®å¤ä¸äºå°bug
```

### Comparing `nonebot_plugin_spark_gpt-0.1.1/PKG-INFO` & `nonebot_plugin_spark_gpt-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-spark-gpt
-Version: 0.1.1
+Version: 0.1.2
 Summary: Spark-GPT,将多来源的gpt接入qq及更多平台,使用便捷,管理完善,功能强大
 Author: canxin121
 Author-email: 1969730106@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -20,14 +20,15 @@
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1,<3.0.0) ; extra == "onebot"
 Requires-Dist: nonebot-plugin-guild-patch
 Requires-Dist: nonebot2 (>=2.0.0-beta.1,<3.0.0)
 Requires-Dist: playwright (>=1.33.0,<2.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pymdown-extensions (>=9.11,<10.0)
 Requires-Dist: python-markdown-math (>=0.8,<0.9)
+Requires-Dist: slack-sdk (>=3.21.3,<4.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://github.com/canxin121">
     <img src="https://socialify.git.ci/canxin121/Spark-GPT/image?font=Raleway&forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=Auto" width="700" height="350">
   </a>
   <h1>Spark-GPT</h1>
@@ -60,15 +61,21 @@
 >
 ## [必看教程-残心小站-文档库](https://canxin121.github.io/docs/docs/Spark_GPT.html )
 
 > 用户交流群:[610948446](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=KHGqjjbiz6fpRr-W2X9SugTXThKFiprJ&authKey=LhpClaGtc4%2Ff3EL7f4IIIt7F94vLHJj4HSS8c2YCE55nRBRBtftzla%2Bgj7pa0fWX&noverify=0&group_code=610948446
 )
 ---
 
-- 目前支持将Poe,NewBing,Dalle,ChatGPT (session token)接入qq
+- 目前支持将Poe,NewBing,Dalle,ChatGPT (session token),Claude(slack)接入qq
 
 | Image 1 | Image 2 |
 |:-------:|:-------:|
 | ![1](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(1).png) | ![2](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(2).png) |
-| ![3](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png) | ![4](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(5).png) |
-| ![5](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(4).png) |                                   |
+| ![3](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png) | ![4](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(4).png) |
+| ![5](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(5).png) | ![6](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(6).png) |
+
+## 更新
+
+- 2023.5.11 0.1.2:  
+    1.增加claude_slack  
+    2.修复一些小bug
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-spark-gpt Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-spark-gpt Version: 0.1.2 Summary:
 Spark-
 GPT,å°å¤æ¥æºçgptæ¥å¥qqåæ´å¤å¹³å°,ä½¿ç¨ä¾¿æ·,ç®¡çå®å,åè½å¼ºå¤§
 Author: canxin121 Author-email: 1969730106@qq.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: onebot Requires-Dist: aiofiles (>=23.1.0,<24.0.0) Requires-
 Dist: aiohttp (>=3.8.4,<4.0.0) Requires-Dist: bidict (>=0.22.1,<0.23.0)
 Requires-Dist: edgegpt (>=0.3.6,<0.4.0) Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: imagegen (>=0.2,<0.3) Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: markdown (>=3.4.3,<4.0.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.0.0-beta.1,<3.0.0) ; extra == "onebot" Requires-Dist: nonebot-plugin-
 guild-patch Requires-Dist: nonebot2 (>=2.0.0-beta.1,<3.0.0) Requires-Dist:
 playwright (>=1.33.0,<2.0.0) Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pymdown-extensions (>=9.11,<10.0) Requires-Dist: python-
-markdown-math (>=0.8,<0.9) Description-Content-Type: text/markdown
+markdown-math (>=0.8,<0.9) Requires-Dist: slack-sdk (>=3.21.3,<4.0.0)
+Description-Content-Type: text/markdown
                 [https://socialify.git.ci/canxin121/Spark-GPT/
 image?font=Raleway&forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=Auto]
                             ****** Spark-GPT ******
                                    Spark-GPT
                             [pypi] [python] [pypi]
                                [onebot]_[github]
 --- [![æ®å¿å°ç«-ææ¡£åº](https://github.com/canxin121/Spark-GPT/blob/
@@ -25,15 +26,17 @@
 ) > è¯¦ç»æç¨ï¼å¿çï¼å¦åä¸ä¼ä½¿ç¨ï¼ ç¹å»é¾æ¥è·³è½¬ð
 ç¹å»å¾çè·³è½¬âï¸ > è¯¦ç»æç¨ï¼å¿çï¼å¦åä¸ä¼ä½¿ç¨ï¼
 ç¹å»é¾æ¥è·³è½¬ð ç¹å»å¾çè·³è½¬âï¸ > ## [å¿çæç¨-
 æ®å¿å°ç«-ææ¡£åº](https://canxin121.github.io/docs/docs/Spark_GPT.html )
 > ç¨æ·äº¤æµç¾¤:[610948446](http://qm.qq.com/cgi-bin/qm/
 qr?_wv=1027&k=KHGqjjbiz6fpRr-
 W2X9SugTXThKFiprJ&authKey=LhpClaGtc4%2Ff3EL7f4IIIt7F94vLHJj4HSS8c2YCE55nRBRBtftzla%2Bgj7pa0fWX&noverify=0&group_code=610948446
-) --- - ç®åæ¯æå°Poe,NewBing,Dalle,ChatGPT (session token)æ¥å¥qq |
-Image 1 | Image 2 | |:-------:|:-------:| | ![1](https://github.com/canxin121/
-Spark-GPT/blob/main/source/spark/demo(1).png) | ![2](https://github.com/
-canxin121/Spark-GPT/blob/main/source/spark/demo(2).png) | | ![3](https://
-github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png) | ![4]
-(https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(5).png) | |
-![5](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(4).png)
-| |
+) --- - ç®åæ¯æå°Poe,NewBing,Dalle,ChatGPT (session token),Claude
+(slack)æ¥å¥qq | Image 1 | Image 2 | |:-------:|:-------:| | ![1](https://
+github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(1).png) | ![2]
+(https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(2).png) | |
+![3](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png)
+| ![4](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo
+(4).png) | | ![5](https://github.com/canxin121/Spark-GPT/blob/main/source/
+spark/demo(5).png) | ![6](https://github.com/canxin121/Spark-GPT/blob/main/
+source/spark/demo(6).png) | ## æ´æ° - 2023.5.11 0.1.2: 1.å¢å claude_slack
+2.ä¿®å¤ä¸äºå°bug
```

