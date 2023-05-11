# Comparing `tmp/arclet-alconna-ichika-0.13.0rc2.tar.gz` & `tmp/arclet-alconna-ichika-0.13.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-ichika-0.13.0rc2.tar", last modified: Tue May  9 04:37:11 2023, max compression
+gzip compressed data, was "arclet-alconna-ichika-0.13.0rc3.tar", last modified: Wed May 10 05:58:55 2023, max compression
```

## Comparing `arclet-alconna-ichika-0.13.0rc2.tar` & `arclet-alconna-ichika-0.13.0rc3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-ichika-0.13.0rc2/LICENSE
--rw-r--r--   0        0        0     6194 2023-05-09 04:32:45.106719 arclet-alconna-ichika-0.13.0rc2/pyproject.toml
--rw-r--r--   0        0        0     7138 2023-01-30 09:01:24.879470 arclet-alconna-ichika-0.13.0rc2/README.md
--rw-r--r--   0        0        0       80 2023-05-09 04:08:01.631055 arclet-alconna-ichika-0.13.0rc2/src/arclet/alconna/ichika/__init__.py
--rw-r--r--   0        0        0     6127 2023-05-09 04:36:47.494072 arclet-alconna-ichika-0.13.0rc2/src/arclet/alconna/ichika/adapter.py
--rw-r--r--   0        0        0     1256 2023-05-09 04:21:37.796354 arclet-alconna-ichika-0.13.0rc2/src/arclet/alconna/ichika/typings.py
--rw-r--r--   0        0        0     7591 1970-01-01 00:00:00.000000 arclet-alconna-ichika-0.13.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-ichika-0.13.0rc3/LICENSE
+-rw-r--r--   0        0        0     6194 2023-05-09 08:40:44.827327 arclet-alconna-ichika-0.13.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     7395 2023-05-10 05:58:09.949751 arclet-alconna-ichika-0.13.0rc3/README.md
+-rw-r--r--   0        0        0       80 2023-05-09 04:08:01.631055 arclet-alconna-ichika-0.13.0rc3/src/arclet/alconna/ichika/__init__.py
+-rw-r--r--   0        0        0     6369 2023-05-09 09:28:21.208364 arclet-alconna-ichika-0.13.0rc3/src/arclet/alconna/ichika/adapter.py
+-rw-r--r--   0        0        0     1256 2023-05-09 04:21:37.796354 arclet-alconna-ichika-0.13.0rc3/src/arclet/alconna/ichika/typings.py
+-rw-r--r--   0        0        0     7838 1970-01-01 00:00:00.000000 arclet-alconna-ichika-0.13.0rc3/PKG-INFO
```

### Comparing `arclet-alconna-ichika-0.13.0rc2/LICENSE` & `arclet-alconna-ichika-0.13.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ichika-0.13.0rc2/pyproject.toml` & `arclet-alconna-ichika-0.13.0rc3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arclet-alconna-ichika"
-version = "0.13.0rc2"
+version = "0.13.0rc3"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "ichika>=0.0.5",
 ]
 description = "Support Alconna to BlueGlassBlock/Ichika"
@@ -56,15 +56,15 @@
 [tool.mina.packages.core]
 includes = [
     "src/arclet/alconna/graia",
 ]
 
 [tool.mina.packages.core.project]
 name = "arclet-alconna-graia"
-version = "0.13.0rc2"
+version = "0.13.0rc3"
 description = "Support Alconna to GraiaProject"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -108,20 +108,20 @@
 alconna_behavior = "arclet.alconna.graia.create:AlconnaBehaviorCreator"
 
 [tool.mina.packages.ariadne]
 includes = [
     "src/arclet/alconna/ariadne",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.13.0, >= 0.13.0rc2",
+    "arclet-alconna-graia<0.13.0, >= 0.13.0rc3",
 ]
 
 [tool.mina.packages.ariadne.project]
 name = "arclet-alconna-ariadne"
-version = "0.13.0rc2"
+version = "0.13.0rc3"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "graia-ariadne<1.0.0, >=0.7.14",
 ]
 description = "Support Alconna to GraiaProject/Ariadne"
@@ -149,20 +149,20 @@
 repository = "https://github.com/ArcletProject/Alconna-Graia"
 
 [tool.mina.packages.avilla]
 includes = [
     "src/arclet/alconna/avilla",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.13.0, >= 0.13.0rc2",
+    "arclet-alconna-graia<0.13.0, >= 0.13.0rc3",
 ]
 
 [tool.mina.packages.avilla.project]
 name = "arclet-alconna-avilla"
-version = "0.13.0rc2"
+version = "0.13.0rc3"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "avilla-core>=1.0.0a5",
 ]
 description = "Support Alconna to GraiaProject/Avilla"
