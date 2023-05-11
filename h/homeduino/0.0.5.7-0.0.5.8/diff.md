# Comparing `tmp/homeduino-0.0.5.7.tar.gz` & `tmp/homeduino-0.0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeduino-0.0.5.7.tar", last modified: Tue Mar  7 00:37:43 2023, max compression
+gzip compressed data, was "homeduino-0.0.5.8.tar", last modified: Thu May 11 16:46:52 2023, max compression
```

## Comparing `homeduino-0.0.5.7.tar` & `homeduino-0.0.5.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 00:37:43.286609 homeduino-0.0.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-03-07 00:37:33.000000 homeduino-0.0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-07 00:37:43.286609 homeduino-0.0.5.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 00:37:43.286609 homeduino-0.0.5.7/homeduino/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-07 00:37:33.000000 homeduino-0.0.5.7/homeduino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-03-07 00:37:33.000000 homeduino-0.0.5.7/homeduino/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-03-07 00:37:33.000000 homeduino-0.0.5.7/homeduino/homeduino.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 00:37:43.286609 homeduino-0.0.5.7/homeduino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-07 00:37:43.000000 homeduino-0.0.5.7/homeduino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-07 00:37:43.000000 homeduino-0.0.5.7/homeduino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 00:37:43.000000 homeduino-0.0.5.7/homeduino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-07 00:37:43.000000 homeduino-0.0.5.7/homeduino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-07 00:37:43.000000 homeduino-0.0.5.7/homeduino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-07 00:37:33.000000 homeduino-0.0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 00:37:43.286609 homeduino-0.0.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:46:52.451246 homeduino-0.0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-11 16:46:32.000000 homeduino-0.0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-11 16:46:52.451246 homeduino-0.0.5.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:46:52.451246 homeduino-0.0.5.8/homeduino/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-11 16:46:32.000000 homeduino-0.0.5.8/homeduino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-11 16:46:32.000000 homeduino-0.0.5.8/homeduino/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-05-11 16:46:32.000000 homeduino-0.0.5.8/homeduino/homeduino.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:46:52.451246 homeduino-0.0.5.8/homeduino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-11 16:46:52.000000 homeduino-0.0.5.8/homeduino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-11 16:46:52.000000 homeduino-0.0.5.8/homeduino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:46:52.000000 homeduino-0.0.5.8/homeduino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 16:46:52.000000 homeduino-0.0.5.8/homeduino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 16:46:52.000000 homeduino-0.0.5.8/homeduino.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-11 16:46:32.000000 homeduino-0.0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:46:52.451246 homeduino-0.0.5.8/setup.cfg
```

### Comparing `homeduino-0.0.5.7/LICENSE` & `homeduino-0.0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `homeduino-0.0.5.7/PKG-INFO` & `homeduino-0.0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeduino
-Version: 0.0.5.7
+Version: 0.0.5.8
 Summary: Homeduino library
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/homeduino.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/homeduino.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `homeduino-0.0.5.7/homeduino/__main__.py` & `homeduino-0.0.5.8/homeduino/__main__.py`

 * *Files identical despite different names*

### Comparing `homeduino-0.0.5.7/homeduino/homeduino.py` & `homeduino-0.0.5.8/homeduino/homeduino.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,53 @@
 import asyncio
 import logging
 import os
 import sys
 import time
 from asyncio.transports import BaseTransport
 from collections import deque
+from datetime import datetime
 from functools import partial
 from typing import Any, Optional
 
 import serial_asyncio
 from rfcontrol import controller
+from serial.serialutil import SerialException
 from serial_asyncio import SerialTransport
-from datetime import datetime
 
 logger = logging.getLogger(__name__)
 
 _RESPONSE_TIMEOUT = 1
+_BUSY_TIMEOUT = 1
 
 
 class HomeduinoError(Exception):
     """Generic Homeduino error."""
 
 
 class ResponseTimeoutError(HomeduinoError):
     """
     Response timeout error.
 
     If the response takes to long to receive.
     """
 
+
+class DisconnectedError(HomeduinoError):
+    """Homeduino Disconnected error."""
+
+
+class NotReadyError(HomeduinoError):
+    """Homeduino not ready error."""
+
+
+class TooBusyError(HomeduinoError):
+    """Homeduino Disconnected error."""
+
+
 class HomeduinoProtocol(asyncio.Protocol):
     rf_receive_callbacks = []
 
     transport: SerialTransport = None
 
     ready = False
     _tx_busy = False
@@ -70,78 +85,82 @@
             decoded_data = data.decode()
         except UnicodeDecodeError:
             invalid_data = data.decode(errors="replace")
             logger.warning(
                 "Error during decode of data, invalid data: %s", invalid_data
             )
         else:
