# Comparing `tmp/trill-0.0.8.tar.gz` & `tmp/trill-0.0.9.tar.gz`

## Comparing `trill-0.0.8.tar` & `trill-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 trill-0.0.8/.env
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 trill-0.0.8/Makefile
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 trill-0.0.8/_version.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 trill-0.0.8/requirements-dev.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 trill-0.0.8/rolls.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 trill-0.0.8/setup.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 trill-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 trill-0.0.8/.github/workflows/test.yml
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 trill-0.0.8/.vscode/settings.json
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 trill-0.0.8/examples/rolls.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/__init__.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/error.py
--rw-r--r--   0        0        0    19199 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/interpreter.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/main.py
--rw-r--r--   0        0        0    19895 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/parser.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/reserved.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/string.py
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tokenizer.py
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tokens.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/ast/__init__.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/ast/base.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/ast/expression.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/ast/printer.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/ast/statement.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tests/__init__.py
--rw-r--r--   0        0        0    10634 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tests/cases.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tests/test_errors.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tests/test_interpreter.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tests/test_parser.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tests/test_string.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tests/test_syntax_tree.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 trill-0.0.8/src/trill/tests/test_tokenizer.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 trill-0.0.8/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 trill-0.0.8/LICENSE
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 trill-0.0.8/README.md
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 trill-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 trill-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 trill-0.0.9/.env
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 trill-0.0.9/Makefile
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 trill-0.0.9/_version.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 trill-0.0.9/requirements-dev.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 trill-0.0.9/rolls.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 trill-0.0.9/setup.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 trill-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 trill-0.0.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 trill-0.0.9/.vscode/settings.json
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 trill-0.0.9/examples/rolls.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/__init__.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/error.py
+-rw-r--r--   0        0        0    19199 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/interpreter.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/main.py
+-rw-r--r--   0        0        0    19895 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/parser.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/reserved.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/string.py
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/tokenizer.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/tokens.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/ast/__init__.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/ast/base.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/ast/expression.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/ast/printer.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/ast/statement.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/tests/__init__.py
+-rw-r--r--   0        0        0    10634 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/tests/cases.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/tests/test_errors.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/tests/test_interpreter.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/tests/test_parser.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/tests/test_string.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/tests/test_syntax_tree.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 trill-0.0.9/src/trill/tests/test_tokenizer.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 trill-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 trill-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 trill-0.0.9/README.md
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 trill-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 trill-0.0.9/PKG-INFO
```

### Comparing `trill-0.0.8/Makefile` & `trill-0.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/.github/workflows/publish.yml` & `trill-0.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/.github/workflows/test.yml` & `trill-0.0.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/examples/rolls.py` & `trill-0.0.9/examples/rolls.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/__init__.py` & `trill-0.0.9/src/trill/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 from typing import Optional
 from .tokenizer import Tokenizer
 from .parser import Parser
 from .interpreter import Interpreter
 from .error import handler as error_handler
 
 
-def trill(roll: str, seed: Optional[int] = None):
+def trill(roll: str, seed: Optional[int] = None,
+          average: bool = False):
     tokens = Tokenizer(roll).scan_tokens()
 
     if error_handler.had_error:
         return [None, error_handler.error_report]
 
     parsed = Parser(tokens).parse()
 
     if error_handler.had_error:
         return [None, error_handler.error_report]
 
-    result = Interpreter(seed).interpret(parsed)
+    result = Interpreter(seed).interpret(parsed, average=average)
 
     return [result, error_handler.error_report]
```

### Comparing `trill-0.0.8/src/trill/error.py` & `trill-0.0.9/src/trill/error.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/interpreter.py` & `trill-0.0.9/src/trill/interpreter.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/main.py` & `trill-0.0.9/src/trill/main.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/parser.py` & `trill-0.0.9/src/trill/parser.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/reserved.py` & `trill-0.0.9/src/trill/reserved.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/string.py` & `trill-0.0.9/src/trill/string.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/tokenizer.py` & `trill-0.0.9/src/trill/tokenizer.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/tokens.py` & `trill-0.0.9/src/trill/tokens.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/ast/base.py` & `trill-0.0.9/src/trill/ast/base.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/ast/expression.py` & `trill-0.0.9/src/trill/ast/expression.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/ast/printer.py` & `trill-0.0.9/src/trill/ast/printer.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/ast/statement.py` & `trill-0.0.9/src/trill/ast/statement.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/tests/cases.py` & `trill-0.0.9/src/trill/tests/cases.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/tests/test_errors.py` & `trill-0.0.9/src/trill/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/tests/test_interpreter.py` & `trill-0.0.9/src/trill/tests/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/tests/test_parser.py` & `trill-0.0.9/src/trill/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/tests/test_syntax_tree.py` & `trill-0.0.9/src/trill/tests/test_syntax_tree.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/src/trill/tests/test_tokenizer.py` & `trill-0.0.9/src/trill/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/LICENSE` & `trill-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/README.md` & `trill-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/pyproject.toml` & `trill-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trill-0.0.8/PKG-INFO` & `trill-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trill
-Version: 0.0.8
+Version: 0.0.9
 Summary: Troll language parser and interpreter.
 Project-URL: Homepage, https://github.com/gregersn/Trill
 Author-email: Greger Stolt Nilsen <gregersn@gmail.com>
 License: Copyright © 2022-2023 Greger Stolt Nilsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

