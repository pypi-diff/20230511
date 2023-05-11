# Comparing `tmp/robotcode_debugger-0.36.0.tar.gz` & `tmp/robotcode_debugger-0.37.0.tar.gz`

## Comparing `robotcode_debugger-0.36.0.tar` & `robotcode_debugger-0.37.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/src/robotcode/debugger/__init__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/src/robotcode/debugger/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/src/robotcode/debugger/__version__.py
--rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/src/robotcode/debugger/cli.py
--rw-r--r--   0        0        0    24396 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/src/robotcode/debugger/dap_types.py
--rw-r--r--   0        0        0    49582 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/src/robotcode/debugger/debugger.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/src/robotcode/debugger/hooks.py
--rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/src/robotcode/debugger/listeners.py
--rw-r--r--   0        0        0    12511 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/src/robotcode/debugger/protocol.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/src/robotcode/debugger/py.typed
--rw-r--r--   0        0        0     7618 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/src/robotcode/debugger/run.py
--rw-r--r--   0        0        0    15002 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/src/robotcode/debugger/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/src/robotcode/debugger/launcher/__init__.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/src/robotcode/debugger/launcher/cli.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/src/robotcode/debugger/launcher/client.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/src/robotcode/debugger/launcher/run.py
--rw-r--r--   0        0        0    13643 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/src/robotcode/debugger/launcher/server.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/LICENSE.txt
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/README.md
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/pyproject.toml
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 robotcode_debugger-0.36.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/src/robotcode/debugger/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/src/robotcode/debugger/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/src/robotcode/debugger/__version__.py
+-rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/src/robotcode/debugger/cli.py
+-rw-r--r--   0        0        0    24396 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/src/robotcode/debugger/dap_types.py
+-rw-r--r--   0        0        0    49582 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/src/robotcode/debugger/debugger.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/src/robotcode/debugger/hooks.py
+-rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/src/robotcode/debugger/listeners.py
+-rw-r--r--   0        0        0    12511 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/src/robotcode/debugger/protocol.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/src/robotcode/debugger/py.typed
+-rw-r--r--   0        0        0     7618 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/src/robotcode/debugger/run.py
+-rw-r--r--   0        0        0    15002 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/src/robotcode/debugger/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/src/robotcode/debugger/launcher/__init__.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/src/robotcode/debugger/launcher/cli.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/src/robotcode/debugger/launcher/client.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/src/robotcode/debugger/launcher/run.py
+-rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/src/robotcode/debugger/launcher/server.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/LICENSE.txt
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/README.md
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/pyproject.toml
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.0/PKG-INFO
```

### Comparing `robotcode_debugger-0.36.0/src/robotcode/debugger/cli.py` & `robotcode_debugger-0.37.0/src/robotcode/debugger/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.36.0/src/robotcode/debugger/dap_types.py` & `robotcode_debugger-0.37.0/src/robotcode/debugger/dap_types.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.36.0/src/robotcode/debugger/debugger.py` & `robotcode_debugger-0.37.0/src/robotcode/debugger/debugger.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.36.0/src/robotcode/debugger/listeners.py` & `robotcode_debugger-0.37.0/src/robotcode/debugger/listeners.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.36.0/src/robotcode/debugger/protocol.py` & `robotcode_debugger-0.37.0/src/robotcode/debugger/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.36.0/src/robotcode/debugger/run.py` & `robotcode_debugger-0.37.0/src/robotcode/debugger/run.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.36.0/src/robotcode/debugger/server.py` & `robotcode_debugger-0.37.0/src/robotcode/debugger/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.36.0/src/robotcode/debugger/launcher/cli.py` & `robotcode_debugger-0.37.0/src/robotcode/debugger/launcher/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.36.0/src/robotcode/debugger/launcher/client.py` & `robotcode_debugger-0.37.0/src/robotcode/debugger/launcher/client.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.36.0/src/robotcode/debugger/launcher/run.py` & `robotcode_debugger-0.37.0/src/robotcode/debugger/launcher/run.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.36.0/src/robotcode/debugger/launcher/server.py` & `robotcode_debugger-0.37.0/src/robotcode/debugger/launcher/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,72 +161,73 @@
         outputTimestamps: Optional[bool] = False,  # noqa: N803
         groupOutput: Optional[bool] = False,  # noqa: N803
         stopOnEntry: Optional[bool] = False,  # noqa: N803
         dryRun: Optional[bool] = None,  # noqa: N803
         mode: Optional[str] = None,
         variableFiles: Optional[List[str]] = None,  # noqa: N803
         languages: Optional[List[str]] = None,
-        arguments: Optional[LaunchRequestArguments] = None,
         include: Optional[List[str]] = None,
         exclude: Optional[List[str]] = None,
         robotCodeArgs: Optional[List[str]] = None,  # noqa: N803
