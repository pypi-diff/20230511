# Comparing `tmp/arclet-alconna-tools-0.6.0.tar.gz` & `tmp/arclet-alconna-tools-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-tools-0.6.0.tar", last modified: Thu May 11 05:50:17 2023, max compression
+gzip compressed data, was "arclet-alconna-tools-0.6.0rc1.tar", last modified: Mon May  8 16:36:19 2023, max compression
```

## Comparing `arclet-alconna-tools-0.6.0.tar` & `arclet-alconna-tools-0.6.0rc1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 arclet-alconna-tools-0.6.0/LICENSE
--rw-r--r--   0        0        0     1075 2023-05-10 15:10:24.655658 arclet-alconna-tools-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      749 2023-05-10 16:28:11.249182 arclet-alconna-tools-0.6.0/README.md
--rw-r--r--   0        0        0      387 2023-05-10 14:13:40.054086 arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/__init__.py
--rw-r--r--   0        0        0     2355 2023-05-08 11:53:03.567259 arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/actions.py
--rw-r--r--   0        0        0      866 2023-05-07 05:15:13.324038 arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/checker.py
--rw-r--r--   0        0        0       96 2023-05-08 11:53:03.585160 arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/config.py
--rw-r--r--   0        0        0    27790 2023-05-10 15:20:00.955959 arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/construct.py
--rw-r--r--   0        0        0     3879 2023-05-07 05:15:13.335037 arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/debug.py
--rw-r--r--   0        0        0    17620 2023-05-10 14:36:13.901208 arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/formatter.py
--rw-r--r--   0        0        0       26 2023-05-08 11:44:10.335552 arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/i18n/.config.json
--rw-r--r--   0        0        0      692 2023-05-08 16:08:05.985424 arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/i18n/en-US.json
--rw-r--r--   0        0        0      661 2023-05-08 16:18:05.842731 arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/i18n/zh-CN.json
--rw-r--r--   0        0        0     4453 2023-05-07 05:35:56.817434 arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/pattern.py
--rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 arclet-alconna-tools-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 arclet-alconna-tools-0.6.0rc1/LICENSE
+-rw-r--r--   0        0        0     1081 2023-05-08 16:35:08.337284 arclet-alconna-tools-0.6.0rc1/pyproject.toml
+-rw-r--r--   0        0        0       53 2022-09-16 06:41:48.807371 arclet-alconna-tools-0.6.0rc1/README.md
+-rw-r--r--   0        0        0      391 2023-05-08 11:53:03.576121 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/__init__.py
+-rw-r--r--   0        0        0     2355 2023-05-08 11:53:03.567259 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/actions.py
+-rw-r--r--   0        0        0      866 2023-05-07 05:15:13.324038 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/checker.py
+-rw-r--r--   0        0        0       96 2023-05-08 11:53:03.585160 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/config.py
+-rw-r--r--   0        0        0    27100 2023-05-08 15:07:41.119518 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/construct.py
+-rw-r--r--   0        0        0     3879 2023-05-07 05:15:13.335037 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/debug.py
+-rw-r--r--   0        0        0    17495 2023-05-08 16:19:03.896293 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/formatter.py
+-rw-r--r--   0        0        0       26 2023-05-08 11:44:10.335552 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/i18n/.config.json
+-rw-r--r--   0        0        0      692 2023-05-08 16:08:05.985424 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/i18n/en-US.json
+-rw-r--r--   0        0        0      661 2023-05-08 16:18:05.842731 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/i18n/zh-CN.json
+-rw-r--r--   0        0        0     4453 2023-05-07 05:35:56.817434 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/pattern.py
+-rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 arclet-alconna-tools-0.6.0rc1/PKG-INFO
```

### Comparing `arclet-alconna-tools-0.6.0/LICENSE` & `arclet-alconna-tools-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.0/pyproject.toml` & `arclet-alconna-tools-0.6.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "arclet-alconna-tools"
-version = "0.6.0"
+version = "0.6.0rc1"
 description = "Builtin Tools for Alconna"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "nepattern<0.6.0, >=0.5.0",
