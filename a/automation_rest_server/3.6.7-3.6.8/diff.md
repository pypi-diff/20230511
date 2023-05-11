# Comparing `tmp/automation_rest_server-3.6.7.tar.gz` & `tmp/automation_rest_server-3.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\automation_rest_server-3.6.7.tar", last modified: Wed Apr 19 05:42:05 2023, max compression
+gzip compressed data, was "dist\automation_rest_server-3.6.8.tar", last modified: Wed May 10 08:47:26 2023, max compression
```

## Comparing `automation_rest_server-3.6.7.tar` & `automation_rest_server-3.6.8.tar`

### file list

```diff
@@ -1,157 +1,159 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:05.000000 automation_rest_server-3.6.7/
--rw-rw-rw-   0        0        0     1098 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/LICENSE.txt
--rw-rw-rw-   0        0        0      687 2022-08-30 06:56:12.000000 automation_rest_server-3.6.7/MANIFEST.in
--rw-rw-rw-   0        0        0      551 2023-04-19 05:42:05.000000 automation_rest_server-3.6.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:03.000000 automation_rest_server-3.6.7/automation_rest_server/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:04.000000 automation_rest_server-3.6.7/automation_rest_server/configuration/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/configuration/__init__.py
--rw-rw-rw-   0        0        0      581 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/configuration/config.yaml
--rw-rw-rw-   0        0        0     1099 2022-12-13 11:04:16.000000 automation_rest_server-3.6.7/automation_rest_server/configuration/firmware_build.yaml
--rw-rw-rw-   0        0        0  1333232 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/configuration/pci.ids
--rw-rw-rw-   0        0        0      157 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/configuration/version.yaml
--rw-rw-rw-   0        0        0       83 2022-08-25 03:13:17.000000 automation_rest_server-3.6.7/automation_rest_server/configuration/web_server.yaml
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:04.000000 automation_rest_server-3.6.7/automation_rest_server/rest_client/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:18:57.000000 automation_rest_server-3.6.7/automation_rest_server/rest_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:04.000000 automation_rest_server-3.6.7/automation_rest_server/rest_client/resource/
--rw-rw-rw-   0        0        0        0 2022-08-10 09:04:38.000000 automation_rest_server-3.6.7/automation_rest_server/rest_client/resource/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:04.000000 automation_rest_server-3.6.7/automation_rest_server/rest_client/resource/models/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:20:01.000000 automation_rest_server-3.6.7/automation_rest_server/rest_client/resource/models/__init__.py
--rw-rw-rw-   0        0        0     4264 2022-08-12 01:44:10.000000 automation_rest_server-3.6.7/automation_rest_server/rest_client/resource/models/helper.py
--rw-rw-rw-   0        0        0     1944 2022-08-17 05:58:24.000000 automation_rest_server-3.6.7/automation_rest_server/rest_client/resource/node_resource.py
--rw-rw-rw-   0        0        0     1374 2022-08-30 04:43:20.000000 automation_rest_server-3.6.7/automation_rest_server/rest_client/resource/test_resource.py
--rw-rw-rw-   0        0        0      340 2022-08-25 03:00:40.000000 automation_rest_server-3.6.7/automation_rest_server/rest_client/resource/web_resource.py
--rw-rw-rw-   0        0        0     2536 2023-02-21 08:02:23.000000 automation_rest_server-3.6.7/automation_rest_server/rest_client/web_rest_client.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:04.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/__init__.py
--rw-rw-rw-   0        0        0     1678 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/reset_server.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:04.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/__init__.py
--rw-rw-rw-   0        0        0     2150 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/benchmark_resource.py
--rw-rw-rw-   0        0        0     1956 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/build_firmware_resource.py
--rw-rw-rw-   0        0        0      933 2022-12-12 01:57:01.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/git_resource.py
--rw-rw-rw-   0        0        0      850 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:04.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/models/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/models/__init__.py
--rw-rw-rw-   0        0        0     2044 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/models/ftp_server.py
--rw-rw-rw-   0        0        0     1732 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/models/helper.py
--rw-rw-rw-   0        0        0      958 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/oakgate_resource.py
--rw-rw-rw-   0        0        0      691 2022-08-11 02:31:16.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/operation_resource.py
--rw-rw-rw-   0        0        0     1641 2022-09-20 01:54:25.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/state_resource.py
--rw-rw-rw-   0        0        0     1085 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/stop_flag_resource.py
--rw-rw-rw-   0        0        0     6233 2022-12-03 07:36:31.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/test_resource.py
--rw-rw-rw-   0        0        0     1244 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/upgrade_resource.py
--rw-rw-rw-   0        0        0     5980 2023-03-06 02:10:37.000000 automation_rest_server-3.6.7/automation_rest_server/run.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:04.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/__init__.py
--rw-rw-rw-   0        0        0     6679 2022-09-20 04:46:34.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/database.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:04.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/dut/
--rw-rw-rw-   0        0        0        0 2021-11-12 08:10:50.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/dut/__init__.py
--rw-rw-rw-   0        0        0     3082 2023-04-19 05:40:44.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/dut/slot.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:04.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/dut/sub_slot/
--rw-rw-rw-   0        0        0        0 2021-11-24 03:48:51.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/dut/sub_slot/__init__.py
--rw-rw-rw-   0        0        0     1434 2022-09-15 07:43:45.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py
--rw-rw-rw-   0        0        0     3541 2023-04-17 06:49:22.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py
--rw-rw-rw-   0        0        0      901 2023-04-19 03:39:13.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py
--rw-rw-rw-   0        0        0     8892 2022-09-27 01:01:15.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:04.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/engine/
--rw-rw-rw-   0        0        0      214 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/engine/__init__.py
--rw-rw-rw-   0        0        0     2067 2022-12-13 09:26:23.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/engine/nose_engine.py
--rw-rw-rw-   0        0        0     4926 2023-02-16 01:39:59.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/engine/oakgate_engine.py
--rw-rw-rw-   0        0        0     4007 2023-03-02 06:19:25.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/engine/perses_engine.py
--rw-rw-rw-   0        0        0     1489 2022-09-30 01:53:36.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py
--rw-rw-rw-   0        0        0      239 2023-04-07 02:04:12.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/engine/special_parameter.py
--rw-rw-rw-   0        0        0     3562 2022-09-20 07:48:14.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/engine/sse_engine.py
--rw-rw-rw-   0        0        0     1517 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_build.py
--rw-rw-rw-   0        0        0     2724 2022-12-14 00:39:53.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_download.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:05.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/__init__.py
--rw-rw-rw-   0        0        0     7168 2022-12-13 11:05:02.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:05.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/oakgate/
--rw-rw-rw-   0        0        0        0 2023-04-11 02:31:20.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/oakgate/__init__.py
--rw-rw-rw-   0        0        0     2925 2023-04-11 02:43:50.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py
--rw-rw-rw-   0        0        0     2691 2023-04-17 07:35:59.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py
--rw-rw-rw-   0        0        0      669 2023-04-11 02:57:44.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py
--rw-rw-rw-   0        0        0     1992 2023-04-10 08:33:59.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py
--rw-rw-rw-   0        0        0     1581 2022-09-27 01:01:15.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py
--rw-rw-rw-   0        0        0     2344 2023-04-09 02:31:46.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py
--rw-rw-rw-   0        0        0     5467 2022-08-12 02:31:49.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/node_database.py
--rw-rw-rw-   0        0        0    10717 2023-04-19 03:38:41.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/performance_database.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:05.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/reboot_engine/
--rw-rw-rw-   0        0        0       50 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/reboot_engine/__init__.py
--rw-rw-rw-   0        0        0     2439 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py
--rw-rw-rw-   0        0        0     2052 2023-04-04 09:26:41.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/state.py
--rw-rw-rw-   0        0        0      672 2022-12-13 03:29:14.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/status_file.py
--rw-rw-rw-   0        0        0     5684 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/test_base.py
--rw-rw-rw-   0        0        0     1973 2023-02-14 08:06:21.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/test_benchmark.py
--rw-rw-rw-   0        0        0     3512 2023-02-07 07:54:27.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/test_benchmark_group.py
--rw-rw-rw-   0        0        0     1263 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/test_case.py
--rw-rw-rw-   0        0        0    21722 2023-04-04 09:26:41.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/test_pool.py
--rw-rw-rw-   0        0        0      892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/test_reboot_handle.py
--rw-rw-rw-   0        0        0     4365 2022-12-03 07:44:06.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/test_result.py
--rw-rw-rw-   0        0        0     3757 2023-03-02 10:28:02.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/test_runner.py
--rw-rw-rw-   0        0        0     4717 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/test_framework/test_suite.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:05.000000 automation_rest_server-3.6.7/automation_rest_server/tool/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/tool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:05.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/
--rw-rw-rw-   0        0        0        0 2021-11-12 06:54:04.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:05.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/dll/
--rw-rw-rw-   0        0        0        0 2021-10-23 02:17:43.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/dll/__init__.py
--rw-rw-rw-   0        0        0    24064 2021-10-23 02:17:43.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/dll/buf.dll
--rw-rw-rw-   0        0        0    12760 2021-10-23 02:17:43.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/dll/buf.so
--rw-rw-rw-   0        0        0      777 2021-10-23 02:17:43.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/dll/build.py
--rw-rw-rw-   0        0        0      861 2022-09-15 07:43:45.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/linux_nvme.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:05.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/
--rw-rw-rw-   0        0        0        0 2021-11-23 06:34:00.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/__init__.py
--rw-rw-rw-   0        0        0    14077 2021-11-23 06:29:25.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/buf.py
--rw-rw-rw-   0        0        0     4722 2021-11-23 06:25:09.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/ctype.py
--rw-rw-rw-   0        0        0    39204 2021-11-23 06:28:50.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/get_feature.py
--rw-rw-rw-   0        0        0    38547 2022-09-15 07:43:45.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/ioctl.py
--rw-rw-rw-   0        0        0    23303 2022-09-15 07:42:03.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/nvme.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:05.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/
--rw-rw-rw-   0        0        0      256 2021-11-23 06:21:15.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/__init__.py
--rw-rw-rw-   0        0        0    30449 2021-11-23 06:59:35.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/command.py
--rw-rw-rw-   0        0        0    15322 2021-11-23 06:59:35.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/features.py
--rw-rw-rw-   0        0        0     1104 2021-10-23 02:17:43.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/hmb.py
--rw-rw-rw-   0        0        0    16135 2021-11-23 07:31:19.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/identify.py
--rw-rw-rw-   0        0        0    13915 2021-11-23 06:59:59.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/log_page.py
--rw-rw-rw-   0        0        0     2361 2021-11-12 10:37:37.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/memory.py
--rw-rw-rw-   0        0        0    10510 2021-10-23 02:17:43.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/pcie.py
--rw-rw-rw-   0        0        0    35527 2021-10-23 02:17:43.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/registers.py
--rw-rw-rw-   0        0        0     9095 2021-11-24 06:24:21.000000 automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/utility_vu.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:05.000000 automation_rest_server-3.6.7/automation_rest_server/tool/diskpart/
--rw-rw-rw-   0        0        0       56 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/tool/diskpart/__init__.py
--rw-rw-rw-   0        0        0      770 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/tool/diskpart/diskpart.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:05.000000 automation_rest_server-3.6.7/automation_rest_server/tool/fio/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/tool/fio/__init__.py
--rw-rw-rw-   0        0        0    18967 2023-02-23 03:46:38.000000 automation_rest_server-3.6.7/automation_rest_server/tool/fio/fio.py
--rw-rw-rw-   0        0        0     5032 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/tool/fio/fio_linux.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:05.000000 automation_rest_server-3.6.7/automation_rest_server/tool/fio/tool/
--rw-rw-rw-   0        0        0  4733892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/tool/fio/tool/fio
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:05.000000 automation_rest_server-3.6.7/automation_rest_server/tool/git/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/tool/git/__init__.py
--rw-rw-rw-   0        0        0     5645 2023-03-02 10:20:30.000000 automation_rest_server-3.6.7/automation_rest_server/tool/git/git_operator.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:05.000000 automation_rest_server-3.6.7/automation_rest_server/tool/iometer/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/tool/iometer/__init__.py
--rw-rw-rw-   0        0        0     9223 2023-02-07 08:25:51.000000 automation_rest_server-3.6.7/automation_rest_server/tool/iometer/iometer.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:05.000000 automation_rest_server-3.6.7/automation_rest_server/utils/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/utils/__init__.py
--rw-rw-rw-   0        0        0    12385 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/utils/buf.py
--rw-rw-rw-   0        0        0     5636 2023-04-10 09:29:00.000000 automation_rest_server-3.6.7/automation_rest_server/utils/firmware_path.py
--rw-rw-rw-   0        0        0     3697 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/utils/log.py
--rw-rw-rw-   0        0        0      386 2023-02-23 02:34:33.000000 automation_rest_server-3.6.7/automation_rest_server/utils/message.py
--rw-rw-rw-   0        0        0     3532 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/utils/nose_xml.py
--rw-rw-rw-   0        0        0     1742 2022-09-20 07:22:33.000000 automation_rest_server-3.6.7/automation_rest_server/utils/pip_operation.py
--rw-rw-rw-   0        0        0     1823 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/utils/process.py
--rw-rw-rw-   0        0        0     9222 2022-06-02 02:49:38.000000 automation_rest_server-3.6.7/automation_rest_server/utils/ssh.py
--rw-rw-rw-   0        0        0     5366 2022-12-22 01:47:58.000000 automation_rest_server-3.6.7/automation_rest_server/utils/system.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:42:03.000000 automation_rest_server-3.6.7/automation_rest_server.egg-info/
--rw-rw-rw-   0        0        0      551 2023-04-19 05:42:03.000000 automation_rest_server-3.6.7/automation_rest_server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6858 2023-04-19 05:42:03.000000 automation_rest_server-3.6.7/automation_rest_server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 05:42:03.000000 automation_rest_server-3.6.7/automation_rest_server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-04-19 05:42:03.000000 automation_rest_server-3.6.7/automation_rest_server.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-04-19 05:42:03.000000 automation_rest_server-3.6.7/automation_rest_server.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-04-19 05:42:03.000000 automation_rest_server-3.6.7/automation_rest_server.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       64 2023-04-19 05:42:05.000000 automation_rest_server-3.6.7/setup.cfg
--rw-rw-rw-   0        0        0     1177 2023-04-19 05:41:51.000000 automation_rest_server-3.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/
+-rw-rw-rw-   0        0        0     1098 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      687 2022-08-30 06:56:12.000000 automation_rest_server-3.6.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      551 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/configuration/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/configuration/__init__.py
+-rw-rw-rw-   0        0        0      581 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/configuration/config.yaml
+-rw-rw-rw-   0        0        0     1099 2022-12-13 11:04:16.000000 automation_rest_server-3.6.8/automation_rest_server/configuration/firmware_build.yaml
+-rw-rw-rw-   0        0        0  1333232 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/configuration/pci.ids
+-rw-rw-rw-   0        0        0      157 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/configuration/version.yaml
+-rw-rw-rw-   0        0        0       83 2022-08-25 03:13:17.000000 automation_rest_server-3.6.8/automation_rest_server/configuration/web_server.yaml
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:18:57.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/
+-rw-rw-rw-   0        0        0        0 2022-08-10 09:04:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/models/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:20:01.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/models/__init__.py
+-rw-rw-rw-   0        0        0     4257 2023-05-10 02:20:31.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/models/helper.py
+-rw-rw-rw-   0        0        0     1944 2022-08-17 05:58:24.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/node_resource.py
+-rw-rw-rw-   0        0        0     1374 2022-08-30 04:43:20.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/test_resource.py
+-rw-rw-rw-   0        0        0      340 2022-08-25 03:00:40.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/web_resource.py
+-rw-rw-rw-   0        0        0     2536 2023-02-21 08:02:23.000000 automation_rest_server-3.6.8/automation_rest_server/rest_client/web_rest_client.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/__init__.py
+-rw-rw-rw-   0        0        0     1678 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/reset_server.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/__init__.py
+-rw-rw-rw-   0        0        0     2150 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/benchmark_resource.py
+-rw-rw-rw-   0        0        0     1956 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/build_firmware_resource.py
+-rw-rw-rw-   0        0        0      933 2022-12-12 01:57:01.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/git_resource.py
+-rw-rw-rw-   0        0        0      850 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/models/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/models/__init__.py
+-rw-rw-rw-   0        0        0     2044 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/models/ftp_server.py
+-rw-rw-rw-   0        0        0     1732 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/models/helper.py
+-rw-rw-rw-   0        0        0      958 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/oakgate_resource.py
+-rw-rw-rw-   0        0        0      691 2022-08-11 02:31:16.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/operation_resource.py
+-rw-rw-rw-   0        0        0     1641 2022-09-20 01:54:25.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/state_resource.py
+-rw-rw-rw-   0        0        0     1085 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/stop_flag_resource.py
+-rw-rw-rw-   0        0        0     6233 2022-12-03 07:36:31.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/test_resource.py
+-rw-rw-rw-   0        0        0     1295 2023-05-10 02:20:31.000000 automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/upgrade_resource.py
+-rw-rw-rw-   0        0        0     6063 2023-05-04 07:05:41.000000 automation_rest_server-3.6.8/automation_rest_server/run.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/__init__.py
+-rw-rw-rw-   0        0        0     6679 2022-09-20 04:46:34.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/database.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/
+-rw-rw-rw-   0        0        0        0 2021-11-12 08:10:50.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/__init__.py
+-rw-rw-rw-   0        0        0     3082 2023-04-19 05:40:44.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/slot.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/
+-rw-rw-rw-   0        0        0        0 2021-11-24 03:48:51.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/__init__.py
+-rw-rw-rw-   0        0        0     1434 2022-09-15 07:43:45.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py
+-rw-rw-rw-   0        0        0     3541 2023-04-17 06:49:22.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py
+-rw-rw-rw-   0        0        0      901 2023-04-19 03:39:13.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py
+-rw-rw-rw-   0        0        0     8894 2023-05-09 09:27:56.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/
+-rw-rw-rw-   0        0        0      214 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/__init__.py
+-rw-rw-rw-   0        0        0     2068 2023-04-25 07:50:43.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/nose_engine.py
+-rw-rw-rw-   0        0        0     4926 2023-02-16 01:39:59.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/oakgate_engine.py
+-rw-rw-rw-   0        0        0     4007 2023-03-02 06:19:25.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/perses_engine.py
+-rw-rw-rw-   0        0        0     1489 2022-09-30 01:53:36.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py
+-rw-rw-rw-   0        0        0      239 2023-04-07 02:04:12.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/special_parameter.py
+-rw-rw-rw-   0        0        0     3562 2022-09-20 07:48:14.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/sse_engine.py
+-rw-rw-rw-   0        0        0     4006 2023-04-25 07:48:48.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/venus_engine.py
+-rw-rw-rw-   0        0        0     1517 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_build.py
+-rw-rw-rw-   0        0        0     3049 2023-05-10 02:58:49.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_download.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/__init__.py
+-rw-rw-rw-   0        0        0     7168 2022-12-13 11:05:02.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py
+-rw-rw-rw-   0        0        0     5908 2023-05-10 07:34:30.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/logic_with_firmware_engine.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/oakgate/
+-rw-rw-rw-   0        0        0        0 2023-04-11 02:31:20.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/oakgate/__init__.py
+-rw-rw-rw-   0        0        0     2925 2023-04-11 02:43:50.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py
+-rw-rw-rw-   0        0        0     2691 2023-04-17 07:35:59.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py
+-rw-rw-rw-   0        0        0      671 2023-05-10 02:30:29.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py
+-rw-rw-rw-   0        0        0     1996 2023-05-10 03:22:37.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py
+-rw-rw-rw-   0        0        0     1585 2023-05-10 02:30:15.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py
+-rw-rw-rw-   0        0        0     2344 2023-04-09 02:31:46.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py
+-rw-rw-rw-   0        0        0     5139 2023-05-10 07:14:09.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/node_database.py
+-rw-rw-rw-   0        0        0    10717 2023-04-19 03:38:41.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/performance_database.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/reboot_engine/
+-rw-rw-rw-   0        0        0       50 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/reboot_engine/__init__.py
+-rw-rw-rw-   0        0        0     2439 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py
+-rw-rw-rw-   0        0        0     2055 2023-05-10 02:51:26.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/state.py
+-rw-rw-rw-   0        0        0      672 2022-12-13 03:29:14.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/status_file.py
+-rw-rw-rw-   0        0        0     5684 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_base.py
+-rw-rw-rw-   0        0        0     1973 2023-02-14 08:06:21.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_benchmark.py
+-rw-rw-rw-   0        0        0     3512 2023-02-07 07:54:27.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_benchmark_group.py
+-rw-rw-rw-   0        0        0     1263 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_case.py
+-rw-rw-rw-   0        0        0    22062 2023-05-10 02:21:32.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_pool.py
+-rw-rw-rw-   0        0        0      892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_reboot_handle.py
+-rw-rw-rw-   0        0        0     4365 2022-12-03 07:44:06.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_result.py
+-rw-rw-rw-   0        0        0     3757 2023-03-02 10:28:02.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_runner.py
+-rw-rw-rw-   0        0        0     4717 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/test_framework/test_suite.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/
+-rw-rw-rw-   0        0        0        0 2021-11-12 06:54:04.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/dll/
+-rw-rw-rw-   0        0        0        0 2021-10-23 02:17:43.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/dll/__init__.py
+-rw-rw-rw-   0        0        0    24064 2021-10-23 02:17:43.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/dll/buf.dll
+-rw-rw-rw-   0        0        0    12760 2021-10-23 02:17:43.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/dll/buf.so
+-rw-rw-rw-   0        0        0      777 2021-10-23 02:17:43.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/dll/build.py
+-rw-rw-rw-   0        0        0      861 2022-09-15 07:43:45.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/linux_nvme.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/
+-rw-rw-rw-   0        0        0        0 2021-11-23 06:34:00.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/__init__.py
+-rw-rw-rw-   0        0        0    14077 2021-11-23 06:29:25.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/buf.py
+-rw-rw-rw-   0        0        0     4722 2021-11-23 06:25:09.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/ctype.py
+-rw-rw-rw-   0        0        0    39204 2021-11-23 06:28:50.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/get_feature.py
+-rw-rw-rw-   0        0        0    38547 2022-09-15 07:43:45.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/ioctl.py
+-rw-rw-rw-   0        0        0    23303 2022-09-15 07:42:03.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/nvme.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/
+-rw-rw-rw-   0        0        0      256 2021-11-23 06:21:15.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/__init__.py
+-rw-rw-rw-   0        0        0    30449 2021-11-23 06:59:35.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/command.py
+-rw-rw-rw-   0        0        0    15322 2021-11-23 06:59:35.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/features.py
+-rw-rw-rw-   0        0        0     1104 2021-10-23 02:17:43.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/hmb.py
+-rw-rw-rw-   0        0        0    16135 2021-11-23 07:31:19.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/identify.py
+-rw-rw-rw-   0        0        0    13915 2021-11-23 06:59:59.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/log_page.py
+-rw-rw-rw-   0        0        0     2361 2021-11-12 10:37:37.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/memory.py
+-rw-rw-rw-   0        0        0    10510 2021-10-23 02:17:43.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/pcie.py
+-rw-rw-rw-   0        0        0    35527 2021-10-23 02:17:43.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/registers.py
+-rw-rw-rw-   0        0        0     9095 2021-11-24 06:24:21.000000 automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/utility_vu.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/diskpart/
+-rw-rw-rw-   0        0        0       56 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/diskpart/__init__.py
+-rw-rw-rw-   0        0        0      770 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/diskpart/diskpart.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/fio/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/fio/__init__.py
+-rw-rw-rw-   0        0        0    18967 2023-02-23 03:46:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/fio/fio.py
+-rw-rw-rw-   0        0        0     5032 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/fio/fio_linux.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/fio/tool/
+-rw-rw-rw-   0        0        0  4733892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/fio/tool/fio
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/git/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/git/__init__.py
+-rw-rw-rw-   0        0        0     5645 2023-03-02 10:20:30.000000 automation_rest_server-3.6.8/automation_rest_server/tool/git/git_operator.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/tool/iometer/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/tool/iometer/__init__.py
+-rw-rw-rw-   0        0        0     9223 2023-02-07 08:25:51.000000 automation_rest_server-3.6.8/automation_rest_server/tool/iometer/iometer.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server/utils/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/utils/__init__.py
+-rw-rw-rw-   0        0        0    12385 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/utils/buf.py
+-rw-rw-rw-   0        0        0     5636 2023-04-10 09:29:00.000000 automation_rest_server-3.6.8/automation_rest_server/utils/firmware_path.py
+-rw-rw-rw-   0        0        0     3697 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/utils/log.py
+-rw-rw-rw-   0        0        0      386 2023-02-23 02:34:33.000000 automation_rest_server-3.6.8/automation_rest_server/utils/message.py
+-rw-rw-rw-   0        0        0     3532 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/utils/nose_xml.py
+-rw-rw-rw-   0        0        0     1742 2022-09-20 07:22:33.000000 automation_rest_server-3.6.8/automation_rest_server/utils/pip_operation.py
+-rw-rw-rw-   0        0        0     1823 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/utils/process.py
+-rw-rw-rw-   0        0        0     9222 2022-06-02 02:49:38.000000 automation_rest_server-3.6.8/automation_rest_server/utils/ssh.py
+-rw-rw-rw-   0        0        0     5366 2022-12-22 01:47:58.000000 automation_rest_server-3.6.8/automation_rest_server/utils/system.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server.egg-info/
+-rw-rw-rw-   0        0        0      551 2023-05-10 08:47:25.000000 automation_rest_server-3.6.8/automation_rest_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7003 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/automation_rest_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 08:47:25.000000 automation_rest_server-3.6.8/automation_rest_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-10 08:47:25.000000 automation_rest_server-3.6.8/automation_rest_server.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       98 2023-05-10 08:47:25.000000 automation_rest_server-3.6.8/automation_rest_server.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-05-10 08:47:25.000000 automation_rest_server-3.6.8/automation_rest_server.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       64 2023-05-10 08:47:26.000000 automation_rest_server-3.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     1211 2023-05-10 08:47:20.000000 automation_rest_server-3.6.8/setup.py
```

### Comparing `automation_rest_server-3.6.7/LICENSE.txt` & `automation_rest_server-3.6.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/MANIFEST.in` & `automation_rest_server-3.6.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/PKG-INFO` & `automation_rest_server-3.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: automation_rest_server
-Version: 3.6.7
+Version: 3.6.8
 Summary: NVMe production server
 Home-page: https://pypi.org/project/automation_rest_server
 Author: yuwen123441
 Author-email: yuwen123441@126.com
 License: MIT License
 Description: UNKNOWN
 Keywords: runner,server
