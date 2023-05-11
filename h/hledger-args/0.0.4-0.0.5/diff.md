# Comparing `tmp/hledger_args-0.0.4.tar.gz` & `tmp/hledger_args-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hledger_args-0.0.4.tar", last modified: Wed May 10 18:06:18 2023, max compression
+gzip compressed data, was "hledger_args-0.0.5.tar", last modified: Thu May 11 02:16:36 2023, max compression
```

## Comparing `hledger_args-0.0.4.tar` & `hledger_args-0.0.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:06:18.090762 hledger_args-0.0.4/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4210 2023-05-10 18:06:18.090762 hledger_args-0.0.4/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3870 2023-05-10 18:04:25.000000 hledger_args-0.0.4/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:06:18.086763 hledger_args-0.0.4/docs/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3870 2023-05-10 18:04:25.000000 hledger_args-0.0.4/docs/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:06:18.087762 hledger_args-0.0.4/hledger_args/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:28.000000 hledger_args-0.0.4/hledger_args/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       84 2023-05-09 19:53:32.000000 hledger_args-0.0.4/hledger_args/__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1288 2023-05-09 16:59:35.000000 hledger_args-0.0.4/hledger_args/base_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1199 2023-05-09 16:57:24.000000 hledger_args-0.0.4/hledger_args/batch_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3016 2023-05-10 17:51:43.000000 hledger_args-0.0.4/hledger_args/cli.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3425 2023-05-10 18:03:07.000000 hledger_args-0.0.4/hledger_args/inter_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3115 2023-05-09 16:55:37.000000 hledger_args-0.0.4/hledger_args/options.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:06:18.088763 hledger_args-0.0.4/hledger_args.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4210 2023-05-10 18:06:18.000000 hledger_args-0.0.4/hledger_args.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      718 2023-05-10 18:06:18.000000 hledger_args-0.0.4/hledger_args.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-10 18:06:18.000000 hledger_args-0.0.4/hledger_args.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-05-10 18:06:18.000000 hledger_args-0.0.4/hledger_args.egg-info/entry_points.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       29 2023-05-10 18:06:18.000000 hledger_args-0.0.4/hledger_args.egg-info/requires.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       40 2023-05-10 18:06:18.000000 hledger_args-0.0.4/hledger_args.egg-info/top_level.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1152 2023-05-10 18:04:42.000000 hledger_args-0.0.4/pyproject.toml
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-10 18:06:18.090762 hledger_args-0.0.4/setup.cfg
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:06:18.088763 hledger_args-0.0.4/tests/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:22.000000 hledger_args-0.0.4/tests/__init__.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:06:18.083763 hledger_args-0.0.4/venv/
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:06:18.090762 hledger_args-0.0.4/venv/bin/
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2html.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2html4.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2html5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2latex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2man.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2odt.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2s5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2xetex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2xml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rstpep2html.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-11 02:16:36.423049 hledger_args-0.0.5/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4504 2023-05-11 02:16:36.423049 hledger_args-0.0.5/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4164 2023-05-11 02:06:47.000000 hledger_args-0.0.5/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-11 02:16:36.415049 hledger_args-0.0.5/docs/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4164 2023-05-11 02:06:47.000000 hledger_args-0.0.5/docs/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-11 02:16:36.417049 hledger_args-0.0.5/hledger_args/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:28.000000 hledger_args-0.0.5/hledger_args/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       84 2023-05-09 19:53:32.000000 hledger_args-0.0.5/hledger_args/__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1288 2023-05-09 16:59:35.000000 hledger_args-0.0.5/hledger_args/base_args.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1199 2023-05-09 16:57:24.000000 hledger_args-0.0.5/hledger_args/batch_args.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3132 2023-05-11 02:12:14.000000 hledger_args-0.0.5/hledger_args/cli.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4684 2023-05-11 02:15:32.000000 hledger_args-0.0.5/hledger_args/inter_args.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3115 2023-05-09 16:55:37.000000 hledger_args-0.0.5/hledger_args/options.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-11 02:16:36.418049 hledger_args-0.0.5/hledger_args.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4504 2023-05-11 02:16:36.000000 hledger_args-0.0.5/hledger_args.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      718 2023-05-11 02:16:36.000000 hledger_args-0.0.5/hledger_args.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-11 02:16:36.000000 hledger_args-0.0.5/hledger_args.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-05-11 02:16:36.000000 hledger_args-0.0.5/hledger_args.egg-info/entry_points.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       29 2023-05-11 02:16:36.000000 hledger_args-0.0.5/hledger_args.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       40 2023-05-11 02:16:36.000000 hledger_args-0.0.5/hledger_args.egg-info/top_level.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1152 2023-05-11 02:14:53.000000 hledger_args-0.0.5/pyproject.toml
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-11 02:16:36.424049 hledger_args-0.0.5/setup.cfg
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-11 02:16:36.418049 hledger_args-0.0.5/tests/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:22.000000 hledger_args-0.0.5/tests/__init__.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-11 02:16:36.415049 hledger_args-0.0.5/venv/
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-11 02:16:36.423049 hledger_args-0.0.5/venv/bin/
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-05-09 16:48:40.000000 hledger_args-0.0.5/venv/bin/rst2html.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-05-09 16:48:40.000000 hledger_args-0.0.5/venv/bin/rst2html4.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-05-09 16:48:40.000000 hledger_args-0.0.5/venv/bin/rst2html5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-05-09 16:48:40.000000 hledger_args-0.0.5/venv/bin/rst2latex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-05-09 16:48:40.000000 hledger_args-0.0.5/venv/bin/rst2man.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-05-09 16:48:40.000000 hledger_args-0.0.5/venv/bin/rst2odt.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-05-09 16:48:40.000000 hledger_args-0.0.5/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-05-09 16:48:40.000000 hledger_args-0.0.5/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-05-09 16:48:40.000000 hledger_args-0.0.5/venv/bin/rst2s5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-05-09 16:48:40.000000 hledger_args-0.0.5/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-05-09 16:48:40.000000 hledger_args-0.0.5/venv/bin/rst2xml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-05-09 16:48:40.000000 hledger_args-0.0.5/venv/bin/rstpep2html.py
```

### Comparing `hledger_args-0.0.4/PKG-INFO` & `hledger_args-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hledger_args
-Version: 0.0.4
+Version: 0.0.5
 License: MIT License
 Project-URL: homepage, https://github.com/edkedk99/hledger-args
 Project-URL: documentation, https://edkedk99.github.io/hledger-args/
 Project-URL: repository, https://github.com/edkedk99/hledger-args
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -20,18 +20,21 @@
 
 Instead of giving the the desired command thru a command-line argument, choose it by selecting from a menu using the flag *--interactive*
 
 ### Special placeholders
 
 | Placeholders | Description                                                                    |
 |--------------|--------------------------------------------------------------------------------|
