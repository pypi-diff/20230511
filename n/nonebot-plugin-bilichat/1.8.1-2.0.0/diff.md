# Comparing `tmp/nonebot_plugin_bilichat-1.8.1.tar.gz` & `tmp/nonebot_plugin_bilichat-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-1.8.1.tar", last modified: Sun May  7 17:18:19 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.0.0.tar", last modified: Thu May 11 16:36:34 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-1.8.1.tar` & `nonebot_plugin_bilichat-2.0.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0    34523 2023-05-07 17:18:04.896358 nonebot_plugin_bilichat-1.8.1/LICENSE
--rw-r--r--   0        0        0    11854 2023-05-07 17:18:04.896358 nonebot_plugin_bilichat-1.8.1/README.md
--rw-r--r--   0        0        0     5837 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4809 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6439 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      399 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-05-07 17:18:04.908358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1045 2023-05-07 17:18:04.908358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5825 2023-05-07 17:18:04.908358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-05-07 17:18:04.908358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2343 2023-05-07 17:18:04.908358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-05-07 17:18:04.908358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     2268 2023-05-07 17:18:04.908358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/utils.py
--rw-r--r--   0        0        0     1780 2023-05-07 17:18:04.908358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1407 2023-05-07 17:18:19.236206 nonebot_plugin_bilichat-1.8.1/pyproject.toml
--rw-r--r--   0        0        0    13143 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-11 16:36:22.185470 nonebot_plugin_bilichat-2.0.0/LICENSE
+-rw-r--r--   0        0        0    11827 2023-05-11 16:36:22.185470 nonebot_plugin_bilichat-2.0.0/README.md
+-rw-r--r--   0        0        0     7862 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4805 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6439 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      399 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-05-11 16:36:22.193471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-05-11 16:36:22.197471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1045 2023-05-11 16:36:22.197471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5825 2023-05-11 16:36:22.197471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-05-11 16:36:22.197471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2343 2023-05-11 16:36:22.197471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-05-11 16:36:22.197471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-05-11 16:36:22.197471 nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1447 2023-05-11 16:36:34.873490 nonebot_plugin_bilichat-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    13164 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.0.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-1.8.1/LICENSE` & `nonebot_plugin_bilichat-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/README.md` & `nonebot_plugin_bilichat-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 ### 通用配置项
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | bilichat_block              | bool      | False | 是否拦截事件(防止其他插件二次解析) |
 | bilichat_enable_private     | bool      | True  | 是否允许响应私聊 |
 | bilichat_enable_self        | bool      | False | 是否允许响应自身的消息 |
-| bilichat_enable_v12_channel | bool      | True  | ~~是否允许响应频道消息(ob12专属)~~(暂未实现) |
+| bilichat_enable_channel     | bool      | True  | 是否允许响应频道的消息 |
 | bilichat_enable_unkown_src  | bool      | False | 是否允许响应未知来源的消息 |
 | bilichat_whitelist          | list[str] | []    | **响应**的群聊(频道)名单, 会覆盖黑名单 |
 | bilichat_blacklist          | list[str] | []    | **不响应**的群聊(频道)名单 |
 | bilichat_dynamic_font       | str       | None  | 视频信息及词云图片使用的字体 |
 | bilichat_cd_time            | int       | 120   | 对同一视频的响应冷却时间(防止刷屏) |
 | bilichat_neterror_retry     | int       | 3     | 对部分网络请求错误的尝试次数 |
 | bilichat_use_bcut_asr       | bool      | True  | 是否在**没有字幕时**调用必剪接口生成字幕 |
```

#### html2text {}

```diff
@@ -31,20 +31,19 @@
 æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot_plugin_bilichat"]  ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½®, éç½®åä¸º**éå¿é¡»é¡¹**
 ### éç¨éç½®é¡¹ | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:
 |:----:|:----:| | bilichat_block | bool | False | æ¯å¦æ¦æªäºä»¶
 (é²æ­¢å¶ä»æä»¶äºæ¬¡è§£æ) | | bilichat_enable_private | bool | True |
 æ¯å¦åè®¸ååºç§è | | bilichat_enable_self | bool | False |