```

### Comparing `automation_rest_server-3.6.7/automation_rest_server/configuration/config.yaml` & `automation_rest_server-3.6.8/automation_rest_server/configuration/config.yaml`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/configuration/firmware_build.yaml` & `automation_rest_server-3.6.8/automation_rest_server/configuration/firmware_build.yaml`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/configuration/pci.ids` & `automation_rest_server-3.6.8/automation_rest_server/configuration/pci.ids`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/rest_client/resource/models/helper.py` & `automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/models/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,11 +131,11 @@
 
 class TestType(object):
 
     TestCase = 1
     TestSuite = 2
     TestBenchmark = 3
     TestBenchmarkGroup = 4
-    DownloadSerial = 10
+    UPGRADE = 10
 
     def __init__(self):
         pass
```

### Comparing `automation_rest_server-3.6.7/automation_rest_server/rest_client/resource/node_resource.py` & `automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/node_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/rest_client/resource/test_resource.py` & `automation_rest_server-3.6.8/automation_rest_server/rest_client/resource/test_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/rest_client/web_rest_client.py` & `automation_rest_server-3.6.8/automation_rest_server/rest_client/web_rest_client.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/rest_server/reset_server.py` & `automation_rest_server-3.6.8/automation_rest_server/rest_server/reset_server.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/benchmark_resource.py` & `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/benchmark_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/build_firmware_resource.py` & `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/build_firmware_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/git_resource.py` & `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/git_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py` & `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/models/ftp_server.py` & `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/models/ftp_server.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/models/helper.py` & `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/models/helper.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/oakgate_resource.py` & `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/oakgate_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/operation_resource.py` & `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/operation_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/state_resource.py` & `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/state_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/stop_flag_resource.py` & `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/stop_flag_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/test_resource.py` & `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/test_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/rest_server/resource/upgrade_resource.py` & `automation_rest_server-3.6.8/automation_rest_server/rest_server/resource/upgrade_resource.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,17 +21,18 @@
         self.test_pool = TestPool()
 
     @marshal_with(resource_fields, envelope='resource')
     def post(self):
         args = PARSER.parse_args()
         parameters = eval(args["parameters"])
         execute_name = args['execute_name']
