# Comparing `tmp/arclet-alconna-1.7.0rc6.tar.gz` & `tmp/arclet-alconna-1.7.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-1.7.0rc6.tar", last modified: Mon May  8 16:34:17 2023, max compression
+gzip compressed data, was "arclet-alconna-1.7.0rc7.tar", last modified: Tue May  9 04:08:31 2023, max compression
```

## Comparing `arclet-alconna-1.7.0rc6.tar` & `arclet-alconna-1.7.0rc7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.0rc6/LICENSE
--rw-r--r--   0        0        0     2813 2023-05-07 16:32:54.439874 arclet-alconna-1.7.0rc6/pyproject.toml
--rw-r--r--   0        0        0     6702 2023-05-08 08:04:29.409891 arclet-alconna-1.7.0rc6/README-EN.md
--rw-r--r--   0        0        0     1087 2023-05-08 16:32:38.530616 arclet-alconna-1.7.0rc6/src/arclet/alconna/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 16:29:22.798529 arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/__init__.py
--rw-r--r--   0        0        0    18070 2023-05-08 06:36:38.138006 arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_analyser.py
--rw-r--r--   0        0        0     8361 2023-05-07 16:29:22.799529 arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_argv.py
--rw-r--r--   0        0        0    22923 2023-05-08 08:02:25.512945 arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_handlers.py
--rw-r--r--   0        0        0     7811 2023-05-08 06:38:21.959747 arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_header.py
--rw-r--r--   0        0        0      837 2023-05-07 16:29:22.801529 arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_util.py
--rw-r--r--   0        0        0     1785 2023-05-08 05:11:19.754526 arclet-alconna-1.7.0rc6/src/arclet/alconna/action.py
--rw-r--r--   0        0        0    14478 2023-05-08 06:44:47.137906 arclet-alconna-1.7.0rc6/src/arclet/alconna/args.py
--rw-r--r--   0        0        0     1243 2023-05-07 16:29:22.804526 arclet-alconna-1.7.0rc6/src/arclet/alconna/argv.py
--rw-r--r--   0        0        0    15913 2023-05-07 16:32:41.201286 arclet-alconna-1.7.0rc6/src/arclet/alconna/arparma.py
--rw-r--r--   0        0        0    12902 2023-05-08 05:22:02.753182 arclet-alconna-1.7.0rc6/src/arclet/alconna/base.py
--rw-r--r--   0        0        0     1889 2023-05-08 06:44:58.844442 arclet-alconna-1.7.0rc6/src/arclet/alconna/builtin.py
--rw-r--r--   0        0        0     4868 2023-05-08 06:45:27.372580 arclet-alconna-1.7.0rc6/src/arclet/alconna/completion.py
--rw-r--r--   0        0        0     4463 2023-05-08 15:45:12.657524 arclet-alconna-1.7.0rc6/src/arclet/alconna/config.py
--rw-r--r--   0        0        0    14858 2023-05-08 12:05:48.939938 arclet-alconna-1.7.0rc6/src/arclet/alconna/core.py
--rw-r--r--   0        0        0     2615 2023-05-07 16:32:47.490076 arclet-alconna-1.7.0rc6/src/arclet/alconna/duplication.py
--rw-r--r--   0        0        0     1070 2023-05-07 16:32:49.003053 arclet-alconna-1.7.0rc6/src/arclet/alconna/exceptions.py
--rw-r--r--   0        0        0    11252 2023-05-08 16:28:22.675096 arclet-alconna-1.7.0rc6/src/arclet/alconna/formatter.py
--rw-r--r--   0        0        0       99 2023-05-07 16:29:22.812601 arclet-alconna-1.7.0rc6/src/arclet/alconna/i18n/.config.json
--rw-r--r--   0        0        0     3565 2023-05-07 16:29:22.813522 arclet-alconna-1.7.0rc6/src/arclet/alconna/i18n/en-US.json
--rw-r--r--   0        0        0     3602 2023-05-07 16:29:22.813850 arclet-alconna-1.7.0rc6/src/arclet/alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0    16838 2023-05-08 06:47:44.520450 arclet-alconna-1.7.0rc6/src/arclet/alconna/manager.py
--rw-r--r--   0        0        0     1430 2023-05-07 16:32:50.831111 arclet-alconna-1.7.0rc6/src/arclet/alconna/model.py
--rw-r--r--   0        0        0     1943 2023-05-07 16:32:51.478127 arclet-alconna-1.7.0rc6/src/arclet/alconna/model.pyi
--rw-r--r--   0        0        0     3940 2023-05-07 16:32:52.687122 arclet-alconna-1.7.0rc6/src/arclet/alconna/output.py
--rw-r--r--   0        0        0        0 2023-05-07 16:29:22.816522 arclet-alconna-1.7.0rc6/src/arclet/alconna/py.typed
--rw-r--r--   0        0        0     5813 2023-05-07 16:32:58.355410 arclet-alconna-1.7.0rc6/src/arclet/alconna/stub.py
--rw-r--r--   0        0        0     3584 2023-05-07 16:32:58.778521 arclet-alconna-1.7.0rc6/src/arclet/alconna/typing.py
--rw-r--r--   0        0        0     3254 2023-05-08 06:48:40.755418 arclet-alconna-1.7.0rc6/tests/analyser_test.py
--rw-r--r--   0        0        0     7223 2023-05-07 16:29:22.820523 arclet-alconna-1.7.0rc6/tests/args_test.py
--rw-r--r--   0        0        0     2167 2023-05-07 16:32:42.508980 arclet-alconna-1.7.0rc6/tests/base_test.py
--rw-r--r--   0        0        0     3113 2023-05-08 06:49:11.411375 arclet-alconna-1.7.0rc6/tests/components_test.py
--rw-r--r--   0        0        0     1199 2023-05-07 16:29:22.822522 arclet-alconna-1.7.0rc6/tests/config_test.py
--rw-r--r--   0        0        0    23213 2023-05-08 06:49:45.049528 arclet-alconna-1.7.0rc6/tests/core_test.py
--rw-r--r--   0        0        0      505 2023-05-07 16:29:22.823526 arclet-alconna-1.7.0rc6/tests/util_test.py
--rw-r--r--   0        0        0     7366 1970-01-01 00:00:00.000000 arclet-alconna-1.7.0rc6/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.0rc7/LICENSE
+-rw-r--r--   0        0        0     2813 2023-05-07 16:32:54.439874 arclet-alconna-1.7.0rc7/pyproject.toml
+-rw-r--r--   0        0        0     6702 2023-05-08 08:04:29.409891 arclet-alconna-1.7.0rc7/README-EN.md
+-rw-r--r--   0        0        0     1087 2023-05-09 04:08:23.241662 arclet-alconna-1.7.0rc7/src/arclet/alconna/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 16:29:22.798529 arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/__init__.py
+-rw-r--r--   0        0        0    18068 2023-05-09 02:30:18.661298 arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_analyser.py
+-rw-r--r--   0        0        0     8454 2023-05-09 02:55:46.376874 arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_argv.py
+-rw-r--r--   0        0        0    23058 2023-05-09 03:22:21.186877 arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_handlers.py
+-rw-r--r--   0        0        0     7811 2023-05-08 06:38:21.959747 arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_header.py
+-rw-r--r--   0        0        0      837 2023-05-07 16:29:22.801529 arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_util.py
+-rw-r--r--   0        0        0     1785 2023-05-08 05:11:19.754526 arclet-alconna-1.7.0rc7/src/arclet/alconna/action.py
+-rw-r--r--   0        0        0    14478 2023-05-08 06:44:47.137906 arclet-alconna-1.7.0rc7/src/arclet/alconna/args.py
+-rw-r--r--   0        0        0     1435 2023-05-08 17:20:30.396974 arclet-alconna-1.7.0rc7/src/arclet/alconna/argv.py
+-rw-r--r--   0        0        0    15913 2023-05-07 16:32:41.201286 arclet-alconna-1.7.0rc7/src/arclet/alconna/arparma.py
+-rw-r--r--   0        0        0    12902 2023-05-08 05:22:02.753182 arclet-alconna-1.7.0rc7/src/arclet/alconna/base.py
+-rw-r--r--   0        0        0     1889 2023-05-08 06:44:58.844442 arclet-alconna-1.7.0rc7/src/arclet/alconna/builtin.py
+-rw-r--r--   0        0        0     4872 2023-05-09 02:30:18.674447 arclet-alconna-1.7.0rc7/src/arclet/alconna/completion.py
+-rw-r--r--   0        0        0     4463 2023-05-08 15:45:12.657524 arclet-alconna-1.7.0rc7/src/arclet/alconna/config.py
+-rw-r--r--   0        0        0    14858 2023-05-08 12:05:48.939938 arclet-alconna-1.7.0rc7/src/arclet/alconna/core.py
+-rw-r--r--   0        0        0     2615 2023-05-07 16:32:47.490076 arclet-alconna-1.7.0rc7/src/arclet/alconna/duplication.py
+-rw-r--r--   0        0        0     1070 2023-05-07 16:32:49.003053 arclet-alconna-1.7.0rc7/src/arclet/alconna/exceptions.py
+-rw-r--r--   0        0        0    11252 2023-05-08 16:28:22.675096 arclet-alconna-1.7.0rc7/src/arclet/alconna/formatter.py
+-rw-r--r--   0        0        0       99 2023-05-07 16:29:22.812601 arclet-alconna-1.7.0rc7/src/arclet/alconna/i18n/.config.json
+-rw-r--r--   0        0        0     3565 2023-05-07 16:29:22.813522 arclet-alconna-1.7.0rc7/src/arclet/alconna/i18n/en-US.json
+-rw-r--r--   0        0        0     3602 2023-05-07 16:29:22.813850 arclet-alconna-1.7.0rc7/src/arclet/alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0    16956 2023-05-08 17:23:28.473144 arclet-alconna-1.7.0rc7/src/arclet/alconna/manager.py
+-rw-r--r--   0        0        0     1430 2023-05-07 16:32:50.831111 arclet-alconna-1.7.0rc7/src/arclet/alconna/model.py
+-rw-r--r--   0        0        0     1943 2023-05-07 16:32:51.478127 arclet-alconna-1.7.0rc7/src/arclet/alconna/model.pyi
+-rw-r--r--   0        0        0     3940 2023-05-07 16:32:52.687122 arclet-alconna-1.7.0rc7/src/arclet/alconna/output.py
+-rw-r--r--   0        0        0        0 2023-05-07 16:29:22.816522 arclet-alconna-1.7.0rc7/src/arclet/alconna/py.typed
+-rw-r--r--   0        0        0     5813 2023-05-07 16:32:58.355410 arclet-alconna-1.7.0rc7/src/arclet/alconna/stub.py
+-rw-r--r--   0        0        0     3584 2023-05-07 16:32:58.778521 arclet-alconna-1.7.0rc7/src/arclet/alconna/typing.py
+-rw-r--r--   0        0        0     3254 2023-05-08 06:48:40.755418 arclet-alconna-1.7.0rc7/tests/analyser_test.py
+-rw-r--r--   0        0        0     7223 2023-05-07 16:29:22.820523 arclet-alconna-1.7.0rc7/tests/args_test.py
+-rw-r--r--   0        0        0     2167 2023-05-07 16:32:42.508980 arclet-alconna-1.7.0rc7/tests/base_test.py
+-rw-r--r--   0        0        0     3113 2023-05-08 06:49:11.411375 arclet-alconna-1.7.0rc7/tests/components_test.py
+-rw-r--r--   0        0        0     1199 2023-05-07 16:29:22.822522 arclet-alconna-1.7.0rc7/tests/config_test.py
+-rw-r--r--   0        0        0    23219 2023-05-09 02:35:51.817251 arclet-alconna-1.7.0rc7/tests/core_test.py
+-rw-r--r--   0        0        0      505 2023-05-07 16:29:22.823526 arclet-alconna-1.7.0rc7/tests/util_test.py
+-rw-r--r--   0        0        0     7366 1970-01-01 00:00:00.000000 arclet-alconna-1.7.0rc7/PKG-INFO
```

### Comparing `arclet-alconna-1.7.0rc6/LICENSE` & `arclet-alconna-1.7.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/pyproject.toml` & `arclet-alconna-1.7.0rc7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
-version = "1.7.0rc6"
+version = "1.7.0rc7"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://arcletproject.github.io/docs/alconna/tutorial"
 repository = "https://github.com/ArcletProject/Alconna"
