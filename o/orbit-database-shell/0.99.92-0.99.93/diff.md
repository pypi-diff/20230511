# Comparing `tmp/orbit_database_shell-0.99.92.tar.gz` & `tmp/orbit_database_shell-0.99.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_database_shell-0.99.92.tar", max compression
+gzip compressed data, was "orbit_database_shell-0.99.93.tar", max compression
```

## Comparing `orbit_database_shell-0.99.92.tar` & `orbit_database_shell-0.99.93.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1099 2023-05-10 11:34:30.904299 orbit_database_shell-0.99.92/LICENSE.md
--rw-r--r--   0        0        0        0 2023-05-10 11:15:26.057288 orbit_database_shell-0.99.92/README.md
--rwxr-xr-x   0        0        0        0 2023-05-10 11:54:13.621441 orbit_database_shell-0.99.92/orbit_database_shell/__init__.py
--rwxr-xr-x   0        0        0     1851 2023-05-11 13:22:32.666261 orbit_database_shell-0.99.92/orbit_database_shell/__main__.py
--rwxr-xr-x   0        0        0    24679 2023-05-11 13:22:51.769833 orbit_database_shell-0.99.92/orbit_database_shell/odb_actions.py
--rwxr-xr-x   0        0        0     4169 2023-05-10 14:32:56.666736 orbit_database_shell-0.99.92/orbit_database_shell/odb_completers.py
--rw-r--r--   0        0        0     1186 2023-05-10 15:56:22.156530 orbit_database_shell-0.99.92/orbit_database_shell/odb_decorators.py
--rwxr-xr-x   0        0        0     7071 2023-05-11 13:23:09.617433 orbit_database_shell-0.99.92/orbit_database_shell/odb_grammar.py
--rwxr-xr-x   0        0        0    46376 2023-05-11 12:30:35.883941 orbit_database_shell-0.99.92/orbit_database_shell/odb_help.py
--rw-r--r--   0        0        0      522 2023-05-11 13:24:04.788196 orbit_database_shell-0.99.92/pyproject.toml
--rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 orbit_database_shell-0.99.92/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-10 11:34:30.904299 orbit_database_shell-0.99.93/LICENSE.md
+-rw-r--r--   0        0        0     2289 2023-05-11 15:50:19.047142 orbit_database_shell-0.99.93/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-10 11:54:13.621441 orbit_database_shell-0.99.93/orbit_database_shell/__init__.py
+-rwxr-xr-x   0        0        0     1876 2023-05-11 15:18:01.901901 orbit_database_shell-0.99.93/orbit_database_shell/__main__.py
+-rwxr-xr-x   0        0        0    24822 2023-05-11 15:22:05.776682 orbit_database_shell-0.99.93/orbit_database_shell/odb_actions.py
+-rwxr-xr-x   0        0        0     4169 2023-05-10 14:32:56.666736 orbit_database_shell-0.99.93/orbit_database_shell/odb_completers.py
+-rw-r--r--   0        0        0     1988 2023-05-11 15:01:59.418713 orbit_database_shell-0.99.93/orbit_database_shell/odb_decorators.py
+-rwxr-xr-x   0        0        0     7071 2023-05-11 13:23:09.617433 orbit_database_shell-0.99.93/orbit_database_shell/odb_grammar.py
+-rwxr-xr-x   0        0        0    46376 2023-05-11 12:30:35.883941 orbit_database_shell-0.99.93/orbit_database_shell/odb_help.py
+-rw-r--r--   0        0        0     1315 2023-05-11 15:57:21.529383 orbit_database_shell-0.99.93/pyproject.toml
+-rw-r--r--   0        0        0     3768 1970-01-01 00:00:00.000000 orbit_database_shell-0.99.93/PKG-INFO
```

### Comparing `orbit_database_shell-0.99.92/LICENSE.md` & `orbit_database_shell-0.99.93/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-0.99.92/orbit_database_shell/__main__.py` & `orbit_database_shell-0.99.93/orbit_database_shell/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 from pathlib import Path, PosixPath
 from prompt_toolkit import PromptSession
 from prompt_toolkit.history import FileHistory
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.shortcuts import CompleteStyle
 from orbit_database_shell.odb_grammar import Completer, lexer, grammar, grammar_style
 from orbit_database_shell.odb_actions import Actions
