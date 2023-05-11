# Comparing `tmp/chatplayground-1.1.1.tar.gz` & `tmp/chatplayground-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatplayground-1.1.1.tar", max compression
+gzip compressed data, was "chatplayground-1.1.2.tar", max compression
```

## Comparing `chatplayground-1.1.1.tar` & `chatplayground-1.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-05-10 09:42:40.414148 chatplayground-1.1.1/LICENSE
--rw-r--r--   0        0        0     4574 2023-05-10 09:42:40.414148 chatplayground-1.1.1/README.md
--rw-r--r--   0        0        0       17 2023-05-10 09:42:40.418148 chatplayground-1.1.1/chatplayground/.gitignore
--rw-r--r--   0        0        0       22 2023-05-10 09:42:40.418148 chatplayground-1.1.1/chatplayground/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 09:42:40.418148 chatplayground-1.1.1/chatplayground/app/__init__.py
--rw-r--r--   0        0        0   108121 2023-05-10 09:42:40.418148 chatplayground-1.1.1/chatplayground/app/app.py
--rw-r--r--   0        0        0    15406 2023-05-10 09:42:40.418148 chatplayground-1.1.1/chatplayground/assets/favicon.ico
--rw-r--r--   0        0        0     1281 2023-05-10 09:42:40.418148 chatplayground-1.1.1/chatplayground/assets/react-json-view-lite.css
--rw-r--r--   0        0        0   178190 2023-05-10 09:42:40.418148 chatplayground-1.1.1/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json
--rw-r--r--   0        0        0      921 2023-05-10 09:42:40.418148 chatplayground-1.1.1/chatplayground/pcconfig.py
--rw-r--r--   0        0        0     3081 2023-05-10 09:42:40.442148 chatplayground-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     6941 1970-01-01 00:00:00.000000 chatplayground-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-11 15:26:03.377943 chatplayground-1.1.2/LICENSE
+-rw-r--r--   0        0        0     4574 2023-05-11 15:26:03.381943 chatplayground-1.1.2/README.md
+-rw-r--r--   0        0        0       17 2023-05-11 15:26:03.381943 chatplayground-1.1.2/chatplayground/.gitignore
+-rw-r--r--   0        0        0       22 2023-05-11 15:26:03.381943 chatplayground-1.1.2/chatplayground/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:26:03.381943 chatplayground-1.1.2/chatplayground/app/__init__.py
+-rw-r--r--   0        0        0   109826 2023-05-11 15:26:03.381943 chatplayground-1.1.2/chatplayground/app/app.py
+-rw-r--r--   0        0        0    15406 2023-05-11 15:26:03.381943 chatplayground-1.1.2/chatplayground/assets/favicon.ico
+-rw-r--r--   0        0        0     1281 2023-05-11 15:26:03.381943 chatplayground-1.1.2/chatplayground/assets/react-json-view-lite.css
+-rw-r--r--   0        0        0   178190 2023-05-11 15:26:03.381943 chatplayground-1.1.2/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json
+-rw-r--r--   0        0        0      921 2023-05-11 15:26:03.381943 chatplayground-1.1.2/chatplayground/pcconfig.py
+-rw-r--r--   0        0        0     3081 2023-05-11 15:26:03.409944 chatplayground-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6941 1970-01-01 00:00:00.000000 chatplayground-1.1.2/PKG-INFO
```

### Comparing `chatplayground-1.1.1/LICENSE` & `chatplayground-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatplayground-1.1.1/README.md` & `chatplayground-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `chatplayground-1.1.1/chatplayground/app/app.py` & `chatplayground-1.1.2/chatplayground/app/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,18 +277,25 @@
 
     auto_focus: Var[typing.Union[str, int, bool]]
 
 
 auto_focus_text_area = AutoFocusTextArea.create
 
 
+class AutoFocusInput(pc.Input):
+    """Text area that supports the autofocus attribute."""
+
+    auto_focus: Var[typing.Union[str, int, bool]]
+
+
+auto_focus_input = AutoFocusInput.create
+
+
 def render_tooltip(*args, **kwargs):
-    """
-    Render a tooltip.
-    """
+    """Render a tooltip."""
     return pc.tooltip(*args, **kwargs, open_delay=500)
 
 
 class UID:
     """A unique ID generator that uses the current time and a counter to generate unique IDs.
 
     TODO: this is not thread safe, but that should not be a problem for now.
@@ -1548,14 +1555,49 @@
             on_submit=State.update_note,
             on_cancel=State.cancel_note_editing,
             margin="0.25em",
         ),
     )
 
 
+def render_title_editor():
+    """Render the title editor."""
+    # TODO: this is only because I cannot make the editable not very jerky.
+
+    return pc.cond(
+        ~State.title_editor,
+        pc.button(
+            pc.flex(
+                pc.cond(
+                    State.title_text,
+                    pc.text(State.title_text, width="100%"),
+                    pc.text("Untitled", color=SolarizedColors.base1, width="100%"),
+                ),
+                pc.spacer(),
+                pc.icon(tag="edit", size="xs"),
+                width="100%",
+                style={"text-align": "left"},
+                padding="0.25em",
+                margin="4px",
+            ),
+            on_click=State.start_title_editing(None),
+            variant="ghost",
+            width="100%",
+        ),
+        auto_focus_input(
+            default_value=State.title_text,
+            on_blur=State.update_title,
+            on_key_up=State.on_title_key_up,
+            on_change=State.set_title_text,
+            margin="0.25em",
+            auto_focus=True,
+        ),
+    )
+
+
 def render_model_options():
     """Render the model options."""
     return pc.table_container(
         pc.table(
             pc.tbody(
                 pc.tr(
                     pc.th("Model"),
@@ -1715,23 +1757,17 @@
                         variant=pc.cond(MessageGridState.is_grid_visible, 'solid', 'ghost'),
                         on_click=MessageGridState.toggle_grid,
                     ),
                     label="Toggle the expose-like message grid",
                 ),
             ),
             pc.heading(
-                pc.editable(
-                    pc.editable_preview(),
-                    pc.editable_input(),
-                    value=State.title_text,
-                    placeholder="Untitled",
-                    on_change=State.set_title_text,
-                    on_submit=State.update_title,
-                ),
+                render_title_editor(),
                 size="md",
+                width="100%",
             ),
         ),
         pc.divider(margin="0.5em"),
         pc.box(
             render_note_editor(),
             padding="0.5em",
         ),
@@ -2082,34 +2118,35 @@
         'note_editor',
         'drawer_visible',
         'title_text',
     ]
 
     message_exploration: MessageExploration = MessageExploration()
     note_editor: bool = False
-    drawer_visible: bool = False
-
+    title_editor: bool = False
     title_text: str = ""
+    drawer_visible: bool = False
 
     def on_message_exploration_update(self, message_exploration_uid: str):
         """Called when a message exploration is updated by the StoredExplorationsSingleton."""
         if message_exploration_uid != self.message_exploration.uid:
             return
 
-        return self.select_message_exploration(self, message_exploration_uid)  # type: ignore
+        message_exploration = message_explorations_singleton.get(self, message_exploration_uid)
+        self._set_message_exploration(self, message_exploration)  # type: ignore
 
     def new_message_exploration(self):
         """Create a new message exploration and make it the current one."""
         self._set_message_exploration(self, MessageExploration())  # type: ignore
 
     def select_message_exploration(self, message_exploration_uid: str):
         """Select a message exploration by its UID and make it the current one."""
+        self.drawer_visible = False
         message_exploration = message_explorations_singleton.get(self, message_exploration_uid)
-        if message_exploration != self.message_exploration:
-            self._set_message_exploration(self, message_exploration)  # type: ignore
+        self._set_message_exploration(self, message_exploration)  # type: ignore
 
     def _update_message_exploration_registry(self):
         message_explorations_singleton.update(self, self.message_exploration)
 
     @property
     def message_map(self):
         """Get the message map from the current message exploration."""
@@ -2145,16 +2182,34 @@
         self.message_exploration.note = content
         self._update_message_exploration_registry(self)  # type: ignore
         self.note_editor = False
         self.mark_dirty()
 
     def update_title(self, content):
         """Update the title in the current message exploration."""
-        self.message_exploration.title = content
+        print(f"Updating title to {content}")
+        self.message_exploration.title = content.strip()
         self._update_message_exploration_registry(self)  # type: ignore
+        self.title_editor = False
+        self.mark_dirty()
+
+    def on_title_key_up(self, key):
+        """Called when a key is pressed while editing the title."""
+        if key in ["Escape", "Enter"]:
+            if key == "Enter":
+                self.update_title(self, self.title_text)   # type: ignore
+            elif key == "Escape":
+                self.title_text = self.message_exploration.title
+
+            self.title_editor = False
+            self.mark_dirty()
+
+    def start_title_editing(self, _: typing.Any):
+        """Start editing the note."""
+        self.title_editor = True
         self.mark_dirty()
 
     @pc.var
     def get_available_message_explorations(self) -> list[MessageExploration]:
         """Get all available message explorations."""
         return message_explorations_singleton.get_all(self)
 
@@ -2172,15 +2227,14 @@
         :param message_exploration: The message exploration to set.
 
         This mainly ensures that the title and note fields are set correctly.
         """
         if message_exploration != self.message_exploration:
             self.message_exploration = message_exploration
             self.title_text = message_exploration.title
-            self.drawer_visible = False
             self.mark_dirty()
 
 
 class RemoveExplorationModalState(State):
     """The state for the remove exploration modal (to confirm removing a thread).
 
     TODO: display the whole thread so we can confirm we're removing the right one.
```