-| {account}    | fuzzy search existing accounts or new                                          |
-| {payee}      | fuzzy search existing payee or new                                             |
-| {tag}        | fuzzy search existing tags and values or new                                   |
+| {account}    | fuzzy search existing accounts                                                 |
+| {payee}      | fuzzy search existing payee                                                    |
+| {tag}        | fuzzy search existing tags and values                                          |
+| {tag_name}   | search tag name after "_" and fuzzy search existing values for this tag        |
 | {months}     | prompt initial and end dates both inclusive. **Diferent from default hledger** |
+| {type}       | select between accounts type                                                   |
+| {cur}        | fuzzy search existing commodities                                              |
 
 
 ## Installation
 
 ### Dependencies
 
 - python 3.8
```

### Comparing `hledger_args-0.0.4/README.md` & `hledger_args-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,21 @@
 
 Instead of giving the the desired command thru a command-line argument, choose it by selecting from a menu using the flag *--interactive*
 
 ### Special placeholders
 
 | Placeholders | Description                                                                    |
 |--------------|--------------------------------------------------------------------------------|
-| {account}    | fuzzy search existing accounts or new                                          |
-| {payee}      | fuzzy search existing payee or new                                             |
-| {tag}        | fuzzy search existing tags and values or new                                   |
+| {account}    | fuzzy search existing accounts                                                 |
+| {payee}      | fuzzy search existing payee                                                    |
+| {tag}        | fuzzy search existing tags and values                                          |
+| {tag_name}   | search tag name after "_" and fuzzy search existing values for this tag        |
 | {months}     | prompt initial and end dates both inclusive. **Diferent from default hledger** |
+| {type}       | select between accounts type                                                   |
+| {cur}        | fuzzy search existing commodities                                              |
 
 
 ## Installation
 
 ### Dependencies
 
 - python 3.8
```

### Comparing `hledger_args-0.0.4/docs/README.md` & `hledger_args-0.0.5/docs/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,21 @@
 
 Instead of giving the the desired command thru a command-line argument, choose it by selecting from a menu using the flag *--interactive*
 
 ### Special placeholders
 
 | Placeholders | Description                                                                    |
 |--------------|--------------------------------------------------------------------------------|