+from orbit_database_shell.odb_decorators import banner
 
 __author__ = 'Gareth Bult'
 __banner__ = 'Orbit-DB'
 __copyright__ = 'Copyright 2023, Mad Penguin Consulting Ltd'
 __credits__ = ['Gareth Bult']
 __license__ = 'MIT'
 __version__ = '0.99.91'
 __maintainer__ = 'Gareth Bult'
 __email__ = 'gareth@madpenguin.uk'
 __status__ = 'Development'
 
-if __name__ == '__main__':
-    actions = Actions()
-    with open('./banner.txt') as io:
-        actions.notice(io.read())
+
+def main ():
+    actions = Actions().notice(banner)
     folder = Path('~/.orbit').expanduser()
     folder.mkdir(exist_ok=True, parents=True)
     session = PromptSession(
         history=FileHistory(PosixPath(folder / 'shell_history')),
         complete_style=CompleteStyle.READLINE_LIKE,
         auto_suggest=AutoSuggestFromHistory(),
         validate_while_typing=True,
@@ -44,7 +44,11 @@
                 continue
             actions.complete(action, user_input.variables())
         except KeyboardInterrupt:
             continue
         except EOFError:
             break
     actions.info('[shell terminated]')
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `orbit_database_shell-0.99.92/orbit_database_shell/odb_actions.py` & `orbit_database_shell-0.99.93/orbit_database_shell/odb_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,27 +49,27 @@
         if hasattr(self, f'do_{action}'):
             getattr(self, f'do_{action}')(variables)
         else:
             self.error(f'Syntax Ok but {action} is not available')
 
     def warning(self, text):
         print(HTML(f'<orange>{text}</orange>'))
-        return None
+        return self
 
     def error(self, text):
         print(HTML(f'<red>{text}</red>'))
-        return None
+        return self
 
     def info(self, text):
         print(HTML(f'<green>{text}</green>'))
-        return None
+        return self
 
     def notice(self, text):
         print(HTML(f'<blue>{text}</blue>'))
-        return None
+        return self
 
     @property
     def database_name(self):
         name = self._db_name if self._db else 'none'
         return [('class:database', name), ('class:chevron', '> ')]
 
     @property
@@ -294,15 +294,19 @@
         databases = self.load_databases()
         if not len(databases):
             return self.error(f'No databases registered!')
         
         tab = self.richTable(['Database name', 'Mapped', 'Used', '(%)', 'Path'])
         for name, path in databases.items():
             mdb = Path(path) / 'data.mdb'
-            stat = mdb.stat()
+            try:
+                stat = mdb.stat()
+            except FileNotFoundError:
+                self.error(f'Database is missing: {path}')
+                continue
             mapped = stat.st_size
             divisor = 1024
             units = 'K'
             if mapped > 1024 * 1024 * 1024:
                 divisor = 1024 * 1024 * 1024
                 units = 'G'
             elif mapped > 1024 * 1024:
```

### Comparing `orbit_database_shell-0.99.92/orbit_database_shell/odb_completers.py` & `orbit_database_shell-0.99.93/orbit_database_shell/odb_completers.py`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-0.99.92/orbit_database_shell/odb_grammar.py` & `orbit_database_shell-0.99.93/orbit_database_shell/odb_grammar.py`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-0.99.92/orbit_database_shell/odb_help.py` & `orbit_database_shell-0.99.93/orbit_database_shell/odb_help.py`

 * *Files identical despite different names*