@@ -191,20 +191,20 @@
 repository = "https://github.com/ArcletProject/Alconna-Graia"
 
 [tool.mina.packages.ichika]
 includes = [
     "src/arclet/alconna/ichika",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.13.0, >= 0.13.0rc2",
+    "arclet-alconna-graia<0.13.0, >= 0.13.0rc3",
 ]
 
 [tool.mina.packages.ichika.project]
 name = "arclet-alconna-ichika"
-version = "0.13.0rc2"
+version = "0.13.0rc3"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "ichika>=0.0.5",
 ]
 description = "Support Alconna to BlueGlassBlock/Ichika"
```

### Comparing `arclet-alconna-ichika-0.13.0rc2/README.md` & `arclet-alconna-ichika-0.13.0rc3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,21 @@
 或
 
 ```shell
 pip install arclet-alconna-graia, arclet-alconna-avilla
 pdm add arclet-alconna-graia, arclet-alconna-avilla
 ```
 
+或
+
+```shell
+pip install arclet-alconna-graia, arclet-alconna-ichika
+pdm add arclet-alconna-graia, arclet-alconna-ichika
+```
+
 ## 前提
 
 Alconna-Graia 现在依赖 `Launart` 的 `service` 功能
 
 你需要在你使用 Alconna-Graia 组件时加入如下代码：
 
 ```python
@@ -170,15 +177,15 @@
 
 @alcommand(Alconna("!jrrp", Args["sth", str, 1123]), private=False)
 async def test1(result: Arpamar, sth: Match[str]):
     print("sign:", result)
     print("match", sth.available, sth.result)
 
 
-@alcommand("[!|.]hello <name:str>;say <word>", send_error=True)
+@alcommand("[!|.]hello <name:str>", send_error=True)
 async def test1(result: Arpamar, name: Match[str]):
     print("sign:", result)
     print("match", name.available, name.result)
 
     
 @listen(...) 
 @from_command("foo bar {baz}")
@@ -216,27 +223,30 @@
 class AlconnaDispatcher(BaseDispatcher, Generic[TOHandler]):
     def __init__(
         self,
         command: Alconna | AlconnaGroup,
         *,
         send_flag: Literal["reply", "post", "stay"] = "stay",
         skip_for_unmatch: bool = True,
-        message_converter: Callable[[str], MessageChain | Coroutine[Any, Any, MessageChain]] | None = None,
+        comp_session: Optional[CompConfig] = None,
+        message_converter: Callable[[OutType, str], MessageChain | Coroutine[Any, Any, MessageChain]] | None = None,
     ): ...
 ```
 
 `command`: 使用的 Alconna 指令
 
 `send_flag`: 解析期间输出信息的发送方式
 - reply: 直接发送给指令发送者
 - post: 以事件通过 Broadcast 广播
 - stay: 存入 AlconnaProperty 传递给事件处理器
 
 `skip_for_unmatch`: 解析失败时是否跳过, 否则错误信息按 send_flag 处理
 
+`comp_session`: 补全会话配置, 不传入则不启用补全会话
+
 `message_converter`: send_flag 为 reply 时 输出信息的预处理器
 
 ## 附加组件
 
 - `Match`: 查询某个参数是否匹配，如`foo: Match[int]`。使用时以 `Match.available` 判断是否匹配成功，以
 `Match.result` 获取匹配结果
```

### Comparing `arclet-alconna-ichika-0.13.0rc2/src/arclet/alconna/ichika/adapter.py` & `arclet-alconna-ichika-0.13.0rc3/src/arclet/alconna/ichika/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from __future__ import annotations
 
 from contextlib import suppress
 from typing import Any, Callable, Iterable
 
-from graia.broadcast.interrupt import Waiter
-from ichika.client import Client
-from ichika.graia import IchikaClientDispatcher, CLIENT_INSTANCE
-from ichika.graia.event import GroupMessage, FriendMessage, MessageEvent
-from ichika.message.elements import At, Text
-from ichika.core import Friend
 from graia.amnesia.message import MessageChain
 from graia.broadcast.builtin.decorators import Depend
 from graia.broadcast.exceptions import ExecutionStop
 from graia.broadcast.interfaces.dispatcher import DispatcherInterface
-from graia.broadcast.utilles import run_always_await, dispatcher_mixin_handler, T_Dispatcher
+from graia.broadcast.interrupt import Waiter
+from graia.broadcast.utilles import (
+    T_Dispatcher,
+    dispatcher_mixin_handler,
+    run_always_await,
+)
+from ichika.client import Client
+from ichika.core import Friend
+from ichika.graia import CLIENT_INSTANCE, IchikaClientDispatcher
+from ichika.graia.event import FriendMessage, GroupMessage, MessageEvent
+from ichika.message.elements import At, Text
 
 from arclet.alconna import Arparma, argv_config