-æ¯å¦åè®¸ååºèªèº«çæ¶æ¯ | | bilichat_enable_v12_channel | bool | True
-| ~~æ¯å¦åè®¸ååºé¢éæ¶æ¯(ob12ä¸å±)~~(ææªå®ç°) | |
-bilichat_enable_unkown_src | bool | False |
-æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist | list[str] | []
-| **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | | bilichat_blacklist
-| list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
+æ¯å¦åè®¸ååºèªèº«çæ¶æ¯ | | bilichat_enable_channel | bool | True |
+æ¯å¦åè®¸ååºé¢éçæ¶æ¯ | | bilichat_enable_unkown_src | bool | False
+| æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist | list[str] |
+[] | **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | |
+bilichat_blacklist | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
 (é²æ­¢å·å±) | | bilichat_neterror_retry | int | 3 |
 å¯¹é¨åç½ç»è¯·æ±éè¯¯çå°è¯æ¬¡æ° | | bilichat_use_bcut_asr | bool |
 True | æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | æ³¨: 1.
 ç±äº OneBot
 åè®®æªè§å®æ¯å¦åºä¸æ¥èªèº«äºä»¶ï¼å æ­¤å¨ä¸åçåºæ¯ä¸è½å¦è·åèªèº«äºä»¶å¹¶ä¸ä¸å®ï¼`bilichat_enable_self`
