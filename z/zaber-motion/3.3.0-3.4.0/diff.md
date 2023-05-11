# Comparing `tmp/zaber_motion-3.3.0.tar.gz` & `tmp/zaber_motion-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zaber_motion-3.3.0.tar", last modified: Fri Apr 28 18:32:16 2023, max compression
+gzip compressed data, was "zaber_motion-3.4.0.tar", last modified: Thu May 11 19:08:40 2023, max compression
```

## Comparing `zaber_motion-3.3.0.tar` & `zaber_motion-3.4.0.tar`

### file list

```diff
@@ -1,171 +1,187 @@
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.371494 zaber_motion-3.3.0/
--rw-r--r--   0 zaber      (501) staff       (20)      218 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/DESCRIPTION.md
--rw-r--r--   0 zaber      (501) staff       (20)   109244 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/LICENSE.txt
--rw-r--r--   0 zaber      (501) staff       (20)       13 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/MANIFEST.in
--rw-r--r--   0 zaber      (501) staff       (20)      808 2023-04-28 18:32:16.371584 zaber_motion-3.3.0/PKG-INFO
--rw-r--r--   0 zaber      (501) staff       (20)      218 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/README.md
--rw-r--r--   0 zaber      (501) staff       (20)      134 2023-04-28 18:32:16.371935 zaber_motion-3.3.0/setup.cfg
--rw-r--r--   0 zaber      (501) staff       (20)     1371 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/setup.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.331669 zaber_motion-3.3.0/test/
--rw-r--r--   0 zaber      (501) staff       (20)     3544 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/test/test_integration.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.335566 zaber_motion-3.3.0/zaber_motion/
--rw-r--r--   0 zaber      (501) staff       (20)     5735 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/__init__.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.348326 zaber_motion-3.3.0/zaber_motion/ascii/
--rw-r--r--   0 zaber      (501) staff       (20)     2337 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     2185 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/alert_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     8708 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/all_axes.py
--rw-r--r--   0 zaber      (501) staff       (20)    40795 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/axis.py
--rw-r--r--   0 zaber      (501) staff       (20)     2259 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/axis_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)    12689 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/axis_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      272 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     1265 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/can_set_state_axis_response.py
--rw-r--r--   0 zaber      (501) staff       (20)     1530 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/can_set_state_device_response.py
--rw-r--r--   0 zaber      (501) staff       (20)    36081 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/connection.py
--rw-r--r--   0 zaber      (501) staff       (20)     1887 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/conversion_factor.py
--rw-r--r--   0 zaber      (501) staff       (20)    23731 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/device.py
--rw-r--r--   0 zaber      (501) staff       (20)     2801 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/device_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)    17751 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/device_io.py
--rw-r--r--   0 zaber      (501) staff       (20)     2077 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/device_io_info.py
--rw-r--r--   0 zaber      (501) staff       (20)    10347 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/device_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)    36231 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/lockstep.py
--rw-r--r--   0 zaber      (501) staff       (20)     1671 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/lockstep_axes.py
--rw-r--r--   0 zaber      (501) staff       (20)      386 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/message_type.py
--rw-r--r--   0 zaber      (501) staff       (20)    15804 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/oscilloscope.py
--rw-r--r--   0 zaber      (501) staff       (20)     1303 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/oscilloscope_capture_properties.py
--rw-r--r--   0 zaber      (501) staff       (20)     4860 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/oscilloscope_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1601 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/paramset_info.py
--rw-r--r--   0 zaber      (501) staff       (20)     2078 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/pid_tuning.py
--rw-r--r--   0 zaber      (501) staff       (20)     2896 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/response.py
--rw-r--r--   0 zaber      (501) staff       (20)    19220 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/servo_tuner.py
--rw-r--r--   0 zaber      (501) staff       (20)     1801 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/servo_tuning_param.py
--rw-r--r--   0 zaber      (501) staff       (20)      384 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/servo_tuning_paramset.py
--rw-r--r--   0 zaber      (501) staff       (20)    22658 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/setting_constants.py
--rw-r--r--   0 zaber      (501) staff       (20)     1893 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/simple_tuning_param_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)    26082 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/storage.py
--rw-r--r--   0 zaber      (501) staff       (20)    74838 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/stream.py
--rw-r--r--   0 zaber      (501) staff       (20)     2133 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/stream_axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)      253 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/stream_axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3080 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/stream_buffer.py
--rw-r--r--   0 zaber      (501) staff       (20)      273 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/stream_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     5345 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/transport.py
--rw-r--r--   0 zaber      (501) staff       (20)     2966 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/unknown_response_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     2855 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/warning_flags.py
--rw-r--r--   0 zaber      (501) staff       (20)     5066 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/ascii/warnings.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.351203 zaber_motion-3.3.0/zaber_motion/binary/
--rw-r--r--   0 zaber      (501) staff       (20)      653 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     1941 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/binary_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)     3132 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/command_code.py
--rw-r--r--   0 zaber      (501) staff       (20)    19348 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/connection.py
--rw-r--r--   0 zaber      (501) staff       (20)    28560 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/device.py
--rw-r--r--   0 zaber      (501) staff       (20)     3361 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/device_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)     3346 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/device_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      276 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/device_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3116 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/error_code.py
--rw-r--r--   0 zaber      (501) staff       (20)     1498 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/message.py
--rw-r--r--   0 zaber      (501) staff       (20)      415 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/reply_code.py
--rw-r--r--   0 zaber      (501) staff       (20)     1552 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/reply_only_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     1588 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/binary/unknown_response_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     1153 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/bindings.py
--rw-r--r--   0 zaber      (501) staff       (20)     4196 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/call.py
--rw-r--r--   0 zaber      (501) staff       (20)     6453 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/convert_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      257 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/device_db_source_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     2200 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/events.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.367318 zaber_motion-3.3.0/zaber_motion/exceptions/
--rw-r--r--   0 zaber      (501) staff       (20)     6320 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     1121 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/binary_command_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      991 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/binary_command_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1045 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/command_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1840 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/command_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/command_preempted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1129 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/command_too_long_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1971 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/command_too_long_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      304 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/connection_closed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/connection_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/conversion_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1158 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/device_address_conflict_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1126 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/device_address_conflict_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      314 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/device_busy_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1092 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/device_db_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      911 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/device_db_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      283 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/device_detection_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      335 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/device_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      317 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/device_not_identified_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1065 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/g_code_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1321 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/g_code_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1036 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/g_code_syntax_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1300 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/g_code_syntax_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      309 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/internal_error_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      295 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/invalid_argument_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      300 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/invalid_data_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      310 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/invalid_operation_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1058 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/invalid_packet_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1198 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/invalid_packet_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      282 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/invalid_park_state_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1091 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/invalid_response_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      928 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/invalid_response_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      342 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/io_channel_out_of_range_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      297 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/io_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      322 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/lockstep_enabled_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      329 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/lockstep_not_enabled_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      396 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/motion_lib_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1070 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1852 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1137 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1875 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/no_device_found_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      297 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/no_value_for_key_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/not_supported_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/os_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      317 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/out_of_request_ids_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      300 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/request_timeout_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      349 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/serial_port_busy_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     3228 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/set_device_state_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1085 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/set_device_state_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     2372 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/set_peripheral_state_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1120 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/setting_not_found_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1060 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/stream_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1232 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/stream_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      323 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/stream_mode_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1134 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/stream_movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1313 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/stream_movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1199 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/stream_movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1348 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      282 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/stream_setup_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      341 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/timeout_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      320 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/transport_already_used_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      335 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/exceptions/unknown_request_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     2106 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/firmware_version.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.369428 zaber_motion-3.3.0/zaber_motion/gcode/
--rw-r--r--   0 zaber      (501) staff       (20)      578 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     2269 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)     1571 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/axis_mapping.py
--rw-r--r--   0 zaber      (501) staff       (20)     2170 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/axis_transformation.py
--rw-r--r--   0 zaber      (501) staff       (20)     2313 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/device_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)    12275 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/offline_translator.py
--rw-r--r--   0 zaber      (501) staff       (20)     1555 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/translate_message.py
--rw-r--r--   0 zaber      (501) staff       (20)     1401 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/translate_result.py
--rw-r--r--   0 zaber      (501) staff       (20)    12899 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/translator.py
--rw-r--r--   0 zaber      (501) staff       (20)     2225 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/gcode/translator_config.py
--rw-r--r--   0 zaber      (501) staff       (20)     2838 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/library.py
--rw-r--r--   0 zaber      (501) staff       (20)      279 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/log_output_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     1519 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/measurement.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.369862 zaber_motion-3.3.0/zaber_motion/microscopy/
--rw-r--r--   0 zaber      (501) staff       (20)       68 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/microscopy/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     6181 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/microscopy/objective_changer.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.370685 zaber_motion-3.3.0/zaber_motion/protobufs/
--rw-r--r--   0 zaber      (501) staff       (20)        0 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/protobufs/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)    62415 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/protobufs/main_pb2.py
--rw-r--r--   0 zaber      (501) staff       (20)   190301 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/protobufs/main_pb2.pyi
--rw-r--r--   0 zaber      (501) staff       (20)        0 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/py.typed
--rw-r--r--   0 zaber      (501) staff       (20)      278 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/rotation_direction.py
--rw-r--r--   0 zaber      (501) staff       (20)      987 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/serialization.py
--rw-r--r--   0 zaber      (501) staff       (20)     2108 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/tools.py
--rw-r--r--   0 zaber      (501) staff       (20)     5744 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/units.py
--rw-r--r--   0 zaber      (501) staff       (20)       22 2023-04-28 18:31:26.000000 zaber_motion-3.3.0/zaber_motion/version.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-04-28 18:32:16.336507 zaber_motion-3.3.0/zaber_motion.egg-info/
--rw-r--r--   0 zaber      (501) staff       (20)      808 2023-04-28 18:32:16.000000 zaber_motion-3.3.0/zaber_motion.egg-info/PKG-INFO
--rw-r--r--   0 zaber      (501) staff       (20)     6798 2023-04-28 18:32:16.000000 zaber_motion-3.3.0/zaber_motion.egg-info/SOURCES.txt
--rw-r--r--   0 zaber      (501) staff       (20)        1 2023-04-28 18:32:16.000000 zaber_motion-3.3.0/zaber_motion.egg-info/dependency_links.txt
--rw-r--r--   0 zaber      (501) staff       (20)      239 2023-04-28 18:32:16.000000 zaber_motion-3.3.0/zaber_motion.egg-info/requires.txt
--rw-r--r--   0 zaber      (501) staff       (20)       13 2023-04-28 18:32:16.000000 zaber_motion-3.3.0/zaber_motion.egg-info/top_level.txt
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-11 19:08:40.429664 zaber_motion-3.4.0/
+-rw-r--r--   0 zaber      (501) staff       (20)      218 2023-05-11 19:07:57.000000 zaber_motion-3.4.0/DESCRIPTION.md
+-rw-r--r--   0 zaber      (501) staff       (20)   109244 2023-05-11 19:07:57.000000 zaber_motion-3.4.0/LICENSE.txt
+-rw-r--r--   0 zaber      (501) staff       (20)       13 2023-05-11 19:07:57.000000 zaber_motion-3.4.0/MANIFEST.in
+-rw-r--r--   0 zaber      (501) staff       (20)      808 2023-05-11 19:08:40.429723 zaber_motion-3.4.0/PKG-INFO
+-rw-r--r--   0 zaber      (501) staff       (20)      218 2023-05-11 19:07:57.000000 zaber_motion-3.4.0/README.md
+-rw-r--r--   0 zaber      (501) staff       (20)      134 2023-05-11 19:08:40.429959 zaber_motion-3.4.0/setup.cfg
+-rw-r--r--   0 zaber      (501) staff       (20)     1371 2023-05-11 19:07:57.000000 zaber_motion-3.4.0/setup.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-11 19:08:40.409658 zaber_motion-3.4.0/test/
+-rw-r--r--   0 zaber      (501) staff       (20)     3544 2023-05-11 19:07:57.000000 zaber_motion-3.4.0/test/test_integration.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-11 19:08:40.411473 zaber_motion-3.4.0/zaber_motion/
+-rw-r--r--   0 zaber      (501) staff       (20)     6545 2023-05-11 19:07:57.000000 zaber_motion-3.4.0/zaber_motion/__init__.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-11 19:08:40.417615 zaber_motion-3.4.0/zaber_motion/ascii/
+-rw-r--r--   0 zaber      (501) staff       (20)     2604 2023-05-11 19:07:57.000000 zaber_motion-3.4.0/zaber_motion/ascii/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2185 2023-05-11 19:07:57.000000 zaber_motion-3.4.0/zaber_motion/ascii/alert_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     8708 2023-05-11 19:07:57.000000 zaber_motion-3.4.0/zaber_motion/ascii/all_axes.py
+-rw-r--r--   0 zaber      (501) staff       (20)    40795 2023-05-11 19:07:57.000000 zaber_motion-3.4.0/zaber_motion/ascii/axis.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2259 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/axis_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12689 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/axis_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      272 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1265 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/can_set_state_axis_response.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1530 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/can_set_state_device_response.py
+-rw-r--r--   0 zaber      (501) staff       (20)    36081 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/connection.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1887 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/conversion_factor.py
+-rw-r--r--   0 zaber      (501) staff       (20)    24838 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/device.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2801 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/device_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)    17751 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/device_io.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2077 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/device_io_info.py
+-rw-r--r--   0 zaber      (501) staff       (20)    10347 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/device_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)    36231 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/lockstep.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1671 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/lockstep_axes.py
+-rw-r--r--   0 zaber      (501) staff       (20)      386 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/message_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)    15804 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/oscilloscope.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1303 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/oscilloscope_capture_properties.py
+-rw-r--r--   0 zaber      (501) staff       (20)     4860 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/oscilloscope_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1601 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/paramset_info.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2078 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/pid_tuning.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2094 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/pvt_axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)      256 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/pvt_axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3190 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/pvt_buffer.py
+-rw-r--r--   0 zaber      (501) staff       (20)      247 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/pvt_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)    32301 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/pvt_sequence.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2896 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/response.py
+-rw-r--r--   0 zaber      (501) staff       (20)    19220 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/servo_tuner.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1801 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/servo_tuning_param.py
+-rw-r--r--   0 zaber      (501) staff       (20)      384 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/servo_tuning_paramset.py
+-rw-r--r--   0 zaber      (501) staff       (20)    22658 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/setting_constants.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1893 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/simple_tuning_param_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)    26082 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/storage.py
+-rw-r--r--   0 zaber      (501) staff       (20)    75822 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/stream.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2133 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/stream_axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)      253 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/stream_axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3084 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/stream_buffer.py
+-rw-r--r--   0 zaber      (501) staff       (20)      273 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/stream_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5345 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/transport.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2966 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/unknown_response_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2855 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/warning_flags.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5066 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/ascii/warnings.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-11 19:08:40.419127 zaber_motion-3.4.0/zaber_motion/binary/
+-rw-r--r--   0 zaber      (501) staff       (20)      653 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/binary/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1941 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/binary/binary_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3132 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/binary/command_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)    19348 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/binary/connection.py
+-rw-r--r--   0 zaber      (501) staff       (20)    28560 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/binary/device.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3361 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/binary/device_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3346 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/binary/device_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      276 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/binary/device_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3116 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/binary/error_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1498 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/binary/message.py
+-rw-r--r--   0 zaber      (501) staff       (20)      415 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/binary/reply_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1552 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/binary/reply_only_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1588 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/binary/unknown_response_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1153 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/bindings.py
+-rw-r--r--   0 zaber      (501) staff       (20)     4196 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/call.py
+-rw-r--r--   0 zaber      (501) staff       (20)     7349 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/convert_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      257 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/device_db_source_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2200 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/events.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-11 19:08:40.427722 zaber_motion-3.4.0/zaber_motion/exceptions/
+-rw-r--r--   0 zaber      (501) staff       (20)     7384 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1121 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/binary_command_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      991 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/binary_command_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1045 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/command_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1840 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/command_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/command_preempted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1129 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/command_too_long_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1971 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/command_too_long_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      304 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/connection_closed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/connection_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/conversion_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1158 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/device_address_conflict_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1126 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/device_address_conflict_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      314 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/device_busy_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1092 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/device_db_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      911 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/device_db_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      283 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/device_detection_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      335 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/device_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      317 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/device_not_identified_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1065 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/g_code_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1321 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/g_code_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1036 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/g_code_syntax_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1300 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/g_code_syntax_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      309 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/internal_error_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      295 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/invalid_argument_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      300 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/invalid_data_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      310 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/invalid_operation_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1058 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/invalid_packet_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1198 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/invalid_packet_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      282 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/invalid_park_state_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1140 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/invalid_pvt_point.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1091 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/invalid_response_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      928 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/invalid_response_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      342 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/io_channel_out_of_range_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      297 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/io_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      322 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/lockstep_enabled_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      329 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/lockstep_not_enabled_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      396 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/motion_lib_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1070 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1852 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1137 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1875 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/no_device_found_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      297 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/no_value_for_key_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/not_supported_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/os_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      317 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/out_of_request_ids_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      323 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/pvt_discontinuity_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1037 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/pvt_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1749 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/pvt_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      326 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/pvt_mode_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1102 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/pvt_movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1292 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/pvt_movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1169 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/pvt_movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1327 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      285 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/pvt_setup_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      300 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/request_timeout_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      349 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/serial_port_busy_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3228 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/set_device_state_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1085 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/set_device_state_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2372 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/set_peripheral_state_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1120 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/setting_not_found_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      320 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/stream_discontinuity_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1060 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/stream_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1232 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/stream_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      323 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/stream_mode_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1134 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/stream_movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1313 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/stream_movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1199 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/stream_movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1348 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      282 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/stream_setup_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      341 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/timeout_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      320 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/transport_already_used_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      335 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/exceptions/unknown_request_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2106 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/firmware_version.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-11 19:08:40.428838 zaber_motion-3.4.0/zaber_motion/gcode/
+-rw-r--r--   0 zaber      (501) staff       (20)      578 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/gcode/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2269 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/gcode/axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1571 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/gcode/axis_mapping.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2170 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/gcode/axis_transformation.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2313 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/gcode/device_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12275 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/gcode/offline_translator.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1555 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/gcode/translate_message.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1401 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/gcode/translate_result.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12899 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/gcode/translator.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2225 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/gcode/translator_config.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2838 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/library.py
+-rw-r--r--   0 zaber      (501) staff       (20)      279 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/log_output_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1519 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/measurement.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-11 19:08:40.429071 zaber_motion-3.4.0/zaber_motion/microscopy/
+-rw-r--r--   0 zaber      (501) staff       (20)       68 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/microscopy/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     6181 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/microscopy/objective_changer.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-11 19:08:40.429441 zaber_motion-3.4.0/zaber_motion/protobufs/
+-rw-r--r--   0 zaber      (501) staff       (20)        0 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/protobufs/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)    65620 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/protobufs/main_pb2.py
+-rw-r--r--   0 zaber      (501) staff       (20)   200026 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/protobufs/main_pb2.pyi
+-rw-r--r--   0 zaber      (501) staff       (20)        0 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/py.typed
+-rw-r--r--   0 zaber      (501) staff       (20)      278 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/rotation_direction.py
+-rw-r--r--   0 zaber      (501) staff       (20)      987 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/serialization.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2108 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/tools.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5744 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/units.py
+-rw-r--r--   0 zaber      (501) staff       (20)       22 2023-05-11 19:07:58.000000 zaber_motion-3.4.0/zaber_motion/version.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-11 19:08:40.412028 zaber_motion-3.4.0/zaber_motion.egg-info/
+-rw-r--r--   0 zaber      (501) staff       (20)      808 2023-05-11 19:08:40.000000 zaber_motion-3.4.0/zaber_motion.egg-info/PKG-INFO
+-rw-r--r--   0 zaber      (501) staff       (20)     7588 2023-05-11 19:08:40.000000 zaber_motion-3.4.0/zaber_motion.egg-info/SOURCES.txt
+-rw-r--r--   0 zaber      (501) staff       (20)        1 2023-05-11 19:08:40.000000 zaber_motion-3.4.0/zaber_motion.egg-info/dependency_links.txt
+-rw-r--r--   0 zaber      (501) staff       (20)      239 2023-05-11 19:08:40.000000 zaber_motion-3.4.0/zaber_motion.egg-info/requires.txt
+-rw-r--r--   0 zaber      (501) staff       (20)       13 2023-05-11 19:08:40.000000 zaber_motion-3.4.0/zaber_motion.egg-info/top_level.txt
```

### Comparing `zaber_motion-3.3.0/LICENSE.txt` & `zaber_motion-3.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/PKG-INFO` & `zaber_motion-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaber_motion
-Version: 3.3.0
+Version: 3.4.0
 Summary: A library for communicating with Zaber devices
 Home-page: https://gitlab.com/ZaberTech/zaber-motion-lib
 Author: Zaber Technologies Inc.
 Author-email: contact@zaber.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `zaber_motion-3.3.0/setup.py` & `zaber_motion-3.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read_from_file(*filename):
     with open(path.join(*filename), 'r') as f:
         return f.read()
 
 
 setup(
     name='zaber_motion',
-    version='3.3.0',
+    version='3.4.0',
     packages=find_packages(exclude=["test*", "test_*", "*_test*"]),
     package_data={
         '': ['*.pyi', 'py.typed']
     },
     description='A library for communicating with Zaber devices',
     long_description=read_from_file('DESCRIPTION.md'),
     long_description_content_type="text/markdown",
@@ -32,12 +32,12 @@
         'License :: OSI Approved :: MIT License',
     ],
     keywords='',
     python_requires='>=3.7',
     install_requires=[
         'protobuf>=3.20.0,<4.22.0',
         'rx>=3.0.0',
-        'zaber_motion_bindings_windows==3.3.0;platform_system=="Windows"',
-        'zaber_motion_bindings_linux==3.3.0;platform_system=="Linux"',
-        'zaber_motion_bindings_darwin==3.3.0;platform_system=="Darwin"',
+        'zaber_motion_bindings_windows==3.4.0;platform_system=="Windows"',
+        'zaber_motion_bindings_linux==3.4.0;platform_system=="Linux"',
+        'zaber_motion_bindings_darwin==3.4.0;platform_system=="Darwin"',
     ],
 )
```

### Comparing `zaber_motion-3.3.0/test/test_integration.py` & `zaber_motion-3.4.0/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/__init__.py` & `zaber_motion-3.4.0/zaber_motion/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,19 +43,26 @@
 from .exceptions import MovementFailedException as MovementFailedException
 from .exceptions import MovementInterruptedException as MovementInterruptedException
 from .exceptions import NoDeviceFoundException as NoDeviceFoundException
 from .exceptions import NoValueForKeyException as NoValueForKeyException
 from .exceptions import NotSupportedException as NotSupportedException
 from .exceptions import OsFailedException as OsFailedException
 from .exceptions import OutOfRequestIdsException as OutOfRequestIdsException
+from .exceptions import PvtDiscontinuityException as PvtDiscontinuityException
+from .exceptions import PvtExecutionException as PvtExecutionException
+from .exceptions import PvtModeException as PvtModeException
+from .exceptions import PvtMovementFailedException as PvtMovementFailedException
+from .exceptions import PvtMovementInterruptedException as PvtMovementInterruptedException
+from .exceptions import PvtSetupFailedException as PvtSetupFailedException
 from .exceptions import RequestTimeoutException as RequestTimeoutException
 from .exceptions import SerialPortBusyException as SerialPortBusyException
 from .exceptions import SetDeviceStateFailedException as SetDeviceStateFailedException
 from .exceptions import SetPeripheralStateFailedException as SetPeripheralStateFailedException
 from .exceptions import SettingNotFoundException as SettingNotFoundException
