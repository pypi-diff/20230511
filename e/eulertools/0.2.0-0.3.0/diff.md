# Comparing `tmp/eulertools-0.2.0.tar.gz` & `tmp/eulertools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulertools-0.2.0.tar", max compression
+gzip compressed data, was "eulertools-0.3.0.tar", max compression
```

## Comparing `eulertools-0.2.0.tar` & `eulertools-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     7652 2023-05-09 19:41:34.782813 eulertools-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      976 2023-05-09 19:41:34.788663 eulertools-0.2.0/README.rst
--rw-r--r--   0        0        0     2694 2023-05-09 20:14:22.716835 eulertools-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-09 19:41:34.789309 eulertools-0.2.0/src/eulertools/__init__.py
--rw-r--r--   0        0        0       22 2023-05-09 20:14:22.713108 eulertools-0.2.0/src/eulertools/__version__.py
--rw-r--r--   0        0        0      793 2023-05-09 19:41:34.789676 eulertools-0.2.0/src/eulertools/benchmark.py
--rw-r--r--   0        0        0     1711 2023-05-09 19:41:34.789870 eulertools-0.2.0/src/eulertools/compare.py
--rw-r--r--   0        0        0     1254 2023-05-09 19:41:34.790077 eulertools-0.2.0/src/eulertools/generate.py
--rw-r--r--   0        0        0     4228 2023-05-09 19:41:34.790221 eulertools-0.2.0/src/eulertools/main.py
--rw-r--r--   0        0        0     2722 2023-05-09 19:41:34.790377 eulertools-0.2.0/src/eulertools/run.py
--rw-r--r--   0        0        0      915 2023-05-09 19:41:34.790517 eulertools-0.2.0/src/eulertools/statement.py
--rw-r--r--   0        0        0     1042 2023-05-09 19:41:34.790650 eulertools-0.2.0/src/eulertools/test.py
--rw-r--r--   0        0        0     1957 2023-05-09 19:41:34.790786 eulertools-0.2.0/src/eulertools/timeit.py
--rw-r--r--   0        0        0      946 2023-05-09 19:41:34.790928 eulertools-0.2.0/src/eulertools/update.py
--rw-r--r--   0        0        0     5613 2023-05-09 20:02:38.633861 eulertools-0.2.0/src/eulertools/utils.py
--rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 eulertools-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-05-09 19:41:34.782813 eulertools-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0      976 2023-05-09 19:41:34.788663 eulertools-0.3.0/README.rst
+-rw-r--r--   0        0        0     2694 2023-05-11 15:59:49.025802 eulertools-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 19:41:34.789309 eulertools-0.3.0/src/eulertools/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-11 15:59:49.013459 eulertools-0.3.0/src/eulertools/__version__.py
+-rw-r--r--   0        0        0      793 2023-05-09 19:41:34.789676 eulertools-0.3.0/src/eulertools/benchmark.py
+-rw-r--r--   0        0        0     1724 2023-05-11 15:59:14.099647 eulertools-0.3.0/src/eulertools/compare.py
+-rw-r--r--   0        0        0     1209 2023-05-11 15:59:14.375119 eulertools-0.3.0/src/eulertools/generate.py
+-rw-r--r--   0        0        0     4255 2023-05-11 15:59:14.375397 eulertools-0.3.0/src/eulertools/main.py
+-rw-r--r--   0        0        0     2799 2023-05-11 15:59:14.375661 eulertools-0.3.0/src/eulertools/run.py
+-rw-r--r--   0        0        0      915 2023-05-09 19:41:34.790517 eulertools-0.3.0/src/eulertools/statement.py
+-rw-r--r--   0        0        0     1042 2023-05-11 15:05:17.461116 eulertools-0.3.0/src/eulertools/test.py
+-rw-r--r--   0        0        0     1943 2023-05-11 15:05:17.464023 eulertools-0.3.0/src/eulertools/timeit.py
+-rw-r--r--   0        0        0      946 2023-05-11 15:05:17.460986 eulertools-0.3.0/src/eulertools/update.py
+-rw-r--r--   0        0        0     5654 2023-05-11 15:59:14.099956 eulertools-0.3.0/src/eulertools/utils.py
+-rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 eulertools-0.3.0/PKG-INFO
```

### Comparing `eulertools-0.2.0/LICENSE.txt` & `eulertools-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eulertools-0.2.0/README.rst` & `eulertools-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `eulertools-0.2.0/pyproject.toml` & `eulertools-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "eulertools"
-version = "0.2.0"
+version = "0.3.0"
 description = "Multilanguage competitive coding toolbox"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "README.rst"
```

### Comparing `eulertools-0.2.0/src/eulertools/benchmark.py` & `eulertools-0.3.0/src/eulertools/benchmark.py`

 * *Files identical despite different names*

