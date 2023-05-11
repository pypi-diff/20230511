# Comparing `tmp/nonebot-plugin-alconna-0.4.0.tar.gz` & `tmp/nonebot-plugin-alconna-0.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-alconna-0.4.0.tar", last modified: Thu May 11 06:05:27 2023, max compression
+gzip compressed data, was "nonebot-plugin-alconna-0.4.0rc1.tar", last modified: Wed May 10 10:32:49 2023, max compression
```

## Comparing `nonebot-plugin-alconna-0.4.0.tar` & `nonebot-plugin-alconna-0.4.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.4.0/LICENSE
--rw-r--r--   0        0        0     1135 2023-05-11 02:05:54.054693 nonebot-plugin-alconna-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     8579 2023-05-11 05:49:49.600962 nonebot-plugin-alconna-0.4.0/README.md
--rw-r--r--   0        0        0     1208 2023-05-10 08:50:46.247626 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/__init__.py
--rw-r--r--   0        0        0      383 2023-05-11 04:41:26.166268 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/__init__.py
--rw-r--r--   0        0        0      523 2023-05-10 10:09:15.599546 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/bilibili.py
--rw-r--r--   0        0        0     1007 2023-05-10 10:09:15.573188 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/console.py
--rw-r--r--   0        0        0     1661 2023-05-10 10:09:15.609172 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/ding.py
--rw-r--r--   0        0        0     2141 2023-05-10 10:09:15.564123 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/feishu.py
--rw-r--r--   0        0        0      519 2023-05-10 10:09:15.541809 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/github.py
--rw-r--r--   0        0        0     1163 2023-05-10 10:09:15.636179 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/kook.py
--rw-r--r--   0        0        0      761 2023-05-10 10:09:15.651191 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/minecraft.py
--rw-r--r--   0        0        0     3155 2023-05-10 10:09:15.519983 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/mirai.py
--rw-r--r--   0        0        0     1088 2023-05-10 10:09:15.628175 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/ntchat.py
--rw-r--r--   0        0        0     3177 2023-05-10 10:09:15.618177 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/onebot11.py
--rw-r--r--   0        0        0     2517 2023-05-10 10:09:15.661217 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/onebot12.py
--rw-r--r--   0        0        0     3227 2023-05-10 10:09:15.529594 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/qqguild.py
--rw-r--r--   0        0        0     3126 2023-05-10 10:09:15.670151 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/telegram.py
--rw-r--r--   0        0        0      581 2023-05-10 10:09:15.553296 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/argv.py
--rw-r--r--   0        0        0      405 2023-05-10 09:00:57.054628 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/config.py
--rw-r--r--   0        0        0      180 2023-05-10 08:33:24.079951 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/consts.py
--rw-r--r--   0        0        0      115 2023-05-10 08:33:24.132983 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/i18n/.config.json
--rw-r--r--   0        0        0      190 2023-05-10 08:33:24.069340 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/i18n/en-US.json
--rw-r--r--   0        0        0      170 2023-05-10 08:33:24.090951 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0     3812 2023-05-10 09:00:57.030628 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/matcher.py
--rw-r--r--   0        0        0     1499 2023-05-10 08:54:25.558632 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/matcher.pyi
--rw-r--r--   0        0        0     1417 2023-05-10 08:27:49.596958 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/model.py
--rw-r--r--   0        0        0     2187 2023-04-02 14:03:55.798752 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/params.py
--rw-r--r--   0        0        0     9203 2023-05-11 02:04:08.656227 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/rule.py
--rw-r--r--   0        0        0     1967 2023-05-11 04:48:52.932671 nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/typings.py
--rw-r--r--   0        0        0     8658 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.4.0rc1/LICENSE
+-rw-r--r--   0        0        0     1144 2023-05-10 08:21:46.157932 nonebot-plugin-alconna-0.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     7529 2023-05-10 08:21:46.125592 nonebot-plugin-alconna-0.4.0rc1/README.md
+-rw-r--r--   0        0        0     1208 2023-05-10 08:50:46.247626 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-26 16:08:53.308451 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/__init__.py
+-rw-r--r--   0        0        0      523 2023-05-10 10:09:15.599546 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/bilibili.py
+-rw-r--r--   0        0        0     1007 2023-05-10 10:09:15.573188 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/console.py
+-rw-r--r--   0        0        0     1661 2023-05-10 10:09:15.609172 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/ding.py
+-rw-r--r--   0        0        0     2141 2023-05-10 10:09:15.564123 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/feishu.py
+-rw-r--r--   0        0        0      519 2023-05-10 10:09:15.541809 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/github.py
+-rw-r--r--   0        0        0     1163 2023-05-10 10:09:15.636179 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/kook.py
+-rw-r--r--   0        0        0      761 2023-05-10 10:09:15.651191 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/minecraft.py
+-rw-r--r--   0        0        0     3155 2023-05-10 10:09:15.519983 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/mirai.py
+-rw-r--r--   0        0        0     1088 2023-05-10 10:09:15.628175 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/ntchat.py
+-rw-r--r--   0        0        0     3177 2023-05-10 10:09:15.618177 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/onebot11.py
+-rw-r--r--   0        0        0     2517 2023-05-10 10:09:15.661217 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/onebot12.py
+-rw-r--r--   0        0        0     3227 2023-05-10 10:09:15.529594 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/qqguild.py
+-rw-r--r--   0        0        0     3126 2023-05-10 10:09:15.670151 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/telegram.py
+-rw-r--r--   0        0        0      581 2023-05-10 10:09:15.553296 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/argv.py
+-rw-r--r--   0        0        0      405 2023-05-10 09:00:57.054628 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/config.py
+-rw-r--r--   0        0        0      180 2023-05-10 08:33:24.079951 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/consts.py
+-rw-r--r--   0        0        0      115 2023-05-10 08:33:24.132983 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/i18n/.config.json
+-rw-r--r--   0        0        0      190 2023-05-10 08:33:24.069340 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/i18n/en-US.json
+-rw-r--r--   0        0        0      170 2023-05-10 08:33:24.090951 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0     3812 2023-05-10 09:00:57.030628 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/matcher.py
+-rw-r--r--   0        0        0     1499 2023-05-10 08:54:25.558632 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/matcher.pyi
+-rw-r--r--   0        0        0     1417 2023-05-10 08:27:49.596958 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/model.py
+-rw-r--r--   0        0        0     2187 2023-04-02 14:03:55.798752 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/params.py
+-rw-r--r--   0        0        0     9071 2023-05-10 10:32:39.813272 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/rule.py
+-rw-r--r--   0        0        0     1591 2023-05-10 08:33:24.123949 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/typings.py
+-rw-r--r--   0        0        0     7641 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.4.0rc1/PKG-INFO
```

### Comparing `nonebot-plugin-alconna-0.4.0/LICENSE` & `nonebot-plugin-alconna-0.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/pyproject.toml` & `nonebot-plugin-alconna-0.4.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "nonebot-plugin-alconna"
-version = "0.4.0"
+version = "0.4.0rc1"
 description = "Alconna Adapter for Nonebot"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc4",