+from .exceptions import StreamDiscontinuityException as StreamDiscontinuityException
 from .exceptions import StreamExecutionException as StreamExecutionException
 from .exceptions import StreamModeException as StreamModeException
 from .exceptions import StreamMovementFailedException as StreamMovementFailedException
 from .exceptions import StreamMovementInterruptedException as StreamMovementInterruptedException
 from .exceptions import StreamSetupFailedException as StreamSetupFailedException
 from .exceptions import TimeoutException as TimeoutException
 from .exceptions import TransportAlreadyUsedException as TransportAlreadyUsedException
@@ -67,12 +74,15 @@
 from .exceptions import DeviceDbFailedExceptionData as DeviceDbFailedExceptionData
 from .exceptions import GCodeExecutionExceptionData as GCodeExecutionExceptionData
 from .exceptions import GCodeSyntaxExceptionData as GCodeSyntaxExceptionData
 from .exceptions import InvalidPacketExceptionData as InvalidPacketExceptionData
 from .exceptions import InvalidResponseExceptionData as InvalidResponseExceptionData
 from .exceptions import MovementFailedExceptionData as MovementFailedExceptionData
 from .exceptions import MovementInterruptedExceptionData as MovementInterruptedExceptionData
+from .exceptions import PvtExecutionExceptionData as PvtExecutionExceptionData
+from .exceptions import PvtMovementFailedExceptionData as PvtMovementFailedExceptionData
+from .exceptions import PvtMovementInterruptedExceptionData as PvtMovementInterruptedExceptionData
 from .exceptions import SetDeviceStateExceptionData as SetDeviceStateExceptionData
 from .exceptions import SetPeripheralStateExceptionData as SetPeripheralStateExceptionData
 from .exceptions import StreamExecutionExceptionData as StreamExecutionExceptionData
 from .exceptions import StreamMovementFailedExceptionData as StreamMovementFailedExceptionData
 from .exceptions import StreamMovementInterruptedExceptionData as StreamMovementInterruptedExceptionData
```

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/__init__.py` & `zaber_motion-3.4.0/zaber_motion/ascii/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,7 +33,12 @@
 from .pid_tuning import PidTuning as PidTuning
 from .servo_tuning_param import ServoTuningParam as ServoTuningParam
 from .simple_tuning_param_definition import SimpleTuningParamDefinition as SimpleTuningParamDefinition
 from .storage import AxisStorage as AxisStorage, DeviceStorage as DeviceStorage
 from .conversion_factor import ConversionFactor as ConversionFactor
 from .can_set_state_axis_response import CanSetStateAxisResponse as CanSetStateAxisResponse
 from .can_set_state_device_response import CanSetStateDeviceResponse as CanSetStateDeviceResponse
+from .pvt_sequence import PvtSequence as PvtSequence
+from .pvt_buffer import PvtBuffer as PvtBuffer
+from .pvt_mode import PvtMode as PvtMode
+from .pvt_axis_type import PvtAxisType as PvtAxisType
+from .pvt_axis_definition import PvtAxisDefinition as PvtAxisDefinition
```

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/alert_event.py` & `zaber_motion-3.4.0/zaber_motion/ascii/alert_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/all_axes.py` & `zaber_motion-3.4.0/zaber_motion/ascii/all_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/axis.py` & `zaber_motion-3.4.0/zaber_motion/ascii/axis.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/axis_identity.py` & `zaber_motion-3.4.0/zaber_motion/ascii/axis_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/axis_settings.py` & `zaber_motion-3.4.0/zaber_motion/ascii/axis_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/can_set_state_axis_response.py` & `zaber_motion-3.4.0/zaber_motion/ascii/can_set_state_axis_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/can_set_state_device_response.py` & `zaber_motion-3.4.0/zaber_motion/ascii/can_set_state_device_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/connection.py` & `zaber_motion-3.4.0/zaber_motion/ascii/connection.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/conversion_factor.py` & `zaber_motion-3.4.0/zaber_motion/ascii/conversion_factor.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/device.py` & `zaber_motion-3.4.0/zaber_motion/ascii/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from .response import Response
 from .lockstep import Lockstep
 from .oscilloscope import Oscilloscope
 from .storage import DeviceStorage
 from .stream import Stream
 from .stream_buffer import StreamBuffer
 from .can_set_state_device_response import CanSetStateDeviceResponse
+from .pvt_sequence import PvtSequence
+from .pvt_buffer import PvtBuffer
 from ..firmware_version import FirmwareVersion
 from ..measurement import Measurement
 
 if TYPE_CHECKING:
     from .connection import Connection
 
 
@@ -489,14 +491,50 @@
             StreamBuffer instance.
         """
         if stream_buffer_id <= 0:
             raise ValueError('Invalid value; stream buffers are numbered from 1.')
 
         return StreamBuffer(self, stream_buffer_id)
 
+    def get_pvt(
+            self,
+            pvt_id: int
+    ) -> PvtSequence:
+        """
+        Gets a PvtSequence class instance which allows you to control a particular PVT sequence on the device.
+
+        Args:
+            pvt_id: The ID of the PVT sequence to control. The IDs start at 1.
+
+        Returns:
+            PvtSequence instance.
+        """
+        if pvt_id <= 0:
+            raise ValueError('Invalid value; PVT sequences are numbered from 1.')
+
+        return PvtSequence(self, pvt_id)
+
+    def get_pvt_buffer(
+            self,
+            pvt_buffer_id: int
+    ) -> PvtBuffer:
+        """
+        Gets a PvtBuffer class instance which is a handle for a PVT buffer on the device.
+
+        Args:
+            pvt_buffer_id: The ID of the PVT buffer to control. PVT buffer IDs start at one.
+
+        Returns:
+            PvtBuffer instance.
+        """
+        if pvt_buffer_id <= 0:
+            raise ValueError('Invalid value; PVT buffers are numbered from 1.')
+
+        return PvtBuffer(self, pvt_buffer_id)
+
     def get_state(
             self
     ) -> str:
         """
         Returns a serialization of the current device state that can be saved and reapplied.
 
         Returns:
```

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/device_identity.py` & `zaber_motion-3.4.0/zaber_motion/ascii/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/device_io.py` & `zaber_motion-3.4.0/zaber_motion/ascii/device_io.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/device_io_info.py` & `zaber_motion-3.4.0/zaber_motion/ascii/device_io_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/device_settings.py` & `zaber_motion-3.4.0/zaber_motion/ascii/device_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/lockstep.py` & `zaber_motion-3.4.0/zaber_motion/ascii/lockstep.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/lockstep_axes.py` & `zaber_motion-3.4.0/zaber_motion/ascii/lockstep_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/oscilloscope.py` & `zaber_motion-3.4.0/zaber_motion/ascii/oscilloscope.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/oscilloscope_capture_properties.py` & `zaber_motion-3.4.0/zaber_motion/ascii/oscilloscope_capture_properties.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/oscilloscope_data.py` & `zaber_motion-3.4.0/zaber_motion/ascii/oscilloscope_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/paramset_info.py` & `zaber_motion-3.4.0/zaber_motion/ascii/paramset_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/pid_tuning.py` & `zaber_motion-3.4.0/zaber_motion/ascii/pid_tuning.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/response.py` & `zaber_motion-3.4.0/zaber_motion/ascii/response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/servo_tuner.py` & `zaber_motion-3.4.0/zaber_motion/ascii/servo_tuner.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/servo_tuning_param.py` & `zaber_motion-3.4.0/zaber_motion/ascii/servo_tuning_param.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/setting_constants.py` & `zaber_motion-3.4.0/zaber_motion/ascii/setting_constants.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/simple_tuning_param_definition.py` & `zaber_motion-3.4.0/zaber_motion/ascii/simple_tuning_param_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/storage.py` & `zaber_motion-3.4.0/zaber_motion/ascii/storage.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/stream.py` & `zaber_motion-3.4.0/zaber_motion/ascii/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 if TYPE_CHECKING:
     from .device import Device
 
 
 class Stream:
     """
-    A handle for a stream with this ID on the device.
+    A handle for a stream with this number on the device.
     Streams provide a way to execute or store a sequence of actions.
     Stream methods append actions to a queue which executes or stores actions in a first in, first out order.
     """
 
     @property
     def device(self) -> 'Device':
         """
@@ -1000,15 +1000,15 @@
         """
         Wait for the value of a analog input channel to reach a condition concerning a given value.
 
         Args:
             channel_number: The number of the analog input channel.
                 Channel numbers are numbered from one.
             condition: A condition (e.g. <, <=, ==, !=).
-            value: The value that the condition concerns, in volts.
+            value: The value that the condition concerns, in Volts.
         """
         request = main_pb2.StreamWaitAnalogInputRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.channel_number = channel_number
         request.condition = condition
@@ -1024,15 +1024,15 @@
         """
         Wait for the value of a analog input channel to reach a condition concerning a given value.
 
         Args:
             channel_number: The number of the analog input channel.
                 Channel numbers are numbered from one.
             condition: A condition (e.g. <, <=, ==, !=).
-            value: The value that the condition concerns, in volts.
+            value: The value that the condition concerns, in Volts.
         """
         request = main_pb2.StreamWaitAnalogInputRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.channel_number = channel_number
         request.condition = condition
@@ -1088,15 +1088,15 @@
     ) -> None:
         """
         Set the value of an analog output channel.
 
         Args:
             channel_number: The number of the analog output channel.
                 Channel numbers are numbered from one.
-            value: The value to set the channel to, in volts.
+            value: The value to set the channel to, in Volts.
         """
         request = main_pb2.StreamSetAnalogOutputRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.channel_number = channel_number
         request.value = value
@@ -1109,15 +1109,15 @@
     ) -> None:
         """
         Set the value of an analog output channel.
 
         Args:
             channel_number: The number of the analog output channel.
                 Channel numbers are numbered from one.
-            value: The value to set the channel to, in volts.
+            value: The value to set the channel to, in Volts.
         """
         request = main_pb2.StreamSetAnalogOutputRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.channel_number = channel_number
         request.value = value
@@ -1197,15 +1197,15 @@
             self,
             values: List[float]
     ) -> None:
         """
         Sets values for all analog output channels.
 
         Args:
-            values: Voltage values to set the output channels to.
+            values: The values to set the output channels to, in Volts.
         """
         request = main_pb2.StreamSetAllAnalogOutputsRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.values.extend(values)
         call("device/stream_set_all_analog_outputs", request)
@@ -1214,15 +1214,15 @@
             self,
             values: List[float]
     ) -> None:
         """
         Sets values for all analog output channels.
 
         Args:
-            values: Voltage values to set the output channels to.
+            values: The values to set the output channels to, in Volts.
         """
         request = main_pb2.StreamSetAllAnalogOutputsRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.values.extend(values)
         await call_async("device/stream_set_all_analog_outputs", request)
@@ -1672,30 +1672,30 @@
         call_sync("device/stream_to_string", request, response)
         return response.value
 
     def disable(
             self
     ) -> None:
         """
-        Disable the stream.
+        Disables the stream.
         If the stream is not setup, this command does nothing.
         Once disabled, the stream will no longer accept stream commands.
         The stream will process the rest of the commands in the queue until it is empty.
         """
         request = main_pb2.StreamEmptyRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         call("device/stream_disable", request)
 
     async def disable_async(
             self
     ) -> None:
         """
-        Disable the stream.
+        Disables the stream.
         If the stream is not setup, this command does nothing.
         Once disabled, the stream will no longer accept stream commands.
         The stream will process the rest of the commands in the queue until it is empty.
         """
         request = main_pb2.StreamEmptyRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
@@ -1810,14 +1810,38 @@
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         response = main_pb2.BoolResponse()
         await call_async("device/stream_check_disabled", request, response)
         return response.value
 
+    def treat_discontinuities_as_error(
+            self
+    ) -> None:
+        """
+        Makes the stream throw StreamDiscontinuityException when it encounters discontinuities (ND warning flag).
+        """
+        request = main_pb2.StreamEmptyRequest()
+        request.interface_id = self.device.connection.interface_id
+        request.device = self.device.device_address
+        request.stream_id = self.stream_id
+        call_sync("device/stream_treat_discontinuities", request)
+
+    def ignore_current_discontinuity(
+            self
+    ) -> None:
+        """
+        Prevents StreamDiscontinuityException as a result of expected discontinuity when resuming streaming.
+        """
+        request = main_pb2.StreamEmptyRequest()
+        request.interface_id = self.device.connection.interface_id
+        request.device = self.device.device_address
+        request.stream_id = self.stream_id
+        call_sync("device/stream_ignore_discontinuity", request)
+
     def __retrieve_axes(
             self
     ) -> List[StreamAxisDefinition]:
         """
         Gets the axes of the stream.
 
         Returns:
```

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/stream_axis_definition.py` & `zaber_motion-3.4.0/zaber_motion/ascii/stream_axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/stream_buffer.py` & `zaber_motion-3.4.0/zaber_motion/ascii/stream_buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 if TYPE_CHECKING:
     from .device import Device
 
 
 class StreamBuffer:
     """
-    Represents a stream buffer with this ID on a device.
+    Represents a stream buffer with this number on a device.
     A stream buffer is a place to store a queue of stream actions.
     """
 
     @property
     def device(self) -> 'Device':
         """
         The Device this buffer exists on.
```

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/transport.py` & `zaber_motion-3.4.0/zaber_motion/ascii/transport.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/unknown_response_event.py` & `zaber_motion-3.4.0/zaber_motion/ascii/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/warning_flags.py` & `zaber_motion-3.4.0/zaber_motion/ascii/warning_flags.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/ascii/warnings.py` & `zaber_motion-3.4.0/zaber_motion/ascii/warnings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/binary/__init__.py` & `zaber_motion-3.4.0/zaber_motion/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/binary/binary_settings.py` & `zaber_motion-3.4.0/zaber_motion/binary/binary_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/binary/command_code.py` & `zaber_motion-3.4.0/zaber_motion/binary/command_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/binary/connection.py` & `zaber_motion-3.4.0/zaber_motion/binary/connection.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/binary/device.py` & `zaber_motion-3.4.0/zaber_motion/binary/device.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/binary/device_identity.py` & `zaber_motion-3.4.0/zaber_motion/binary/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/binary/device_settings.py` & `zaber_motion-3.4.0/zaber_motion/binary/device_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/binary/error_code.py` & `zaber_motion-3.4.0/zaber_motion/binary/error_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/binary/message.py` & `zaber_motion-3.4.0/zaber_motion/binary/message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/binary/reply_only_event.py` & `zaber_motion-3.4.0/zaber_motion/binary/reply_only_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/binary/unknown_response_event.py` & `zaber_motion-3.4.0/zaber_motion/binary/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/bindings.py` & `zaber_motion-3.4.0/zaber_motion/bindings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/call.py` & `zaber_motion-3.4.0/zaber_motion/call.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/convert_exception.py` & `zaber_motion-3.4.0/zaber_motion/convert_exception.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,19 +32,26 @@
 from .exceptions.movement_failed_exception import MovementFailedException
 from .exceptions.movement_interrupted_exception import MovementInterruptedException
 from .exceptions.no_device_found_exception import NoDeviceFoundException
 from .exceptions.no_value_for_key_exception import NoValueForKeyException
 from .exceptions.not_supported_exception import NotSupportedException
 from .exceptions.os_failed_exception import OsFailedException
 from .exceptions.out_of_request_ids_exception import OutOfRequestIdsException
+from .exceptions.pvt_discontinuity_exception import PvtDiscontinuityException
+from .exceptions.pvt_execution_exception import PvtExecutionException
+from .exceptions.pvt_mode_exception import PvtModeException
+from .exceptions.pvt_movement_failed_exception import PvtMovementFailedException
+from .exceptions.pvt_movement_interrupted_exception import PvtMovementInterruptedException
+from .exceptions.pvt_setup_failed_exception import PvtSetupFailedException
 from .exceptions.request_timeout_exception import RequestTimeoutException
 from .exceptions.serial_port_busy_exception import SerialPortBusyException
 from .exceptions.set_device_state_failed_exception import SetDeviceStateFailedException
 from .exceptions.set_peripheral_state_failed_exception import SetPeripheralStateFailedException
 from .exceptions.setting_not_found_exception import SettingNotFoundException
+from .exceptions.stream_discontinuity_exception import StreamDiscontinuityException
 from .exceptions.stream_execution_exception import StreamExecutionException
 from .exceptions.stream_mode_exception import StreamModeException
 from .exceptions.stream_movement_failed_exception import StreamMovementFailedException
 from .exceptions.stream_movement_interrupted_exception import StreamMovementInterruptedException
 from .exceptions.stream_setup_failed_exception import StreamSetupFailedException
 from .exceptions.timeout_exception import TimeoutException
 from .exceptions.transport_already_used_exception import TransportAlreadyUsedException
@@ -80,19 +87,26 @@
     "MOVEMENT_FAILED": MovementFailedException,
     "MOVEMENT_INTERRUPTED": MovementInterruptedException,
     "NO_DEVICE_FOUND": NoDeviceFoundException,
     "NO_VALUE_FOR_KEY": NoValueForKeyException,
     "NOT_SUPPORTED": NotSupportedException,
     "OS_FAILED": OsFailedException,
     "OUT_OF_REQUEST_IDS": OutOfRequestIdsException,
+    "PVT_DISCONTINUITY": PvtDiscontinuityException,
+    "PVT_EXECUTION": PvtExecutionException,
+    "PVT_MODE": PvtModeException,
+    "PVT_MOVEMENT_FAILED": PvtMovementFailedException,
+    "PVT_MOVEMENT_INTERRUPTED": PvtMovementInterruptedException,
+    "PVT_SETUP_FAILED": PvtSetupFailedException,
     "REQUEST_TIMEOUT": RequestTimeoutException,
     "SERIAL_PORT_BUSY": SerialPortBusyException,
     "SET_DEVICE_STATE_FAILED": SetDeviceStateFailedException,
     "SET_PERIPHERAL_STATE_FAILED": SetPeripheralStateFailedException,
     "SETTING_NOT_FOUND": SettingNotFoundException,
+    "STREAM_DISCONTINUITY": StreamDiscontinuityException,
     "STREAM_EXECUTION": StreamExecutionException,
     "STREAM_MODE": StreamModeException,
     "STREAM_MOVEMENT_FAILED": StreamMovementFailedException,
     "STREAM_MOVEMENT_INTERRUPTED": StreamMovementInterruptedException,
     "STREAM_SETUP_FAILED": StreamSetupFailedException,
     "TIMEOUT": TimeoutException,
     "TRANSPORT_ALREADY_USED": TransportAlreadyUsedException,
```

### Comparing `zaber_motion-3.3.0/zaber_motion/events.py` & `zaber_motion-3.4.0/zaber_motion/events.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/__init__.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,26 @@
 from .movement_failed_exception import MovementFailedException as MovementFailedException
 from .movement_interrupted_exception import MovementInterruptedException as MovementInterruptedException
 from .no_device_found_exception import NoDeviceFoundException as NoDeviceFoundException
 from .no_value_for_key_exception import NoValueForKeyException as NoValueForKeyException
 from .not_supported_exception import NotSupportedException as NotSupportedException
 from .os_failed_exception import OsFailedException as OsFailedException
 from .out_of_request_ids_exception import OutOfRequestIdsException as OutOfRequestIdsException
+from .pvt_discontinuity_exception import PvtDiscontinuityException as PvtDiscontinuityException
+from .pvt_execution_exception import PvtExecutionException as PvtExecutionException
+from .pvt_mode_exception import PvtModeException as PvtModeException
+from .pvt_movement_failed_exception import PvtMovementFailedException as PvtMovementFailedException
+from .pvt_movement_interrupted_exception import PvtMovementInterruptedException as PvtMovementInterruptedException
+from .pvt_setup_failed_exception import PvtSetupFailedException as PvtSetupFailedException
 from .request_timeout_exception import RequestTimeoutException as RequestTimeoutException
 from .serial_port_busy_exception import SerialPortBusyException as SerialPortBusyException
 from .set_device_state_failed_exception import SetDeviceStateFailedException as SetDeviceStateFailedException
 from .set_peripheral_state_failed_exception import SetPeripheralStateFailedException as SetPeripheralStateFailedException
 from .setting_not_found_exception import SettingNotFoundException as SettingNotFoundException
+from .stream_discontinuity_exception import StreamDiscontinuityException as StreamDiscontinuityException
 from .stream_execution_exception import StreamExecutionException as StreamExecutionException
 from .stream_mode_exception import StreamModeException as StreamModeException
 from .stream_movement_failed_exception import StreamMovementFailedException as StreamMovementFailedException
 from .stream_movement_interrupted_exception import StreamMovementInterruptedException as StreamMovementInterruptedException
 from .stream_setup_failed_exception import StreamSetupFailedException as StreamSetupFailedException
 from .timeout_exception import TimeoutException as TimeoutException
 from .transport_already_used_exception import TransportAlreadyUsedException as TransportAlreadyUsedException
@@ -54,15 +61,19 @@
 from .command_failed_exception_data import CommandFailedExceptionData as CommandFailedExceptionData
 from .command_too_long_exception_data import CommandTooLongExceptionData as CommandTooLongExceptionData
 from .device_address_conflict_exception_data import DeviceAddressConflictExceptionData as DeviceAddressConflictExceptionData
 from .device_db_failed_exception_data import DeviceDbFailedExceptionData as DeviceDbFailedExceptionData
 from .g_code_execution_exception_data import GCodeExecutionExceptionData as GCodeExecutionExceptionData
 from .g_code_syntax_exception_data import GCodeSyntaxExceptionData as GCodeSyntaxExceptionData
 from .invalid_packet_exception_data import InvalidPacketExceptionData as InvalidPacketExceptionData
+from .invalid_pvt_point import InvalidPvtPoint as InvalidPvtPoint
 from .invalid_response_exception_data import InvalidResponseExceptionData as InvalidResponseExceptionData
 from .movement_failed_exception_data import MovementFailedExceptionData as MovementFailedExceptionData
 from .movement_interrupted_exception_data import MovementInterruptedExceptionData as MovementInterruptedExceptionData
+from .pvt_execution_exception_data import PvtExecutionExceptionData as PvtExecutionExceptionData
+from .pvt_movement_failed_exception_data import PvtMovementFailedExceptionData as PvtMovementFailedExceptionData
+from .pvt_movement_interrupted_exception_data import PvtMovementInterruptedExceptionData as PvtMovementInterruptedExceptionData
 from .set_device_state_exception_data import SetDeviceStateExceptionData as SetDeviceStateExceptionData
 from .set_peripheral_state_exception_data import SetPeripheralStateExceptionData as SetPeripheralStateExceptionData
 from .stream_execution_exception_data import StreamExecutionExceptionData as StreamExecutionExceptionData
 from .stream_movement_failed_exception_data import StreamMovementFailedExceptionData as StreamMovementFailedExceptionData
 from .stream_movement_interrupted_exception_data import StreamMovementInterruptedExceptionData as StreamMovementInterruptedExceptionData
```

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/binary_command_failed_exception.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/binary_command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/binary_command_failed_exception_data.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/binary_command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/command_failed_exception.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/command_failed_exception_data.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/command_too_long_exception.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/command_too_long_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/command_too_long_exception_data.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/command_too_long_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/device_address_conflict_exception.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/device_address_conflict_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/device_address_conflict_exception_data.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/device_address_conflict_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/device_db_failed_exception.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/device_db_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/device_db_failed_exception_data.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/device_db_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/g_code_execution_exception.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/g_code_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/g_code_execution_exception_data.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/g_code_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/g_code_syntax_exception.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/g_code_syntax_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/g_code_syntax_exception_data.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/g_code_syntax_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/invalid_packet_exception.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/invalid_packet_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/invalid_packet_exception_data.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/invalid_packet_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/invalid_response_exception.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/invalid_response_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/invalid_response_exception_data.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/invalid_response_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/movement_failed_exception.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/movement_failed_exception_data.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/movement_interrupted_exception.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/movement_interrupted_exception_data.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/set_device_state_exception_data.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/set_device_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/set_device_state_failed_exception.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/set_device_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/set_peripheral_state_exception_data.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/set_peripheral_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/set_peripheral_state_failed_exception.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/set_peripheral_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/stream_execution_exception.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/stream_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/stream_execution_exception_data.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/stream_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/stream_movement_failed_exception.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/stream_movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/stream_movement_failed_exception_data.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/stream_movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/stream_movement_interrupted_exception.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/stream_movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py` & `zaber_motion-3.4.0/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/firmware_version.py` & `zaber_motion-3.4.0/zaber_motion/firmware_version.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/gcode/__init__.py` & `zaber_motion-3.4.0/zaber_motion/gcode/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/gcode/axis_definition.py` & `zaber_motion-3.4.0/zaber_motion/gcode/axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/gcode/axis_mapping.py` & `zaber_motion-3.4.0/zaber_motion/gcode/axis_mapping.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/gcode/axis_transformation.py` & `zaber_motion-3.4.0/zaber_motion/gcode/axis_transformation.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/gcode/device_definition.py` & `zaber_motion-3.4.0/zaber_motion/gcode/device_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/gcode/offline_translator.py` & `zaber_motion-3.4.0/zaber_motion/gcode/offline_translator.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/gcode/translate_message.py` & `zaber_motion-3.4.0/zaber_motion/gcode/translate_message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/gcode/translate_result.py` & `zaber_motion-3.4.0/zaber_motion/gcode/translate_result.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/gcode/translator.py` & `zaber_motion-3.4.0/zaber_motion/gcode/translator.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/gcode/translator_config.py` & `zaber_motion-3.4.0/zaber_motion/gcode/translator_config.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/library.py` & `zaber_motion-3.4.0/zaber_motion/library.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/measurement.py` & `zaber_motion-3.4.0/zaber_motion/measurement.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/microscopy/objective_changer.py` & `zaber_motion-3.4.0/zaber_motion/microscopy/objective_changer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/protobufs/main_pb2.py` & `zaber_motion-3.4.0/zaber_motion/protobufs/main_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14protobufs/main.proto\x12\x16zaber.motion.protobufs\"\x1a\n\x07Request\x12\x0f\n\x07request\x18\x01 \x01(\t\"\xb9\x01\n\x08Response\x12?\n\x08response\x18\x01 \x01(\x0e\x32-.zaber.motion.protobufs.Response.ResponseType\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"!\n\x0cResponseType\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x16\n\x05\x45vent\x12\r\n\x05\x65vent\x18\x01 \x01(\t\"\x0e\n\x0c\x45mptyRequest\"\x1d\n\x0c\x42oolResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\x1f\n\x0e\x44oubleResponse\x12\r\n\x05value\x18\x01 \x01(\x01\"%\n\x13\x44oubleArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"\x1c\n\x0bIntResponse\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1f\n\x0eStringResponse\x12\r\n\x05value\x18\x01 \x01(\t\"%\n\x13StringArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xdd\x01\n\x0c\x41xisIdentity\x12\x15\n\ris_peripheral\x18\x01 \x01(\x08\x12\x15\n\rperipheral_id\x18\x02 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x03 \x01(\t\x12@\n\taxis_type\x18\x04 \x01(\x0e\x32-.zaber.motion.protobufs.AxisIdentity.AxisType\x12\x13\n\x0bis_modified\x18\x05 \x01(\x08\"/\n\x08\x41xisType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\xcb\x01\n\x0e\x44\x65viceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\naxis_count\x18\x04 \x01(\x05\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x13\n\x0bis_modified\x18\x06 \x01(\x08\x12\x15\n\ris_integrated\x18\x07 \x01(\x08\">\n\x0f\x46irmwareVersion\x12\r\n\x05major\x18\x01 \x01(\x05\x12\r\n\x05minor\x18\x02 \x01(\x05\x12\r\n\x05\x62uild\x18\x03 \x01(\x05\"\x8a\x01\n\x0c\x44\x65viceIOInfo\x12\x1d\n\x15number_analog_outputs\x18\x02 \x01(\x05\x12\x1c\n\x14number_analog_inputs\x18\x03 \x01(\x05\x12\x1e\n\x16number_digital_outputs\x18\x04 \x01(\x05\x12\x1d\n\x15number_digital_inputs\x18\x05 \x01(\x05\"*\n\x0bMeasurement\x12\r\n\x05value\x18\x01 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\">\n\x14StreamAxisDefinition\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x11\n\taxis_type\x18\x02 \x01(\x05\"<\n\x1aInvalidPacketExceptionData\x12\x0e\n\x06packet\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\">\n\"DeviceAddressConflictExceptionData\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"b\n MovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"J\n&StreamMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"]\n\x1bMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"E\n!StreamMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1cStreamExecutionExceptionData\x12\x12\n\nerror_flag\x18\x03 \x01(\t\x12\x0e\n\x06reason\x18\x04 \x01(\t\"0\n\x1cInvalidResponseExceptionData\x12\x10\n\x08response\x18\x01 \x01(\t\"m\n\x1a\x43ommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\t\x12\x12\n\nreply_flag\x18\x05 \x01(\t\x12\x0e\n\x06status\x18\x06 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x07 \x01(\t\"9\n BinaryCommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\x05\"\x89\x01\n\x1fSetPeripheralStateExceptionData\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x10\n\x08settings\x18\x02 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x03 \x01(\t\x12\x0f\n\x07storage\x18\x04 \x03(\t\x12\x18\n\x10stored_positions\x18\x05 \x03(\t\"\xe8\x01\n\x1bSetDeviceStateExceptionData\x12L\n\x0bperipherals\x18\x02 \x03(\x0b\x32\x37.zaber.motion.protobufs.SetPeripheralStateExceptionData\x12\x10\n\x08settings\x18\x03 \x03(\t\x12\x16\n\x0estream_buffers\x18\x04 \x03(\t\x12\x10\n\x08triggers\x18\x05 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x06 \x01(\t\x12\x0f\n\x07storage\x18\x07 \x03(\t\x12\x18\n\x10stored_positions\x18\x08 \x03(\t\"g\n\x1b\x43ommandTooLongExceptionData\x12\x0b\n\x03\x66it\x18\x01 \x01(\t\x12\x11\n\tremainder\x18\x02 \x01(\t\x12\x13\n\x0bpacket_size\x18\x03 \x01(\x05\x12\x13\n\x0bpackets_max\x18\x04 \x01(\x05\"V\n\x0bTestRequest\x12\x14\n\x0creturn_error\x18\x01 \x01(\x08\x12\x11\n\tdata_ping\x18\x02 \x01(\t\x12\x1e\n\x16return_error_with_data\x18\x03 \x01(\x08\"!\n\x0cTestResponse\x12\x11\n\tdata_pong\x18\x01 \x01(\t\"%\n\x10TestResponseLong\x12\x11\n\tdata_pong\x18\x01 \x03(\t\"\x19\n\tTestEvent\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"-\n\x1cToolsListSerialPortsResponse\x12\r\n\x05ports\x18\x01 \x03(\t\"&\n\x16SetInternalModeRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x08\"I\n\x18SetDeviceDbSourceRequest\x12\x13\n\x0bsource_type\x18\x01 \x01(\x05\x12\x18\n\x10url_or_file_path\x18\x02 \x01(\t\"G\n\x1aToggleDeviceDbStoreRequest\x12\x11\n\ttoggle_on\x18\x01 \x01(\x08\x12\x16\n\x0estore_location\x18\x02 \x01(\t\"+\n\x1b\x44\x65viceDbFailedExceptionData\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xa7\x02\n\x14OpenInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x11\n\ttransport\x18\x06 \x01(\x05\x12 \n\x18reject_routed_connection\x18\x07 \x01(\x08\x12\x10\n\x08\x63loud_id\x18\x08 \x01(\t\x12\x17\n\x0f\x63onnection_name\x18\t \x01(\t\x12\r\n\x05realm\x18\n \x01(\t\x12\r\n\x05token\x18\x0b \x01(\t\x12\x0b\n\x03\x61pi\x18\x0c \x01(\t\"-\n\x15OpenInterfaceResponse\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"-\n\x15InterfaceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"C\n\x1aSetInterfaceTimeoutRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\"N\n\"SetInterfaceChecksumEnabledRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\"F\n\x10\x41xisEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\"\x83\x01\n\x15GenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x05\"\xc8\x01\n\x16GenericCommandResponse\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"e\n GenericCommandResponseCollection\x12\x41\n\tresponses\x18\x02 \x03(\x0b\x32..zaber.motion.protobufs.GenericCommandResponse\"\xdc\x01\n\x14UnknownResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"\x83\x01\n\nAlertEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\t\"t\n\x11\x44isconnectedEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"~\n\x15\x44\x65viceIdentifyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12?\n\x0e\x61ssume_version\x18\x03 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\"D\n\x15\x44\x65viceRenumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x15\n\rfirst_address\x18\x02 \x01(\x05\"E\n\x13\x44\x65viceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"\'\n\x14\x44\x65viceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"`\n\x11\x44\x65viceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"n\n\x1a\x44\x65viceWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"\xd0\x02\n\x11\x44\x65viceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12@\n\x04type\x18\x05 \x01(\x0e\x32\x32.zaber.motion.protobufs.DeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\x10\n\x08velocity\x18\x08 \x01(\x01\x12\x15\n\rvelocity_unit\x18\t \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\n \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0b \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"`\n\x11\x44\x65viceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"C\n\x12\x44\x65viceOnAllRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"/\n\x13\x44\x65viceOnAllResponse\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"]\n\x18\x44\x65viceGetWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05\x63lear\x18\x04 \x01(\x08\"*\n\x19\x44\x65viceGetWarningsResponse\x12\r\n\x05\x66lags\x18\x01 \x03(\t\"x\n\x1aWaitToClearWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07timeout\x18\x04 \x01(\x01\x12\x15\n\rwarning_flags\x18\x05 \x03(\t\"Z\n\x1c\x44\x65viceGetAllDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\"/\n\x1d\x44\x65viceGetAllDigitalIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x08\"Y\n\x1b\x44\x65viceGetAllAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\".\n\x1c\x44\x65viceGetAllAnalogIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"o\n\x19\x44\x65viceGetDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"n\n\x18\x44\x65viceGetAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"Y\n!DeviceSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x08\"X\n DeviceSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x01\"l\n\x1d\x44\x65viceSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x08\"k\n\x1c\x44\x65viceSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\"6\n\x13SetLogOutputRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x05\x12\x11\n\tfile_path\x18\x02 \x01(\t\"l\n\x17\x44\x65viceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x94\x01\n\x1b\x44\x65viceConvertSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\r\n\x05value\x18\x06 \x01(\x01\x12\x13\n\x0b\x66rom_native\x18\x07 \x01(\x08\"{\n\x17\x44\x65viceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"p\n\x1a\x44\x65viceSetSettingStrRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\"\x9e\x01\n\x15PrepareCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x18\n\x10\x63ommand_template\x18\x04 \x01(\t\x12\x37\n\nparameters\x18\x05 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"M\n\x14WaitToRespondRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\"f\n\x15LockstepEnableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x04 \x03(\x05\"r\n\x16LockstepDisableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"\xe1\x02\n\x13LockstepMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12\x42\n\x04type\x18\x05 \x01(\x0e\x32\x34.zaber.motion.protobufs.LockstepMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x08 \x01(\t\x12\x10\n\x08velocity\x18\t \x01(\x01\x12\x15\n\rvelocity_unit\x18\n \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\x0b \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0c \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"}\n\x1cLockstepWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"W\n\x14LockstepEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\"N\n\x0cLockstepAxes\x12\x0e\n\x06\x61xis_1\x18\x01 \x01(\x05\x12\x0e\n\x06\x61xis_2\x18\x02 \x01(\x05\x12\x0e\n\x06\x61xis_3\x18\x03 \x01(\x05\x12\x0e\n\x06\x61xis_4\x18\x04 \x01(\x05\".\n\x1eLockstepGetAxisNumbersResponse\x12\x0c\n\x04\x61xes\x18\x01 \x03(\x05\"c\n\x12LockstepGetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\x86\x01\n\x12LockstepSetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\x12\n\naxis_index\x18\x06 \x01(\x05\"d\n\x1dOscilloscopeAddChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\"k\n\x1cOscilloscopeStartStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\r\n\x05start\x18\x03 \x01(\x08\x12\x16\n\x0e\x63\x61pture_length\x18\x04 \x01(\x05\",\n\x18OscilloscopeReadResponse\x12\x10\n\x08\x64\x61ta_ids\x18\x01 \x03(\x05\"-\n\x1aOscilloscopeDataIdentifier\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\"E\n\x1dOscilloscopeCaptureProperties\x12\x0f\n\x07setting\x18\x01 \x01(\t\x12\x13\n\x0b\x61xis_number\x18\x02 \x01(\x05\";\n\x1aOscilloscopeDataGetRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\"T\n$OscilloscopeDataGetSampleTimeRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\"2\n\"OscilloscopeDataGetSamplesResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x01\"_\n\x16StreamSetupLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x04 \x03(\x05\"\x96\x01\n\x1fStreamSetupLiveCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12:\n\x04\x61xes\x18\x04 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"w\n\x17StreamSetupStoreRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x15\n\rstream_buffer\x18\x04 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x05 \x03(\x05\"\xae\x01\n StreamSetupStoreCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x15\n\rstream_buffer\x18\x04 \x01(\x05\x12:\n\x04\x61xes\x18\x05 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\x8a\x01\n$StreamSetupStoreArbitraryAxesRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x15\n\rstream_buffer\x18\x04 \x01(\x05\x12\x12\n\naxes_count\x18\x05 \x01(\x05\"c\n\x11StreamCallRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x15\n\rstream_buffer\x18\x04 \x01(\x05\"\xf8\x01\n\x11StreamLineRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12<\n\x04type\x18\x04 \x01(\x0e\x32..zaber.motion.protobufs.StreamLineRequest.Type\x12\x35\n\x08\x65ndpoint\x18\x05 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x06 \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xb1\x03\n\x10StreamArcRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12;\n\x04type\x18\x04 \x01(\x0e\x32-.zaber.motion.protobufs.StreamArcRequest.Type\x12\x1a\n\x12rotation_direction\x18\x05 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x06 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_x\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_y\x18\t \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\n \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xcf\x02\n\x13StreamCircleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12>\n\x04type\x18\x04 \x01(\x0e\x32\x30.zaber.motion.protobufs.StreamCircleRequest.Type\x12\x1a\n\x12rotation_direction\x18\x05 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x06 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x08 \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x7f\n\x1dStreamWaitDigitalInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\x12\r\n\x05value\x18\x05 \x01(\x08\"\x91\x01\n\x1cStreamWaitAnalogInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\x12\x11\n\tcondition\x18\x05 \x01(\t\x12\r\n\x05value\x18\x06 \x01(\x01\"\x7f\n\x1dStreamSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\x12\r\n\x05value\x18\x05 \x01(\x08\"~\n\x1cStreamSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\x12\r\n\x05value\x18\x05 \x01(\x01\"s\n StreamToggleDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"l\n!StreamSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0e\n\x06values\x18\x04 \x03(\x08\"k\n StreamSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0e\n\x06values\x18\x04 \x03(\x01\"h\n\x11StreamWaitRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"s\n\x1aStreamWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"M\n\x12StreamEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\"S\n\x15StreamGetAxesResponse\x12:\n\x04\x61xes\x18\x01 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"a\n\x18StreamGetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"t\n\x18StreamSetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x11\n\tmax_speed\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"r\n)StreamGetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\x97\x01\n)StreamSetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12#\n\x1bmax_tangential_acceleration\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"s\n*StreamGetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\x99\x01\n*StreamSetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12$\n\x1cmax_centripetal_acceleration\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"X\n\x1dStreamBufferGetContentRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\"6\n\x1eStreamBufferGetContentResponse\x12\x14\n\x0c\x62uffer_lines\x18\x01 \x03(\t\"S\n\x18StreamBufferEraseRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\"g\n\x1bStreamGenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\"j\n StreamGenericCommandBatchRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\r\n\x05\x62\x61tch\x18\x04 \x03(\t\"c\n\x14\x42inaryReplyOnlyEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\xbb\x01\n\x1aOpenBinaryInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x17\n\x0fuse_message_ids\x18\x06 \x01(\x08\"i\n\x1aUnknownBinaryResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\x82\x01\n\x14GenericBinaryRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x01\"F\n\rBinaryMessage\x12\x16\n\x0e\x64\x65vice_address\x18\x01 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x02 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x05\"R\n\x17\x42inaryMessageCollection\x12\x37\n\x08messages\x18\x02 \x03(\x0b\x32%.zaber.motion.protobufs.BinaryMessage\":\n\x12\x44\x65viceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\"\xd9\x02\n\x14\x42inaryDeviceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x15\n\ris_peripheral\x18\x06 \x01(\x08\x12\x15\n\rperipheral_id\x18\x07 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x08 \x01(\t\x12L\n\x0b\x64\x65vice_type\x18\t \x01(\x0e\x32\x37.zaber.motion.protobufs.BinaryDeviceIdentity.DeviceType\"1\n\nDeviceType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\x99\x01\n\x1d\x42inaryGenericWithUnitsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x01\x12\x11\n\tfrom_unit\x18\x05 \x01(\t\x12\x0f\n\x07to_unit\x18\x06 \x01(\t\x12\x0f\n\x07timeout\x18\x07 \x01(\x01\"^\n\x17\x42inaryDeviceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\xda\x01\n\x17\x42inaryDeviceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x46\n\x04type\x18\x04 \x01(\x0e\x32\x38.zaber.motion.protobufs.BinaryDeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"%\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\"^\n\x17\x42inaryDeviceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"K\n\x19\x42inaryDeviceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"-\n\x1a\x42inaryDeviceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"d\n\x1d\x42inaryDeviceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"s\n\x1d\x42inaryDeviceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"2\n\x1a\x43ustomInterfaceReadRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"D\n\x1b\x43ustomInterfaceWriteRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"3\n\x1b\x43ustomInterfaceOpenResponse\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"J\n\x1b\x43ustomInterfaceCloseRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"W\n\x12\x43\x61nSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\"=\n\x17\x43\x61nSetStateAxisResponse\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"p\n\x19\x43\x61nSetStateDeviceResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x44\n\x0b\x61xis_errors\x18\x02 \x03(\x0b\x32/.zaber.motion.protobufs.CanSetStateAxisResponse\"i\n\x0fSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65vice_only\x18\x05 \x01(\x08\"Z\n\x12ServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\"/\n\x10ServoTuningParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"g\n\x0cParamsetInfo\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x05\x12\x38\n\x06params\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"\x9e\x01\n\x15SetServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12?\n\rtuning_params\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"n\n\x0cLoadParamset\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x13\n\x0bto_paramset\x18\x04 \x01(\x05\x12\x15\n\rfrom_paramset\x18\x05 \x01(\x05\"\x8d\x01\n\x18SetServoTuningPIDRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\t\n\x01p\x18\x05 \x01(\x01\x12\t\n\x01i\x18\x06 \x01(\x01\x12\t\n\x01\x64\x18\x07 \x01(\x01\x12\n\n\x02\x66\x63\x18\x08 \x01(\x01\"W\n\tPidTuning\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\t\n\x01p\x18\x03 \x01(\x01\x12\t\n\x01i\x18\x04 \x01(\x01\x12\t\n\x01\x64\x18\x05 \x01(\x01\x12\n\n\x02\x66\x63\x18\x06 \x01(\x01\"\xc2\x01\n\x0fSetSimpleTuning\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\x15\n\rcarriage_mass\x18\x05 \x01(\x01\x12\x11\n\tload_mass\x18\x06 \x01(\x01\x12?\n\rtuning_params\x18\x07 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"d\n\x1bSimpleTuningParamDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tmin_label\x18\x02 \x01(\t\x12\x11\n\tmax_label\x18\x03 \x01(\t\x12\x11\n\tdata_type\x18\x04 \x01(\t\"m\n&GetSimpleTuningParamDefinitionResponse\x12\x43\n\x06params\x18\x01 \x03(\x0b\x32\x33.zaber.motion.protobufs.SimpleTuningParamDefinition\"\x95\x01\n\x17TranslatorCreateRequest\x12@\n\ndefinition\x18\x01 \x01(\x0b\x32,.zaber.motion.protobufs.TranslatorDefinition\x12\x38\n\x06\x63onfig\x18\x02 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"1\n\x18TranslatorCreateResponse\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"O\n\x18TranslatorAxisDefinition\x12\x15\n\rperipheral_id\x18\x01 \x01(\x05\x12\x1c\n\x14microstep_resolution\x18\x02 \x01(\x05\"\xa1\x01\n\x14TranslatorDefinition\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12>\n\x04\x61xes\x18\x02 \x03(\x0b\x32\x30.zaber.motion.protobufs.TranslatorAxisDefinition\x12\x36\n\tmax_speed\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\xac\x01\n\x10TranslatorConfig\x12\x44\n\raxis_mappings\x18\x01 \x03(\x0b\x32-.zaber.motion.protobufs.TranslatorAxisMapping\x12R\n\x14\x61xis_transformations\x18\x02 \x03(\x0b\x32\x34.zaber.motion.protobufs.TranslatorAxisTransformation\"@\n\x15TranslatorAxisMapping\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x12\n\naxis_index\x18\x02 \x01(\x05\"~\n\x1cTranslatorAxisTransformation\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x0f\n\x07scaling\x18\x02 \x01(\x01\x12\x38\n\x0btranslation\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"B\n\x1aTranslatorTranslateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\r\n\x05\x62lock\x18\x02 \x01(\t\"I\n\x10TranslateMessage\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x12\n\nfrom_block\x18\x02 \x01(\x05\x12\x10\n\x08to_block\x18\x03 \x01(\x05\"k\n\x1bTranslatorTranslateResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\x12:\n\x08warnings\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.TranslateMessage\"@\n\x18GCodeSyntaxExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"C\n\x1bGCodeExecutionExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"L\n\x1aTranslatorFlushLiveRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"+\n\x17TranslatorFlushResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\"\x90\x01\n\x1bTranslatorCreateLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"\x91\x01\n!TranslatorCreateFromDeviceRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x03 \x03(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"/\n\x16TranslatorEmptyRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"^\n TranslatorSetTraverseRateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x15\n\rtraverse_rate\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"g\n TranslatorSetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x10\n\x08position\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"U\n TranslatorGetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x0c\n\x04unit\x18\x03 \x01(\t\"n\n\x1eTranslatorGetAxisOffsetRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x19\n\x11\x63oordinate_system\x18\x02 \x01(\t\x12\x0c\n\x04\x61xis\x18\x03 \x01(\t\x12\x0c\n\x04unit\x18\x04 \x01(\t\"R\n$TranslatorSetFeedRateOverrideRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x13\n\x0b\x63oefficient\x18\x02 \x01(\x01\"y\n\x17\x44\x65viceSetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\x12\x0e\n\x06\x65ncode\x18\x06 \x01(\x08\"j\n\x17\x44\x65viceGetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\x0e\n\x06\x64\x65\x63ode\x18\x05 \x01(\x08\"o\n\x1d\x44\x65viceSetStorageNumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\"m\n\x1b\x44\x65viceSetStorageBoolRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x08\"W\n\x14\x44\x65viceStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\"b\n\x1c\x44\x65viceStorageListKeysRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0e\n\x06prefix\x18\x04 \x01(\t\"\xa1\x01\n\x1f\x44\x65viceSetUnitConversionsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12=\n\x0b\x63onversions\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ConversionFactor\"@\n\x10\x43onversionFactor\x12\x0f\n\x07setting\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"^\n\x17ObjectiveChangerRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\"?\n\x1eObjectiveChangerCreateResponse\x12\x0e\n\x06turret\x18\x02 \x01(\x05\x12\r\n\x05\x66ocus\x18\x03 \x01(\x05\"\xb2\x01\n\x1dObjectiveChangerChangeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\x12\x11\n\tobjective\x18\x04 \x01(\x05\x12\x39\n\x0c\x66ocus_offset\x18\x05 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement*-\n\x0bMessageType\x12\t\n\x05REPLY\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\t\n\x05\x41LERT\x10\x02*\xa1\x08\n\x06\x45rrors\x12\x13\n\x0fREQUEST_TIMEOUT\x10\x00\x12\x15\n\x11\x43ONNECTION_CLOSED\x10\x01\x12\x14\n\x10INVALID_ARGUMENT\x10\x02\x12\x16\n\x12OUT_OF_REQUEST_IDS\x10\x03\x12\x12\n\x0eINVALID_PACKET\x10\x04\x12\x15\n\x11\x43ONNECTION_FAILED\x10\x05\x12\x13\n\x0fUNKNOWN_REQUEST\x10\x06\x12\x12\n\x0e\x43OMMAND_FAILED\x10\x07\x12\x14\n\x10\x44\x45VICE_DB_FAILED\x10\x08\x12\x10\n\x0cINVALID_DATA\x10\t\x12\x19\n\x15\x44\x45VICE_NOT_IDENTIFIED\x10\n\x12\x15\n\x11\x43ONVERSION_FAILED\x10\x0b\x12\x1b\n\x17\x44\x45VICE_ADDRESS_CONFLICT\x10\x0c\x12\x13\n\x0fNO_DEVICE_FOUND\x10\r\x12\x18\n\x14MOVEMENT_INTERRUPTED\x10\x0e\x12\x13\n\x0fMOVEMENT_FAILED\x10\x0f\x12\r\n\tIO_FAILED\x10\x10\x12\x14\n\x10INVALID_RESPONSE\x10\x11\x12\x11\n\rNOT_SUPPORTED\x10\x12\x12\x11\n\rDEVICE_FAILED\x10\x13\x12\r\n\tOS_FAILED\x10\x14\x12\x12\n\x0eINTERNAL_ERROR\x10\x16\x12\x19\n\x15\x42INARY_COMMAND_FAILED\x10\x18\x12\x15\n\x11\x43OMMAND_PREEMPTED\x10\x19\x12\x18\n\x14LOCKSTEP_NOT_ENABLED\x10\x1a\x12\x14\n\x10LOCKSTEP_ENABLED\x10\x1b\x12\x1b\n\x17IO_CHANNEL_OUT_OF_RANGE\x10\x1c\x12\x15\n\x11SETTING_NOT_FOUND\x10\x1d\x12\x0f\n\x0bSTREAM_MODE\x10\x1e\x12\x14\n\x10STREAM_EXECUTION\x10\x1f\x12\x1a\n\x16STREAM_MOVEMENT_FAILED\x10 \x12\x17\n\x13STREAM_SETUP_FAILED\x10!\x12\x0f\n\x0b\x44\x45VICE_BUSY\x10\"\x12\x1f\n\x1bSTREAM_MOVEMENT_INTERRUPTED\x10#\x12\x16\n\x12INVALID_PARK_STATE\x10$\x12\x14\n\x10SERIAL_PORT_BUSY\x10%\x12\x1a\n\x16TRANSPORT_ALREADY_USED\x10&\x12\x1f\n\x1bSET_PERIPHERAL_STATE_FAILED\x10\'\x12\x1b\n\x17SET_DEVICE_STATE_FAILED\x10(\x12\x11\n\rG_CODE_SYNTAX\x10)\x12\x14\n\x10G_CODE_EXECUTION\x10*\x12\x15\n\x11INVALID_OPERATION\x10+\x12\x14\n\x10\x43OMMAND_TOO_LONG\x10,\x12\x14\n\x10NO_VALUE_FOR_KEY\x10-\x12\x1b\n\x17\x44\x45VICE_DETECTION_FAILED\x10.\x12\x0b\n\x07TIMEOUT\x10/*Q\n\rInterfaceType\x12\x0f\n\x0bSERIAL_PORT\x10\x00\x12\x07\n\x03TCP\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\x12\x07\n\x03IOT\x10\x03\x12\x11\n\rNETWORK_SHARE\x10\x04\x42$Z\"./protobufs;zaber_motion_protobufsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14protobufs/main.proto\x12\x16zaber.motion.protobufs\"\x1a\n\x07Request\x12\x0f\n\x07request\x18\x01 \x01(\t\"\xb9\x01\n\x08Response\x12?\n\x08response\x18\x01 \x01(\x0e\x32-.zaber.motion.protobufs.Response.ResponseType\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"!\n\x0cResponseType\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x16\n\x05\x45vent\x12\r\n\x05\x65vent\x18\x01 \x01(\t\"\x0e\n\x0c\x45mptyRequest\"\x1d\n\x0c\x42oolResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\x1f\n\x0e\x44oubleResponse\x12\r\n\x05value\x18\x01 \x01(\x01\"%\n\x13\x44oubleArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"\x1c\n\x0bIntResponse\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1f\n\x0eStringResponse\x12\r\n\x05value\x18\x01 \x01(\t\"%\n\x13StringArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xdd\x01\n\x0c\x41xisIdentity\x12\x15\n\ris_peripheral\x18\x01 \x01(\x08\x12\x15\n\rperipheral_id\x18\x02 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x03 \x01(\t\x12@\n\taxis_type\x18\x04 \x01(\x0e\x32-.zaber.motion.protobufs.AxisIdentity.AxisType\x12\x13\n\x0bis_modified\x18\x05 \x01(\x08\"/\n\x08\x41xisType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\xcb\x01\n\x0e\x44\x65viceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\naxis_count\x18\x04 \x01(\x05\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x13\n\x0bis_modified\x18\x06 \x01(\x08\x12\x15\n\ris_integrated\x18\x07 \x01(\x08\">\n\x0f\x46irmwareVersion\x12\r\n\x05major\x18\x01 \x01(\x05\x12\r\n\x05minor\x18\x02 \x01(\x05\x12\r\n\x05\x62uild\x18\x03 \x01(\x05\"\x8a\x01\n\x0c\x44\x65viceIOInfo\x12\x1d\n\x15number_analog_outputs\x18\x02 \x01(\x05\x12\x1c\n\x14number_analog_inputs\x18\x03 \x01(\x05\x12\x1e\n\x16number_digital_outputs\x18\x04 \x01(\x05\x12\x1d\n\x15number_digital_inputs\x18\x05 \x01(\x05\"*\n\x0bMeasurement\x12\r\n\x05value\x18\x01 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\">\n\x14StreamAxisDefinition\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x11\n\taxis_type\x18\x02 \x01(\x05\"<\n\x1aInvalidPacketExceptionData\x12\x0e\n\x06packet\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\">\n\"DeviceAddressConflictExceptionData\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"b\n MovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"J\n&StreamMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"G\n#PvtMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"]\n\x1bMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"E\n!StreamMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1ePvtMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1cStreamExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"\x80\x01\n\x19PvtExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12?\n\x0einvalid_points\x18\x03 \x03(\x0b\x32\'.zaber.motion.protobufs.InvalidPvtPoint\"/\n\x0fInvalidPvtPoint\x12\r\n\x05index\x18\x01 \x01(\x05\x12\r\n\x05point\x18\x02 \x01(\t\"0\n\x1cInvalidResponseExceptionData\x12\x10\n\x08response\x18\x01 \x01(\t\"m\n\x1a\x43ommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\t\x12\x12\n\nreply_flag\x18\x05 \x01(\t\x12\x0e\n\x06status\x18\x06 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x07 \x01(\t\"9\n BinaryCommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\x05\"\x89\x01\n\x1fSetPeripheralStateExceptionData\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x10\n\x08settings\x18\x02 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x03 \x01(\t\x12\x0f\n\x07storage\x18\x04 \x03(\t\x12\x18\n\x10stored_positions\x18\x05 \x03(\t\"\xe8\x01\n\x1bSetDeviceStateExceptionData\x12L\n\x0bperipherals\x18\x02 \x03(\x0b\x32\x37.zaber.motion.protobufs.SetPeripheralStateExceptionData\x12\x10\n\x08settings\x18\x03 \x03(\t\x12\x16\n\x0estream_buffers\x18\x04 \x03(\t\x12\x10\n\x08triggers\x18\x05 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x06 \x01(\t\x12\x0f\n\x07storage\x18\x07 \x03(\t\x12\x18\n\x10stored_positions\x18\x08 \x03(\t\"g\n\x1b\x43ommandTooLongExceptionData\x12\x0b\n\x03\x66it\x18\x01 \x01(\t\x12\x11\n\tremainder\x18\x02 \x01(\t\x12\x13\n\x0bpacket_size\x18\x03 \x01(\x05\x12\x13\n\x0bpackets_max\x18\x04 \x01(\x05\"V\n\x0bTestRequest\x12\x14\n\x0creturn_error\x18\x01 \x01(\x08\x12\x11\n\tdata_ping\x18\x02 \x01(\t\x12\x1e\n\x16return_error_with_data\x18\x03 \x01(\x08\"!\n\x0cTestResponse\x12\x11\n\tdata_pong\x18\x01 \x01(\t\"%\n\x10TestResponseLong\x12\x11\n\tdata_pong\x18\x01 \x03(\t\"\x19\n\tTestEvent\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"-\n\x1cToolsListSerialPortsResponse\x12\r\n\x05ports\x18\x01 \x03(\t\"&\n\x16SetInternalModeRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x08\"I\n\x18SetDeviceDbSourceRequest\x12\x13\n\x0bsource_type\x18\x01 \x01(\x05\x12\x18\n\x10url_or_file_path\x18\x02 \x01(\t\"G\n\x1aToggleDeviceDbStoreRequest\x12\x11\n\ttoggle_on\x18\x01 \x01(\x08\x12\x16\n\x0estore_location\x18\x02 \x01(\t\"+\n\x1b\x44\x65viceDbFailedExceptionData\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xa7\x02\n\x14OpenInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x11\n\ttransport\x18\x06 \x01(\x05\x12 \n\x18reject_routed_connection\x18\x07 \x01(\x08\x12\x10\n\x08\x63loud_id\x18\x08 \x01(\t\x12\x17\n\x0f\x63onnection_name\x18\t \x01(\t\x12\r\n\x05realm\x18\n \x01(\t\x12\r\n\x05token\x18\x0b \x01(\t\x12\x0b\n\x03\x61pi\x18\x0c \x01(\t\"-\n\x15OpenInterfaceResponse\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"-\n\x15InterfaceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"C\n\x1aSetInterfaceTimeoutRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\"N\n\"SetInterfaceChecksumEnabledRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\"F\n\x10\x41xisEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\"\x83\x01\n\x15GenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x05\"\xc8\x01\n\x16GenericCommandResponse\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"e\n GenericCommandResponseCollection\x12\x41\n\tresponses\x18\x02 \x03(\x0b\x32..zaber.motion.protobufs.GenericCommandResponse\"\xdc\x01\n\x14UnknownResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"\x83\x01\n\nAlertEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\t\"t\n\x11\x44isconnectedEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"~\n\x15\x44\x65viceIdentifyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12?\n\x0e\x61ssume_version\x18\x03 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\"D\n\x15\x44\x65viceRenumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x15\n\rfirst_address\x18\x02 \x01(\x05\"E\n\x13\x44\x65viceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"\'\n\x14\x44\x65viceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"`\n\x11\x44\x65viceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"n\n\x1a\x44\x65viceWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"\xd0\x02\n\x11\x44\x65viceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12@\n\x04type\x18\x05 \x01(\x0e\x32\x32.zaber.motion.protobufs.DeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\x10\n\x08velocity\x18\x08 \x01(\x01\x12\x15\n\rvelocity_unit\x18\t \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\n \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0b \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"`\n\x11\x44\x65viceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"C\n\x12\x44\x65viceOnAllRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"/\n\x13\x44\x65viceOnAllResponse\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"]\n\x18\x44\x65viceGetWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05\x63lear\x18\x04 \x01(\x08\"*\n\x19\x44\x65viceGetWarningsResponse\x12\r\n\x05\x66lags\x18\x01 \x03(\t\"x\n\x1aWaitToClearWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07timeout\x18\x04 \x01(\x01\x12\x15\n\rwarning_flags\x18\x05 \x03(\t\"Z\n\x1c\x44\x65viceGetAllDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\"/\n\x1d\x44\x65viceGetAllDigitalIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x08\"Y\n\x1b\x44\x65viceGetAllAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\".\n\x1c\x44\x65viceGetAllAnalogIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"o\n\x19\x44\x65viceGetDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"n\n\x18\x44\x65viceGetAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"Y\n!DeviceSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x08\"X\n DeviceSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x01\"l\n\x1d\x44\x65viceSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x08\"k\n\x1c\x44\x65viceSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\"6\n\x13SetLogOutputRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x05\x12\x11\n\tfile_path\x18\x02 \x01(\t\"l\n\x17\x44\x65viceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x94\x01\n\x1b\x44\x65viceConvertSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\r\n\x05value\x18\x06 \x01(\x01\x12\x13\n\x0b\x66rom_native\x18\x07 \x01(\x08\"{\n\x17\x44\x65viceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"p\n\x1a\x44\x65viceSetSettingStrRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\"\x9e\x01\n\x15PrepareCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x18\n\x10\x63ommand_template\x18\x04 \x01(\t\x12\x37\n\nparameters\x18\x05 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"M\n\x14WaitToRespondRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\"f\n\x15LockstepEnableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x04 \x03(\x05\"r\n\x16LockstepDisableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"\xe1\x02\n\x13LockstepMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12\x42\n\x04type\x18\x05 \x01(\x0e\x32\x34.zaber.motion.protobufs.LockstepMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x08 \x01(\t\x12\x10\n\x08velocity\x18\t \x01(\x01\x12\x15\n\rvelocity_unit\x18\n \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\x0b \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0c \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"}\n\x1cLockstepWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"W\n\x14LockstepEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\"N\n\x0cLockstepAxes\x12\x0e\n\x06\x61xis_1\x18\x01 \x01(\x05\x12\x0e\n\x06\x61xis_2\x18\x02 \x01(\x05\x12\x0e\n\x06\x61xis_3\x18\x03 \x01(\x05\x12\x0e\n\x06\x61xis_4\x18\x04 \x01(\x05\".\n\x1eLockstepGetAxisNumbersResponse\x12\x0c\n\x04\x61xes\x18\x01 \x03(\x05\"c\n\x12LockstepGetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\x86\x01\n\x12LockstepSetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\x12\n\naxis_index\x18\x06 \x01(\x05\"d\n\x1dOscilloscopeAddChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\"k\n\x1cOscilloscopeStartStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\r\n\x05start\x18\x03 \x01(\x08\x12\x16\n\x0e\x63\x61pture_length\x18\x04 \x01(\x05\",\n\x18OscilloscopeReadResponse\x12\x10\n\x08\x64\x61ta_ids\x18\x01 \x03(\x05\"-\n\x1aOscilloscopeDataIdentifier\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\"E\n\x1dOscilloscopeCaptureProperties\x12\x0f\n\x07setting\x18\x01 \x01(\t\x12\x13\n\x0b\x61xis_number\x18\x02 \x01(\x05\";\n\x1aOscilloscopeDataGetRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\"T\n$OscilloscopeDataGetSampleTimeRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\"2\n\"OscilloscopeDataGetSamplesResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x01\"l\n\x16StreamSetupLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04\x61xes\x18\x05 \x03(\x05\"\xa3\x01\n\x1fStreamSetupLiveCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04\x61xes\x18\x05 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\x98\x01\n\x17StreamSetupStoreRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x07 \x03(\x05\"\xcf\x01\n StreamSetupStoreCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12:\n\x04\x61xes\x18\x07 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\xab\x01\n$StreamSetupStoreArbitraryAxesRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x12\n\naxes_count\x18\x07 \x01(\x05\"\x84\x01\n\x11StreamCallRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\"\xd1\x02\n\x0fPvtPointRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04type\x18\x05 \x01(\x0e\x32,.zaber.motion.protobufs.PvtPointRequest.Type\x12\x36\n\tpositions\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x37\n\nvelocities\x18\x07 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x31\n\x04time\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x85\x02\n\x11StreamLineRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12<\n\x04type\x18\x05 \x01(\x0e\x32..zaber.motion.protobufs.StreamLineRequest.Type\x12\x35\n\x08\x65ndpoint\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x07 \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xbe\x03\n\x10StreamArcRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12;\n\x04type\x18\x05 \x01(\x0e\x32-.zaber.motion.protobufs.StreamArcRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_x\x18\t \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_y\x18\n \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x0b \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xdc\x02\n\x13StreamCircleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12>\n\x04type\x18\x05 \x01(\x0e\x32\x30.zaber.motion.protobufs.StreamCircleRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\t \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x8c\x01\n\x1dStreamWaitDigitalInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x9e\x01\n\x1cStreamWaitAnalogInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\x11\n\tcondition\x18\x06 \x01(\t\x12\r\n\x05value\x18\x07 \x01(\x01\"\x8c\x01\n\x1dStreamSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x8b\x01\n\x1cStreamSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x01\"\x80\x01\n StreamToggleDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\"y\n!StreamSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x08\"x\n StreamSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x01\"u\n\x11StreamWaitRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04time\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n\x1aStreamWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x1c\n\x14throw_error_on_fault\x18\x05 \x01(\x08\"Z\n\x12StreamEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"S\n\x15StreamGetAxesResponse\x12:\n\x04\x61xes\x18\x01 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"n\n\x18StreamGetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x81\x01\n\x18StreamSetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x05 \x01(\x08\x12\x11\n\tmax_speed\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\"\x7f\n)StreamGetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa4\x01\n)StreamSetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12#\n\x1bmax_tangential_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n*StreamGetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa6\x01\n*StreamSetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12$\n\x1cmax_centripetal_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"e\n\x1dStreamBufferGetContentRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"6\n\x1eStreamBufferGetContentResponse\x12\x14\n\x0c\x62uffer_lines\x18\x01 \x03(\t\"`\n\x18StreamBufferEraseRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"t\n\x1bStreamGenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0f\n\x07\x63ommand\x18\x05 \x01(\t\"w\n StreamGenericCommandBatchRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\r\n\x05\x62\x61tch\x18\x05 \x03(\t\"c\n\x14\x42inaryReplyOnlyEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\xbb\x01\n\x1aOpenBinaryInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x17\n\x0fuse_message_ids\x18\x06 \x01(\x08\"i\n\x1aUnknownBinaryResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\x82\x01\n\x14GenericBinaryRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x01\"F\n\rBinaryMessage\x12\x16\n\x0e\x64\x65vice_address\x18\x01 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x02 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x05\"R\n\x17\x42inaryMessageCollection\x12\x37\n\x08messages\x18\x02 \x03(\x0b\x32%.zaber.motion.protobufs.BinaryMessage\":\n\x12\x44\x65viceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\"\xd9\x02\n\x14\x42inaryDeviceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x15\n\ris_peripheral\x18\x06 \x01(\x08\x12\x15\n\rperipheral_id\x18\x07 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x08 \x01(\t\x12L\n\x0b\x64\x65vice_type\x18\t \x01(\x0e\x32\x37.zaber.motion.protobufs.BinaryDeviceIdentity.DeviceType\"1\n\nDeviceType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\x99\x01\n\x1d\x42inaryGenericWithUnitsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x01\x12\x11\n\tfrom_unit\x18\x05 \x01(\t\x12\x0f\n\x07to_unit\x18\x06 \x01(\t\x12\x0f\n\x07timeout\x18\x07 \x01(\x01\"^\n\x17\x42inaryDeviceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\xda\x01\n\x17\x42inaryDeviceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x46\n\x04type\x18\x04 \x01(\x0e\x32\x38.zaber.motion.protobufs.BinaryDeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"%\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\"^\n\x17\x42inaryDeviceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"K\n\x19\x42inaryDeviceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"-\n\x1a\x42inaryDeviceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"d\n\x1d\x42inaryDeviceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"s\n\x1d\x42inaryDeviceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"2\n\x1a\x43ustomInterfaceReadRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"D\n\x1b\x43ustomInterfaceWriteRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"3\n\x1b\x43ustomInterfaceOpenResponse\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"J\n\x1b\x43ustomInterfaceCloseRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"W\n\x12\x43\x61nSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\"=\n\x17\x43\x61nSetStateAxisResponse\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"p\n\x19\x43\x61nSetStateDeviceResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x44\n\x0b\x61xis_errors\x18\x02 \x03(\x0b\x32/.zaber.motion.protobufs.CanSetStateAxisResponse\"i\n\x0fSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65vice_only\x18\x05 \x01(\x08\"Z\n\x12ServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\"/\n\x10ServoTuningParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"g\n\x0cParamsetInfo\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x05\x12\x38\n\x06params\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"\x9e\x01\n\x15SetServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12?\n\rtuning_params\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"n\n\x0cLoadParamset\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x13\n\x0bto_paramset\x18\x04 \x01(\x05\x12\x15\n\rfrom_paramset\x18\x05 \x01(\x05\"\x8d\x01\n\x18SetServoTuningPIDRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\t\n\x01p\x18\x05 \x01(\x01\x12\t\n\x01i\x18\x06 \x01(\x01\x12\t\n\x01\x64\x18\x07 \x01(\x01\x12\n\n\x02\x66\x63\x18\x08 \x01(\x01\"W\n\tPidTuning\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\t\n\x01p\x18\x03 \x01(\x01\x12\t\n\x01i\x18\x04 \x01(\x01\x12\t\n\x01\x64\x18\x05 \x01(\x01\x12\n\n\x02\x66\x63\x18\x06 \x01(\x01\"\xc2\x01\n\x0fSetSimpleTuning\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\x15\n\rcarriage_mass\x18\x05 \x01(\x01\x12\x11\n\tload_mass\x18\x06 \x01(\x01\x12?\n\rtuning_params\x18\x07 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"d\n\x1bSimpleTuningParamDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tmin_label\x18\x02 \x01(\t\x12\x11\n\tmax_label\x18\x03 \x01(\t\x12\x11\n\tdata_type\x18\x04 \x01(\t\"m\n&GetSimpleTuningParamDefinitionResponse\x12\x43\n\x06params\x18\x01 \x03(\x0b\x32\x33.zaber.motion.protobufs.SimpleTuningParamDefinition\"\x95\x01\n\x17TranslatorCreateRequest\x12@\n\ndefinition\x18\x01 \x01(\x0b\x32,.zaber.motion.protobufs.TranslatorDefinition\x12\x38\n\x06\x63onfig\x18\x02 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"1\n\x18TranslatorCreateResponse\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"O\n\x18TranslatorAxisDefinition\x12\x15\n\rperipheral_id\x18\x01 \x01(\x05\x12\x1c\n\x14microstep_resolution\x18\x02 \x01(\x05\"\xa1\x01\n\x14TranslatorDefinition\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12>\n\x04\x61xes\x18\x02 \x03(\x0b\x32\x30.zaber.motion.protobufs.TranslatorAxisDefinition\x12\x36\n\tmax_speed\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\xac\x01\n\x10TranslatorConfig\x12\x44\n\raxis_mappings\x18\x01 \x03(\x0b\x32-.zaber.motion.protobufs.TranslatorAxisMapping\x12R\n\x14\x61xis_transformations\x18\x02 \x03(\x0b\x32\x34.zaber.motion.protobufs.TranslatorAxisTransformation\"@\n\x15TranslatorAxisMapping\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x12\n\naxis_index\x18\x02 \x01(\x05\"~\n\x1cTranslatorAxisTransformation\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x0f\n\x07scaling\x18\x02 \x01(\x01\x12\x38\n\x0btranslation\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"B\n\x1aTranslatorTranslateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\r\n\x05\x62lock\x18\x02 \x01(\t\"I\n\x10TranslateMessage\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x12\n\nfrom_block\x18\x02 \x01(\x05\x12\x10\n\x08to_block\x18\x03 \x01(\x05\"k\n\x1bTranslatorTranslateResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\x12:\n\x08warnings\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.TranslateMessage\"@\n\x18GCodeSyntaxExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"C\n\x1bGCodeExecutionExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"L\n\x1aTranslatorFlushLiveRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"+\n\x17TranslatorFlushResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\"\x90\x01\n\x1bTranslatorCreateLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"\x91\x01\n!TranslatorCreateFromDeviceRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x03 \x03(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"/\n\x16TranslatorEmptyRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"^\n TranslatorSetTraverseRateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x15\n\rtraverse_rate\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"g\n TranslatorSetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x10\n\x08position\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"U\n TranslatorGetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x0c\n\x04unit\x18\x03 \x01(\t\"n\n\x1eTranslatorGetAxisOffsetRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x19\n\x11\x63oordinate_system\x18\x02 \x01(\t\x12\x0c\n\x04\x61xis\x18\x03 \x01(\t\x12\x0c\n\x04unit\x18\x04 \x01(\t\"R\n$TranslatorSetFeedRateOverrideRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x13\n\x0b\x63oefficient\x18\x02 \x01(\x01\"y\n\x17\x44\x65viceSetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\x12\x0e\n\x06\x65ncode\x18\x06 \x01(\x08\"j\n\x17\x44\x65viceGetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\x0e\n\x06\x64\x65\x63ode\x18\x05 \x01(\x08\"o\n\x1d\x44\x65viceSetStorageNumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\"m\n\x1b\x44\x65viceSetStorageBoolRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x08\"W\n\x14\x44\x65viceStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\"b\n\x1c\x44\x65viceStorageListKeysRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0e\n\x06prefix\x18\x04 \x01(\t\"\xa1\x01\n\x1f\x44\x65viceSetUnitConversionsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12=\n\x0b\x63onversions\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ConversionFactor\"@\n\x10\x43onversionFactor\x12\x0f\n\x07setting\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"^\n\x17ObjectiveChangerRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\"?\n\x1eObjectiveChangerCreateResponse\x12\x0e\n\x06turret\x18\x02 \x01(\x05\x12\r\n\x05\x66ocus\x18\x03 \x01(\x05\"\xb2\x01\n\x1dObjectiveChangerChangeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\x12\x11\n\tobjective\x18\x04 \x01(\x05\x12\x39\n\x0c\x66ocus_offset\x18\x05 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement*-\n\x0bMessageType\x12\t\n\x05REPLY\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\t\n\x05\x41LERT\x10\x02*\xc0\t\n\x06\x45rrors\x12\x13\n\x0fREQUEST_TIMEOUT\x10\x00\x12\x15\n\x11\x43ONNECTION_CLOSED\x10\x01\x12\x14\n\x10INVALID_ARGUMENT\x10\x02\x12\x16\n\x12OUT_OF_REQUEST_IDS\x10\x03\x12\x12\n\x0eINVALID_PACKET\x10\x04\x12\x15\n\x11\x43ONNECTION_FAILED\x10\x05\x12\x13\n\x0fUNKNOWN_REQUEST\x10\x06\x12\x12\n\x0e\x43OMMAND_FAILED\x10\x07\x12\x14\n\x10\x44\x45VICE_DB_FAILED\x10\x08\x12\x10\n\x0cINVALID_DATA\x10\t\x12\x19\n\x15\x44\x45VICE_NOT_IDENTIFIED\x10\n\x12\x15\n\x11\x43ONVERSION_FAILED\x10\x0b\x12\x1b\n\x17\x44\x45VICE_ADDRESS_CONFLICT\x10\x0c\x12\x13\n\x0fNO_DEVICE_FOUND\x10\r\x12\x18\n\x14MOVEMENT_INTERRUPTED\x10\x0e\x12\x13\n\x0fMOVEMENT_FAILED\x10\x0f\x12\r\n\tIO_FAILED\x10\x10\x12\x14\n\x10INVALID_RESPONSE\x10\x11\x12\x11\n\rNOT_SUPPORTED\x10\x12\x12\x11\n\rDEVICE_FAILED\x10\x13\x12\r\n\tOS_FAILED\x10\x14\x12\x12\n\x0eINTERNAL_ERROR\x10\x16\x12\x19\n\x15\x42INARY_COMMAND_FAILED\x10\x18\x12\x15\n\x11\x43OMMAND_PREEMPTED\x10\x19\x12\x18\n\x14LOCKSTEP_NOT_ENABLED\x10\x1a\x12\x14\n\x10LOCKSTEP_ENABLED\x10\x1b\x12\x1b\n\x17IO_CHANNEL_OUT_OF_RANGE\x10\x1c\x12\x15\n\x11SETTING_NOT_FOUND\x10\x1d\x12\x0f\n\x0bSTREAM_MODE\x10\x1e\x12\x14\n\x10STREAM_EXECUTION\x10\x1f\x12\x1a\n\x16STREAM_MOVEMENT_FAILED\x10 \x12\x17\n\x13STREAM_SETUP_FAILED\x10!\x12\x0f\n\x0b\x44\x45VICE_BUSY\x10\"\x12\x1f\n\x1bSTREAM_MOVEMENT_INTERRUPTED\x10#\x12\x16\n\x12INVALID_PARK_STATE\x10$\x12\x14\n\x10SERIAL_PORT_BUSY\x10%\x12\x1a\n\x16TRANSPORT_ALREADY_USED\x10&\x12\x1f\n\x1bSET_PERIPHERAL_STATE_FAILED\x10\'\x12\x1b\n\x17SET_DEVICE_STATE_FAILED\x10(\x12\x11\n\rG_CODE_SYNTAX\x10)\x12\x14\n\x10G_CODE_EXECUTION\x10*\x12\x15\n\x11INVALID_OPERATION\x10+\x12\x14\n\x10\x43OMMAND_TOO_LONG\x10,\x12\x14\n\x10NO_VALUE_FOR_KEY\x10-\x12\x1b\n\x17\x44\x45VICE_DETECTION_FAILED\x10.\x12\x0b\n\x07TIMEOUT\x10/\x12\x0c\n\x08PVT_MODE\x10\x30\x12\x11\n\rPVT_EXECUTION\x10\x31\x12\x14\n\x10PVT_SETUP_FAILED\x10\x32\x12\x17\n\x13PVT_MOVEMENT_FAILED\x10\x33\x12\x1c\n\x18PVT_MOVEMENT_INTERRUPTED\x10\x34\x12\x15\n\x11PVT_DISCONTINUITY\x10\x35\x12\x18\n\x14STREAM_DISCONTINUITY\x10\x36*Q\n\rInterfaceType\x12\x0f\n\x0bSERIAL_PORT\x10\x00\x12\x07\n\x03TCP\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\x12\x07\n\x03IOT\x10\x03\x12\x11\n\rNETWORK_SHARE\x10\x04\x42$Z\"./protobufs;zaber_motion_protobufsb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protobufs.main_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\"./protobufs;zaber_motion_protobufs'
-  _MESSAGETYPE._serialized_start=20920
-  _MESSAGETYPE._serialized_end=20965
-  _ERRORS._serialized_start=20968
-  _ERRORS._serialized_end=22025
-  _INTERFACETYPE._serialized_start=22027
-  _INTERFACETYPE._serialized_end=22108
+  _MESSAGETYPE._serialized_start=22047
+  _MESSAGETYPE._serialized_end=22092
+  _ERRORS._serialized_start=22095
+  _ERRORS._serialized_end=23311
+  _INTERFACETYPE._serialized_start=23313
+  _INTERFACETYPE._serialized_end=23394
   _REQUEST._serialized_start=48
   _REQUEST._serialized_end=74
   _RESPONSE._serialized_start=77
   _RESPONSE._serialized_end=262
   _RESPONSE_RESPONSETYPE._serialized_start=229
   _RESPONSE_RESPONSETYPE._serialized_end=262
   _EVENT._serialized_start=264
@@ -67,376 +67,388 @@
   _INVALIDPACKETEXCEPTIONDATA._serialized_end=1312
   _DEVICEADDRESSCONFLICTEXCEPTIONDATA._serialized_start=1314
   _DEVICEADDRESSCONFLICTEXCEPTIONDATA._serialized_end=1376
   _MOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_start=1378
   _MOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_end=1476
   _STREAMMOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_start=1478
   _STREAMMOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_end=1552
-  _MOVEMENTFAILEDEXCEPTIONDATA._serialized_start=1554
-  _MOVEMENTFAILEDEXCEPTIONDATA._serialized_end=1647
-  _STREAMMOVEMENTFAILEDEXCEPTIONDATA._serialized_start=1649
-  _STREAMMOVEMENTFAILEDEXCEPTIONDATA._serialized_end=1718
-  _STREAMEXECUTIONEXCEPTIONDATA._serialized_start=1720
-  _STREAMEXECUTIONEXCEPTIONDATA._serialized_end=1786
-  _INVALIDRESPONSEEXCEPTIONDATA._serialized_start=1788
-  _INVALIDRESPONSEEXCEPTIONDATA._serialized_end=1836
-  _COMMANDFAILEDEXCEPTIONDATA._serialized_start=1838
-  _COMMANDFAILEDEXCEPTIONDATA._serialized_end=1947
-  _BINARYCOMMANDFAILEDEXCEPTIONDATA._serialized_start=1949
-  _BINARYCOMMANDFAILEDEXCEPTIONDATA._serialized_end=2006
-  _SETPERIPHERALSTATEEXCEPTIONDATA._serialized_start=2009
-  _SETPERIPHERALSTATEEXCEPTIONDATA._serialized_end=2146
-  _SETDEVICESTATEEXCEPTIONDATA._serialized_start=2149
-  _SETDEVICESTATEEXCEPTIONDATA._serialized_end=2381
-  _COMMANDTOOLONGEXCEPTIONDATA._serialized_start=2383
-  _COMMANDTOOLONGEXCEPTIONDATA._serialized_end=2486
-  _TESTREQUEST._serialized_start=2488
-  _TESTREQUEST._serialized_end=2574
-  _TESTRESPONSE._serialized_start=2576
-  _TESTRESPONSE._serialized_end=2609
-  _TESTRESPONSELONG._serialized_start=2611
-  _TESTRESPONSELONG._serialized_end=2648
-  _TESTEVENT._serialized_start=2650
-  _TESTEVENT._serialized_end=2675
-  _TOOLSLISTSERIALPORTSRESPONSE._serialized_start=2677
-  _TOOLSLISTSERIALPORTSRESPONSE._serialized_end=2722
-  _SETINTERNALMODEREQUEST._serialized_start=2724
-  _SETINTERNALMODEREQUEST._serialized_end=2762
-  _SETDEVICEDBSOURCEREQUEST._serialized_start=2764
-  _SETDEVICEDBSOURCEREQUEST._serialized_end=2837
-  _TOGGLEDEVICEDBSTOREREQUEST._serialized_start=2839
-  _TOGGLEDEVICEDBSTOREREQUEST._serialized_end=2910
-  _DEVICEDBFAILEDEXCEPTIONDATA._serialized_start=2912
-  _DEVICEDBFAILEDEXCEPTIONDATA._serialized_end=2955
-  _OPENINTERFACEREQUEST._serialized_start=2958
-  _OPENINTERFACEREQUEST._serialized_end=3253
-  _OPENINTERFACERESPONSE._serialized_start=3255
-  _OPENINTERFACERESPONSE._serialized_end=3300
-  _INTERFACEEMPTYREQUEST._serialized_start=3302
-  _INTERFACEEMPTYREQUEST._serialized_end=3347
-  _SETINTERFACETIMEOUTREQUEST._serialized_start=3349
-  _SETINTERFACETIMEOUTREQUEST._serialized_end=3416
-  _SETINTERFACECHECKSUMENABLEDREQUEST._serialized_start=3418
-  _SETINTERFACECHECKSUMENABLEDREQUEST._serialized_end=3496
-  _AXISEMPTYREQUEST._serialized_start=3498
-  _AXISEMPTYREQUEST._serialized_end=3568
-  _GENERICCOMMANDREQUEST._serialized_start=3571
-  _GENERICCOMMANDREQUEST._serialized_end=3702
-  _GENERICCOMMANDRESPONSE._serialized_start=3705
-  _GENERICCOMMANDRESPONSE._serialized_end=3905
-  _GENERICCOMMANDRESPONSECOLLECTION._serialized_start=3907
-  _GENERICCOMMANDRESPONSECOLLECTION._serialized_end=4008
-  _UNKNOWNRESPONSEEVENT._serialized_start=4011
-  _UNKNOWNRESPONSEEVENT._serialized_end=4231
-  _ALERTEVENT._serialized_start=4234
-  _ALERTEVENT._serialized_end=4365
-  _DISCONNECTEDEVENT._serialized_start=4367
-  _DISCONNECTEDEVENT._serialized_end=4483
-  _DEVICEIDENTIFYREQUEST._serialized_start=4485
-  _DEVICEIDENTIFYREQUEST._serialized_end=4611
-  _DEVICERENUMBERREQUEST._serialized_start=4613
-  _DEVICERENUMBERREQUEST._serialized_end=4681
-  _DEVICEDETECTREQUEST._serialized_start=4683
-  _DEVICEDETECTREQUEST._serialized_end=4752
-  _DEVICEDETECTRESPONSE._serialized_start=4754
-  _DEVICEDETECTRESPONSE._serialized_end=4793
-  _DEVICEHOMEREQUEST._serialized_start=4795
-  _DEVICEHOMEREQUEST._serialized_end=4891
-  _DEVICEWAITUNTILIDLEREQUEST._serialized_start=4893
-  _DEVICEWAITUNTILIDLEREQUEST._serialized_end=5003
-  _DEVICEMOVEREQUEST._serialized_start=5006
-  _DEVICEMOVEREQUEST._serialized_end=5342
-  _DEVICEMOVEREQUEST_MOVETYPE._serialized_start=5287
-  _DEVICEMOVEREQUEST_MOVETYPE._serialized_end=5342
-  _DEVICESTOPREQUEST._serialized_start=5344
-  _DEVICESTOPREQUEST._serialized_end=5440
-  _DEVICEONALLREQUEST._serialized_start=5442
-  _DEVICEONALLREQUEST._serialized_end=5509
-  _DEVICEONALLRESPONSE._serialized_start=5511
-  _DEVICEONALLRESPONSE._serialized_end=5558
-  _DEVICEGETWARNINGSREQUEST._serialized_start=5560
-  _DEVICEGETWARNINGSREQUEST._serialized_end=5653
-  _DEVICEGETWARNINGSRESPONSE._serialized_start=5655
-  _DEVICEGETWARNINGSRESPONSE._serialized_end=5697
-  _WAITTOCLEARWARNINGSREQUEST._serialized_start=5699
-  _WAITTOCLEARWARNINGSREQUEST._serialized_end=5819
-  _DEVICEGETALLDIGITALIOREQUEST._serialized_start=5821
-  _DEVICEGETALLDIGITALIOREQUEST._serialized_end=5911
-  _DEVICEGETALLDIGITALIORESPONSE._serialized_start=5913
-  _DEVICEGETALLDIGITALIORESPONSE._serialized_end=5960
-  _DEVICEGETALLANALOGIOREQUEST._serialized_start=5962
-  _DEVICEGETALLANALOGIOREQUEST._serialized_end=6051
-  _DEVICEGETALLANALOGIORESPONSE._serialized_start=6053
-  _DEVICEGETALLANALOGIORESPONSE._serialized_end=6099
-  _DEVICEGETDIGITALIOREQUEST._serialized_start=6101
-  _DEVICEGETDIGITALIOREQUEST._serialized_end=6212
-  _DEVICEGETANALOGIOREQUEST._serialized_start=6214
-  _DEVICEGETANALOGIOREQUEST._serialized_end=6324
-  _DEVICESETALLDIGITALOUTPUTSREQUEST._serialized_start=6326
-  _DEVICESETALLDIGITALOUTPUTSREQUEST._serialized_end=6415
-  _DEVICESETALLANALOGOUTPUTSREQUEST._serialized_start=6417
-  _DEVICESETALLANALOGOUTPUTSREQUEST._serialized_end=6505
-  _DEVICESETDIGITALOUTPUTREQUEST._serialized_start=6507
-  _DEVICESETDIGITALOUTPUTREQUEST._serialized_end=6615
-  _DEVICESETANALOGOUTPUTREQUEST._serialized_start=6617
-  _DEVICESETANALOGOUTPUTREQUEST._serialized_end=6724
-  _SETLOGOUTPUTREQUEST._serialized_start=6726
-  _SETLOGOUTPUTREQUEST._serialized_end=6780
-  _DEVICEGETSETTINGREQUEST._serialized_start=6782
-  _DEVICEGETSETTINGREQUEST._serialized_end=6890
-  _DEVICECONVERTSETTINGREQUEST._serialized_start=6893
-  _DEVICECONVERTSETTINGREQUEST._serialized_end=7041
-  _DEVICESETSETTINGREQUEST._serialized_start=7043
-  _DEVICESETSETTINGREQUEST._serialized_end=7166
-  _DEVICESETSETTINGSTRREQUEST._serialized_start=7168
-  _DEVICESETSETTINGSTRREQUEST._serialized_end=7280
-  _PREPARECOMMANDREQUEST._serialized_start=7283
-  _PREPARECOMMANDREQUEST._serialized_end=7441
-  _WAITTORESPONDREQUEST._serialized_start=7443
-  _WAITTORESPONDREQUEST._serialized_end=7520
-  _LOCKSTEPENABLEREQUEST._serialized_start=7522
-  _LOCKSTEPENABLEREQUEST._serialized_end=7624
-  _LOCKSTEPDISABLEREQUEST._serialized_start=7626
-  _LOCKSTEPDISABLEREQUEST._serialized_end=7740
-  _LOCKSTEPSTOPREQUEST._serialized_start=7742
-  _LOCKSTEPSTOPREQUEST._serialized_end=7853
-  _LOCKSTEPHOMEREQUEST._serialized_start=7855
-  _LOCKSTEPHOMEREQUEST._serialized_end=7966
-  _LOCKSTEPMOVEREQUEST._serialized_start=7969
-  _LOCKSTEPMOVEREQUEST._serialized_end=8322
-  _LOCKSTEPMOVEREQUEST_MOVETYPE._serialized_start=5287
-  _LOCKSTEPMOVEREQUEST_MOVETYPE._serialized_end=5342
-  _LOCKSTEPWAITUNTILIDLEREQUEST._serialized_start=8324
-  _LOCKSTEPWAITUNTILIDLEREQUEST._serialized_end=8449
-  _LOCKSTEPEMPTYREQUEST._serialized_start=8451
-  _LOCKSTEPEMPTYREQUEST._serialized_end=8538
-  _LOCKSTEPAXES._serialized_start=8540
-  _LOCKSTEPAXES._serialized_end=8618
-  _LOCKSTEPGETAXISNUMBERSRESPONSE._serialized_start=8620
-  _LOCKSTEPGETAXISNUMBERSRESPONSE._serialized_end=8666
-  _LOCKSTEPGETREQUEST._serialized_start=8668
-  _LOCKSTEPGETREQUEST._serialized_end=8767
-  _LOCKSTEPSETREQUEST._serialized_start=8770
-  _LOCKSTEPSETREQUEST._serialized_end=8904
-  _OSCILLOSCOPEADDCHANNELREQUEST._serialized_start=8906
-  _OSCILLOSCOPEADDCHANNELREQUEST._serialized_end=9006
-  _OSCILLOSCOPESTARTSTOPREQUEST._serialized_start=9008
-  _OSCILLOSCOPESTARTSTOPREQUEST._serialized_end=9115
-  _OSCILLOSCOPEREADRESPONSE._serialized_start=9117
-  _OSCILLOSCOPEREADRESPONSE._serialized_end=9161
-  _OSCILLOSCOPEDATAIDENTIFIER._serialized_start=9163
-  _OSCILLOSCOPEDATAIDENTIFIER._serialized_end=9208
-  _OSCILLOSCOPECAPTUREPROPERTIES._serialized_start=9210
-  _OSCILLOSCOPECAPTUREPROPERTIES._serialized_end=9279
-  _OSCILLOSCOPEDATAGETREQUEST._serialized_start=9281
-  _OSCILLOSCOPEDATAGETREQUEST._serialized_end=9340
-  _OSCILLOSCOPEDATAGETSAMPLETIMEREQUEST._serialized_start=9342
-  _OSCILLOSCOPEDATAGETSAMPLETIMEREQUEST._serialized_end=9426
-  _OSCILLOSCOPEDATAGETSAMPLESRESPONSE._serialized_start=9428
-  _OSCILLOSCOPEDATAGETSAMPLESRESPONSE._serialized_end=9478
-  _STREAMSETUPLIVEREQUEST._serialized_start=9480
-  _STREAMSETUPLIVEREQUEST._serialized_end=9575
-  _STREAMSETUPLIVECOMPOSITEREQUEST._serialized_start=9578
-  _STREAMSETUPLIVECOMPOSITEREQUEST._serialized_end=9728
-  _STREAMSETUPSTOREREQUEST._serialized_start=9730
-  _STREAMSETUPSTOREREQUEST._serialized_end=9849
-  _STREAMSETUPSTORECOMPOSITEREQUEST._serialized_start=9852
-  _STREAMSETUPSTORECOMPOSITEREQUEST._serialized_end=10026
-  _STREAMSETUPSTOREARBITRARYAXESREQUEST._serialized_start=10029
-  _STREAMSETUPSTOREARBITRARYAXESREQUEST._serialized_end=10167
-  _STREAMCALLREQUEST._serialized_start=10169
-  _STREAMCALLREQUEST._serialized_end=10268
-  _STREAMLINEREQUEST._serialized_start=10271
-  _STREAMLINEREQUEST._serialized_end=10519
-  _STREAMLINEREQUEST_TYPE._serialized_start=10495
-  _STREAMLINEREQUEST_TYPE._serialized_end=10519
-  _STREAMARCREQUEST._serialized_start=10522
-  _STREAMARCREQUEST._serialized_end=10955
-  _STREAMARCREQUEST_TYPE._serialized_start=10495
-  _STREAMARCREQUEST_TYPE._serialized_end=10519
-  _STREAMCIRCLEREQUEST._serialized_start=10958
-  _STREAMCIRCLEREQUEST._serialized_end=11293
-  _STREAMCIRCLEREQUEST_TYPE._serialized_start=10495
-  _STREAMCIRCLEREQUEST_TYPE._serialized_end=10519
-  _STREAMWAITDIGITALINPUTREQUEST._serialized_start=11295
-  _STREAMWAITDIGITALINPUTREQUEST._serialized_end=11422
-  _STREAMWAITANALOGINPUTREQUEST._serialized_start=11425
-  _STREAMWAITANALOGINPUTREQUEST._serialized_end=11570
-  _STREAMSETDIGITALOUTPUTREQUEST._serialized_start=11572
-  _STREAMSETDIGITALOUTPUTREQUEST._serialized_end=11699
-  _STREAMSETANALOGOUTPUTREQUEST._serialized_start=11701
-  _STREAMSETANALOGOUTPUTREQUEST._serialized_end=11827
-  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_start=11829
-  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_end=11944
-  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_start=11946
-  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_end=12054
-  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_start=12056
-  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_end=12163
-  _STREAMWAITREQUEST._serialized_start=12165
-  _STREAMWAITREQUEST._serialized_end=12269
-  _STREAMWAITUNTILIDLEREQUEST._serialized_start=12271
-  _STREAMWAITUNTILIDLEREQUEST._serialized_end=12386
-  _STREAMEMPTYREQUEST._serialized_start=12388
-  _STREAMEMPTYREQUEST._serialized_end=12465
-  _STREAMGETAXESRESPONSE._serialized_start=12467
-  _STREAMGETAXESRESPONSE._serialized_end=12550
-  _STREAMGETMAXSPEEDREQUEST._serialized_start=12552
-  _STREAMGETMAXSPEEDREQUEST._serialized_end=12649
-  _STREAMSETMAXSPEEDREQUEST._serialized_start=12651
-  _STREAMSETMAXSPEEDREQUEST._serialized_end=12767
-  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=12769
-  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=12883
-  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=12886
-  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=13037
-  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=13039
-  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=13154
-  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=13157
-  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=13310
-  _STREAMBUFFERGETCONTENTREQUEST._serialized_start=13312
-  _STREAMBUFFERGETCONTENTREQUEST._serialized_end=13400
-  _STREAMBUFFERGETCONTENTRESPONSE._serialized_start=13402
-  _STREAMBUFFERGETCONTENTRESPONSE._serialized_end=13456
-  _STREAMBUFFERERASEREQUEST._serialized_start=13458
-  _STREAMBUFFERERASEREQUEST._serialized_end=13541
-  _STREAMGENERICCOMMANDREQUEST._serialized_start=13543
-  _STREAMGENERICCOMMANDREQUEST._serialized_end=13646
-  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_start=13648
-  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_end=13754
-  _BINARYREPLYONLYEVENT._serialized_start=13756
-  _BINARYREPLYONLYEVENT._serialized_end=13855
-  _OPENBINARYINTERFACEREQUEST._serialized_start=13858
-  _OPENBINARYINTERFACEREQUEST._serialized_end=14045
-  _UNKNOWNBINARYRESPONSEEVENT._serialized_start=14047
-  _UNKNOWNBINARYRESPONSEEVENT._serialized_end=14152
-  _GENERICBINARYREQUEST._serialized_start=14155
-  _GENERICBINARYREQUEST._serialized_end=14285
-  _BINARYMESSAGE._serialized_start=14287
-  _BINARYMESSAGE._serialized_end=14357
-  _BINARYMESSAGECOLLECTION._serialized_start=14359
-  _BINARYMESSAGECOLLECTION._serialized_end=14441
-  _DEVICEEMPTYREQUEST._serialized_start=14443
-  _DEVICEEMPTYREQUEST._serialized_end=14501
-  _BINARYDEVICEIDENTITY._serialized_start=14504
-  _BINARYDEVICEIDENTITY._serialized_end=14849
-  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_start=14800
-  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_end=14849
-  _BINARYGENERICWITHUNITSREQUEST._serialized_start=14852
-  _BINARYGENERICWITHUNITSREQUEST._serialized_end=15005
-  _BINARYDEVICEHOMEREQUEST._serialized_start=15007
-  _BINARYDEVICEHOMEREQUEST._serialized_end=15101
-  _BINARYDEVICEMOVEREQUEST._serialized_start=15104
-  _BINARYDEVICEMOVEREQUEST._serialized_end=15322
-  _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_start=5287
-  _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_end=5324
-  _BINARYDEVICESTOPREQUEST._serialized_start=15324
-  _BINARYDEVICESTOPREQUEST._serialized_end=15418
-  _BINARYDEVICEDETECTREQUEST._serialized_start=15420
-  _BINARYDEVICEDETECTREQUEST._serialized_end=15495
-  _BINARYDEVICEDETECTRESPONSE._serialized_start=15497
-  _BINARYDEVICEDETECTRESPONSE._serialized_end=15542
-  _BINARYDEVICEGETSETTINGREQUEST._serialized_start=15544
-  _BINARYDEVICEGETSETTINGREQUEST._serialized_end=15644
-  _BINARYDEVICESETSETTINGREQUEST._serialized_start=15646
-  _BINARYDEVICESETSETTINGREQUEST._serialized_end=15761
-  _CUSTOMINTERFACEREADREQUEST._serialized_start=15763
-  _CUSTOMINTERFACEREADREQUEST._serialized_end=15813
-  _CUSTOMINTERFACEWRITEREQUEST._serialized_start=15815
-  _CUSTOMINTERFACEWRITEREQUEST._serialized_end=15883
-  _CUSTOMINTERFACEOPENRESPONSE._serialized_start=15885
-  _CUSTOMINTERFACEOPENRESPONSE._serialized_end=15936
-  _CUSTOMINTERFACECLOSEREQUEST._serialized_start=15938
-  _CUSTOMINTERFACECLOSEREQUEST._serialized_end=16012
-  _CANSETSTATEREQUEST._serialized_start=16014
-  _CANSETSTATEREQUEST._serialized_end=16101
-  _CANSETSTATEAXISRESPONSE._serialized_start=16103
-  _CANSETSTATEAXISRESPONSE._serialized_end=16164
-  _CANSETSTATEDEVICERESPONSE._serialized_start=16166
-  _CANSETSTATEDEVICERESPONSE._serialized_end=16278
-  _SETSTATEREQUEST._serialized_start=16280
-  _SETSTATEREQUEST._serialized_end=16385
-  _SERVOTUNINGREQUEST._serialized_start=16387
-  _SERVOTUNINGREQUEST._serialized_end=16477
-  _SERVOTUNINGPARAM._serialized_start=16479
-  _SERVOTUNINGPARAM._serialized_end=16526
-  _PARAMSETINFO._serialized_start=16528
-  _PARAMSETINFO._serialized_end=16631
-  _SETSERVOTUNINGREQUEST._serialized_start=16634
-  _SETSERVOTUNINGREQUEST._serialized_end=16792
-  _LOADPARAMSET._serialized_start=16794
-  _LOADPARAMSET._serialized_end=16904
-  _SETSERVOTUNINGPIDREQUEST._serialized_start=16907
-  _SETSERVOTUNINGPIDREQUEST._serialized_end=17048
-  _PIDTUNING._serialized_start=17050
-  _PIDTUNING._serialized_end=17137
-  _SETSIMPLETUNING._serialized_start=17140
-  _SETSIMPLETUNING._serialized_end=17334
-  _SIMPLETUNINGPARAMDEFINITION._serialized_start=17336
-  _SIMPLETUNINGPARAMDEFINITION._serialized_end=17436
-  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_start=17438
-  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_end=17547
-  _TRANSLATORCREATEREQUEST._serialized_start=17550
-  _TRANSLATORCREATEREQUEST._serialized_end=17699
-  _TRANSLATORCREATERESPONSE._serialized_start=17701
-  _TRANSLATORCREATERESPONSE._serialized_end=17750
-  _TRANSLATORAXISDEFINITION._serialized_start=17752
-  _TRANSLATORAXISDEFINITION._serialized_end=17831
-  _TRANSLATORDEFINITION._serialized_start=17834
-  _TRANSLATORDEFINITION._serialized_end=17995
-  _TRANSLATORCONFIG._serialized_start=17998
-  _TRANSLATORCONFIG._serialized_end=18170
-  _TRANSLATORAXISMAPPING._serialized_start=18172
-  _TRANSLATORAXISMAPPING._serialized_end=18236
-  _TRANSLATORAXISTRANSFORMATION._serialized_start=18238
-  _TRANSLATORAXISTRANSFORMATION._serialized_end=18364
-  _TRANSLATORTRANSLATEREQUEST._serialized_start=18366
-  _TRANSLATORTRANSLATEREQUEST._serialized_end=18432
-  _TRANSLATEMESSAGE._serialized_start=18434
-  _TRANSLATEMESSAGE._serialized_end=18507
-  _TRANSLATORTRANSLATERESPONSE._serialized_start=18509
-  _TRANSLATORTRANSLATERESPONSE._serialized_end=18616
-  _GCODESYNTAXEXCEPTIONDATA._serialized_start=18618
-  _GCODESYNTAXEXCEPTIONDATA._serialized_end=18682
-  _GCODEEXECUTIONEXCEPTIONDATA._serialized_start=18684
-  _GCODEEXECUTIONEXCEPTIONDATA._serialized_end=18751
-  _TRANSLATORFLUSHLIVEREQUEST._serialized_start=18753
-  _TRANSLATORFLUSHLIVEREQUEST._serialized_end=18829
-  _TRANSLATORFLUSHRESPONSE._serialized_start=18831
-  _TRANSLATORFLUSHRESPONSE._serialized_end=18874
-  _TRANSLATORCREATELIVEREQUEST._serialized_start=18877
-  _TRANSLATORCREATELIVEREQUEST._serialized_end=19021
-  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_start=19024
-  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_end=19169
-  _TRANSLATOREMPTYREQUEST._serialized_start=19171
-  _TRANSLATOREMPTYREQUEST._serialized_end=19218
-  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_start=19220
-  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_end=19314
-  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_start=19316
-  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_end=19419
-  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_start=19421
-  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_end=19506
-  _TRANSLATORGETAXISOFFSETREQUEST._serialized_start=19508
-  _TRANSLATORGETAXISOFFSETREQUEST._serialized_end=19618
-  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_start=19620
-  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_end=19702
-  _DEVICESETSTORAGEREQUEST._serialized_start=19704
-  _DEVICESETSTORAGEREQUEST._serialized_end=19825
-  _DEVICEGETSTORAGEREQUEST._serialized_start=19827
-  _DEVICEGETSTORAGEREQUEST._serialized_end=19933
-  _DEVICESETSTORAGENUMBERREQUEST._serialized_start=19935
-  _DEVICESETSTORAGENUMBERREQUEST._serialized_end=20046
-  _DEVICESETSTORAGEBOOLREQUEST._serialized_start=20048
-  _DEVICESETSTORAGEBOOLREQUEST._serialized_end=20157
-  _DEVICESTORAGEREQUEST._serialized_start=20159
-  _DEVICESTORAGEREQUEST._serialized_end=20246
-  _DEVICESTORAGELISTKEYSREQUEST._serialized_start=20248
-  _DEVICESTORAGELISTKEYSREQUEST._serialized_end=20346
-  _DEVICESETUNITCONVERSIONSREQUEST._serialized_start=20349
-  _DEVICESETUNITCONVERSIONSREQUEST._serialized_end=20510
-  _CONVERSIONFACTOR._serialized_start=20512
-  _CONVERSIONFACTOR._serialized_end=20576
-  _OBJECTIVECHANGERREQUEST._serialized_start=20578
-  _OBJECTIVECHANGERREQUEST._serialized_end=20672
-  _OBJECTIVECHANGERCREATERESPONSE._serialized_start=20674
-  _OBJECTIVECHANGERCREATERESPONSE._serialized_end=20737
-  _OBJECTIVECHANGERCHANGEREQUEST._serialized_start=20740
-  _OBJECTIVECHANGERCHANGEREQUEST._serialized_end=20918
+  _PVTMOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_start=1554
+  _PVTMOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_end=1625
+  _MOVEMENTFAILEDEXCEPTIONDATA._serialized_start=1627
+  _MOVEMENTFAILEDEXCEPTIONDATA._serialized_end=1720
+  _STREAMMOVEMENTFAILEDEXCEPTIONDATA._serialized_start=1722
+  _STREAMMOVEMENTFAILEDEXCEPTIONDATA._serialized_end=1791
+  _PVTMOVEMENTFAILEDEXCEPTIONDATA._serialized_start=1793
+  _PVTMOVEMENTFAILEDEXCEPTIONDATA._serialized_end=1859
+  _STREAMEXECUTIONEXCEPTIONDATA._serialized_start=1861
+  _STREAMEXECUTIONEXCEPTIONDATA._serialized_end=1927
+  _PVTEXECUTIONEXCEPTIONDATA._serialized_start=1930
+  _PVTEXECUTIONEXCEPTIONDATA._serialized_end=2058
+  _INVALIDPVTPOINT._serialized_start=2060
+  _INVALIDPVTPOINT._serialized_end=2107
+  _INVALIDRESPONSEEXCEPTIONDATA._serialized_start=2109
+  _INVALIDRESPONSEEXCEPTIONDATA._serialized_end=2157
+  _COMMANDFAILEDEXCEPTIONDATA._serialized_start=2159
+  _COMMANDFAILEDEXCEPTIONDATA._serialized_end=2268
+  _BINARYCOMMANDFAILEDEXCEPTIONDATA._serialized_start=2270
+  _BINARYCOMMANDFAILEDEXCEPTIONDATA._serialized_end=2327
+  _SETPERIPHERALSTATEEXCEPTIONDATA._serialized_start=2330
+  _SETPERIPHERALSTATEEXCEPTIONDATA._serialized_end=2467
+  _SETDEVICESTATEEXCEPTIONDATA._serialized_start=2470
+  _SETDEVICESTATEEXCEPTIONDATA._serialized_end=2702
+  _COMMANDTOOLONGEXCEPTIONDATA._serialized_start=2704
+  _COMMANDTOOLONGEXCEPTIONDATA._serialized_end=2807
+  _TESTREQUEST._serialized_start=2809
+  _TESTREQUEST._serialized_end=2895
+  _TESTRESPONSE._serialized_start=2897
+  _TESTRESPONSE._serialized_end=2930
+  _TESTRESPONSELONG._serialized_start=2932
+  _TESTRESPONSELONG._serialized_end=2969
+  _TESTEVENT._serialized_start=2971
+  _TESTEVENT._serialized_end=2996
+  _TOOLSLISTSERIALPORTSRESPONSE._serialized_start=2998
+  _TOOLSLISTSERIALPORTSRESPONSE._serialized_end=3043
+  _SETINTERNALMODEREQUEST._serialized_start=3045
+  _SETINTERNALMODEREQUEST._serialized_end=3083
+  _SETDEVICEDBSOURCEREQUEST._serialized_start=3085
+  _SETDEVICEDBSOURCEREQUEST._serialized_end=3158
+  _TOGGLEDEVICEDBSTOREREQUEST._serialized_start=3160
+  _TOGGLEDEVICEDBSTOREREQUEST._serialized_end=3231
+  _DEVICEDBFAILEDEXCEPTIONDATA._serialized_start=3233
+  _DEVICEDBFAILEDEXCEPTIONDATA._serialized_end=3276
+  _OPENINTERFACEREQUEST._serialized_start=3279
+  _OPENINTERFACEREQUEST._serialized_end=3574
+  _OPENINTERFACERESPONSE._serialized_start=3576
+  _OPENINTERFACERESPONSE._serialized_end=3621
+  _INTERFACEEMPTYREQUEST._serialized_start=3623
+  _INTERFACEEMPTYREQUEST._serialized_end=3668
+  _SETINTERFACETIMEOUTREQUEST._serialized_start=3670
+  _SETINTERFACETIMEOUTREQUEST._serialized_end=3737
+  _SETINTERFACECHECKSUMENABLEDREQUEST._serialized_start=3739
+  _SETINTERFACECHECKSUMENABLEDREQUEST._serialized_end=3817
+  _AXISEMPTYREQUEST._serialized_start=3819
+  _AXISEMPTYREQUEST._serialized_end=3889
+  _GENERICCOMMANDREQUEST._serialized_start=3892
+  _GENERICCOMMANDREQUEST._serialized_end=4023
+  _GENERICCOMMANDRESPONSE._serialized_start=4026
+  _GENERICCOMMANDRESPONSE._serialized_end=4226
+  _GENERICCOMMANDRESPONSECOLLECTION._serialized_start=4228
+  _GENERICCOMMANDRESPONSECOLLECTION._serialized_end=4329
+  _UNKNOWNRESPONSEEVENT._serialized_start=4332
+  _UNKNOWNRESPONSEEVENT._serialized_end=4552
+  _ALERTEVENT._serialized_start=4555
+  _ALERTEVENT._serialized_end=4686
+  _DISCONNECTEDEVENT._serialized_start=4688
+  _DISCONNECTEDEVENT._serialized_end=4804
+  _DEVICEIDENTIFYREQUEST._serialized_start=4806
+  _DEVICEIDENTIFYREQUEST._serialized_end=4932
+  _DEVICERENUMBERREQUEST._serialized_start=4934
+  _DEVICERENUMBERREQUEST._serialized_end=5002
+  _DEVICEDETECTREQUEST._serialized_start=5004
+  _DEVICEDETECTREQUEST._serialized_end=5073
+  _DEVICEDETECTRESPONSE._serialized_start=5075
+  _DEVICEDETECTRESPONSE._serialized_end=5114
+  _DEVICEHOMEREQUEST._serialized_start=5116
+  _DEVICEHOMEREQUEST._serialized_end=5212
+  _DEVICEWAITUNTILIDLEREQUEST._serialized_start=5214
+  _DEVICEWAITUNTILIDLEREQUEST._serialized_end=5324
+  _DEVICEMOVEREQUEST._serialized_start=5327
+  _DEVICEMOVEREQUEST._serialized_end=5663
+  _DEVICEMOVEREQUEST_MOVETYPE._serialized_start=5608
+  _DEVICEMOVEREQUEST_MOVETYPE._serialized_end=5663
+  _DEVICESTOPREQUEST._serialized_start=5665
+  _DEVICESTOPREQUEST._serialized_end=5761
+  _DEVICEONALLREQUEST._serialized_start=5763
+  _DEVICEONALLREQUEST._serialized_end=5830
+  _DEVICEONALLRESPONSE._serialized_start=5832
+  _DEVICEONALLRESPONSE._serialized_end=5879
+  _DEVICEGETWARNINGSREQUEST._serialized_start=5881
+  _DEVICEGETWARNINGSREQUEST._serialized_end=5974
+  _DEVICEGETWARNINGSRESPONSE._serialized_start=5976
+  _DEVICEGETWARNINGSRESPONSE._serialized_end=6018
+  _WAITTOCLEARWARNINGSREQUEST._serialized_start=6020
+  _WAITTOCLEARWARNINGSREQUEST._serialized_end=6140
+  _DEVICEGETALLDIGITALIOREQUEST._serialized_start=6142
+  _DEVICEGETALLDIGITALIOREQUEST._serialized_end=6232
+  _DEVICEGETALLDIGITALIORESPONSE._serialized_start=6234
+  _DEVICEGETALLDIGITALIORESPONSE._serialized_end=6281
+  _DEVICEGETALLANALOGIOREQUEST._serialized_start=6283
+  _DEVICEGETALLANALOGIOREQUEST._serialized_end=6372
+  _DEVICEGETALLANALOGIORESPONSE._serialized_start=6374
+  _DEVICEGETALLANALOGIORESPONSE._serialized_end=6420
+  _DEVICEGETDIGITALIOREQUEST._serialized_start=6422
+  _DEVICEGETDIGITALIOREQUEST._serialized_end=6533
+  _DEVICEGETANALOGIOREQUEST._serialized_start=6535
+  _DEVICEGETANALOGIOREQUEST._serialized_end=6645
+  _DEVICESETALLDIGITALOUTPUTSREQUEST._serialized_start=6647
+  _DEVICESETALLDIGITALOUTPUTSREQUEST._serialized_end=6736
+  _DEVICESETALLANALOGOUTPUTSREQUEST._serialized_start=6738
+  _DEVICESETALLANALOGOUTPUTSREQUEST._serialized_end=6826
+  _DEVICESETDIGITALOUTPUTREQUEST._serialized_start=6828
+  _DEVICESETDIGITALOUTPUTREQUEST._serialized_end=6936
+  _DEVICESETANALOGOUTPUTREQUEST._serialized_start=6938
+  _DEVICESETANALOGOUTPUTREQUEST._serialized_end=7045
+  _SETLOGOUTPUTREQUEST._serialized_start=7047
+  _SETLOGOUTPUTREQUEST._serialized_end=7101
+  _DEVICEGETSETTINGREQUEST._serialized_start=7103
+  _DEVICEGETSETTINGREQUEST._serialized_end=7211
+  _DEVICECONVERTSETTINGREQUEST._serialized_start=7214
+  _DEVICECONVERTSETTINGREQUEST._serialized_end=7362
+  _DEVICESETSETTINGREQUEST._serialized_start=7364
+  _DEVICESETSETTINGREQUEST._serialized_end=7487
+  _DEVICESETSETTINGSTRREQUEST._serialized_start=7489
+  _DEVICESETSETTINGSTRREQUEST._serialized_end=7601
+  _PREPARECOMMANDREQUEST._serialized_start=7604
+  _PREPARECOMMANDREQUEST._serialized_end=7762
+  _WAITTORESPONDREQUEST._serialized_start=7764
+  _WAITTORESPONDREQUEST._serialized_end=7841
+  _LOCKSTEPENABLEREQUEST._serialized_start=7843
+  _LOCKSTEPENABLEREQUEST._serialized_end=7945
+  _LOCKSTEPDISABLEREQUEST._serialized_start=7947
+  _LOCKSTEPDISABLEREQUEST._serialized_end=8061
+  _LOCKSTEPSTOPREQUEST._serialized_start=8063
+  _LOCKSTEPSTOPREQUEST._serialized_end=8174
+  _LOCKSTEPHOMEREQUEST._serialized_start=8176
+  _LOCKSTEPHOMEREQUEST._serialized_end=8287
+  _LOCKSTEPMOVEREQUEST._serialized_start=8290
+  _LOCKSTEPMOVEREQUEST._serialized_end=8643
+  _LOCKSTEPMOVEREQUEST_MOVETYPE._serialized_start=5608
+  _LOCKSTEPMOVEREQUEST_MOVETYPE._serialized_end=5663
+  _LOCKSTEPWAITUNTILIDLEREQUEST._serialized_start=8645
+  _LOCKSTEPWAITUNTILIDLEREQUEST._serialized_end=8770
+  _LOCKSTEPEMPTYREQUEST._serialized_start=8772
+  _LOCKSTEPEMPTYREQUEST._serialized_end=8859
+  _LOCKSTEPAXES._serialized_start=8861
+  _LOCKSTEPAXES._serialized_end=8939
+  _LOCKSTEPGETAXISNUMBERSRESPONSE._serialized_start=8941
+  _LOCKSTEPGETAXISNUMBERSRESPONSE._serialized_end=8987
+  _LOCKSTEPGETREQUEST._serialized_start=8989
+  _LOCKSTEPGETREQUEST._serialized_end=9088
+  _LOCKSTEPSETREQUEST._serialized_start=9091
+  _LOCKSTEPSETREQUEST._serialized_end=9225
+  _OSCILLOSCOPEADDCHANNELREQUEST._serialized_start=9227
+  _OSCILLOSCOPEADDCHANNELREQUEST._serialized_end=9327
+  _OSCILLOSCOPESTARTSTOPREQUEST._serialized_start=9329
+  _OSCILLOSCOPESTARTSTOPREQUEST._serialized_end=9436
+  _OSCILLOSCOPEREADRESPONSE._serialized_start=9438
+  _OSCILLOSCOPEREADRESPONSE._serialized_end=9482
+  _OSCILLOSCOPEDATAIDENTIFIER._serialized_start=9484
+  _OSCILLOSCOPEDATAIDENTIFIER._serialized_end=9529
+  _OSCILLOSCOPECAPTUREPROPERTIES._serialized_start=9531
+  _OSCILLOSCOPECAPTUREPROPERTIES._serialized_end=9600
+  _OSCILLOSCOPEDATAGETREQUEST._serialized_start=9602
+  _OSCILLOSCOPEDATAGETREQUEST._serialized_end=9661
+  _OSCILLOSCOPEDATAGETSAMPLETIMEREQUEST._serialized_start=9663
+  _OSCILLOSCOPEDATAGETSAMPLETIMEREQUEST._serialized_end=9747
+  _OSCILLOSCOPEDATAGETSAMPLESRESPONSE._serialized_start=9749
+  _OSCILLOSCOPEDATAGETSAMPLESRESPONSE._serialized_end=9799
+  _STREAMSETUPLIVEREQUEST._serialized_start=9801
+  _STREAMSETUPLIVEREQUEST._serialized_end=9909
+  _STREAMSETUPLIVECOMPOSITEREQUEST._serialized_start=9912
+  _STREAMSETUPLIVECOMPOSITEREQUEST._serialized_end=10075
+  _STREAMSETUPSTOREREQUEST._serialized_start=10078
+  _STREAMSETUPSTOREREQUEST._serialized_end=10230
+  _STREAMSETUPSTORECOMPOSITEREQUEST._serialized_start=10233
+  _STREAMSETUPSTORECOMPOSITEREQUEST._serialized_end=10440
+  _STREAMSETUPSTOREARBITRARYAXESREQUEST._serialized_start=10443
+  _STREAMSETUPSTOREARBITRARYAXESREQUEST._serialized_end=10614
+  _STREAMCALLREQUEST._serialized_start=10617
+  _STREAMCALLREQUEST._serialized_end=10749
+  _PVTPOINTREQUEST._serialized_start=10752
+  _PVTPOINTREQUEST._serialized_end=11089
+  _PVTPOINTREQUEST_TYPE._serialized_start=11065
+  _PVTPOINTREQUEST_TYPE._serialized_end=11089
+  _STREAMLINEREQUEST._serialized_start=11092
+  _STREAMLINEREQUEST._serialized_end=11353
+  _STREAMLINEREQUEST_TYPE._serialized_start=11065
+  _STREAMLINEREQUEST_TYPE._serialized_end=11089
+  _STREAMARCREQUEST._serialized_start=11356
+  _STREAMARCREQUEST._serialized_end=11802
+  _STREAMARCREQUEST_TYPE._serialized_start=11065
+  _STREAMARCREQUEST_TYPE._serialized_end=11089
+  _STREAMCIRCLEREQUEST._serialized_start=11805
+  _STREAMCIRCLEREQUEST._serialized_end=12153
+  _STREAMCIRCLEREQUEST_TYPE._serialized_start=11065
+  _STREAMCIRCLEREQUEST_TYPE._serialized_end=11089
+  _STREAMWAITDIGITALINPUTREQUEST._serialized_start=12156
+  _STREAMWAITDIGITALINPUTREQUEST._serialized_end=12296
+  _STREAMWAITANALOGINPUTREQUEST._serialized_start=12299
+  _STREAMWAITANALOGINPUTREQUEST._serialized_end=12457
+  _STREAMSETDIGITALOUTPUTREQUEST._serialized_start=12460
+  _STREAMSETDIGITALOUTPUTREQUEST._serialized_end=12600
+  _STREAMSETANALOGOUTPUTREQUEST._serialized_start=12603
+  _STREAMSETANALOGOUTPUTREQUEST._serialized_end=12742
+  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_start=12745
+  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_end=12873
+  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_start=12875
+  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_end=12996
+  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_start=12998
+  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_end=13118
+  _STREAMWAITREQUEST._serialized_start=13120
+  _STREAMWAITREQUEST._serialized_end=13237
+  _STREAMWAITUNTILIDLEREQUEST._serialized_start=13240
+  _STREAMWAITUNTILIDLEREQUEST._serialized_end=13368
+  _STREAMEMPTYREQUEST._serialized_start=13370
+  _STREAMEMPTYREQUEST._serialized_end=13460
+  _STREAMGETAXESRESPONSE._serialized_start=13462
+  _STREAMGETAXESRESPONSE._serialized_end=13545
+  _STREAMGETMAXSPEEDREQUEST._serialized_start=13547
+  _STREAMGETMAXSPEEDREQUEST._serialized_end=13657
+  _STREAMSETMAXSPEEDREQUEST._serialized_start=13660
+  _STREAMSETMAXSPEEDREQUEST._serialized_end=13789
+  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=13791
+  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=13918
+  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=13921
+  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=14085
+  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=14088
+  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=14216
+  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=14219
+  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=14385
+  _STREAMBUFFERGETCONTENTREQUEST._serialized_start=14387
+  _STREAMBUFFERGETCONTENTREQUEST._serialized_end=14488
+  _STREAMBUFFERGETCONTENTRESPONSE._serialized_start=14490
+  _STREAMBUFFERGETCONTENTRESPONSE._serialized_end=14544
+  _STREAMBUFFERERASEREQUEST._serialized_start=14546
+  _STREAMBUFFERERASEREQUEST._serialized_end=14642
+  _STREAMGENERICCOMMANDREQUEST._serialized_start=14644
+  _STREAMGENERICCOMMANDREQUEST._serialized_end=14760
+  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_start=14762
+  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_end=14881
+  _BINARYREPLYONLYEVENT._serialized_start=14883
+  _BINARYREPLYONLYEVENT._serialized_end=14982
+  _OPENBINARYINTERFACEREQUEST._serialized_start=14985
+  _OPENBINARYINTERFACEREQUEST._serialized_end=15172
+  _UNKNOWNBINARYRESPONSEEVENT._serialized_start=15174
+  _UNKNOWNBINARYRESPONSEEVENT._serialized_end=15279
+  _GENERICBINARYREQUEST._serialized_start=15282
+  _GENERICBINARYREQUEST._serialized_end=15412
+  _BINARYMESSAGE._serialized_start=15414
+  _BINARYMESSAGE._serialized_end=15484
+  _BINARYMESSAGECOLLECTION._serialized_start=15486
+  _BINARYMESSAGECOLLECTION._serialized_end=15568
+  _DEVICEEMPTYREQUEST._serialized_start=15570
+  _DEVICEEMPTYREQUEST._serialized_end=15628
+  _BINARYDEVICEIDENTITY._serialized_start=15631
+  _BINARYDEVICEIDENTITY._serialized_end=15976
+  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_start=15927
+  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_end=15976
+  _BINARYGENERICWITHUNITSREQUEST._serialized_start=15979
+  _BINARYGENERICWITHUNITSREQUEST._serialized_end=16132
+  _BINARYDEVICEHOMEREQUEST._serialized_start=16134
+  _BINARYDEVICEHOMEREQUEST._serialized_end=16228
+  _BINARYDEVICEMOVEREQUEST._serialized_start=16231
+  _BINARYDEVICEMOVEREQUEST._serialized_end=16449
+  _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_start=5608
+  _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_end=5645
+  _BINARYDEVICESTOPREQUEST._serialized_start=16451
+  _BINARYDEVICESTOPREQUEST._serialized_end=16545
+  _BINARYDEVICEDETECTREQUEST._serialized_start=16547
+  _BINARYDEVICEDETECTREQUEST._serialized_end=16622
+  _BINARYDEVICEDETECTRESPONSE._serialized_start=16624
+  _BINARYDEVICEDETECTRESPONSE._serialized_end=16669
+  _BINARYDEVICEGETSETTINGREQUEST._serialized_start=16671
+  _BINARYDEVICEGETSETTINGREQUEST._serialized_end=16771
+  _BINARYDEVICESETSETTINGREQUEST._serialized_start=16773
+  _BINARYDEVICESETSETTINGREQUEST._serialized_end=16888
+  _CUSTOMINTERFACEREADREQUEST._serialized_start=16890
+  _CUSTOMINTERFACEREADREQUEST._serialized_end=16940
+  _CUSTOMINTERFACEWRITEREQUEST._serialized_start=16942
+  _CUSTOMINTERFACEWRITEREQUEST._serialized_end=17010
+  _CUSTOMINTERFACEOPENRESPONSE._serialized_start=17012
+  _CUSTOMINTERFACEOPENRESPONSE._serialized_end=17063
+  _CUSTOMINTERFACECLOSEREQUEST._serialized_start=17065
+  _CUSTOMINTERFACECLOSEREQUEST._serialized_end=17139
+  _CANSETSTATEREQUEST._serialized_start=17141
+  _CANSETSTATEREQUEST._serialized_end=17228
+  _CANSETSTATEAXISRESPONSE._serialized_start=17230
+  _CANSETSTATEAXISRESPONSE._serialized_end=17291
+  _CANSETSTATEDEVICERESPONSE._serialized_start=17293
+  _CANSETSTATEDEVICERESPONSE._serialized_end=17405
+  _SETSTATEREQUEST._serialized_start=17407
+  _SETSTATEREQUEST._serialized_end=17512
+  _SERVOTUNINGREQUEST._serialized_start=17514
+  _SERVOTUNINGREQUEST._serialized_end=17604
+  _SERVOTUNINGPARAM._serialized_start=17606
+  _SERVOTUNINGPARAM._serialized_end=17653
+  _PARAMSETINFO._serialized_start=17655
+  _PARAMSETINFO._serialized_end=17758
+  _SETSERVOTUNINGREQUEST._serialized_start=17761
+  _SETSERVOTUNINGREQUEST._serialized_end=17919
+  _LOADPARAMSET._serialized_start=17921
+  _LOADPARAMSET._serialized_end=18031
+  _SETSERVOTUNINGPIDREQUEST._serialized_start=18034
+  _SETSERVOTUNINGPIDREQUEST._serialized_end=18175
+  _PIDTUNING._serialized_start=18177
+  _PIDTUNING._serialized_end=18264
+  _SETSIMPLETUNING._serialized_start=18267
+  _SETSIMPLETUNING._serialized_end=18461
+  _SIMPLETUNINGPARAMDEFINITION._serialized_start=18463
+  _SIMPLETUNINGPARAMDEFINITION._serialized_end=18563
+  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_start=18565
+  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_end=18674
+  _TRANSLATORCREATEREQUEST._serialized_start=18677
+  _TRANSLATORCREATEREQUEST._serialized_end=18826
+  _TRANSLATORCREATERESPONSE._serialized_start=18828
+  _TRANSLATORCREATERESPONSE._serialized_end=18877
+  _TRANSLATORAXISDEFINITION._serialized_start=18879
+  _TRANSLATORAXISDEFINITION._serialized_end=18958
+  _TRANSLATORDEFINITION._serialized_start=18961
+  _TRANSLATORDEFINITION._serialized_end=19122
+  _TRANSLATORCONFIG._serialized_start=19125
+  _TRANSLATORCONFIG._serialized_end=19297
+  _TRANSLATORAXISMAPPING._serialized_start=19299
+  _TRANSLATORAXISMAPPING._serialized_end=19363
+  _TRANSLATORAXISTRANSFORMATION._serialized_start=19365
+  _TRANSLATORAXISTRANSFORMATION._serialized_end=19491
+  _TRANSLATORTRANSLATEREQUEST._serialized_start=19493
+  _TRANSLATORTRANSLATEREQUEST._serialized_end=19559
+  _TRANSLATEMESSAGE._serialized_start=19561
+  _TRANSLATEMESSAGE._serialized_end=19634
+  _TRANSLATORTRANSLATERESPONSE._serialized_start=19636
+  _TRANSLATORTRANSLATERESPONSE._serialized_end=19743
+  _GCODESYNTAXEXCEPTIONDATA._serialized_start=19745
+  _GCODESYNTAXEXCEPTIONDATA._serialized_end=19809
+  _GCODEEXECUTIONEXCEPTIONDATA._serialized_start=19811
+  _GCODEEXECUTIONEXCEPTIONDATA._serialized_end=19878
+  _TRANSLATORFLUSHLIVEREQUEST._serialized_start=19880
+  _TRANSLATORFLUSHLIVEREQUEST._serialized_end=19956
+  _TRANSLATORFLUSHRESPONSE._serialized_start=19958
+  _TRANSLATORFLUSHRESPONSE._serialized_end=20001
+  _TRANSLATORCREATELIVEREQUEST._serialized_start=20004
+  _TRANSLATORCREATELIVEREQUEST._serialized_end=20148
+  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_start=20151
+  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_end=20296
+  _TRANSLATOREMPTYREQUEST._serialized_start=20298
+  _TRANSLATOREMPTYREQUEST._serialized_end=20345
+  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_start=20347
+  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_end=20441
+  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_start=20443
+  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_end=20546
+  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_start=20548
+  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_end=20633
+  _TRANSLATORGETAXISOFFSETREQUEST._serialized_start=20635
+  _TRANSLATORGETAXISOFFSETREQUEST._serialized_end=20745
+  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_start=20747
+  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_end=20829
+  _DEVICESETSTORAGEREQUEST._serialized_start=20831
+  _DEVICESETSTORAGEREQUEST._serialized_end=20952
+  _DEVICEGETSTORAGEREQUEST._serialized_start=20954
+  _DEVICEGETSTORAGEREQUEST._serialized_end=21060
+  _DEVICESETSTORAGENUMBERREQUEST._serialized_start=21062
+  _DEVICESETSTORAGENUMBERREQUEST._serialized_end=21173
+  _DEVICESETSTORAGEBOOLREQUEST._serialized_start=21175
+  _DEVICESETSTORAGEBOOLREQUEST._serialized_end=21284
+  _DEVICESTORAGEREQUEST._serialized_start=21286
+  _DEVICESTORAGEREQUEST._serialized_end=21373
+  _DEVICESTORAGELISTKEYSREQUEST._serialized_start=21375
+  _DEVICESTORAGELISTKEYSREQUEST._serialized_end=21473
+  _DEVICESETUNITCONVERSIONSREQUEST._serialized_start=21476
+  _DEVICESETUNITCONVERSIONSREQUEST._serialized_end=21637
+  _CONVERSIONFACTOR._serialized_start=21639
+  _CONVERSIONFACTOR._serialized_end=21703
+  _OBJECTIVECHANGERREQUEST._serialized_start=21705
+  _OBJECTIVECHANGERREQUEST._serialized_end=21799
+  _OBJECTIVECHANGERCREATERESPONSE._serialized_start=21801
+  _OBJECTIVECHANGERCREATERESPONSE._serialized_end=21864
+  _OBJECTIVECHANGERCHANGEREQUEST._serialized_start=21867
+  _OBJECTIVECHANGERCHANGEREQUEST._serialized_end=22045
 # @@protoc_insertion_point(module_scope)
```

### Comparing `zaber_motion-3.3.0/zaber_motion/protobufs/main_pb2.pyi` & `zaber_motion-3.4.0/zaber_motion/protobufs/main_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,21 @@
     G_CODE_SYNTAX: _Errors.ValueType  # 41
     G_CODE_EXECUTION: _Errors.ValueType  # 42
     INVALID_OPERATION: _Errors.ValueType  # 43
     COMMAND_TOO_LONG: _Errors.ValueType  # 44
     NO_VALUE_FOR_KEY: _Errors.ValueType  # 45
     DEVICE_DETECTION_FAILED: _Errors.ValueType  # 46
     TIMEOUT: _Errors.ValueType  # 47
+    PVT_MODE: _Errors.ValueType  # 48
+    PVT_EXECUTION: _Errors.ValueType  # 49
+    PVT_SETUP_FAILED: _Errors.ValueType  # 50
+    PVT_MOVEMENT_FAILED: _Errors.ValueType  # 51
+    PVT_MOVEMENT_INTERRUPTED: _Errors.ValueType  # 52
+    PVT_DISCONTINUITY: _Errors.ValueType  # 53
+    STREAM_DISCONTINUITY: _Errors.ValueType  # 54
 
 class Errors(_Errors, metaclass=_ErrorsEnumTypeWrapper): ...
 
 REQUEST_TIMEOUT: Errors.ValueType  # 0
 CONNECTION_CLOSED: Errors.ValueType  # 1
 INVALID_ARGUMENT: Errors.ValueType  # 2
 OUT_OF_REQUEST_IDS: Errors.ValueType  # 3
@@ -133,14 +140,21 @@
 G_CODE_SYNTAX: Errors.ValueType  # 41
 G_CODE_EXECUTION: Errors.ValueType  # 42
 INVALID_OPERATION: Errors.ValueType  # 43
 COMMAND_TOO_LONG: Errors.ValueType  # 44
 NO_VALUE_FOR_KEY: Errors.ValueType  # 45
 DEVICE_DETECTION_FAILED: Errors.ValueType  # 46
 TIMEOUT: Errors.ValueType  # 47
+PVT_MODE: Errors.ValueType  # 48
+PVT_EXECUTION: Errors.ValueType  # 49
+PVT_SETUP_FAILED: Errors.ValueType  # 50
+PVT_MOVEMENT_FAILED: Errors.ValueType  # 51
+PVT_MOVEMENT_INTERRUPTED: Errors.ValueType  # 52
+PVT_DISCONTINUITY: Errors.ValueType  # 53
+STREAM_DISCONTINUITY: Errors.ValueType  # 54
 global___Errors = Errors
 
 class _InterfaceType:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _InterfaceTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_InterfaceType.ValueType], builtins.type):
@@ -563,14 +577,33 @@
         reason: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["reason", b"reason", "warnings", b"warnings"]) -> None: ...
 
 global___StreamMovementInterruptedExceptionData = StreamMovementInterruptedExceptionData
 
 @typing_extensions.final
+class PvtMovementInterruptedExceptionData(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    WARNINGS_FIELD_NUMBER: builtins.int
+    REASON_FIELD_NUMBER: builtins.int
+    @property
+    def warnings(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    reason: builtins.str
+    def __init__(
+        self,
+        *,
+        warnings: collections.abc.Iterable[builtins.str] | None = ...,
+        reason: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["reason", b"reason", "warnings", b"warnings"]) -> None: ...
+
+global___PvtMovementInterruptedExceptionData = PvtMovementInterruptedExceptionData
+
+@typing_extensions.final
 class MovementFailedExceptionData(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     WARNINGS_FIELD_NUMBER: builtins.int
     REASON_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     AXIS_FIELD_NUMBER: builtins.int
@@ -607,14 +640,33 @@
         reason: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["reason", b"reason", "warnings", b"warnings"]) -> None: ...
 
 global___StreamMovementFailedExceptionData = StreamMovementFailedExceptionData
 
 @typing_extensions.final
+class PvtMovementFailedExceptionData(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    WARNINGS_FIELD_NUMBER: builtins.int
+    REASON_FIELD_NUMBER: builtins.int
+    @property
+    def warnings(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    reason: builtins.str
+    def __init__(
+        self,
+        *,
+        warnings: collections.abc.Iterable[builtins.str] | None = ...,
+        reason: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["reason", b"reason", "warnings", b"warnings"]) -> None: ...
+
+global___PvtMovementFailedExceptionData = PvtMovementFailedExceptionData
+
+@typing_extensions.final
 class StreamExecutionExceptionData(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ERROR_FLAG_FIELD_NUMBER: builtins.int
     REASON_FIELD_NUMBER: builtins.int
     error_flag: builtins.str
     reason: builtins.str
@@ -625,14 +677,54 @@
         reason: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["error_flag", b"error_flag", "reason", b"reason"]) -> None: ...
 
 global___StreamExecutionExceptionData = StreamExecutionExceptionData
 
 @typing_extensions.final
+class PvtExecutionExceptionData(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    ERROR_FLAG_FIELD_NUMBER: builtins.int
+    REASON_FIELD_NUMBER: builtins.int
+    INVALID_POINTS_FIELD_NUMBER: builtins.int
+    error_flag: builtins.str
+    reason: builtins.str
+    @property
+    def invalid_points(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___InvalidPvtPoint]: ...
+    def __init__(
+        self,
+        *,
+        error_flag: builtins.str = ...,
+        reason: builtins.str = ...,
+        invalid_points: collections.abc.Iterable[global___InvalidPvtPoint] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["error_flag", b"error_flag", "invalid_points", b"invalid_points", "reason", b"reason"]) -> None: ...
+
+global___PvtExecutionExceptionData = PvtExecutionExceptionData
+
+@typing_extensions.final
+class InvalidPvtPoint(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    INDEX_FIELD_NUMBER: builtins.int
+    POINT_FIELD_NUMBER: builtins.int
+    index: builtins.int
+    point: builtins.str
+    def __init__(
+        self,
+        *,
+        index: builtins.int = ...,
+        point: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["index", b"index", "point", b"point"]) -> None: ...
+
+global___InvalidPvtPoint = InvalidPvtPoint
+
+@typing_extensions.final
 class InvalidResponseExceptionData(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESPONSE_FIELD_NUMBER: builtins.int
     response: builtins.str
     def __init__(
         self,
@@ -2541,171 +2633,256 @@
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     AXES_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     @property
     def axes(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         axes: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["axes", b"axes", "device", b"device", "interface_id", b"interface_id", "stream_id", b"stream_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["axes", b"axes", "device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id"]) -> None: ...
 
 global___StreamSetupLiveRequest = StreamSetupLiveRequest
 
 @typing_extensions.final
 class StreamSetupLiveCompositeRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     AXES_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     @property
     def axes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___StreamAxisDefinition]: ...
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         axes: collections.abc.Iterable[global___StreamAxisDefinition] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["axes", b"axes", "device", b"device", "interface_id", b"interface_id", "stream_id", b"stream_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["axes", b"axes", "device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id"]) -> None: ...
 
 global___StreamSetupLiveCompositeRequest = StreamSetupLiveCompositeRequest
 
 @typing_extensions.final
 class StreamSetupStoreRequest(google.protobuf.message.Message):
     """device/stream_setup_store"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     STREAM_BUFFER_FIELD_NUMBER: builtins.int