```

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,52 @@
+import contextlib
 import re
 import shlex
 from itertools import chain
-from typing import cast
+from typing import Union, cast
 
 from nonebot.adapters import MessageSegment
+from nonebot.adapters.mirai2 import Bot as Mirai_Bot
+from nonebot.adapters.mirai2.event import FriendMessage as Mirai_PME
+from nonebot.adapters.mirai2.event import GroupMessage as Mirai_GME
+from nonebot.adapters.mirai2.event import MessageEvent as Mirai_ME
+from nonebot.adapters.onebot.v11 import Bot as V11_Bot
 from nonebot.adapters.onebot.v11 import GroupMessageEvent as V11_GME
+from nonebot.adapters.onebot.v11 import MessageEvent as V11_ME
 from nonebot.adapters.onebot.v11 import PrivateMessageEvent as V11_PME
+from nonebot.adapters.onebot.v12 import Bot as V12_Bot
+from nonebot.adapters.onebot.v12 import ChannelMessageEvent as V12_CME
 from nonebot.adapters.onebot.v12 import GroupMessageEvent as V12_GME
+from nonebot.adapters.onebot.v12 import MessageEvent as V12_ME
 from nonebot.adapters.onebot.v12 import PrivateMessageEvent as V12_PME
+from nonebot.adapters.qqguild import Bot as QG_Bot
+from nonebot.adapters.qqguild.event import MessageEvent as QG_ME
 from nonebot.consts import REGEX_GROUP, REGEX_STR
 from nonebot.exception import FinishedException
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.params import Depends
-from nonebot.plugin import PluginMetadata, on_regex
+from nonebot.plugin import PluginMetadata, on_regex, require
 from nonebot.rule import Rule
 from nonebot.typing import T_State
 
 from .config import __version__, plugin_config
 from .lib.b23_extract import b23_extract
 from .lib.content_resolve import get_column_basic, get_content_cache, get_video_basic
 from .model.arguments import Options, parser
 from .model.exception import AbortError
 from .optional import capture_exception  # type: ignore
-from .utils import BOT, MESSAGE_EVENT, get_image, get_reply
+
+require("nonebot_plugin_segbuilder")
+
+
+from nonebot_plugin_segbuilder import SegmentBuilder
+
+BOT = Union[V11_Bot, V12_Bot, QG_Bot, Mirai_Bot]
+MESSAGE_EVENT = Union[V11_ME, V12_ME, QG_ME, Mirai_ME]
 
 if plugin_config.bilichat_openai_token or plugin_config.bilichat_newbing_cookie:
     ENABLE_SUMMARY = True
     from .summary import summarization
 else:
     ENABLE_SUMMARY = False
 
@@ -47,23 +66,26 @@
     },
 )
 
 
 async def _bili_check(bot: BOT, event: MESSAGE_EVENT, state: T_State):
     if str(event.get_user_id()) == str(bot.self_id):
         return plugin_config.bilichat_enable_self
-    elif isinstance(event, (V11_PME, V12_PME)):
-        state["_uid_"] = event.user_id
+    elif isinstance(event, (V11_PME, V12_PME, Mirai_PME)):
+        state["_uid_"] = event.get_user_id()
         return plugin_config.bilichat_enable_private
     elif isinstance(event, (V11_GME, V12_GME)):
         state["_uid_"] = event.group_id
         return plugin_config.verify_permission(event.group_id)
-    # elif isinstance(event, V12_CME):
-    #     state["_uid_"] = event.channel_id
-    #     return plugin_config.bilichat_enable_v12_channel
+    elif isinstance(event, Mirai_GME):
+        state["_uid_"] = event.sender.group.id
+        return plugin_config.verify_permission(event.sender.group.id)
+    elif isinstance(event, (V12_CME, QG_ME)):
+        state["_uid_"] = event.channel_id
+        return plugin_config.bilichat_enable_channel
     else:
         state["_uid_"] = "unkown"
         return plugin_config.bilichat_enable_unkown_src
 
 
 bili = on_regex(
     r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})|cv(\d{1,16})",
@@ -113,28 +135,38 @@
 async def video_info(
     bot: BOT,
     event: MESSAGE_EVENT,
     state: T_State,
     matcher: Matcher,
     options: Options = Depends(get_args),
 ):
-    reply = await get_reply(event)
+    DISABLE_REPLY = isinstance(bot, Mirai_Bot)  # 部分平台Reply暂不可用
+    DISABLE_LINK = isinstance(bot, QG_Bot)  # 部分平台发送链接都要审核
+    SEND_IMAGE_SEPARATELY = isinstance(bot, QG_Bot)  # 部分平台无法一次性发送多张图片，或无法与其他消息组合发出
+    reply = "" if DISABLE_REPLY else await SegmentBuilder.reply(bot, event)
     # basic info
     bili_number, uid = state["bili_number"], state["_uid_"]
     if bili_number[:2] in ["BV", "bv", "av"]:
         msg, img, info = await get_video_basic(bili_number, uid)
         if not msg or not info:
             raise FinishedException
         if not img:
             await matcher.finish(reply + msg)
         elif img != "IMG_RENDER_DISABLED":
-            image = await get_image(img, bot)
-            msgid = (await matcher.send(reply + image + msg))["message_id"]  # type: ignore
-            if plugin_config.bilichat_reply_to_basic_info:
-                reply = await get_reply(event, msgid)
+            image = await SegmentBuilder.image(bot, img)
+            msg = "" if DISABLE_LINK else msg
+            if SEND_IMAGE_SEPARATELY:
+                if reply and msg:
+                    await matcher.send(reply + msg)
+                re_msg = await matcher.send(image)
+            else:
+                re_msg = await matcher.send(reply + image + msg)
+            if plugin_config.bilichat_reply_to_basic_info and not DISABLE_REPLY:
+                with contextlib.suppress(Exception):
+                    reply = await SegmentBuilder.reply(bot, event, re_msg["message_id"])
     elif bili_number[:2] == "cv" and FUTUER_FUCTIONS:
         info = await get_column_basic(bili_number, uid)
         if not info:
             raise FinishedException
         elif isinstance(info, str):
             await matcher.finish(reply + info)
     else:
@@ -155,22 +187,31 @@
         logger.exception(e)
         await matcher.finish(f"{reply}未知错误: {e}")
 
     # wordcloud
     wc_image = ""
     if plugin_config.bilichat_word_cloud:
         if image := await wordcloud(cache=cache, cid=str(info.cid)):
-            wc_image = await get_image(image, bot)
+            wc_image = await SegmentBuilder.image(bot, image)
         else:
             await matcher.finish(f"{reply}视频无有效字幕")
 
     # summary
     summary = ""
     if ENABLE_SUMMARY:
         if summary := await summarization(cache=cache, cid=str(info.cid)):
             if isinstance(summary, bytes):
-                summary = await get_image(summary, bot)
+                summary = await SegmentBuilder.image(bot, summary)
         else:
             await matcher.finish(f"{reply}视频无有效字幕")
 
-    if wc_image or summary:
+    if wc_image:
+        if SEND_IMAGE_SEPARATELY:
+            await matcher.send(wc_image)
+            if summary:
+                await matcher.finish(summary)
+        await matcher.finish(reply + wc_image + summary)  # type: ignore
+
+    elif summary:
+        if SEND_IMAGE_SEPARATELY:
+            await matcher.finish(summary)
         await matcher.finish(reply + wc_image + summary)  # type: ignore
```

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 class Config(BaseModel):
     # general
     bilichat_block: bool = False
     bilichat_enable_private: bool = True
     bilichat_enable_self: bool = False