+        print("download para", parameters, execute_name)
         result = self._async_download(execute_name, parameters)
         return result
 
     def _async_download(self, test_name, parameters):
         data = list()
-        key = self.test_pool.add_test(test_name, TestType.DownloadSerial, parameters)
+        key = self.test_pool.add_test(test_name, TestType.UPGRADE, parameters)
         data.append(key)
         state_ = State.PASS if key is not None else State.ERROR_NOT_FOUND
         result = {"data": data, "state": state_, "msg": "Test {} key {}".format(test_name, key)}
         return result
```

### Comparing `automation_rest_server-3.6.7/automation_rest_server/run.py` & `automation_rest_server-3.6.8/automation_rest_server/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from test_framework.test_pool import TestPool
 from test_framework.test_suite import TestSuite
 from test_framework.test_case import TestCase
 from rest_server.reset_server import *
 from rest_server.resource.models.ftp_server import thread_start_ftp_server
 from test_framework.database import update_abnormal_end_tests
 from rest_client.web_rest_client import decorate_api_node_startup
+from test_framework.node_database import check_node_table
 
 
 def add_sub_argument_group(subparsers, name, handler_function):
     regression_parser = subparsers.add_parser(name, help='%s tests executor' % name)
     regression_required_arguments = regression_parser.add_argument_group('required arguments')
     regression_required_arguments.add_argument('--name', '-n', type=str, required=False,
                                                help='test suite ,test case name or operation name', default="fio")