-    "arclet-alconna>=1.7.0",
+    "arclet-alconna>=1.7.0rc6",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/actions.py` & `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/actions.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/checker.py` & `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/checker.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/construct.py` & `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/construct.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,20 +425,14 @@
         for p in re.findall(r"\[(.+?)]", _others):
             res = re.split("[:=]", p)
             res[0] = f"{res[0]};?"
             arg.append(res)
         return arg
 
     def __init__(self, command: str, help_text: Optional[str] = None):
-        """创建 AlconnaString
-
-        Args:
-            command (str): 命令字符串, 例如 `test <message:str:hello> #HELP_STRING`
-            help_text (Optional[str], optional): 选填的命令的帮助文本.
-        """
         self.buffer = {}
         self.options = []
         self.meta = CommandMeta(description=help_text, fuzzy_match=True)
         head, others = split_once(command, (" ",))
         if mat := re.match(r"^\[(.+?)]$", head):
             self.buffer["prefixes"] = mat[1].split("|")
         else:
@@ -446,22 +440,14 @@
         args = self.args_gen(others)
         if help_string := re.findall(r"(?: )#(.+)$", others):  # noqa
             self.meta.description = help_string[0]
         custom_types = getattr(inspect.getmodule(inspect.stack()[1][0]), "__dict__", {})
         self.buffer["main_args"] = args_from_list(args, custom_types.copy())
 
     def option(self, name: str, opt: Optional[str] = None, default: Any = None, action: Optional[Action] = None):
-        """添加一个选项
-
-        Args:
-            name (str): 选项的实际名称
-            opt (Optional[str], optional): 选项的字符串, 例如 `--foo -f <val:bool>`.
-            default (Any, optional): 选项的默认值.
-            action (Optional[Action], optional): 选项的动作.
-        """
         if opt is None:
             self.options.append(
                 Option(name, default=default, action=action)
             )
             return self
         parts = split(opt, (" ",))
         aliases = []
@@ -482,25 +468,22 @@
             opt = Option("|".join(aliases), _args, dest=name, default=default, action=action, help_text=help_text)
         else:
             opt = Option(name, _args, default=default, action=action, help_text=help_text)
         self.options.append(opt)
         return self
 
     def usage(self, content: str):
-        """设置命令的使用方法"""
         self.meta.usage = content
         return self
 
     def example(self, content: str):
-        """设置命令的使用示例"""
         self.meta.example = content
         return self
 
     def build(self):
-        """构造为 Alconna 对象"""
         return Alconna(*self.buffer.values(), *self.options, meta=self.meta)
 
 class MountConfig(TypedDict):
     prefixes: NotRequired[List[str]]
     raise_exception: NotRequired[bool]
     description: NotRequired[str]
     # get_subcommand: NotRequired[bool]
```

### Comparing `arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/debug.py` & `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/debug.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/formatter.py` & `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/formatter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 from typing import List, Dict, Any, Union, Tuple, Optional
-from nepattern import Empty, AllParam, AnyOne, AnyString
+from nepattern import Empty, AllParam
 from tarina import lang
 from arclet.alconna.args import Args, Arg
 from arclet.alconna.base import Subcommand, Option
 from arclet.alconna.formatter import TextFormatter, Trace
 
 
-class ShellTextFormatter(TextFormatter):
+class ArgParserTextFormatter(TextFormatter):
     """
-    shell 风格的帮助文本格式化器
+    argparser 风格的帮助文本格式化器
     """
 
     def format(self, trace: Trace) -> str:
         parts = trace.body  # type: ignore
         sub_names = [i.name for i in filter(lambda x: isinstance(x, Subcommand), parts)]
         opt_names = [min(i.aliases, key=len) for i in filter(lambda x: isinstance(x, Option), parts)]
         sub_names = f"{{{','.join(sub_names)}}}" if sub_names else ""
         opt_names = (" ".join(f"[{i}]" for i in opt_names)) if opt_names else ""
         topic = f"{lang.require('tools', 'format.ap.title')}: {trace.head['name']} {opt_names}\n {sub_names}"
         header = self.header(trace.head, trace.separators)
         param = self.parameters(trace.args)
         body = self.body(parts)