-            logger.debug("received data: %s", decoded_data.strip())
+            logger.debug("Received data: %s", decoded_data.strip())
             self._str_buffer += decoded_data
             while "\r\n" in self._str_buffer:
                 line, self._str_buffer = self._str_buffer.split("\r\n", 1)
                 line = line.strip()
                 if line == "ready":
                     self.handle_ready()
                 elif line.startswith("RF receive "):
                     self.handle_rf_receive(line)
                 elif line.startswith("KP "):
                     self.handle_key_press(line)
                 elif line != "" and self._tx_busy:
                     self.str_buffer.append(line)
 
-    def handle_ready(self):
+    def handle_ready(self) -> None:
         self.ready = True
         logger.info("Homeduino is connected")
 
-    def handle_rf_receive(self, line: str):
+    def handle_rf_receive(self, line: str) -> None:
         logger.debug(line)
 
         # The first 8 numbers are the pulse lengths and the last string of numbers is the pulse sequence
         parts = line.split(" ")
 
         pulse_lengths = [int(i) for i in parts[2:9]]
         # logger.debug("pulse lengths: %s", pulse_lengths)
         pulse_sequence = parts[10]
 
         # Match pulse sequence to a protocol
         decoded = controller.decode_pulses(pulse_lengths, pulse_sequence)
 
         if len(decoded) == 0:
-            logger.warn("No protocol for %s %s", pulse_lengths, pulse_sequence)
+            logger.warning("No protocol for %s %s", pulse_lengths, pulse_sequence)
         elif len(self.rf_receive_callbacks) == 0:
             logger.debug("No receive callbacks configured")
         else:
             for protocol in decoded:
                 logger.debug("Forwarding RF protocol to receive callbacks")
                 for rf_receive_callback in self.rf_receive_callbacks:
                     rf_receive_callback(protocol)
 
-    def handle_key_press(self, line: str):
+    def handle_key_press(self, line: str) -> None:
         logger.debug(line)
         # Ignoring key presses for now
 
     async def send(self, packet: str) -> str:
         """Encode and put packet string onto write buffer."""
 
         if not self.transport:
-            logger.error("Not connected")
-            return None
+            raise DisconnectedError("Homeduino is not connected")
 
         if not self.ready:
             logger.error("Not ready")
-            return None
+            raise NotReadyError("Homeduino is not ready")
 
+        start_time = datetime.now()
         while self._tx_busy is True:
-            logger.info("Too busy to transmit %s", packet)
-            await asyncio.sleep(0.1)
+            logger.debug("Busy")
+            if (datetime.now() - start_time).total_seconds() < _BUSY_TIMEOUT:
+                await asyncio.sleep(0.1)
+            else:
+                logger.error("Too busy to transmit %s", packet)
+                raise TooBusyError("Homeduino is too busy to transmit")
         self._tx_busy = True
 
         try:
             data = packet + "\n"
-            logger.debug("writing data: %s", repr(data))
+            logger.debug("Writing data: %s", repr(data))
             # type ignore: transport from create_connection is documented to be
             # implementation specific bidirectional, even though typed as
             # BaseTransport
             self.transport.write(data.encode())  # type: ignore
 
             # Wait for response
             logger.debug("Waiting for command response")
@@ -157,106 +176,118 @@
             raise ResponseTimeoutError("Timeout while waiting for command response")
         finally:
             self._tx_busy = False
 
         return None
 
     def connection_lost(self, exc: Optional[Exception]) -> None:
-        logger.info("port closed")
+        logger.info("Port closed")
         if exc:
-            logger.exception("disconnected due to exception")
+            logger.exception("Disconnected due to exception")
         else:
-            logger.info("disconnected because of close/abort.")
+            logger.info("Disconnected because of close/abort")
 
         self.transport = None
         self.ready = False
 
 
 class Homeduino:
-    transport: SerialTransport = None
     protocol: HomeduinoProtocol = None
     rf_receive_callbacks = []
 
     def __init__(
         self,
         serial_port: str,
         receive_pin: int,
         send_pin: int,
         dht_pin: int = None,
         loop=None,
     ):
         # Test if the device exists
         if not os.path.exists(serial_port):
-            logger.warn("No such file or directory: '%s'", serial_port)
+            logger.warning("No such file or directory: '%s'", serial_port)
 
         self.serial_port = serial_port
         # self.receive_pin = receive_pin
         self.receive_interrupt = receive_pin - 2
         self.send_pin = send_pin
         self.dht_pin = dht_pin
 
         if loop is None:
             loop = asyncio.get_event_loop()
         self.loop = loop
 
     async def connect(self) -> bool:
-        if self.transport is None:
-            protocol_factory = partial(HomeduinoProtocol, loop=self.loop)
+        if not self.connected():
+            try:
+                protocol_factory = partial(HomeduinoProtocol, loop=self.loop)
+
+                (
+                    _transport,
+                    self.protocol,
+                ) = await serial_asyncio.create_serial_connection(
+                    self.loop,
+                    protocol_factory,
+                    self.serial_port,
+                    baudrate=115200,
+                    bytesize=serial_asyncio.serial.EIGHTBITS,
+                    parity=serial_asyncio.serial.PARITY_NONE,
+                    stopbits=serial_asyncio.serial.STOPBITS_ONE,
+                )
 
-            (
-                self.transport,
-                self.protocol,
-            ) = await serial_asyncio.create_serial_connection(
-                self.loop,
-                protocol_factory,
-                self.serial_port,
-                baudrate=115200,
-                bytesize=serial_asyncio.serial.EIGHTBITS,
-                parity=serial_asyncio.serial.PARITY_NONE,
-                stopbits=serial_asyncio.serial.STOPBITS_ONE,
-            )
-
-            while not self.protocol.ready:
-                await asyncio.sleep(0.1)
+                while not self.protocol.ready:
+                    await asyncio.sleep(0.1)
 
-            await self.protocol.set_receive_interrupt(self.receive_interrupt)
+                await self.protocol.set_receive_interrupt(self.receive_interrupt)
 
-            for rf_receive_callback in self.rf_receive_callbacks:
-                self.protocol.add_rf_receive_callback(rf_receive_callback)
+                for rf_receive_callback in self.rf_receive_callbacks:
+                    self.protocol.add_rf_receive_callback(rf_receive_callback)
 
-            return True
+                return True
+            except SerialException as ex:
+                logger.error(ex)
 
         return False
 
-    def disconnect(self):
-        if self.transport is not None:
+    def connected(self) -> bool:
+        if self.protocol is None or self.protocol.transport is None:
+            return False
+
+        return True
+
+    def disconnect(self) -> None:
+        if self.connected():
             logger.debug("Disconnecting Homeduino")
-            self.transport.close()
+            self.protocol.transport.close()
+            self.protocol = None
 
     async def ping(self) -> bool:
-        if self.protocol is not None:
-            logger.debug("Pinging Homeduino")
-            message = f"PING {time.time()}"
-            response = await self.protocol.send(message)
-            if response == message:
-                logger.debug("Pinging Homeduino successful")
-                return True
+        if not self.connected():
+            raise DisconnectedError("Homeduino is not connected")
 
-            logger.error("Pinging Homeduino failed")
+        logger.debug("Pinging Homeduino")
+        message = f"PING {time.time()}"
+        response = await self.protocol.send(message)
+        if response == message:
+            logger.debug("Pinging Homeduino successful")
+            return True
 
+        logger.error("Pinging Homeduino failed")
         return False
 
-    def add_rf_receive_callback(self, rf_receive_callback):
-        if self.protocol is not None:
+    def add_rf_receive_callback(self, rf_receive_callback) -> None:
+        self.rf_receive_callbacks.append(rf_receive_callback)
+        if self.connected():
             self.protocol.add_rf_receive_callback(rf_receive_callback)
-        else:
-            self.rf_receive_callbacks.append(rf_receive_callback)
 
     async def rf_send(self, rf_protocol: str, values) -> bool:
-        if self.protocol is not None and self.send_pin is not None:
+        if not self.connected():
+            raise DisconnectedError("Homeduino is not connected")
+
+        if self.send_pin is not None:
             rf_protocol = getattr(sys.modules[controller.__name__], rf_protocol)
             logger.debug(rf_protocol)
 
             packet = f"RF send {self.send_pin} 3 "
 
             for pulse_length in rf_protocol.pulse_lengths:
                 packet += f"{pulse_length} "
@@ -266,13 +297,15 @@
                 packet += "0 "
                 i += 1
 
             packet += rf_protocol.encode(**values)
 
             response = await self.protocol.send(packet)
             return response == "ACK"
+
         return False
 
     async def send(self, command) -> str:
-        if self.protocol is not None:
-            return await self.protocol.send(command)
-        return None
+        if not self.connected():
+            raise DisconnectedError("Homeduino is not connected")
+
+        return await self.protocol.send(command)
```

### Comparing `homeduino-0.0.5.7/homeduino.egg-info/PKG-INFO` & `homeduino-0.0.5.8/homeduino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeduino
-Version: 0.0.5.7
+Version: 0.0.5.8
 Summary: Homeduino library
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/homeduino.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/homeduino.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `homeduino-0.0.5.7/pyproject.toml` & `homeduino-0.0.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "homeduino"
-version = "0.0.5.7"
+version = "0.0.5.8"
 license = {text = "Apache-2.0"}
 authors = [
     { name="Rogier van Staveren" }
 ]
 description = "Homeduino library"
 readme = "README.md"
 requires-python = ">=3.7"
```

