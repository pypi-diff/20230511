# Comparing `tmp/me_setups-1.6.9.tar.gz` & `tmp/me_setups-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "me_setups-1.6.9.tar", last modified: Thu Apr 20 07:05:09 2023, max compression
+gzip compressed data, was "me_setups-1.7.0.tar", last modified: Thu May 11 12:13:18 2023, max compression
```

## Comparing `me_setups-1.6.9.tar` & `me_setups-1.7.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-20 07:05:09.090435 me_setups-1.6.9/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-04-20 07:05:09.091765 me_setups-1.6.9/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.6.9/README.md
--rw-r--r--   0 idof     (12090585) develop   (1000)     1192 2023-04-20 07:05:09.121060 me_setups-1.6.9/setup.cfg
--rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.6.9/setup.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-20 07:05:09.024309 me_setups-1.6.9/src/
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-20 07:05:09.041357 me_setups-1.6.9/src/me_setups/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.6.9/src/me_setups/__init__.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-20 07:05:09.070338 me_setups-1.6.9/src/me_setups/boards/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.6.9/src/me_setups/boards/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.6.9/src/me_setups/boards/default_boards.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    10927 2023-04-20 07:02:32.000000 me_setups-1.6.9/src/me_setups/boards/gas52.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.6.9/src/me_setups/boards/types.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-20 07:05:09.087410 me_setups-1.6.9/src/me_setups/components/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.6.9/src/me_setups/components/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     8506 2023-04-17 14:42:22.000000 me_setups-1.6.9/src/me_setups/components/comp.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    11985 2023-04-20 07:02:32.000000 me_setups-1.6.9/src/me_setups/components/eqs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      178 2023-02-20 11:40:34.000000 me_setups-1.6.9/src/me_setups/components/mcs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     4047 2023-02-27 18:33:55.000000 me_setups-1.6.9/src/me_setups/components/mcu.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-03-15 13:23:19.000000 me_setups-1.6.9/src/me_setups/utils.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-20 07:05:09.057312 me_setups-1.6.9/src/me_setups.egg-info/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-04-20 07:05:08.000000 me_setups-1.6.9/src/me_setups.egg-info/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-04-20 07:05:08.000000 me_setups-1.6.9/src/me_setups.egg-info/SOURCES.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-04-20 07:05:08.000000 me_setups-1.6.9/src/me_setups.egg-info/dependency_links.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-04-20 07:05:08.000000 me_setups-1.6.9/src/me_setups.egg-info/requires.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-04-20 07:05:08.000000 me_setups-1.6.9/src/me_setups.egg-info/top_level.txt
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-05-11 12:13:18.112064 me_setups-1.7.0/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-05-11 12:13:18.112963 me_setups-1.7.0/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.7.0/README.md
+-rw-r--r--   0 idof     (12090585) develop   (1000)     1242 2023-05-11 12:13:18.114179 me_setups-1.7.0/setup.cfg
+-rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.7.0/setup.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-05-11 12:13:18.071964 me_setups-1.7.0/src/
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-05-11 12:13:18.082531 me_setups-1.7.0/src/me_setups/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.7.0/src/me_setups/__init__.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-05-11 12:13:18.098998 me_setups-1.7.0/src/me_setups/boards/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.7.0/src/me_setups/boards/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.7.0/src/me_setups/boards/default_boards.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    11329 2023-05-11 12:09:03.000000 me_setups-1.7.0/src/me_setups/boards/gas52.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.7.0/src/me_setups/boards/types.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-05-11 12:13:18.110539 me_setups-1.7.0/src/me_setups/components/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.7.0/src/me_setups/components/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     8962 2023-05-11 12:09:03.000000 me_setups-1.7.0/src/me_setups/components/comp.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    12717 2023-05-11 12:09:03.000000 me_setups-1.7.0/src/me_setups/components/eqs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      198 2023-05-11 12:09:03.000000 me_setups-1.7.0/src/me_setups/components/mcs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     4187 2023-05-11 12:09:03.000000 me_setups-1.7.0/src/me_setups/components/mcu.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-03-15 13:23:19.000000 me_setups-1.7.0/src/me_setups/utils.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-05-11 12:13:18.093674 me_setups-1.7.0/src/me_setups.egg-info/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-05-11 12:13:18.000000 me_setups-1.7.0/src/me_setups.egg-info/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-05-11 12:13:18.000000 me_setups-1.7.0/src/me_setups.egg-info/SOURCES.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-05-11 12:13:18.000000 me_setups-1.7.0/src/me_setups.egg-info/dependency_links.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-05-11 12:13:18.000000 me_setups-1.7.0/src/me_setups.egg-info/requires.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-05-11 12:13:18.000000 me_setups-1.7.0/src/me_setups.egg-info/top_level.txt
```

### Comparing `me_setups-1.6.9/PKG-INFO` & `me_setups-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me_setups
-Version: 1.6.9
+Version: 1.7.0
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.6.9/setup.cfg` & `me_setups-1.7.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = me_setups
-version = 1.6.9
+version = 1.7.0
 description = Abstraction for Mobileye setups.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://gitlab.mobileye.com/idof/me-setups
 author = Ido Frenkel
 author_email = ido.frenkel@mobileye.com
 classifiers = 