-        return header % (topic, param, body)
+        return f"{topic}\n{header % (param, body)}"
 
     def param(self, parameter: Arg) -> str:
         name = parameter.name
         if str(parameter.value).strip("'\"") == name:
             return f"[{name}]" if parameter.optional else name
         if parameter.hidden:
             return f"[{name.upper()}]" if parameter.optional else name.upper()
         if parameter.value is AllParam:
             return f"{name.upper()}..."
         arg = f"[{name.upper()}" if parameter.optional else name.upper()
-        if parameter.value not in (AnyOne, AnyString):
-            arg += f":{parameter.value}"
+        arg += f":{parameter.value}"
         if parameter.field.display is Empty:
             arg += "=None"
         elif parameter.field.display is not None:
             arg += f"={parameter.field.display}"
         return f"{arg}]" if parameter.optional else arg
 
     def parameters(self, args: Args) -> str:
@@ -47,30 +46,30 @@
                 continue
             if len(arg.separators) == 1:
                 sep = ' ' if arg.separators[0] == ' ' else f' {arg.separators[0]!r} '
             else:
                 sep = f"[{'|'.join(arg.separators)!r}]"
             res += self.param(arg) + sep
         notice = [(arg.name, arg.notice) for arg in args.argument if arg.notice]
-        return f"{res}\n{lang.require('tools', 'format.ap.notice')}:\n  - " + \
-            "\n  - ".join(f"{v[0]}: {v[1]}" for v in notice) if notice else res
+        return f"{res}\n  {lang.require('tools', 'format.ap.notice')}:\n  " + \
+            "\n  ".join(f"{v[0]}: {v[1]}" for v in notice) if notice else res
 
     def header(self, root: Dict[str, Any], separators: Tuple[str, ...]) -> str:
-        help_string = f"{desc}\n" if (desc := root.get("description")) else ""
+        help_string = f"\n{lang.require('tools', 'format.ap.desc')}: {desc}\n" if (desc := root.get("description")) else ""
         usage = f"\n{lang.require('tools', 'format.ap.usage')}: {usage}\n" if (usage := root.get("usage")) else ""
         example = f"\n{lang.require('tools', 'format.ap.example')}: {example}\n" if (example := root.get("example")) else ""
         header_text = (
             f"[{''.join(map(str, headers))}]"
             if (headers := root.get("header", [])) and headers != [""]
             else ""
         )
         cmd = f"{header_text}{root.get('name', '')}"
         sep = separators[0]
         command_string = (cmd or root["name"]) + sep
