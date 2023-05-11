# Comparing `tmp/automation_rest_server-3.6.8.tar.gz` & `tmp/automation_rest_server-3.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\automation_rest_server-3.6.8.tar", last modified: Wed May 10 08:47:26 2023, max compression
+gzip compressed data, was "dist\automation_rest_server-3.6.9.tar", last modified: Thu May 11 08:02:54 2023, max compression
```

## Comparing `automation_rest_server-3.6.8.tar` & `automation_rest_server-3.6.9.tar`

### file list

```diff
@@ -1,159 +1,160 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/
--rw-rw-rw-   0        0        0     1098 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/LICENSE.txt
--rw-rw-rw-   0        0        0      687 2022-08-30 06:56:12.000000 automation_rest_server-3.6.8/MANIFEST.in
--rw-rw-rw-   0        0        0      551 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/configuration/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/configuration/__init__.py
--rw-rw-rw-   0        0        0      581 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/configuration/config.yaml
--rw-rw-rw-   0        0        0     1099 2022-12-13 11:04:16.000000 automation_rest_server-3.6.8/automation_rest_server/configuration/firmware_build.yaml
--rw-rw-rw-   0        0        0  1333232 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/configuration/pci.ids
--rw-rw-rw-   0        0        0      157 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/configuration/version.yaml
--rw-rw-rw-   0        0        0       83 2022-08-25 03:13:17.000000 automation_rest_server-3.6.8/automation_rest_server/configuration/web_server.yaml
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:18:57.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/
--rw-rw-rw-   0        0        0        0 2022-08-10 09:04:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/models/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:20:01.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/models/__init__.py
--rw-rw-rw-   0        0        0     4257 2023-05-10 02:20:31.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/models/helper.py
--rw-rw-rw-   0        0        0     1944 2022-08-17 05:58:24.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/node_resource.py
--rw-rw-rw-   0        0        0     1374 2022-08-30 04:43:20.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/test_resource.py
--rw-rw-rw-   0        0        0      340 2022-08-25 03:00:40.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/web_resource.py
--rw-rw-rw-   0        0        0     2536 2023-02-21 08:02:23.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/web_rest_client.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/__init__.py
--rw-rw-rw-   0        0        0     1678 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/reset_server.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/__init__.py
--rw-rw-rw-   0        0        0     2150 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/benchmark_resource.py
--rw-rw-rw-   0        0        0     1956 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/build_firmware_resource.py
--rw-rw-rw-   0        0        0      933 2022-12-12 01:57:01.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/git_resource.py
--rw-rw-rw-   0        0        0      850 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/models/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/models/__init__.py
--rw-rw-rw-   0        0        0     2044 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/models/ftp_server.py
--rw-rw-rw-   0        0        0     1732 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/models/helper.py
--rw-rw-rw-   0        0        0      958 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/oakgate_resource.py
--rw-rw-rw-   0        0        0      691 2022-08-11 02:31:16.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/operation_resource.py
--rw-rw-rw-   0        0        0     1641 2022-09-20 01:54:25.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/state_resource.py
--rw-rw-rw-   0        0        0     1085 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/stop_flag_resource.py
--rw-rw-rw-   0        0        0     6233 2022-12-03 07:36:31.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/test_resource.py
--rw-rw-rw-   0        0        0     1295 2023-05-10 02:20:31.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/upgrade_resource.py
--rw-rw-rw-   0        0        0     6063 2023-05-04 07:05:41.000000 automation_rest_server-3.6.8/automation_rest_server/run.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/__init__.py
--rw-rw-rw-   0        0        0     6679 2022-09-20 04:46:34.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/database.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/
--rw-rw-rw-   0        0        0        0 2021-11-12 08:10:50.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/__init__.py
--rw-rw-rw-   0        0        0     3082 2023-04-19 05:40:44.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/slot.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/
--rw-rw-rw-   0        0        0        0 2021-11-24 03:48:51.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/__init__.py
--rw-rw-rw-   0        0        0     1434 2022-09-15 07:43:45.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py
--rw-rw-rw-   0        0        0     3541 2023-04-17 06:49:22.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py
--rw-rw-rw-   0        0        0      901 2023-04-19 03:39:13.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py
--rw-rw-rw-   0        0        0     8894 2023-05-09 09:27:56.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/
--rw-rw-rw-   0        0        0      214 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/__init__.py
--rw-rw-rw-   0        0        0     2068 2023-04-25 07:50:43.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/nose_engine.py
--rw-rw-rw-   0        0        0     4926 2023-02-16 01:39:59.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/oakgate_engine.py
--rw-rw-rw-   0        0        0     4007 2023-03-02 06:19:25.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/perses_engine.py
--rw-rw-rw-   0        0        0     1489 2022-09-30 01:53:36.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py
--rw-rw-rw-   0        0        0      239 2023-04-07 02:04:12.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/special_parameter.py
--rw-rw-rw-   0        0        0     3562 2022-09-20 07:48:14.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/sse_engine.py
--rw-rw-rw-   0        0        0     4006 2023-04-25 07:48:48.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/venus_engine.py
--rw-rw-rw-   0        0        0     1517 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_build.py
--rw-rw-rw-   0        0        0     3049 2023-05-10 02:58:49.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_download.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/__init__.py
--rw-rw-rw-   0        0        0     7168 2022-12-13 11:05:02.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py
--rw-rw-rw-   0        0        0     5908 2023-05-10 07:34:30.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/logic_with_firmware_engine.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/oakgate/
--rw-rw-rw-   0        0        0        0 2023-04-11 02:31:20.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/oakgate/__init__.py
--rw-rw-rw-   0        0        0     2925 2023-04-11 02:43:50.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py
--rw-rw-rw-   0        0        0     2691 2023-04-17 07:35:59.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py
--rw-rw-rw-   0        0        0      671 2023-05-10 02:30:29.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py
--rw-rw-rw-   0        0        0     1996 2023-05-10 03:22:37.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py
--rw-rw-rw-   0        0        0     1585 2023-05-10 02:30:15.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py
--rw-rw-rw-   0        0        0     2344 2023-04-09 02:31:46.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py
--rw-rw-rw-   0        0        0     5139 2023-05-10 07:14:09.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/node_database.py
--rw-rw-rw-   0        0        0    10717 2023-04-19 03:38:41.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/performance_database.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/reboot_engine/
--rw-rw-rw-   0        0        0       50 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/reboot_engine/__init__.py
--rw-rw-rw-   0        0        0     2439 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py
--rw-rw-rw-   0        0        0     2055 2023-05-10 02:51:26.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/state.py
--rw-rw-rw-   0        0        0      672 2022-12-13 03:29:14.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/status_file.py
--rw-rw-rw-   0        0        0     5684 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_base.py
--rw-rw-rw-   0        0        0     1973 2023-02-14 08:06:21.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_benchmark.py
--rw-rw-rw-   0        0        0     3512 2023-02-07 07:54:27.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_benchmark_group.py
--rw-rw-rw-   0        0        0     1263 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_case.py
--rw-rw-rw-   0        0        0    22062 2023-05-10 02:21:32.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_pool.py
--rw-rw-rw-   0        0        0      892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_reboot_handle.py
--rw-rw-rw-   0        0        0     4365 2022-12-03 07:44:06.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_result.py
--rw-rw-rw-   0        0        0     3757 2023-03-02 10:28:02.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_runner.py
--rw-rw-rw-   0        0        0     4717 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_suite.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/
--rw-rw-rw-   0        0        0        0 2021-11-12 06:54:04.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/dll/
--rw-rw-rw-   0        0        0        0 2021-10-23 02:17:43.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/dll/__init__.py
--rw-rw-rw-   0        0        0    24064 2021-10-23 02:17:43.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/dll/buf.dll
--rw-rw-rw-   0        0        0    12760 2021-10-23 02:17:43.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/dll/buf.so
--rw-rw-rw-   0        0        0      777 2021-10-23 02:17:43.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/dll/build.py
--rw-rw-rw-   0        0        0      861 2022-09-15 07:43:45.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/linux_nvme.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/
--rw-rw-rw-   0        0        0        0 2021-11-23 06:34:00.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/__init__.py
--rw-rw-rw-   0        0        0    14077 2021-11-23 06:29:25.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/buf.py
--rw-rw-rw-   0        0        0     4722 2021-11-23 06:25:09.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/ctype.py
--rw-rw-rw-   0        0        0    39204 2021-11-23 06:28:50.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/get_feature.py
--rw-rw-rw-   0        0        0    38547 2022-09-15 07:43:45.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/ioctl.py
--rw-rw-rw-   0        0        0    23303 2022-09-15 07:42:03.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/nvme.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/
--rw-rw-rw-   0        0        0      256 2021-11-23 06:21:15.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/__init__.py
--rw-rw-rw-   0        0        0    30449 2021-11-23 06:59:35.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/command.py
--rw-rw-rw-   0        0        0    15322 2021-11-23 06:59:35.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/features.py
--rw-rw-rw-   0        0        0     1104 2021-10-23 02:17:43.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/hmb.py
--rw-rw-rw-   0        0        0    16135 2021-11-23 07:31:19.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/identify.py
--rw-rw-rw-   0        0        0    13915 2021-11-23 06:59:59.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/log_page.py
--rw-rw-rw-   0        0        0     2361 2021-11-12 10:37:37.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/memory.py
--rw-rw-rw-   0        0        0    10510 2021-10-23 02:17:43.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/pcie.py
--rw-rw-rw-   0        0        0    35527 2021-10-23 02:17:43.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/registers.py
--rw-rw-rw-   0        0        0     9095 2021-11-24 06:24:21.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/utility_vu.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/diskpart/
--rw-rw-rw-   0        0        0       56 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/diskpart/__init__.py
--rw-rw-rw-   0        0        0      770 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/diskpart/diskpart.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/fio/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/fio/__init__.py
--rw-rw-rw-   0        0        0    18967 2023-02-23 03:46:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/fio/fio.py
--rw-rw-rw-   0        0        0     5032 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/fio/fio_linux.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/fio/tool/
--rw-rw-rw-   0        0        0  4733892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/fio/tool/fio
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/git/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/git/__init__.py
--rw-rw-rw-   0        0        0     5645 2023-03-02 10:20:30.000000 automation_rest_server-3.6.8/automation_rest_server/tool/git/git_operator.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/iometer/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/iometer/__init__.py
--rw-rw-rw-   0        0        0     9223 2023-02-07 08:25:51.000000 automation_rest_server-3.6.8/automation_rest_server/tool/iometer/iometer.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/utils/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/utils/__init__.py
--rw-rw-rw-   0        0        0    12385 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/utils/buf.py
--rw-rw-rw-   0        0        0     5636 2023-04-10 09:29:00.000000 automation_rest_server-3.6.8/automation_rest_server/utils/firmware_path.py
--rw-rw-rw-   0        0        0     3697 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/utils/log.py
--rw-rw-rw-   0        0        0      386 2023-02-23 02:34:33.000000 automation_rest_server-3.6.8/automation_rest_server/utils/message.py
--rw-rw-rw-   0        0        0     3532 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/utils/nose_xml.py
--rw-rw-rw-   0        0        0     1742 2022-09-20 07:22:33.000000 automation_rest_server-3.6.8/automation_rest_server/utils/pip_operation.py
--rw-rw-rw-   0        0        0     1823 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/utils/process.py
--rw-rw-rw-   0        0        0     9222 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/utils/ssh.py
--rw-rw-rw-   0        0        0     5366 2022-12-22 01:47:58.000000 automation_rest_server-3.6.8/automation_rest_server/utils/system.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server.egg-info/
--rw-rw-rw-   0        0        0      551 2023-05-10 08:47:25.000000 automation_rest_server-3.6.8/automation_rest_server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7003 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 08:47:25.000000 automation_rest_server-3.6.8/automation_rest_server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-10 08:47:25.000000 automation_rest_server-3.6.8/automation_rest_server.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       98 2023-05-10 08:47:25.000000 automation_rest_server-3.6.8/automation_rest_server.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-05-10 08:47:25.000000 automation_rest_server-3.6.8/automation_rest_server.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       64 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/setup.cfg
--rw-rw-rw-   0        0        0     1211 2023-05-10 08:47:20.000000 automation_rest_server-3.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/
+-rw-rw-rw-   0        0        0     1098 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      687 2022-08-30 06:56:12.000000 automation_rest_server-3.6.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      551 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:53.000000 automation_rest_server-3.6.9/automation_rest_server/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/configuration/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/configuration/__init__.py
+-rw-rw-rw-   0        0        0      581 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/configuration/config.yaml
+-rw-rw-rw-   0        0        0     1099 2022-12-13 11:04:16.000000 automation_rest_server-3.6.9/automation_rest_server/configuration/firmware_build.yaml
+-rw-rw-rw-   0        0        0  1333232 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/configuration/pci.ids
+-rw-rw-rw-   0        0        0      157 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/configuration/version.yaml
+-rw-rw-rw-   0        0        0       83 2022-08-25 03:13:17.000000 automation_rest_server-3.6.9/automation_rest_server/configuration/web_server.yaml
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:18:57.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/
+-rw-rw-rw-   0        0        0        0 2022-08-10 09:04:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/models/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:20:01.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/models/__init__.py
+-rw-rw-rw-   0        0        0     4257 2023-05-10 02:20:31.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/models/helper.py
+-rw-rw-rw-   0        0        0     1944 2022-08-17 05:58:24.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/node_resource.py
+-rw-rw-rw-   0        0        0     1374 2022-08-30 04:43:20.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/test_resource.py
+-rw-rw-rw-   0        0        0      340 2022-08-25 03:00:40.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/web_resource.py
+-rw-rw-rw-   0        0        0     2536 2023-02-21 08:02:23.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/web_rest_client.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/__init__.py
+-rw-rw-rw-   0        0        0     1678 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/reset_server.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/__init__.py
+-rw-rw-rw-   0        0        0     2150 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/benchmark_resource.py
+-rw-rw-rw-   0        0        0     1956 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/build_firmware_resource.py
+-rw-rw-rw-   0        0        0      933 2022-12-12 01:57:01.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/git_resource.py
+-rw-rw-rw-   0        0        0      850 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/models/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/models/__init__.py
+-rw-rw-rw-   0        0        0     2044 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/models/ftp_server.py
+-rw-rw-rw-   0        0        0     1732 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/models/helper.py
+-rw-rw-rw-   0        0        0      958 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/oakgate_resource.py
+-rw-rw-rw-   0        0        0      691 2022-08-11 02:31:16.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/operation_resource.py
+-rw-rw-rw-   0        0        0     1641 2022-09-20 01:54:25.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/state_resource.py
+-rw-rw-rw-   0        0        0     1085 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/stop_flag_resource.py
+-rw-rw-rw-   0        0        0     6233 2022-12-03 07:36:31.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/test_resource.py
+-rw-rw-rw-   0        0        0     1295 2023-05-10 02:20:31.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/upgrade_resource.py
+-rw-rw-rw-   0        0        0     6063 2023-05-04 07:05:41.000000 automation_rest_server-3.6.9/automation_rest_server/run.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/__init__.py
+-rw-rw-rw-   0        0        0     6679 2022-09-20 04:46:34.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/database.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/
+-rw-rw-rw-   0        0        0        0 2021-11-12 08:10:50.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/__init__.py
+-rw-rw-rw-   0        0        0     3082 2023-04-19 05:40:44.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/slot.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/
+-rw-rw-rw-   0        0        0        0 2021-11-24 03:48:51.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/__init__.py
+-rw-rw-rw-   0        0        0     1434 2022-09-15 07:43:45.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py
+-rw-rw-rw-   0        0        0     3541 2023-04-17 06:49:22.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py
+-rw-rw-rw-   0        0        0      901 2023-04-19 03:39:13.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py
+-rw-rw-rw-   0        0        0     8894 2023-05-09 09:27:56.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/
+-rw-rw-rw-   0        0        0      214 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/__init__.py
+-rw-rw-rw-   0        0        0     2068 2023-04-25 07:50:43.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/nose_engine.py
+-rw-rw-rw-   0        0        0     4926 2023-02-16 01:39:59.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/oakgate_engine.py
+-rw-rw-rw-   0        0        0     4007 2023-03-02 06:19:25.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/perses_engine.py
+-rw-rw-rw-   0        0        0     1489 2022-09-30 01:53:36.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py
+-rw-rw-rw-   0        0        0      239 2023-04-07 02:04:12.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/special_parameter.py
+-rw-rw-rw-   0        0        0     3562 2022-09-20 07:48:14.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/sse_engine.py
+-rw-rw-rw-   0        0        0     4006 2023-04-25 07:48:48.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/venus_engine.py
+-rw-rw-rw-   0        0        0     1517 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_build.py
+-rw-rw-rw-   0        0        0     3049 2023-05-10 02:58:49.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_download.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/__init__.py
+-rw-rw-rw-   0        0        0     7168 2022-12-13 11:05:02.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py
+-rw-rw-rw-   0        0        0     6196 2023-05-11 07:52:03.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/logic_with_firmware_engine.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/oakgate/
+-rw-rw-rw-   0        0        0        0 2023-04-11 02:31:20.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/oakgate/__init__.py
+-rw-rw-rw-   0        0        0     2925 2023-04-11 02:43:50.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py
+-rw-rw-rw-   0        0        0     2691 2023-04-17 07:35:59.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py
+-rw-rw-rw-   0        0        0      671 2023-05-10 02:30:29.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py
+-rw-rw-rw-   0        0        0     1996 2023-05-10 03:22:37.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py
+-rw-rw-rw-   0        0        0     1585 2023-05-10 02:30:15.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py
+-rw-rw-rw-   0        0        0     2344 2023-04-09 02:31:46.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py
+-rw-rw-rw-   0        0        0     5139 2023-05-10 07:14:09.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/node_database.py
+-rw-rw-rw-   0        0        0    10717 2023-04-19 03:38:41.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/performance_database.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/reboot_engine/
+-rw-rw-rw-   0        0        0       50 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/reboot_engine/__init__.py
+-rw-rw-rw-   0        0        0     2439 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py
+-rw-rw-rw-   0        0        0     2055 2023-05-10 02:51:26.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/state.py
+-rw-rw-rw-   0        0        0      672 2022-12-13 03:29:14.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/status_file.py
+-rw-rw-rw-   0        0        0     5684 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_base.py
+-rw-rw-rw-   0        0        0     1973 2023-02-14 08:06:21.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_benchmark.py
+-rw-rw-rw-   0        0        0     3512 2023-02-07 07:54:27.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_benchmark_group.py
+-rw-rw-rw-   0        0        0     1263 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_case.py
+-rw-rw-rw-   0        0        0    22062 2023-05-10 02:21:32.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_pool.py
+-rw-rw-rw-   0        0        0      892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_reboot_handle.py
+-rw-rw-rw-   0        0        0     4365 2022-12-03 07:44:06.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_result.py
+-rw-rw-rw-   0        0        0     3757 2023-03-02 10:28:02.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_runner.py
+-rw-rw-rw-   0        0        0     4717 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_suite.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/
+-rw-rw-rw-   0        0        0        0 2021-11-12 06:54:04.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/dll/
+-rw-rw-rw-   0        0        0        0 2021-10-23 02:17:43.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/dll/__init__.py
+-rw-rw-rw-   0        0        0    24064 2021-10-23 02:17:43.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/dll/buf.dll
+-rw-rw-rw-   0        0        0    12760 2021-10-23 02:17:43.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/dll/buf.so
+-rw-rw-rw-   0        0        0      777 2021-10-23 02:17:43.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/dll/build.py
+-rw-rw-rw-   0        0        0      861 2022-09-15 07:43:45.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/linux_nvme.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/
+-rw-rw-rw-   0        0        0        0 2021-11-23 06:34:00.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/__init__.py
+-rw-rw-rw-   0        0        0    14077 2021-11-23 06:29:25.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/buf.py
+-rw-rw-rw-   0        0        0     4722 2021-11-23 06:25:09.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/ctype.py
+-rw-rw-rw-   0        0        0    39204 2021-11-23 06:28:50.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/get_feature.py
+-rw-rw-rw-   0        0        0    38547 2022-09-15 07:43:45.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/ioctl.py
+-rw-rw-rw-   0        0        0    23303 2022-09-15 07:42:03.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/nvme.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/
+-rw-rw-rw-   0        0        0      256 2021-11-23 06:21:15.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/__init__.py
+-rw-rw-rw-   0        0        0    30449 2021-11-23 06:59:35.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/command.py
+-rw-rw-rw-   0        0        0    15322 2021-11-23 06:59:35.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/features.py
+-rw-rw-rw-   0        0        0     1104 2021-10-23 02:17:43.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/hmb.py
+-rw-rw-rw-   0        0        0    16135 2021-11-23 07:31:19.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/identify.py
+-rw-rw-rw-   0        0        0    13915 2021-11-23 06:59:59.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/log_page.py
+-rw-rw-rw-   0        0        0     2361 2021-11-12 10:37:37.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/memory.py
+-rw-rw-rw-   0        0        0    10510 2021-10-23 02:17:43.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/pcie.py
+-rw-rw-rw-   0        0        0    35527 2021-10-23 02:17:43.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/registers.py
+-rw-rw-rw-   0        0        0     9095 2021-11-24 06:24:21.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/utility_vu.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/diskpart/
+-rw-rw-rw-   0        0        0       56 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/diskpart/__init__.py
+-rw-rw-rw-   0        0        0      770 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/diskpart/diskpart.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/fio/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/fio/__init__.py
+-rw-rw-rw-   0        0        0    18967 2023-02-23 03:46:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/fio/fio.py
+-rw-rw-rw-   0        0        0     5032 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/fio/fio_linux.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/fio/tool/
+-rw-rw-rw-   0        0        0  4733892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/fio/tool/fio
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/git/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/git/__init__.py
+-rw-rw-rw-   0        0        0     5645 2023-03-02 10:20:30.000000 automation_rest_server-3.6.9/automation_rest_server/tool/git/git_operator.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/iometer/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/iometer/__init__.py
+-rw-rw-rw-   0        0        0     9223 2023-02-07 08:25:51.000000 automation_rest_server-3.6.9/automation_rest_server/tool/iometer/iometer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/utils/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/utils/__init__.py
+-rw-rw-rw-   0        0        0    12385 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/utils/buf.py
+-rw-rw-rw-   0        0        0     5636 2023-04-10 09:29:00.000000 automation_rest_server-3.6.9/automation_rest_server/utils/firmware_path.py
+-rw-rw-rw-   0        0        0     3697 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/utils/log.py
+-rw-rw-rw-   0        0        0      386 2023-02-23 02:34:33.000000 automation_rest_server-3.6.9/automation_rest_server/utils/message.py
+-rw-rw-rw-   0        0        0     3532 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/utils/nose_xml.py
+-rw-rw-rw-   0        0        0     1742 2022-09-20 07:22:33.000000 automation_rest_server-3.6.9/automation_rest_server/utils/pip_operation.py
+-rw-rw-rw-   0        0        0     1823 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/utils/process.py
+-rw-rw-rw-   0        0        0     3157 2023-05-11 07:32:58.000000 automation_rest_server-3.6.9/automation_rest_server/utils/serial_tool.py
+-rw-rw-rw-   0        0        0     9222 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/utils/ssh.py
+-rw-rw-rw-   0        0        0     5366 2022-12-22 01:47:58.000000 automation_rest_server-3.6.9/automation_rest_server/utils/system.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:02:53.000000 automation_rest_server-3.6.9/automation_rest_server.egg-info/
+-rw-rw-rw-   0        0        0      551 2023-05-11 08:02:53.000000 automation_rest_server-3.6.9/automation_rest_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7047 2023-05-11 08:02:53.000000 automation_rest_server-3.6.9/automation_rest_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 08:02:53.000000 automation_rest_server-3.6.9/automation_rest_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-11 08:02:53.000000 automation_rest_server-3.6.9/automation_rest_server.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       98 2023-05-11 08:02:53.000000 automation_rest_server-3.6.9/automation_rest_server.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-05-11 08:02:53.000000 automation_rest_server-3.6.9/automation_rest_server.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       64 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     1211 2023-05-11 08:02:35.000000 automation_rest_server-3.6.9/setup.py
```

### Comparing `automation_rest_server-3.6.8/LICENSE.txt` & `automation_rest_server-3.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/MANIFEST.in` & `automation_rest_server-3.6.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/PKG-INFO` & `automation_rest_server-3.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: automation_rest_server
-Version: 3.6.8
+Version: 3.6.9
 Summary: NVMe production server
 Home-page: https://pypi.org/project/automation_rest_server
 Author: yuwen123441
 Author-email: yuwen123441@126.com
 License: MIT License
 Description: UNKNOWN
 Keywords: runner,server