-    "arclet-alconna<2.0.0, >=1.7.0",
-    "arclet-alconna-tools<0.7.0, >=0.6.0",
+    "arclet-alconna<2.0.0, >=1.7.0rc6",
+    "arclet-alconna-tools<0.7.0, >=0.6.0rc1",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "command",
     "argparse",
     "cli",
```

### Comparing `nonebot-plugin-alconna-0.4.0/README.md` & `nonebot-plugin-alconna-0.4.0rc1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 ## 特性
 
 - 完整的 Alconna 特性支持
 - 基本的 rule, matcher 与 依赖注入
 - 自动回复命令帮助信息 (help, shortcut, completion) 选项
 - 现有全部协议的 Segment 标注
 - match_value, match_path 等检查函数
-- 补全会话支持
 
 ## 讨论
 
 QQ 交流群: [链接](https://jq.qq.com/?_wv=1027&k=PUPOnCSH)
 
 
 ## 使用方法
@@ -53,70 +52,46 @@
 assert res.matched
 assert res.query("foo.foo") == 123
 assert not alc.parse(Message(["Hello!", img])).matched
 ```
 
 ### MessageSegment 标注
 
-特定适配器:
-
 ```python
 from nonebot_plugin_alconna.adapters.onebot12 import Mention
 from nonebot.adapters.onebot.v12 import Message
 from arclet.alconna import Alconna, Args
 
 msg = Message(["Hello!", Mention("123")])
 print(msg)  # Hello![mention:user_id=123]
 
 alc = Alconna("Hello!", Args["target", Mention])
 res = alc.parse(msg)
 assert res.matched
 assert res.query("target").data['user_id'] == '123'
 ```
 
-通用标注:
-
-```python
-from nonebot.adapters.onebot.v12 import Message as Ob12M, MessageSegment as Ob12MS
-from nonebot.adapters.onebot.v11 import Message as Ob11M, MessageSegment as Ob11MS
-from nonebot_plugin_alconna.adapters import At
-from arclet.alconna import Alconna, Args
-
-msg1 = Ob12M(["Hello!", Ob12MS.mention("123")])
-print(msg1)  # Hello![mention:user_id=123]
-msg2 = Ob11M(["Hello!", Ob11MS.at(123)])
-print(msg2)  # Hello![CQ:at,qq=123]
-
-alc = Alconna("Hello!", Args["target", At])
-res1 = alc.parse(msg1)
-assert res1.matched
-assert res1.query("target").data['user_id'] == '123'
-
-res2 = alc.parse(msg2)
-assert res2.matched
-assert res2.query("target").data['qq'] == 123
-```
-
 ### Matcher 与 依赖注入
 ```python
 ...
 from nonebot import require
 require("nonebot_plugin_alconna")
 ...
 
 from nonebot_plugin_alconna import (
     on_alconna, 
     Match,
     Query,
     AlconnaMatch, 
     AlconnaQuery,
+    AlconnaResult, 
     AlcMatches,
     AlcResult
 )
-from arclet.alconna import Alconna, Args, Option
+from arclet.alconna import Alconna, Args, Arparma, Option
 
 test = on_alconna(
     Alconna(
         "test",
         Option("foo", Args["bar", int]),
         Option("baz", Args["qux", bool, False])
     ),
@@ -166,17 +141,17 @@
     ),
     Subcommand(
         "list",
         Option("--out-dated")
     )
 )
 