-    bilichat_enable_v12_channel: bool = True
+    bilichat_enable_channel: bool = True
     bilichat_enable_unkown_src: bool = False
     bilichat_whitelist: List[str] = []
     bilichat_blacklist: List[str] = []
     bilichat_dynamic_font: Optional[str]
     bilichat_cd_time: int = 120
     bilichat_neterror_retry = 3
     nickname: List[str] = ["awesome-nonebot"]
```

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.0.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.1/pyproject.toml` & `nonebot_plugin_bilichat-2.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,29 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "1.8.1"
+version = "2.0.0"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
     "bilireq>=0.2.4",
     "qrcode>=7.4.2",
     "pillow>=9.5.0",
     "lxml>=4.9.2",
     "nonebot-plugin-localstore>=0.4.1",
     "nonebot-adapter-onebot>=2.2.2",
+    "nonebot-plugin-segbuilder>=0.1.1",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "AGPL3.0"
```

### Comparing `nonebot_plugin_bilichat-1.8.1/PKG-INFO` & `nonebot_plugin_bilichat-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 1.8.1
+Version: 2.0.0
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2
+Requires-Dist: nonebot-plugin-segbuilder>=0.1.1
 Requires-Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra"
 Requires-Dist: jieba>=0.42.1; extra == "wordcloud"
 Requires-Dist: wordcloud>=1.8.2.2; extra == "wordcloud"
 Requires-Dist: tiktoken-async>=0.3.2; extra == "openai"
 Requires-Dist: minidynamicrender>=1.1.9; extra == "openai"
 Requires-Dist: EdgeGPT>=0.1.22.1; extra == "newbing"
 Requires-Dist: minidynamicrender>=1.1.9; extra == "newbing"
@@ -173,15 +174,15 @@
 ### 通用配置项
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | bilichat_block              | bool      | False | 是否拦截事件(防止其他插件二次解析) |
 | bilichat_enable_private     | bool      | True  | 是否允许响应私聊 |
 | bilichat_enable_self        | bool      | False | 是否允许响应自身的消息 |