@@ -53,14 +54,15 @@
     add_sub_argument_group(subparsers, 'testcase', test_case_handle)
     add_sub_argument_group(subparsers, 'start', start_rest_server)
     return parser
 
 
 @decorate_api_node_startup
 def start_rest_server(args):
+    check_node_table()
     _ = TestPool(args.reboot, args.dut)
     if args.reboot is False:
         update_abnormal_end_tests()
     thread_start_ftp_server()
     APP.run(host="0.0.0.0", port=args.port)
```

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/database.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/dut/slot.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import re
 import platform
 from utils import log
 from utils.ssh import SSH
 from utils.system import get_vendor_name
 from test_framework.state import SlotState
 
+
 class PowercycleSlot(object):
 
     def __init__(self):
         super().__init__()
         self.ssh = None
         self.cntid = None
         self.nsid = None
```

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/engine/nose_engine.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/nose_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             msg += err.decode('utf-8')
         if out is not None:
             msg += out.decode('utf-8')
         return msg
 
     def save_msg(self, msg, test_case):
         test_function = test_case.split(".")
-        log_file = "{}_{}.log".format(test_function[-1],time.time())
+        log_file = "{}_{}.log".format(test_function[-1], time.time())
         log_path = os.path.join(self.log_path, log_file)
         with open(log_path, "w") as file_:
             file_.write(msg)
         return log_path
 
     def command_run_test(self, test_case, test_path):
         test_function = test_case.split(".")
