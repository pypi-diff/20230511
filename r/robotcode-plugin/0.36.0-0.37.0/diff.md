# Comparing `tmp/robotcode_plugin-0.36.0.tar.gz` & `tmp/robotcode_plugin-0.37.0.tar.gz`

## Comparing `robotcode_plugin-0.36.0.tar` & `robotcode_plugin-0.37.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 robotcode_plugin-0.36.0/src/robotcode/plugin/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_plugin-0.36.0/src/robotcode/plugin/__version__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 robotcode_plugin-0.36.0/src/robotcode/plugin/manager.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_plugin-0.36.0/src/robotcode/plugin/py.typed
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 robotcode_plugin-0.36.0/src/robotcode/plugin/specs.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 robotcode_plugin-0.36.0/src/robotcode/plugin/click_helper/aliases.py
--rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 robotcode_plugin-0.36.0/src/robotcode/plugin/click_helper/options.py
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 robotcode_plugin-0.36.0/src/robotcode/plugin/click_helper/types.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_plugin-0.36.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_plugin-0.36.0/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_plugin-0.36.0/README.md
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 robotcode_plugin-0.36.0/pyproject.toml
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 robotcode_plugin-0.36.0/PKG-INFO
+-rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 robotcode_plugin-0.37.0/src/robotcode/plugin/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_plugin-0.37.0/src/robotcode/plugin/__version__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 robotcode_plugin-0.37.0/src/robotcode/plugin/manager.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_plugin-0.37.0/src/robotcode/plugin/py.typed
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 robotcode_plugin-0.37.0/src/robotcode/plugin/specs.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 robotcode_plugin-0.37.0/src/robotcode/plugin/click_helper/aliases.py
+-rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 robotcode_plugin-0.37.0/src/robotcode/plugin/click_helper/options.py
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 robotcode_plugin-0.37.0/src/robotcode/plugin/click_helper/types.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_plugin-0.37.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_plugin-0.37.0/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_plugin-0.37.0/README.md
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 robotcode_plugin-0.37.0/pyproject.toml
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 robotcode_plugin-0.37.0/PKG-INFO
```

### Comparing `robotcode_plugin-0.36.0/src/robotcode/plugin/__init__.py` & `robotcode_plugin-0.37.0/src/robotcode/plugin/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 import dataclasses
 import sys
 from dataclasses import dataclass
 from enum import Enum, unique
 from pathlib import Path
-from typing import IO, Any, AnyStr, Callable, Iterable, List, Optional, TypeVar, Union, cast
+from typing import IO, Any, AnyStr, Callable, Iterable, Optional, Sequence, TypeVar, Union, cast
 
 import click
 import pluggy
 from robotcode.core.dataclasses import as_dict, as_json
 
-__all__ = ["hookimpl", "CommonConfig", "pass_application"]
+__all__ = [
+    "hookimpl",
+    "CommonConfig",
+    "pass_application",
+    "Application",
+    "UnknownError",
+    "OutputFormat",
+    "ColoredOutput",
+]
 
 F = TypeVar("F", bound=Callable[..., Any])
 hookimpl = cast(Callable[[F], F], pluggy.HookimplMarker("robotcode"))
 
 
 class UnknownError(click.ClickException):
     """An unknown error occurred."""
@@ -37,19 +45,20 @@
 
     def __str__(self) -> str:
         return self.value
 
 
 @dataclass
 class CommonConfig:
-    config_files: Optional[List[Path]] = None
-    profiles: Optional[List[str]] = None
+    config_files: Optional[Sequence[Path]] = None
+    profiles: Optional[Sequence[str]] = None
     dry: bool = False
     verbose: bool = False
     colored_output: ColoredOutput = ColoredOutput.AUTO
+    default_paths: Optional[Sequence[str]] = None
     launcher_script: Optional[str] = None
     output_format: Optional[OutputFormat] = None
     pager: Optional[bool] = None
 
 
 class Application:
     def __init__(self) -> None:
@@ -60,15 +69,15 @@
         return self.config.colored_output in [ColoredOutput.AUTO, ColoredOutput.YES]
 
     def verbose(
         self,
         message: Union[str, Callable[[], Any], None],
         file: Optional[IO[AnyStr]] = None,
         nl: bool = True,
-        err: bool = False,
+        err: bool = True,
     ) -> None:
         if self.config.verbose:
             click.secho(
                 message() if callable(message) else message,
                 file=file,
                 nl=nl,
                 err=err,
@@ -137,15 +146,18 @@
                     console.print(Syntax(text, format, background_color="default"))
 
                 return
             except ImportError:
                 if self.config.colored_output == ColoredOutput.YES:
                     self.warning('Package "rich" is required to use colored output.')
 
-        self.echo(text)
+        if self.config.pager:
+            self.echo_via_pager(text)
+        else:
+            self.echo(text)
 
         return
 
     def echo(
         self,
         message: Union[str, Callable[[], Any], None],
         file: Optional[IO[AnyStr]] = None,
@@ -172,20 +184,22 @@
                         for result in super().__rich_console__(console, options):
                             cast(Text, result).justify = "left"
 
                             yield result
 
                 Markdown.elements["heading_open"] = MyHeading
 
+                markdown = Markdown(text, justify="left", code_theme="default")
+
                 console = Console()
                 if self.config.pager:
-                    with console.pager(styles=self.colored, links=self.colored):
-                        console.print(Markdown(text, justify="left"))
+                    with console.pager(styles=True, links=True):
+                        console.print(markdown)
                 else:
-                    console.print(Markdown(text, justify="left"))
+                    console.print(markdown)
                 return
             except ImportError:
                 if self.config.colored_output == ColoredOutput.YES:
                     self.warning('Package "rich" is required to use colored output.')
 
         self.echo_via_pager(text)
```

### Comparing `robotcode_plugin-0.36.0/src/robotcode/plugin/manager.py` & `robotcode_plugin-0.37.0/src/robotcode/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.36.0/src/robotcode/plugin/click_helper/aliases.py` & `robotcode_plugin-0.37.0/src/robotcode/plugin/click_helper/aliases.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.36.0/src/robotcode/plugin/click_helper/options.py` & `robotcode_plugin-0.37.0/src/robotcode/plugin/click_helper/options.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.36.0/src/robotcode/plugin/click_helper/types.py` & `robotcode_plugin-0.37.0/src/robotcode/plugin/click_helper/types.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.36.0/.gitignore` & `robotcode_plugin-0.37.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.36.0/LICENSE.txt` & `robotcode_plugin-0.37.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.36.0/README.md` & `robotcode_plugin-0.37.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.36.0/pyproject.toml` & `robotcode_plugin-0.37.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.36.0/PKG-INFO` & `robotcode_plugin-0.37.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-plugin
-Version: 0.36.0
+Version: 0.37.0
 Summary: Some classes for RobotCode plugin management
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
 Author-email: Daniel Biehl <dbiehl@live.de>
```

