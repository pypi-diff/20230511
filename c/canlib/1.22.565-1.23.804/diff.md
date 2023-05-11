# Comparing `tmp/canlib-1.22.565.tar.gz` & `tmp/canlib-1.23.804.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\Data\220908~2\pycanlib\DEFAUL~2\src\dist\tmpctk6w1id\canlib-1.22.565.tar", last modified: Thu Sep  8 20:46:04 2022, max compression
+gzip compressed data, was "D:\build\Data\230505~2\pycanlib\DEFAUL~2\src\dist\.tmp-m0l1p9lt\canlib-1.23.804.tar", last modified: Fri May  5 19:32:19 2023, max compression
```

## Comparing `canlib-1.22.565.tar` & `canlib-1.23.804.tar`

### file list

```diff
@@ -1,121 +1,129 @@
-drwxrwxrwx   0        0        0        0 2022-09-08 20:46:04.000000 canlib-1.22.565/
--rw-rw-rw-   0        0        0     1068 2022-09-08 20:43:58.000000 canlib-1.22.565/LICENSE
--rw-rw-rw-   0        0        0       59 2022-09-08 20:43:58.000000 canlib-1.22.565/MANIFEST.in
--rw-rw-rw-   0        0        0     7536 2022-09-08 20:46:04.000000 canlib-1.22.565/PKG-INFO
--rw-rw-rw-   0        0        0     6792 2022-09-08 20:43:58.000000 canlib-1.22.565/README.rst
--rw-rw-rw-   0        0        0    25288 2022-09-08 20:44:05.000000 canlib-1.22.565/Relnotes.rst
-drwxrwxrwx   0        0        0        0 2022-09-08 20:46:04.000000 canlib-1.22.565/canlib/
--rw-rw-rw-   0        0        0      385 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/__about__.py
--rw-rw-rw-   0        0        0      221 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/__init__.py
--rw-rw-rw-   0        0        0       26 2022-09-08 20:44:05.000000 canlib-1.22.565/canlib/__version__.py
-drwxrwxrwx   0        0        0        0 2022-09-08 20:46:04.000000 canlib-1.22.565/canlib/canlib/
--rw-rw-rw-   0        0        0     2427 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/canlib/__init__.py
--rw-rw-rw-   0        0        0      725 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/canlib/_channel.py
--rw-rw-rw-   0        0        0    22718 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/canlib/busparams.py
--rw-rw-rw-   0        0        0    60559 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/canlib/channel.py
--rw-rw-rw-   0        0        0    18151 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/canlib/channeldata.py
--rw-rw-rw-   0        0        0    10771 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/canlib/constants.py
--rw-rw-rw-   0        0        0     9063 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/canlib/dll.py
--rw-rw-rw-   0        0        0    30453 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/canlib/enums.py
--rw-rw-rw-   0        0        0     6531 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/canlib/envvar.py
--rw-rw-rw-   0        0        0     5906 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/canlib/exceptions.py
--rw-rw-rw-   0        0        0    15796 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/canlib/iocontrol.py
--rw-rw-rw-   0        0        0    22000 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/canlib/iopin.py
--rw-rw-rw-   0        0        0     6796 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/canlib/objbuf.py
--rw-rw-rw-   0        0        0     3068 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/canlib/structures.py
--rw-rw-rw-   0        0        0     4932 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/canlib/txe.py
--rw-rw-rw-   0        0        0    15687 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/canlib/wrapper.py
--rw-rw-rw-   0        0        0      360 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/cenum.py
--rw-rw-rw-   0        0        0     7805 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/deprecation.py
--rw-rw-rw-   0        0        0    16036 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/device.py
--rw-rw-rw-   0        0        0     8974 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/dllLoader.py
--rw-rw-rw-   0        0        0     7583 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/ean.py
--rw-rw-rw-   0        0        0      760 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/exceptions.py
--rw-rw-rw-   0        0        0     4003 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/frame.py
--rw-rw-rw-   0        0        0     8738 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/futureapi.py
--rw-rw-rw-   0        0        0     5195 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/j1939.py
--rw-rw-rw-   0        0        0    12275 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvDevice.py
--rw-rw-rw-   0        0        0    25506 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvMemoConfig.py
--rw-rw-rw-   0        0        0      115 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvMessage.py
--rw-rw-rw-   0        0        0      247 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvaMemoLibXml.py
-drwxrwxrwx   0        0        0        0 2022-09-08 20:46:04.000000 canlib-1.22.565/canlib/kvadblib/
--rw-rw-rw-   0        0        0     1517 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvadblib/__init__.py
--rw-rw-rw-   0        0        0     3498 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvadblib/attribute.py
--rw-rw-rw-   0        0        0     8276 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvadblib/attributedef.py
--rw-rw-rw-   0        0        0     1189 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvadblib/bound_message.py
--rw-rw-rw-   0        0        0     2099 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvadblib/bound_signal.py
--rw-rw-rw-   0        0        0       11 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvadblib/constants.py
--rw-rw-rw-   0        0        0    18943 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvadblib/dbc.py
--rw-rw-rw-   0        0        0    11330 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvadblib/dll.py
--rw-rw-rw-   0        0        0     2611 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvadblib/enums.py
--rw-rw-rw-   0        0        0     3130 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvadblib/exceptions.py
--rw-rw-rw-   0        0        0     3530 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvadblib/framebox.py
--rw-rw-rw-   0        0        0    12525 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvadblib/message.py
--rw-rw-rw-   0        0        0     4207 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvadblib/node.py
--rw-rw-rw-   0        0        0    15148 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvadblib/signal.py
--rw-rw-rw-   0        0        0     2326 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvadblib/wrapper.py
-drwxrwxrwx   0        0        0        0 2022-09-08 20:46:04.000000 canlib-1.22.565/canlib/kvamemolibxml/
--rw-rw-rw-   0        0        0     1441 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvamemolibxml/__init__.py
--rw-rw-rw-   0        0        0     4778 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvamemolibxml/configuration.py
--rw-rw-rw-   0        0        0       85 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvamemolibxml/constants.py
--rw-rw-rw-   0        0        0     1587 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvamemolibxml/dll.py
--rw-rw-rw-   0        0        0     3864 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvamemolibxml/enums.py
--rw-rw-rw-   0        0        0     1995 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvamemolibxml/exceptions.py
--rw-rw-rw-   0        0        0     7078 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvamemolibxml/wrapper.py
-drwxrwxrwx   0        0        0        0 2022-09-08 20:46:04.000000 canlib-1.22.565/canlib/kvlclib/
--rw-rw-rw-   0        0        0      761 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvlclib/__init__.py
--rw-rw-rw-   0        0        0     2182 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvlclib/constants.py
--rw-rw-rw-   0        0        0    11729 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvlclib/converter.py
--rw-rw-rw-   0        0        0     4464 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvlclib/deprecated.py
--rw-rw-rw-   0        0        0     3277 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvlclib/dll.py
--rw-rw-rw-   0        0        0     3242 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvlclib/enums.py
--rw-rw-rw-   0        0        0     2333 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvlclib/exceptions.py
--rw-rw-rw-   0        0        0     4745 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvlclib/properties.py
--rw-rw-rw-   0        0        0     3696 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvlclib/readerformat.py
--rw-rw-rw-   0        0        0      766 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvlclib/wrapper.py
--rw-rw-rw-   0        0        0     4390 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvlclib/writerformat.py
-drwxrwxrwx   0        0        0        0 2022-09-08 20:46:04.000000 canlib-1.22.565/canlib/kvmlib/
--rw-rw-rw-   0        0        0     1579 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvmlib/__init__.py
--rw-rw-rw-   0        0        0     2123 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvmlib/constants.py
--rw-rw-rw-   0        0        0    15889 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvmlib/deprecated.py
--rw-rw-rw-   0        0        0     5307 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvmlib/dll.py
--rw-rw-rw-   0        0        0     3429 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvmlib/enums.py
--rw-rw-rw-   0        0        0    16016 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvmlib/events.py
--rw-rw-rw-   0        0        0     2607 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvmlib/exceptions.py
--rw-rw-rw-   0        0        0     6624 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvmlib/kme.py
--rw-rw-rw-   0        0        0     3196 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvmlib/kmf.py
--rw-rw-rw-   0        0        0     3501 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvmlib/log.py
--rw-rw-rw-   0        0        0     4657 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvmlib/logfile.py
--rw-rw-rw-   0        0        0    10133 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvmlib/memorator.py
--rw-rw-rw-   0        0        0      396 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvmlib/messages.py
--rw-rw-rw-   0        0        0      547 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvmlib/wrapper.py
-drwxrwxrwx   0        0        0        0 2022-09-08 20:46:04.000000 canlib-1.22.565/canlib/kvrlib/
--rw-rw-rw-   0        0        0     2506 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvrlib/__init__.py
--rw-rw-rw-   0        0        0     1886 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvrlib/address.py
--rw-rw-rw-   0        0        0     4565 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvrlib/constants.py
--rw-rw-rw-   0        0        0    14748 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvrlib/discovery.py
--rw-rw-rw-   0        0        0     6340 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvrlib/dll.py
--rw-rw-rw-   0        0        0     6646 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvrlib/enums.py
--rw-rw-rw-   0        0        0     1971 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvrlib/exceptions.py
--rw-rw-rw-   0        0        0     7016 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvrlib/infoset.py
--rw-rw-rw-   0        0        0    23169 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvrlib/remotedevice.py
--rw-rw-rw-   0        0        0      923 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvrlib/service.py
--rw-rw-rw-   0        0        0     5172 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvrlib/structures.py
--rw-rw-rw-   0        0        0    13293 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/kvrlib/wrapper.py
-drwxrwxrwx   0        0        0        0 2022-09-08 20:46:04.000000 canlib-1.22.565/canlib/linlib/
--rw-rw-rw-   0        0        0      538 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/linlib/__init__.py
--rw-rw-rw-   0        0        0    15071 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/linlib/channel.py
--rw-rw-rw-   0        0        0     3148 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/linlib/dll.py
--rw-rw-rw-   0        0        0     3799 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/linlib/enums.py
--rw-rw-rw-   0        0        0     2928 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/linlib/exceptions.py
--rw-rw-rw-   0        0        0     2721 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/linlib/structures.py
--rw-rw-rw-   0        0        0     4607 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/linlib/wrapper.py
--rw-rw-rw-   0        0        0     3509 2022-09-08 20:43:58.000000 canlib-1.22.565/canlib/versionnumber.py
-drwxrwxrwx   0        0        0        0 2022-09-08 20:46:04.000000 canlib-1.22.565/canlib.egg-info/
--rw-rw-rw-   0        0        0     7536 2022-09-08 20:46:04.000000 canlib-1.22.565/canlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2717 2022-09-08 20:46:04.000000 canlib-1.22.565/canlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-08 20:46:04.000000 canlib-1.22.565/canlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2022-09-08 20:46:04.000000 canlib-1.22.565/canlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-09-08 20:46:04.000000 canlib-1.22.565/canlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-08 20:46:04.000000 canlib-1.22.565/setup.cfg
--rw-rw-rw-   0        0        0     2381 2022-09-08 20:43:58.000000 canlib-1.22.565/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:32:19.000000 canlib-1.23.804/
+-rw-rw-rw-   0        0        0     1068 2023-05-05 19:30:12.000000 canlib-1.23.804/LICENSE
+-rw-rw-rw-   0        0        0       59 2023-05-05 19:30:12.000000 canlib-1.23.804/MANIFEST.in
+-rw-rw-rw-   0        0        0     7536 2023-05-05 19:32:19.000000 canlib-1.23.804/PKG-INFO
+-rw-rw-rw-   0        0        0     6792 2023-05-05 19:30:12.000000 canlib-1.23.804/README.rst
+-rw-rw-rw-   0        0        0    25511 2023-05-05 19:30:15.000000 canlib-1.23.804/Relnotes.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 19:32:19.000000 canlib-1.23.804/canlib/
+-rw-rw-rw-   0        0        0      385 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/__about__.py
+-rw-rw-rw-   0        0        0      221 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/__init__.py
+-rw-rw-rw-   0        0        0       26 2023-05-05 19:30:14.000000 canlib-1.23.804/canlib/__version__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:32:19.000000 canlib-1.23.804/canlib/canlib/
+-rw-rw-rw-   0        0        0     2477 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/canlib/__init__.py
+-rw-rw-rw-   0        0        0      725 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/canlib/_channel.py
+-rw-rw-rw-   0        0        0    22718 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/canlib/busparams.py
+-rw-rw-rw-   0        0        0    60559 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/canlib/channel.py
+-rw-rw-rw-   0        0        0    18151 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/canlib/channeldata.py
+-rw-rw-rw-   0        0        0    10771 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/canlib/constants.py
+-rw-rw-rw-   0        0        0     9455 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/canlib/dll.py
+-rw-rw-rw-   0        0        0    30453 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/canlib/enums.py
+-rw-rw-rw-   0        0        0     6531 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/canlib/envvar.py
+-rw-rw-rw-   0        0        0     5906 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/canlib/exceptions.py
+-rw-rw-rw-   0        0        0    15796 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/canlib/iocontrol.py
+-rw-rw-rw-   0        0        0    22000 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/canlib/iopin.py
+-rw-rw-rw-   0        0        0     6796 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/canlib/objbuf.py
+-rw-rw-rw-   0        0        0     3305 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/canlib/structures.py
+-rw-rw-rw-   0        0        0     2935 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/canlib/timedomain.py
+-rw-rw-rw-   0        0        0     4932 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/canlib/txe.py
+-rw-rw-rw-   0        0        0    15687 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/canlib/wrapper.py
+-rw-rw-rw-   0        0        0      360 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/cenum.py
+-rw-rw-rw-   0        0        0     7805 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/deprecation.py
+-rw-rw-rw-   0        0        0    16036 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/device.py
+-rw-rw-rw-   0        0        0     8974 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/dllLoader.py
+-rw-rw-rw-   0        0        0     7583 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/ean.py
+-rw-rw-rw-   0        0        0      760 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/exceptions.py
+-rw-rw-rw-   0        0        0     4003 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/frame.py
+-rw-rw-rw-   0        0        0     8738 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/futureapi.py
+-rw-rw-rw-   0        0        0     5195 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/j1939.py
+-rw-rw-rw-   0        0        0    12275 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvDevice.py
+-rw-rw-rw-   0        0        0    25506 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvMemoConfig.py
+-rw-rw-rw-   0        0        0      115 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvMessage.py
+-rw-rw-rw-   0        0        0      247 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvaMemoLibXml.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:32:19.000000 canlib-1.23.804/canlib/kvadblib/
+-rw-rw-rw-   0        0        0     1517 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvadblib/__init__.py
+-rw-rw-rw-   0        0        0     3498 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvadblib/attribute.py
+-rw-rw-rw-   0        0        0     8276 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvadblib/attributedef.py
+-rw-rw-rw-   0        0        0     1189 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvadblib/bound_message.py
+-rw-rw-rw-   0        0        0     2099 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvadblib/bound_signal.py
+-rw-rw-rw-   0        0        0       11 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvadblib/constants.py
+-rw-rw-rw-   0        0        0    18943 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvadblib/dbc.py
+-rw-rw-rw-   0        0        0    11330 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvadblib/dll.py
+-rw-rw-rw-   0        0        0     2611 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvadblib/enums.py
+-rw-rw-rw-   0        0        0     3130 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvadblib/exceptions.py
+-rw-rw-rw-   0        0        0     3530 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvadblib/framebox.py
+-rw-rw-rw-   0        0        0    12525 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvadblib/message.py
+-rw-rw-rw-   0        0        0     4207 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvadblib/node.py
+-rw-rw-rw-   0        0        0    15148 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvadblib/signal.py
+-rw-rw-rw-   0        0        0     2326 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvadblib/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:32:19.000000 canlib-1.23.804/canlib/kvamemolibxml/
+-rw-rw-rw-   0        0        0     1441 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvamemolibxml/__init__.py
+-rw-rw-rw-   0        0        0     4778 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvamemolibxml/configuration.py
+-rw-rw-rw-   0        0        0       85 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvamemolibxml/constants.py
+-rw-rw-rw-   0        0        0     1587 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvamemolibxml/dll.py
+-rw-rw-rw-   0        0        0     3864 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvamemolibxml/enums.py
+-rw-rw-rw-   0        0        0     1995 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvamemolibxml/exceptions.py
+-rw-rw-rw-   0        0        0     7078 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvamemolibxml/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:32:19.000000 canlib-1.23.804/canlib/kvlclib/
+-rw-rw-rw-   0        0        0      761 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvlclib/__init__.py
+-rw-rw-rw-   0        0        0     2182 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvlclib/constants.py
+-rw-rw-rw-   0        0        0    11729 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvlclib/converter.py
+-rw-rw-rw-   0        0        0     4464 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvlclib/deprecated.py
+-rw-rw-rw-   0        0        0     3277 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvlclib/dll.py
+-rw-rw-rw-   0        0        0     3242 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvlclib/enums.py
+-rw-rw-rw-   0        0        0     2333 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvlclib/exceptions.py
+-rw-rw-rw-   0        0        0     4745 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvlclib/properties.py
+-rw-rw-rw-   0        0        0     3696 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvlclib/readerformat.py
+-rw-rw-rw-   0        0        0      766 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvlclib/wrapper.py
+-rw-rw-rw-   0        0        0     4390 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvlclib/writerformat.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:32:19.000000 canlib-1.23.804/canlib/kvmlib/
+-rw-rw-rw-   0        0        0     1579 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvmlib/__init__.py
+-rw-rw-rw-   0        0        0     2123 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvmlib/constants.py
+-rw-rw-rw-   0        0        0    15889 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvmlib/deprecated.py
+-rw-rw-rw-   0        0        0     5307 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvmlib/dll.py
+-rw-rw-rw-   0        0        0     3429 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvmlib/enums.py
+-rw-rw-rw-   0        0        0    16016 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvmlib/events.py
+-rw-rw-rw-   0        0        0     2607 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvmlib/exceptions.py
+-rw-rw-rw-   0        0        0     6624 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvmlib/kme.py
+-rw-rw-rw-   0        0        0     3196 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvmlib/kmf.py
+-rw-rw-rw-   0        0        0     3501 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvmlib/log.py
+-rw-rw-rw-   0        0        0     4657 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvmlib/logfile.py
+-rw-rw-rw-   0        0        0    10133 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvmlib/memorator.py
+-rw-rw-rw-   0        0        0      396 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvmlib/messages.py
+-rw-rw-rw-   0        0        0      547 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvmlib/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:32:19.000000 canlib-1.23.804/canlib/kvrlib/
+-rw-rw-rw-   0        0        0     2506 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvrlib/__init__.py
+-rw-rw-rw-   0        0        0     1886 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvrlib/address.py
+-rw-rw-rw-   0        0        0     4565 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvrlib/constants.py
+-rw-rw-rw-   0        0        0    14748 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvrlib/discovery.py
+-rw-rw-rw-   0        0        0     6340 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvrlib/dll.py
+-rw-rw-rw-   0        0        0     6646 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvrlib/enums.py
+-rw-rw-rw-   0        0        0     1971 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvrlib/exceptions.py
+-rw-rw-rw-   0        0        0     7016 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvrlib/infoset.py
+-rw-rw-rw-   0        0        0    23169 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvrlib/remotedevice.py
+-rw-rw-rw-   0        0        0      923 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvrlib/service.py
+-rw-rw-rw-   0        0        0     5172 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvrlib/structures.py
+-rw-rw-rw-   0        0        0    13293 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/kvrlib/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:32:19.000000 canlib-1.23.804/canlib/linlib/
+-rw-rw-rw-   0        0        0      538 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/linlib/__init__.py
+-rw-rw-rw-   0        0        0    15071 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/linlib/channel.py
+-rw-rw-rw-   0        0        0     3148 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/linlib/dll.py
+-rw-rw-rw-   0        0        0     3799 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/linlib/enums.py
+-rw-rw-rw-   0        0        0     2928 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/linlib/exceptions.py
+-rw-rw-rw-   0        0        0     2721 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/linlib/structures.py
+-rw-rw-rw-   0        0        0     4607 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/linlib/wrapper.py
+-rw-rw-rw-   0        0        0     3509 2023-05-05 19:30:12.000000 canlib-1.23.804/canlib/versionnumber.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:32:19.000000 canlib-1.23.804/canlib.egg-info/
+-rw-rw-rw-   0        0        0     7536 2023-05-05 19:32:19.000000 canlib-1.23.804/canlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2882 2023-05-05 19:32:19.000000 canlib-1.23.804/canlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 19:32:19.000000 canlib-1.23.804/canlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2023-05-05 19:32:19.000000 canlib-1.23.804/canlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 19:32:19.000000 canlib-1.23.804/canlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 19:32:19.000000 canlib-1.23.804/setup.cfg
+-rw-rw-rw-   0        0        0     2381 2023-05-05 19:30:12.000000 canlib-1.23.804/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:32:19.000000 canlib-1.23.804/tests/
+-rw-rw-rw-   0        0        0     6044 2023-05-05 19:30:13.000000 canlib-1.23.804/tests/test_Frame.py
+-rw-rw-rw-   0        0        0     7525 2023-05-05 19:30:13.000000 canlib-1.23.804/tests/test_bound_signal.py
+-rw-rw-rw-   0        0        0     2374 2023-05-05 19:30:13.000000 canlib-1.23.804/tests/test_device.py
+-rw-rw-rw-   0        0        0     1730 2023-05-05 19:30:13.000000 canlib-1.23.804/tests/test_ean.py
+-rw-rw-rw-   0        0        0      641 2023-05-05 19:30:13.000000 canlib-1.23.804/tests/test_kvDevice.py
+-rw-rw-rw-   0        0        0     2237 2023-05-05 19:30:13.000000 canlib-1.23.804/tests/test_versionnumber.py
```

### Comparing `canlib-1.22.565/LICENSE` & `canlib-1.23.804/LICENSE`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/PKG-INFO` & `canlib-1.23.804/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canlib
-Version: 1.22.565
+Version: 1.23.804
 Summary: Python wrapper for Kvaser CANlib
 Home-page: https://github.com/Kvaser/pycanlib
 Author: Kvaser AB
 Author-email: support@kvaser.com
 License: MIT
 Keywords: development
 Classifier: Development Status :: 4 - Beta
```

