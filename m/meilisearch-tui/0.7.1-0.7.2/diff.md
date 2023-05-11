# Comparing `tmp/meilisearch_tui-0.7.1.tar.gz` & `tmp/meilisearch_tui-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_tui-0.7.1.tar", max compression
+gzip compressed data, was "meilisearch_tui-0.7.2.tar", max compression
```

## Comparing `meilisearch_tui-0.7.1.tar` & `meilisearch_tui-0.7.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-04-19 12:02:49.865236 meilisearch_tui-0.7.1/LICENSE
--rw-r--r--   0        0        0     2045 2023-04-19 12:02:49.865236 meilisearch_tui-0.7.1/README.md
--rw-r--r--   0        0        0        0 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/__init__.py
--rw-r--r--   0        0        0      115 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/__main__.py
--rw-r--r--   0        0        0      608 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/client.py
--rw-r--r--   0        0        0     3226 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/config.py
--rw-r--r--   0        0        0       86 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/errors.py
--rw-r--r--   0        0        0     2776 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/main.py
--rw-r--r--   0        0        0     1909 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/meilisearch.css
--rw-r--r--   0        0        0        0 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/py.typed
--rw-r--r--   0        0        0        0 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/screens/__init__.py
--rw-r--r--   0        0        0     4548 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/screens/configuration.py
--rw-r--r--   0        0        0    29002 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/screens/indexes.py
--rw-r--r--   0        0        0     6241 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/screens/search.py
--rw-r--r--   0        0        0      897 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/utils.py
--rw-r--r--   0        0        0        0 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/widgets/__init__.py
--rw-r--r--   0        0        0      844 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/widgets/index.py
--rw-r--r--   0        0        0     1543 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/widgets/index_sidebar.py
--rw-r--r--   0        0        0     1730 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/widgets/input.py
--rw-r--r--   0        0        0      709 2023-04-19 12:02:49.869236 meilisearch_tui-0.7.1/meilisearch_tui/widgets/messages.py
--rw-r--r--   0        0        0     2005 2023-04-19 12:02:49.873236 meilisearch_tui-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3297 1970-01-01 00:00:00.000000 meilisearch_tui-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 20:23:04.069288 meilisearch_tui-0.7.2/LICENSE
+-rw-r--r--   0        0        0     2045 2023-05-11 20:23:04.069288 meilisearch_tui-0.7.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/__init__.py
+-rw-r--r--   0        0        0      115 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/__main__.py
+-rw-r--r--   0        0        0      608 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/client.py
+-rw-r--r--   0        0        0     3226 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/config.py
+-rw-r--r--   0        0        0       86 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/errors.py
+-rw-r--r--   0        0        0     2776 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/main.py
+-rw-r--r--   0        0        0     1908 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/meilisearch.css
+-rw-r--r--   0        0        0        0 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/py.typed
+-rw-r--r--   0        0        0        0 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/screens/__init__.py
+-rw-r--r--   0        0        0     4548 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/screens/configuration.py
+-rw-r--r--   0        0        0    29130 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/screens/indexes.py
+-rw-r--r--   0        0        0     6273 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/screens/search.py
+-rw-r--r--   0        0        0      897 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/utils.py
+-rw-r--r--   0        0        0        0 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/widgets/__init__.py
+-rw-r--r--   0        0        0      844 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/widgets/index.py
+-rw-r--r--   0        0        0     1543 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/widgets/index_sidebar.py
+-rw-r--r--   0        0        0     1730 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/widgets/input.py
+-rw-r--r--   0        0        0      709 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/meilisearch_tui/widgets/messages.py
+-rw-r--r--   0        0        0     2083 2023-05-11 20:23:04.073288 meilisearch_tui-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3297 1970-01-01 00:00:00.000000 meilisearch_tui-0.7.2/PKG-INFO
```

### Comparing `meilisearch_tui-0.7.1/LICENSE` & `meilisearch_tui-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.1/README.md` & `meilisearch_tui-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.1/meilisearch_tui/client.py` & `meilisearch_tui-0.7.2/meilisearch_tui/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.1/meilisearch_tui/config.py` & `meilisearch_tui-0.7.2/meilisearch_tui/config.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.1/meilisearch_tui/main.py` & `meilisearch_tui-0.7.2/meilisearch_tui/main.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.1/meilisearch_tui/meilisearch.css` & `meilisearch_tui-0.7.2/meilisearch_tui/meilisearch.css`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,14 @@
   width: 100%;
   height: auto;
 }
 
 #results-container {
   background: $background 50%;
   margin: 0 0 1 0;
-  height: 100%;
+  height: 84%;
   overflow: hidden auto;
   border: tall $background;
   scrollbar-color: $primary-lighten-1;
   scrollbar-color-hover: $primary-lighten-1;
   scrollbar-color-active: $primary;
 }
```