+    PVT_BUFFER_FIELD_NUMBER: builtins.int
     AXES_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     stream_buffer: builtins.int
+    pvt_buffer: builtins.int
     @property
     def axes(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         stream_buffer: builtins.int = ...,
+        pvt_buffer: builtins.int = ...,
         axes: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["axes", b"axes", "device", b"device", "interface_id", b"interface_id", "stream_buffer", b"stream_buffer", "stream_id", b"stream_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["axes", b"axes", "device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "pvt_buffer", b"pvt_buffer", "stream_buffer", b"stream_buffer", "stream_id", b"stream_id"]) -> None: ...
 
 global___StreamSetupStoreRequest = StreamSetupStoreRequest
 
 @typing_extensions.final
 class StreamSetupStoreCompositeRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     STREAM_BUFFER_FIELD_NUMBER: builtins.int
+    PVT_BUFFER_FIELD_NUMBER: builtins.int
     AXES_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     stream_buffer: builtins.int
+    pvt_buffer: builtins.int
     @property
     def axes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___StreamAxisDefinition]: ...
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         stream_buffer: builtins.int = ...,
+        pvt_buffer: builtins.int = ...,
         axes: collections.abc.Iterable[global___StreamAxisDefinition] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["axes", b"axes", "device", b"device", "interface_id", b"interface_id", "stream_buffer", b"stream_buffer", "stream_id", b"stream_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["axes", b"axes", "device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "pvt_buffer", b"pvt_buffer", "stream_buffer", b"stream_buffer", "stream_id", b"stream_id"]) -> None: ...
 
 global___StreamSetupStoreCompositeRequest = StreamSetupStoreCompositeRequest
 
 @typing_extensions.final
 class StreamSetupStoreArbitraryAxesRequest(google.protobuf.message.Message):
     """device/stream_enable_store_arbitrary_axes"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     STREAM_BUFFER_FIELD_NUMBER: builtins.int
+    PVT_BUFFER_FIELD_NUMBER: builtins.int
     AXES_COUNT_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     stream_buffer: builtins.int
+    pvt_buffer: builtins.int
     axes_count: builtins.int
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         stream_buffer: builtins.int = ...,
+        pvt_buffer: builtins.int = ...,
         axes_count: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["axes_count", b"axes_count", "device", b"device", "interface_id", b"interface_id", "stream_buffer", b"stream_buffer", "stream_id", b"stream_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["axes_count", b"axes_count", "device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "pvt_buffer", b"pvt_buffer", "stream_buffer", b"stream_buffer", "stream_id", b"stream_id"]) -> None: ...
 
 global___StreamSetupStoreArbitraryAxesRequest = StreamSetupStoreArbitraryAxesRequest
 
 @typing_extensions.final
 class StreamCallRequest(google.protobuf.message.Message):
     """device/stream_call"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     STREAM_BUFFER_FIELD_NUMBER: builtins.int
