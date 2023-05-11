# Comparing `tmp/sds011lib-0.1.0.tar.gz` & `tmp/sds011lib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sds011lib-0.1.0.tar", max compression
+gzip compressed data, was "sds011lib-0.2.0.tar", max compression
```

## Comparing `sds011lib-0.1.0.tar` & `sds011lib-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-05-04 05:40:14.558027 sds011lib-0.1.0/LICENSE
--rw-r--r--   0        0        0      622 2023-05-04 05:40:14.558027 sds011lib-0.1.0/README.md
--rw-r--r--   0        0        0      863 2023-05-04 05:40:14.558027 sds011lib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    17192 2023-05-04 05:40:14.558027 sds011lib-0.1.0/sds011lib/__init__.py
--rw-r--r--   0        0        0     1505 2023-05-04 05:40:14.558027 sds011lib-0.1.0/sds011lib/constants.py
--rw-r--r--   0        0        0     2332 2023-05-04 05:40:14.558027 sds011lib-0.1.0/sds011lib/exceptions.py
--rw-r--r--   0        0        0     5796 2023-05-04 05:40:14.558027 sds011lib-0.1.0/sds011lib/responses.py
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 sds011lib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-11 03:31:51.862807 sds011lib-0.2.0/LICENSE
+-rw-r--r--   0        0        0      710 2023-05-11 03:31:51.862807 sds011lib-0.2.0/README.md
+-rw-r--r--   0        0        0      955 2023-05-11 03:31:51.866807 sds011lib-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    19852 2023-05-11 03:31:51.866807 sds011lib-0.2.0/sds011lib/__init__.py
+-rw-r--r--   0        0        0     1505 2023-05-11 03:31:51.866807 sds011lib-0.2.0/sds011lib/constants.py
+-rw-r--r--   0        0        0     2332 2023-05-11 03:31:51.866807 sds011lib-0.2.0/sds011lib/exceptions.py
+-rw-r--r--   0        0        0     5797 2023-05-11 03:31:51.866807 sds011lib-0.2.0/sds011lib/responses.py
+-rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 sds011lib-0.2.0/PKG-INFO
```

### Comparing `sds011lib-0.1.0/LICENSE` & `sds011lib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sds011lib-0.1.0/README.md` & `sds011lib-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # sds011lib
 