### Comparing `chatplayground-1.1.1/chatplayground/assets/favicon.ico` & `chatplayground-1.1.2/chatplayground/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `chatplayground-1.1.1/chatplayground/assets/react-json-view-lite.css` & `chatplayground-1.1.2/chatplayground/assets/react-json-view-lite.css`

 * *Files identical despite different names*

### Comparing `chatplayground-1.1.1/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json` & `chatplayground-1.1.2/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json`

 * *Files identical despite different names*

### Comparing `chatplayground-1.1.1/chatplayground/pcconfig.py` & `chatplayground-1.1.2/chatplayground/pcconfig.py`

 * *Files identical despite different names*

### Comparing `chatplayground-1.1.1/pyproject.toml` & `chatplayground-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "chatplayground"
-version = "1.1.1"
+version = "1.1.2"
 homepage = "https://github.com/blackhc/chatplayground"
 description = "ChatPlayground for LLMs"
 authors = ["Andreas Kirsch <blackhc@gmail.com>"]
 readme = "README.md"
 license =  "GPL-3.0-only"
 classifiers=[
     'Development Status :: 4 - Beta',
```

### Comparing `chatplayground-1.1.1/PKG-INFO` & `chatplayground-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatplayground
-Version: 1.1.1
+Version: 1.1.2
 Summary: ChatPlayground for LLMs
 Home-page: https://github.com/blackhc/chatplayground
 License: GPL-3.0-only
 Author: Andreas Kirsch
 Author-email: blackhc@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

