# Comparing `tmp/feathers-0.1.1.tar.gz` & `tmp/feathers-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feathers-0.1.1.tar", max compression
+gzip compressed data, was "feathers-0.1.2.tar", max compression
```

## Comparing `feathers-0.1.1.tar` & `feathers-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,19 @@
--rw-r--r--   0        0        0       29 2023-05-04 04:58:16.361797 feathers-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/__init__.py
--rw-r--r--   0        0        0       53 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/__main__.py
--rw-r--r--   0        0        0      161 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/demo.py
--rw-r--r--   0        0        0       97 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/widgets/__init__.py
--rw-r--r--   0        0        0      118 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/widgets/help/__init__.py
--rw-r--r--   0        0        0     1002 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/widgets/help/_base.py
--rw-r--r--   0        0        0     1684 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/widgets/help/_help.py
--rw-r--r--   0        0        0     5944 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/widgets/help/_long_help.py
--rw-r--r--   0        0        0      714 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/widgets/help/_models.py
--rw-r--r--   0        0        0     3948 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/widgets/help/_short_help.py
--rw-r--r--   0        0        0     1307 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/widgets/help/_utils.py
--rw-r--r--   0        0        0      882 2023-05-04 04:58:16.361797 feathers-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 feathers-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-05-11 13:14:26.704562 feathers-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 13:14:26.704562 feathers-0.1.2/feathers/__init__.py
+-rw-r--r--   0        0        0       53 2023-05-11 13:14:26.704562 feathers-0.1.2/feathers/__main__.py
+-rw-r--r--   0        0        0     5955 2023-05-11 13:14:26.704562 feathers-0.1.2/feathers/cache.py
+-rw-r--r--   0        0        0      161 2023-05-11 13:14:26.704562 feathers-0.1.2/feathers/demo.py
+-rw-r--r--   0        0        0       64 2023-05-11 13:14:26.704562 feathers-0.1.2/feathers/utils/__init__.py
+-rw-r--r--   0        0        0      763 2023-05-11 13:14:26.704562 feathers-0.1.2/feathers/utils/_errors.py
+-rw-r--r--   0        0        0      202 2023-05-11 13:14:26.704562 feathers-0.1.2/feathers/widgets/__init__.py
+-rw-r--r--   0        0        0     5737 2023-05-11 13:14:26.704562 feathers-0.1.2/feathers/widgets/_cached_view.py
+-rw-r--r--   0        0        0     9016 2023-05-11 13:14:26.704562 feathers-0.1.2/feathers/widgets/_nav_view.py
+-rw-r--r--   0        0        0      118 2023-05-11 13:14:26.704562 feathers-0.1.2/feathers/widgets/help/__init__.py
+-rw-r--r--   0        0        0     1125 2023-05-11 13:14:26.704562 feathers-0.1.2/feathers/widgets/help/_base.py
+-rw-r--r--   0        0        0     3684 2023-05-11 13:14:26.704562 feathers-0.1.2/feathers/widgets/help/_help.py
+-rw-r--r--   0        0        0     5784 2023-05-11 13:14:26.704562 feathers-0.1.2/feathers/widgets/help/_long_help.py
+-rw-r--r--   0        0        0      714 2023-05-11 13:14:26.704562 feathers-0.1.2/feathers/widgets/help/_models.py
+-rw-r--r--   0        0        0     3999 2023-05-11 13:14:26.704562 feathers-0.1.2/feathers/widgets/help/_short_help.py
+-rw-r--r--   0        0        0     1307 2023-05-11 13:14:26.704562 feathers-0.1.2/feathers/widgets/help/_utils.py
+-rw-r--r--   0        0        0      907 2023-05-11 13:14:26.708562 feathers-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 feathers-0.1.2/PKG-INFO
```

### Comparing `feathers-0.1.1/feathers/widgets/help/_base.py` & `feathers-0.1.2/feathers/widgets/help/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,19 @@
     def _on_resize(self, _: events.Resize) -> None:
         self.__reset(None)
 
     # called by textual
     def _on_mount(self, _: events.Mount) -> None:
         self.watch(self.screen, "focused", self.__reset)
         self.watch(self.screen, "stack_updates", self.__reset)
