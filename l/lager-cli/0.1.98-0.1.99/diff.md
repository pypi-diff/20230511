# Comparing `tmp/lager-cli-0.1.98.tar.gz` & `tmp/lager-cli-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lager-cli-0.1.98.tar", last modified: Fri Aug 20 22:22:23 2021, max compression
+gzip compressed data, was "lager-cli-0.1.99.tar", last modified: Tue Sep  7 18:14:37 2021, max compression
```

## Comparing `lager-cli-0.1.98.tar` & `lager-cli-0.1.99.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.156313 lager-cli-0.1.98/
--rw-r--r--   0 ehaas      (501) staff       (20)    33886 2020-10-17 16:52:22.000000 lager-cli-0.1.98/LICENSE
--rw-r--r--   0 ehaas      (501) staff       (20)      853 2021-08-20 22:22:23.155773 lager-cli-0.1.98/PKG-INFO
--rw-r--r--   0 ehaas      (501) staff       (20)      126 2020-10-16 03:32:31.000000 lager-cli-0.1.98/README.md
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.103441 lager-cli-0.1.98/lager_cli/
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.110774 lager-cli-0.1.98/lager_cli/PyCRC/
--rw-r--r--   0 ehaas      (501) staff       (20)     1679 2021-08-20 19:34:40.000000 lager-cli-0.1.98/lager_cli/PyCRC/CRC16.py
--rw-r--r--   0 ehaas      (501) staff       (20)     1903 2021-08-20 19:34:40.000000 lager-cli-0.1.98/lager_cli/PyCRC/CRC16DNP.py
--rw-r--r--   0 ehaas      (501) staff       (20)     1890 2021-08-20 19:34:40.000000 lager-cli-0.1.98/lager_cli/PyCRC/CRC16Kermit.py
--rw-r--r--   0 ehaas      (501) staff       (20)     1794 2021-08-20 19:34:40.000000 lager-cli-0.1.98/lager_cli/PyCRC/CRC16SICK.py
--rw-r--r--   0 ehaas      (501) staff       (20)     1704 2021-08-20 19:34:40.000000 lager-cli-0.1.98/lager_cli/PyCRC/CRC32.py
--rw-r--r--   0 ehaas      (501) staff       (20)     2267 2021-08-20 19:34:40.000000 lager-cli-0.1.98/lager_cli/PyCRC/CRCCCITT.py
--rwxr-xr-x   0 ehaas      (501) staff       (20)      123 2021-08-20 19:34:40.000000 lager-cli-0.1.98/lager_cli/PyCRC/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)      956 2021-08-20 22:21:56.000000 lager-cli-0.1.98/lager_cli/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)      150 2020-07-01 20:32:58.000000 lager-cli-0.1.98/lager_cli/__main__.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.111763 lager-cli-0.1.98/lager_cli/adc/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-12-01 22:44:05.000000 lager-cli-0.1.98/lager_cli/adc/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     1977 2020-12-21 17:50:11.000000 lager-cli-0.1.98/lager_cli/adc/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.120284 lager-cli-0.1.98/lager_cli/auth/
--rw-r--r--   0 ehaas      (501) staff       (20)     3122 2021-01-12 18:34:44.000000 lager-cli-0.1.98/lager_cli/auth/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     3486 2020-08-21 19:02:41.000000 lager-cli-0.1.98/lager_cli/auth/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.121509 lager-cli-0.1.98/lager_cli/ble/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2021-03-09 18:05:12.000000 lager-cli-0.1.98/lager_cli/ble/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     2619 2021-04-22 22:14:22.000000 lager-cli-0.1.98/lager_cli/ble/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.122625 lager-cli-0.1.98/lager_cli/canbus/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-10-21 16:03:40.000000 lager-cli-0.1.98/lager_cli/canbus/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     5626 2021-04-14 22:10:26.000000 lager-cli-0.1.98/lager_cli/canbus/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.123729 lager-cli-0.1.98/lager_cli/chip_erase/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2021-06-14 17:50:49.000000 lager-cli-0.1.98/lager_cli/chip_erase/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     1153 2021-06-15 15:24:50.000000 lager-cli-0.1.98/lager_cli/chip_erase/commands.py
--rw-r--r--   0 ehaas      (501) staff       (20)     4405 2021-07-08 22:17:50.000000 lager-cli-0.1.98/lager_cli/cli.py
--rw-r--r--   0 ehaas      (501) staff       (20)     3358 2020-10-16 16:54:45.000000 lager-cli-0.1.98/lager_cli/config.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.124945 lager-cli-0.1.98/lager_cli/connect/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-07-09 18:58:17.000000 lager-cli-0.1.98/lager_cli/connect/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     4333 2021-06-15 15:26:22.000000 lager-cli-0.1.98/lager_cli/connect/commands.py
--rw-r--r--   0 ehaas      (501) staff       (20)    21547 2021-07-21 20:23:44.000000 lager-cli-0.1.98/lager_cli/context.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.126255 lager-cli-0.1.98/lager_cli/devenv/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-06-30 23:18:40.000000 lager-cli-0.1.98/lager_cli/devenv/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     5498 2021-07-16 20:31:17.000000 lager-cli-0.1.98/lager_cli/devenv/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.127587 lager-cli-0.1.98/lager_cli/erase/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-06-30 23:18:40.000000 lager-cli-0.1.98/lager_cli/erase/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)      752 2020-07-21 18:37:02.000000 lager-cli-0.1.98/lager_cli/erase/commands.py
--rw-r--r--   0 ehaas      (501) staff       (20)      103 2020-10-01 23:32:31.000000 lager-cli-0.1.98/lager_cli/exceptions.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.128880 lager-cli-0.1.98/lager_cli/exec/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-06-30 23:18:40.000000 lager-cli-0.1.98/lager_cli/exec/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     6093 2021-07-08 20:58:22.000000 lager-cli-0.1.98/lager_cli/exec/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.130144 lager-cli-0.1.98/lager_cli/flash/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-06-30 23:18:40.000000 lager-cli-0.1.98/lager_cli/flash/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     2129 2021-04-09 03:35:22.000000 lager-cli-0.1.98/lager_cli/flash/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.131205 lager-cli-0.1.98/lager_cli/gateway/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-04-30 16:59:17.000000 lager-cli-0.1.98/lager_cli/gateway/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     5506 2021-01-29 00:36:06.000000 lager-cli-0.1.98/lager_cli/gateway/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.132713 lager-cli-0.1.98/lager_cli/gdbserver/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-07-09 17:46:44.000000 lager-cli-0.1.98/lager_cli/gdbserver/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     3233 2021-03-10 19:51:16.000000 lager-cli-0.1.98/lager_cli/gdbserver/commands.py
--rw-r--r--   0 ehaas      (501) staff       (20)     6455 2021-04-14 19:23:12.000000 lager-cli-0.1.98/lager_cli/gdbserver/tunnel.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.134443 lager-cli-0.1.98/lager_cli/gpio/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-08-12 21:54:20.000000 lager-cli-0.1.98/lager_cli/gpio/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     3582 2021-06-16 20:17:12.000000 lager-cli-0.1.98/lager_cli/gpio/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.135791 lager-cli-0.1.98/lager_cli/grafana/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2021-04-27 19:37:07.000000 lager-cli-0.1.98/lager_cli/grafana/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     1476 2021-04-27 19:38:29.000000 lager-cli-0.1.98/lager_cli/grafana/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.136942 lager-cli-0.1.98/lager_cli/i2c/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2021-03-11 23:33:10.000000 lager-cli-0.1.98/lager_cli/i2c/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     6789 2021-03-17 23:14:11.000000 lager-cli-0.1.98/lager_cli/i2c/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.138685 lager-cli-0.1.98/lager_cli/job/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-05-22 20:02:14.000000 lager-cli-0.1.98/lager_cli/job/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     1071 2020-10-28 21:50:47.000000 lager-cli-0.1.98/lager_cli/job/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.140021 lager-cli-0.1.98/lager_cli/lister/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-05-05 19:15:34.000000 lager-cli-0.1.98/lager_cli/lister/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     1145 2020-08-26 21:56:57.000000 lager-cli-0.1.98/lager_cli/lister/commands.py
--rw-r--r--   0 ehaas      (501) staff       (20)     6146 2021-08-20 22:11:40.000000 lager-cli-0.1.98/lager_cli/matchers.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.141183 lager-cli-0.1.98/lager_cli/openocd/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-09-10 21:09:47.000000 lager-cli-0.1.98/lager_cli/openocd/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     1815 2020-09-10 21:20:46.000000 lager-cli-0.1.98/lager_cli/openocd/commands.py
--rw-r--r--   0 ehaas      (501) staff       (20)     9300 2021-03-12 23:18:29.000000 lager-cli-0.1.98/lager_cli/paramtypes.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.142044 lager-cli-0.1.98/lager_cli/pigpio/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2021-03-10 19:46:50.000000 lager-cli-0.1.98/lager_cli/pigpio/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     1490 2021-03-10 19:46:50.000000 lager-cli-0.1.98/lager_cli/pigpio/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.143357 lager-cli-0.1.98/lager_cli/pip/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2021-07-08 22:15:46.000000 lager-cli-0.1.98/lager_cli/pip/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     1843 2021-07-08 23:11:00.000000 lager-cli-0.1.98/lager_cli/pip/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.144462 lager-cli-0.1.98/lager_cli/python/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-09-10 22:40:41.000000 lager-cli-0.1.98/lager_cli/python/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     8476 2021-07-12 16:42:49.000000 lager-cli-0.1.98/lager_cli/python/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.146063 lager-cli-0.1.98/lager_cli/reset/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-06-30 23:18:40.000000 lager-cli-0.1.98/lager_cli/reset/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)      829 2020-07-21 18:53:46.000000 lager-cli-0.1.98/lager_cli/reset/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.147278 lager-cli-0.1.98/lager_cli/run/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-06-30 23:18:40.000000 lager-cli-0.1.98/lager_cli/run/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)      561 2020-07-21 18:54:17.000000 lager-cli-0.1.98/lager_cli/run/commands.py
--rw-r--r--   0 ehaas      (501) staff       (20)      951 2020-10-01 23:24:49.000000 lager-cli-0.1.98/lager_cli/safe_unpickle.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.148305 lager-cli-0.1.98/lager_cli/serial_ports/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-11-03 18:15:25.000000 lager-cli-0.1.98/lager_cli/serial_ports/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     1090 2020-11-03 18:19:53.000000 lager-cli-0.1.98/lager_cli/serial_ports/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.149219 lager-cli-0.1.98/lager_cli/setter/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-05-05 21:50:01.000000 lager-cli-0.1.98/lager_cli/setter/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)      785 2020-07-01 17:04:51.000000 lager-cli-0.1.98/lager_cli/setter/commands.py
--rw-r--r--   0 ehaas      (501) staff       (20)     5576 2021-08-20 21:56:41.000000 lager-cli-0.1.98/lager_cli/simple_hdlc.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.150228 lager-cli-0.1.98/lager_cli/spi/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2021-03-11 23:33:03.000000 lager-cli-0.1.98/lager_cli/spi/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)    11229 2021-03-17 23:14:11.000000 lager-cli-0.1.98/lager_cli/spi/commands.py
--rw-r--r--   0 ehaas      (501) staff       (20)    12256 2021-08-20 22:11:40.000000 lager-cli-0.1.98/lager_cli/status.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.151732 lager-cli-0.1.98/lager_cli/testrun/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-07-07 18:11:15.000000 lager-cli-0.1.98/lager_cli/testrun/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     4102 2021-04-14 22:08:40.000000 lager-cli-0.1.98/lager_cli/testrun/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.152888 lager-cli-0.1.98/lager_cli/uart/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-06-29 23:01:20.000000 lager-cli-0.1.98/lager_cli/uart/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     4789 2021-08-20 21:56:41.000000 lager-cli-0.1.98/lager_cli/uart/commands.py
--rw-r--r--   0 ehaas      (501) staff       (20)     7146 2020-11-02 17:37:15.000000 lager-cli-0.1.98/lager_cli/util.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.153985 lager-cli-0.1.98/lager_cli/webcam/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2021-02-03 04:05:31.000000 lager-cli-0.1.98/lager_cli/webcam/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     1492 2021-02-03 06:52:54.000000 lager-cli-0.1.98/lager_cli/webcam/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.154968 lager-cli-0.1.98/lager_cli/wifi/
--rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-09-27 22:31:49.000000 lager-cli-0.1.98/lager_cli/wifi/__init__.py
--rw-r--r--   0 ehaas      (501) staff       (20)     3156 2021-03-15 15:57:15.000000 lager-cli-0.1.98/lager_cli/wifi/commands.py
-drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-08-20 22:22:23.106843 lager-cli-0.1.98/lager_cli.egg-info/
--rw-r--r--   0 ehaas      (501) staff       (20)      853 2021-08-20 22:22:22.000000 lager-cli-0.1.98/lager_cli.egg-info/PKG-INFO
--rw-r--r--   0 ehaas      (501) staff       (20)     2420 2021-08-20 22:22:22.000000 lager-cli-0.1.98/lager_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ehaas      (501) staff       (20)        1 2021-08-20 22:22:22.000000 lager-cli-0.1.98/lager_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ehaas      (501) staff       (20)       45 2021-08-20 22:22:22.000000 lager-cli-0.1.98/lager_cli.egg-info/entry_points.txt
--rw-r--r--   0 ehaas      (501) staff       (20)      432 2021-08-20 22:22:22.000000 lager-cli-0.1.98/lager_cli.egg-info/requires.txt
--rw-r--r--   0 ehaas      (501) staff       (20)       10 2021-08-20 22:22:22.000000 lager-cli-0.1.98/lager_cli.egg-info/top_level.txt
--rw-r--r--   0 ehaas      (501) staff       (20)       38 2021-08-20 22:22:23.156487 lager-cli-0.1.98/setup.cfg
--rw-r--r--   0 ehaas      (501) staff       (20)     2132 2021-06-16 20:17:12.000000 lager-cli-0.1.98/setup.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.770677 lager-cli-0.1.99/
+-rw-r--r--   0 ehaas      (501) staff       (20)    33886 2020-10-17 16:52:22.000000 lager-cli-0.1.99/LICENSE
+-rw-r--r--   0 ehaas      (501) staff       (20)      853 2021-09-07 18:14:37.770114 lager-cli-0.1.99/PKG-INFO
+-rw-r--r--   0 ehaas      (501) staff       (20)      126 2020-10-16 03:32:31.000000 lager-cli-0.1.99/README.md
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.700779 lager-cli-0.1.99/lager_cli/
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.706853 lager-cli-0.1.99/lager_cli/PyCRC/
+-rw-r--r--   0 ehaas      (501) staff       (20)     1679 2021-08-20 19:34:40.000000 lager-cli-0.1.99/lager_cli/PyCRC/CRC16.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     1903 2021-08-20 19:34:40.000000 lager-cli-0.1.99/lager_cli/PyCRC/CRC16DNP.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     1890 2021-08-20 19:34:40.000000 lager-cli-0.1.99/lager_cli/PyCRC/CRC16Kermit.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     1794 2021-08-20 19:34:40.000000 lager-cli-0.1.99/lager_cli/PyCRC/CRC16SICK.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     1704 2021-08-20 19:34:40.000000 lager-cli-0.1.99/lager_cli/PyCRC/CRC32.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     2267 2021-08-20 19:34:40.000000 lager-cli-0.1.99/lager_cli/PyCRC/CRCCCITT.py
+-rwxr-xr-x   0 ehaas      (501) staff       (20)      123 2021-08-20 19:34:40.000000 lager-cli-0.1.99/lager_cli/PyCRC/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)      956 2021-09-07 18:14:19.000000 lager-cli-0.1.99/lager_cli/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)      150 2020-07-01 20:32:58.000000 lager-cli-0.1.99/lager_cli/__main__.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.707641 lager-cli-0.1.99/lager_cli/adc/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-12-01 22:44:05.000000 lager-cli-0.1.99/lager_cli/adc/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     1977 2020-12-21 17:50:11.000000 lager-cli-0.1.99/lager_cli/adc/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.708680 lager-cli-0.1.99/lager_cli/auth/
+-rw-r--r--   0 ehaas      (501) staff       (20)     3122 2021-01-12 18:34:44.000000 lager-cli-0.1.99/lager_cli/auth/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     3486 2020-08-21 19:02:41.000000 lager-cli-0.1.99/lager_cli/auth/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.709656 lager-cli-0.1.99/lager_cli/ble/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2021-03-09 18:05:12.000000 lager-cli-0.1.99/lager_cli/ble/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     2619 2021-04-22 22:14:22.000000 lager-cli-0.1.99/lager_cli/ble/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.717586 lager-cli-0.1.99/lager_cli/canbus/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-10-21 16:03:40.000000 lager-cli-0.1.99/lager_cli/canbus/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     5626 2021-04-14 22:10:26.000000 lager-cli-0.1.99/lager_cli/canbus/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.719007 lager-cli-0.1.99/lager_cli/chip_erase/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2021-06-14 17:50:49.000000 lager-cli-0.1.99/lager_cli/chip_erase/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     1153 2021-06-15 15:24:50.000000 lager-cli-0.1.99/lager_cli/chip_erase/commands.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     4405 2021-07-08 22:17:50.000000 lager-cli-0.1.99/lager_cli/cli.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     3358 2020-10-16 16:54:45.000000 lager-cli-0.1.99/lager_cli/config.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.720411 lager-cli-0.1.99/lager_cli/connect/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-07-09 18:58:17.000000 lager-cli-0.1.99/lager_cli/connect/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     4333 2021-06-15 15:26:22.000000 lager-cli-0.1.99/lager_cli/connect/commands.py
+-rw-r--r--   0 ehaas      (501) staff       (20)    21547 2021-07-21 20:23:44.000000 lager-cli-0.1.99/lager_cli/context.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.721831 lager-cli-0.1.99/lager_cli/devenv/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-06-30 23:18:40.000000 lager-cli-0.1.99/lager_cli/devenv/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     5498 2021-07-16 20:31:17.000000 lager-cli-0.1.99/lager_cli/devenv/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.723200 lager-cli-0.1.99/lager_cli/erase/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-06-30 23:18:40.000000 lager-cli-0.1.99/lager_cli/erase/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)      752 2020-07-21 18:37:02.000000 lager-cli-0.1.99/lager_cli/erase/commands.py
+-rw-r--r--   0 ehaas      (501) staff       (20)      103 2020-10-01 23:32:31.000000 lager-cli-0.1.99/lager_cli/exceptions.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.724627 lager-cli-0.1.99/lager_cli/exec/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-06-30 23:18:40.000000 lager-cli-0.1.99/lager_cli/exec/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     6093 2021-07-08 20:58:22.000000 lager-cli-0.1.99/lager_cli/exec/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.726053 lager-cli-0.1.99/lager_cli/flash/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-06-30 23:18:40.000000 lager-cli-0.1.99/lager_cli/flash/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     2129 2021-04-09 03:35:22.000000 lager-cli-0.1.99/lager_cli/flash/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.727419 lager-cli-0.1.99/lager_cli/gateway/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-04-30 16:59:17.000000 lager-cli-0.1.99/lager_cli/gateway/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     5506 2021-01-29 00:36:06.000000 lager-cli-0.1.99/lager_cli/gateway/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.751590 lager-cli-0.1.99/lager_cli/gdbserver/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-07-09 17:46:44.000000 lager-cli-0.1.99/lager_cli/gdbserver/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     3233 2021-03-10 19:51:16.000000 lager-cli-0.1.99/lager_cli/gdbserver/commands.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     6455 2021-04-14 19:23:12.000000 lager-cli-0.1.99/lager_cli/gdbserver/tunnel.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.752745 lager-cli-0.1.99/lager_cli/gpio/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-08-12 21:54:20.000000 lager-cli-0.1.99/lager_cli/gpio/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     3582 2021-06-16 20:17:12.000000 lager-cli-0.1.99/lager_cli/gpio/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.753593 lager-cli-0.1.99/lager_cli/grafana/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2021-04-27 19:37:07.000000 lager-cli-0.1.99/lager_cli/grafana/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     1476 2021-04-27 19:38:29.000000 lager-cli-0.1.99/lager_cli/grafana/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.754738 lager-cli-0.1.99/lager_cli/i2c/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2021-03-11 23:33:10.000000 lager-cli-0.1.99/lager_cli/i2c/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     6789 2021-03-17 23:14:11.000000 lager-cli-0.1.99/lager_cli/i2c/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.755834 lager-cli-0.1.99/lager_cli/job/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-05-22 20:02:14.000000 lager-cli-0.1.99/lager_cli/job/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     1071 2020-10-28 21:50:47.000000 lager-cli-0.1.99/lager_cli/job/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.756769 lager-cli-0.1.99/lager_cli/lister/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-05-05 19:15:34.000000 lager-cli-0.1.99/lager_cli/lister/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     1145 2020-08-26 21:56:57.000000 lager-cli-0.1.99/lager_cli/lister/commands.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     6146 2021-08-20 22:11:40.000000 lager-cli-0.1.99/lager_cli/matchers.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.757874 lager-cli-0.1.99/lager_cli/openocd/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-09-10 21:09:47.000000 lager-cli-0.1.99/lager_cli/openocd/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     1815 2020-09-10 21:20:46.000000 lager-cli-0.1.99/lager_cli/openocd/commands.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     9300 2021-03-12 23:18:29.000000 lager-cli-0.1.99/lager_cli/paramtypes.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.759069 lager-cli-0.1.99/lager_cli/pigpio/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2021-03-10 19:46:50.000000 lager-cli-0.1.99/lager_cli/pigpio/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     1490 2021-03-10 19:46:50.000000 lager-cli-0.1.99/lager_cli/pigpio/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.760130 lager-cli-0.1.99/lager_cli/pip/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2021-07-08 22:15:46.000000 lager-cli-0.1.99/lager_cli/pip/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     1843 2021-07-08 23:11:00.000000 lager-cli-0.1.99/lager_cli/pip/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.760893 lager-cli-0.1.99/lager_cli/python/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-09-10 22:40:41.000000 lager-cli-0.1.99/lager_cli/python/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     8476 2021-07-12 16:42:49.000000 lager-cli-0.1.99/lager_cli/python/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.762023 lager-cli-0.1.99/lager_cli/reset/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-06-30 23:18:40.000000 lager-cli-0.1.99/lager_cli/reset/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)      829 2020-07-21 18:53:46.000000 lager-cli-0.1.99/lager_cli/reset/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.762942 lager-cli-0.1.99/lager_cli/run/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-06-30 23:18:40.000000 lager-cli-0.1.99/lager_cli/run/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)      561 2020-07-21 18:54:17.000000 lager-cli-0.1.99/lager_cli/run/commands.py
+-rw-r--r--   0 ehaas      (501) staff       (20)      951 2020-10-01 23:24:49.000000 lager-cli-0.1.99/lager_cli/safe_unpickle.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.763848 lager-cli-0.1.99/lager_cli/serial_ports/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-11-03 18:15:25.000000 lager-cli-0.1.99/lager_cli/serial_ports/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     1090 2020-11-03 18:19:53.000000 lager-cli-0.1.99/lager_cli/serial_ports/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.764775 lager-cli-0.1.99/lager_cli/setter/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-05-05 21:50:01.000000 lager-cli-0.1.99/lager_cli/setter/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)      785 2020-07-01 17:04:51.000000 lager-cli-0.1.99/lager_cli/setter/commands.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     5576 2021-08-20 21:56:41.000000 lager-cli-0.1.99/lager_cli/simple_hdlc.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.765706 lager-cli-0.1.99/lager_cli/spi/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2021-03-11 23:33:03.000000 lager-cli-0.1.99/lager_cli/spi/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)    11229 2021-03-17 23:14:11.000000 lager-cli-0.1.99/lager_cli/spi/commands.py
+-rw-r--r--   0 ehaas      (501) staff       (20)    12256 2021-08-20 22:11:40.000000 lager-cli-0.1.99/lager_cli/status.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.766676 lager-cli-0.1.99/lager_cli/testrun/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-07-07 18:11:15.000000 lager-cli-0.1.99/lager_cli/testrun/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     4102 2021-04-14 22:08:40.000000 lager-cli-0.1.99/lager_cli/testrun/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.767462 lager-cli-0.1.99/lager_cli/uart/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-06-29 23:01:20.000000 lager-cli-0.1.99/lager_cli/uart/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     4789 2021-08-20 21:56:41.000000 lager-cli-0.1.99/lager_cli/uart/commands.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     7146 2020-11-02 17:37:15.000000 lager-cli-0.1.99/lager_cli/util.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.768152 lager-cli-0.1.99/lager_cli/webcam/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2021-02-03 04:05:31.000000 lager-cli-0.1.99/lager_cli/webcam/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     1492 2021-02-03 06:52:54.000000 lager-cli-0.1.99/lager_cli/webcam/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.769272 lager-cli-0.1.99/lager_cli/wifi/
+-rw-r--r--   0 ehaas      (501) staff       (20)        0 2020-09-27 22:31:49.000000 lager-cli-0.1.99/lager_cli/wifi/__init__.py
+-rw-r--r--   0 ehaas      (501) staff       (20)     3156 2021-03-15 15:57:15.000000 lager-cli-0.1.99/lager_cli/wifi/commands.py
+drwxr-xr-x   0 ehaas      (501) staff       (20)        0 2021-09-07 18:14:37.703925 lager-cli-0.1.99/lager_cli.egg-info/
+-rw-r--r--   0 ehaas      (501) staff       (20)      853 2021-09-07 18:14:36.000000 lager-cli-0.1.99/lager_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ehaas      (501) staff       (20)     2420 2021-09-07 18:14:37.000000 lager-cli-0.1.99/lager_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ehaas      (501) staff       (20)        1 2021-09-07 18:14:36.000000 lager-cli-0.1.99/lager_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ehaas      (501) staff       (20)       45 2021-09-07 18:14:36.000000 lager-cli-0.1.99/lager_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ehaas      (501) staff       (20)      434 2021-09-07 18:14:36.000000 lager-cli-0.1.99/lager_cli.egg-info/requires.txt
+-rw-r--r--   0 ehaas      (501) staff       (20)       10 2021-09-07 18:14:37.000000 lager-cli-0.1.99/lager_cli.egg-info/top_level.txt
+-rw-r--r--   0 ehaas      (501) staff       (20)       38 2021-09-07 18:14:37.770857 lager-cli-0.1.99/setup.cfg
+-rw-r--r--   0 ehaas      (501) staff       (20)     2134 2021-09-07 18:13:57.000000 lager-cli-0.1.99/setup.py
```

### Comparing `lager-cli-0.1.98/LICENSE` & `lager-cli-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/PKG-INFO` & `lager-cli-0.1.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lager-cli
-Version: 0.1.98
+Version: 0.1.99
 Summary: Lager Command Line Interface
 Home-page: https://github.com/lagerdata/lager-cli
 Author: Lager Data LLC
 Author-email: hello@lagerdata.com
 Maintainer: Lager Data LLC
 Maintainer-email: hello@lagerdata.com
 License: AGPLv3