```

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/engine/oakgate_engine.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/oakgate_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/engine/perses_engine.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/perses_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/engine/sse_engine.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/engine/sse_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_build.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_build.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_download.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_download.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 from multiprocessing import Queue
 from test_framework.state import State, DownloadType
-from test_framework.firmware_engine.oakgate_download_engine import OakgateDownload
-from test_framework.firmware_engine.perses_download_engine import PersesDownload
+from test_framework.firmware_engine.oakgate_download_engine import OakgateDownloader
+from test_framework.firmware_engine.perses_download_engine import PersesDownloader
+from test_framework.firmware_engine.logic_with_firmware_engine import LogicFWDownloader
 from utils.process import MyProcess
 from utils.system import get_automation_platform
 from tool.git.git_operator import GitOperator
 from utils import log
 
 
 class FirmwareDownloader(object):
@@ -14,22 +15,23 @@
     def __init__(self, execute_name):
         self.process_run_ = None
         self.results = list()
         self.execute_name = execute_name
         self.runner = None
 
     def get_download_engine(self, test_parameters):
-        platform = get_automation_platform()
-        if platform == "oakgate":
-            self.runner = OakgateDownload()
-        elif platform == "perses":
-            self.runner = PersesDownload()
-        else:
-            pass
-
+        if int(test_parameters["upgrade_type"]) in [DownloadType.two_step_download, DownloadType.NVMe]:
+            platform = get_automation_platform()
+            if platform == "oakgate":
+                self.runner = OakgateDownloader()
+            elif platform == "perses":
+                self.runner = PersesDownloader()
+        elif int(test_parameters["upgrade_type"]) == DownloadType.logic_fw:
+            self.runner = LogicFWDownloader()
+            
     @staticmethod
     def update_git(parameters):
         if "git_version" in parameters.keys():
             user = parameters["git_user"]
             passwd = parameters["git_key"]
             git_version = parameters["git_version"]
             log.INFO(f"Git update: user: {user}, passwd: {passwd}, version: {git_version}")
@@ -37,17 +39,17 @@
             msg, ret = git.update_latest_code(git_version)
             log.INFO(f"Git update result:  {ret}, msg: {msg}")
 
     def _run(self, test_parameters, queue):
         try:
             self.get_download_engine(test_parameters)
             if self.runner is not None:
-                status, log = self.runner.run(test_parameters)
+                status, msg = self.runner.run(test_parameters)
                 ret = State.PASS if status == 0 else State.FAIL
-                result = {"name": self.execute_name, "result": ret, "log": log}
+                result = {"name": self.execute_name, "result": ret, "log": msg}
             else:
                 result = {"name": self.execute_name, "result": State.FAIL, "log": "prun start in wrong path"}
             queue.put(result)
         except Exception as e:
             log.INFO(e)
             result = None
         return result
```

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from utils.system import decorate_exception_result
 from test_framework.state import UpgradeType
 from test_framework.firmware_engine.oakgate.nvme_download import NVMeDownload
 from test_framework.firmware_engine.oakgate.two_step_download import OakgateTwoStepDownload
 
 