+        self.__reset(None)
+
+    # called by textual
+    def _notify_style_update(self) -> None:
+        self.__reset(None)
 
     @abstractmethod
     def _create_help(self) -> Text:
         pass
 
     def _can_switch(self) -> bool:
         return True
```

### Comparing `feathers-0.1.1/feathers/widgets/help/_long_help.py` & `feathers-0.1.2/feathers/widgets/help/_long_help.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,47 +25,40 @@
     def __post_init__(self) -> None:
         self._col_count: int | None = None
         self._col_w: int | None = None
         self._entry_key_w: int | None = None
         self._entry_sep_w: int | None = None
         self._entry_desc_w: int | None = None
 
-    def _entry_key_width(self) -> int:
+    def _key_width(self) -> int:
         if self._entry_key_w is None:
             max_provided_key_width = max(len(entry.name) for entry in self.entries)
             self._entry_key_w = min(max_provided_key_width, self.max_key_w)
         return self._entry_key_w
 
-    def _entry_separator_width(self) -> int:
+    def _separator_width(self) -> int:
         if self._entry_sep_w is None:
             self._entry_sep_w = min(len(self.separator), self.max_separator_w)
         return self._entry_sep_w
 
-    def _entry_desc_width(self) -> int:
+    def _desc_width(self) -> int:
         if self._entry_desc_w is None:
             max_provided_desc_width = max(len(entry.description) for entry in self.entries)
-            leftover_width = self.max_w - (
-                self._entry_key_width() + self._entry_separator_width() + (2 * self.col_padding)
-            )
+            leftover_width = self.max_w - (self._key_width() + self._separator_width() + (2 * self.col_padding))
             self._entry_desc_w = min(max_provided_desc_width, leftover_width)
         return self._entry_desc_w
 
     @property
     def entry_widths(self) -> tuple[int, int, int]:
-        return (self._entry_key_width(), self._entry_separator_width(), self._entry_desc_width())
+        return (self._key_width(), self._separator_width(), self._desc_width())
 
     @property
     def col_width(self) -> int:
         if self._col_w is None:
-            entry_w = (
-                self._entry_key_width()
-                + self._entry_separator_width()
-                + self._entry_desc_width()
-                + (2 * self.col_padding)
-            )
+            entry_w = self._key_width() + self._separator_width() + self._desc_width() + (2 * self.col_padding)
             self._col_w = min(entry_w, self.max_w)
         return self._col_w
 
     @property
     def col_count(self) -> int:
         if self._col_count is None:
             self._col_count = max(1, math.floor(self.width / self.col_width))
@@ -151,19 +144,19 @@
             desc_text.pad(1, self._pad_box)
         line_text.append(desc_text)
 
         return line_text
 
     def _create_help(self) -> Text:
         # avoid division by zero
-        if self.size.width == 0:
+        if self.content_size.width == 0:
             return Text("")
 
         entries = self._get_entries_from_bindings()
-        self._measurement = Measurement(self.size.width, entries, self._separator)
+        self._measurement = Measurement(self.content_size.width, entries, self._separator)
         entry_texts = [self.__entry_text(e) for e in entries]
 
         line_text = Text(
             style=self.rich_style,
             no_wrap=True,
             overflow="ellipsis",
             justify="left",
```

### Comparing `feathers-0.1.1/feathers/widgets/help/_models.py` & `feathers-0.1.2/feathers/widgets/help/_models.py`

 * *Files identical despite different names*

### Comparing `feathers-0.1.1/feathers/widgets/help/_short_help.py` & `feathers-0.1.2/feathers/widgets/help/_short_help.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,45 @@
         separator: str,
         placeholder_text: str = "No key mappings found. Trying changing focus",
     ) -> None:
         super().__init__(id=id)
         self.toggle_key = toggle_key
         self.separator = separator
         self.placeholder_text: str = placeholder_text
+
         self._can_switch_to_long_help: bool = False