-`sds011lib` is a fully-typed, nearly-complete, python3 library for interacting with the SDS011 Air Quality Sensor.
+![Main](https://github.com/TimOrme/sds011lib/actions/workflows/main.yml/badge.svg)
+
+`sds011lib` is a fully-typed, nearly-complete, python 3.8+ library for interacting with the SDS011 Air Quality Sensor.
 
 The full documentation is available at https://timorme.github.io/sds011lib/
 
 ## Installation
 
 ```commandline
 pip install sds011lib
```

### Comparing `sds011lib-0.1.0/pyproject.toml` & `sds011lib-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sds011lib"
-version = "0.1.0"
+version = "0.2.0"
 description = "SDS011 Library"
 authors = ["Tim Orme <TimothyOrme@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyserial = "^3.5"
@@ -16,20 +16,25 @@
 mypy = "^1.1.1"
 types-pyserial = "^3.5.0.8"
 myst-parser = "^1.0.0"
 mkdocs = "^1.4.2"
 mkdocs-gitbook = "^0.0.1"
 mkdocs-material = "^9.1.8"
 mkdocstrings = {extras = ["python"], version = "^0.21.2"}
+tox = "^4.5.1"
 
 [tool.ruff]
 select = ["E", "F", "D"]
 ignore = ["D203", "D213"]
 line-length = 120
 
+[tool.ruff.pydocstyle]
+# Use Google-style docstrings.
+convention = "google"
+
 [tool.ruff.per-file-ignores]
 "tests/*" = ["D100", "D101", "D102", "D103", "D104" ]  # We dont need docstrings in tests
 
 [[tool.mypy.overrides]]
 module = "serial.*"
 ignore_missing_imports = true
```

### Comparing `sds011lib-0.1.0/sds011lib/__init__.py` & `sds011lib-0.2.0/sds011lib/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 Device: https://www.amazon.com/SDS011-Quality-Detection-Conditioning-Monitor/dp/B07FSDMRR5
 
 Spec: https://cdn.sparkfun.com/assets/parts/1/2/2/7/5/Laser_Dust_Sensor_Control_Protocol_V1.3.pdf
 Spec: https://cdn-reichelt.de/documents/datenblatt/X200/SDS011-DATASHEET.pdf
 """
 
 import time
+
+import serial
+
 from .responses import (
     QueryResponse,
     ReportingModeResponse,
     SleepWakeReadResponse,
     DeviceIdResponse,
     CheckFirmwareResponse,
     WorkingPeriodReadResponse,
@@ -18,25 +21,26 @@
 from . import constants as con
 from .exceptions import (
     IncompleteReadException,
     IncorrectCommandException,
     IncorrectCommandCodeException,
 )
 
-from typing import Protocol
+from typing import Protocol, Union, Optional, runtime_checkable
 
 
+@runtime_checkable
 class SerialLike(Protocol):
     """A serial-like device."""
 
     def read(self, size: int) -> bytes:
         """Read data from the device."""
         pass
 
-    def write(self, data: bytes) -> int:
+    def write(self, data: bytes) -> Optional[int]:
         """Write data from the device."""
         pass
 
     def open(self) -> None:
         """Open a connection to the device."""
         pass
 
@@ -44,50 +48,55 @@
         """Close a connection to the device."""
         pass
 
 
 class SDS011Reader:
     """NOVA PM SDS011 Reader."""
 
-    def __init__(self, ser_dev: SerialLike, send_command_sleep: int = 1):
+    def __init__(self, ser_dev: Union[str, SerialLike], send_command_sleep: int = 1):
         """Create a basic device.
 
         This is mostly a low level implementation. For practical purposes, most users will want to use the
         SDS011QueryReader or SDS011ActiveReader.  This implementation would only be useful for very special cases, and
         serves as the base class for the other reader implementations anyways.
 
         Args:
-            ser_dev: A serial device.
+            ser_dev: A path to a serial device, or an instance of serial.Serial.
             send_command_sleep: The number of seconds to sleep after sending a command to the device.
         """
-        self.ser = ser_dev
+        if isinstance(ser_dev, str):
+            self.ser: SerialLike = serial.Serial(ser_dev, timeout=2)
+        elif isinstance(ser_dev, SerialLike):
+            self.ser = ser_dev
+        else:
+            raise AttributeError("ser_dev must be a string or Serial-like object.")
         self.send_command_sleep = send_command_sleep
 
-    def request_data(self) -> None:
+    def request_data(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
         """Submit a request to the device to return pollutant data."""
-        cmd = con.Command.QUERY.value + (b"\x00" * 12) + con.ALL_SENSOR_ID
+        cmd = con.Command.QUERY.value + (b"\x00" * 12) + device_id
         self._send_command(cmd)
 
     def query_data(self) -> QueryResponse:
         """Query the device for pollutant data.
 
         Returns:
             Pollutant data from the device.
 
         """
         return QueryResponse(self._read_response())
 
-    def request_reporting_mode(self) -> None:
+    def request_reporting_mode(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
         """Submit a request to the device to return the current reporting mode."""
         cmd = (
             con.Command.SET_REPORTING_MODE.value
             + con.OperationType.QUERY.value
             + con.ReportingMode.ACTIVE.value
             + (b"\x00" * 10)
-            + con.ALL_SENSOR_ID
+            + device_id
         )
         self._send_command(cmd)
 
     def query_reporting_mode(self) -> ReportingModeResponse:
         """Get the current reporting mode of the device.
 
         Returns:
@@ -114,88 +123,94 @@
         except IncorrectCommandException:
             pass
         except IncompleteReadException:
             pass
         except IncorrectCommandCodeException:
             pass
 
-    def _set_reporting_mode(self, reporting_mode: con.ReportingMode) -> None:
+    def _set_reporting_mode(
+        self, reporting_mode: con.ReportingMode, device_id: bytes = con.ALL_SENSOR_ID
+    ) -> None:
         """Set the reporting mode, either ACTIVE or QUERYING.
 
         ACTIVE mode means the device will always return a Query command response when data is asked for, regardless of
         what command was sent.
 
         QUERYING mode means the device will only return responses to submitted commands, even for Query commands.
 
         ACTIVE mode is the factory default, but generally, QUERYING mode is preferrable for the longevity of the device.
 
         Args:
             reporting_mode: The reporting mode to set.
+            device_id: The device ID to set reporting mode on.
         """
         cmd = (
             con.Command.SET_REPORTING_MODE.value
             + con.OperationType.SET_MODE.value
             + reporting_mode.value
             + (b"\x00" * 10)
-            + con.ALL_SENSOR_ID
+            + device_id
         )
         self._send_command(cmd)
         # Switching between reporting modes is finicky; resetting the serial connection seems to address issues.
         self.ser.close()
         self.ser.open()
 
-    def request_sleep_state(self) -> None:
+    def request_sleep_state(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
         """Submit a request to get the current sleep state."""
         cmd = (
             con.Command.SET_SLEEP.value
             + con.OperationType.QUERY.value
             + b"\x00"
             + (b"\x00" * 10)
-            + con.ALL_SENSOR_ID
+            + device_id
         )
         self._send_command(cmd)
 
     def query_sleep_state(self) -> SleepWakeReadResponse:
         """Get the current sleep state.
 
         Returns:
             The current sleep state of the device.
         """
         return SleepWakeReadResponse(self._read_response())
 
-    def set_sleep_state(self, sleep_state: con.SleepState) -> None:
+    def set_sleep_state(
+        self, sleep_state: con.SleepState, device_id: bytes = con.ALL_SENSOR_ID
+    ) -> None:
         """Set the sleep state, either wake or sleep.
 
         Args:
             sleep_state: The sleep state to set, either SleepState.WAKE or SleepState.SLEEP
+            device_id: The device ID to sleep or wake.
         """
         cmd = (
             con.Command.SET_SLEEP.value
             + con.OperationType.SET_MODE.value
             + sleep_state.value
             + (b"\x00" * 10)
-            + con.ALL_SENSOR_ID
+            + device_id
         )
         self._send_command(cmd)
 
-    def sleep(self) -> None:
+    def sleep(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
         """Put the device to sleep, turning off fan and diode."""
-        self.set_sleep_state(con.SleepState.SLEEP)
+        self.set_sleep_state(con.SleepState.SLEEP, device_id)
 
-    def wake(self) -> None:
+    def wake(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
         """Wake the device up to start reading, turning on fan and diode."""
-        self.set_sleep_state(con.SleepState.WAKE)
+        self.set_sleep_state(con.SleepState.WAKE, device_id)
 
-    def safe_wake(self) -> None:
+    def safe_wake(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
         """Wake the device up, if you don't know what mode its in.
 
         This operates as a fire-and-forget, even in query mode.  You shouldn't have to (and can't) query for a response
         after this command.
         """
-        self.wake()
+        self.wake(device_id=device_id)
         # If we were in query mode, this would flush out the response.  If in active mode, this would be return read
         # data, but we don't care.
         self.ser.read(10)
 
     def set_device_id(
         self, device_id: bytes, target_device_id: bytes = con.ALL_SENSOR_ID
     ) -> None:
@@ -223,62 +238,61 @@
 
         Returns:
             The current device ID.
 
         """
         return DeviceIdResponse(self._read_response())
 
-    def request_working_period(self) -> None:
+    def request_working_period(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
         """Submit a request to retrieve the current working period for the device."""
         cmd = (
             con.Command.SET_WORKING_PERIOD.value
             + con.OperationType.QUERY.value
             + (b"\x00" * 11)
-            + con.ALL_SENSOR_ID
+            + device_id
         )
         self._send_command(cmd)
 
     def query_working_period(self) -> WorkingPeriodReadResponse:
         """Retrieve the current working period for the device.
 
         Returns:
             The current working period set for the device.
 
         """
         return WorkingPeriodReadResponse(self._read_response())
 
-    def set_working_period(self, working_period: int) -> None:
+    def set_working_period(
+        self, working_period: int, device_id: bytes = con.ALL_SENSOR_ID
+    ) -> None:
         """Set the working period for the device.
 
         Working period must be between 0 and 30.
 
         0 means the device will read continuously.
         Any value 1-30 means the device will wake and read for 30 seconds every n*60-30 seconds.
 
         Args:
             working_period: A value 0-30 to set as the new working period
+            device_id: The device ID to set the working period for.
         """
         if 0 >= working_period >= 30:
             raise AttributeError("Working period must be between 0 and 30")
         cmd = (
             con.Command.SET_WORKING_PERIOD.value
             + con.OperationType.SET_MODE.value
             + bytes([working_period])
             + (b"\x00" * 10)
-            + con.ALL_SENSOR_ID
+            + device_id
         )
         self._send_command(cmd)
 
-    def request_firmware_version(self) -> None:
+    def request_firmware_version(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
         """Submit a request to retrieve the firmware version from the device."""
-        cmd = (
-            con.Command.CHECK_FIRMWARE_VERSION.value
-            + (b"\x00" * 12)
-            + con.ALL_SENSOR_ID
-        )
+        cmd = con.Command.CHECK_FIRMWARE_VERSION.value + (b"\x00" * 12) + device_id
         self._send_command(cmd)
 
     def query_firmware_version(self) -> CheckFirmwareResponse:
         """Retrieve the firmware version from the device.
 
         Returns:
             The firmware version from the device.
@@ -302,33 +316,33 @@
         full_command = head + cmd + bytes([self._cmd_checksum(cmd)]) + con.TAIL
         if len(full_command) != 19:
             raise Exception(f"Command length must be 19, but was {len(full_command)}")
         self.ser.write(full_command)
         time.sleep(self.send_command_sleep)
 
     def _read_response(self) -> bytes:
-        """
-        Read a response from the device.
+        """Read a response from the device.
+
+        Responses from the device should always be 10 bytes in length.
 
-        Responses from the device should always be 10 bytes in lenght.
         Returns:
             Bytes from the device.
 
         Raises:
             IncompleteReadException: If the number of bytes read is not 10.
 
         """
         result = self.ser.read(10)
         if len(result) != 10:
             raise IncompleteReadException(len(result))
         return result
 
     def _cmd_checksum(self, data: bytes) -> int:
-        """
-        Generate a checksum for the data bytes of a command.
+        """Generate a checksum for the data bytes of a command.
+
         Args:
             data: The data bytes of write command.
 
         Returns:
             An integer checksum of the bytes passed.
 
         """
@@ -336,174 +350,214 @@
             raise AttributeError("Invalid checksum length.")
         return sum(d for d in data) % 256
 
 
 class SDS011QueryReader:
     """Reader working in query mode."""
 
-    def __init__(self, ser_dev: SerialLike, send_command_sleep: int = 1):
+    def __init__(self, ser_dev: Union[str, SerialLike], send_command_sleep: int = 1):
         """Create a reader which operates exclusively in query mode.
 
         Args:
-            ser_dev: A serial device.
+            ser_dev: A path to a serial device, or an instance of serial.Serial.
             send_command_sleep: The number of seconds to sleep after sending a command to the device.
         """
         self.base_reader = SDS011Reader(
             ser_dev=ser_dev, send_command_sleep=send_command_sleep
         )
-        self.base_reader.safe_wake()
+        self.base_reader.safe_wake(device_id=con.ALL_SENSOR_ID)
         self.base_reader.set_query_mode()
 
-    def query(self) -> QueryResponse:
-        """
-        Query the device for pollutant data.
+    def query(self, device_id: bytes = con.ALL_SENSOR_ID) -> QueryResponse:
+        """Query the device for pollutant data.
+
+        Args:
+            device_id: The device ID to get pollutant data for.
 
         Returns:
             The latest pollutant data.
 
         """
-        self.base_reader.request_data()
+        self.base_reader.request_data(device_id=device_id)
         return self.base_reader.query_data()
 
-    def get_reporting_mode(self) -> ReportingModeResponse:
-        """
-        Get the current reporting mode of the device.
+    def get_reporting_mode(
+        self, device_id: bytes = con.ALL_SENSOR_ID
+    ) -> ReportingModeResponse:
+        """Get the current reporting mode of the device.
+
+        Args:
+            device_id: The device ID to get the reporting mode for.
 
         Returns:
             The current reporting mode of the device.
 
         """
-        self.base_reader.request_reporting_mode()
+        self.base_reader.request_reporting_mode(device_id=device_id)
         return self.base_reader.query_reporting_mode()
 
-    def get_sleep_state(self) -> SleepWakeReadResponse:
+    def get_sleep_state(
+        self, device_id: bytes = con.ALL_SENSOR_ID
+    ) -> SleepWakeReadResponse:
         """Get the current sleep state.
 
+        Args:
+            device_id: The device ID to get the sleep state for.
+
         Returns:
             The current sleep state of the device.
         """
-        self.base_reader.request_sleep_state()
+        self.base_reader.request_sleep_state(device_id=device_id)
         return self.base_reader.query_sleep_state()
 
-    def sleep(self) -> SleepWakeReadResponse:
+    def sleep(self, device_id: bytes = con.ALL_SENSOR_ID) -> SleepWakeReadResponse:
         """Put the device to sleep, turning off fan and diode.
 
+        Args:
+            device_id: The device ID to put to sleep.
+
         Returns:
             The new sleep state of the device.
         """
-        self.base_reader.sleep()
+        self.base_reader.sleep(device_id=device_id)
         return self.base_reader.query_sleep_state()
 
-    def wake(self) -> SleepWakeReadResponse:
+    def wake(self, device_id: bytes = con.ALL_SENSOR_ID) -> SleepWakeReadResponse:
         """Wake the device up to start reading, turning on the fan and diode.
 
+        Args:
+            device_id: The device ID to wake up.
+
+
         Returns:
             The new sleep state of the device.
         """
-        self.base_reader.wake()
+        self.base_reader.wake(device_id=device_id)
         return self.base_reader.query_sleep_state()
 
     def set_device_id(
         self, device_id: bytes, target_device_id: bytes = con.ALL_SENSOR_ID
     ) -> DeviceIdResponse:
         """Set the device ID.
 
         Args:
             device_id: The new, 4-byte device ID to set.
             target_device_id: The target device ID.
 
         Returns:
             A response with the new device ID.
         """
-        self.base_reader.set_device_id(device_id, target_device_id)
+        self.base_reader.set_device_id(
+            device_id=device_id, target_device_id=target_device_id
+        )
         return self.base_reader.query_device_id()
 
-    def get_working_period(self) -> WorkingPeriodReadResponse:
-        """
-        Retrieve the current working period for the device.
+    def get_working_period(
+        self, device_id: bytes = con.ALL_SENSOR_ID
+    ) -> WorkingPeriodReadResponse:
+        """Retrieve the current working period for the device.
+
+        Args:
+            device_id: The device ID to get the working period for.
 
         Returns:
             A response with the current working period.
         """
-        self.base_reader.request_working_period()
+        self.base_reader.request_working_period(device_id=device_id)
         return self.base_reader.query_working_period()
 
-    def set_working_period(self, working_period: int) -> WorkingPeriodReadResponse:
-        """
-        Set the working period for the device.
+    def set_working_period(
+        self, working_period: int, device_id: bytes = con.ALL_SENSOR_ID
+    ) -> WorkingPeriodReadResponse:
+        """Set the working period for the device.
 
         Working period must be between 0 and 30.
 
         0 means the device will read continuously.
         Any value 1-30 means the device will wake and read for 30 seconds every n*60-30 seconds.
 
         Args:
             working_period: A value 0-30 to set as the new working period
+            device_id: The device ID to set the working period for.
 
         Returns:
             A response with the new working period
 
         """
-        self.base_reader.set_working_period(working_period)
+        self.base_reader.set_working_period(
+            working_period=working_period, device_id=device_id
+        )
         return self.base_reader.query_working_period()
 
-    def get_firmware_version(self) -> CheckFirmwareResponse:
+    def get_firmware_version(
+        self, device_id: bytes = con.ALL_SENSOR_ID
+    ) -> CheckFirmwareResponse:
         """Retrieve the firmware version from the device.
 
+        Args:
+            device_id: The device ID to retrieve firmware version for.
+
         Returns:
             The firmware version of the device
 
         """
-        self.base_reader.request_firmware_version()
+        self.base_reader.request_firmware_version(device_id=device_id)
         return self.base_reader.query_firmware_version()
 
 
 class SDS011ActiveReader:
     """Active Mode Reader.
 
     Use with caution! Active mode is unpredictable.  Query mode is much preferred.
     """
 
-    def __init__(self, ser_dev: SerialLike, send_command_sleep: int = 2):
+    def __init__(self, ser_dev: Union[str, SerialLike], send_command_sleep: int = 2):
         """Create a reader which operates exclusively in active mode.
 
         Args:
-            ser_dev: A serial device.
+            ser_dev: A path to a serial device, or an instance of serial.Serial.
             send_command_sleep: The number of seconds to sleep after sending a command to the device.
         """
         self.base_reader = SDS011Reader(
             ser_dev=ser_dev, send_command_sleep=send_command_sleep
         )
-        self.ser_dev = ser_dev
+        self.ser_dev: SerialLike = self.base_reader.ser
         self.base_reader.safe_wake()
         self.base_reader.set_active_mode()
 
     def query(self) -> QueryResponse:
-        """
-        Query the device for pollutant data.
+        """Query the device for pollutant data.
 
         Returns:
             The latest pollutant data.
 
         """
         return self.base_reader.query_data()
 
-    def sleep(self) -> None:
-        """Put the device to sleep, turning off fan and diode."""
-        self.base_reader.sleep()
+    def sleep(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
+        """Put the device to sleep, turning off fan and diode.
+
+        Args:
+            device_id: The device ID to put to sleep.
+        """
+        self.base_reader.sleep(device_id)
 
         # Sleep seems to behave very strangely in active mode.  It continually outputs data for old commands for quite
         # a while before eventually having nothing to report.  This forces it to "drain" whatever it was doing before
         # returning, but also feels quite dangerous.
         while len(self.ser_dev.read(10)) == 10:
             pass
 
-    def wake(self) -> None:
-        """Wake the device up to start reading, turning on the fan and diode."""
-        self.base_reader.wake()
+    def wake(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
+        """Wake the device up to start reading, turning on the fan and diode.
+
+        Args:
+            device_id: The device ID to wake up.
+        """
+        self.base_reader.wake(device_id)
         self.ser_dev.read(10)
 
     def set_device_id(
         self, device_id: bytes, target_device_id: bytes = con.ALL_SENSOR_ID
     ) -> None:
         """Set the device ID.
 
@@ -513,24 +567,26 @@
 
         Returns:
             A response with the new device ID.
         """
         self.base_reader.set_device_id(device_id, target_device_id)
         self.ser_dev.read(10)
 
-    def set_working_period(self, working_period: int) -> None:
-        """
-        Set the working period for the device.
+    def set_working_period(
+        self, working_period: int, device_id: bytes = con.ALL_SENSOR_ID
+    ) -> None:
+        """Set the working period for the device.
 
         Working period must be between 0 and 30.
 
         0 means the device will read continuously.
         Any value 1-30 means the device will wake and read for 30 seconds every n*60-30 seconds.
 
         Args:
             working_period: A value 0-30 to set as the new working period
+            device_id: The device ID to set the working period for.
 
         Returns:
             A response with the new working period
         """
-        self.base_reader.set_working_period(working_period)
+        self.base_reader.set_working_period(working_period, device_id)
         self.ser_dev.read(10)
```

### Comparing `sds011lib-0.1.0/sds011lib/constants.py` & `sds011lib-0.2.0/sds011lib/constants.py`

 * *Files identical despite different names*

### Comparing `sds011lib-0.1.0/sds011lib/exceptions.py` & `sds011lib-0.2.0/sds011lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `sds011lib-0.1.0/sds011lib/responses.py` & `sds011lib-0.2.0/sds011lib/responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
     def __init__(self, data: bytes):
         """Create a device ID response."""
         super().__init__(data, command_code=Command.SET_DEVICE_ID)
 
 
 class SleepWakeReadResponse(ReadResponse):
     """Sleep/Wake Response.
+
     Attributes:
         operation_type: The operation type the response is for, either QUERY or SET_MODE.
         state: The current sleep state, either WAKE or SLEEP.
 
     """
 
     def __init__(self, data: bytes):
```

### Comparing `sds011lib-0.1.0/PKG-INFO` & `sds011lib-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: sds011lib
-Version: 0.1.0
+Version: 0.2.0
 Summary: SDS011 Library
 Author: Tim Orme
 Author-email: TimothyOrme@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyserial (>=3.5,<4.0)
 Description-Content-Type: text/markdown
 
 # sds011lib
 
-`sds011lib` is a fully-typed, nearly-complete, python3 library for interacting with the SDS011 Air Quality Sensor.
+![Main](https://github.com/TimOrme/sds011lib/actions/workflows/main.yml/badge.svg)
+
+`sds011lib` is a fully-typed, nearly-complete, python 3.8+ library for interacting with the SDS011 Air Quality Sensor.
 
 The full documentation is available at https://timorme.github.io/sds011lib/
 
 ## Installation
 
 ```commandline
 pip install sds011lib
```