```

### Comparing `automation_rest_server-3.6.8/automation_rest_server/configuration/config.yaml` & `automation_rest_server-3.6.9/automation_rest_server/configuration/config.yaml`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/configuration/firmware_build.yaml` & `automation_rest_server-3.6.9/automation_rest_server/configuration/firmware_build.yaml`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/configuration/pci.ids` & `automation_rest_server-3.6.9/automation_rest_server/configuration/pci.ids`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/models/helper.py` & `automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/models/helper.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/node_resource.py` & `automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/node_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/test_resource.py` & `automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/test_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/rest_client/web_rest_client.py` & `automation_rest_server-3.6.9/automation_rest_server/rest_client/web_rest_client.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/rest_server/reset_server.py` & `automation_rest_server-3.6.9/automation_rest_server/rest_server/reset_server.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/benchmark_resource.py` & `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/benchmark_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/build_firmware_resource.py` & `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/build_firmware_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/git_resource.py` & `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/git_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py` & `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/models/ftp_server.py` & `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/models/ftp_server.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/models/helper.py` & `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/models/helper.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/oakgate_resource.py` & `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/oakgate_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/operation_resource.py` & `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/operation_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/state_resource.py` & `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/state_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/stop_flag_resource.py` & `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/stop_flag_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/test_resource.py` & `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/test_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/upgrade_resource.py` & `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/upgrade_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/run.py` & `automation_rest_server-3.6.9/automation_rest_server/run.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/database.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/slot.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/nose_engine.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/nose_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/oakgate_engine.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/oakgate_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/perses_engine.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/perses_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/sse_engine.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/sse_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/venus_engine.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/venus_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_build.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_build.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_download.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_download.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/logic_with_firmware_engine.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/logic_with_firmware_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,365 +6,383 @@
 00000050: 6769 742e 6769 745f 6f70 6572 6174 6f72  git.git_operator
 00000060: 2069 6d70 6f72 7420 4769 744f 7065 7261   import GitOpera
 00000070: 746f 720d 0a66 726f 6d20 7574 696c 732e  tor..from utils.
 00000080: 7373 6820 696d 706f 7274 2053 5348 0d0a  ssh import SSH..
 00000090: 6672 6f6d 2075 7469 6c73 2e73 7973 7465  from utils.syste
 000000a0: 6d20 696d 706f 7274 2064 6563 6f72 6174  m import decorat
 000000b0: 655f 6578 6365 7074 696f 6e5f 7265 7375  e_exception_resu
-000000c0: 6c74 0d0a 6672 6f6d 2075 7469 6c73 2069  lt..from utils i
-000000d0: 6d70 6f72 7420 6c6f 670d 0a0d 0a0d 0a63  mport log......c
-000000e0: 6c61 7373 204c 6f67 6963 4657 446f 776e  lass LogicFWDown
-000000f0: 6c6f 6164 6572 286f 626a 6563 7429 3a0d  loader(object):.
-00000100: 0a0d 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
-00000110: 745f 5f28 7365 6c66 293a 0d0a 2020 2020  t__(self):..    
-00000120: 2020 2020 7365 6c66 2e69 635f 6674 7020      self.ic_ftp 
-00000130: 3d20 2231 3732 2e32 392e 302e 3230 3822  = "172.29.0.208"
-00000140: 0d0a 2020 2020 2020 2020 7365 6c66 2e69  ..        self.i
-00000150: 635f 6674 705f 7573 6572 203d 2022 6c61  c_ftp_user = "la
-00000160: 6222 0d0a 2020 2020 2020 2020 7365 6c66  b"..        self
-00000170: 2e69 635f 6674 705f 7077 6420 3d20 226c  .ic_ftp_pwd = "l
-00000180: 6162 220d 0a20 2020 2020 2020 2073 656c  ab"..        sel
-00000190: 662e 6674 705f 7061 7474 656e 203d 2022  f.ftp_patten = "
-000001a0: 6670 6761 2e37 7a22 0d0a 2020 2020 2020  fpga.7z"..      
-000001b0: 2020 7365 6c66 2e6c 6f63 616c 5f66 7470    self.local_ftp
-000001c0: 5f70 6174 6820 3d20 7222 433a 5c70 7275  _path = r"C:\pru
-000001d0: 6e22 0d0a 2020 2020 2020 2020 7365 6c66  n"..        self
-000001e0: 2e6c 6f63 616c 5f66 7470 5f66 7067 615f  .local_ftp_fpga_
-000001f0: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
-00000200: 6f69 6e28 7365 6c66 2e6c 6f63 616c 5f66  oin(self.local_f
-00000210: 7470 5f70 6174 682c 2022 6670 6761 2229  tp_path, "fpga")
-00000220: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00000230: 6f63 616c 5f66 775f 7061 7468 203d 206f  ocal_fw_path = o
-00000240: 732e 7061 7468 2e6a 6f69 6e28 7365 6c66  s.path.join(self
-00000250: 2e6c 6f63 616c 5f66 7470 5f70 6174 682c  .local_ftp_path,
-00000260: 2022 6669 726d 7761 7265 2229 0d0a 2020   "firmware")..  
-00000270: 2020 2020 2020 7365 6c66 2e67 6974 5f75        self.git_u
-00000280: 726c 203d 2022 6874 7470 733a 2f2f 6769  rl = "https://gi
-00000290: 742e 636e 6578 6c61 6273 2e63 6f6d 2f63  t.cnexlabs.com/c
-000002a0: 6e65 782d 6669 726d 7761 7265 2f74 6168  nex-firmware/tah
-000002b0: 6f65 5f66 772e 6769 7422 0d0a 2020 2020  oe_fw.git"..    
-000002c0: 2020 2020 7365 6c66 2e6c 6f63 616c 5f66      self.local_f
-000002d0: 775f 706a 5f70 6174 6820 3d20 7365 6c66  w_pj_path = self
-000002e0: 2e67 6574 5f67 6974 5f70 726f 6a65 6374  .get_git_project
-000002f0: 5f70 6174 6828 290d 0a20 2020 2020 2020  _path()..       
-00000300: 2073 656c 662e 696e 6974 5f6c 6f63 616c   self.init_local
-00000310: 5f66 6f6c 6465 7228 290d 0a0d 0a20 2020  _folder()....   
-00000320: 2064 6566 2069 6e69 745f 6c6f 6361 6c5f   def init_local_
-00000330: 666f 6c64 6572 2873 656c 6629 3a0d 0a20  folder(self):.. 
-00000340: 2020 2020 2020 2069 6e69 745f 7061 7468         init_path
-00000350: 203d 205b 7365 6c66 2e6c 6f63 616c 5f66   = [self.local_f
-00000360: 7470 5f70 6174 682c 2073 656c 662e 6c6f  tp_path, self.lo
-00000370: 6361 6c5f 6674 705f 6670 6761 5f70 6174  cal_ftp_fpga_pat
-00000380: 682c 2073 656c 662e 6c6f 6361 6c5f 6677  h, self.local_fw
-00000390: 5f70 6174 685d 0d0a 2020 2020 2020 2020  _path]..        
-000003a0: 666f 7220 7465 6d70 5f70 6174 6820 696e  for temp_path in
-000003b0: 2069 6e69 745f 7061 7468 3a0d 0a20 2020   init_path:..   
-000003c0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-000003d0: 6f73 2e70 6174 682e 6578 6973 7473 2874  os.path.exists(t
-000003e0: 656d 705f 7061 7468 293a 0d0a 2020 2020  emp_path):..    
-000003f0: 2020 2020 2020 2020 2020 2020 6f73 2e6d              os.m
-00000400: 6b64 6972 2874 656d 705f 7061 7468 290d  kdir(temp_path).
-00000410: 0a0d 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
-00000420: 7468 6f64 0d0a 2020 2020 6465 6620 6973  thod..    def is
-00000430: 5f64 6972 6563 746f 7279 2866 7470 2c20  _directory(ftp, 
-00000440: 7061 7468 293a 0d0a 2020 2020 2020 2020  path):..        
-00000450: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-00000460: 2020 6674 702e 6377 6428 7061 7468 290d    ftp.cwd(path).
-00000470: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00000480: 7572 6e20 5472 7565 0d0a 2020 2020 2020  urn True..      
-00000490: 2020 6578 6365 7074 2066 7470 6c69 622e    except ftplib.
-000004a0: 6572 726f 725f 7065 726d 3a0d 0a20 2020  error_perm:..   
-000004b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000004c0: 4661 6c73 650d 0a0d 0a20 2020 2040 7374  False....    @st
-000004d0: 6174 6963 6d65 7468 6f64 0d0a 2020 2020  aticmethod..    
-000004e0: 6465 6620 756e 7a69 705f 6670 6761 5f66  def unzip_fpga_f
-000004f0: 696c 6528 7a69 705f 7061 7468 293a 0d0a  ile(zip_path):..
-00000500: 2020 2020 2020 2020 7769 7468 2070 7937          with py7
-00000510: 7a72 2e53 6576 656e 5a69 7046 696c 6528  zr.SevenZipFile(
-00000520: 7a69 705f 7061 7468 2c20 6d6f 6465 3d22  zip_path, mode="
-00000530: 7222 2920 6173 207a 3a0d 0a20 2020 2020  r") as z:..     
-00000540: 2020 2020 2020 207a 2e65 7874 7261 6374         z.extract
-00000550: 616c 6c28 7061 7468 3d6f 732e 7061 7468  all(path=os.path
-00000560: 2e64 6972 6e61 6d65 287a 6970 5f70 6174  .dirname(zip_pat
-00000570: 6829 290d 0a20 2020 2020 2020 2075 6e7a  h))..        unz
-00000580: 6970 5f66 6f6c 6465 7220 3d20 6f73 2e70  ip_folder = os.p
-00000590: 6174 682e 7370 6c69 7465 7874 286f 732e  ath.splitext(os.
-000005a0: 7061 7468 2e62 6173 656e 616d 6528 7a69  path.basename(zi
-000005b0: 705f 7061 7468 2929 5b30 5d0d 0a20 2020  p_path))[0]..   
-000005c0: 2020 2020 2075 6e7a 6970 5f66 6f6c 6465       unzip_folde
-000005d0: 725f 7061 7468 203d 206f 732e 7061 7468  r_path = os.path
-000005e0: 2e6a 6f69 6e28 6f73 2e70 6174 682e 6469  .join(os.path.di
-000005f0: 726e 616d 6528 7a69 705f 7061 7468 292c  rname(zip_path),
-00000600: 2075 6e7a 6970 5f66 6f6c 6465 7229 0d0a   unzip_folder)..
-00000610: 2020 2020 2020 2020 666f 7220 7465 6d70          for temp
-00000620: 2069 6e20 6f73 2e6c 6973 7464 6972 2875   in os.listdir(u
-00000630: 6e7a 6970 5f66 6f6c 6465 725f 7061 7468  nzip_folder_path
-00000640: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00000650: 6966 2074 656d 702e 656e 6473 7769 7468  if temp.endswith
-00000660: 2822 2e73 6f66 2229 3a0d 0a20 2020 2020  (".sof"):..     
-00000670: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00000680: 6e20 6f73 2e70 6174 682e 6a6f 696e 2875  n os.path.join(u
-00000690: 6e7a 6970 5f66 6f6c 6465 725f 7061 7468  nzip_folder_path
-000006a0: 2c20 7465 6d70 290d 0a0d 0a20 2020 2064  , temp)....    d
-000006b0: 6566 2066 7470 5f64 6f77 6e6c 6f61 645f  ef ftp_download_
-000006c0: 6669 6c65 2873 656c 662c 2066 7470 2c20  file(self, ftp, 
-000006d0: 6670 6761 5f66 6f6c 6465 722c 2066 7067  fpga_folder, fpg
-000006e0: 615f 6669 6c65 293a 0d0a 2020 2020 2020  a_file):..      
-000006f0: 2020 6c6f 6361 6c5f 7061 7468 203d 206f    local_path = o
-00000700: 732e 7061 7468 2e6a 6f69 6e28 7365 6c66  s.path.join(self
-00000710: 2e6c 6f63 616c 5f66 7470 5f66 7067 615f  .local_ftp_fpga_
-00000720: 7061 7468 2c20 6670 6761 5f66 6f6c 6465  path, fpga_folde
-00000730: 7229 0d0a 2020 2020 2020 2020 6966 206f  r)..        if o
-00000740: 732e 7061 7468 2e65 7869 7374 7328 6c6f  s.path.exists(lo
-00000750: 6361 6c5f 7061 7468 293a 0d0a 2020 2020  cal_path):..    
-00000760: 2020 2020 2020 2020 7368 7574 696c 2e72          shutil.r
-00000770: 6d74 7265 6528 6c6f 6361 6c5f 7061 7468  mtree(local_path
-00000780: 290d 0a20 2020 2020 2020 206f 732e 6d6b  )..        os.mk
-00000790: 6469 7228 6c6f 6361 6c5f 7061 7468 290d  dir(local_path).
-000007a0: 0a20 2020 2020 2020 206c 6f63 616c 5f66  .        local_f
-000007b0: 7067 615f 6669 6c65 203d 206f 732e 7061  pga_file = os.pa
-000007c0: 7468 2e6a 6f69 6e28 6c6f 6361 6c5f 7061  th.join(local_pa
-000007d0: 7468 2c20 6670 6761 5f66 696c 6529 0d0a  th, fpga_file)..
-000007e0: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-000007f0: 6e28 6c6f 6361 6c5f 6670 6761 5f66 696c  n(local_fpga_fil
-00000800: 652c 2027 7762 2729 2061 7320 663a 0d0a  e, 'wb') as f:..
-00000810: 2020 2020 2020 2020 2020 2020 6674 702e              ftp.
-00000820: 7265 7472 6269 6e61 7279 2866 2752 4554  retrbinary(f'RET
-00000830: 5220 7b66 7067 615f 6669 6c65 7d27 2c20  R {fpga_file}', 
-00000840: 662e 7772 6974 6529 0d0a 2020 2020 2020  f.write)..      
-00000850: 2020 7265 7475 726e 206c 6f63 616c 5f66    return local_f
-00000860: 7067 615f 6669 6c65 0d0a 0d0a 2020 2020  pga_file....    
-00000870: 6465 6620 5f67 6574 5f66 696c 655f 6e61  def _get_file_na
-00000880: 6d65 2873 656c 662c 2066 7470 293a 0d0a  me(self, ftp):..
-00000890: 2020 2020 2020 2020 6670 6761 5f66 696c          fpga_fil
-000008a0: 6520 3d20 4e6f 6e65 0d0a 2020 2020 2020  e = None..      
-000008b0: 2020 6669 6c65 6e61 6d65 7320 3d20 6674    filenames = ft
-000008c0: 702e 6e6c 7374 2829 0d0a 2020 2020 2020  p.nlst()..      
-000008d0: 2020 666f 7220 6669 6c65 5f20 696e 2066    for file_ in f
-000008e0: 696c 656e 616d 6573 3a0d 0a20 2020 2020  ilenames:..     
-000008f0: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
-00000900: 7470 5f70 6174 7465 6e20 696e 2066 696c  tp_patten in fil
-00000910: 655f 3a0d 0a20 2020 2020 2020 2020 2020  e_:..           
-00000920: 2020 2020 2066 7067 615f 6669 6c65 203d       fpga_file =
-00000930: 2066 696c 655f 0d0a 2020 2020 2020 2020   file_..        
-00000940: 2020 2020 2020 2020 6272 6561 6b0d 0a20          break.. 
-00000950: 2020 2020 2020 2072 6574 7572 6e20 6670         return fp
-00000960: 6761 5f66 696c 650d 0a0d 0a20 2020 2064  ga_file....    d
-00000970: 6566 2073 706c 6974 5f70 6174 685f 666f  ef split_path_fo
-00000980: 6c64 6572 5f66 696c 6528 7365 6c66 2c20  lder_file(self, 
-00000990: 6674 702c 2066 7470 5f70 6174 6829 3a0d  ftp, ftp_path):.
-000009a0: 0a20 2020 2020 2020 2066 7470 5f70 6174  .        ftp_pat
-000009b0: 6820 3d20 6674 705f 7061 7468 2e72 6570  h = ftp_path.rep
-000009c0: 6c61 6365 2866 2266 7470 3a2f 2f7b 7365  lace(f"ftp://{se
-000009d0: 6c66 2e69 635f 6674 707d 2f22 2c20 2222  lf.ic_ftp}/", ""
-000009e0: 290d 0a20 2020 2020 2020 2073 706c 6974  )..        split
-000009f0: 5f70 6174 6873 203d 2066 7470 5f70 6174  _paths = ftp_pat
-00000a00: 682e 7370 6c69 7428 222f 2229 0d0a 2020  h.split("/")..  
-00000a10: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00000a20: 662e 6973 5f64 6972 6563 746f 7279 2866  f.is_directory(f
-00000a30: 7470 2c20 6674 705f 7061 7468 293a 0d0a  tp, ftp_path):..
-00000a40: 2020 2020 2020 2020 2020 2020 6670 6761              fpga
-00000a50: 5f66 696c 6520 3d20 7370 6c69 745f 7061  _file = split_pa
-00000a60: 7468 735b 2d31 5d0d 0a20 2020 2020 2020  ths[-1]..       
-00000a70: 2020 2020 2066 7067 615f 666f 6c64 6572       fpga_folder
-00000a80: 203d 2073 706c 6974 5f70 6174 6873 5b2d   = split_paths[-
-00000a90: 325d 0d0a 2020 2020 2020 2020 2020 2020  2]..            
-00000aa0: 6674 702e 6377 6428 6f73 2e70 6174 682e  ftp.cwd(os.path.
-00000ab0: 6469 726e 616d 6528 6674 705f 7061 7468  dirname(ftp_path
-00000ac0: 2929 0d0a 2020 2020 2020 2020 656c 7365  ))..        else
-00000ad0: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
-00000ae0: 7067 615f 666f 6c64 6572 203d 2073 706c  pga_folder = spl
-00000af0: 6974 5f70 6174 6873 5b2d 315d 2069 6620  it_paths[-1] if 
-00000b00: 7370 6c69 745f 7061 7468 735b 2d31 5d20  split_paths[-1] 
-00000b10: 213d 2022 2220 656c 7365 2073 706c 6974  != "" else split
-00000b20: 5f70 6174 6873 5b2d 325d 0d0a 2020 2020  _paths[-2]..    
-00000b30: 2020 2020 2020 2020 6670 6761 5f66 696c          fpga_fil
-00000b40: 6520 3d20 7365 6c66 2e5f 6765 745f 6669  e = self._get_fi
-00000b50: 6c65 5f6e 616d 6528 6674 7029 0d0a 2020  le_name(ftp)..  
-00000b60: 2020 2020 2020 7265 7475 726e 2066 7067        return fpg
-00000b70: 615f 666f 6c64 6572 2c20 6670 6761 5f66  a_folder, fpga_f
-00000b80: 696c 650d 0a0d 0a20 2020 2064 6566 2067  ile....    def g
-00000b90: 6574 5f66 7067 615f 6672 6f6d 5f66 7470  et_fpga_from_ftp
-00000ba0: 2873 656c 662c 2066 7470 5f70 6174 6829  (self, ftp_path)
-00000bb0: 3a0d 0a20 2020 2020 2020 206c 6f67 2e49  :..        log.I
-00000bc0: 4e46 4f28 6622 4265 6769 6e20 746f 2067  NFO(f"Begin to g
-00000bd0: 6574 2073 6f66 2066 726f 6d20 7b66 7470  et sof from {ftp
-00000be0: 5f70 6174 687d 2229 0d0a 2020 2020 2020  _path}")..      
-00000bf0: 2020 6674 7020 3d20 6674 706c 6962 2e46    ftp = ftplib.F
-00000c00: 5450 2873 656c 662e 6963 5f66 7470 2c20  TP(self.ic_ftp, 
-00000c10: 7365 6c66 2e69 635f 6674 705f 7573 6572  self.ic_ftp_user
-00000c20: 2c20 7365 6c66 2e69 635f 6674 705f 7077  , self.ic_ftp_pw
-00000c30: 6429 0d0a 2020 2020 2020 2020 6670 6761  d)..        fpga
-00000c40: 5f66 6f6c 6465 722c 2066 7067 615f 6669  _folder, fpga_fi
-00000c50: 6c65 203d 2073 656c 662e 7370 6c69 745f  le = self.split_
-00000c60: 7061 7468 5f66 6f6c 6465 725f 6669 6c65  path_folder_file
-00000c70: 2866 7470 2c20 6674 705f 7061 7468 290d  (ftp, ftp_path).
-00000c80: 0a20 2020 2020 2020 2064 6c5f 6670 6761  .        dl_fpga
-00000c90: 5f70 6174 6820 3d20 7365 6c66 2e66 7470  _path = self.ftp
-00000ca0: 5f64 6f77 6e6c 6f61 645f 6669 6c65 2866  _download_file(f
-00000cb0: 7470 2c20 6670 6761 5f66 6f6c 6465 722c  tp, fpga_folder,
-00000cc0: 2066 7067 615f 6669 6c65 290d 0a20 2020   fpga_file)..   
-00000cd0: 2020 2020 2073 6f66 5f66 696c 6520 3d20       sof_file = 
-00000ce0: 7365 6c66 2e75 6e7a 6970 5f66 7067 615f  self.unzip_fpga_
-00000cf0: 6669 6c65 2864 6c5f 6670 6761 5f70 6174  file(dl_fpga_pat
-00000d00: 6829 0d0a 2020 2020 2020 2020 6c6f 672e  h)..        log.
-00000d10: 494e 464f 2866 2247 6574 2073 6f66 207b  INFO(f"Get sof {
-00000d20: 736f 665f 6669 6c65 7d20 6672 6f6d 2066  sof_file} from f
-00000d30: 7470 2229 0d0a 2020 2020 2020 2020 6674  tp")..        ft
-00000d40: 702e 7175 6974 2829 0d0a 2020 2020 2020  p.quit()..      
-00000d50: 2020 6966 2073 6f66 5f66 696c 6520 6973    if sof_file is
-00000d60: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00000d70: 2020 2020 7261 6973 6520 5275 6e74 696d      raise Runtim
-00000d80: 6545 7272 6f72 2866 2273 6f66 5f66 696c  eError(f"sof_fil
-00000d90: 6520 6765 7420 6661 696c 6564 3a20 7b66  e get failed: {f
-00000da0: 7470 5f70 6174 687d 2229 0d0a 2020 2020  tp_path}")..    
-00000db0: 2020 2020 7265 7475 726e 2073 6f66 5f66      return sof_f
-00000dc0: 696c 650d 0a0d 0a20 2020 2064 6566 2067  ile....    def g
-00000dd0: 6574 5f67 6974 5f70 726f 6a65 6374 5f70  et_git_project_p
-00000de0: 6174 6828 7365 6c66 293a 0d0a 2020 2020  ath(self):..    
-00000df0: 2020 2020 6261 7365 6e61 6d65 203d 206f      basename = o
-00000e00: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
-00000e10: 7365 6c66 2e67 6974 5f75 726c 290d 0a20  self.git_url).. 
-00000e20: 2020 2020 2020 2066 6f6c 6465 725f 6e61         folder_na
-00000e30: 6d65 203d 206f 732e 7061 7468 2e73 706c  me = os.path.spl
-00000e40: 6974 6578 7428 6261 7365 6e61 6d65 295b  itext(basename)[
-00000e50: 305d 0d0a 2020 2020 2020 2020 7265 7475  0]..        retu
-00000e60: 726e 206f 732e 7061 7468 2e6a 6f69 6e28  rn os.path.join(
-00000e70: 7365 6c66 2e6c 6f63 616c 5f66 775f 7061  self.local_fw_pa
-00000e80: 7468 2c20 666f 6c64 6572 5f6e 616d 6529  th, folder_name)
-00000e90: 0d0a 0d0a 2020 2020 6465 6620 7570 6461  ....    def upda
-00000ea0: 7465 5f66 775f 636f 6465 2873 656c 662c  te_fw_code(self,
-00000eb0: 2062 7261 6e63 6829 3a0d 0a20 2020 2020   branch):..     
-00000ec0: 2020 206c 6f63 616c 5f66 775f 7061 7468     local_fw_path
-00000ed0: 203d 2073 656c 662e 6c6f 6361 6c5f 6677   = self.local_fw
-00000ee0: 5f70 6a5f 7061 7468 2069 6620 6f73 2e70  _pj_path if os.p
-00000ef0: 6174 682e 6578 6973 7473 2873 656c 662e  ath.exists(self.
-00000f00: 6c6f 6361 6c5f 6677 5f70 6a5f 7061 7468  local_fw_pj_path
-00000f10: 2920 656c 7365 2073 656c 662e 6c6f 6361  ) else self.loca
-00000f20: 6c5f 6677 5f70 6174 680d 0a20 2020 2020  l_fw_path..     
-00000f30: 2020 2067 6974 203d 2047 6974 4f70 6572     git = GitOper
-00000f40: 6174 6f72 2822 7368 616f 6269 6e2e 7368  ator("shaobin.sh
-00000f50: 7522 2c20 2243 6e65 7821 3230 3234 222c  u", "Cnex!2024",
-00000f60: 206c 6f63 616c 5f66 775f 7061 7468 290d   local_fw_path).
-00000f70: 0a20 2020 2020 2020 2069 6620 6f73 2e70  .        if os.p
-00000f80: 6174 682e 6578 6973 7473 2873 656c 662e  ath.exists(self.
-00000f90: 6c6f 6361 6c5f 6677 5f70 6a5f 7061 7468  local_fw_pj_path
-00000fa0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00000fb0: 6e65 775f 6d73 672c 2072 6574 203d 2067  new_msg, ret = g
-00000fc0: 6974 2e75 7064 6174 655f 6c61 7465 7374  it.update_latest
-00000fd0: 5f63 6f64 6528 6622 6f72 6967 696e 2f7b  _code(f"origin/{
-00000fe0: 6272 616e 6368 7d22 290d 0a20 2020 2020  branch}")..     
-00000ff0: 2020 2020 2020 2069 6620 7265 7420 213d         if ret !=
-00001000: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-00001010: 2020 2020 2072 6169 7365 2052 756e 7469       raise Runti
-00001020: 6d65 4572 726f 7228 6622 4769 7420 7570  meError(f"Git up
-00001030: 6461 7465 2066 6169 6c65 642c 2075 726c  date failed, url
-00001040: 3a7b 7365 6c66 2e67 6974 5f75 726c 7d20  :{self.git_url} 
-00001050: 6272 616e 6368 3a7b 6272 616e 6368 7d22  branch:{branch}"
-00001060: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
-00001070: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00001080: 2067 6974 2e63 6c6f 6e65 2873 656c 662e   git.clone(self.
-00001090: 6769 745f 7572 6c2c 2066 226f 7269 6769  git_url, f"origi
-000010a0: 6e2f 7b62 7261 6e63 687d 2229 2021 3d20  n/{branch}") != 
-000010b0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-000010c0: 2020 2020 7261 6973 6520 5275 6e74 696d      raise Runtim
-000010d0: 6545 7272 6f72 2866 2247 6974 2063 6c6f  eError(f"Git clo
-000010e0: 6e65 2066 6169 6c65 642c 2075 726c 3a7b  ne failed, url:{
-000010f0: 7365 6c66 2e67 6974 5f75 726c 7d20 6272  self.git_url} br
-00001100: 616e 6368 3a7b 6272 616e 6368 7d22 290d  anch:{branch}").
-00001110: 0a0d 0a20 2020 2064 6566 2063 6f70 795f  ...    def copy_
-00001120: 736f 665f 325f 6677 2873 656c 662c 2073  sof_2_fw(self, s
-00001130: 7263 5f73 6f66 293a 0d0a 2020 2020 2020  rc_sof):..      
-00001140: 2020 6473 745f 736f 6620 3d20 6f73 2e70    dst_sof = os.p
-00001150: 6174 682e 6a6f 696e 2873 656c 662e 6c6f  ath.join(self.lo
-00001160: 6361 6c5f 6677 5f70 6a5f 7061 7468 2c20  cal_fw_pj_path, 
-00001170: 2274 6168 6f65 2e73 6f66 2229 0d0a 2020  "tahoe.sof")..  
-00001180: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
-00001190: 2e65 7869 7374 7328 6473 745f 736f 6629  .exists(dst_sof)
-000011a0: 3a0d 0a20 2020 2020 2020 2020 2020 206f  :..            o
-000011b0: 732e 7265 6d6f 7665 2864 7374 5f73 6f66  s.remove(dst_sof
-000011c0: 290d 0a20 2020 2020 2020 2073 6875 7469  )..        shuti
-000011d0: 6c2e 636f 7079 2873 7263 5f73 6f66 2c20  l.copy(src_sof, 
-000011e0: 6473 745f 736f 6629 0d0a 0d0a 2020 2020  dst_sof)....    
-000011f0: 6465 6620 6c6f 6164 5f61 6c6c 2873 656c  def load_all(sel
-00001200: 6629 3a0d 0a20 2020 2020 2020 2063 6d64  f):..        cmd
-00001210: 203d 2066 2263 6420 2f64 207b 7365 6c66   = f"cd /d {self
-00001220: 2e6c 6f63 616c 5f66 775f 706a 5f70 6174  .local_fw_pj_pat
-00001230: 687d 2026 2620 6c6f 6164 5f61 6c6c 2e62  h} && load_all.b
-00001240: 6174 220d 0a20 2020 2020 2020 206c 6f67  at"..        log
-00001250: 2e49 4e46 4f28 6622 7570 6772 6164 6520  .INFO(f"upgrade 
-00001260: 6c6f 6769 6320 616e 6420 6669 726d 7761  logic and firmwa
-00001270: 7265 2077 6974 6820 636d 643a 207b 636d  re with cmd: {cm
-00001280: 647d 2229 0d0a 2020 2020 2020 2020 7265  d}")..        re
-00001290: 7420 3d20 6f73 2e73 7973 7465 6d28 636d  t = os.system(cm
-000012a0: 6429 0d0a 2020 2020 2020 2020 6966 2072  d)..        if r
-000012b0: 6574 2021 3d20 303a 0d0a 2020 2020 2020  et != 0:..      
-000012c0: 2020 2020 2020 7261 6973 6520 5275 6e74        raise Runt
-000012d0: 696d 6545 7272 6f72 2822 6c6f 6164 5f61  imeError("load_a
-000012e0: 6c6c 2066 6169 6c65 6422 290d 0a20 2020  ll failed")..   
-000012f0: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
-00001300: 3630 290d 0a0d 0a20 2020 2064 6566 2069  60)....    def i
-00001310: 6e73 6d6f 645f 6b6f 2873 656c 662c 2073  nsmod_ko(self, s
-00001320: 7368 2c20 7665 6e75 7329 3a0d 0a20 2020  sh, venus):..   
-00001330: 2020 2020 206b 6f5f 7061 7468 203d 2066       ko_path = f
-00001340: 227b 7665 6e75 737d 2f62 696e 2f74 6168  "{venus}/bin/tah
-00001350: 6f65 2f71 615f 6d6f 6465 220d 0a20 2020  oe/qa_mode"..   
-00001360: 2020 2020 2063 6d64 203d 2066 2263 6420       cmd = f"cd 
-00001370: 7b6b 6f5f 7061 7468 7d20 2626 2069 6e73  {ko_path} && ins
-00001380: 6d6f 6420 6e65 7875 732e 6b6f 2026 2620  mod nexus.ko && 
-00001390: 696e 736d 6f64 206b 7465 7374 2e6b 6f22  insmod ktest.ko"
-000013a0: 0d0a 2020 2020 2020 2020 7374 6174 7573  ..        status
-000013b0: 2c20 6f75 7470 7574 203d 2073 7368 2e63  , output = ssh.c
-000013c0: 6f6d 6d61 6e64 2863 6d64 290d 0a20 2020  ommand(cmd)..   
-000013d0: 2020 2020 2069 6620 7374 6174 7573 2021       if status !
-000013e0: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
-000013f0: 2020 7261 6973 6520 5275 6e74 696d 6545    raise RuntimeE
-00001400: 7272 6f72 2866 2269 6e73 6d6f 6420 6661  rror(f"insmod fa
-00001410: 696c 6564 2c20 636d 643a 207b 636d 647d  iled, cmd: {cmd}
-00001420: 2e20 4f75 7470 7574 3a7b 6f75 7470 7574  . Output:{output
-00001430: 7d22 290d 0a0d 0a20 2020 2064 6566 2072  }")....    def r
-00001440: 6562 6f6f 745f 6c69 6e75 7828 7365 6c66  eboot_linux(self
-00001450: 2c20 6c69 6e75 782c 2075 7365 722c 2070  , linux, user, p
-00001460: 7764 2c20 7665 6e75 735f 7061 7468 293a  wd, venus_path):
-00001470: 0d0a 2020 2020 2020 2020 7373 6820 3d20  ..        ssh = 
-00001480: 5353 4828 6c69 6e75 782c 2075 7365 726e  SSH(linux, usern
-00001490: 616d 653d 7573 6572 2c20 7061 7373 776f  ame=user, passwo
-000014a0: 7264 3d70 7764 290d 0a20 2020 2020 2020  rd=pwd)..       
-000014b0: 2073 7368 2e6f 7065 6e28 290d 0a20 2020   ssh.open()..   
-000014c0: 2020 2020 2073 7368 2e63 6f6d 6d61 6e64       ssh.command
-000014d0: 5f77 6974 686f 7574 5f72 6573 756c 7428  _without_result(
-000014e0: 2272 6562 6f6f 7420 2d6e 6622 2c20 7469  "reboot -nf", ti
-000014f0: 6d65 6f75 743d 3130 290d 0a20 2020 2020  meout=10)..     
-00001500: 2020 2074 696d 652e 736c 6565 7028 3630     time.sleep(60
-00001510: 290d 0a20 2020 2020 2020 2073 7368 2e6f  )..        ssh.o
-00001520: 7065 6e28 290d 0a20 2020 2020 2020 2073  pen()..        s
-00001530: 656c 662e 696e 736d 6f64 5f6b 6f28 7373  elf.insmod_ko(ss
-00001540: 682c 2076 656e 7573 5f70 6174 6829 0d0a  h, venus_path)..
-00001550: 0d0a 2020 2020 4064 6563 6f72 6174 655f  ..    @decorate_
-00001560: 6578 6365 7074 696f 6e5f 7265 7375 6c74  exception_result
-00001570: 0d0a 2020 2020 6465 6620 7275 6e28 7365  ..    def run(se
-00001580: 6c66 2c20 7061 7261 293a 0d0a 2020 2020  lf, para):..    
-00001590: 2020 2020 6c6f 672e 494e 464f 2822 4265      log.INFO("Be
-000015a0: 6769 6e20 746f 2064 6f77 6e6c 6f61 6420  gin to download 
-000015b0: 6c6f 6769 6320 616e 6420 6669 726d 7761  logic and firmwa
-000015c0: 7265 2229 0d0a 2020 2020 2020 2020 7372  re")..        sr
-000015d0: 635f 736f 6620 3d20 7365 6c66 2e67 6574  c_sof = self.get
-000015e0: 5f66 7067 615f 6672 6f6d 5f66 7470 2870  _fpga_from_ftp(p
-000015f0: 6172 615b 2269 635f 6c6f 6769 6322 5d29  ara["ic_logic"])
-00001600: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-00001610: 7064 6174 655f 6677 5f63 6f64 6528 7061  pdate_fw_code(pa
-00001620: 7261 5b22 6963 5f66 775f 6272 616e 6368  ra["ic_fw_branch
-00001630: 225d 290d 0a20 2020 2020 2020 2073 656c  "])..        sel
-00001640: 662e 636f 7079 5f73 6f66 5f32 5f66 7728  f.copy_sof_2_fw(
-00001650: 7372 635f 736f 6629 0d0a 2020 2020 2020  src_sof)..      
-00001660: 2020 7365 6c66 2e6c 6f61 645f 616c 6c28    self.load_all(
-00001670: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00001680: 7265 626f 6f74 5f6c 696e 7578 2870 6172  reboot_linux(par
-00001690: 615b 2274 6172 6765 745f 6970 225d 2c20  a["target_ip"], 
-000016a0: 7061 7261 5b22 6c69 6e75 785f 7573 6572  para["linux_user
-000016b0: 225d 2c20 7061 7261 5b22 6c69 6e75 785f  "], para["linux_
-000016c0: 7077 6422 5d2c 2070 6172 615b 2277 6f72  pwd"], para["wor
-000016d0: 6b5f 7061 7468 225d 290d 0a20 2020 2020  k_path"])..     
-000016e0: 2020 2072 6574 7572 6e20 302c 2022 646f     return 0, "do
-000016f0: 776e 6c6f 6164 206c 6f67 6963 2061 6e64  wnload logic and
-00001700: 2066 6972 6d77 6172 6520 7375 6363 6565   firmware succee
-00001710: 6422 0d0a                                d"..
+000000c0: 6c74 0d0a 6672 6f6d 2075 7469 6c73 2e73  lt..from utils.s
+000000d0: 6572 6961 6c5f 746f 6f6c 2069 6d70 6f72  erial_tool impor
+000000e0: 7420 436e 6578 5365 7269 616c 0d0a 6672  t CnexSerial..fr
+000000f0: 6f6d 2075 7469 6c73 2069 6d70 6f72 7420  om utils import 
+00000100: 6c6f 670d 0a0d 0a0d 0a63 6c61 7373 204c  log......class L
+00000110: 6f67 6963 4657 446f 776e 6c6f 6164 6572  ogicFWDownloader
+00000120: 286f 626a 6563 7429 3a0d 0a0d 0a20 2020  (object):....   
+00000130: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00000140: 6c66 293a 0d0a 2020 2020 2020 2020 7365  lf):..        se
+00000150: 6c66 2e69 635f 6674 7020 3d20 2231 3732  lf.ic_ftp = "172
+00000160: 2e32 392e 302e 3230 3822 0d0a 2020 2020  .29.0.208"..    
+00000170: 2020 2020 7365 6c66 2e69 635f 6674 705f      self.ic_ftp_
+00000180: 7573 6572 203d 2022 6c61 6222 0d0a 2020  user = "lab"..  
+00000190: 2020 2020 2020 7365 6c66 2e69 635f 6674        self.ic_ft
+000001a0: 705f 7077 6420 3d20 226c 6162 220d 0a20  p_pwd = "lab".. 
+000001b0: 2020 2020 2020 2073 656c 662e 6674 705f         self.ftp_
+000001c0: 7061 7474 656e 203d 2022 6670 6761 2e37  patten = "fpga.7
+000001d0: 7a22 0d0a 2020 2020 2020 2020 7365 6c66  z"..        self
+000001e0: 2e6c 6f63 616c 5f66 7470 5f70 6174 6820  .local_ftp_path 
+000001f0: 3d20 7222 433a 5c70 7275 6e22 0d0a 2020  = r"C:\prun"..  
+00000200: 2020 2020 2020 7365 6c66 2e6c 6f63 616c        self.local
+00000210: 5f66 7470 5f66 7067 615f 7061 7468 203d  _ftp_fpga_path =
+00000220: 206f 732e 7061 7468 2e6a 6f69 6e28 7365   os.path.join(se
+00000230: 6c66 2e6c 6f63 616c 5f66 7470 5f70 6174  lf.local_ftp_pat
+00000240: 682c 2022 6670 6761 2229 0d0a 2020 2020  h, "fpga")..    
+00000250: 2020 2020 7365 6c66 2e6c 6f63 616c 5f66      self.local_f
+00000260: 775f 7061 7468 203d 206f 732e 7061 7468  w_path = os.path
+00000270: 2e6a 6f69 6e28 7365 6c66 2e6c 6f63 616c  .join(self.local
+00000280: 5f66 7470 5f70 6174 682c 2022 6669 726d  _ftp_path, "firm
+00000290: 7761 7265 2229 0d0a 2020 2020 2020 2020  ware")..        
+000002a0: 7365 6c66 2e67 6974 5f75 726c 203d 2022  self.git_url = "
+000002b0: 6874 7470 733a 2f2f 6769 742e 636e 6578  https://git.cnex
+000002c0: 6c61 6273 2e63 6f6d 2f63 6e65 782d 6669  labs.com/cnex-fi
+000002d0: 726d 7761 7265 2f74 6168 6f65 5f66 772e  rmware/tahoe_fw.
+000002e0: 6769 7422 0d0a 2020 2020 2020 2020 7365  git"..        se
+000002f0: 6c66 2e6c 6f63 616c 5f66 775f 706a 5f70  lf.local_fw_pj_p
+00000300: 6174 6820 3d20 7365 6c66 2e67 6574 5f67  ath = self.get_g
+00000310: 6974 5f70 726f 6a65 6374 5f70 6174 6828  it_project_path(
+00000320: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00000330: 696e 6974 5f6c 6f63 616c 5f66 6f6c 6465  init_local_folde
+00000340: 7228 290d 0a0d 0a20 2020 2064 6566 2069  r()....    def i
+00000350: 6e69 745f 6c6f 6361 6c5f 666f 6c64 6572  nit_local_folder
+00000360: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00000370: 2069 6e69 745f 7061 7468 203d 205b 7365   init_path = [se
+00000380: 6c66 2e6c 6f63 616c 5f66 7470 5f70 6174  lf.local_ftp_pat
+00000390: 682c 2073 656c 662e 6c6f 6361 6c5f 6674  h, self.local_ft
+000003a0: 705f 6670 6761 5f70 6174 682c 2073 656c  p_fpga_path, sel
+000003b0: 662e 6c6f 6361 6c5f 6677 5f70 6174 685d  f.local_fw_path]
+000003c0: 0d0a 2020 2020 2020 2020 666f 7220 7465  ..        for te
+000003d0: 6d70 5f70 6174 6820 696e 2069 6e69 745f  mp_path in init_
+000003e0: 7061 7468 3a0d 0a20 2020 2020 2020 2020  path:..         
+000003f0: 2020 2069 6620 6e6f 7420 6f73 2e70 6174     if not os.pat
+00000400: 682e 6578 6973 7473 2874 656d 705f 7061  h.exists(temp_pa
+00000410: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
+00000420: 2020 2020 2020 6f73 2e6d 6b64 6972 2874        os.mkdir(t
+00000430: 656d 705f 7061 7468 290d 0a0d 0a20 2020  emp_path)....   
+00000440: 2040 7374 6174 6963 6d65 7468 6f64 0d0a   @staticmethod..
+00000450: 2020 2020 6465 6620 6973 5f64 6972 6563      def is_direc
+00000460: 746f 7279 2866 7470 2c20 7061 7468 293a  tory(ftp, path):
+00000470: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
+00000480: 2020 2020 2020 2020 2020 2020 6674 702e              ftp.
+00000490: 6377 6428 7061 7468 290d 0a20 2020 2020  cwd(path)..     
+000004a0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+000004b0: 7565 0d0a 2020 2020 2020 2020 6578 6365  ue..        exce
+000004c0: 7074 2066 7470 6c69 622e 6572 726f 725f  pt ftplib.error_
+000004d0: 7065 726d 3a0d 0a20 2020 2020 2020 2020  perm:..         
+000004e0: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
+000004f0: 0a0d 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
+00000500: 7468 6f64 0d0a 2020 2020 6465 6620 756e  thod..    def un
+00000510: 7a69 705f 6670 6761 5f66 696c 6528 7a69  zip_fpga_file(zi
+00000520: 705f 7061 7468 293a 0d0a 2020 2020 2020  p_path):..      
+00000530: 2020 7769 7468 2070 7937 7a72 2e53 6576    with py7zr.Sev
+00000540: 656e 5a69 7046 696c 6528 7a69 705f 7061  enZipFile(zip_pa
+00000550: 7468 2c20 6d6f 6465 3d22 7222 2920 6173  th, mode="r") as
+00000560: 207a 3a0d 0a20 2020 2020 2020 2020 2020   z:..           
+00000570: 207a 2e65 7874 7261 6374 616c 6c28 7061   z.extractall(pa
+00000580: 7468 3d6f 732e 7061 7468 2e64 6972 6e61  th=os.path.dirna
+00000590: 6d65 287a 6970 5f70 6174 6829 290d 0a20  me(zip_path)).. 
+000005a0: 2020 2020 2020 2075 6e7a 6970 5f66 6f6c         unzip_fol
+000005b0: 6465 7220 3d20 6f73 2e70 6174 682e 7370  der = os.path.sp
+000005c0: 6c69 7465 7874 286f 732e 7061 7468 2e62  litext(os.path.b
+000005d0: 6173 656e 616d 6528 7a69 705f 7061 7468  asename(zip_path
+000005e0: 2929 5b30 5d0d 0a20 2020 2020 2020 2075  ))[0]..        u
+000005f0: 6e7a 6970 5f66 6f6c 6465 725f 7061 7468  nzip_folder_path
+00000600: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+00000610: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
+00000620: 7a69 705f 7061 7468 292c 2075 6e7a 6970  zip_path), unzip
+00000630: 5f66 6f6c 6465 7229 0d0a 2020 2020 2020  _folder)..      
+00000640: 2020 666f 7220 7465 6d70 2069 6e20 6f73    for temp in os
+00000650: 2e6c 6973 7464 6972 2875 6e7a 6970 5f66  .listdir(unzip_f
+00000660: 6f6c 6465 725f 7061 7468 293a 0d0a 2020  older_path):..  
+00000670: 2020 2020 2020 2020 2020 6966 2074 656d            if tem
+00000680: 702e 656e 6473 7769 7468 2822 2e73 6f66  p.endswith(".sof
+00000690: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
+000006a0: 2020 2020 2072 6574 7572 6e20 6f73 2e70       return os.p
+000006b0: 6174 682e 6a6f 696e 2875 6e7a 6970 5f66  ath.join(unzip_f
+000006c0: 6f6c 6465 725f 7061 7468 2c20 7465 6d70  older_path, temp
+000006d0: 290d 0a0d 0a20 2020 2064 6566 2066 7470  )....    def ftp
+000006e0: 5f64 6f77 6e6c 6f61 645f 6669 6c65 2873  _download_file(s
+000006f0: 656c 662c 2066 7470 2c20 6670 6761 5f66  elf, ftp, fpga_f
+00000700: 6f6c 6465 722c 2066 7067 615f 6669 6c65  older, fpga_file
+00000710: 293a 0d0a 2020 2020 2020 2020 6c6f 6361  ):..        loca
+00000720: 6c5f 7061 7468 203d 206f 732e 7061 7468  l_path = os.path
+00000730: 2e6a 6f69 6e28 7365 6c66 2e6c 6f63 616c  .join(self.local
+00000740: 5f66 7470 5f66 7067 615f 7061 7468 2c20  _ftp_fpga_path, 
+00000750: 6670 6761 5f66 6f6c 6465 7229 0d0a 2020  fpga_folder)..  
+00000760: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
+00000770: 2e65 7869 7374 7328 6c6f 6361 6c5f 7061  .exists(local_pa
+00000780: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
+00000790: 2020 7368 7574 696c 2e72 6d74 7265 6528    shutil.rmtree(
+000007a0: 6c6f 6361 6c5f 7061 7468 290d 0a20 2020  local_path)..   
+000007b0: 2020 2020 206f 732e 6d6b 6469 7228 6c6f       os.mkdir(lo
+000007c0: 6361 6c5f 7061 7468 290d 0a20 2020 2020  cal_path)..     
+000007d0: 2020 206c 6f63 616c 5f66 7067 615f 6669     local_fpga_fi
+000007e0: 6c65 203d 206f 732e 7061 7468 2e6a 6f69  le = os.path.joi
+000007f0: 6e28 6c6f 6361 6c5f 7061 7468 2c20 6670  n(local_path, fp
+00000800: 6761 5f66 696c 6529 0d0a 2020 2020 2020  ga_file)..      
+00000810: 2020 7769 7468 206f 7065 6e28 6c6f 6361    with open(loca
+00000820: 6c5f 6670 6761 5f66 696c 652c 2027 7762  l_fpga_file, 'wb
+00000830: 2729 2061 7320 663a 0d0a 2020 2020 2020  ') as f:..      
+00000840: 2020 2020 2020 6674 702e 7265 7472 6269        ftp.retrbi
+00000850: 6e61 7279 2866 2752 4554 5220 7b66 7067  nary(f'RETR {fpg
+00000860: 615f 6669 6c65 7d27 2c20 662e 7772 6974  a_file}', f.writ
+00000870: 6529 0d0a 2020 2020 2020 2020 7265 7475  e)..        retu
+00000880: 726e 206c 6f63 616c 5f66 7067 615f 6669  rn local_fpga_fi
+00000890: 6c65 0d0a 0d0a 2020 2020 6465 6620 5f67  le....    def _g
+000008a0: 6574 5f66 696c 655f 6e61 6d65 2873 656c  et_file_name(sel
+000008b0: 662c 2066 7470 293a 0d0a 2020 2020 2020  f, ftp):..      
+000008c0: 2020 6670 6761 5f66 696c 6520 3d20 4e6f    fpga_file = No
+000008d0: 6e65 0d0a 2020 2020 2020 2020 6669 6c65  ne..        file
+000008e0: 6e61 6d65 7320 3d20 6674 702e 6e6c 7374  names = ftp.nlst
+000008f0: 2829 0d0a 2020 2020 2020 2020 666f 7220  ()..        for 
+00000900: 6669 6c65 5f20 696e 2066 696c 656e 616d  file_ in filenam
+00000910: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
+00000920: 2069 6620 7365 6c66 2e66 7470 5f70 6174   if self.ftp_pat
+00000930: 7465 6e20 696e 2066 696c 655f 3a0d 0a20  ten in file_:.. 
+00000940: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00000950: 7067 615f 6669 6c65 203d 2066 696c 655f  pga_file = file_
+00000960: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000970: 2020 6272 6561 6b0d 0a20 2020 2020 2020    break..       
+00000980: 2072 6574 7572 6e20 6670 6761 5f66 696c   return fpga_fil
+00000990: 650d 0a0d 0a20 2020 2064 6566 2073 706c  e....    def spl
+000009a0: 6974 5f70 6174 685f 666f 6c64 6572 5f66  it_path_folder_f
+000009b0: 696c 6528 7365 6c66 2c20 6674 702c 2066  ile(self, ftp, f
+000009c0: 7470 5f70 6174 6829 3a0d 0a20 2020 2020  tp_path):..     
+000009d0: 2020 2066 7470 5f70 6174 6820 3d20 6674     ftp_path = ft
+000009e0: 705f 7061 7468 2e72 6570 6c61 6365 2866  p_path.replace(f
+000009f0: 2266 7470 3a2f 2f7b 7365 6c66 2e69 635f  "ftp://{self.ic_
+00000a00: 6674 707d 2f22 2c20 2222 290d 0a20 2020  ftp}/", "")..   
+00000a10: 2020 2020 2073 706c 6974 5f70 6174 6873       split_paths
+00000a20: 203d 2066 7470 5f70 6174 682e 7370 6c69   = ftp_path.spli
+00000a30: 7428 222f 2229 0d0a 2020 2020 2020 2020  t("/")..        
+00000a40: 6966 206e 6f74 2073 656c 662e 6973 5f64  if not self.is_d
+00000a50: 6972 6563 746f 7279 2866 7470 2c20 6674  irectory(ftp, ft
+00000a60: 705f 7061 7468 293a 0d0a 2020 2020 2020  p_path):..      
+00000a70: 2020 2020 2020 6670 6761 5f66 696c 6520        fpga_file 
+00000a80: 3d20 7370 6c69 745f 7061 7468 735b 2d31  = split_paths[-1
+00000a90: 5d0d 0a20 2020 2020 2020 2020 2020 2066  ]..            f
+00000aa0: 7067 615f 666f 6c64 6572 203d 2073 706c  pga_folder = spl
+00000ab0: 6974 5f70 6174 6873 5b2d 325d 0d0a 2020  it_paths[-2]..  
+00000ac0: 2020 2020 2020 2020 2020 6674 702e 6377            ftp.cw
+00000ad0: 6428 6f73 2e70 6174 682e 6469 726e 616d  d(os.path.dirnam
+00000ae0: 6528 6674 705f 7061 7468 2929 0d0a 2020  e(ftp_path))..  
+00000af0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00000b00: 2020 2020 2020 2020 2066 7067 615f 666f           fpga_fo
+00000b10: 6c64 6572 203d 2073 706c 6974 5f70 6174  lder = split_pat
+00000b20: 6873 5b2d 315d 2069 6620 7370 6c69 745f  hs[-1] if split_
+00000b30: 7061 7468 735b 2d31 5d20 213d 2022 2220  paths[-1] != "" 
+00000b40: 656c 7365 2073 706c 6974 5f70 6174 6873  else split_paths
+00000b50: 5b2d 325d 0d0a 2020 2020 2020 2020 2020  [-2]..          
+00000b60: 2020 6670 6761 5f66 696c 6520 3d20 7365    fpga_file = se
+00000b70: 6c66 2e5f 6765 745f 6669 6c65 5f6e 616d  lf._get_file_nam
+00000b80: 6528 6674 7029 0d0a 2020 2020 2020 2020  e(ftp)..        
+00000b90: 7265 7475 726e 2066 7067 615f 666f 6c64  return fpga_fold
+00000ba0: 6572 2c20 6670 6761 5f66 696c 650d 0a0d  er, fpga_file...
+00000bb0: 0a20 2020 2064 6566 2067 6574 5f66 7067  .    def get_fpg
+00000bc0: 615f 6672 6f6d 5f66 7470 2873 656c 662c  a_from_ftp(self,
+00000bd0: 2066 7470 5f70 6174 6829 3a0d 0a20 2020   ftp_path):..   
+00000be0: 2020 2020 206c 6f67 2e49 4e46 4f28 6622       log.INFO(f"
+00000bf0: 4265 6769 6e20 746f 2067 6574 2073 6f66  Begin to get sof
+00000c00: 2066 726f 6d20 7b66 7470 5f70 6174 687d   from {ftp_path}
+00000c10: 2229 0d0a 2020 2020 2020 2020 6674 7020  ")..        ftp 
+00000c20: 3d20 6674 706c 6962 2e46 5450 2873 656c  = ftplib.FTP(sel
+00000c30: 662e 6963 5f66 7470 2c20 7365 6c66 2e69  f.ic_ftp, self.i
+00000c40: 635f 6674 705f 7573 6572 2c20 7365 6c66  c_ftp_user, self
+00000c50: 2e69 635f 6674 705f 7077 6429 0d0a 2020  .ic_ftp_pwd)..  
+00000c60: 2020 2020 2020 6670 6761 5f66 6f6c 6465        fpga_folde
+00000c70: 722c 2066 7067 615f 6669 6c65 203d 2073  r, fpga_file = s
+00000c80: 656c 662e 7370 6c69 745f 7061 7468 5f66  elf.split_path_f
+00000c90: 6f6c 6465 725f 6669 6c65 2866 7470 2c20  older_file(ftp, 
+00000ca0: 6674 705f 7061 7468 290d 0a20 2020 2020  ftp_path)..     
+00000cb0: 2020 2064 6c5f 6670 6761 5f70 6174 6820     dl_fpga_path 
+00000cc0: 3d20 7365 6c66 2e66 7470 5f64 6f77 6e6c  = self.ftp_downl
+00000cd0: 6f61 645f 6669 6c65 2866 7470 2c20 6670  oad_file(ftp, fp
+00000ce0: 6761 5f66 6f6c 6465 722c 2066 7067 615f  ga_folder, fpga_
+00000cf0: 6669 6c65 290d 0a20 2020 2020 2020 2073  file)..        s
+00000d00: 6f66 5f66 696c 6520 3d20 7365 6c66 2e75  of_file = self.u
+00000d10: 6e7a 6970 5f66 7067 615f 6669 6c65 2864  nzip_fpga_file(d
+00000d20: 6c5f 6670 6761 5f70 6174 6829 0d0a 2020  l_fpga_path)..  
+00000d30: 2020 2020 2020 6c6f 672e 494e 464f 2866        log.INFO(f
+00000d40: 2247 6574 2073 6f66 207b 736f 665f 6669  "Get sof {sof_fi
+00000d50: 6c65 7d20 6672 6f6d 2066 7470 2229 0d0a  le} from ftp")..
+00000d60: 2020 2020 2020 2020 6674 702e 7175 6974          ftp.quit
+00000d70: 2829 0d0a 2020 2020 2020 2020 6966 2073  ()..        if s
+00000d80: 6f66 5f66 696c 6520 6973 204e 6f6e 653a  of_file is None:
+00000d90: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+00000da0: 6973 6520 5275 6e74 696d 6545 7272 6f72  ise RuntimeError
+00000db0: 2866 2273 6f66 5f66 696c 6520 6765 7420  (f"sof_file get 
+00000dc0: 6661 696c 6564 3a20 7b66 7470 5f70 6174  failed: {ftp_pat
+00000dd0: 687d 2229 0d0a 2020 2020 2020 2020 7265  h}")..        re
+00000de0: 7475 726e 2073 6f66 5f66 696c 650d 0a0d  turn sof_file...
+00000df0: 0a20 2020 2064 6566 2067 6574 5f67 6974  .    def get_git
+00000e00: 5f70 726f 6a65 6374 5f70 6174 6828 7365  _project_path(se
+00000e10: 6c66 293a 0d0a 2020 2020 2020 2020 6261  lf):..        ba
+00000e20: 7365 6e61 6d65 203d 206f 732e 7061 7468  sename = os.path
+00000e30: 2e62 6173 656e 616d 6528 7365 6c66 2e67  .basename(self.g
+00000e40: 6974 5f75 726c 290d 0a20 2020 2020 2020  it_url)..       
+00000e50: 2066 6f6c 6465 725f 6e61 6d65 203d 206f   folder_name = o
+00000e60: 732e 7061 7468 2e73 706c 6974 6578 7428  s.path.splitext(
+00000e70: 6261 7365 6e61 6d65 295b 305d 0d0a 2020  basename)[0]..  
+00000e80: 2020 2020 2020 7265 7475 726e 206f 732e        return os.
+00000e90: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e6c  path.join(self.l
+00000ea0: 6f63 616c 5f66 775f 7061 7468 2c20 666f  ocal_fw_path, fo
+00000eb0: 6c64 6572 5f6e 616d 6529 0d0a 0d0a 2020  lder_name)....  
+00000ec0: 2020 6465 6620 7570 6461 7465 5f66 775f    def update_fw_
+00000ed0: 636f 6465 2873 656c 662c 2062 7261 6e63  code(self, branc
+00000ee0: 6829 3a0d 0a20 2020 2020 2020 206c 6f63  h):..        loc
+00000ef0: 616c 5f66 775f 7061 7468 203d 2073 656c  al_fw_path = sel
+00000f00: 662e 6c6f 6361 6c5f 6677 5f70 6a5f 7061  f.local_fw_pj_pa
+00000f10: 7468 2069 6620 6f73 2e70 6174 682e 6578  th if os.path.ex
+00000f20: 6973 7473 2873 656c 662e 6c6f 6361 6c5f  ists(self.local_
+00000f30: 6677 5f70 6a5f 7061 7468 2920 656c 7365  fw_pj_path) else
+00000f40: 2073 656c 662e 6c6f 6361 6c5f 6677 5f70   self.local_fw_p
+00000f50: 6174 680d 0a20 2020 2020 2020 2067 6974  ath..        git
+00000f60: 203d 2047 6974 4f70 6572 6174 6f72 2822   = GitOperator("
+00000f70: 7368 616f 6269 6e2e 7368 7522 2c20 2243  shaobin.shu", "C
+00000f80: 6e65 7821 3230 3234 222c 206c 6f63 616c  nex!2024", local
+00000f90: 5f66 775f 7061 7468 290d 0a20 2020 2020  _fw_path)..     
+00000fa0: 2020 2069 6620 6f73 2e70 6174 682e 6578     if os.path.ex
+00000fb0: 6973 7473 2873 656c 662e 6c6f 6361 6c5f  ists(self.local_
+00000fc0: 6677 5f70 6a5f 7061 7468 293a 0d0a 2020  fw_pj_path):..  
+00000fd0: 2020 2020 2020 2020 2020 6e65 775f 6d73            new_ms
+00000fe0: 672c 2072 6574 203d 2067 6974 2e75 7064  g, ret = git.upd
+00000ff0: 6174 655f 6c61 7465 7374 5f63 6f64 6528  ate_latest_code(
+00001000: 6622 6f72 6967 696e 2f7b 6272 616e 6368  f"origin/{branch
+00001010: 7d22 290d 0a20 2020 2020 2020 2020 2020  }")..           
+00001020: 2069 6620 7265 7420 213d 2030 3a0d 0a20   if ret != 0:.. 
+00001030: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00001040: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
+00001050: 7228 6622 4769 7420 7570 6461 7465 2066  r(f"Git update f
+00001060: 6169 6c65 642c 2075 726c 3a7b 7365 6c66  ailed, url:{self
+00001070: 2e67 6974 5f75 726c 7d20 6272 616e 6368  .git_url} branch
+00001080: 3a7b 6272 616e 6368 7d22 290d 0a20 2020  :{branch}")..   
+00001090: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+000010a0: 2020 2020 2020 2020 6966 2067 6974 2e63          if git.c
+000010b0: 6c6f 6e65 2873 656c 662e 6769 745f 7572  lone(self.git_ur
+000010c0: 6c2c 2066 226f 7269 6769 6e2f 7b62 7261  l, f"origin/{bra
+000010d0: 6e63 687d 2229 2021 3d20 303a 0d0a 2020  nch}") != 0:..  
+000010e0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+000010f0: 6973 6520 5275 6e74 696d 6545 7272 6f72  ise RuntimeError
+00001100: 2866 2247 6974 2063 6c6f 6e65 2066 6169  (f"Git clone fai
+00001110: 6c65 642c 2075 726c 3a7b 7365 6c66 2e67  led, url:{self.g
+00001120: 6974 5f75 726c 7d20 6272 616e 6368 3a7b  it_url} branch:{
+00001130: 6272 616e 6368 7d22 290d 0a0d 0a20 2020  branch}")....   
+00001140: 2064 6566 2063 6f70 795f 736f 665f 325f   def copy_sof_2_
+00001150: 6677 2873 656c 662c 2073 7263 5f73 6f66  fw(self, src_sof
+00001160: 293a 0d0a 2020 2020 2020 2020 6473 745f  ):..        dst_
+00001170: 736f 6620 3d20 6f73 2e70 6174 682e 6a6f  sof = os.path.jo
+00001180: 696e 2873 656c 662e 6c6f 6361 6c5f 6677  in(self.local_fw
+00001190: 5f70 6a5f 7061 7468 2c20 2274 6168 6f65  _pj_path, "tahoe
+000011a0: 2e73 6f66 2229 0d0a 2020 2020 2020 2020  .sof")..        
+000011b0: 6966 206f 732e 7061 7468 2e65 7869 7374  if os.path.exist
+000011c0: 7328 6473 745f 736f 6629 3a0d 0a20 2020  s(dst_sof):..   
+000011d0: 2020 2020 2020 2020 206f 732e 7265 6d6f           os.remo
+000011e0: 7665 2864 7374 5f73 6f66 290d 0a20 2020  ve(dst_sof)..   
+000011f0: 2020 2020 2073 6875 7469 6c2e 636f 7079       shutil.copy
+00001200: 2873 7263 5f73 6f66 2c20 6473 745f 736f  (src_sof, dst_so
+00001210: 6629 0d0a 0d0a 2020 2020 6465 6620 6c6f  f)....    def lo
+00001220: 6164 5f61 6c6c 2873 656c 6629 3a0d 0a20  ad_all(self):.. 
+00001230: 2020 2020 2020 2063 6d64 203d 2066 2263         cmd = f"c
+00001240: 6420 2f64 207b 7365 6c66 2e6c 6f63 616c  d /d {self.local
+00001250: 5f66 775f 706a 5f70 6174 687d 2026 2620  _fw_pj_path} && 
+00001260: 6c6f 6164 5f61 6c6c 2e62 6174 220d 0a20  load_all.bat".. 
+00001270: 2020 2020 2020 206c 6f67 2e49 4e46 4f28         log.INFO(
+00001280: 6622 7570 6772 6164 6520 6c6f 6769 6320  f"upgrade logic 
+00001290: 616e 6420 6669 726d 7761 7265 2077 6974  and firmware wit
+000012a0: 6820 636d 643a 207b 636d 647d 2229 0d0a  h cmd: {cmd}")..
+000012b0: 2020 2020 2020 2020 7265 7420 3d20 6f73          ret = os
+000012c0: 2e73 7973 7465 6d28 636d 6429 0d0a 2020  .system(cmd)..  
+000012d0: 2020 2020 2020 6966 2072 6574 2021 3d20        if ret != 
+000012e0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+000012f0: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
+00001300: 6f72 2822 6c6f 6164 5f61 6c6c 2066 6169  or("load_all fai
+00001310: 6c65 6422 290d 0a20 2020 2020 2020 2074  led")..        t
+00001320: 696d 652e 736c 6565 7028 3630 290d 0a0d  ime.sleep(60)...
+00001330: 0a20 2020 2064 6566 2069 6e73 6d6f 645f  .    def insmod_
+00001340: 6b6f 2873 656c 662c 2073 7368 2c20 7665  ko(self, ssh, ve
+00001350: 6e75 7329 3a0d 0a20 2020 2020 2020 206b  nus):..        k
+00001360: 6f5f 7061 7468 203d 2066 227b 7665 6e75  o_path = f"{venu
+00001370: 737d 2f62 696e 2f74 6168 6f65 2f71 615f  s}/bin/tahoe/qa_
+00001380: 6d6f 6465 220d 0a20 2020 2020 2020 2063  mode"..        c
+00001390: 6d64 203d 2066 2263 6420 7b6b 6f5f 7061  md = f"cd {ko_pa
+000013a0: 7468 7d20 2626 2069 6e73 6d6f 6420 6e65  th} && insmod ne
+000013b0: 7875 732e 6b6f 2026 2620 696e 736d 6f64  xus.ko && insmod
+000013c0: 206b 7465 7374 2e6b 6f22 0d0a 2020 2020   ktest.ko"..    
+000013d0: 2020 2020 7374 6174 7573 2c20 6f75 7470      status, outp
+000013e0: 7574 203d 2073 7368 2e63 6f6d 6d61 6e64  ut = ssh.command
+000013f0: 2863 6d64 290d 0a20 2020 2020 2020 2069  (cmd)..        i
+00001400: 6620 7374 6174 7573 2021 3d20 303a 0d0a  f status != 0:..
+00001410: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00001420: 6520 5275 6e74 696d 6545 7272 6f72 2866  e RuntimeError(f
+00001430: 2269 6e73 6d6f 6420 6661 696c 6564 2c20  "insmod failed, 
+00001440: 636d 643a 207b 636d 647d 2e20 4f75 7470  cmd: {cmd}. Outp
+00001450: 7574 3a7b 6f75 7470 7574 7d22 290d 0a0d  ut:{output}")...
+00001460: 0a20 2020 2064 6566 2072 6562 6f6f 745f  .    def reboot_
+00001470: 6c69 6e75 7828 7365 6c66 2c20 6c69 6e75  linux(self, linu
+00001480: 782c 2075 7365 722c 2070 7764 2c20 7665  x, user, pwd, ve
+00001490: 6e75 735f 7061 7468 293a 0d0a 2020 2020  nus_path):..    
+000014a0: 2020 2020 7373 6820 3d20 5353 4828 6c69      ssh = SSH(li
+000014b0: 6e75 782c 2075 7365 726e 616d 653d 7573  nux, username=us
+000014c0: 6572 2c20 7061 7373 776f 7264 3d70 7764  er, password=pwd
+000014d0: 290d 0a20 2020 2020 2020 2073 7368 2e6f  )..        ssh.o
+000014e0: 7065 6e28 290d 0a20 2020 2020 2020 2073  pen()..        s
+000014f0: 7368 2e63 6f6d 6d61 6e64 5f77 6974 686f  sh.command_witho
+00001500: 7574 5f72 6573 756c 7428 2272 6562 6f6f  ut_result("reboo
+00001510: 7420 2d6e 6622 2c20 7469 6d65 6f75 743d  t -nf", timeout=
+00001520: 3130 290d 0a20 2020 2020 2020 2074 696d  10)..        tim
+00001530: 652e 736c 6565 7028 3630 290d 0a20 2020  e.sleep(60)..   
+00001540: 2020 2020 2073 7368 2e6f 7065 6e28 290d       ssh.open().
+00001550: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+00001560: 736d 6f64 5f6b 6f28 7373 682c 2076 656e  smod_ko(ssh, ven
+00001570: 7573 5f70 6174 6829 0d0a 0d0a 2020 2020  us_path)....    
+00001580: 4073 7461 7469 636d 6574 686f 640d 0a20  @staticmethod.. 
+00001590: 2020 2064 6566 2063 6c65 6172 5f75 6172     def clear_uar
+000015a0: 7428 636f 6d29 3a0d 0a20 2020 2020 2020  t(com):..       
+000015b0: 2073 6572 203d 2043 6e65 7853 6572 6961   ser = CnexSeria
+000015c0: 6c28 636f 6d29 0d0a 2020 2020 2020 2020  l(com)..        
+000015d0: 7365 722e 636c 6f73 655f 7474 6572 6d70  ser.close_ttermp
+000015e0: 726f 2829 0d0a 2020 2020 2020 2020 7469  ro()..        ti
+000015f0: 6d65 2e73 6c65 6570 2832 290d 0a20 2020  me.sleep(2)..   
+00001600: 2020 2020 2073 6572 2e63 6c65 6172 7370       ser.clearsp
+00001610: 6931 2829 0d0a 2020 2020 2020 2020 7469  i1()..        ti
+00001620: 6d65 2e73 6c65 6570 2832 290d 0a20 2020  me.sleep(2)..   
+00001630: 2020 2020 2073 6572 2e6f 7065 6e5f 7474       ser.open_tt
+00001640: 6572 6d70 726f 2829 0d0a 0d0a 2020 2020  ermpro()....    
+00001650: 4064 6563 6f72 6174 655f 6578 6365 7074  @decorate_except
+00001660: 696f 6e5f 7265 7375 6c74 0d0a 2020 2020  ion_result..    
+00001670: 6465 6620 7275 6e28 7365 6c66 2c20 7061  def run(self, pa
+00001680: 7261 293a 0d0a 2020 2020 2020 2020 6c6f  ra):..        lo
+00001690: 672e 494e 464f 2822 4265 6769 6e20 746f  g.INFO("Begin to
+000016a0: 2064 6f77 6e6c 6f61 6420 6c6f 6769 6320   download logic 
+000016b0: 616e 6420 6669 726d 7761 7265 2229 0d0a  and firmware")..
+000016c0: 2020 2020 2020 2020 7372 635f 736f 6620          src_sof 
+000016d0: 3d20 7365 6c66 2e67 6574 5f66 7067 615f  = self.get_fpga_
+000016e0: 6672 6f6d 5f66 7470 2870 6172 615b 2269  from_ftp(para["i
+000016f0: 635f 6c6f 6769 6322 5d29 0d0a 2020 2020  c_logic"])..    
+00001700: 2020 2020 7365 6c66 2e75 7064 6174 655f      self.update_
+00001710: 6677 5f63 6f64 6528 7061 7261 5b22 6963  fw_code(para["ic
+00001720: 5f66 775f 6272 616e 6368 225d 290d 0a20  _fw_branch"]).. 
+00001730: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
+00001740: 725f 7561 7274 2870 6172 615b 2263 6f6d  r_uart(para["com
+00001750: 225d 290d 0a20 2020 2020 2020 2073 656c  "])..        sel
+00001760: 662e 636f 7079 5f73 6f66 5f32 5f66 7728  f.copy_sof_2_fw(
+00001770: 7372 635f 736f 6629 0d0a 2020 2020 2020  src_sof)..      
+00001780: 2020 7365 6c66 2e6c 6f61 645f 616c 6c28    self.load_all(
+00001790: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000017a0: 7265 626f 6f74 5f6c 696e 7578 2870 6172  reboot_linux(par
+000017b0: 615b 2274 6172 6765 745f 6970 225d 2c20  a["target_ip"], 
+000017c0: 7061 7261 5b22 6c69 6e75 785f 7573 6572  para["linux_user
+000017d0: 225d 2c20 7061 7261 5b22 6c69 6e75 785f  "], para["linux_
+000017e0: 7077 6422 5d2c 2070 6172 615b 2277 6f72  pwd"], para["wor
+000017f0: 6b5f 7061 7468 225d 290d 0a20 2020 2020  k_path"])..     
+00001800: 2020 2072 6574 7572 6e20 302c 2022 646f     return 0, "do
+00001810: 776e 6c6f 6164 206c 6f67 6963 2061 6e64  wnload logic and
+00001820: 2066 6972 6d77 6172 6520 7375 6363 6565   firmware succee
+00001830: 6422 0d0a                                d"..
```

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/node_database.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/node_database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/performance_database.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/performance_database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/state.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/state.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/status_file.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/status_file.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_base.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_base.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_benchmark.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_benchmark_group.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_benchmark_group.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_case.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_case.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_pool.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_pool.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_reboot_handle.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_reboot_handle.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_result.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_result.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_runner.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_runner.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_suite.py` & `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_suite.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/dll/buf.dll` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/dll/buf.dll`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/dll/buf.so` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/dll/buf.so`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/dll/build.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/dll/build.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/linux_nvme.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/linux_nvme.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/buf.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/buf.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/ctype.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/ctype.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/get_feature.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/get_feature.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/ioctl.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/ioctl.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/nvme.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/nvme.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/command.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/command.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/features.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/features.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/hmb.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/hmb.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/identify.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/identify.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/log_page.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/log_page.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/memory.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/memory.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/pcie.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/pcie.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/registers.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/registers.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/utility_vu.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/utility_vu.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/diskpart/diskpart.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/diskpart/diskpart.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/fio/fio.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/fio/fio.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/fio/fio_linux.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/fio/fio_linux.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/fio/tool/fio` & `automation_rest_server-3.6.9/automation_rest_server/tool/fio/tool/fio`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/git/git_operator.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/git/git_operator.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/tool/iometer/iometer.py` & `automation_rest_server-3.6.9/automation_rest_server/tool/iometer/iometer.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/utils/buf.py` & `automation_rest_server-3.6.9/automation_rest_server/utils/buf.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/utils/firmware_path.py` & `automation_rest_server-3.6.9/automation_rest_server/utils/firmware_path.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/utils/log.py` & `automation_rest_server-3.6.9/automation_rest_server/utils/log.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/utils/nose_xml.py` & `automation_rest_server-3.6.9/automation_rest_server/utils/nose_xml.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/utils/pip_operation.py` & `automation_rest_server-3.6.9/automation_rest_server/utils/pip_operation.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/utils/process.py` & `automation_rest_server-3.6.9/automation_rest_server/utils/process.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/utils/ssh.py` & `automation_rest_server-3.6.9/automation_rest_server/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server/utils/system.py` & `automation_rest_server-3.6.9/automation_rest_server/utils/system.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.8/automation_rest_server.egg-info/PKG-INFO` & `automation_rest_server-3.6.9/automation_rest_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: automation-rest-server
-Version: 3.6.8
+Version: 3.6.9
 Summary: NVMe production server
 Home-page: https://pypi.org/project/automation_rest_server
 Author: yuwen123441
 Author-email: yuwen123441@126.com
 License: MIT License
 Description: UNKNOWN
 Keywords: runner,server
```

### Comparing `automation_rest_server-3.6.8/automation_rest_server.egg-info/SOURCES.txt` & `automation_rest_server-3.6.9/automation_rest_server.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -123,9 +123,10 @@
 automation_rest_server/utils/buf.py
 automation_rest_server/utils/firmware_path.py
 automation_rest_server/utils/log.py
 automation_rest_server/utils/message.py
 automation_rest_server/utils/nose_xml.py
 automation_rest_server/utils/pip_operation.py
 automation_rest_server/utils/process.py
+automation_rest_server/utils/serial_tool.py
 automation_rest_server/utils/ssh.py
 automation_rest_server/utils/system.py
```

### Comparing `automation_rest_server-3.6.8/setup.py` & `automation_rest_server-3.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 packages = ["automation_rest_server"]
 #python setup.py sdist upload  
 #python setup.py bdist_wheel
 
 setup(
     name = 'automation_rest_server',
-    version = '3.6.8',
+    version = '3.6.9',
     keywords = ['runner', 'server'],
     description = 'NVMe production server',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'License :: OSI Approved :: MIT License',
```