-        return f"{help_string}\n%s\n\n{command_string}%s{usage}\n%s{example}"
+        return f"\n{command_string}%s{help_string}{usage}\n%s{example}"
 
     def body(self, parts: List[Union[Option, Subcommand]]) -> str:
         options = []
         opt_description = []
         max_len = 1
         for opt in filter(
             lambda x: isinstance(x, Option) and (x.name not in self.ignore_names or not x.nargs), parts
@@ -151,16 +150,15 @@
         if str(parameter.value).strip("'\"") == name:
             return f"&#91;{name}&#93;" if parameter.optional else name
         if parameter.hidden:
             return f"&#91;{name}&#93;" if parameter.optional else f"&lt;{name}&gt;"
         if parameter.value is AllParam:
             return f"&lt;...{name}&gt;"
         arg = f"&#91;{name}" if parameter.optional else f"&lt;{name}"
-        if parameter.value not in (AnyOne, AnyString):
-            arg += f": {parameter.value}"
+        arg += f": {parameter.value}"
         if parameter.field.display is Empty:
             arg += " = None"
         elif parameter.field.display is not None:
             arg += f" = {parameter.field.display}"
         return f"{arg}&#93;" if parameter.optional else f"{arg}&gt;"
 
     def parameters(self, args: Args) -> Tuple[str, Optional[List[str]]]:
@@ -272,27 +270,26 @@
         sub_names = self._convert(f"{{{','.join(sub_names)}}}\n", "info") if sub_names else ""
         opt_names = self._convert((" ".join(f"[{i}]" for i in opt_names)), 'info') if opt_names else ""
         title = f"{lang.require('tools', 'format.ap.title')}:"
         topic = f"{self._convert(title, 'warn')} {self._convert(trace.head['name'], 'msg')} {opt_names}\n {sub_names}"
         header = self.header(trace.head, trace.separators)
         param = self._convert(self.parameters(trace.args), "success")
         body = self.body(parts)
-        return header % (topic, param, body)
+        return f"{topic}{header % (param, body)}"
 
     def param(self, parameter: Arg) -> str:
         name = parameter.name
         if str(parameter.value).strip("'\"") == name:
             return f"[{name}]" if parameter.optional else name
         if parameter.hidden:
             return f"[{name.upper()}]" if parameter.optional else name.upper()
         if parameter.value is AllParam:
             return f"{name.upper()}..."
         arg = f"[{name.upper()}" if parameter.optional else name.upper()
-        if parameter.value not in (AnyOne, AnyString):
-            arg += f":{parameter.value}"
+        arg += f":{parameter.value}"
         if parameter.field.display is Empty:
             arg += "=None"
         elif parameter.field.display is not None:
             arg += f"={parameter.field.display}"
         return f"{arg}]" if parameter.optional else arg
 
     def parameters(self, args: Args) -> str:
@@ -302,34 +299,34 @@
                 continue
             if len(arg.separators) == 1:
                 sep = ' ' if arg.separators[0] == ' ' else f' {arg.separators[0]!r} '
             else:
                 sep = f"[{'|'.join(arg.separators)!r}]"
             res += self.param(arg) + sep
         notice = [(arg.name, arg.notice) for arg in args.argument if arg.notice]
-        _not = self._convert(f"{lang.require('tools', 'format.ap.notice')}:", 'warn')
-        return f"{res}\n{_not}\n  - " + \
-            "\n  - ".join(self._convert(f"{v[0]}: {v[1]}", "success") for v in notice) if notice else res
+        return f"{res}\n  {lang.require('tools', 'format.ap.notice')}:\n  " + \
+            "\n  ".join(f"{v[0]}: {v[1]}" for v in notice) if notice else res
 
 
     def header(self, root: Dict[str, Any], separators: Tuple[str, ...]) -> str:
+        _desc = f"{lang.require('tools', 'format.ap.desc')}:"
         _usage = f"{lang.require('tools', 'format.ap.usage')}:"
         _example = f"{lang.require('tools', 'format.ap.example')}:"
-        help_string = f"{desc}\n" if (desc := root.get("description")) else ""
+        help_string = f"\n{self._convert(_desc, 'warn')} {desc}\n" if (desc := root.get("description")) else ""
         usage = f"\n{self._convert(_usage, 'warn')} {usage}\n" if (usage := root.get("usage")) else ""
         example = f"\n{self._convert(_example, 'warn')} {example}\n" if (example := root.get("example")) else ""
         header_text = (
             f"[{''.join(map(str, headers))}]"
             if (headers := root.get("header", [])) and headers != [""]
             else ""
         )
         cmd = f"{header_text}{root.get('name', '')}"
         sep = separators[0]
-        command_string = self._convert((cmd or root["name"]) + sep, "msg")
-        return f"{help_string}\n%s\n\n{command_string}%s{usage}\n%s{example}"
+        command_string = self._convert((cmd or root["name"]) + sep, "success")
+        return f"\n{command_string}%s{help_string}{usage}\n%s{example}"
 
     def body(self, parts: List[Union[Option, Subcommand]]) -> str:
         options = []
         opt_description = []
         max_len = 1
         for opt in filter(
             lambda x: isinstance(x, Option) and (x.name not in self.ignore_names or not x.nargs), parts
```

### Comparing `arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/i18n/en-US.json` & `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/i18n/en-US.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/i18n/zh-CN.json` & `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/i18n/zh-CN.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.0/src/arclet/alconna/tools/pattern.py` & `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/pattern.py`

 * *Files identical despite different names*