-pip_update = on_alconna(pip, [assign("install.pak", "pip")])
-pip_match_install = on_alconna(pip, [assign("install")])
-pip_match_list = on_alconna(pip, [assign("list")])
+pip_update = on_alconna(pip, assign("install.pak", "pip"))
+pip_match_install = on_alconna(pip, assign("install"))
+pip_match_list = on_alconna(pip, assign("list"))
 
 @pip_update.handle()
 async def update(arp: CommandResult = AlconnaResult()):
     ...
 
 @pip_match_list.handle()
 async def list_(arp: CommandResult = AlconnaResult()):
@@ -225,38 +200,33 @@
 
 ## 配置
 
 目前配置项有：
 
 - ALCONNA_AUTO_SEND_OUTPUT : 是否全局启用输出信息自动发送
 - ALCONNA_USE_COMMAND_START : 是否将 COMMAND_START 作为全局命令前缀
-- ALCONNA_AUTO_COMPLETION: 是否全局启用补全会话功能
 
 ## 参数解释
 
 ```python
 def on_alconna(
     command: Alconna | str,
-    checker: list[Callable[[Arparma], bool]] | None = None,
+    *checker: Callable[[Arparma], bool],
     skip_for_unmatch: bool = True,
     auto_send_output: bool = False,
-    output_converter: Callable[[OutputType, str], Message | Awaitable[Message]] | None = None,
-    aliases: set[str | tuple[str, ...]] | None = None,
-    comp_config: CompConfig | None = None,
+    output_converter: Callable[[str], Message | Awaitable[Message]] | None = None,
     **kwargs,
 ) -> type[Matcher]:
 ```
 
 - `command`: Alconna 命令
 - `checker`: 命令解析结果的检查器
 - `skip_for_unmatch`: 是否在命令不匹配时跳过该响应
 - `auto_send_output`: 是否自动发送输出信息并跳过响应
 - `output_converter`: 输出信息字符串转换为 Message 方法