-class OakgateDownload(object):
+class OakgateDownloader(object):
 
     def __init__(self):
         pass
 
     @decorate_exception_result
     def run(self, parameters):
         download_type = int(parameters.get("upgrade_type", 1))
```

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import os
 import platform
 from multiprocessing import Queue
 from utils.system import decorate_exception_result
 from test_framework.engine.perses_engine import PersesEngine
 from test_framework.firmware_engine.serial_download_engine import PersesSerialDownloader
 from test_framework.test_base import TestBase
-from utils import log
 from test_framework.state import State, UpgradeType
+from utils import log
 
 
-class PersesDownload(TestBase):
+class PersesDownloader(TestBase):
 
     def __init__(self):
-        super(PersesDownload, self).__init__()
+        super(PersesDownloader, self).__init__()
         self.root_path = os.getcwd()
         self.download_testcase = "test_debug:TestPowerCycleDebug.test_auto_fw_upgrade"
 
     def nvme_download(self, parameters):
         queue = Queue()
         ret, logs = -1, ""
         test_path = self.get_all_script_path(self.download_testcase)
```

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from test_framework.engine.perses_power_cycle_engine import PersesPowerEngine
 from test_framework.test_base import TestBase
 from utils import log
 from utils.firmware_path import FirmwareBinPath
 from test_framework.state import State
 
 
-class PersesDownload(TestBase):
+class PersesDownloader(TestBase):
 
     def __init__(self):
-        super(PersesDownload, self).__init__()
+        super(PersesDownloader, self).__init__()
         self.root_path = os.getcwd()
         self.power_engine = PersesPowerEngine()
         self.fw_path_manage = FirmwareBinPath()
         self.download_testcase = "test_debug:TestPowerCycleDebug.test_fw_upgrade_with_clearspi"
 
     @decorate_exception_result
     def run(self, parameters):
