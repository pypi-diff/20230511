# Comparing `tmp/pywry-0.5.4.tar.gz` & `tmp/pywry-0.5.5.tar.gz`

## Comparing `pywry-0.5.4.tar` & `pywry-0.5.5.tar`

### file list

```diff
@@ -1,22 +1,30 @@
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 pywry-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 pywry-0.5.4/rust_src/pywry/Cargo.toml
--rw-r--r--   0     1001      123     1063 2023-05-08 16:17:17.000000 pywry-0.5.4/rust_src/pywry/LICENSE
--rw-r--r--   0     1001      123     4870 2023-05-08 16:17:17.000000 pywry-0.5.4/rust_src/pywry/README.md
--rw-r--r--   0     1001      123     2149 2023-05-08 16:17:17.000000 pywry-0.5.4/rust_src/pywry/src/constants.rs
--rw-r--r--   0     1001      123     1223 2023-05-08 16:17:17.000000 pywry-0.5.4/rust_src/pywry/src/lib.rs
--rw-r--r--   0     1001      123     1085 2023-05-08 16:17:17.000000 pywry-0.5.4/rust_src/pywry/src/pipe.rs
--rw-r--r--   0     1001      123     4737 2023-05-08 16:17:17.000000 pywry-0.5.4/rust_src/pywry/src/structs.rs
--rw-r--r--   0     1001      123    22038 2023-05-08 16:17:17.000000 pywry-0.5.4/rust_src/pywry/src/window.rs
--rw-r--r--   0     1001      123    60354 2023-05-08 16:17:17.000000 pywry-0.5.4/Cargo.lock
--rw-r--r--   0     1001      123      985 2023-05-08 16:17:17.000000 pywry-0.5.4/python/pywry/backend.py
--rw-r--r--   0     1001      123        0 2023-05-08 16:17:17.000000 pywry-0.5.4/python/pywry/py.typed
--rw-r--r--   0     1001      123      154 2023-05-08 16:17:17.000000 pywry-0.5.4/python/pywry/pywry.pyi
--rw-r--r--   0     1001      123    13031 2023-05-08 16:17:17.000000 pywry-0.5.4/python/pywry/core.py
--rw-r--r--   0     1001      123      180 2023-05-08 16:17:17.000000 pywry-0.5.4/python/pywry/__init__.py
--rw-r--r--   0     1001      123      733 2023-05-08 16:17:17.000000 pywry-0.5.4/Cargo.toml
--rw-r--r--   0     1001      123     2149 2023-05-08 16:17:17.000000 pywry-0.5.4/src/constants.rs
--rw-r--r--   0     1001      123     1223 2023-05-08 16:17:17.000000 pywry-0.5.4/src/lib.rs
--rw-r--r--   0     1001      123     1085 2023-05-08 16:17:17.000000 pywry-0.5.4/src/pipe.rs
--rw-r--r--   0     1001      123     4737 2023-05-08 16:17:17.000000 pywry-0.5.4/src/structs.rs
--rw-r--r--   0     1001      123    22038 2023-05-08 16:17:17.000000 pywry-0.5.4/src/window.rs
--rw-r--r--   0        0        0     5472 1970-01-01 00:00:00.000000 pywry-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 pywry-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 pywry-0.5.5/rust_src/pywry/Cargo.toml
+-rw-r--r--   0     1001      123     1063 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/LICENSE
+-rw-r--r--   0     1001      123     4997 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/README.md
+-rw-r--r--   0     1001      123     3954 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/constants.rs
+-rw-r--r--   0     1001      123     8710 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/events.rs
+-rw-r--r--   0     1001      123     5570 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/handlers.rs
+-rw-r--r--   0     1001      123     7311 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/headless.rs
+-rw-r--r--   0     1001      123     1762 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/lib.rs
+-rw-r--r--   0     1001      123     1086 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/pipe.rs
+-rw-r--r--   0     1001      123     9060 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/structs.rs
+-rw-r--r--   0     1001      123     1663 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/utils.rs
+-rw-r--r--   0     1001      123     7965 2023-05-11 09:41:22.000000 pywry-0.5.5/rust_src/pywry/src/window.rs
+-rw-r--r--   0     1001      123    60354 2023-05-11 09:41:22.000000 pywry-0.5.5/Cargo.lock
+-rw-r--r--   0     1001      123     1155 2023-05-11 09:41:22.000000 pywry-0.5.5/python/pywry/backend.py
+-rw-r--r--   0     1001      123        0 2023-05-11 09:41:22.000000 pywry-0.5.5/python/pywry/py.typed
+-rw-r--r--   0     1001      123      180 2023-05-11 09:41:22.000000 pywry-0.5.5/python/pywry/__init__.py
+-rw-r--r--   0     1001      123    14558 2023-05-11 09:41:22.000000 pywry-0.5.5/python/pywry/core.py
+-rw-r--r--   0     1001      123      217 2023-05-11 09:41:22.000000 pywry-0.5.5/python/pywry/pywry.pyi
+-rw-r--r--   0     1001      123      733 2023-05-11 09:41:22.000000 pywry-0.5.5/Cargo.toml
+-rw-r--r--   0     1001      123     3954 2023-05-11 09:41:22.000000 pywry-0.5.5/src/constants.rs
+-rw-r--r--   0     1001      123     8710 2023-05-11 09:41:22.000000 pywry-0.5.5/src/events.rs
+-rw-r--r--   0     1001      123     5570 2023-05-11 09:41:22.000000 pywry-0.5.5/src/handlers.rs
+-rw-r--r--   0     1001      123     7311 2023-05-11 09:41:22.000000 pywry-0.5.5/src/headless.rs
+-rw-r--r--   0     1001      123     1762 2023-05-11 09:41:22.000000 pywry-0.5.5/src/lib.rs
+-rw-r--r--   0     1001      123     1086 2023-05-11 09:41:22.000000 pywry-0.5.5/src/pipe.rs
+-rw-r--r--   0     1001      123     9060 2023-05-11 09:41:22.000000 pywry-0.5.5/src/structs.rs
+-rw-r--r--   0     1001      123     1663 2023-05-11 09:41:22.000000 pywry-0.5.5/src/utils.rs
+-rw-r--r--   0     1001      123     7965 2023-05-11 09:41:22.000000 pywry-0.5.5/src/window.rs
+-rw-r--r--   0        0        0     5599 1970-01-01 00:00:00.000000 pywry-0.5.5/PKG-INFO
```