```

### Comparing `arclet-alconna-1.7.0rc6/README-EN.md` & `arclet-alconna-1.7.0rc7/README-EN.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/__init__.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 from .builtin import set_default
 from .model import OptionResult, SubcommandResult, HeadResult
 from .output import output_manager
 from .formatter import TextFormatter
 from .duplication import Duplication
 from .stub import ArgsStub, OptionStub, SubcommandStub
 
-__version__ = "1.7.0rc6"
+__version__ = "1.7.0rc7"
 
 # backward compatibility
 Arpamar = Arparma
 DataCollectionContainer = Argv
```

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_analyser.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_analyser.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
                 data_index += 1
             elif mat := re.search(r"\{\*(.*)\}", unit, re.DOTALL):
                 sep = mat[1]
                 argv.raw_data[i] = unit.replace(f"{{*{sep}}}", (sep or ' ').join(map(str, data)))
                 data.clear()
 
         argv.bak_data = argv.raw_data.copy()
-        argv.addon(*data).addon(*short.get('args', []))
+        argv.addon(data).addon(short.get('args', []))
         if reg:
             groups: tuple[str, ...] = reg.groups()
             gdict: dict[str, str] = reg.groupdict()
             for j, unit in enumerate(argv.raw_data):
                 if not isinstance(unit, str):
                     continue
                 for i, c in enumerate(groups):
```

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_argv.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_argv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field, InitVar
-from typing import Any, Callable, Generic, ClassVar
+from typing import Any, Callable, Generic, ClassVar, Iterable
 from typing_extensions import Self
 from tarina import split, split_once, lang
 
 from ..args import Arg
 from ..config import Namespace, config
 from ..base import Option, Subcommand
 from ..exceptions import NullMessage