+    PVT_BUFFER_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     stream_buffer: builtins.int
+    pvt_buffer: builtins.int
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         stream_buffer: builtins.int = ...,
+        pvt_buffer: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "stream_buffer", b"stream_buffer", "stream_id", b"stream_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "pvt_buffer", b"pvt_buffer", "stream_buffer", b"stream_buffer", "stream_id", b"stream_id"]) -> None: ...
 
 global___StreamCallRequest = StreamCallRequest
 
 @typing_extensions.final
+class PvtPointRequest(google.protobuf.message.Message):
+    """device/pvt_point"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    class _Type:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _TypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[PvtPointRequest._Type.ValueType], builtins.type):  # noqa: F821
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        ABS: PvtPointRequest._Type.ValueType  # 0
+        REL: PvtPointRequest._Type.ValueType  # 1
+
+    class Type(_Type, metaclass=_TypeEnumTypeWrapper): ...
+    ABS: PvtPointRequest.Type.ValueType  # 0
+    REL: PvtPointRequest.Type.ValueType  # 1
+
+    INTERFACE_ID_FIELD_NUMBER: builtins.int
+    DEVICE_FIELD_NUMBER: builtins.int
+    STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
+    TYPE_FIELD_NUMBER: builtins.int
+    POSITIONS_FIELD_NUMBER: builtins.int
+    VELOCITIES_FIELD_NUMBER: builtins.int
+    TIME_FIELD_NUMBER: builtins.int
+    interface_id: builtins.int
+    device: builtins.int
+    stream_id: builtins.int
+    pvt: builtins.bool
+    type: global___PvtPointRequest.Type.ValueType
+    @property
+    def positions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Measurement]: ...
+    @property
+    def velocities(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Measurement]: ...
+    @property
+    def time(self) -> global___Measurement: ...
+    def __init__(
+        self,
+        *,
+        interface_id: builtins.int = ...,
+        device: builtins.int = ...,
+        stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
+        type: global___PvtPointRequest.Type.ValueType = ...,
+        positions: collections.abc.Iterable[global___Measurement] | None = ...,
+        velocities: collections.abc.Iterable[global___Measurement] | None = ...,
+        time: global___Measurement | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["time", b"time"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "positions", b"positions", "pvt", b"pvt", "stream_id", b"stream_id", "time", b"time", "type", b"type", "velocities", b"velocities"]) -> None: ...
+
+global___PvtPointRequest = PvtPointRequest
+
+@typing_extensions.final
 class StreamLineRequest(google.protobuf.message.Message):
     """device/stream_line"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Type:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -2719,36 +2896,39 @@
     class Type(_Type, metaclass=_TypeEnumTypeWrapper): ...
     ABS: StreamLineRequest.Type.ValueType  # 0
     REL: StreamLineRequest.Type.ValueType  # 1
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     ENDPOINT_FIELD_NUMBER: builtins.int
     TARGET_AXES_INDICES_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     type: global___StreamLineRequest.Type.ValueType
     @property
     def endpoint(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Measurement]: ...
     @property
     def target_axes_indices(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         type: global___StreamLineRequest.Type.ValueType = ...,
         endpoint: collections.abc.Iterable[global___Measurement] | None = ...,
         target_axes_indices: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "endpoint", b"endpoint", "interface_id", b"interface_id", "stream_id", b"stream_id", "target_axes_indices", b"target_axes_indices", "type", b"type"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "endpoint", b"endpoint", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id", "target_axes_indices", b"target_axes_indices", "type", b"type"]) -> None: ...
 
 global___StreamLineRequest = StreamLineRequest
 
 @typing_extensions.final
 class StreamArcRequest(google.protobuf.message.Message):
     """device/stream_arc"""
 
@@ -2766,24 +2946,26 @@
     class Type(_Type, metaclass=_TypeEnumTypeWrapper): ...
     ABS: StreamArcRequest.Type.ValueType  # 0
     REL: StreamArcRequest.Type.ValueType  # 1
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     ROTATION_DIRECTION_FIELD_NUMBER: builtins.int
     CENTER_X_FIELD_NUMBER: builtins.int
     CENTER_Y_FIELD_NUMBER: builtins.int
     END_X_FIELD_NUMBER: builtins.int
     END_Y_FIELD_NUMBER: builtins.int
     TARGET_AXES_INDICES_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     type: global___StreamArcRequest.Type.ValueType
     rotation_direction: builtins.int
     @property
     def center_x(self) -> global___Measurement: ...
     @property
     def center_y(self) -> global___Measurement: ...
     @property
@@ -2794,24 +2976,25 @@
     def target_axes_indices(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         type: global___StreamArcRequest.Type.ValueType = ...,
         rotation_direction: builtins.int = ...,
         center_x: global___Measurement | None = ...,
         center_y: global___Measurement | None = ...,
         end_x: global___Measurement | None = ...,
         end_y: global___Measurement | None = ...,
         target_axes_indices: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["center_x", b"center_x", "center_y", b"center_y", "end_x", b"end_x", "end_y", b"end_y"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["center_x", b"center_x", "center_y", b"center_y", "device", b"device", "end_x", b"end_x", "end_y", b"end_y", "interface_id", b"interface_id", "rotation_direction", b"rotation_direction", "stream_id", b"stream_id", "target_axes_indices", b"target_axes_indices", "type", b"type"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["center_x", b"center_x", "center_y", b"center_y", "device", b"device", "end_x", b"end_x", "end_y", b"end_y", "interface_id", b"interface_id", "pvt", b"pvt", "rotation_direction", b"rotation_direction", "stream_id", b"stream_id", "target_axes_indices", b"target_axes_indices", "type", b"type"]) -> None: ...
 
 global___StreamArcRequest = StreamArcRequest
 
 @typing_extensions.final
 class StreamCircleRequest(google.protobuf.message.Message):
     """device/stream_circle"""
 
@@ -2829,319 +3012,352 @@
     class Type(_Type, metaclass=_TypeEnumTypeWrapper): ...
     ABS: StreamCircleRequest.Type.ValueType  # 0
     REL: StreamCircleRequest.Type.ValueType  # 1
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     ROTATION_DIRECTION_FIELD_NUMBER: builtins.int
     CENTER_X_FIELD_NUMBER: builtins.int
     CENTER_Y_FIELD_NUMBER: builtins.int
     TARGET_AXES_INDICES_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     type: global___StreamCircleRequest.Type.ValueType
     rotation_direction: builtins.int
     @property
     def center_x(self) -> global___Measurement: ...
     @property
     def center_y(self) -> global___Measurement: ...
     @property
     def target_axes_indices(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         type: global___StreamCircleRequest.Type.ValueType = ...,
         rotation_direction: builtins.int = ...,
         center_x: global___Measurement | None = ...,
         center_y: global___Measurement | None = ...,
         target_axes_indices: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["center_x", b"center_x", "center_y", b"center_y"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["center_x", b"center_x", "center_y", b"center_y", "device", b"device", "interface_id", b"interface_id", "rotation_direction", b"rotation_direction", "stream_id", b"stream_id", "target_axes_indices", b"target_axes_indices", "type", b"type"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["center_x", b"center_x", "center_y", b"center_y", "device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "rotation_direction", b"rotation_direction", "stream_id", b"stream_id", "target_axes_indices", b"target_axes_indices", "type", b"type"]) -> None: ...
 
 global___StreamCircleRequest = StreamCircleRequest
 
 @typing_extensions.final
 class StreamWaitDigitalInputRequest(google.protobuf.message.Message):
     """device/stream_wait_digital_input"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     CHANNEL_NUMBER_FIELD_NUMBER: builtins.int
     VALUE_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     channel_number: builtins.int
     value: builtins.bool
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         channel_number: builtins.int = ...,
         value: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["channel_number", b"channel_number", "device", b"device", "interface_id", b"interface_id", "stream_id", b"stream_id", "value", b"value"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["channel_number", b"channel_number", "device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id", "value", b"value"]) -> None: ...
 
 global___StreamWaitDigitalInputRequest = StreamWaitDigitalInputRequest
 
 @typing_extensions.final
 class StreamWaitAnalogInputRequest(google.protobuf.message.Message):
     """device/stream_wait_analog_input"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     CHANNEL_NUMBER_FIELD_NUMBER: builtins.int
     CONDITION_FIELD_NUMBER: builtins.int
     VALUE_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     channel_number: builtins.int
     condition: builtins.str
     value: builtins.float
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         channel_number: builtins.int = ...,
         condition: builtins.str = ...,
         value: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["channel_number", b"channel_number", "condition", b"condition", "device", b"device", "interface_id", b"interface_id", "stream_id", b"stream_id", "value", b"value"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["channel_number", b"channel_number", "condition", b"condition", "device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id", "value", b"value"]) -> None: ...
 
 global___StreamWaitAnalogInputRequest = StreamWaitAnalogInputRequest
 
 @typing_extensions.final
 class StreamSetDigitalOutputRequest(google.protobuf.message.Message):
     """device/stream_set_digital_output"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     CHANNEL_NUMBER_FIELD_NUMBER: builtins.int
     VALUE_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     channel_number: builtins.int
     value: builtins.bool
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         channel_number: builtins.int = ...,
         value: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["channel_number", b"channel_number", "device", b"device", "interface_id", b"interface_id", "stream_id", b"stream_id", "value", b"value"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["channel_number", b"channel_number", "device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id", "value", b"value"]) -> None: ...
 
 global___StreamSetDigitalOutputRequest = StreamSetDigitalOutputRequest
 
 @typing_extensions.final
 class StreamSetAnalogOutputRequest(google.protobuf.message.Message):
     """device/stream_set_analog_output"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     CHANNEL_NUMBER_FIELD_NUMBER: builtins.int
     VALUE_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     channel_number: builtins.int
     value: builtins.float
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         channel_number: builtins.int = ...,
         value: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["channel_number", b"channel_number", "device", b"device", "interface_id", b"interface_id", "stream_id", b"stream_id", "value", b"value"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["channel_number", b"channel_number", "device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id", "value", b"value"]) -> None: ...
 
 global___StreamSetAnalogOutputRequest = StreamSetAnalogOutputRequest
 
 @typing_extensions.final
 class StreamToggleDigitalOutputRequest(google.protobuf.message.Message):
     """device/stream_toggle_digital_output"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     CHANNEL_NUMBER_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     channel_number: builtins.int
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         channel_number: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["channel_number", b"channel_number", "device", b"device", "interface_id", b"interface_id", "stream_id", b"stream_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["channel_number", b"channel_number", "device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id"]) -> None: ...
 
 global___StreamToggleDigitalOutputRequest = StreamToggleDigitalOutputRequest
 
 @typing_extensions.final
 class StreamSetAllDigitalOutputsRequest(google.protobuf.message.Message):
     """device/stream_set_all_digital_outputs"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     VALUES_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     @property
     def values(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.bool]: ...
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         values: collections.abc.Iterable[builtins.bool] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "stream_id", b"stream_id", "values", b"values"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id", "values", b"values"]) -> None: ...
 
 global___StreamSetAllDigitalOutputsRequest = StreamSetAllDigitalOutputsRequest
 
 @typing_extensions.final
 class StreamSetAllAnalogOutputsRequest(google.protobuf.message.Message):
     """device/stream_set_all_analog_outputs"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     VALUES_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     @property
     def values(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         values: collections.abc.Iterable[builtins.float] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "stream_id", b"stream_id", "values", b"values"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id", "values", b"values"]) -> None: ...
 
 global___StreamSetAllAnalogOutputsRequest = StreamSetAllAnalogOutputsRequest
 
 @typing_extensions.final
 class StreamWaitRequest(google.protobuf.message.Message):
     """device/stream_wait"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     TIME_FIELD_NUMBER: builtins.int
     UNIT_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     time: builtins.float
     unit: builtins.str
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         time: builtins.float = ...,
         unit: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "stream_id", b"stream_id", "time", b"time", "unit", b"unit"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id", "time", b"time", "unit", b"unit"]) -> None: ...
 
 global___StreamWaitRequest = StreamWaitRequest
 
 @typing_extensions.final
 class StreamWaitUntilIdleRequest(google.protobuf.message.Message):
     """device/stream_wait_until_idle"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     THROW_ERROR_ON_FAULT_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     throw_error_on_fault: builtins.bool
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         throw_error_on_fault: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "stream_id", b"stream_id", "throw_error_on_fault", b"throw_error_on_fault"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id", "throw_error_on_fault", b"throw_error_on_fault"]) -> None: ...
 
 global___StreamWaitUntilIdleRequest = StreamWaitUntilIdleRequest
 
 @typing_extensions.final
 class StreamEmptyRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "stream_id", b"stream_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id"]) -> None: ...
 
 global___StreamEmptyRequest = StreamEmptyRequest
 
 @typing_extensions.final
 class StreamGetAxesResponse(google.protobuf.message.Message):
     """device/stream_get_axes"""
 
@@ -3164,190 +3380,211 @@
     """device/stream_get_max_speed"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     UNIT_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     unit: builtins.str
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         unit: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "stream_id", b"stream_id", "unit", b"unit"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id", "unit", b"unit"]) -> None: ...
 
 global___StreamGetMaxSpeedRequest = StreamGetMaxSpeedRequest
 
 @typing_extensions.final
 class StreamSetMaxSpeedRequest(google.protobuf.message.Message):
     """device/stream_set_max_speed"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     MAX_SPEED_FIELD_NUMBER: builtins.int
     UNIT_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     max_speed: builtins.float
     unit: builtins.str
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         max_speed: builtins.float = ...,
         unit: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "max_speed", b"max_speed", "stream_id", b"stream_id", "unit", b"unit"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "max_speed", b"max_speed", "pvt", b"pvt", "stream_id", b"stream_id", "unit", b"unit"]) -> None: ...
 
 global___StreamSetMaxSpeedRequest = StreamSetMaxSpeedRequest
 
 @typing_extensions.final
 class StreamGetMaxTangentialAccelerationRequest(google.protobuf.message.Message):
     """device/stream_get_max_tangential_acceleration"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     UNIT_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     unit: builtins.str
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         unit: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "stream_id", b"stream_id", "unit", b"unit"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id", "unit", b"unit"]) -> None: ...
 
 global___StreamGetMaxTangentialAccelerationRequest = StreamGetMaxTangentialAccelerationRequest
 
 @typing_extensions.final
 class StreamSetMaxTangentialAccelerationRequest(google.protobuf.message.Message):
     """device/stream_set_max_tangential_acceleration"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     MAX_TANGENTIAL_ACCELERATION_FIELD_NUMBER: builtins.int
     UNIT_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     max_tangential_acceleration: builtins.float
     unit: builtins.str
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         max_tangential_acceleration: builtins.float = ...,
         unit: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "max_tangential_acceleration", b"max_tangential_acceleration", "stream_id", b"stream_id", "unit", b"unit"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "max_tangential_acceleration", b"max_tangential_acceleration", "pvt", b"pvt", "stream_id", b"stream_id", "unit", b"unit"]) -> None: ...
 
 global___StreamSetMaxTangentialAccelerationRequest = StreamSetMaxTangentialAccelerationRequest
 
 @typing_extensions.final
 class StreamGetMaxCentripetalAccelerationRequest(google.protobuf.message.Message):
     """device/stream_get_max_centripetal_acceleration"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     UNIT_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     unit: builtins.str
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         unit: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "stream_id", b"stream_id", "unit", b"unit"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id", "unit", b"unit"]) -> None: ...
 
 global___StreamGetMaxCentripetalAccelerationRequest = StreamGetMaxCentripetalAccelerationRequest
 
 @typing_extensions.final
 class StreamSetMaxCentripetalAccelerationRequest(google.protobuf.message.Message):
     """device/stream_set_max_centripetal_acceleration"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     MAX_CENTRIPETAL_ACCELERATION_FIELD_NUMBER: builtins.int
     UNIT_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     max_centripetal_acceleration: builtins.float
     unit: builtins.str
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         max_centripetal_acceleration: builtins.float = ...,
         unit: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "max_centripetal_acceleration", b"max_centripetal_acceleration", "stream_id", b"stream_id", "unit", b"unit"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "interface_id", b"interface_id", "max_centripetal_acceleration", b"max_centripetal_acceleration", "pvt", b"pvt", "stream_id", b"stream_id", "unit", b"unit"]) -> None: ...
 
 global___StreamSetMaxCentripetalAccelerationRequest = StreamSetMaxCentripetalAccelerationRequest
 
 @typing_extensions.final
 class StreamBufferGetContentRequest(google.protobuf.message.Message):
     """device/stream_buffer_get_content"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     BUFFER_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     buffer_id: builtins.int
+    pvt: builtins.bool
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         buffer_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["buffer_id", b"buffer_id", "device", b"device", "interface_id", b"interface_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["buffer_id", b"buffer_id", "device", b"device", "interface_id", b"interface_id", "pvt", b"pvt"]) -> None: ...
 
 global___StreamBufferGetContentRequest = StreamBufferGetContentRequest
 
 @typing_extensions.final
 class StreamBufferGetContentResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -3368,78 +3605,87 @@
     """device/stream_buffer_erase"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     BUFFER_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     buffer_id: builtins.int
+    pvt: builtins.bool
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         buffer_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["buffer_id", b"buffer_id", "device", b"device", "interface_id", b"interface_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["buffer_id", b"buffer_id", "device", b"device", "interface_id", b"interface_id", "pvt", b"pvt"]) -> None: ...
 
 global___StreamBufferEraseRequest = StreamBufferEraseRequest
 
 @typing_extensions.final
 class StreamGenericCommandRequest(google.protobuf.message.Message):
     """device/stream_generic_command"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     COMMAND_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     command: builtins.str
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         command: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["command", b"command", "device", b"device", "interface_id", b"interface_id", "stream_id", b"stream_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["command", b"command", "device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id"]) -> None: ...
 
 global___StreamGenericCommandRequest = StreamGenericCommandRequest
 
 @typing_extensions.final
 class StreamGenericCommandBatchRequest(google.protobuf.message.Message):
     """device/stream_generic_command_batch"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     STREAM_ID_FIELD_NUMBER: builtins.int
+    PVT_FIELD_NUMBER: builtins.int
     BATCH_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
+    pvt: builtins.bool
     @property
     def batch(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
+        pvt: builtins.bool = ...,
         batch: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["batch", b"batch", "device", b"device", "interface_id", b"interface_id", "stream_id", b"stream_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["batch", b"batch", "device", b"device", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id"]) -> None: ...
 
 global___StreamGenericCommandBatchRequest = StreamGenericCommandBatchRequest
 
 @typing_extensions.final
 class BinaryReplyOnlyEvent(google.protobuf.message.Message):
     """---- binary/interface ----
```

### Comparing `zaber_motion-3.3.0/zaber_motion/serialization.py` & `zaber_motion-3.4.0/zaber_motion/serialization.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/tools.py` & `zaber_motion-3.4.0/zaber_motion/tools.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion/units.py` & `zaber_motion-3.4.0/zaber_motion/units.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.3.0/zaber_motion.egg-info/PKG-INFO` & `zaber_motion-3.4.0/zaber_motion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaber-motion
-Version: 3.3.0
+Version: 3.4.0
 Summary: A library for communicating with Zaber devices
 Home-page: https://gitlab.com/ZaberTech/zaber-motion-lib
 Author: Zaber Technologies Inc.
 Author-email: contact@zaber.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `zaber_motion-3.3.0/zaber_motion.egg-info/SOURCES.txt` & `zaber_motion-3.4.0/zaber_motion.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,19 @@
 zaber_motion/ascii/lockstep_axes.py
 zaber_motion/ascii/message_type.py
 zaber_motion/ascii/oscilloscope.py
 zaber_motion/ascii/oscilloscope_capture_properties.py
 zaber_motion/ascii/oscilloscope_data.py
 zaber_motion/ascii/paramset_info.py
 zaber_motion/ascii/pid_tuning.py
+zaber_motion/ascii/pvt_axis_definition.py
+zaber_motion/ascii/pvt_axis_type.py
+zaber_motion/ascii/pvt_buffer.py
+zaber_motion/ascii/pvt_mode.py
+zaber_motion/ascii/pvt_sequence.py
 zaber_motion/ascii/response.py
 zaber_motion/ascii/servo_tuner.py
 zaber_motion/ascii/servo_tuning_param.py
 zaber_motion/ascii/servo_tuning_paramset.py
 zaber_motion/ascii/setting_constants.py
 zaber_motion/ascii/simple_tuning_param_definition.py
 zaber_motion/ascii/storage.py
@@ -105,14 +110,15 @@
 zaber_motion/exceptions/internal_error_exception.py
 zaber_motion/exceptions/invalid_argument_exception.py
 zaber_motion/exceptions/invalid_data_exception.py
 zaber_motion/exceptions/invalid_operation_exception.py
 zaber_motion/exceptions/invalid_packet_exception.py
 zaber_motion/exceptions/invalid_packet_exception_data.py
 zaber_motion/exceptions/invalid_park_state_exception.py
+zaber_motion/exceptions/invalid_pvt_point.py
 zaber_motion/exceptions/invalid_response_exception.py
 zaber_motion/exceptions/invalid_response_exception_data.py
 zaber_motion/exceptions/io_channel_out_of_range_exception.py
 zaber_motion/exceptions/io_failed_exception.py
 zaber_motion/exceptions/lockstep_enabled_exception.py
 zaber_motion/exceptions/lockstep_not_enabled_exception.py
 zaber_motion/exceptions/motion_lib_exception.py
@@ -121,21 +127,31 @@
 zaber_motion/exceptions/movement_interrupted_exception.py
 zaber_motion/exceptions/movement_interrupted_exception_data.py
 zaber_motion/exceptions/no_device_found_exception.py
 zaber_motion/exceptions/no_value_for_key_exception.py
 zaber_motion/exceptions/not_supported_exception.py
 zaber_motion/exceptions/os_failed_exception.py
 zaber_motion/exceptions/out_of_request_ids_exception.py
+zaber_motion/exceptions/pvt_discontinuity_exception.py
+zaber_motion/exceptions/pvt_execution_exception.py
+zaber_motion/exceptions/pvt_execution_exception_data.py
+zaber_motion/exceptions/pvt_mode_exception.py
+zaber_motion/exceptions/pvt_movement_failed_exception.py
+zaber_motion/exceptions/pvt_movement_failed_exception_data.py
+zaber_motion/exceptions/pvt_movement_interrupted_exception.py
+zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py
+zaber_motion/exceptions/pvt_setup_failed_exception.py
 zaber_motion/exceptions/request_timeout_exception.py
 zaber_motion/exceptions/serial_port_busy_exception.py
 zaber_motion/exceptions/set_device_state_exception_data.py
 zaber_motion/exceptions/set_device_state_failed_exception.py
 zaber_motion/exceptions/set_peripheral_state_exception_data.py
 zaber_motion/exceptions/set_peripheral_state_failed_exception.py
 zaber_motion/exceptions/setting_not_found_exception.py
+zaber_motion/exceptions/stream_discontinuity_exception.py
 zaber_motion/exceptions/stream_execution_exception.py
 zaber_motion/exceptions/stream_execution_exception_data.py
 zaber_motion/exceptions/stream_mode_exception.py
 zaber_motion/exceptions/stream_movement_failed_exception.py
 zaber_motion/exceptions/stream_movement_failed_exception_data.py
 zaber_motion/exceptions/stream_movement_interrupted_exception.py
 zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
```