### Comparing `canlib-1.22.565/README.rst` & `canlib-1.23.804/README.rst`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/Relnotes.rst` & `canlib-1.23.804/Relnotes.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 ===========================================================================
 This is the release notes for the pycanlib module.
 
 .. contents::
     :depth: 2
 
 
+New Features and Fixed Problems in V1.23.804  (05-MAY-2023)
+===========================================================================
+* `.canlib`:
+
+  - Added support for time domains `~canlib.canlib.TimeDomain`.
+
+
 New Features and Fixed Problems in V1.22.565  (08-SEP-2022)
 ===========================================================================
 * `.canlib`:
 
   - Added support for object buffers `.canlib.objbuf`.
```

### Comparing `canlib-1.22.565/canlib/canlib/__init__.py` & `canlib-1.23.804/canlib/canlib/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,11 +36,11 @@
     enumerate_hardware, getChannelData_CardNumber,
     getChannelData_Chan_No_On_Card, getChannelData_Channel_Flags,
     getChannelData_Cust_Name, getChannelData_DriverName, getChannelData_EAN,
     getChannelData_EAN_short, getChannelData_Firmware, getChannelData_Name,
     getChannelData_Serial, getErrorText, getNumberOfChannels, getVersion,
     initializeLibrary, prodversion, reinitializeLibrary, translateBaud,
     unloadLibrary)