@@ -125,27 +125,29 @@
             raise NullMessage(lang.require("argv", "null_message").format(target=data))
         self.ndata = i
         self.bak_data = raw_data.copy()
         if self.message_cache:
             self.token = self.generate_token(raw_data)
         return self
 
-    def addon(self, *data: str | Any) -> Self:
+    def addon(self, data: Iterable[str | Any]) -> Self:
         """添加命令元素
 
         Args:
-            *data (str | Any): 命令元素
+            data (Iterable[str | Any]): 命令元素
 
         Returns:
             Self: 自身
         """
         self.raw_data = self.bak_data.copy()
         for i, d in enumerate(data):
             if not d:
                 continue
+            if res := self.to_text(d):
+                d = res
             if isinstance(d, str) and i > 0 and isinstance(self.raw_data[-1], str):
                 self.raw_data[-1] += f"{self.separators[0]}{d}"
             else:
                 self.raw_data.append(d)
                 self.ndata += 1
         self.current_index = 0
         self.bak_data = self.raw_data.copy()
```

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_handlers.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,18 @@
                     )
                 analyse_option(analyser, argv, param)
             else:
                 if param.command.requires and analyser.sentences != param.command.requires:
                     return lang.require("subcommand", "require_error").format(
                         source=param.command.name, target=' '.join(analyser.sentences)
                     )
-                analyser.subcommands_result[param.command.dest] = param.process(argv).result()
+                try:
+                    param.process(argv)
+                finally:
+                    analyser.subcommands_result[param.command.dest] = param.result()
             _data.clear()
             return True
         except ParamsUnmatched as e:
             if argv.context.__class__ is Arg:
                 raise e
             argv.data_reset(_data, _index)
 
@@ -426,15 +429,18 @@
     elif _param is not None:
         if _param.command.requires and analyser.sentences != _param.command.requires:
             raise ParamsUnmatched(
                 lang.require("subcommand", "require_error").format(
                     source=_param.command.name, target=' '.join(analyser.sentences)
                 )
             )
-        analyser.subcommands_result[_param.command.dest] = _param.process(argv).result()
+        try:
+            _param.process(argv)
+        finally:
+            analyser.subcommands_result[_param.command.dest] = _param.result()
     else:
         raise TerminateLoop(str(_text))
     analyser.sentences.clear()
     argv.context = None
 
 
 def analyse_header(header: Header, argv: Argv) -> HeadResult:
```

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_header.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_header.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/_internal/_util.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/_internal/_util.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/action.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/action.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/args.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/args.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/argv.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/argv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from __future__ import annotations
 