-| {account}    | fuzzy search existing accounts or new                                          |
-| {payee}      | fuzzy search existing payee or new                                             |
-| {tag}        | fuzzy search existing tags and values or new                                   |
+| {account}    | fuzzy search existing accounts                                                 |
+| {payee}      | fuzzy search existing payee                                                    |
+| {tag}        | fuzzy search existing tags and values                                          |
+| {tag_name}   | search tag name after "_" and fuzzy search existing values for this tag        |
 | {months}     | prompt initial and end dates both inclusive. **Diferent from default hledger** |
+| {type}       | select between accounts type                                                   |
+| {cur}        | fuzzy search existing commodities                                              |
 
 
 ## Installation
 
 ### Dependencies
 
 - python 3.8
```

### Comparing `hledger_args-0.0.4/hledger_args/base_args.py` & `hledger_args-0.0.5/hledger_args/base_args.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.4/hledger_args/batch_args.py` & `hledger_args-0.0.5/hledger_args/batch_args.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.4/hledger_args/cli.py` & `hledger_args-0.0.5/hledger_args/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
      In basic usage, this package is a replacement for [hledger argument file](https://hledger.org/1.29/hledger.html#command-arguments) using custom directives inside the journal file, instead of referencing to an argument file
 
      **Interactive Mode**: Instead of giving the desired command thru a command-line argument, choose it by selecting from a menu using the flag *--interactive*
 
      **Placeholder Command Substitution**: In Interactive Mode, a command can use placeholders by putting them between *curly braces* and additional prompts wil ask for the value and do the proper substitution
 
-     **Special Placeholders**: *{account}, {payee}, {tag} and {months}* are special placeholders that offers autocomplete with fuzzy search using data from the journal
+     **Special Placeholders**: *{account}, {payee}, {tag}, {tag_name}, {months}, {type}, {cur}* are special placeholders that offers autocomplete with fuzzy search using data from the journal. See the [README](https://github.com/edkedk99/hledger-args) for explanation on each of them
 
      **Sub directive format**:
 
      ```text
      #+args [command name]:[hledger options]
      #+args [other command_name]:[other hledger options]
      ```
```

### Comparing `hledger_args-0.0.4/hledger_args/inter_args.py` & `hledger_args-0.0.5/hledger_args/inter_args.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,34 +5,42 @@
 
 import questionary
 from prompt_toolkit.shortcuts import CompleteStyle
 
 from .base_args import BaseArgs
 
 
+def val_date(date: str):
+    try:
+        datetime.strptime(date, "%Y-%m-%d")
+        return True
+    except ValueError:
+        return "Invalid date format"
+
+
+def val_existing(choices: List[str], value: str):
+    if value in choices:
+        return True
+    else:
+        return "Only existing values are accepted"
+
+
 def custom_autocomplete(name: str, choices: List[str]):
     question = questionary.autocomplete(
         f"{name} (TAB to autocomplete)",
         choices=choices,
+        validate=lambda value: val_existing(choices, value),
         ignore_case=True,
         match_middle=True,
         style=questionary.Style([("answer", "fg:#f71b07")]),
         complete_style=CompleteStyle.MULTI_COLUMN,
     )
     return question
 
 
-def val_date(date: str):
-    try:
-        datetime.strptime(date, "%Y-%m-%d")
-        return True
-    except ValueError:
-        return "Invalid date format"
-
-
 class InteractiveArgs(BaseArgs):
     def __init__(self, files: Tuple[str, ...]) -> None:
         super().__init__(files)
 
     def ask_placeholder(self, placeholder: str) -> str:
         if placeholder == "account":
             choices = self.get_hledger_lines(["accounts"])
@@ -42,28 +50,54 @@
             tag = custom_autocomplete(placeholder, choices=tags).ask()
 
             tag_values = self.get_hledger_lines(["tags", tag, "--values"])
             value = custom_autocomplete(
                 f"Value for tag {tag}", choices=tag_values
             ).ask()
             answer = f'"tag:{tag}={value}"'
+        elif placeholder.startswith("tag_"):
+            tag_name = placeholder.split("_", 1)[1]
+            tag_values = self.get_hledger_lines(["tags", tag_name, "--values"])
+            value = custom_autocomplete(
+                f"Value for tag {tag_name}", choices=tag_values
+            ).ask()
+            answer = f'"tag:{tag_name}={value}"'
         elif placeholder == "months":
             initial: str = questionary.text(
                 "Initial", instruction="YYYY-MM-DD", validate=val_date
             ).ask()
             final = questionary.text(
                 "Final (inclusive)", instruction="YYYY-MM-DD", validate=val_date
             ).ask()
             next_final_date = datetime.strptime(final, "%Y-%m-%d") + timedelta(days=1)
             next_final = next_final_date.strftime("%Y-%m-%d")
             answer = f"--begin {initial} --end {next_final}"
         elif placeholder == "payee":
             choices = self.get_hledger_lines(["payees"])
             payee = custom_autocomplete(placeholder, choices).ask()
             answer = f'"payee:{payee}"'
+        elif placeholder == "cur":
+            choices = self.get_hledger_lines(["commodities"])
+            commodity = custom_autocomplete(placeholder, choices).ask()
+            answer = f'"cur:{commodity}"'
+        elif placeholder == "type":
+            types = dict(
+                Asset="A",
+                Liability="L",
+                Equity="E",
+                Revenue="R",
+                Expense="X",
+                Cash="C",
+                Conversion="V",
+            )
+            choices = list(types.keys())
+            _type = questionary.select("Account Type", choices=choices).ask()
+            type_code = types[_type]
+            answer = f'"type:{type_code}"'
+
         else:
             answer = questionary.text(placeholder).ask()
 
         return answer
 
     def substitute(self, match: re.Match):
         placeholder: Optional[str] = match.group(1)
```

### Comparing `hledger_args-0.0.4/hledger_args/options.py` & `hledger_args-0.0.5/hledger_args/options.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.4/hledger_args.egg-info/PKG-INFO` & `hledger_args-0.0.5/hledger_args.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hledger-args
-Version: 0.0.4
+Version: 0.0.5
 License: MIT License
 Project-URL: homepage, https://github.com/edkedk99/hledger-args
 Project-URL: documentation, https://edkedk99.github.io/hledger-args/
 Project-URL: repository, https://github.com/edkedk99/hledger-args
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -20,18 +20,21 @@
 
 Instead of giving the the desired command thru a command-line argument, choose it by selecting from a menu using the flag *--interactive*
 
 ### Special placeholders
 
 | Placeholders | Description                                                                    |
 |--------------|--------------------------------------------------------------------------------|
-| {account}    | fuzzy search existing accounts or new                                          |
-| {payee}      | fuzzy search existing payee or new                                             |
-| {tag}        | fuzzy search existing tags and values or new                                   |
+| {account}    | fuzzy search existing accounts                                                 |
+| {payee}      | fuzzy search existing payee                                                    |
+| {tag}        | fuzzy search existing tags and values                                          |
+| {tag_name}   | search tag name after "_" and fuzzy search existing values for this tag        |
 | {months}     | prompt initial and end dates both inclusive. **Diferent from default hledger** |
+| {type}       | select between accounts type                                                   |
+| {cur}        | fuzzy search existing commodities                                              |
 
 
 ## Installation
 
 ### Dependencies
 
 - python 3.8
```

### Comparing `hledger_args-0.0.4/hledger_args.egg-info/SOURCES.txt` & `hledger_args-0.0.5/hledger_args.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.4/pyproject.toml` & `hledger_args-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 keyword = ["hledger","PTA", "investments", "accounting"]
 classifiers = [""]
 author = "Eduardo"
 author_email = "edkedk99@hotmail.com"
 
 [project]
 name = "hledger_args"
-version = "0.0.4"
+version = "0.0.5"
 readme= "docs/README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 dependencies = [
 	     "click",
 	     "rich_click",
 	     "questionary"
```

### Comparing `hledger_args-0.0.4/venv/bin/rst2html.py` & `hledger_args-0.0.5/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.4/venv/bin/rst2html4.py` & `hledger_args-0.0.5/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.4/venv/bin/rst2html5.py` & `hledger_args-0.0.5/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.4/venv/bin/rst2latex.py` & `hledger_args-0.0.5/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.4/venv/bin/rst2man.py` & `hledger_args-0.0.5/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.4/venv/bin/rst2odt.py` & `hledger_args-0.0.5/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.4/venv/bin/rst2odt_prepstyles.py` & `hledger_args-0.0.5/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.4/venv/bin/rst2pseudoxml.py` & `hledger_args-0.0.5/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.4/venv/bin/rst2s5.py` & `hledger_args-0.0.5/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.4/venv/bin/rst2xetex.py` & `hledger_args-0.0.5/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.4/venv/bin/rst2xml.py` & `hledger_args-0.0.5/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.4/venv/bin/rstpep2html.py` & `hledger_args-0.0.5/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