### Comparing `pywry-0.5.4/pyproject.toml` & `pywry-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pywry"
-version = "0.5.4"
+version = "0.5.5"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: POSIX",
     "Operating System :: Microsoft :: Windows",
```

### Comparing `pywry-0.5.4/rust_src/pywry/Cargo.toml` & `pywry-0.5.5/rust_src/pywry/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.5.4"
+version = "0.5.5"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
```

### Comparing `pywry-0.5.4/rust_src/pywry/LICENSE` & `pywry-0.5.5/rust_src/pywry/LICENSE`

 * *Files identical despite different names*

### Comparing `pywry-0.5.4/rust_src/pywry/README.md` & `pywry-0.5.5/rust_src/pywry/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # PyWry Web Viewer
 
+![signal-2023-05-08-171646_002](https://github.com/OpenBB-finance/pywry/assets/25267873/a19338f7-0149-4ada-8fc7-389ae36c39fc)
+
 Easily create HTML webviewers in python utilizing the [wry](https://github.com/tauri-apps/wry) library. Unlike many HTML viewers that exist for Python - Pywry allows you to run javacsript. PyWry is also a ~2mb footprint for Mac and Windows - Linux will require a few more libraries which are listed below.
 
 Please note: this library is currently in early alpha and is NOT ready for production use.
 
 ## Installation
 
 ---------------------
```

### Comparing `pywry-0.5.4/rust_src/pywry/src/pipe.rs` & `pywry-0.5.5/rust_src/pywry/src/pipe.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use std::sync::mpsc::Sender;
 use tokio::io::{self, AsyncBufReadExt};
 
 pub async fn send_message(sender: Sender<String>, message: String) {
     let trimmed_line = message.trim();
     if !trimmed_line.is_empty() && trimmed_line.starts_with('{') && trimmed_line.ends_with('}') {
-        let _ = sender.send(message);
+        sender.send(message).unwrap();
     }
 }
 
 pub async fn run_listener(sender: Sender<String>) -> Result<(), Box<dyn std::error::Error>> {
     let stdin = io::stdin();
     let mut reader = io::BufReader::new(stdin);
     let rt = tokio::runtime::Runtime::new()?;
```

### Comparing `pywry-0.5.4/Cargo.lock` & `pywry-0.5.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1481,15 +1481,15 @@
 checksum = "a915bd72824962bf190bbd3e8a044cccb695d1409f73ff5493712eda5136c7a8"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pywry"
-version = "0.5.4"
+version = "0.5.5"
 dependencies = [
  "image",
  "mime_guess",
  "open",
  "pyo3",
  "serde",
  "serde_json",
```

### Comparing `pywry-0.5.4/python/pywry/backend.py` & `pywry-0.5.5/python/pywry/backend.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,32 +4,37 @@
 import setproctitle
 
 from pywry import PyWry
 
 __all__ = ["start_backend"]
 
 
-def start_backend(debug: bool = False):
+def start_backend(headless: bool = False, debug: bool = False) -> None:
     """Start the backend."""
     try:
         proc_title = os.environ.get("PYWRY_PROCESS_NAME", "PyWry").replace(" ", "")
         setproctitle.setproctitle(proc_title)
         import ctypes  # pylint: disable=import-outside-toplevel
 
         # We need to set an app id so that the taskbar icon is correct on Windows
         ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID("openbb")
     except (AttributeError, ImportError, OSError):
         pass
+
     backend = PyWry()
+    if headless:
+        return backend.base.start_headless(debug)
+
     backend.base.start(debug)
 
 
 if __name__ == "__main__":
     sys_args = sys.argv[1:]
     sys_args = [arg.lower() for arg in sys_args]
 
     if "--start" in sys_args or sys.platform == "darwin":
+        headless = "--headless" in sys_args
         debug = (
             "--debug" in sys_args
             or os.environ.get("DEBUG_MODE", "False").lower() == "true"
         )  # noqa
-        start_backend(debug)
+        start_backend(headless=headless, debug=debug)
```

### Comparing `pywry-0.5.4/python/pywry/core.py` & `pywry-0.5.5/python/pywry/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import re
 import subprocess
 import sys
 import threading
 import traceback
 from asyncio.exceptions import CancelledError, IncompleteReadError, TimeoutError
 from pathlib import Path
+from queue import Queue
 from typing import List, Optional, Union
 
 import setproctitle
 
 from pywry import pywry
 
 __all__ = ["PyWry", "BackendFailedToStart"]
@@ -46,14 +47,15 @@
 
 
 class PyWry:
     """This class handles the wry functionality, by spinning up a rust program that
     listens to pipes and shows windows with provided html and json data.
     """
 
+    _bootargs: List[str] = []
     __version__ = pywry.__version__
 
     def __new__(cls, *args, **kwargs):  # pylint: disable=unused-argument
         "Makes the class a 'singleton' by only allowing one instance at a time"
         if not hasattr(cls, "instance"):
             cls.instance = super().__new__(cls)
         return cls.instance
@@ -64,14 +66,15 @@
         max_retries: int = 30,
         proc_name: str = "PyWry",
     ):
         self.max_retries: int = max_retries
         self.proc_name: str = proc_name
 
         self.outgoing: List[str] = []
+        self.recv: Queue[dict] = Queue()
         self.init_engine: List[str] = []
         self.daemon: bool = daemon
         self.debug: bool = False
         self.shell: bool = False
         self.base = pywry.WindowManager()
 
         try:
@@ -226,36 +229,35 @@
                     self._is_closed.set()
 
             kwargs = dict(
                 stdin=subprocess.PIPE,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
             )
-            cmd = [sys.executable, "-m", "pywry.backend", "--start"]
-            if self.debug:
-                cmd.append("--debug")
+            cmd = [sys.executable, "-m", "pywry.backend", "--start"] + self._bootargs
 
             # for pyinstaller builds
             if hasattr(sys, "frozen"):
                 # pylint: disable=E1101,W0212
                 exec_name = os.environ.get("PYWRY_EXECUTABLE", "PyWry")
                 pywrypath = (Path(sys._MEIPASS) / exec_name).resolve()
-                cmd = f"{exec_name} --start{' --debug' if self.debug else ''}"
+                cmd = f"{exec_name} --start{' '.join(self._bootargs)}"
                 if sys.platform == "darwin":
                     cmd = f"'{pywrypath}'"
 
                 kwargs.update(dict(cwd=str(pywrypath.parent)))
                 self.shell = True
 
             env = os.environ.copy()
             env["PYWRY_PROCESS_NAME"] = self.proc_name
 
             runner = asyncio.create_subprocess_exec(
                 *cmd,
                 env=env,
+                limit=2**64,
                 **kwargs,
             )
 
             if self.shell:
                 if isinstance(cmd, list):
                     cmd = " ".join(cmd)
                 runner = asyncio.create_subprocess_shell(
@@ -276,22 +278,46 @@
             # Unix machines may need a little more time to start the backend
             if sys.platform != "win32":
                 await asyncio.sleep(3)
 
         except Exception as proc_err:
             raise BackendFailedToStart("Could not start backend") from proc_err
 
+    def print_message(self, message: dict):
+        """Print messages from the backend."""
+        print_style = {
+            "error": "\033[91m",
+            "info": "\033[93m",
+            "debug": "\033[92m",
+        }
+        if (
+            key := re.search(r"error|info|debug", ",".join(message.keys()))
+        ) is not None:
+            return print(f"{print_style[key.group()]}{message[key.group()]}")
+
+        print(message)
+
+    async def recv_message(self, data: str):
+        """Creates a new task to process messages from the stdout reader."""
+        try:
+            message: dict = json.loads(data)
+            if message.get("result", None):
+                return self.recv.put(message, block=False)
+            self.print_message(message)
+        except (json.JSONDecodeError, AttributeError):
+            print(data)
+
     async def stdout_reader(self):
         """Read stdout from the backend."""
+
         try:
             while self._is_started.is_set():
                 if data := (await self.runner.stdout.readline()).decode().strip():
-                    print(data)
-
-                await asyncio.sleep(0.1)
+                    asyncio.create_task(self.recv_message(data))
+                await asyncio.sleep(0.02)
 
         except Exception as proc_err:
             await self.exception_handler(proc_err)
 
     async def stderr_reader(self):
         """Read stderr from the backend."""
         # Ignore some messages from the backend that can be confusing to users
@@ -299,15 +325,15 @@
         ignore_regex = r"(Wayland|Compositor|webkit_download|NeedDebuggerBreak)"
         try:
             while self._is_started.is_set():
                 if data := (await self.runner.stderr.readline()).decode().strip():
                     if data and not re.search(ignore_regex, data):
                         print(data)
 
-                await asyncio.sleep(0.1)
+                await asyncio.sleep(1)
 
         except Exception as proc_err:
             await self.exception_handler(proc_err)
 
     async def run_backend(self):
         """Runs the backend and starts the main loop."""
         await self.handle_start()
@@ -323,28 +349,29 @@
             await asyncio.sleep(0.1)
         try:
             if self.init_engine:
                 # if there is data in the init_engine list,
                 # we send it to the backend and clear the list
                 for msg in self.init_engine:
                     self.runner.stdin.write(f"{msg}\n".encode())
+                    await self.runner.stdin.drain()
                 self.init_engine = []
 
             while self._is_started.is_set():
                 try:
                     if self.outgoing:
                         data = self.outgoing.pop(0)
                         with self.lock:
                             self.init_engine.append(data)
                         self.runner.stdin.write(f"{data}\n".encode())
                         await self.runner.stdin.drain()
 
                         self.init_engine = []
 
-                    await asyncio.sleep(0.1)
+                    await asyncio.sleep(0.5)
 
                 except (BrokenPipeError, ConnectionResetError) as runtime_err:
                     await self.exception_handler(runtime_err)
                     await self.run_backend()
 
                 except AsyncioException as asyncio_err:
                     await self.exception_handler(asyncio_err, subtract=1)
@@ -368,28 +395,43 @@
         self.max_retries -= subtract
         await asyncio.sleep(sleep)
 
     def run(self):
         """Run the backend."""
         asyncio.run(self.run_backend())
 
-    def start(self, debug: bool = False):
-        """Creates a new thread and runs the backend in it."""
+    def start(self, debug: bool = False, headless: bool = False):
+        """Creates a new thread and runs the backend in it.
+
+        Parameters
+        ----------
+        debug : bool, optional
+            Whether to print debug messages, by default False
+        headless : bool, optional
+            Whether to run the backend in headless mode for plotly image exports,
+            by default False
+        """
         if self._is_started.is_set():
             return
         self.debug = debug
 
+        for arg, flag in zip([debug, headless], ["debug", "headless"]):
+            if arg:
+                self._bootargs.append(f"--{flag}")
+
         thread = threading.Thread(target=self.run, daemon=self.daemon)
         thread.start()
 
         with self.lock:
             if self.thread and self.thread.is_alive():
                 self.thread.join()
             self.thread = thread
 
+        if headless:
+            self.loop.run_until_complete(asyncio.sleep(3))
         self.loop.run_until_complete(self.check_backend())
 
     def close(self, reset: bool = False):  # pylint: disable=unused-argument
         """Close the backend."""
         with self.lock:
             self._is_started.clear()
             self._is_closed.set()
```

### Comparing `pywry-0.5.4/Cargo.toml` & `pywry-0.5.5/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.5.4"
+version = "0.5.5"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
```

### Comparing `pywry-0.5.4/src/pipe.rs` & `pywry-0.5.5/src/pipe.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use std::sync::mpsc::Sender;
 use tokio::io::{self, AsyncBufReadExt};
 
 pub async fn send_message(sender: Sender<String>, message: String) {
     let trimmed_line = message.trim();
     if !trimmed_line.is_empty() && trimmed_line.starts_with('{') && trimmed_line.ends_with('}') {
-        let _ = sender.send(message);
+        sender.send(message).unwrap();
     }
 }
 
 pub async fn run_listener(sender: Sender<String>) -> Result<(), Box<dyn std::error::Error>> {
     let stdin = io::stdin();
     let mut reader = io::BufReader::new(stdin);
     let rt = tokio::runtime::Runtime::new()?;
```

### Comparing `pywry-0.5.4/PKG-INFO` & `pywry-0.5.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywry
-Version: 0.5.4
+Version: 0.5.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Requires-Dist: setproctitle
@@ -13,14 +13,16 @@
 Provides-Extra: dev
 License-File: LICENSE
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PyWry Web Viewer
 
+![signal-2023-05-08-171646_002](https://github.com/OpenBB-finance/pywry/assets/25267873/a19338f7-0149-4ada-8fc7-389ae36c39fc)
+
 Easily create HTML webviewers in python utilizing the [wry](https://github.com/tauri-apps/wry) library. Unlike many HTML viewers that exist for Python - Pywry allows you to run javacsript. PyWry is also a ~2mb footprint for Mac and Windows - Linux will require a few more libraries which are listed below.
 
 Please note: this library is currently in early alpha and is NOT ready for production use.
 
 ## Installation
 
 ---------------------
```