### Comparing `meilisearch_tui-0.7.1/meilisearch_tui/screens/configuration.py` & `meilisearch_tui-0.7.2/meilisearch_tui/screens/configuration.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.1/meilisearch_tui/screens/indexes.py` & `meilisearch_tui-0.7.2/meilisearch_tui/screens/indexes.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MeilisearchError,
 )
 from meilisearch_python_async.models.settings import (
     MeilisearchSettings as MeilisearchSettingsInfo,
 )
 from textual import events
 from textual.app import ComposeResult
-from textual.containers import Center, Container, Content, Horizontal
+from textual.containers import Center, Container, Horizontal, VerticalScroll
 from textual.message import Message
 from textual.reactive import reactive
 from textual.screen import Screen
 from textual.widget import Widget
 from textual.widgets import (
     Button,
     DirectoryTree,
@@ -286,15 +286,15 @@
         self.data_load_error.visible = False
         self.data_file.focus()
 
     def on_directory_tree_file_selected(self, event: DirectoryTree.FileSelected) -> None:
         """Called when the user click a file in the directory tree."""
         event.stop()
         try:
-            self.data_file.value = event.path
+            self.data_file.value = str(event.path)
         except Exception:
             raise
 
     async def on_button_pressed(self, event: Button.Pressed) -> None:
         button_id = event.button.id
 
         if button_id == "load-data-button":
@@ -610,59 +610,61 @@
         self.pagination_input.value = results.pagination.json() if results.pagination else "{}"
         self.synonyms_input.focus()
 
 
 class MeilisearchSettings(Widget):
     DEFAULT_CSS = """
     MeilisearchSettings {
-        height: 90;
+        height: 108;
+        width: 100%;
     }
     """
 
     selected_index: reactive[str | None] = reactive(None, layout=True)
     edit_view = reactive(False, layout=True)
 
     def compose(self) -> ComposeResult:
-        with Content(id="results-container"):
-            yield Markdown(id="results")
-            with Center():
-                yield Button("Edit Settings", id="edit-settings-button")
-        with Content(id="edit-settings"):
-            yield EditMeilisearchSettings()
+        with Container(id="results-container"):
+            with Container(id="view-settings"):
+                yield Markdown(id="results")
+                with Center():
+                    yield Button("Edit Settings", id="edit-settings-button")
+            with VerticalScroll(id="edit-settings"):
+                yield EditMeilisearchSettings()
 
     @cached_property
     def results(self) -> Markdown:
         return self.query_one("#results", Markdown)
 
     @cached_property
-    def results_container(self) -> Content:
-        return self.query_one("#results-container", Content)
+    def view_settings(self) -> Container:
+        return self.query_one("#view-settings", Container)
 
     @cached_property
     def edit_settings_button(self) -> Button:
         return self.query_one("#edit-settings-button", Button)
 
     @cached_property
-    def edit_settings_container(self) -> Content:
-        return self.query_one("#edit-settings", Content)
+    def edit_settings_container(self) -> VerticalScroll:
+        return self.query_one("#edit-settings", VerticalScroll)
 
     @cached_property
     def edit_meilisearch_settings(self) -> EditMeilisearchSettings:
         return self.query_one(EditMeilisearchSettings)
 
     async def watch_selected_index(self) -> None:
         asyncio.create_task(self.load_settings())
         self.edit_meilisearch_settings.selected_index = self.selected_index
 
     def watch_edit_view(self) -> None:
         if self.edit_view:
-            self.results_container.display = False
+            self.view_settings.display = False
             self.edit_settings_container.display = True
         else:
-            self.results_container.display = True
+            self.view_settings.display = True
             self.edit_settings_container.display = False
 
     async def on_edit_meilisearch_settings_settings_saved(
         self, event: EditMeilisearchSettings.SettingsSaved
     ) -> None:
         if event.settings_saved:
             self.edit_view = False
@@ -709,15 +711,15 @@
 
         return "\n".join(lines)
 
 
 class IndexScreen(Screen):
     def compose(self) -> ComposeResult:
         yield IndexSidebar(classes="sidebar")
-        with Container(id="body"):
+        with VerticalScroll(id="body"):
             with TabbedContent(initial="index-settings"):
                 with TabPane("Index Settings", id="index-settings"):
                     yield MeilisearchSettings()
                 with TabPane("Add Index", id="add-index"):
                     yield AddIndex()
                 with TabPane("Delete Index", id="delete-index"):
                     yield DeleteIndex()
@@ -727,16 +729,16 @@
         yield Footer()
 
     @cached_property
     def add_index(self) -> AddIndex:
         return self.query_one(AddIndex)
 
     @cached_property
-    def body(self) -> Container:
-        return self.query_one("#body", Container)
+    def body(self) -> VerticalScroll:
+        return self.query_one("#body", VerticalScroll)
 
     @cached_property
     def data_load(self) -> DataLoad:
         return self.query_one(DataLoad)
 
     @cached_property
     def delete_index(self) -> DeleteIndex:
```

### Comparing `meilisearch_tui-0.7.1/meilisearch_tui/screens/search.py` & `meilisearch_tui-0.7.2/meilisearch_tui/screens/search.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import cached_property
 
 from aiocache import cached
 from meilisearch_python_async.errors import MeilisearchCommunicationError
 from meilisearch_python_async.models.search import SearchResults
 from textual import events
 from textual.app import ComposeResult
-from textual.containers import Center, Container, Content
+from textual.containers import Center, VerticalScroll
 from textual.screen import Screen
 from textual.widgets import Button, Footer, Input, Markdown, Static
 
 from meilisearch_tui.client import get_client
 from meilisearch_tui.widgets.index_sidebar import IndexSidebar
 from meilisearch_tui.widgets.messages import ErrorMessage
 
@@ -22,26 +22,26 @@
         super().__init__()
         self.limit = 20
         self.selected_index: str | None = None
 
     def compose(self) -> ComposeResult:
         yield ErrorMessage("", classes="message-centered", id="generic-error")
         yield IndexSidebar(classes="sidebar")
-        with Container(id="body"):
+        with VerticalScroll(id="body"):
             yield Static("No index selected", id="index-name", classes="bottom-spacer")
             yield Input(placeholder="Search", classes="bottom-spacer", id="search")
-            with Content(id="results-container"):
+            with VerticalScroll(id="results-container"):
                 yield Markdown(id="results")
             with Center():
                 yield Button(label="Load More", classes="bottom-spacer", id="load-more-button")
         yield Footer()
 
     @cached_property
-    def body_container(self) -> Container:
-        return self.query_one("#body", Container)
+    def body_container(self) -> VerticalScroll:
+        return self.query_one("#body", VerticalScroll)
 
     @cached_property
     def generic_error(self) -> ErrorMessage:
         return self.query_one("#generic-error", ErrorMessage)
 
     @cached_property
     def index_sidebar(self) -> IndexSidebar:
@@ -52,16 +52,16 @@
         return self.query_one("#index-name", Static)
 
     @cached_property
     def search_input(self) -> Input:
         return self.query_one("#search", Input)
 
     @cached_property
-    def results_container(self) -> Content:
-        return self.query_one("#results-container", Content)
+    def results_container(self) -> VerticalScroll:
+        return self.query_one("#results-container", VerticalScroll)
 
     @cached_property
     def results(self) -> Markdown:
         return self.query_one("#results", Markdown)
 
     @cached_property
     def load_more_button(self) -> Button:
```

### Comparing `meilisearch_tui-0.7.1/meilisearch_tui/utils.py` & `meilisearch_tui-0.7.2/meilisearch_tui/utils.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.1/meilisearch_tui/widgets/index.py` & `meilisearch_tui-0.7.2/meilisearch_tui/widgets/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.1/meilisearch_tui/widgets/index_sidebar.py` & `meilisearch_tui-0.7.2/meilisearch_tui/widgets/index_sidebar.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.1/meilisearch_tui/widgets/input.py` & `meilisearch_tui-0.7.2/meilisearch_tui/widgets/input.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.1/meilisearch_tui/widgets/messages.py` & `meilisearch_tui-0.7.2/meilisearch_tui/widgets/messages.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.1/pyproject.toml` & `meilisearch_tui-0.7.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-tui"
-version = "0.7.1"
+version = "0.7.2"
 description = "A TUI for Managing and Searching with Meilisearch"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-tui"
 homepage = "https://github.com/sanders41/meilisearch-tui"
 documentation = "https://github.com/sanders41/meilisearch-tui"
@@ -17,31 +17,31 @@
   "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-meilisearch-python-async = "1.2.0"
-textual = "0.20.1"
+meilisearch-python-async = "1.2.2"
+textual = "0.24.1"
 uvloop = {version = "0.17.0", markers = "sys_platform != 'win32'"}
-aiocache = "0.12.0"
+aiocache = "0.12.1"
 
 [tool.poetry.group.dev.dependencies]
 aiohttp = "3.8.4"
 black = "23.3.0"
 click = "8.1.3"
 msgpack = "1.0.5"
-mypy = "1.2.0"
-pre-commit = "3.2.2"
+mypy = "1.3.0"
+pre-commit = "3.3.1"
 pytest = "7.3.1"
 pytest-asyncio = "0.21.0"
 pytest-cov = "4.0.0"
-ruff = "0.0.261"
-tox = "4.4.12"
+ruff = "0.0.265"
+tox = "4.5.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 meilisearch = "meilisearch_tui.__main__:main"
@@ -71,14 +71,18 @@
 check_untyped_defs = true
 disallow_untyped_defs = true
 
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 disallow_untyped_defs = false
 
+[[tool.mypy.overrides]]
+module = ["aiocache.*"]
+ignore_missing_imports = true
+
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--cov=meilisearch_tui --cov-report term-missing"
 asyncio_mode = "auto"
 
 [tool.coverage.report]
 exclude_lines = ["if __name__ == .__main__.:", "pragma: no cover"]
```

### Comparing `meilisearch_tui-0.7.1/PKG-INFO` & `meilisearch_tui-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearch-tui
-Version: 0.7.1
+Version: 0.7.2
 Summary: A TUI for Managing and Searching with Meilisearch
 Home-page: https://github.com/sanders41/meilisearch-tui
 License: MIT
 Keywords: meilisearch,tui
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: aiocache (==0.12.0)
-Requires-Dist: meilisearch-python-async (==1.2.0)
-Requires-Dist: textual (==0.20.1)
+Requires-Dist: aiocache (==0.12.1)
+Requires-Dist: meilisearch-python-async (==1.2.2)
+Requires-Dist: textual (==0.24.1)
 Requires-Dist: uvloop (==0.17.0) ; sys_platform != "win32"
 Project-URL: Documentation, https://github.com/sanders41/meilisearch-tui
 Project-URL: Repository, https://github.com/sanders41/meilisearch-tui
 Description-Content-Type: text/markdown
 
 # Meilisearch TUI
```