```

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/node_database.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/node_database.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,40 +26,36 @@
 
     def create_node_state_table(self, node_ip, port):
         table_name ="{}:{}".format(node_ip, port)
         if self.is_exist_table(table_name) is False:
             self.create_table(table_name, NODE_STATE_TABLE_COLUM)
         return table_name
 
-    def create_new_node(self, node, port):
-        table_name = self.create_node_state_table(node["ip"], port)
+    def create_new_node(self, ip, port):
+        table_name = self.create_node_state_table(ip, port)
         update_time = self.get_datetime()
-        self.insert_to_table("node", vendor=node["vendor_name"],
-            ip=node["ip"],
-            name="env_{}".format(node["ip"]),
-            system=node["operating_system"],
-            capacity=node["capacity"],
-            fw=node["fw_version"],
-            state=NodeState.verdicts_map[NodeState.Idle],
-            state_table=table_name,
-            port=port,
-            update_time=update_time)
+        self.insert_to_table("node",
+                             ip=ip,
+                             state=NodeState.verdicts_map[NodeState.Idle],
+                             state_table=table_name,
+                             port=port,
+                             update_time=update_time)
 
     def update_exist_node(self, node, port):
         update_time = self.get_datetime()
         platform = get_automation_platform()
         str_date = "`system`='{}',capacity='{}',fw='{}',vendor='{}', update_time='{}',platform='{}'".format(
             node["operating_system"], node["capacity"], node["fw_version"],
             node["vendor_name"], update_time, platform)
         update_command = "UPDATE node SET {} WHERE ip='{}' AND port='{}'".format(str_date, node["ip"], port)
         self.cursor.execute(update_command)
         self.conn.commit()
 
-    def is_exist_node(self, node, port):
-        sql_command = "SELECT * from node WHERE ip='{}' AND port='{}'".format(node["ip"], port)
+    def is_exist_node(self, ip, port):
+        sql_command = "SELECT * from node WHERE ip='{}' AND port='{}'".format(ip, port)
         self.cursor.execute(sql_command)
         gets = self.cursor.fetchone()
         result = True if gets else False
         return result
 
     def get_node_table_name(self, ip, port):
         sea_string = "SELECT state_table FROM node WHERE `ip`='{}' AND `port`={}".format(ip, port)
@@ -84,43 +80,39 @@
         self.conn.commit()
 
     def update_power_cycle_node_state(self, state):
         if "TARGETIP" in os.environ.keys():
             target_ip = os.environ['TARGETIP']
             port = os.environ.get('prun_port', '5000')
             if target_ip != "0.0.0.0":
-                table = "`{}:{}`".format(target_ip, port)
+                table = "{}:{}".format(target_ip, port)
                 if self.is_exist_table(target_ip) is True:
                     self.insert_to_table(table, state=NodeState.verdicts_map[state])
 
 
-def update_env_state(func):
-    def func_wrapper(*args, **kwargs):
-        node = func(*args, **kwargs)
-        try:
-            port = os.environ.get('prun_port', '5000')
-            sql_connection = NodeSqlConnection()
-            if sql_connection.is_exist_node(node, port) is True:
-                sql_connection.update_exist_node(node, port)
-            else:
-                sql_connection.create_new_node(node, port)
-        except Exception as all_exception:
-            log.ERR(all_exception)
-        return node
-    return func_wrapper
+def check_node_table():
+    try:
+        ip = get_ip_address()
+        port = os.environ.get('prun_port', '5000')
+        sql_connection = NodeSqlConnection()
+        if sql_connection.is_exist_node(ip, port) is False:
+            sql_connection.create_new_node(ip, port)
+    except Exception as all_exception:
+        log.ERR(all_exception)
+    return
 
 
-def update_node_state(func):
+def decorate_update_node_state(func):
     def func_wrapper(*args, **kwargs):
         is_updated, state = func(*args, **kwargs)
         if is_updated is True:
             try:
                 sql_connection = NodeSqlConnection()
                 sql_connection.update_node_state(state)
-                sql_connection.update_power_cycle_node_state(state)
+                # sql_connection.update_power_cycle_node_state(state)
             except Exception as all_exception:
                 log.ERR(all_exception)
         return is_updated, state
     return func_wrapper
 
 
 def node_heart_beat(func):
```

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/performance_database.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/performance_database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/state.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/state.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,23 +38,23 @@
 class TestType(object):
 
     TestCase = 1
     TestSuite = 2
     TestBenchmark = 3
     TestBenchmarkGroup = 4
     TestRebootHandle = 5
-    DownloadSerial = 10
+    UPGRADE = 10
     BuildFirmware = 11
     url_map = {
         TestCase: "test",
         TestSuite: "test",
         TestBenchmark: "test",
         TestBenchmarkGroup: "test",
         TestRebootHandle: "test",
-        DownloadSerial: "download",
+        UPGRADE: "download",
         BuildFirmware: "build"
     }
 
     def __init__(self):
         pass
 
 
@@ -70,15 +70,16 @@
         Idle: "idle",
     }
 
 
 class DownloadType(object):
 
     NVMe = 0
-    SerialTestPlatform = 1
+    two_step_download = 1
+    logic_fw = 2
 
 
 class SlotState(object):
     Idle = 0
     Standby = 1
     Build = 2
     Download = 3