-- `aliases`: 命令别名, 作用类似于 `on_command`
-- `comp_config`: 补全会话配置, 不传入则不启用补全会话
 
 ## 提供了 MessageSegment标注 的协议:
 
 | 协议名称                                                                | 路径                                   |
 |---------------------------------------------------------------------|--------------------------------------|
 | [OneBot 协议](https://onebot.dev/)                                    | adapters.onebot11, adapters.onebot12 |
 | [Telegram](https://core.telegram.org/bots/api)                      | adapters.telegram                    |
```

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/__init__.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/bilibili.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/bilibili.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/console.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/console.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/ding.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/ding.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/feishu.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/feishu.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/github.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/github.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/kook.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/kook.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/minecraft.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/minecraft.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/mirai.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/mirai.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/ntchat.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/ntchat.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/onebot11.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/onebot11.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/onebot12.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/onebot12.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/qqguild.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/adapters/telegram.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/telegram.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/argv.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/argv.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/matcher.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/matcher.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/matcher.pyi` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/matcher.pyi`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/model.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/model.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/params.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/params.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/rule.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,65 +114,61 @@
             meta=CommandMeta(hide=True, compact=True)
         )
         _waiter = on_message(priority=self.comp_config.get('priority', -100), block=True)
         _futures: Dict[str, asyncio.Future] = {}
 
         @_waiter.handle()
         async def _waiter_handle(content: Message = EventMessage()):
-            if _exit.parse(content).matched:
-                _futures["_"].set_result(False)
-                await _waiter.finish()
-            if (mat := _tab.parse(content)).matched:
-                interface.tab(mat.offset)
-                await self.send("\n".join(interface.lines()), bot, event, res)
-                await _waiter.reject()
-            if (mat := _enter.parse(content)).matched:
-                _futures["_"].set_result(mat.content)
-                await _waiter.finish()
-            await self.send(interface.current(), bot, event, res)
-            await _waiter.reject()
+            _futures["_"].set_result(content)
 
         def clear():
             interface.clear()
             _waiter.destroy()
-            command_manager.delete(_tab)
-            command_manager.delete(_enter)
-            command_manager.delete(_exit)
 
         with interface:
             res = self.command.parse(msg)
         while interface.available:
             res = Arparma(self.command.path, msg, False, error_info=SpecialOptionTriggered("completion"))
             await self.send(str(interface), bot, event, res)
             await self.send(
                 f"{lang.require('alconna/nonebot', 'tab').format(cmd=_tab.command)}\n"
                 f"{lang.require('alconna/nonebot', 'enter').format(cmd=_enter.command)}\n"
                 f"{lang.require('alconna/nonebot', 'exit').format(cmd=_exit.command)}",
                 bot, event, res
             )
-            _future = _futures.setdefault("_", asyncio.get_running_loop().create_future())
-            _future.add_done_callback(lambda x: _futures.pop("_"))
-            try:
-                await asyncio.wait_for(_future, timeout=60)
-            except asyncio.TimeoutError:
-                clear()
-                return res
-            content: Union[Message, bool] = _future.result()
-            if content is False:
-                clear()
-                return res
-            param = list(content)
-            if not param or not param[0]:
-                param = None
-            try:
-                with interface:
-                    res = interface.enter(param)
-            except Exception as e:
-                traceback.print_exc()
-                await self.send(str(e), bot, event, res)
+            while True:
+                _future = _futures.setdefault("_", asyncio.Future())
+                _future.add_done_callback(lambda x: _futures.pop("_"))
+                try:
+                    await asyncio.wait_for(_future, timeout=30)
+                except asyncio.TimeoutError:
+                    clear()
+                    return res
+                content: Message = _future.result()
+                if _exit.parse(content).matched:
+                    clear()
+                    return res
+                if (mat := _tab.parse(content)).matched:
+                    interface.tab(mat.offset)
+                    await self.send("\n".join(interface.lines()), bot, event, res)
+                    continue
+                if (mat := _enter.parse(content)).matched:
+                    param = list(mat.content)
+                    if not param or not param[0]:
+                        param = None
+                    try:
+                        with interface:
+                            res = interface.enter(param)
+                    except Exception as e:
+                        traceback.print_exc()
+                        await self.send(str(e), bot, event, res)
+                        continue
+                    break
+                else:
+                    await self.send(interface.current(), bot, event, res)
         clear()
         return res
 
     async def __call__(self, event: Event, state: T_State, bot: Bot) -> bool:
         if event.get_type() != "message":
             return False
         try:
```

### Comparing `nonebot-plugin-alconna-0.4.0/src/nonebot_plugin_alconna/typings.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/typings.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from nepattern import BasePattern, PatternModel, MatchFailed
 from nonebot.internal.adapter.message import MessageSegment
 
 TMS = TypeVar("TMS", bound=MessageSegment)
 P = ParamSpec("P")
 
 
+def _isinstance(self: BasePattern, seg: MessageSegment):
+    return seg if self.pattern == seg.type else None
+
+
 class SegmentPattern(BasePattern[TMS], Generic[TMS, P]):
     def __init__(
         self,
         name: str,
         origin: type[TMS],
         call: Callable[P, TMS],
         additional: Callable[..., bool] | None = None,
@@ -40,24 +44,7 @@
         return input_
 
     def __call__(self, *args: P.args, **kwargs: P.kwargs) -> TMS:
         return self.call(*args, **kwargs)  # type: ignore
 
 
 OutputType = Literal["help", "shortcut", "completion"]
-
-
-def _isinstance(seg: MessageSegment, accepts: set[str]):
-    return seg if seg.type.lower() in accepts else None
-
-
-def gen_unit(
-    name: str, accepts: set[str], additional: Callable[..., bool] | None = None
-) -> BasePattern[MessageSegment]:
-    return BasePattern(
-        name,
-        PatternModel.TYPE_CONVERT,
-        Any,
-        lambda self, x: _isinstance(x, accepts),
-        accepts=[MessageSegment],
-        validators=[additional] if additional else [],
-    )
```

### Comparing `nonebot-plugin-alconna-0.4.0/PKG-INFO` & `nonebot-plugin-alconna-0.4.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-alconna
-Version: 0.4.0
+Version: 0.4.0rc1
 Summary: Alconna Adapter for Nonebot
 License: MIT
 Keywords: command,argparse,cli,alconna,nonebot
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Project-URL: repository, https://github.com/ArcletProject/nonebot-plugin-alconna
 Description-Content-Type: text/markdown
@@ -36,15 +36,14 @@
 ## 特性
 
 - 完整的 Alconna 特性支持
 - 基本的 rule, matcher 与 依赖注入
 - 自动回复命令帮助信息 (help, shortcut, completion) 选项
 - 现有全部协议的 Segment 标注
 - match_value, match_path 等检查函数
-- 补全会话支持
 
 ## 讨论
 
 QQ 交流群: [链接](https://jq.qq.com/?_wv=1027&k=PUPOnCSH)
 
 
 ## 使用方法
@@ -64,70 +63,46 @@
 assert res.matched
 assert res.query("foo.foo") == 123
 assert not alc.parse(Message(["Hello!", img])).matched
 ```
 
 ### MessageSegment 标注
 
-特定适配器:
-
 ```python
 from nonebot_plugin_alconna.adapters.onebot12 import Mention
 from nonebot.adapters.onebot.v12 import Message
 from arclet.alconna import Alconna, Args
 
 msg = Message(["Hello!", Mention("123")])
 print(msg)  # Hello![mention:user_id=123]
 
 alc = Alconna("Hello!", Args["target", Mention])
 res = alc.parse(msg)
 assert res.matched
 assert res.query("target").data['user_id'] == '123'
 ```
 
-通用标注:
-
-```python
-from nonebot.adapters.onebot.v12 import Message as Ob12M, MessageSegment as Ob12MS
-from nonebot.adapters.onebot.v11 import Message as Ob11M, MessageSegment as Ob11MS
-from nonebot_plugin_alconna.adapters import At
-from arclet.alconna import Alconna, Args
-
-msg1 = Ob12M(["Hello!", Ob12MS.mention("123")])
-print(msg1)  # Hello![mention:user_id=123]
-msg2 = Ob11M(["Hello!", Ob11MS.at(123)])
-print(msg2)  # Hello![CQ:at,qq=123]
-
-alc = Alconna("Hello!", Args["target", At])
-res1 = alc.parse(msg1)
-assert res1.matched
-assert res1.query("target").data['user_id'] == '123'
-
-res2 = alc.parse(msg2)
-assert res2.matched
-assert res2.query("target").data['qq'] == 123
-```
-
 ### Matcher 与 依赖注入
 ```python
 ...
 from nonebot import require
 require("nonebot_plugin_alconna")
 ...
 
 from nonebot_plugin_alconna import (
     on_alconna, 
     Match,
     Query,
     AlconnaMatch, 
     AlconnaQuery,
+    AlconnaResult, 
     AlcMatches,
     AlcResult
 )
-from arclet.alconna import Alconna, Args, Option
+from arclet.alconna import Alconna, Args, Arparma, Option
 
 test = on_alconna(
     Alconna(
         "test",
         Option("foo", Args["bar", int]),
         Option("baz", Args["qux", bool, False])
     ),
@@ -177,17 +152,17 @@
     ),
     Subcommand(
         "list",
         Option("--out-dated")
     )
 )
 
-pip_update = on_alconna(pip, [assign("install.pak", "pip")])
-pip_match_install = on_alconna(pip, [assign("install")])
-pip_match_list = on_alconna(pip, [assign("list")])
+pip_update = on_alconna(pip, assign("install.pak", "pip"))
+pip_match_install = on_alconna(pip, assign("install"))
+pip_match_list = on_alconna(pip, assign("list"))
 
 @pip_update.handle()
 async def update(arp: CommandResult = AlconnaResult()):
     ...
 
 @pip_match_list.handle()
 async def list_(arp: CommandResult = AlconnaResult()):
@@ -236,38 +211,33 @@
 
 ## 配置
 
 目前配置项有：
 
 - ALCONNA_AUTO_SEND_OUTPUT : 是否全局启用输出信息自动发送
 - ALCONNA_USE_COMMAND_START : 是否将 COMMAND_START 作为全局命令前缀
-- ALCONNA_AUTO_COMPLETION: 是否全局启用补全会话功能
 
 ## 参数解释
 
 ```python
 def on_alconna(
     command: Alconna | str,
-    checker: list[Callable[[Arparma], bool]] | None = None,
+    *checker: Callable[[Arparma], bool],
     skip_for_unmatch: bool = True,
     auto_send_output: bool = False,
-    output_converter: Callable[[OutputType, str], Message | Awaitable[Message]] | None = None,
-    aliases: set[str | tuple[str, ...]] | None = None,
-    comp_config: CompConfig | None = None,
+    output_converter: Callable[[str], Message | Awaitable[Message]] | None = None,
     **kwargs,
 ) -> type[Matcher]:
 ```
 
 - `command`: Alconna 命令
 - `checker`: 命令解析结果的检查器
 - `skip_for_unmatch`: 是否在命令不匹配时跳过该响应
 - `auto_send_output`: 是否自动发送输出信息并跳过响应
 - `output_converter`: 输出信息字符串转换为 Message 方法
-- `aliases`: 命令别名, 作用类似于 `on_command`
-- `comp_config`: 补全会话配置, 不传入则不启用补全会话
 
 ## 提供了 MessageSegment标注 的协议:
 
 | 协议名称                                                                | 路径                                   |
 |---------------------------------------------------------------------|--------------------------------------|
 | [OneBot 协议](https://onebot.dev/)                                    | adapters.onebot11, adapters.onebot12 |
 | [Telegram](https://core.telegram.org/bots/api)                      | adapters.telegram                    |
```