-
+from .timedomain import TimeDomain, TimeDomainData
 canError = CanError
 canNoMsg = CanNoMsg
 canScriptFail = CanScriptFail
```

### Comparing `canlib-1.22.565/canlib/canlib/_channel.py` & `canlib-1.23.804/canlib/canlib/_channel.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/canlib/busparams.py` & `canlib-1.23.804/canlib/canlib/busparams.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/canlib/channel.py` & `canlib-1.23.804/canlib/canlib/channel.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/canlib/channeldata.py` & `canlib-1.23.804/canlib/canlib/channeldata.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/canlib/constants.py` & `canlib-1.23.804/canlib/canlib/constants.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/canlib/dll.py` & `canlib-1.23.804/canlib/canlib/dll.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ctypes as ct
 import sys
 
 from .. import dllLoader
 from .exceptions import can_error
-from .structures import CanBusParamsTq, CanBusStatistics
+from .structures import CanBusParamsTq, CanBusStatistics, kvTimeDomainData
 
 _no_errcheck = dllLoader.no_errcheck
 
 if sys.platform.startswith('win'):
     KVCALLBACK_T = ct.WINFUNCTYPE(None, ct.c_int, ct.c_void_p, ct.c_uint)
 else:
     KVCALLBACK_T = ct.CFUNCTYPE(None, ct.c_int, ct.c_void_p, ct.c_uint)