+from contextvars import ContextVar
 from typing import Any, Callable
 
 from .typing import TDC
 from ._internal._argv import Argv
 
-__argv_type__ = Argv
+__argv_type__: ContextVar[type[Argv]] = ContextVar("argv_type", default=Argv)
 
 
 def set_default_argv_type(argv_type: type[Argv]):
     """设置默认的命令行参数类型"""
-    global __argv_type__
-    __argv_type__ = argv_type
+    __argv_type__.set(argv_type)
 
 
 def argv_config(
+    target: type[Argv] | None = None,
     preprocessors: dict[str, Callable[..., Any]] | None = None,
     to_text: Callable[[Any], str | None] | None = None,
     filter_out: list[str] | None = None,
     checker: Callable[[Any], bool] | None = None,
     converter: Callable[[str | list], TDC] | None = None
 ):
     """配置命令行参数
 
     Args:
+        target (type[Argv] | None, optional): 目标命令类型.
         preprocessors (dict[str, Callable[..., Any]] | None, optional): 命令元素的预处理器.
         to_text (Callable[[Any], str | None] | None, optional): 将命令元素转换为文本, 或者返回None以跳过该元素.
         filter_out (list[str] | None, optional): 需要过滤掉的命令元素.
         checker (Callable[[Any], bool] | None, optional): 检查传入命令.
         converter (Callable[[str | list], TDC] | None, optional): 将字符串或列表转为目标命令类型.
     """