```

### Comparing `lager-cli-0.1.98/lager_cli/PyCRC/CRC16.py` & `lager-cli-0.1.99/lager_cli/PyCRC/CRC16.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/PyCRC/CRC16DNP.py` & `lager-cli-0.1.99/lager_cli/PyCRC/CRC16DNP.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/PyCRC/CRC16Kermit.py` & `lager-cli-0.1.99/lager_cli/PyCRC/CRC16Kermit.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/PyCRC/CRC16SICK.py` & `lager-cli-0.1.99/lager_cli/PyCRC/CRC16SICK.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/PyCRC/CRC32.py` & `lager-cli-0.1.99/lager_cli/PyCRC/CRC32.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/PyCRC/CRCCCITT.py` & `lager-cli-0.1.99/lager_cli/PyCRC/CRCCCITT.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/__init__.py` & `lager-cli-0.1.99/lager_cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Lager CLI
 ----
 A Command Line Interface for Lager Data
 """
 
-__version__ = '0.1.98'
+__version__ = '0.1.99'
 
 SUPPORTED_DEVICES = (
     'at91samdexx',
     'at91samdgxx',
     'at91samdxx',
     'atsame70',
     'cc3220s',
```

### Comparing `lager-cli-0.1.98/lager_cli/adc/commands.py` & `lager-cli-0.1.99/lager_cli/adc/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/auth/__init__.py` & `lager-cli-0.1.99/lager_cli/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/auth/commands.py` & `lager-cli-0.1.99/lager_cli/auth/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/ble/commands.py` & `lager-cli-0.1.99/lager_cli/ble/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/canbus/commands.py` & `lager-cli-0.1.99/lager_cli/canbus/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/chip_erase/commands.py` & `lager-cli-0.1.99/lager_cli/chip_erase/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/cli.py` & `lager-cli-0.1.99/lager_cli/cli.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/config.py` & `lager-cli-0.1.99/lager_cli/config.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/connect/commands.py` & `lager-cli-0.1.99/lager_cli/connect/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/context.py` & `lager-cli-0.1.99/lager_cli/context.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/devenv/commands.py` & `lager-cli-0.1.99/lager_cli/devenv/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/erase/commands.py` & `lager-cli-0.1.99/lager_cli/erase/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/exec/commands.py` & `lager-cli-0.1.99/lager_cli/exec/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/flash/commands.py` & `lager-cli-0.1.99/lager_cli/flash/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/gateway/commands.py` & `lager-cli-0.1.99/lager_cli/gateway/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/gdbserver/commands.py` & `lager-cli-0.1.99/lager_cli/gdbserver/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/gdbserver/tunnel.py` & `lager-cli-0.1.99/lager_cli/gdbserver/tunnel.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/gpio/commands.py` & `lager-cli-0.1.99/lager_cli/gpio/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/grafana/commands.py` & `lager-cli-0.1.99/lager_cli/grafana/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/i2c/commands.py` & `lager-cli-0.1.99/lager_cli/i2c/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/job/commands.py` & `lager-cli-0.1.99/lager_cli/job/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/lister/commands.py` & `lager-cli-0.1.99/lager_cli/lister/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/matchers.py` & `lager-cli-0.1.99/lager_cli/matchers.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/openocd/commands.py` & `lager-cli-0.1.99/lager_cli/openocd/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/paramtypes.py` & `lager-cli-0.1.99/lager_cli/paramtypes.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/pigpio/commands.py` & `lager-cli-0.1.99/lager_cli/pigpio/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/pip/commands.py` & `lager-cli-0.1.99/lager_cli/pip/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/python/commands.py` & `lager-cli-0.1.99/lager_cli/python/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/reset/commands.py` & `lager-cli-0.1.99/lager_cli/reset/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/run/commands.py` & `lager-cli-0.1.99/lager_cli/run/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/safe_unpickle.py` & `lager-cli-0.1.99/lager_cli/safe_unpickle.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/serial_ports/commands.py` & `lager-cli-0.1.99/lager_cli/serial_ports/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/setter/commands.py` & `lager-cli-0.1.99/lager_cli/setter/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/simple_hdlc.py` & `lager-cli-0.1.99/lager_cli/simple_hdlc.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/spi/commands.py` & `lager-cli-0.1.99/lager_cli/spi/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/status.py` & `lager-cli-0.1.99/lager_cli/status.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/testrun/commands.py` & `lager-cli-0.1.99/lager_cli/testrun/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/uart/commands.py` & `lager-cli-0.1.99/lager_cli/uart/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/util.py` & `lager-cli-0.1.99/lager_cli/util.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/webcam/commands.py` & `lager-cli-0.1.99/lager_cli/webcam/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli/wifi/commands.py` & `lager-cli-0.1.99/lager_cli/wifi/commands.py`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/lager_cli.egg-info/PKG-INFO` & `lager-cli-0.1.99/lager_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lager-cli
-Version: 0.1.98
+Version: 0.1.99
 Summary: Lager Command Line Interface
 Home-page: https://github.com/lagerdata/lager-cli
 Author: Lager Data LLC
 Author-email: hello@lagerdata.com
 Maintainer: Lager Data LLC
 Maintainer-email: hello@lagerdata.com
 License: AGPLv3
```

### Comparing `lager-cli-0.1.98/lager_cli.egg-info/SOURCES.txt` & `lager-cli-0.1.99/lager_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lager-cli-0.1.98/setup.py` & `lager-cli-0.1.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,31 +42,31 @@
             async-generator == 1.10
             bson == 0.5.10
             certifi == 2020.6.20
             chardet == 3.0.4
             click == 7.1.2
             colorama == 0.4.3
             h11 == 0.9.0
-            idna == 2.9
+            idna == 2.10
             ipaddress == 1.0.23
             multidict == 4.7.6
             outcome == 1.0.1
             pigpio == 1.78
             python-dateutil == 2.8.1
             PyYAML == 5.4
-            requests == 2.23.0
+            requests == 2.24.0
             requests-toolbelt == 0.9.1
             six == 1.15.0
             sniffio == 1.1.0
             sortedcontainers == 2.2.2
             tenacity == 6.2.0
             texttable == 1.6.2
             trio == 0.16.0
             lager-trio-websocket == 0.9.0-dev
-            urllib3 == 1.25.9
+            urllib3 == 1.25.10
             wsproto == 0.14.1
             yarl == 1.4.2
         ''',
         entry_points={
             'console_scripts': [
                 'lager=lager_cli.cli:cli',
             ],
```