@@ -169,14 +169,20 @@
         'kvScriptSendEvent': [[ct.c_int, ct.c_int, ct.c_int, ct.c_int, ct.c_uint]],
         'kvScriptStart': [[ct.c_int, ct.c_int]],
         'kvScriptStatus': [[ct.c_int, ct.c_int, ct.POINTER(ct.c_uint)]],
         'kvScriptStop': [[ct.c_int, ct.c_int, ct.c_int]],
         'kvScriptTxeGetData': [[ct.c_char_p, ct.c_int, ct.c_void_p, ct.POINTER(ct.c_uint)]],
         'kvScriptUnload': [[ct.c_int, ct.c_int]],
         'kvSetNotifyCallback': [[ct.c_int, KVCALLBACK_T, ct.c_void_p, ct.c_uint]],
+        'kvTimeDomainCreate': [[ct.POINTER(ct.c_void_p)]],
+        'kvTimeDomainDelete': [[ct.c_void_p]],
+        'kvTimeDomainAddHandle': [[ct.c_void_p, ct.c_int]],
+        'kvTimeDomainRemoveHandle': [[ct.c_void_p, ct.c_int]],
+        'kvTimeDomainGetData':[[ct.c_void_p, ct.POINTER(kvTimeDomainData), ct.c_size_t]],
+        'kvTimeDomainResetTime':[[ct.c_void_p]],
     }
 
     def __init__(self, ct_dll):
         # set default values for function_prototypes
         self.default_restype = ct.c_int
         self.default_errcheck = self._error_check
         super().__init__(ct_dll, **self.function_prototypes)
