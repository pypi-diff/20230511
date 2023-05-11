# Comparing `tmp/gpt-term-1.0.1.tar.gz` & `tmp/gpt-term-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-term-1.0.1.tar", last modified: Thu Apr 27 08:09:04 2023, max compression
+gzip compressed data, was "gpt-term-1.0.2.tar", last modified: Thu May 11 09:05:29 2023, max compression
```

## Comparing `gpt-term-1.0.1.tar` & `gpt-term-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:09:04.922674 gpt-term-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-27 08:08:52.000000 gpt-term-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 08:08:52.000000 gpt-term-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-04-27 08:09:04.922674 gpt-term-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-04-27 08:08:52.000000 gpt-term-1.0.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-04-27 08:08:52.000000 gpt-term-1.0.1/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:09:04.918673 gpt-term-1.0.1/gpt_term/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 08:08:52.000000 gpt-term-1.0.1/gpt_term/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-27 08:08:52.000000 gpt-term-1.0.1/gpt_term/config.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)    43634 2023-04-27 08:08:52.000000 gpt-term-1.0.1/gpt_term/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:09:04.922674 gpt-term-1.0.1/gpt_term.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-04-27 08:09:04.000000 gpt-term-1.0.1/gpt_term.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-27 08:09:04.000000 gpt-term-1.0.1/gpt_term.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:09:04.000000 gpt-term-1.0.1/gpt_term.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-27 08:09:04.000000 gpt-term-1.0.1/gpt_term.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-27 08:09:04.000000 gpt-term-1.0.1/gpt_term.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 08:09:04.000000 gpt-term-1.0.1/gpt_term.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 08:09:04.922674 gpt-term-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-27 08:08:52.000000 gpt-term-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:05:29.847288 gpt-term-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-11 09:05:16.000000 gpt-term-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 09:05:16.000000 gpt-term-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-05-11 09:05:29.847288 gpt-term-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13525 2023-05-11 09:05:16.000000 gpt-term-1.0.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-05-11 09:05:16.000000 gpt-term-1.0.2/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:05:29.847288 gpt-term-1.0.2/gpt_term/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 09:05:16.000000 gpt-term-1.0.2/gpt_term/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-11 09:05:16.000000 gpt-term-1.0.2/gpt_term/config.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48427 2023-05-11 09:05:16.000000 gpt-term-1.0.2/gpt_term/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:05:29.847288 gpt-term-1.0.2/gpt_term.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-05-11 09:05:29.000000 gpt-term-1.0.2/gpt_term.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-11 09:05:29.000000 gpt-term-1.0.2/gpt_term.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:05:29.000000 gpt-term-1.0.2/gpt_term.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 09:05:29.000000 gpt-term-1.0.2/gpt_term.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 09:05:29.000000 gpt-term-1.0.2/gpt_term.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 09:05:29.000000 gpt-term-1.0.2/gpt_term.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 09:05:29.847288 gpt-term-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-11 09:05:16.000000 gpt-term-1.0.2/setup.py
```

### Comparing `gpt-term-1.0.1/LICENSE` & `gpt-term-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-term-1.0.1/PKG-INFO` & `gpt-term-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: gpt-term
-Version: 1.0.1
-Summary: Use ChatGPT in terminal
-Home-page: https://github.com/xiaoxx970/chatgpt-in-terminal
-Author: xiaoxx970
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## Chat with GPT in Terminal
 
 [![English badge](https://img.shields.io/badge/%E8%8B%B1%E6%96%87-English-blue)](https://github.com/xiaoxx970/chatgpt-in-terminal/blob/main/README.md)
 [![简体中文 badge](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-Simplified%20Chinese-blue)](https://github.com/xiaoxx970/chatgpt-in-terminal/blob/main/README.zh-CN.md)
 [![Platform badge](https://img.shields.io/badge/Platform-MacOS%7CWindows%7CLinux-green)]()
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
 
@@ -31,20 +17,30 @@
 
 ![example](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/small.gif)
 
 Uses the [gpt-3.5-turbo](https://platform.openai.com/docs/guides/chat/chat-completions-beta) model, which is the same model used by ChatGPT (Free Edition), as default.
 
 ## Changelog
 
-### 2023-04-23
-Released `gpt-term` on [Pypi](https://pypi.org/project/gpt-term/), started version control. No need to clone the project locally anymore, simply use the `pip` command to install gpt-term.
+### 2023-05-11
+
+- Find the command the user most likely intended to enter when typing an unrecognized command
+
+### 2023-05-05
+
+- Add `/rand` command to set temperature parameter
+
+- Add overflow mode switch for `/stream` command, now you can run command `/stream visible` to switch to always visible mode. In this mode, the content that exceeds the screen will be scrolled up, and the new content will be output until it is completed
 
 <details>
   <summary>More Change log</summary>
 
+### 2023-04-23
+Released `gpt-term` on [Pypi](https://pypi.org/project/gpt-term/), started version control. No need to clone the project locally anymore, simply use the `pip` command to install gpt-term.
+
 ### 2023-04-15
 
 - Added the ability to create a line break in single-line mode using `Esc` + `Enter`
 
 ### 2023-04-13
 
 - Added the function of generating and setting the terminal title in the background, and now the client will use the summary of the first question content as the terminal title
@@ -123,14 +119,24 @@
 
 ```shell
 gpt-term
 ```
 
 When entering a question in single-line mode, use `Esc` + `Enter` to start a new line, and use `Enter` to submit the question.
 
+Here are some common shortcut keys (also shortcut keys for the shell):
+
+- `Ctrl+_`:	Undo
+- `Ctrl+L`: Clear screen, equivalent to `clear` command in shell
+- `Ctrl+C`: Stop the current answer or cancel the current input
+- `Tab`: Autocomplete commands or parameters
+- `Ctrl+U`: Delete all characters to the left of the cursor
+- `Ctrl+K`: Delete all characters to the right of the cursor
+- `Ctrl+W`: Delete the word to the left of the cursor
+
 > Original chat logs will be saved to `~/.gpt-term/chat.log`
 
 ### Available Arguments
 
 | Arguments     | Description                     | Example                                       |
 | ------------- | ------------------------------- | --------------------------------------------- |
 | -h, --help    | show this help message and exit | `gpt-term --help`                             |
@@ -184,14 +190,22 @@
   >
   > If pasting multi line text, single-line mode can also paste properly
 
 - `/stream`: disable or enable stream mode
 
    > In stream mode, the answer will start outputting as soon as the first response arrives, which can reducing waiting time. Stream mode is on by default.
 
+   - `/stream ellipsis` (default)
+
+     > Switch the mode of streaming output to auto omission, when the output content exceeds the screen, three small dots will be displayed at the bottom of the screen and wait until the output is completed
+
+   - `/stream visible`
+
+      > Toggle the streaming output mode to always visible, in this mode, the content that exceeds the screen will be scrolled up, and the new content will be output until it is completed. Note that in this mode the terminal will not properly clean up off-screen content.
+
 - `/tokens`: Display the total tokens spent and the tokens for the current conversation
 
   > GPT-3.5 has a token limit of 4096; use this command to check if you're approaching the limit
 
 - `/usage`: Display the API credits summary
 
   > This feature may not be stable. If it fails to operate, you can visit the [usage page](https://platform.openai.com/account/usage) to view further information.
@@ -216,14 +230,16 @@
 
 - `/save [filename_or_path]`: Save the chat history to the specified JSON file
 
   > If no filename or path is provided, the client will generate one, and if generation fails, the filename `chat_history_YEAR-MONTH-DAY_HOUR,MINUTE,SECOND.json` is suggested on input.
 
 - `/system [new_prompt]`: Modify the system prompt
 
+- `/rand [randomness]`: Set Model sampling temperature (0~2), higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic.
+
 - `/title [new_title]`: Set terminal title for this chat
 
   > If new_title is not provided, a new title will be generated based on first question
 
 - `/timeout [new_timeout]`: Modify API timeout.
 
   > The default timeout is 30 seconds, it can also be configured by setting `OPENAI_API_TIMEOUT=` in the `~/.gpt-term/config.ini` file.
@@ -275,18 +291,18 @@
 ## Project Structure
 
 ```sh
 .
 ├── LICENSE                   # License
 ├── README.md                 # Documentation
 ├── chat.py                   # Script entry point
-├── config.ini                # API key storage and other settings
 ├── gpt_term                  # Project package folder
 │   ├── __init__.py
+│   ├── config.ini            # API key storage and other settings
 │   └── main.py               # Main program
 ├── requirements.txt          # List of dependencies
 └── setup.py
 ```
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE).
+This project is licensed under the [MIT License](LICENSE).
```

### Comparing `gpt-term-1.0.1/README.md` & `gpt-term-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: gpt-term
+Version: 1.0.2
+Summary: Use ChatGPT in terminal
+Home-page: https://github.com/xiaoxx970/chatgpt-in-terminal
+Author: xiaoxx970
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## Chat with GPT in Terminal
 
 [![English badge](https://img.shields.io/badge/%E8%8B%B1%E6%96%87-English-blue)](https://github.com/xiaoxx970/chatgpt-in-terminal/blob/main/README.md)
 [![简体中文 badge](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-Simplified%20Chinese-blue)](https://github.com/xiaoxx970/chatgpt-in-terminal/blob/main/README.zh-CN.md)
 [![Platform badge](https://img.shields.io/badge/Platform-MacOS%7CWindows%7CLinux-green)]()
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
 
@@ -17,20 +31,30 @@
 
 ![example](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/small.gif)
 
 Uses the [gpt-3.5-turbo](https://platform.openai.com/docs/guides/chat/chat-completions-beta) model, which is the same model used by ChatGPT (Free Edition), as default.
 
 ## Changelog
 
-### 2023-04-23
-Released `gpt-term` on [Pypi](https://pypi.org/project/gpt-term/), started version control. No need to clone the project locally anymore, simply use the `pip` command to install gpt-term.
+### 2023-05-11
+
+- Find the command the user most likely intended to enter when typing an unrecognized command
+
+### 2023-05-05
+
+- Add `/rand` command to set temperature parameter
+
+- Add overflow mode switch for `/stream` command, now you can run command `/stream visible` to switch to always visible mode. In this mode, the content that exceeds the screen will be scrolled up, and the new content will be output until it is completed
 
 <details>
   <summary>More Change log</summary>
 
+### 2023-04-23
+Released `gpt-term` on [Pypi](https://pypi.org/project/gpt-term/), started version control. No need to clone the project locally anymore, simply use the `pip` command to install gpt-term.
+
 ### 2023-04-15
 
 - Added the ability to create a line break in single-line mode using `Esc` + `Enter`
 
 ### 2023-04-13
 
 - Added the function of generating and setting the terminal title in the background, and now the client will use the summary of the first question content as the terminal title
@@ -109,14 +133,24 @@
 
 ```shell
 gpt-term
 ```
 
 When entering a question in single-line mode, use `Esc` + `Enter` to start a new line, and use `Enter` to submit the question.
 
+Here are some common shortcut keys (also shortcut keys for the shell):
+
+- `Ctrl+_`:	Undo
+- `Ctrl+L`: Clear screen, equivalent to `clear` command in shell
+- `Ctrl+C`: Stop the current answer or cancel the current input
+- `Tab`: Autocomplete commands or parameters
+- `Ctrl+U`: Delete all characters to the left of the cursor
+- `Ctrl+K`: Delete all characters to the right of the cursor
+- `Ctrl+W`: Delete the word to the left of the cursor
+
 > Original chat logs will be saved to `~/.gpt-term/chat.log`
 
 ### Available Arguments
 
 | Arguments     | Description                     | Example                                       |
 | ------------- | ------------------------------- | --------------------------------------------- |
 | -h, --help    | show this help message and exit | `gpt-term --help`                             |
@@ -170,14 +204,22 @@
   >
   > If pasting multi line text, single-line mode can also paste properly
 
 - `/stream`: disable or enable stream mode
 
    > In stream mode, the answer will start outputting as soon as the first response arrives, which can reducing waiting time. Stream mode is on by default.
 
+   - `/stream ellipsis` (default)
+
+     > Switch the mode of streaming output to auto omission, when the output content exceeds the screen, three small dots will be displayed at the bottom of the screen and wait until the output is completed
+
+   - `/stream visible`
+
+      > Toggle the streaming output mode to always visible, in this mode, the content that exceeds the screen will be scrolled up, and the new content will be output until it is completed. Note that in this mode the terminal will not properly clean up off-screen content.
+
 - `/tokens`: Display the total tokens spent and the tokens for the current conversation
 
   > GPT-3.5 has a token limit of 4096; use this command to check if you're approaching the limit
 
 - `/usage`: Display the API credits summary
 
   > This feature may not be stable. If it fails to operate, you can visit the [usage page](https://platform.openai.com/account/usage) to view further information.
@@ -202,14 +244,16 @@
 
 - `/save [filename_or_path]`: Save the chat history to the specified JSON file
 
   > If no filename or path is provided, the client will generate one, and if generation fails, the filename `chat_history_YEAR-MONTH-DAY_HOUR,MINUTE,SECOND.json` is suggested on input.
 
 - `/system [new_prompt]`: Modify the system prompt
 
+- `/rand [randomness]`: Set Model sampling temperature (0~2), higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic.
+
 - `/title [new_title]`: Set terminal title for this chat
 
   > If new_title is not provided, a new title will be generated based on first question
 
 - `/timeout [new_timeout]`: Modify API timeout.
 
   > The default timeout is 30 seconds, it can also be configured by setting `OPENAI_API_TIMEOUT=` in the `~/.gpt-term/config.ini` file.
@@ -261,18 +305,18 @@
 ## Project Structure
 
 ```sh
 .
 ├── LICENSE                   # License
 ├── README.md                 # Documentation
 ├── chat.py                   # Script entry point
-├── config.ini                # API key storage and other settings
 ├── gpt_term                  # Project package folder
 │   ├── __init__.py
+│   ├── config.ini            # API key storage and other settings
 │   └── main.py               # Main program
 ├── requirements.txt          # List of dependencies
 └── setup.py
 ```
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE).
+This project is licensed under the [MIT License](LICENSE).
```

### Comparing `gpt-term-1.0.1/gpt_term/config.ini` & `gpt-term-1.0.2/gpt_term/config.ini`

 * *Files identical despite different names*

### Comparing `gpt-term-1.0.1/gpt_term/main.py` & `gpt-term-1.0.2/gpt_term/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 import pyperclip
 import requests
 import sseclient
 import tiktoken
 from packaging.version import parse as parse_version
 from prompt_toolkit import PromptSession, prompt
-from prompt_toolkit.completion import Completer, Completion
+from prompt_toolkit.completion import (Completer, Completion, NestedCompleter,
+                                       PathCompleter)
 from prompt_toolkit.key_binding import KeyBindings
 from prompt_toolkit.keys import Keys
 from prompt_toolkit.shortcuts import confirm
 from prompt_toolkit.styles import Style
 from prompt_toolkit.validation import ValidationError, Validator
 from rich import print as rprint
 from rich.console import Console, Group
@@ -66,34 +67,34 @@
     multi_line_mode = False
     stream_mode = True
 
     @classmethod
     def toggle_raw_mode(cls):
         cls.raw_mode = not cls.raw_mode
         console.print(
-            f"[dim]Raw mode {'enabled' if cls.raw_mode else 'disabled'}, use `/last` to display the last answer.")
+            f"[dim]Raw mode {'[green]enabled[/]' if cls.raw_mode else '[bright_red]disabled[/]'}, use `[bright_magenta]/last[/]` to display the last answer.")
 
     @classmethod
     def toggle_stream_mode(cls):
         cls.stream_mode = not cls.stream_mode
         if cls.stream_mode:
             console.print(
-                f"[dim]Stream mode enabled, the answer will start outputting as soon as the first response arrives.")
+                f"[dim]Stream mode [green]enabled[/], the answer will start outputting as soon as the first response arrives.")
         else:
             console.print(
-                f"[dim]Stream mode disabled, the answer is being displayed after the server finishes responding.")
+                f"[dim]Stream mode [bright_red]disabled[/], the answer is being displayed after the server finishes responding.")
 
     @classmethod
     def toggle_multi_line_mode(cls):
         cls.multi_line_mode = not cls.multi_line_mode
         if cls.multi_line_mode:
             console.print(
-                f"[dim]Multi-line mode enabled, press [[bright_magenta]Esc[/]] + [[bright_magenta]ENTER[/]] to submit.")
+                f"[dim]Multi-line mode [green]enabled[/], press [[bright_magenta]Esc[/]] + [[bright_magenta]ENTER[/]] to submit.")
         else:
-            console.print(f"[dim]Multi-line mode disabled.")
+            console.print(f"[dim]Multi-line mode [bright_red]disabled[/].")
 
 
 class ChatGPT:
     def __init__(self, api_key: str, timeout: float):
         self.api_key = api_key
         self.endpoint = "https://api.openai.com/v1/chat/completions"
         self.headers = {
@@ -102,21 +103,23 @@
         }
         self.messages = [
             {"role": "system", "content": f"You are a helpful assistant.\nKnowledge cutoff: 2021-09\nCurrent date: {datetime.now().strftime('%Y-%m-%d')}"}]
         self.model = 'gpt-3.5-turbo'
         self.tokens_limit = 4096
         # as default: gpt-3.5-turbo has a tokens limit as 4096
         # when model changes, tokens will also be changed
+        self.temperature = 1
         self.total_tokens_spent = 0
         self.current_tokens = count_token(self.messages)
         self.timeout = timeout
         self.title: str = None
         self.gen_title_messages = Queue()
         self.auto_gen_title_background_enable = True
         self.threadlock_total_tokens_spent = threading.Lock()
+        self.stream_overflow = 'ellipsis'
 
         self.credit_total_granted = 0
         self.credit_total_used = 0
         self.credit_used_this_month = 0
         self.credit_plan = ""
 
     def add_total_tokens(self, tokens: int):
@@ -171,15 +174,15 @@
         except requests.exceptions.RequestException as e:
             log.exception(e)
             return None
 
     def process_stream_response(self, response: requests.Response):
         reply: str = ""
         client = sseclient.SSEClient(response)
-        with Live(console=console, auto_refresh=False) as live:
+        with Live(console=console, auto_refresh=False, vertical_overflow=self.stream_overflow) as live:
             try:
                 rprint("[bold cyan]ChatGPT: ")
                 for event in client.events():
                     if event.data == '[DONE]':
                         # finish_reason = part["choices"][0]['finish_reason']
                         break
                     part = json.loads(event.data)
@@ -222,22 +225,31 @@
             tokens_saved = self.current_tokens - new_tokens
             self.current_tokens = new_tokens
 
             console.print(
                 f"[dim]First question: '{truncated_question}' and it's answer has been deleted, saved tokens: {tokens_saved}")
         else:
             console.print("[red]No conversations yet.")
+    
+    def delete_all_conversation(self):
+        del self.messages[1:]
+        self.title = None
+        # recount current tokens
+        self.current_tokens = count_token(self.messages)
+        os.system('cls' if os.name == 'nt' else 'clear')
+        console.print("[dim]Current chat cleared.")
 
     def handle(self, message: str):
         try:
             self.messages.append({"role": "user", "content": message})
             data = {
                 "model": self.model,
                 "messages": self.messages,
-                "stream": ChatMode.stream_mode
+                "stream": ChatMode.stream_mode,
+                "temperature": self.temperature
             }
             response = self.send_request(data)
             if response is None:
                 self.messages.pop()
                 if self.current_tokens >= self.tokens_limit:
                     if confirm("Reached tokens limit, do you want me to forget the earliest message of current chat?"):
                         self.delete_first_conversation()
@@ -471,90 +483,119 @@
             if len(self.messages) > 1:
                 console.print(
                     "[dim]Note this is not a new chat, modifications to the system prompt have limited impact on answers.")
         else:
             console.print(
                 f"[dim]No system prompt found in messages.")
 
+    def set_stream_overflow(self, new_overflow: str):
+        # turn on stream if not
+        if not ChatMode.stream_mode:
+            ChatMode.toggle_stream_mode()
+
+        if new_overflow == self.stream_overflow:
+            console.print("[dim]No change.")
+            return
+
+        old_overflow = self.stream_overflow
+        if new_overflow == 'ellipsis' or new_overflow == 'visible':
+            self.stream_overflow = new_overflow
+            console.print(
+                f"[dim]Stream overflow option has been modified from '{old_overflow}' to '{new_overflow}'.")
+            if new_overflow == 'visible':
+                console.print("[dim]Note that in this mode the terminal will not properly clean up off-screen content.")
+        else:
+            console.print(f"[dim]No such Stream overflow option, remain '{old_overflow}' unchanged.")
+        
+
     def set_model(self, new_model: str):
         old_model = self.model
         if not new_model:
             console.print(
                 f"[dim]Empty input, the model remains '{old_model}'.")
             return
         self.model = str(new_model)
         if "gpt-4-32k" in self.model:
             self.tokens_limit = 32768
         elif "gpt-4" in self.model:
             self.tokens_limit = 8192
         elif "gpt-3.5-turbo" in self.model:
             self.tokens_limit = 4096
         else:
-            self.tokens_limit = -1
+            self.tokens_limit = float('nan')
         console.print(
             f"[dim]Model has been set from '{old_model}' to '{new_model}'.")
 
     def set_timeout(self, timeout):
         try:
             self.timeout = float(timeout)
         except ValueError:
             console.print("[red]Input must be a number")
             return
         console.print(f"[dim]API timeout set to [green]{timeout}s[/].")
 
+    def set_temperature(self, temperature):
+        try:
+            new_temperature = float(temperature)
+        except ValueError:
+            console.print("[red]Input must be a number between 0 and 2")
+            return
+        if new_temperature > 2 or new_temperature < 0:
+            console.print("[red]Input must be a number between 0 and 2")
+            return
+        self.temperature = new_temperature
+        console.print(f"[dim]Randomness set to [green]{temperature}[/].")
+
 
-class CustomCompleter(Completer):
-    commands = [
-        '/raw', '/multi', '/stream', '/tokens', '/usage', '/last', '/copy', '/model', '/save', '/system', '/title', '/timeout', '/undo', '/delete', '/version', '/help', '/exit'
-    ]
-
-    copy_actions = [
-        "code",
-        "all"
-    ]
-
-    delete_actions = [
-        "first",
-        "all"
-    ]
-
-    available_models = [
-        "gpt-3.5-turbo",
-        "gpt-3.5-turbo-0301",
-        "gpt-4",
-        "gpt-4-0314",
-        "gpt-4-32k",
-        "gpt-4-32k-0314",
-    ]
+class CommandCompleter(Completer):
+    def __init__(self):
+        self.nested_completer = NestedCompleter.from_nested_dict({
+            '/raw': None,
+            '/multi': None,
+            '/stream': {"visible", "ellipsis"},
+            '/tokens': None,
+            '/usage': None,
+            '/last': None,
+            '/copy': {"code", "all"},
+            '/model': {
+                "gpt-3.5-turbo",
+                "gpt-3.5-turbo-0301",
+                "gpt-4",
+                "gpt-4-0314",
+                "gpt-4-32k",
+                "gpt-4-32k-031"},
+            '/save': PathCompleter(file_filter=self.path_filter),
+            '/system': None,
+            '/rand': None,
+            '/temperature': None,
+            '/title': None,
+            '/timeout': None,
+            '/undo': None,
+            '/delete': {"first", "all"},
+            '/reset': None,
+            '/version': None,
+            '/help': None,
+            '/exit': None,
+        })
+
+    def path_filter(self, filename):
+        # 路径自动补全，只补全json文件和文件夹
+        return filename.endswith(".json") or os.path.isdir(filename)
 
     def get_completions(self, document, complete_event):
         text = document.text_before_cursor
         if text.startswith('/'):
-            # Check if it's a /model command
-            if text.startswith('/model '):
-                model_prefix = text[7:]
-                for model in self.available_models:
-                    if model.startswith(model_prefix):
-                        yield Completion(model, start_position=-len(model_prefix))
-            # Check if it's a /copy command
-            elif text.startswith('/copy '):
-                copy_prefix = text[6:]
-                for copy in self.copy_actions:
-                    if copy.startswith(copy_prefix):
-                        yield Completion(copy, start_position=-len(copy_prefix))
-            # Check if it's a /delete command
-            elif text.startswith('/delete '):
-                delete_prefix = text[8:]
-                for delete in self.delete_actions:
-                    if delete.startswith(delete_prefix):
-                        yield Completion(delete, start_position=-len(delete_prefix))
-            else:
-                for command in self.commands:
-                    if command.startswith(text):
-                        yield Completion(command, start_position=-len(text))
+            for cmd in self.nested_completer.options.keys():
+                # 如果匹配到第一层命令
+                if text in cmd:
+                    yield Completion(cmd, start_position=-len(text))
+            # 如果匹配到第n层命令
+            if ' ' in text:
+                for sub_cmd in self.nested_completer.get_completions(document, complete_event):
+                    yield sub_cmd
 
 
 def count_token(messages: List[Dict[str, str]]):
     '''计算 messages 占用的 token
     `cl100k_base` 编码适用于: gpt-4, gpt-3.5-turbo, text-embedding-ada-002'''
     encoding = tiktoken.get_encoding("cl100k_base")
     length = 0
@@ -566,14 +607,31 @@
 class NumberValidator(Validator):
     def validate(self, document):
         text = document.text
         if not text.isdigit():
             raise ValidationError(message="Please input an Integer!",
                                   cursor_position=len(text))
 
+class FloatRangeValidator(Validator):
+    def __init__(self, min_value=None, max_value=None):
+        self.min_value = min_value
+        self.max_value = max_value
+
+    def validate(self, document):
+        try:
+            value = float(document.text)
+        except ValueError:
+            raise ValidationError(message='Input must be a number')
+
+        if self.min_value is not None and value < self.min_value:
+            raise ValidationError(message=f'Input must be at least {self.min_value}')
+        if self.max_value is not None and value > self.max_value:
+            raise ValidationError(message=f'Input must be at most {self.max_value}')
+        
+temperature_validator = FloatRangeValidator(min_value=0.0, max_value=2.0)
 
 def print_message(message: Dict[str, str]):
     '''打印单条来自 ChatGPT 或用户的消息'''
     role = message["role"]
     content = message["content"]
     if role == "user":
         print(f"> {content}")
@@ -637,23 +695,46 @@
         os.system(f"title {new_title}")
     else:
         print(f"\033]0;{new_title}\007", end='')
         sys.stdout.flush()
         # flush the stdout buffer in order to making the control sequences effective immediately
     log.debug(f"CLI Title changed to '{new_title}'")
 
+def get_levenshtein_distance(s1: str, s2: str):
+    s1_len = len(s1)
+    s2_len = len(s2)
+
+    v = [[0 for _ in range(s2_len+1)] for _ in range(s1_len+1)]
+    for i in range(0, s1_len+1):
+        for j in range(0, s2_len+1):
+            if i == 0:
+                v[i][j] = j
+            elif j == 0:
+                v[i][j] = i
+            elif s1[i-1] == s2[j-1]:
+                v[i][j] = v[i-1][j-1]
+            else:
+                v[i][j] = min(v[i-1][j-1], min(v[i][j-1], v[i-1][j])) + 1
+
+    return v[s1_len][s2_len]
+
 
 def handle_command(command: str, chat_gpt: ChatGPT, key_bindings: KeyBindings, chat_save_perfix: str):
     '''处理斜杠(/)命令'''
     if command == '/raw':
         ChatMode.toggle_raw_mode()
     elif command == '/multi':
         ChatMode.toggle_multi_line_mode()
-    elif command == '/stream':
-        ChatMode.toggle_stream_mode()
+
+    elif command.startswith('/stream'):
+        args = command.split()
+        if len(args) > 1:
+            chat_gpt.set_stream_overflow(args[1])
+        else:
+            ChatMode.toggle_stream_mode()
 
     elif command == '/tokens':
         chat_gpt.threadlock_total_tokens_spent.acquire()
         console.print(Panel(f"[bold bright_magenta]Total Tokens Spent:[/]\t{chat_gpt.total_tokens_spent}\n"
                             f"[bold green]Current Tokens:[/]\t\t{chat_gpt.current_tokens}/[bold]{chat_gpt.tokens_limit}",
                             title='token_summary', title_align='left', width=40))
         chat_gpt.threadlock_total_tokens_spent.release()
@@ -661,15 +742,15 @@
     elif command == '/usage':
         with console.status("[cyan]Getting credit usage..."):
             if not chat_gpt.get_credit_usage():
                 return
         console.print(Panel(f"[bold green]Total Granted:[/]\t\t${format(chat_gpt.credit_total_granted, '.2f')}\n"
                             f"[bold cyan]Used This Month:[/]\t${format(chat_gpt.credit_used_this_month, '.2f')}\n"
                             f"[bold blue]Used Total:[/]\t\t${format(chat_gpt.credit_total_used, '.2f')}",
-                            title="Credit Summary", title_align='left', subtitle=f"[blue]Plan: {chat_gpt.credit_plan}", width=35))
+                            title="Credit Summary", title_align='left', subtitle=f"[bright_blue]Plan: {chat_gpt.credit_plan}", width=35))
 
     elif command.startswith('/model'):
         args = command.split()
         if len(args) > 1:
             new_model = args[1]
         else:
             new_model = prompt(
@@ -726,14 +807,26 @@
             new_content = prompt(
                 "System prompt: ", default=chat_gpt.messages[0]['content'], style=style, key_bindings=key_bindings)
         if new_content != chat_gpt.messages[0]['content']:
             chat_gpt.modify_system_prompt(new_content)
         else:
             console.print("[dim]No change.")
 
+    elif command.startswith('/rand') or command.startswith('/temperature'):
+        args = command.split()
+        if len(args) > 1:
+            new_temperature = args[1]
+        else:
+            new_temperature = prompt(
+                "New Randomness: ", default=str(chat_gpt.temperature), style=style, validator=temperature_validator)
+        if new_temperature != str(chat_gpt.temperature):
+            chat_gpt.set_temperature(new_temperature)
+        else:
+            console.print("[dim]No change.")            
+
     elif command.startswith('/title'):
         args = command.split()
         if len(args) > 1:
             chat_gpt.title = ' '.join(args[1:])
             change_CLI_title(chat_gpt.title)
         else:
             # generate a new title
@@ -765,25 +858,24 @@
                 truncated_question += "..."
             console.print(
                 f"[dim]Last question: '{truncated_question}' and it's answer has been removed.")
             chat_gpt.current_tokens = count_token(chat_gpt.messages)
         else:
             console.print("[dim]Nothing to undo.")
 
+    elif command.startswith('/reset'):
+        chat_gpt.delete_all_conversation()
+
     elif command.startswith('/delete'):
         args = command.split()
         if len(args) > 1:
             if args[1] == 'first':
                 chat_gpt.delete_first_conversation()
             elif args[1] == 'all':
-                del chat_gpt.messages[1:]
-                chat_gpt.title = None
-                chat_gpt.current_tokens = count_token(chat_gpt.messages)
-                # recount current tokens
-                console.print("[dim]Current chat deleted.")
+                chat_gpt.delete_all_conversation()
             else:
                 console.print(
                     "[dim]Nothing to do. Avaliable delete command: `[bright_magenta]/delete first[/]` or `[bright_magenta]/delete all[/]`")
         else:
             chat_gpt.delete_first_conversation()
 
     elif command == '/version':
@@ -792,35 +884,55 @@
                             f"[bold green]Remote Version:[/]\tv{str(remote_version)}",
                             title='Version', title_align='left', width=28))
         threadlock_remote_version.release()
 
     elif command == '/exit':
         raise EOFError
 
-    else:
+    elif command == '/help':
         console.print('''[bold]Available commands:[/]
     /raw                     - Toggle raw mode (showing raw text of ChatGPT's reply)
     /multi                   - Toggle multi-line mode (allow multi-line input)
-    /stream                  - Toggle stream output mode (flow print the answer)
+    /stream \[overflow_mode]  - Toggle stream output mode (flow print the answer)
     /tokens                  - Show the total tokens spent and the tokens for the current conversation
     /usage                   - Show total credits and current credits used
     /last                    - Display last ChatGPT's reply
     /copy (all)              - Copy the full ChatGPT's last reply (raw) to Clipboard
     /copy code \[index]       - Copy the code in ChatGPT's last reply to Clipboard
     /save \[filename_or_path] - Save the chat history to a file, suggest title if filename_or_path not provided
     /model \[model_name]      - Change AI model
     /system \[new_prompt]     - Modify the system prompt
+    /rand \[randomness]       - Set Model sampling temperature (0~2)
     /title \[new_title]       - Set title for this chat, if new_title is not provided, a new title will be generated
     /timeout \[new_timeout]   - Modify the api timeout
     /undo                    - Undo the last question and remove its answer
     /delete (first)          - Delete the first conversation in current chat
     /delete all              - Clear all messages and conversations current chat
     /version                 - Show gpt-term local and remote version
     /help                    - Show this help message
     /exit                    - Exit the application''')
+        
+    else:
+        set_command = set(command)
+        min_levenshtein_distance = len(command)
+        most_similar_command = ""
+        for slash_command in CustomCompleter.commands:
+            this_levenshtein_distance = get_levenshtein_distance(command, slash_command)
+            if this_levenshtein_distance < min_levenshtein_distance:
+                set_slash_command = set(slash_command)
+                if len(set_command & set_slash_command) / len(set_command | set_slash_command) >= 0.75:
+                    most_similar_command = slash_command
+                    min_levenshtein_distance = this_levenshtein_distance
+        
+        console.print(f"Unrecognized Slash Command `[bold red]{command}[/]`", end=" ")
+        if most_similar_command:
+            console.print(f"Do you mean `[bright magenta]{most_similar_command}[/]`?")
+        else:
+            console.print("")
+        console.print("Use `[bright magenta]/help[/]` to see all available slash commands")
 
 
 def load_chat_history(file_path):
     '''从 file_path 加载聊天记录'''
     try:
         with open(file_path, 'r', encoding='utf-8') as f:
             chat_history = json.load(f)
@@ -964,15 +1076,15 @@
 
     chat_save_perfix = config.get("CHAT_SAVE_PERFIX", "./chat_history_")
 
     chat_gpt = ChatGPT(api_key, api_timeout)
 
     if not config.getboolean("AUTO_GENERATE_TITLE", True):
         chat_gpt.auto_gen_title_background_enable = False
-        log.debug("Auto title generation disabled")
+        log.debug("Auto title generation [bright_red]disabled[/]")
 
     gen_title_daemon_thread = threading.Thread(
         target=chat_gpt.auto_gen_title_background, daemon=True)
     gen_title_daemon_thread.start()
     log.debug("Title generation daemon thread started")
 
     console.print(
@@ -998,23 +1110,23 @@
             log.info(f"Chat history successfully loaded from: {args.load}")
             console.print(
                 f"[dim]Chat history successfully loaded from: [bright_magenta]{args.load}", highlight=False)
 
     session = PromptSession()
 
     # 自定义命令补全，保证输入‘/’后继续显示补全
-    commands = CustomCompleter()
+    command_completer = CommandCompleter()
 
     # 绑定回车事件，达到自定义多行模式的效果
     key_bindings = create_key_bindings()
 
     while True:
         try:
             message = session.prompt(
-                '> ', completer=commands, complete_while_typing=True, key_bindings=key_bindings)
+                '> ', completer=command_completer, complete_while_typing=True, key_bindings=key_bindings)
 
             if message.startswith('/'):
                 command = message.strip().lower()
                 handle_command(command, chat_gpt,
                                key_bindings, chat_save_perfix)
             else:
                 if not message:
```

### Comparing `gpt-term-1.0.1/gpt_term.egg-info/PKG-INFO` & `gpt-term-1.0.2/gpt_term.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-term
-Version: 1.0.1
+Version: 1.0.2
 Summary: Use ChatGPT in terminal
 Home-page: https://github.com/xiaoxx970/chatgpt-in-terminal
 Author: xiaoxx970
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,20 +31,30 @@
 
 ![example](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/small.gif)
 
 Uses the [gpt-3.5-turbo](https://platform.openai.com/docs/guides/chat/chat-completions-beta) model, which is the same model used by ChatGPT (Free Edition), as default.
 
 ## Changelog
 
-### 2023-04-23
-Released `gpt-term` on [Pypi](https://pypi.org/project/gpt-term/), started version control. No need to clone the project locally anymore, simply use the `pip` command to install gpt-term.
+### 2023-05-11
+
+- Find the command the user most likely intended to enter when typing an unrecognized command
+
+### 2023-05-05
+
+- Add `/rand` command to set temperature parameter
+
+- Add overflow mode switch for `/stream` command, now you can run command `/stream visible` to switch to always visible mode. In this mode, the content that exceeds the screen will be scrolled up, and the new content will be output until it is completed
 
 <details>
   <summary>More Change log</summary>
 
+### 2023-04-23
+Released `gpt-term` on [Pypi](https://pypi.org/project/gpt-term/), started version control. No need to clone the project locally anymore, simply use the `pip` command to install gpt-term.
+
 ### 2023-04-15
 
 - Added the ability to create a line break in single-line mode using `Esc` + `Enter`
 
 ### 2023-04-13
 
 - Added the function of generating and setting the terminal title in the background, and now the client will use the summary of the first question content as the terminal title
@@ -123,14 +133,24 @@
 
 ```shell
 gpt-term
 ```
 
 When entering a question in single-line mode, use `Esc` + `Enter` to start a new line, and use `Enter` to submit the question.
 
+Here are some common shortcut keys (also shortcut keys for the shell):
+
+- `Ctrl+_`:	Undo
+- `Ctrl+L`: Clear screen, equivalent to `clear` command in shell
+- `Ctrl+C`: Stop the current answer or cancel the current input
+- `Tab`: Autocomplete commands or parameters
+- `Ctrl+U`: Delete all characters to the left of the cursor
+- `Ctrl+K`: Delete all characters to the right of the cursor
+- `Ctrl+W`: Delete the word to the left of the cursor
+
 > Original chat logs will be saved to `~/.gpt-term/chat.log`
 
 ### Available Arguments
 
 | Arguments     | Description                     | Example                                       |
 | ------------- | ------------------------------- | --------------------------------------------- |
 | -h, --help    | show this help message and exit | `gpt-term --help`                             |
@@ -184,14 +204,22 @@
   >
   > If pasting multi line text, single-line mode can also paste properly
 
 - `/stream`: disable or enable stream mode
 
    > In stream mode, the answer will start outputting as soon as the first response arrives, which can reducing waiting time. Stream mode is on by default.
 
+   - `/stream ellipsis` (default)
+
+     > Switch the mode of streaming output to auto omission, when the output content exceeds the screen, three small dots will be displayed at the bottom of the screen and wait until the output is completed
+
+   - `/stream visible`
+
+      > Toggle the streaming output mode to always visible, in this mode, the content that exceeds the screen will be scrolled up, and the new content will be output until it is completed. Note that in this mode the terminal will not properly clean up off-screen content.
+
 - `/tokens`: Display the total tokens spent and the tokens for the current conversation
 
   > GPT-3.5 has a token limit of 4096; use this command to check if you're approaching the limit
 
 - `/usage`: Display the API credits summary
 
   > This feature may not be stable. If it fails to operate, you can visit the [usage page](https://platform.openai.com/account/usage) to view further information.
@@ -216,14 +244,16 @@
 
 - `/save [filename_or_path]`: Save the chat history to the specified JSON file
 
   > If no filename or path is provided, the client will generate one, and if generation fails, the filename `chat_history_YEAR-MONTH-DAY_HOUR,MINUTE,SECOND.json` is suggested on input.
 
 - `/system [new_prompt]`: Modify the system prompt
 
+- `/rand [randomness]`: Set Model sampling temperature (0~2), higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic.
+
 - `/title [new_title]`: Set terminal title for this chat
 
   > If new_title is not provided, a new title will be generated based on first question
 
 - `/timeout [new_timeout]`: Modify API timeout.
 
   > The default timeout is 30 seconds, it can also be configured by setting `OPENAI_API_TIMEOUT=` in the `~/.gpt-term/config.ini` file.
@@ -275,17 +305,17 @@
 ## Project Structure
 
 ```sh
 .
 ├── LICENSE                   # License
 ├── README.md                 # Documentation
 ├── chat.py                   # Script entry point
-├── config.ini                # API key storage and other settings
 ├── gpt_term                  # Project package folder
 │   ├── __init__.py
+│   ├── config.ini            # API key storage and other settings
 │   └── main.py               # Main program
 ├── requirements.txt          # List of dependencies
 └── setup.py
 ```
 
 ## License
```

### Comparing `gpt-term-1.0.1/setup.py` & `gpt-term-1.0.2/setup.py`

 * *Files identical despite different names*