+from arclet.alconna.exceptions import SpecialOptionTriggered
 
 from ..graia import AlconnaProperty, AlconnaSchema
-from ..graia.argv import MessageChainArgv
 from ..graia.adapter import AlconnaGraiaAdapter
+from ..graia.argv import MessageChainArgv
 from ..graia.dispatcher import AlconnaDispatcher, AlconnaOutputMessage
 from ..graia.model import TSource
 from ..graia.utils import listen
 
 AlconnaDispatcher.default_send_handler = lambda x: MessageChain([Text(x)])
 
 
@@ -72,15 +77,19 @@
                 return AlconnaProperty(result, None, source)
             cache.clear()
             cache.add(dispatcher.command)
         if dispatcher.send_flag == "stay":
             return AlconnaProperty(result, output_text, source)
         if dispatcher.send_flag == "reply":
             client: Client = CLIENT_INSTANCE.get()
-            help_message: MessageChain = await run_always_await(dispatcher.converter, output_text)
+            help_message: MessageChain = await run_always_await(
+                dispatcher.converter,
+                str(result.error_info) if isinstance(result.error_info, SpecialOptionTriggered) else "help",
+                output_text
+            )
             if isinstance(source, GroupMessage):
                 await client.send_group_message(source.group.uin, help_message)
             else:
                 await client.send_friend_message(source.sender.uin, help_message)  # type: ignore
         elif dispatcher.send_flag == "post":
             with suppress(LookupError):
                 interface = DispatcherInterface.ctx.get()
```

### Comparing `arclet-alconna-ichika-0.13.0rc2/src/arclet/alconna/ichika/typings.py` & `arclet-alconna-ichika-0.13.0rc3/src/arclet/alconna/ichika/typings.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ichika-0.13.0rc2/PKG-INFO` & `arclet-alconna-ichika-0.13.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-ichika
-Version: 0.13.0rc2
+Version: 0.13.0rc3
 Summary: Support Alconna to BlueGlassBlock/Ichika
 License: AGPL-3.0
 Keywords: alconna,graia,arclet,ichika
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -32,14 +32,21 @@
 或
 
 ```shell
 pip install arclet-alconna-graia, arclet-alconna-avilla
 pdm add arclet-alconna-graia, arclet-alconna-avilla
 ```
 
+或
+
+```shell
+pip install arclet-alconna-graia, arclet-alconna-ichika
+pdm add arclet-alconna-graia, arclet-alconna-ichika
+```
+
 ## 前提
 
 Alconna-Graia 现在依赖 `Launart` 的 `service` 功能
 
 你需要在你使用 Alconna-Graia 组件时加入如下代码：
 
 ```python
@@ -188,15 +195,15 @@
 
 @alcommand(Alconna("!jrrp", Args["sth", str, 1123]), private=False)
 async def test1(result: Arpamar, sth: Match[str]):
     print("sign:", result)
     print("match", sth.available, sth.result)
 
 
-@alcommand("[!|.]hello <name:str>;say <word>", send_error=True)
+@alcommand("[!|.]hello <name:str>", send_error=True)
 async def test1(result: Arpamar, name: Match[str]):
     print("sign:", result)
     print("match", name.available, name.result)
 
     
 @listen(...) 
 @from_command("foo bar {baz}")
@@ -234,27 +241,30 @@
 class AlconnaDispatcher(BaseDispatcher, Generic[TOHandler]):
     def __init__(
         self,
         command: Alconna | AlconnaGroup,
         *,
         send_flag: Literal["reply", "post", "stay"] = "stay",
         skip_for_unmatch: bool = True,
-        message_converter: Callable[[str], MessageChain | Coroutine[Any, Any, MessageChain]] | None = None,
+        comp_session: Optional[CompConfig] = None,
+        message_converter: Callable[[OutType, str], MessageChain | Coroutine[Any, Any, MessageChain]] | None = None,
     ): ...
 ```
 
 `command`: 使用的 Alconna 指令
 
 `send_flag`: 解析期间输出信息的发送方式
 - reply: 直接发送给指令发送者
 - post: 以事件通过 Broadcast 广播
 - stay: 存入 AlconnaProperty 传递给事件处理器
 
 `skip_for_unmatch`: 解析失败时是否跳过, 否则错误信息按 send_flag 处理
 
+`comp_session`: 补全会话配置, 不传入则不启用补全会话
+
 `message_converter`: send_flag 为 reply 时 输出信息的预处理器
 
 ## 附加组件
 
 - `Match`: 查询某个参数是否匹配，如`foo: Match[int]`。使用时以 `Match.available` 判断是否匹配成功，以
 `Match.result` 获取匹配结果
```