```

### Comparing `canlib-1.22.565/canlib/canlib/enums.py` & `canlib-1.23.804/canlib/canlib/enums.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/canlib/envvar.py` & `canlib-1.23.804/canlib/canlib/envvar.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/canlib/exceptions.py` & `canlib-1.23.804/canlib/canlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/canlib/iocontrol.py` & `canlib-1.23.804/canlib/canlib/iocontrol.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/canlib/iopin.py` & `canlib-1.23.804/canlib/canlib/iopin.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/canlib/objbuf.py` & `canlib-1.23.804/canlib/canlib/objbuf.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/canlib/structures.py` & `canlib-1.23.804/canlib/canlib/structures.py`

 * *Files 12% similar despite different names*

```diff
@@ -89,7 +89,16 @@
     _fields_ = [
         ('version', ct.c_int),  # Version of struct, currently 2
         ('arbitration_min', CanBusParamsTq),
         ('arbitration_max', CanBusParamsTq),
         ('data_min', CanBusParamsTq),
         ('data_max', CanBusParamsTq),
     ]
+
+
+class kvTimeDomainData(ct.Structure):
+    _fields_ = [
+        ('nMagiSyncGroups', ct.c_int),
+        ('nMagiSyncedMembers', ct.c_int),
+        ('nNonMagiSyncCards', ct.c_int),
+        ('nNonMagiSyncedMembers', ct.c_int),
+    ]
```

### Comparing `canlib-1.22.565/canlib/canlib/txe.py` & `canlib-1.23.804/canlib/canlib/txe.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/canlib/wrapper.py` & `canlib-1.23.804/canlib/canlib/wrapper.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/deprecation.py` & `canlib-1.23.804/canlib/deprecation.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/device.py` & `canlib-1.23.804/canlib/device.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/dllLoader.py` & `canlib-1.23.804/canlib/dllLoader.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/ean.py` & `canlib-1.23.804/canlib/ean.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/exceptions.py` & `canlib-1.23.804/canlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/frame.py` & `canlib-1.23.804/canlib/frame.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/futureapi.py` & `canlib-1.23.804/canlib/futureapi.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/j1939.py` & `canlib-1.23.804/canlib/j1939.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvDevice.py` & `canlib-1.23.804/canlib/kvDevice.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvMemoConfig.py` & `canlib-1.23.804/canlib/kvMemoConfig.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvadblib/__init__.py` & `canlib-1.23.804/canlib/kvadblib/__init__.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvadblib/attribute.py` & `canlib-1.23.804/canlib/kvadblib/attribute.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvadblib/attributedef.py` & `canlib-1.23.804/canlib/kvadblib/attributedef.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvadblib/bound_message.py` & `canlib-1.23.804/canlib/kvadblib/bound_message.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvadblib/bound_signal.py` & `canlib-1.23.804/canlib/kvadblib/bound_signal.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvadblib/dbc.py` & `canlib-1.23.804/canlib/kvadblib/dbc.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvadblib/dll.py` & `canlib-1.23.804/canlib/kvadblib/dll.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvadblib/enums.py` & `canlib-1.23.804/canlib/kvadblib/enums.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvadblib/exceptions.py` & `canlib-1.23.804/canlib/kvadblib/exceptions.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvadblib/framebox.py` & `canlib-1.23.804/canlib/kvadblib/framebox.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvadblib/message.py` & `canlib-1.23.804/canlib/kvadblib/message.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvadblib/node.py` & `canlib-1.23.804/canlib/kvadblib/node.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvadblib/signal.py` & `canlib-1.23.804/canlib/kvadblib/signal.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvadblib/wrapper.py` & `canlib-1.23.804/canlib/kvadblib/wrapper.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvamemolibxml/__init__.py` & `canlib-1.23.804/canlib/kvamemolibxml/__init__.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvamemolibxml/configuration.py` & `canlib-1.23.804/canlib/kvamemolibxml/configuration.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvamemolibxml/dll.py` & `canlib-1.23.804/canlib/kvamemolibxml/dll.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvamemolibxml/enums.py` & `canlib-1.23.804/canlib/kvamemolibxml/enums.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvamemolibxml/exceptions.py` & `canlib-1.23.804/canlib/kvamemolibxml/exceptions.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvamemolibxml/wrapper.py` & `canlib-1.23.804/canlib/kvamemolibxml/wrapper.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvlclib/__init__.py` & `canlib-1.23.804/canlib/kvlclib/__init__.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvlclib/constants.py` & `canlib-1.23.804/canlib/kvlclib/constants.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvlclib/converter.py` & `canlib-1.23.804/canlib/kvlclib/converter.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvlclib/deprecated.py` & `canlib-1.23.804/canlib/kvlclib/deprecated.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvlclib/dll.py` & `canlib-1.23.804/canlib/kvlclib/dll.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvlclib/enums.py` & `canlib-1.23.804/canlib/kvlclib/enums.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvlclib/exceptions.py` & `canlib-1.23.804/canlib/kvlclib/exceptions.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvlclib/properties.py` & `canlib-1.23.804/canlib/kvlclib/properties.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvlclib/readerformat.py` & `canlib-1.23.804/canlib/kvlclib/readerformat.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvlclib/wrapper.py` & `canlib-1.23.804/canlib/kvlclib/wrapper.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvlclib/writerformat.py` & `canlib-1.23.804/canlib/kvlclib/writerformat.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvmlib/__init__.py` & `canlib-1.23.804/canlib/kvmlib/__init__.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvmlib/constants.py` & `canlib-1.23.804/canlib/kvmlib/constants.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvmlib/deprecated.py` & `canlib-1.23.804/canlib/kvmlib/deprecated.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvmlib/dll.py` & `canlib-1.23.804/canlib/kvmlib/dll.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvmlib/enums.py` & `canlib-1.23.804/canlib/kvmlib/enums.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvmlib/events.py` & `canlib-1.23.804/canlib/kvmlib/events.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvmlib/exceptions.py` & `canlib-1.23.804/canlib/kvmlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvmlib/kme.py` & `canlib-1.23.804/canlib/kvmlib/kme.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvmlib/kmf.py` & `canlib-1.23.804/canlib/kvmlib/kmf.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvmlib/log.py` & `canlib-1.23.804/canlib/kvmlib/log.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvmlib/logfile.py` & `canlib-1.23.804/canlib/kvmlib/logfile.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvmlib/memorator.py` & `canlib-1.23.804/canlib/kvmlib/memorator.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvmlib/wrapper.py` & `canlib-1.23.804/canlib/kvmlib/wrapper.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvrlib/__init__.py` & `canlib-1.23.804/canlib/kvrlib/__init__.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvrlib/address.py` & `canlib-1.23.804/canlib/kvrlib/address.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvrlib/constants.py` & `canlib-1.23.804/canlib/kvrlib/constants.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvrlib/discovery.py` & `canlib-1.23.804/canlib/kvrlib/discovery.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvrlib/dll.py` & `canlib-1.23.804/canlib/kvrlib/dll.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvrlib/enums.py` & `canlib-1.23.804/canlib/kvrlib/enums.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvrlib/exceptions.py` & `canlib-1.23.804/canlib/kvrlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvrlib/infoset.py` & `canlib-1.23.804/canlib/kvrlib/infoset.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvrlib/remotedevice.py` & `canlib-1.23.804/canlib/kvrlib/remotedevice.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvrlib/service.py` & `canlib-1.23.804/canlib/kvrlib/service.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvrlib/structures.py` & `canlib-1.23.804/canlib/kvrlib/structures.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/kvrlib/wrapper.py` & `canlib-1.23.804/canlib/kvrlib/wrapper.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/linlib/__init__.py` & `canlib-1.23.804/canlib/linlib/__init__.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/linlib/channel.py` & `canlib-1.23.804/canlib/linlib/channel.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/linlib/dll.py` & `canlib-1.23.804/canlib/linlib/dll.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/linlib/enums.py` & `canlib-1.23.804/canlib/linlib/enums.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/linlib/exceptions.py` & `canlib-1.23.804/canlib/linlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/linlib/structures.py` & `canlib-1.23.804/canlib/linlib/structures.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/linlib/wrapper.py` & `canlib-1.23.804/canlib/linlib/wrapper.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib/versionnumber.py` & `canlib-1.23.804/canlib/versionnumber.py`

 * *Files identical despite different names*

### Comparing `canlib-1.22.565/canlib.egg-info/PKG-INFO` & `canlib-1.23.804/canlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canlib
-Version: 1.22.565
+Version: 1.23.804
 Summary: Python wrapper for Kvaser CANlib
 Home-page: https://github.com/Kvaser/pycanlib
 Author: Kvaser AB
 Author-email: support@kvaser.com
 License: MIT
 Keywords: development
 Classifier: Development Status :: 4 - Beta