@@ -30,14 +30,16 @@
 	testing*
 
 [bdist_wheel]
 universal = True
 
 [coverage:run]
 plugins = covdefaults
+omit = 
+	*/lib/*
 
 [flake8]
 max-line-length = 88
 extend-ignore = E203
 
 [mypy]
 check_untyped_defs = true
@@ -48,12 +50,13 @@
 warn_unused_ignores = true
 
 [mypy-testing.*]
 disallow_untyped_defs = false
 
 [mypy-tests.*]
 disallow_untyped_defs = false
+disallow_incomplete_defs = false
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `me_setups-1.6.9/src/me_setups/boards/default_boards.py` & `me_setups-1.7.0/src/me_setups/boards/default_boards.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.6.9/src/me_setups/boards/gas52.py` & `me_setups-1.7.0/src/me_setups/boards/gas52.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import time
 from concurrent.futures import as_completed
 from concurrent.futures import ThreadPoolExecutor
 from subprocess import CompletedProcess
 from typing import Any
 from typing import Generator
 
-if sys.version_info >= (3, 8):
+if sys.version_info >= (3, 8):  # pragma: >=3.8 cover
     from typing import Literal
-else:
+else:  # pragma: <3.8 cover
     from typing_extensions import Literal
 
 from me_setups.boards.types import BoardType
 from me_setups.components.eqs import CoreType
 from me_setups.components.eqs import EyeQ5
 from me_setups.components.eqs import OSType
 from me_setups.components.mcs import Mcs
@@ -62,15 +62,15 @@
               Defaults to "0x3".
         """
         self.logger = logging.getLogger(self.__class__.__name__)
         self.eqs = eqs if eqs else self.create_eqs()
         self.mcu = mcu if mcu else self.create_mcu()
         if pathlib.Path("/dev/MCS").exists():
             self.mcs = Mcs("MCS", "/dev/MCS")
-        else:
+        else:  # pragma: no cover
             self.mcs = None
         self.switch_ver = None
         self.shiq = self.eqs[1]
         self.board_type = board_type
         self.board_name = board_name
         self.board_rev = board_rev
         self._sniffing = False
@@ -80,15 +80,15 @@
         """get all connections
 
         Returns:
             list[EyeQ5 | Mcu | Mcs] | list[EyeQ5 | Mcu]: All serial connections
         """
         conns: list[EyeQ5 | Mcu | Mcs] | list[EyeQ5 | Mcu]
         conns = self.eqs + [self.mcu]
-        if self.mcs is not None:
+        if self.mcs is not None:  # pragma: no branch
             conns = conns + [self.mcs]
         return conns
 
     @contextlib.contextmanager
     def sniff(
         self,
         log_folder: pathlib.Path | str,
@@ -104,16 +104,15 @@
               Defaults to 'a'.
         """
         self.config_log_files(log_folder, mode)
         try:
             self.start_sniffing()
             yield
         finally:
-            if self._sniffing:
-                self.stop_sniffing()
+            self.stop_sniffing()
 
     def start_sniffing(self) -> None:
         """start the sniffing thread for each conn"""
         if self._sniffing:
             return None
 
         self._sniffing = True
@@ -123,14 +122,18 @@
     def stop_sniffing(self) -> None:
         """stop the sniffing thread for each conn"""
         if not self._sniffing:
             return None
 
         for conn in self.conns:
             conn.serial.stop_sniffing()
+
+        for conn in self.conns:
+            conn.serial.sniff_thread.join(10)
+
         self._sniffing = False
 
     def get_eyeq(self, chip: int, mid: int) -> EyeQ5:
         """get eq using chip and mid
 
         Args:
             chip (int): the chip index of the eq
@@ -257,24 +260,26 @@
             NotImplementedError: if reboot is not supported for the board.
         """
         if self.board_type == BoardType.EVO:
             raise NotImplementedError("reboot is not support on EVO")
 
         self.logger.info("rebooting platform...")
 
-        if self.mcs is not None:
+        if self.mcs is not None:  # pragma: no branch
             self.logger.debug("rebooting MCS")
             self.mcs.run_serial_cmd("reboot")
 
         self.logger.debug("rebooting board")
         self.mcu.run_serial_cmd("reboot")
 
         if sleep_after > 0:
             self.logger.info(f"sleeping for {sleep_after} seconds.")
             time.sleep(sleep_after)
+        else:  # pragma: no cover
+            pass
 
     def is_alive(self, timeout: float = 1, frames: int = 10) -> bool:
         """Return if all EQs is alive - MEST and frames is running.
 
         Args:
             timeout (float, optional): timeout to wait until frames. Defaults to 1.
             frames (int, optional): how many frames to wait for. Defaults to 10.
@@ -304,15 +309,20 @@
             dst (pathlib.Path | str): Path to folder to extract to
 
         Returns:
             list[CompletedProcess[str] | None]: status of extracting process.
         """
         with ThreadPoolExecutor(max_workers=len(self.eqs)) as executor:
             fs = [executor.submit(eq.copy_cores, dst, timeout) for eq in self.eqs]
-        return [f.result() for f in fs]
+        result = [f.result() for f in fs]
+        if any(
+            res.returncode != 0 for res in result if res is not None
+        ):  # pragma: no cover
+            self.logger.error("Copying cores failed!")
+        return result
 
     @staticmethod
     def create_eqs(
         pbcm_ports: dict[str, str] = DEFAULT_PBCM_PORTS,
         os_type: OSType = OSType.LINUX,
     ) -> list[EyeQ5]:
         return [EyeQ5(pbcm, port, os_type) for pbcm, port in pbcm_ports.items()]
@@ -322,8 +332,8 @@
         pbc: str = "000",
         port: str = "/dev/MCUE_PBC_000",
         mcu_type: McuType = McuType.ADAM,
     ) -> Mcu:
         return Mcu(pbc, port, mcu_type)
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(eqs={self.eqs}, mcu={self.mcu})"
+        return f"{self.__class__.__name__}(eqs={self.eqs!r}, mcu={self.mcu!r})"
```

### Comparing `me_setups-1.6.9/src/me_setups/components/comp.py` & `me_setups-1.7.0/src/me_setups/components/comp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
 import contextlib
+import datetime
 import logging
 import pathlib
 import sys
 import threading
-from datetime import datetime
 from io import TextIOWrapper
 from time import sleep
 from types import TracebackType
 from typing import Any
 from typing import Generator
 
-if sys.version_info >= (3, 8):
+if sys.version_info >= (3, 8):  # pragma: >=3.8 cover
     from typing import Literal
-else:
+else:  # pragma: <3.8 cover
     from typing_extensions import Literal
 
 from serial import Serial
 from serial import SerialException
 from serial.threaded import LineReader
 
 from me_setups.utils import filter_ansi_escape
@@ -33,15 +33,15 @@
         line (str): line to add timestamp to
 
     Returns:
         str: the line with timestamp prefix - e.g. "[12:24:33.168423] <line>"
     """
 
     def timestamp() -> str:
-        return datetime.now().strftime("[%H:%M:%S.%f]")
+        return datetime.datetime.now().strftime("[%H:%M:%S.%f]")
 
     return f"{timestamp()} {line}"
 
 
 class Sniffer(LineReader):
     TERMINATOR = b"\n"
     log_file: TextIOWrapper | None
@@ -65,17 +65,17 @@
     def handle_line(self, data: str) -> None:
         """handle line and write it to the log file if it is not None
 
         Args:
             data (str): line recived
         """
         if self.log_file is not None:
-            if self.clean_line:
+            if self.clean_line:  # pragma: no cover
                 data = filter_ansi_escape(data)
-            if self.add_timestamp:
+            if self.add_timestamp:  # pragma: no cover
                 data = add_line_timestamp(data)
             self.log_file.write(f"{data}\n")
 
 
 class ReaderThread(threading.Thread):
     def __init__(self, serial: Serial, *args: Any, **kwargs: Any) -> None:
         """create a sniffing thread that allways reads the given serial
@@ -89,40 +89,39 @@
         self.alive = threading.Event()
 
     def stop(self) -> None:
         """\
             Stop sniffing
         """
         self.alive.clear()
-        self.join(5)
 
     def run(self) -> None:
         self.alive.set()
         while self.alive.is_set() and self.serial.is_open:
             try:
                 self.serial.read(self.serial.in_waiting or 1)
-            except SerialException:
+            except SerialException:  # pragma: no cover
                 break
-            except OSError:
+            except OSError:  # pragma: no cover
                 self.serial.close()
                 self.serial.open()
                 self.serial.read(self.serial.in_waiting or 1)
-        if self.alive.is_set():
+        if self.alive.is_set():  # pragma: no cover
             self.alive.clear()
 
-    def __enter__(self) -> ReaderThread:
+    def __enter__(self) -> ReaderThread:  # pragma: no cover
         self.start()
         return self
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc: BaseException | None,
         traceback: TracebackType | None,
-    ) -> bool | None:
+    ) -> bool | None:  # pragma: no cover
         self.stop()
         if exc_type or exc or traceback:
             return False
         else:
             return None
 
 
@@ -150,15 +149,15 @@
         self.protocol.data_received(data)
         return data
 
     @contextlib.contextmanager
     def change_timeout_ctx(
         self,
         timeout: float,
-    ) -> Generator[None, None, None]:
+    ) -> Generator[None, None, None]:  # pragma: no cover
         """contextmanager for temporary change the serial timeout
 
         Args:
             timeout (float): the new timeout for the serial
         """
         orig_timeout = self.timeout
         try:
@@ -169,32 +168,32 @@
 
     def start_sniffing(self) -> ReaderThread:
         """start the sniffing thread
 
         Returns:
             ReaderThread: The sniffing thread
         """
-        if not self.sniff_thread.is_alive():
+        if not self.sniff_thread.is_alive():  # pragma: no cover
             self.sniff_thread = ReaderThread(self)
         self.sniff_thread.start()
         return self.sniff_thread
 
     def stop_sniffing(self) -> None:
         """\
             Stops the Sniffing thread
         """
-        if self.sniff_thread.alive.is_set():
+        if self.sniff_thread.alive.is_set():  # pragma: no cover
             self.sniff_thread.stop()
 
     def config_sniffer(
         self,
         *,
         clean_line: bool = True,
         add_timestamp: bool = True,
-    ) -> None:
+    ) -> None:  # pragma: no cover
         self.protocol.clean_line = clean_line
         self.protocol.add_timestamp = add_timestamp
 
 
 class Component:
     def __init__(self, pbcm: str, port: str) -> None:
         """Base Component containing SerialSniffer by default
@@ -209,15 +208,15 @@
 
     @property
     def prompt(self) -> bytes:
         raise NotImplementedError
 
     @property
     def name(self) -> str:
-        return self._pbcm
+        return self.__str__()
 
     @contextlib.contextmanager
     def sniff(
         self,
         log_file: pathlib.Path | str,
         mode: Literal["w", "a"] = "a",
     ) -> Generator[None, None, None]:
@@ -255,15 +254,15 @@
     ) -> None:
         """config log file for the sniffer.
 
         Args:
             log_file (pathlib.Path | str): path for the log file.
             mode (Literal['w', 'a'], optional): like open(). Defaults to 'a'.
         """
-        if self.serial.sniff_thread.alive.is_set():
+        if self.serial.sniff_thread.alive.is_set():  # pragma: no cover
             self.serial.stop_sniffing()
             assert self.serial.protocol.log_file
             self.serial.protocol.log_file.close()
 
         self.logger.debug(f"configuring log file for serial - {str(log_file)!r}")
         log_file = pathlib.Path(log_file)
         log_file.parent.mkdir(parents=True, exist_ok=True)
@@ -279,23 +278,27 @@
 
         Returns:
             bytes: all data that been read while waiting for the msg.
         """
         self.logger.debug(f"waiting for msg {msg.decode()!r}")
 
         restart_sniffing = False
-        if self.serial.sniff_thread.alive.is_set():
+        if self.serial.sniff_thread.alive.is_set():  # pragma: no cover
             restart_sniffing = True
             self.serial.stop_sniffing()
 
         with self.serial.change_timeout_ctx(timeout):
-            if not self.serial.is_open:
+            if not self.serial.is_open:  # pragma: no cover
                 self.serial.open()
             res = self.serial.read_until(msg)
 
-        if restart_sniffing:
+        if restart_sniffing:  # pragma: no cover
             self.serial.start_sniffing()
 
         return res
 
+    def __str__(self) -> str:
+        return self.__class__.__name__
+
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({self.name})"
+        cls_name = self.__class__.__name__
+        return f"{cls_name}(pbcm={self._pbcm!r}, port={self.serial.port!r})"
```

### Comparing `me_setups-1.6.9/src/me_setups/components/eqs.py` & `me_setups-1.7.0/src/me_setups/components/eqs.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,23 +49,14 @@
             port (str): serial port path e.g. (/dev/ttyUSB2)
             os_type (OSType, optional): The OS type of the EQ. Defaults to LINUX.
         """
         super().__init__(pbcm, port)
         self.os_type = os_type
 
     @property
-    def name(self) -> str:
-        """name of the EQ in this format - 'EQ5_PBCM_<pbcm>'
-
-        Returns:
-            str: the name of the EQ
-        """
-        return f"EQ5_PBCM_{self._pbcm}"
-
-    @property
     def chip(self) -> int:
         """the chip of the EQ
 
         Returns:
             int: the chip of the EQ
         """
         return int(self._pbcm[-2])
@@ -92,33 +83,33 @@
     def ip(self) -> str | None:
         """the IP of the EQ
 
         Returns:
             str | None: the EQ IP for the current OS
         """
         if self.name == "EQ5_PBCM_0000":
-            if self.os_type == OSType.VOIS:
+            if self.os_type == OSType.VOIS:  # pragma: no cover
                 return "169.254.0.11"
             else:
                 return "192.168.19.129"
 
         elif self.name == "EQ5_PBCM_0001":
-            if self.os_type == OSType.VOIS:
+            if self.os_type == OSType.VOIS:  # pragma: no cover
                 return "169.254.0.12"
             else:
                 return "192.168.19.113"
 
         elif self.name == "EQ5_PBCM_0010":
-            if self.os_type == OSType.VOIS:
+            if self.os_type == OSType.VOIS:  # pragma: no cover
                 return "169.254.0.13"
             else:
                 return "192.168.19.105"
 
         elif self.name == "EQ5_PBCM_0011":
-            if self.os_type == OSType.VOIS:
+            if self.os_type == OSType.VOIS:  # pragma: no cover
                 return "169.254.0.14"
             else:
                 return "192.168.19.121"
 
         else:
             raise NotImplementedError(f"ip for {self.name} is not implemented")
 
@@ -173,15 +164,15 @@
             timeout (float, optional): timeout for the copy. Defaults to 5.
             recurcive (bool, optional): recurcive copy includs dirs. Defaults to False.
 
         Returns:
             CompletedProcess[str]: the process
         """
         dst = pathlib.Path(dst)
-        if mkdir:
+        if mkdir:  # pragma: no cover
             self.run_ssh_cmd(f"mkdir -p {dst.parent}")
         return self._scp(
             str(src),
             f"{self._ssh_root}:{dst}",
             timeout,
             recurcive,
             **kwargs,
@@ -201,15 +192,15 @@
         Returns:
             CompletedProcess[str] | None: status of extracting process None if no cores
         """
         cores = self.ssh_cmd_stdout("find /media/storage/crash/ -type f").splitlines()
         if not cores:
             return None
         if not all(core.endswith(".zip") for core in cores):
-            self.wait_for_core_write(core_type=CoreType.PCD)
+            self.wait_for_core_write(core_type=CoreType.PCD)  # pragma: no cover
         return self.copy_from(
             f"{self.crash_folder}/*",
             pathlib.Path(dst) / self.name,
             timeout=timeout,
             recurcive=True,
             mkdir=True,
         )
@@ -217,27 +208,34 @@
     def wait_for_linux_boot(self) -> bool:
         """waits to Linux boot msg "Welcome to EyeQ5"
 
         Returns:
             bool: boot msg recived
         """
         boot_msg = b"Welcome to EyeQ5"
-        return boot_msg in self.wait_for_msg(boot_msg, 120)
+        if boot_msg in self.wait_for_msg(boot_msg, 120):
+            self.logger.debug("Linux boot success waiting 5 seconds for MEST init")
+            time.sleep(5)
+            return True
+        else:  # pragma: no cover
+            self.logger.warning("Linux boot msg did not recived")
+            return False
 
     def get_all_frames(self) -> list[str]:
         """get all frames ran from the app_log
 
         Returns:
             list[str]: list contain all frames that ran
         """
         frames_string = "running frame:"
         pat = re.compile(rf"{frames_string} (\d+)", re.IGNORECASE)
         stdout = self.ssh_cmd_stdout(
             f"grep -i {frames_string!r} /tmp/app_log.txt",
             skip_logging=True,
+            verbose=False,
         )
         return list(dict.fromkeys(pat.findall(stdout)))
 
     def wait_for_frames(
         self,
         timeout: float = 180,
         frames: int = 10,
@@ -247,20 +245,22 @@
         Args:
             timeout (float, optional): how much time to wait. Defaults to 180.
             frames (int, optional): how many frames to wait for. Defaults to 10.
 
         Returns:
             bool: if we got the given number of frames
         """
+        all_frames = []
         _timeout = time.time() + timeout
         while time.time() < _timeout:
             all_frames = self.get_all_frames()
             if len(all_frames) > frames:
                 self.logger.debug(f"last frame is: {all_frames[-1]}")
                 return True
+            time.sleep(1)
 
         self.logger.warning(f"did not run {frames} frames. frames got={all_frames}")
         return False
 
     def is_mest_alive(self) -> bool:
         """Return if MEST is alive"""
         return self.ssh_cmd_stdout("pgrep cv_main_thread") != ""
@@ -328,15 +328,15 @@
             list[str]: list of file in dir.
         """
         ls_cmd = self.run_ssh_cmd(f"ls -1 {_dir}")
         if ls_cmd.returncode == 0:
             return ls_cmd.stdout.splitlines()
         elif "No such file or directory" in ls_cmd.stderr:
             raise FileNotFoundError(ls_cmd.stderr)
-        else:
+        else:  # pragma: no cover
             raise Exception(ls_cmd.stderr)
 
     def wait_for_core_write(
         self,
         core_type: CoreType = CoreType.PCD,
         timeout: float = 180,
     ) -> bool:
@@ -350,15 +350,15 @@
 
         Returns:
             bool: if the core msg has recived.
         """
         self.logger.debug(f"Waiting for {core_type.name} write completion")
         if core_type == CoreType.PCD:
             core_complete_msg = PCD_WRITE_COMPLETE
-        elif core_type == CoreType.FCD:
+        elif core_type == CoreType.FCD:  # pragma: no cover
             core_complete_msg = FCD_WRITE_COMPLETE
         else:
             raise NotImplementedError
         read_from_ser = self.wait_for_msg(core_complete_msg, timeout)
         res = core_complete_msg in read_from_ser
         if not res:
             self.logger.warning(
@@ -372,18 +372,20 @@
         return self.run_ssh_cmd(f"rm -rf {self.crash_folder}", timeout=20)
 
     def _sp_cmd(
         self,
         cmd: list[str],
         timeout: float,
         skip_logging: bool = False,
+        verbose: bool = True,
         **kwargs: Any,
     ) -> CompletedProcess[str]:
-        if not skip_logging:
-            self.logger.debug(f"[ssh] running cmd: {' '.join(cmd)!r}")
+        str_cmd = " ".join(cmd)
+        if verbose:
+            self.logger.debug(f"[ssh] running cmd: {str_cmd!r}")
         try:
             res = subprocess.run(
                 cmd,
                 capture_output=True,
                 timeout=timeout,
                 text=True,
                 **kwargs,
@@ -394,14 +396,17 @@
         if not skip_logging:
             self.logger.debug(
                 "cmd result: ("
                 f"returncode={res.returncode}, "
                 f"stdout={res.stdout!r}, "
                 f"stderr={res.stderr!r})",
             )
+        if verbose and res.returncode != 0:
+            self.logger.warning(f"cmd {str_cmd!r} return code is {res.returncode}")
+            self.logger.warning(f"cmd {str_cmd!r} stderr: {res.stderr!r}")
         return res
 
     def _scp(
         self,
         _from: str,
         _to: str,
         timeout: float = 5,
@@ -410,7 +415,15 @@
     ) -> CompletedProcess[str]:
         cmd = ["scp"] + NO_KEY_CHECK
         if recurcive:
             cmd += ["-r"]
         cmd += [_from]
         cmd += [_to]
         return self._sp_cmd(cmd, timeout, **kwargs)
+
+    def __str__(self) -> str:
+        """name of the EQ in this format - 'EQ5_PBCM_<pbcm>'
+
+        Returns:
+            str: the name of the EQ
+        """
+        return f"EQ5_PBCM_{self._pbcm}"
```

### Comparing `me_setups-1.6.9/src/me_setups/components/mcu.py` & `me_setups-1.7.0/src/me_setups/components/mcu.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,41 +40,41 @@
 
     @property
     def name(self) -> str:
         return f"MCUE_PBC_{self._pbcm}"
 
     @property
     def prompt(self) -> bytes:
-        if self.mcu_type == McuType.MEAVES:
+        if self.mcu_type == McuType.MEAVES:  # pragma: no cover
             return b"Shell>"
         elif self.mcu_type == McuType.ADAM:
             return b">>"
-        elif self.mcu_type == McuType.ASR:
+        elif self.mcu_type == McuType.ASR:  # pragma: no cover
             return b">"
         else:
             raise NotImplementedError
 
     @property
     def ip(self) -> str:
         if self._ip is not None:
             return self._ip
         elif self.mcu_type == McuType.ADAM:
             return "192.168.19.16"
-        elif self.mcu_type == McuType.MEAVES:
+        elif self.mcu_type == McuType.MEAVES:  # pragma: no cover
             return "192.168.19.20"
         else:
             raise NotImplementedError
 
     @ip.setter
     def ip(self, ip: str) -> None:
         self._ip = ip
 
     @property
     def port(self) -> int:
-        if self.mcu_type == McuType.MEAVES:
+        if self.mcu_type == McuType.MEAVES:  # pragma: no cover
             return 9995
         elif self.mcu_type == McuType.ADAM:
             return 4200
         else:
             raise NotImplementedError
 
     @property
@@ -83,37 +83,37 @@
 
     @staticmethod
     def get_eq_name(which_eq: EyeQ5 | str) -> str:
         if isinstance(which_eq, str):
             return which_eq
         return f"EQ{which_eq.chip + 1}.{which_eq.mid}"
 
-    def set_eq_bootmode(self, eq: EyeQ5 | str, mode: str) -> bool:
+    def set_eq_bootmode(self, eq: EyeQ5 | str, mode: str) -> bool:  # pragma: no cover
         eq_name = self.get_eq_name(eq)
         if self.mcu_type == McuType.ADAM:
             cmd = f"set -e {eq_name} -b {mode}"
         elif self.mcu_type in (McuType.MEAVES, McuType.ASR):
             cmd = f"set {eq_name} bootmode {mode}"
         else:
             raise NotImplementedError
         self.run_serial_cmd(cmd)
         return True
 
-    def reset_eq(self, eq: EyeQ5 | str) -> bool:
+    def reset_eq(self, eq: EyeQ5 | str) -> bool:  # pragma: no cover
         eq_name = self.get_eq_name(eq)
         if self.mcu_type == McuType.ADAM:
             cmd = f"reset -e {eq_name}"
         elif self.mcu_type in (McuType.MEAVES, McuType.ASR):
             cmd = f"reset {eq_name}"
         else:
             raise NotImplementedError
         self.run_serial_cmd(cmd)
         return True
 
-    def set_eq_uboot(self, eq: EyeQ5 | str, status: str) -> bool:
+    def set_eq_uboot(self, eq: EyeQ5 | str, status: str) -> bool:  # pragma: no cover
         eq_name = self.get_eq_name(eq)
         if self.mcu_type == McuType.ADAM:
             cmd = f"set -e {eq_name} -u {status}"
         elif self.mcu_type == McuType.MEAVES:
             cmd = f"set {eq_name} uboot {status}"
         else:
             raise NotImplementedError
```

### Comparing `me_setups-1.6.9/src/me_setups.egg-info/PKG-INFO` & `me_setups-1.7.0/src/me_setups.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me-setups
-Version: 1.6.9
+Version: 1.7.0
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.6.9/src/me_setups.egg-info/SOURCES.txt` & `me_setups-1.7.0/src/me_setups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