+        self._text_style = Text(
+            style=self.rich_style,
+            no_wrap=True,
+            overflow="ellipsis",
+            justify="left",
+            end="",
+        )
+
+    def _can_switch(self) -> bool:
+        return self._can_switch_to_long_help
+
+    def _create_help(self) -> Text:
+        text = self._text_style.copy()
+        entries = self.__get_entries()
+
+        if self.__has_long_help_entries(entries):
+            self._can_switch_to_long_help = True
+            entries.append(self.toggle_key)
+        else:
+            self._can_switch_to_long_help = False
+
+        if len(entries) == 0:
+            return self.__get_placeholder_text()
+
+        separator_style = self.get_component_rich_style("shorthelp--separator")
+        separator = text.append(self.separator, separator_style)
+
+        entry_texts = [self.__entry_text(e) for e in entries]
+        return separator.join(entry_texts)
 
     def __entry_text(self, entry: HelpEntry) -> Text:
         key_style = self.get_component_rich_style("shorthelp--key")
         description_style = self.get_component_rich_style("shorthelp--description")
         return Text.assemble((entry.name.lower(), key_style), (f" {entry.description.lower()}", description_style))
 
     def __get_placeholder_text(self) -> Text:
@@ -91,36 +121,7 @@
         return list(dict.fromkeys(keys))  ## dedupe list
 
     def __has_long_help_entries(self, entries: list[HelpEntry]) -> bool:
         long_help_entries = self._get_entries_from_bindings()
         if self.toggle_key in long_help_entries:
             long_help_entries.remove(self.toggle_key)
         return bool(set(long_help_entries) - set(entries))
-
-    def _can_switch(self) -> bool:
-        return self._can_switch_to_long_help
-
-    def _create_help(self) -> Text:
-        text = Text(
-            style=self.rich_style,
-            no_wrap=True,
-            overflow="ellipsis",
-            justify="left",
-            end="",
-        )
-
-        entries = self.__get_entries()
-
-        if self.__has_long_help_entries(entries):
-            self._can_switch_to_long_help = True
-            entries.append(self.toggle_key)
-        else:
-            self._can_switch_to_long_help = False
-
-        if len(entries) == 0:
-            return self.__get_placeholder_text()
-
-        separator_style = self.get_component_rich_style("shorthelp--separator")
-        separator = text.append(self.separator, separator_style)
-
-        entry_texts = [self.__entry_text(e) for e in entries]
-        return separator.join(entry_texts)
```

### Comparing `feathers-0.1.1/feathers/widgets/help/_utils.py` & `feathers-0.1.2/feathers/widgets/help/_utils.py`

 * *Files identical despite different names*

### Comparing `feathers-0.1.1/pyproject.toml` & `feathers-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "feathers"
-version = "0.1.1"
+version = "0.1.2"
 description = "Beautiful TUI components written on top of Textual"
 authors = ["Shashank Tomar <shashank004@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "feathers"}]
 repository = "https://github.com/shashanktomar/feathers"
 keywords = ["textual", "terminal", "TUI"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 rich = "^13.3.5"
-textual = "^0.22.3"
+textual = "^0.24.1"
 
 
 [tool.poetry.group.dev.dependencies]
-textual = {extras = ["dev"], version = "^0.22.3"}
+textual = {extras = ["dev"], version = "^0.24.1"}
 ruff = "^0.0.264"
 black = "^23.3.0"
 mypy = "^1.2.0"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 pytest-asyncio = "^0.21.0"
 
@@ -32,7 +32,10 @@
 # Never enforce `E501` (line length violations).
 ignore = ["E741"]
 select = ["E", "F", "I", "W", "UP"]
 line-length = 120
 
 [tool.black]
 line-length = 120
+
+[pytest]
+log_cli = true
```

### Comparing `feathers-0.1.1/PKG-INFO` & `feathers-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: feathers
-Version: 0.1.1
+Version: 0.1.2
 Summary: Beautiful TUI components written on top of Textual
 Home-page: https://github.com/shashanktomar/feathers
 License: MIT
 Keywords: textual,terminal,TUI
 Author: Shashank Tomar
 Author-email: shashank004@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: rich (>=13.3.5,<14.0.0)
-Requires-Dist: textual (>=0.22.3,<0.23.0)
+Requires-Dist: textual (>=0.24.1,<0.25.0)
 Project-URL: Repository, https://github.com/shashanktomar/feathers
 Description-Content-Type: text/markdown
 
 # Feathers
 
 Work in Progress
```