-    Argv._cache.setdefault(__argv_type__, {}).update(locals())
+    Argv._cache.setdefault(target or __argv_type__.get(), {}).update(locals())
```

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/arparma.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/arparma.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/base.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/base.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/builtin.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/builtin.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/completion.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,19 +81,19 @@
         """
         if not self.prompts:
             raise ValueError("No prompt available.")
         self.index += offset
         self.index %= len(self.prompts)
         return self.prompts[self.index].text
 
-    def enter(self, content: Any | None = None):
+    def enter(self, content: list | None = None):
         """确认当前补全选项。
 
         Args:
-            content (Any, optional): 补全选项的内容。不传入则使用当前选中的补全选项文本
+            content (list, optional): 补全选项的内容。不传入则使用当前选中的补全选项文本
 
         Returns:
             Any: 补全后执行的结果。
 
         Raises:
             ValueError: 当前没有可用的补全选项, 或者当前补全选项不可用。
         """
@@ -108,15 +108,15 @@
         if not prompt.can_use:
             raise ValueError("This prompt cannot be used.")
         if prompt.removal_prefix:
             last = argv.bak_data[-1]
             argv.bak_data[-1] = last[
                 : last.rfind(prompt.removal_prefix)
             ]
-        argv.addon(prompt.text)
+        argv.addon([prompt.text])
         self.clear()
         return self.source.process(argv)
 
     def push(self, *suggests: Prompt):
         """添加补全选项。
 
         Args:
```

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/config.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/config.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/core.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/core.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/duplication.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/duplication.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/exceptions.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/exceptions.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/formatter.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/formatter.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/i18n/en-US.json` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/i18n/en-US.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/i18n/zh-CN.json` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/i18n/zh-CN.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/manager.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,22 +124,22 @@
         return config.namespaces.get(name)
 
     def register(self, command: Alconna) -> None:
         """注册命令解析器, 会同时记录解析器对应的命令"""
         if self.current_count >= self.max_count:
             raise ExceedMaxCount
         self.__argv.pop(command, None)