```

### Comparing `canlib-1.22.565/canlib.egg-info/SOURCES.txt` & `canlib-1.23.804/canlib.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 canlib/canlib/enums.py
 canlib/canlib/envvar.py
 canlib/canlib/exceptions.py
 canlib/canlib/iocontrol.py
 canlib/canlib/iopin.py
 canlib/canlib/objbuf.py
 canlib/canlib/structures.py
+canlib/canlib/timedomain.py
 canlib/canlib/txe.py
 canlib/canlib/wrapper.py
 canlib/kvadblib/__init__.py
 canlib/kvadblib/attribute.py
 canlib/kvadblib/attributedef.py
 canlib/kvadblib/bound_message.py
 canlib/kvadblib/bound_signal.py
@@ -102,8 +103,14 @@
 canlib/kvrlib/wrapper.py
 canlib/linlib/__init__.py
 canlib/linlib/channel.py
 canlib/linlib/dll.py
 canlib/linlib/enums.py
 canlib/linlib/exceptions.py
 canlib/linlib/structures.py
-canlib/linlib/wrapper.py
+canlib/linlib/wrapper.py
+tests/test_Frame.py
+tests/test_bound_signal.py
+tests/test_device.py
+tests/test_ean.py
+tests/test_kvDevice.py
+tests/test_versionnumber.py
```

### Comparing `canlib-1.22.565/setup.py` & `canlib-1.23.804/setup.py`

 * *Files identical despite different names*