-| bilichat_enable_v12_channel | bool      | True  | ~~是否允许响应频道消息(ob12专属)~~(暂未实现) |
+| bilichat_enable_channel     | bool      | True  | 是否允许响应频道的消息 |
 | bilichat_enable_unkown_src  | bool      | False | 是否允许响应未知来源的消息 |
 | bilichat_whitelist          | list[str] | []    | **响应**的群聊(频道)名单, 会覆盖黑名单 |
 | bilichat_blacklist          | list[str] | []    | **不响应**的群聊(频道)名单 |
 | bilichat_dynamic_font       | str       | None  | 视频信息及词云图片使用的字体 |
 | bilichat_cd_time            | int       | 120   | 对同一视频的响应冷却时间(防止刷屏) |
 | bilichat_neterror_retry     | int       | 3     | 对部分网络请求错误的尝试次数 |
 | bilichat_use_bcut_asr       | bool      | True  | 是否在**没有字幕时**调用必剪接口生成字幕 |
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.8.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.0.0 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
-Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra" Requires-Dist:
-jieba>=0.42.1; extra == "wordcloud" Requires-Dist: wordcloud>=1.8.2.2; extra ==
-"wordcloud" Requires-Dist: tiktoken-async>=0.3.2; extra == "openai" Requires-
-Dist: minidynamicrender>=1.1.9; extra == "openai" Requires-Dist:
-EdgeGPT>=0.1.22.1; extra == "newbing" Requires-Dist: minidynamicrender>=1.1.9;
-extra == "newbing" Requires-Dist: jieba>=0.42.1; extra == "all" Requires-Dist:
-wordcloud>=1.8.2.2; extra == "all" Requires-Dist: tiktoken-async>=0.3.2; extra
-== "all" Requires-Dist: EdgeGPT>=0.1.22.1; extra == "all" Requires-Dist:
+Dist: nonebot-plugin-segbuilder>=0.1.1 Requires-Dist: nonebot-plugin-
+sentry>=0.2.2; extra == "extra" Requires-Dist: jieba>=0.42.1; extra ==
+"wordcloud" Requires-Dist: wordcloud>=1.8.2.2; extra == "wordcloud" Requires-
+Dist: tiktoken-async>=0.3.2; extra == "openai" Requires-Dist:
+minidynamicrender>=1.1.9; extra == "openai" Requires-Dist: EdgeGPT>=0.1.22.1;
+extra == "newbing" Requires-Dist: minidynamicrender>=1.1.9; extra == "newbing"
+Requires-Dist: jieba>=0.42.1; extra == "all" Requires-Dist: wordcloud>=1.8.2.2;
+extra == "all" Requires-Dist: tiktoken-async>=0.3.2; extra == "all" Requires-
+Dist: EdgeGPT>=0.1.22.1; extra == "all" Requires-Dist:
 minidynamicrender>=1.1.9; extra == "all" Provides-Extra: extra Provides-Extra:
 wordcloud Provides-Extra: openai Provides-Extra: newbing Provides-Extra: all
 Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
     # nonebot-plugin-bilichat _â¨ å¤åè½çBç«è§é¢è§£æå·¥å· â¨_
 [license] [PyPI_-_Downloads] [pypi] [python] [pdm-managed] [Code_style:_black]
@@ -49,20 +50,19 @@
 æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot_plugin_bilichat"]  ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½®, éç½®åä¸º**éå¿é¡»é¡¹**
 ### éç¨éç½®é¡¹ | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:
 |:----:|:----:| | bilichat_block | bool | False | æ¯å¦æ¦æªäºä»¶
 (é²æ­¢å¶ä»æä»¶äºæ¬¡è§£æ) | | bilichat_enable_private | bool | True |
 æ¯å¦åè®¸ååºç§è | | bilichat_enable_self | bool | False |
-æ¯å¦åè®¸ååºèªèº«çæ¶æ¯ | | bilichat_enable_v12_channel | bool | True
-| ~~æ¯å¦åè®¸ååºé¢éæ¶æ¯(ob12ä¸å±)~~(ææªå®ç°) | |
-bilichat_enable_unkown_src | bool | False |
-æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist | list[str] | []
-| **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | | bilichat_blacklist
-| list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
+æ¯å¦åè®¸ååºèªèº«çæ¶æ¯ | | bilichat_enable_channel | bool | True |
+æ¯å¦åè®¸ååºé¢éçæ¶æ¯ | | bilichat_enable_unkown_src | bool | False
+| æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist | list[str] |
+[] | **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | |
+bilichat_blacklist | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
 (é²æ­¢å·å±) | | bilichat_neterror_retry | int | 3 |
 å¯¹é¨åç½ç»è¯·æ±éè¯¯çå°è¯æ¬¡æ° | | bilichat_use_bcut_asr | bool |
 True | æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | æ³¨: 1.
 ç±äº OneBot
 åè®®æªè§å®æ¯å¦åºä¸æ¥èªèº«äºä»¶ï¼å æ­¤å¨ä¸åçåºæ¯ä¸è½å¦è·åèªèº«äºä»¶å¹¶ä¸ä¸å®ï¼`bilichat_enable_self`
```