### Comparing `eulertools-0.2.0/src/eulertools/compare.py` & `eulertools-0.3.0/src/eulertools/compare.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,13 +37,13 @@
         return [
             language.name,
             *(str(timings.get(problem, "N/A")) for problem in self.problems),
         ]
 
     @staticmethod
     def transpose(matrix: list[list[str]]) -> list[list[str]]:
-        return [list(row) for row in zip(*matrix)]
+        return [list(row) for row in zip(*matrix, strict=True)]
 
     def padded_print(self, string: str, *, heading: bool) -> str:
         if heading:
             return string.center(self.pad_length)
         return string.rjust(self.pad_length)
```

### Comparing `eulertools-0.2.0/src/eulertools/generate.py` & `eulertools-0.3.0/src/eulertools/generate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from pathlib import Path
 
 import jinja2
 
-from eulertools.utils import Language, get_statement, get_solution, get_template
+from eulertools.utils import Language, get_solution, get_statement, get_template
 
 
 class Generate:
     def __init__(self, language: Language, problem: str, *, force: bool = False):
         self.language = language
         self.problem = problem
         self.force = force
 
     def run(self) -> None:
-        extension = self.language.extension
-
         solution = get_solution(self.language, self.problem)
         if solution.exists() and not self.force:
             raise FileExistsError("Solution already exists. Aborting...")
         template = get_template(self.language)
 
         statement = get_statement(self.problem)
         if not statement.exists():
```

### Comparing `eulertools-0.2.0/src/eulertools/main.py` & `eulertools-0.3.0/src/eulertools/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
     generate_parser = subparsers.add_parser("generate")
     language_specific(generate_parser)
     generate_parser.add_argument("-f", "--force", action="store_true")
 
     run_parser = subparsers.add_parser("run")
     language_specific(run_parser)
+    run_parser.add_argument("-d", "--debug", action="store_true")
 
     update_parser = subparsers.add_parser("update")
     language_specific(update_parser)
     update_parser.add_argument("timing")
 
     timeit_parser = subparsers.add_parser("timeit")
     language_specific(timeit_parser)
@@ -81,15 +82,15 @@
         case "generate":
             language = LANGUAGES[options.language]
             problem = get_problem(options.problem)
             Generate(language, problem, force=options.force).run()
         case "run":
             language = LANGUAGES[options.language]
             problem = get_problem(options.problem)
-            Run(language, problem).run()
+            Run(language, problem, debug=options.debug).run()
         case "update":
             language = LANGUAGES[options.language]
             problem = get_problem(options.problem)
             Update(language, problem, options.timing).run()
         case "timeit":
             language = LANGUAGES[options.language]
             problem = get_problem(options.problem)
@@ -98,22 +99,18 @@
                 problem,
                 options.times,
                 run_update=options.update,
                 quiet=options.quiet,
                 print_report=options.report,
             ).run()
         case "benchmark":
-            languages = [
-                LANGUAGES[language] for language in sorted(options.languages)
-            ]
+            languages = [LANGUAGES[language] for language in sorted(options.languages)]
             Benchmark(languages, options.times).run()
         case "compare":
-            languages = [
-                LANGUAGES[language] for language in sorted(options.languages)
-            ]
+            languages = [LANGUAGES[language] for language in sorted(options.languages)]
             problems = sorted(get_problem(problem) for problem in options.problems)
             Compare(languages, problems).run()
         case "test":
             language = LANGUAGES[options.language]
             problems = sorted(get_problem(problem) for problem in options.problems)
             Test(language, problems).run()
         case "statement":
```

### Comparing `eulertools-0.2.0/src/eulertools/run.py` & `eulertools-0.3.0/src/eulertools/run.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 import subprocess
+import sys
 
 from eulertools.utils import Language, Modes, get_answers_dict, get_solution
 
 
 class Run:
     def __init__(
-        self, language: Language, problem: str, *, times: int = 1, mode: str = Modes.RUN
+        self,
+        language: Language,
+        problem: str,
+        *,
+        debug: bool = False,
+        times: int = 1,
+        mode: str = Modes.RUN,
     ):
         self.language = language
         self.problem = problem
         self.mode = mode
         self.times = times
+        self.debug = debug
 
     def run(self) -> list[int]:
         if self.mode == Modes.TIMING and self.times < 3:
             raise ValueError("Timing mode requires at least 3 runs. Aborting...")
 
         if self.mode != Modes.TIMING and self.times != 1:
             raise ValueError("Only timing mode supports multiple runs. Aborting...")
@@ -30,40 +38,42 @@
                 self.problem,
                 self.mode,
                 str(self.times),
             ],
             capture_output=True,
         )
         output = raw_output.stdout.decode()