+        arguments: Optional[LaunchRequestArguments] = None,
         *_args: Any,
         **_kwargs: Any,
     ) -> None:
         from robotcode.core.utils.net import find_free_port
 
         connect_timeout = launcherTimeout or 10
 
         port = find_free_port(DEBUGGER_DEFAULT_PORT)
 
         debugger_script = (
             Path(Path(__file__).parent.parent) if self.debugger_script is None else Path(self.debugger_script)
         )
 
-        run_args = [
+        robotcode_run_args = [
             python,
             str(debugger_script),
             *itertools.chain.from_iterable(["--profile", p] for p in profiles or []),
+            *itertools.chain.from_iterable(["--default-path", p] for p in paths or []),
             *(robotCodeArgs or []),
             "debug",
         ]
 
         if no_debug:
-            run_args += ["--no-debug"]
+            robotcode_run_args += ["--no-debug"]
 
         if port != DEBUGGER_DEFAULT_PORT:
-            run_args += ["--tcp", str(port)]
+            robotcode_run_args += ["--tcp", str(port)]
 
         if debuggerTimeout is not None:
-            run_args += ["wait-for-client-timeout", str(debuggerTimeout)]
+            robotcode_run_args += ["wait-for-client-timeout", str(debuggerTimeout)]
 
         if attachPython and not no_debug:
-            run_args += ["--debugpy"]
+            robotcode_run_args += ["--debugpy"]
 
             if attachPythonPort is not None and attachPythonPort != DEBUGPY_DEFAULT_PORT:
-                run_args += ["--debugpy-port", str(attachPythonPort or 0)]
+                robotcode_run_args += ["--debugpy-port", str(attachPythonPort or 0)]
 
         if outputMessages:
-            run_args += ["--output-messages"]
+            robotcode_run_args += ["--output-messages"]
 
         if not outputLog:
-            run_args += ["--no-output-log"]
+            robotcode_run_args += ["--no-output-log"]
 
         if outputTimestamps:
-            run_args += ["--output-timestamps"]
+            robotcode_run_args += ["--output-timestamps"]
 
         if groupOutput:
-            run_args += ["--group-output"]
+            robotcode_run_args += ["--group-output"]
 
         if stopOnEntry:
-            run_args += ["--stop-on-entry"]
+            robotcode_run_args += ["--stop-on-entry"]
 
-        run_args += debuggerArgs or []
+        robotcode_run_args += debuggerArgs or []
 
-        run_args += ["--"]
+        run_args = []
 
         if get_robot_version() >= (6, 0) and languages:
             for lang in languages:
                 run_args += ["--language", lang]
 
         if mode:
             if mode == "rpa":
@@ -258,32 +259,28 @@
 
         if exclude:
             for v in exclude:
                 run_args += ["-e", f"{v}"]
 
         run_args += args or []
 
-        if paths:
-            for p in paths:
-                run_args.append(p)
-
         if target:
             run_args.append(target)
 
-        if target is not None and not paths and not target:
-            run_args.append(".")
+        if run_args:
+            run_args.insert(0, "--")
 
         env = {k: ("" if v is None else str(v)) for k, v in env.items()} if env else {}
 
         if console in ["integratedTerminal", "externalTerminal"]:
             await self.send_request_async(
                 RunInTerminalRequest(
                     arguments=RunInTerminalRequestArguments(
                         cwd=cwd,
-                        args=run_args,
+                        args=[*robotcode_run_args, *run_args],
                         env=env,
                         kind=RunInTerminalKind.INTEGRATED
                         if console == "integratedTerminal"
                         else RunInTerminalKind.EXTERNAL
                         if console == "externalTerminal"
                         else None,
                         title=name,
```

### Comparing `robotcode_debugger-0.36.0/.gitignore` & `robotcode_debugger-0.37.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.36.0/LICENSE.txt` & `robotcode_debugger-0.37.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.36.0/README.md` & `robotcode_debugger-0.37.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.36.0/pyproject.toml` & `robotcode_debugger-0.37.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,16 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.36.0",
-  "robotcode-runner==0.36.0",
+  "robotcode-jsonrpc2==0.37.0",
+  "robotcode-runner==0.37.0",
 ]
 
 [project.optional-dependencies]
 debugpy = ["debugpy"]
 
 [project.entry-points.robotcode]
 debugger = "robotcode.debugger.hooks"
```

### Comparing `robotcode_debugger-0.36.0/PKG-INFO` & `robotcode_debugger-0.37.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-debugger
-Version: 0.36.0
+Version: 0.37.0
 Summary: RobotCode Debugger for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.36.0
-Requires-Dist: robotcode-runner==0.36.0
+Requires-Dist: robotcode-jsonrpc2==0.37.0
+Requires-Dist: robotcode-runner==0.37.0
 Requires-Dist: robotframework>=4.1.0
 Provides-Extra: debugpy
 Requires-Dist: debugpy; extra == 'debugpy'
 Description-Content-Type: text/markdown
 
 # robotcode-debugger
```