```

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/status_file.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/status_file.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/test_base.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_base.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/test_benchmark.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/test_benchmark_group.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_benchmark_group.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/test_case.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_case.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/test_pool.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from test_framework.state import State
 from test_framework.state import TestType
 from test_framework.node_database import node_heart_beat
 from test_framework.state import NodeState
 from test_framework.status_file import StatusFile
 from test_framework.dut.slot import Slot
 from rest_client.web_rest_client import decorate_api_update_test_result, decorate_api_update_node_status
+from test_framework.node_database import decorate_update_node_state
 from utils import log
 
 
 def singleton(cls):
     _instance = {}
 
     def inner(*args, **kwargs):
@@ -238,20 +239,25 @@
 
     @decorate_api_update_node_status
     def init_node_state(self):
         is_updated = True
         node_state = NodeState.Online
         return is_updated, node_state
 
+    @decorate_update_node_state
     @decorate_api_update_node_status
     def check_and_update_node_state(self, org_node_state):
         is_updated = False
         latest_state = self.get_current_node_state()
         if org_node_state != latest_state:
             is_updated = True
+        now = datetime.now(timezone(timedelta(hours=+8)))
+        if (now.hour == 23 and now.minute == 59 and now.second in range(49, 59)) or\
+                (now.hour == 0 and now.minute == 0 and now.second in range(0, 10)):
+            is_updated = True
         return is_updated, latest_state
 
     def get_current_node_state(self):
         tests = [test for test in self.test_pool if test["state"] in [State.NOT_START, State.RUNNING, State.NONE]]
         if tests:
             node_state = NodeState.Running
         else:
@@ -307,17 +313,17 @@
             self.set_test_parameters(test_parameters)
             thread_, test_object = self._start_test_case_thread(test_name, test_parameters)
         elif test_type == TestType.TestSuite:
             self.set_test_parameters(test_parameters)
             thread_, test_object = self._start_test_suite_thread(test_name, test_parameters)
         elif test_type == TestType.TestBenchmark:
             thread_, test_object = self._start_benchmark_test_thread(test_parameters)
-        elif test_type == TestType.DownloadSerial:
+        elif test_type == TestType.UPGRADE:
             self.set_test_parameters(test_parameters)
-            thread_, test_object = self._start_download_serial_thread(test_name, test_parameters)
+            thread_, test_object = self._start_upgrade_thread(test_name, test_parameters)
         elif test_type == TestType.TestBenchmarkGroup:
             thread_, test_object = self._start_benchmark_group_test_thread(test_name, test_parameters)
         elif test_type == TestType.BuildFirmware:
             thread_, test_object = self._start_firmware_build_thread(test_name, test_parameters)
         elif test_type == TestType.TestRebootHandle:
             thread_, test_object = self._start_reboot_handle_thread(test_name, test_parameters)
         return thread_, test_object
@@ -352,15 +358,15 @@
         test_case = TestCase(test_name)
         thread_tc = MyThread(target=test_case.run, args=(test_name, test_parameters,))
         thread_tc.setDaemon(True)
         thread_tc.start()
         return thread_tc, test_case
 
     @staticmethod
-    def _start_download_serial_thread(execute_name, test_parameters):
+    def _start_upgrade_thread(execute_name, test_parameters):
         downloader = FirmwareDownloader(execute_name)
         thread_tc = MyThread(target=downloader.run, args=(test_parameters,))
         thread_tc.setDaemon(True)
         thread_tc.start()
         return thread_tc, downloader
 
     @staticmethod
```

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/test_reboot_handle.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_reboot_handle.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/test_result.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_result.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/test_runner.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_runner.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/test_framework/test_suite.py` & `automation_rest_server-3.6.8/automation_rest_server/test_framework/test_suite.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/dll/buf.dll` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/dll/buf.dll`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/dll/buf.so` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/dll/buf.so`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/dll/build.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/dll/build.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/linux_nvme.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/linux_nvme.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/buf.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/buf.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/ctype.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/ctype.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/get_feature.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/get_feature.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/ioctl.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/ioctl.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/nvme.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/nvme.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/command.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/command.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/features.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/features.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/hmb.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/hmb.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/identify.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/identify.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/log_page.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/log_page.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/memory.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/memory.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/pcie.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/pcie.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/struct/registers.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/struct/registers.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/device/nvme/utility_vu.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/device/nvme/utility_vu.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/diskpart/diskpart.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/diskpart/diskpart.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/fio/fio.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/fio/fio.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/fio/fio_linux.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/fio/fio_linux.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/fio/tool/fio` & `automation_rest_server-3.6.8/automation_rest_server/tool/fio/tool/fio`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/git/git_operator.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/git/git_operator.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/tool/iometer/iometer.py` & `automation_rest_server-3.6.8/automation_rest_server/tool/iometer/iometer.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/utils/buf.py` & `automation_rest_server-3.6.8/automation_rest_server/utils/buf.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/utils/firmware_path.py` & `automation_rest_server-3.6.8/automation_rest_server/utils/firmware_path.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/utils/log.py` & `automation_rest_server-3.6.8/automation_rest_server/utils/log.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/utils/nose_xml.py` & `automation_rest_server-3.6.8/automation_rest_server/utils/nose_xml.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/utils/pip_operation.py` & `automation_rest_server-3.6.8/automation_rest_server/utils/pip_operation.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/utils/process.py` & `automation_rest_server-3.6.8/automation_rest_server/utils/process.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/utils/ssh.py` & `automation_rest_server-3.6.8/automation_rest_server/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server/utils/system.py` & `automation_rest_server-3.6.8/automation_rest_server/utils/system.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.7/automation_rest_server.egg-info/PKG-INFO` & `automation_rest_server-3.6.8/automation_rest_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: automation-rest-server
-Version: 3.6.7
+Version: 3.6.8
 Summary: NVMe production server
 Home-page: https://pypi.org/project/automation_rest_server
 Author: yuwen123441
 Author-email: yuwen123441@126.com
 License: MIT License
 Description: UNKNOWN
 Keywords: runner,server
```

### Comparing `automation_rest_server-3.6.7/automation_rest_server.egg-info/SOURCES.txt` & `automation_rest_server-3.6.8/automation_rest_server.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -69,16 +69,18 @@
 automation_rest_server/test_framework/engine/__init__.py
 automation_rest_server/test_framework/engine/nose_engine.py
 automation_rest_server/test_framework/engine/oakgate_engine.py
 automation_rest_server/test_framework/engine/perses_engine.py
 automation_rest_server/test_framework/engine/perses_power_cycle_engine.py
 automation_rest_server/test_framework/engine/special_parameter.py
 automation_rest_server/test_framework/engine/sse_engine.py
+automation_rest_server/test_framework/engine/venus_engine.py
 automation_rest_server/test_framework/firmware_engine/__init__.py
 automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py
+automation_rest_server/test_framework/firmware_engine/logic_with_firmware_engine.py
 automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py
 automation_rest_server/test_framework/firmware_engine/perses_download_engine.py
 automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py
 automation_rest_server/test_framework/firmware_engine/serial_download_engine.py
 automation_rest_server/test_framework/firmware_engine/oakgate/__init__.py
 automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py
 automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py
```

### Comparing `automation_rest_server-3.6.7/setup.py` & `automation_rest_server-3.6.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 packages = ["automation_rest_server"]
 #python setup.py sdist upload  
 #python setup.py bdist_wheel
 
 setup(
     name = 'automation_rest_server',
-    version = '3.6.7',
+    version = '3.6.8',
     keywords = ['runner', 'server'],
     description = 'NVMe production server',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'License :: OSI Approved :: MIT License',
@@ -21,15 +21,16 @@
 						'flask-restful',
 						'requests',
 						'PyMySQL==1.0.2',
 						'pyftpdlib',
 						'nose',
 						'nose-printlog',
                         'checksumdir',
-                        'pyyaml'],
+                        'pyyaml',
+                        'py7zr'],
     packages = find_packages(),
     include_package_data=True, 
     author = 'yuwen123441',
     author_email = 'yuwen123441@126.com',
     platforms = 'any',
     entry_points = {
         'console_scripts': [
```