-        self.__argv[command] = __argv_type__(
-            command.namespace_config,
-            fuzzy_match=command.meta.fuzzy_match,
-            to_text=command.namespace_config.to_text,
-            converter=command.namespace_config.converter,
-            separators=command.separators,
-            message_cache=command.namespace_config.enable_message_cache,
-            filter_crlf=not command.meta.keep_crlf,
+        self.__argv[command] = __argv_type__.get()(
+            command.namespace_config,  # type: ignore
+            fuzzy_match=command.meta.fuzzy_match,  # type: ignore
+            to_text=command.namespace_config.to_text,  # type: ignore
+            converter=command.namespace_config.converter,  # type: ignore
+            separators=command.separators,  # type: ignore
+            message_cache=command.namespace_config.enable_message_cache,  # type: ignore
+            filter_crlf=not command.meta.keep_crlf,  # type: ignore
         )
         self.__analysers.pop(command, None)
         self.__analysers[command] = command.compile(None)
         namespace = self.__commands.setdefault(command.namespace, WeakValueDictionary())
         if _cmd := namespace.get(command.name):
             if _cmd == command:
                 return
```

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/model.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/model.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/model.pyi` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/model.pyi`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/output.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/output.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/stub.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/stub.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/src/arclet/alconna/typing.py` & `arclet-alconna-1.7.0rc7/src/arclet/alconna/typing.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/tests/analyser_test.py` & `arclet-alconna-1.7.0rc7/tests/analyser_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/tests/args_test.py` & `arclet-alconna-1.7.0rc7/tests/args_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/tests/base_test.py` & `arclet-alconna-1.7.0rc7/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/tests/components_test.py` & `arclet-alconna-1.7.0rc7/tests/components_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/tests/config_test.py` & `arclet-alconna-1.7.0rc7/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc6/tests/core_test.py` & `arclet-alconna-1.7.0rc7/tests/core_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,25 +473,25 @@
     print("\n", "interface [pending]:")
     with CompSession(alc21) as comp:
         alc21.parse("core21")
     if comp.available:
         print("\n", "current completion:", comp.current())
         print("\n", "next completion:", comp.tab())
         with comp:
-            comp.enter("1")
+            comp.enter(["1"])
         print("\n", "current completion:", comp.current())
-        assert comp.enter("a").matched
+        assert comp.enter(["a"]).matched
 
     with CompSession(alc21) as comp:
         alc21.parse("core21 1 a --comp")
     if comp.available:
         print(comp)
         comp.tab()
         print(comp)
-        assert not comp.enter("-h").matched
+        assert not comp.enter(["-h"]).matched
 
 
 def test_call():
 
     alc22 = Alconna("core22", Args.foo[int], Args.bar[str])
     alc22("core22 123 abc")
```

### Comparing `arclet-alconna-1.7.0rc6/PKG-INFO` & `arclet-alconna-1.7.0rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna
-Version: 1.7.0rc6
+Version: 1.7.0rc7
 Summary: A High-performance, Generality, Humane Command Line Arguments Parser Library.
 License: MIT
 Keywords: command,argparse,fast,alconna,cli,command-line,parsing,optparse
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