+        if self.debug:
+            sys.tracebacklimit = 9999
+            print(output)
         timings = [
             int(line[6:]) or 1
             for line in output.splitlines()
             if line.startswith("Time: ")
         ]
         expected_answers = get_answers_dict(self.problem)
         actual_answers: dict[int, str] = {}
         prefix = "Testing" if self.mode == "test" else "Running"
         for line in output.strip().splitlines():
             if line.startswith("Time: "):
                 continue
             raw_key, value = line.split(maxsplit=1)
             key = int(raw_key[:-1])
             actual_answers[key] = value
+        success = True
         if self.mode == "test" and len(actual_answers) != len(expected_answers):
+            success = False
             print(f"🔴 {prefix} {self.problem}...")
-            raise ValueError(
-                f"Expected {len(expected_answers)} answers, got {len(actual_answers)}"
-            )
         for key, value in actual_answers.items():
-            if self.mode == "run" and key != 1 and value == expected_answers[key]:
-                continue
             if key not in expected_answers:
                 if self.mode != "timing":
                     print(f"🟠 {prefix} {self.problem}/{key}... new response: {value}")
             elif value != expected_answers[key]:
+                success = False
                 print(
                     f"🔴 {prefix} {self.problem}/{key}... expected: {expected_answers[key]}, got: {value}"
                 )
-                raise ValueError("Test failed")
             elif self.mode != "timing":
                 print(f"🟢 {prefix} {self.problem}/{key}... {value}")
+        if not success:
+            raise ValueError(f"{prefix} failed. Aborting...")
         return timings
```

### Comparing `eulertools-0.2.0/src/eulertools/statement.py` & `eulertools-0.3.0/src/eulertools/statement.py`

 * *Files identical despite different names*

### Comparing `eulertools-0.2.0/src/eulertools/test.py` & `eulertools-0.3.0/src/eulertools/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from math import ceil, floor
 
 from eulertools.run import Run
-from eulertools.utils import ANSIEscape, Modes, Language, get_timings
+from eulertools.utils import ANSIEscape, Language, Modes, get_timings
 
 
 class Test:
     def __init__(self, language: Language, problems: list[str]):
         self.language = language
         self.problems = self.discover_problems(problems)
```

### Comparing `eulertools-0.2.0/src/eulertools/timeit.py` & `eulertools-0.3.0/src/eulertools/timeit.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,16 @@
     def run(self) -> None:
         solution = get_solution(self.language, self.problem)
         if not solution.exists():
             raise FileNotFoundError(
                 f"Problem {self.problem} not solved for {self.language}. Aborting..."
             )
         timings = get_timings(self.language)
-        if old_timing := timings.get(self.problem):
-            if not self.run_update:
-                print(f"Old timing: {old_timing}")
+        if (old_timing := timings.get(self.problem)) and not self.run_update:
+            print(f"Old timing: {old_timing}")
         returned_lines = Run(
             self.language, self.problem, mode="timing", times=self.times
         ).run()
         if not returned_lines:
             raise ValueError("No lines returned from Run.")
         average = Timing.from_nanoseconds(get_average(returned_lines))
         if not self.quiet:
```

### Comparing `eulertools-0.2.0/src/eulertools/update.py` & `eulertools-0.3.0/src/eulertools/update.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from eulertools.utils import Timing, Language, get_solution, get_timings, update_timings
+from eulertools.utils import Language, Timing, get_solution, get_timings, update_timings
 
 
 class Update:
     def __init__(self, language: Language, problem: str, timing: str):
         self.language = language
         self.problem = problem
         self.timing = timing
```

### Comparing `eulertools-0.2.0/src/eulertools/utils.py` & `eulertools-0.3.0/src/eulertools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,16 @@
     if len(values) >= 3:
         values = sorted(values)[1:-1]
     return sum(values) // len(values)
 
 
 def get_problem(problem: str) -> str:
     settings = get_settings()
-    return settings["problems"]["format"].format(problem=problem)
+    problem_format: str = settings["problems"]["format"]
+    return problem_format.format(problem=problem)
 
 
 def get_statement(problem: str) -> Path:
     return get_project_root().joinpath("statements", f"{problem}.txt")
 
 
 def get_template(language: Language) -> Path:
```

### Comparing `eulertools-0.2.0/PKG-INFO` & `eulertools-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eulertools
-Version: 0.2.0
+Version: 0.3.0
 Summary: Multilanguage competitive coding toolbox
 Home-page: https://eulertools.readthedocs.io/en/latest/
 License: LGPL-3.0+
 Keywords: leetcode,topcoder,project_euler
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
 Requires-Python: >=3.11,<4.0
```

