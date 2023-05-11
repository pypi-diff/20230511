# Comparing `tmp/omniscript-liveaction-3.0.44.tar.gz` & `tmp/omniscript-liveaction-3.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniscript-liveaction-3.0.44.tar", last modified: Tue Nov 15 01:54:06 2022, max compression
+gzip compressed data, was "omniscript-liveaction-3.0.49.tar", last modified: Thu May 11 20:42:55 2023, max compression
```

## Comparing `omniscript-liveaction-3.0.44.tar` & `omniscript-liveaction-3.0.49.tar`

### file list

```diff
@@ -1,62 +1,88 @@
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2022-11-15 01:54:06.309145 omniscript-liveaction-3.0.44/
--rw-rw-r--   0 gary      (1000) gary      (1000)     1074 2022-09-08 23:54:24.000000 omniscript-liveaction-3.0.44/LICENSE
--rw-rw-r--   0 gary      (1000) gary      (1000)       64 2022-09-23 22:41:06.000000 omniscript-liveaction-3.0.44/MANIFEST.in
--rw-rw-r--   0 gary      (1000) gary      (1000)      568 2022-11-15 01:54:06.309145 omniscript-liveaction-3.0.44/PKG-INFO
--rw-rw-r--   0 gary      (1000) gary      (1000)       65 2022-09-08 23:54:24.000000 omniscript-liveaction-3.0.44/README.md
--rw-rw-r--   0 gary      (1000) gary      (1000)        3 2022-11-15 01:50:47.000000 omniscript-liveaction-3.0.44/build.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)       84 2022-09-14 00:49:41.000000 omniscript-liveaction-3.0.44/pyproject.toml
--rw-rw-r--   0 gary      (1000) gary      (1000)      757 2022-11-15 01:54:06.309145 omniscript-liveaction-3.0.44/setup.cfg
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2022-11-15 01:54:06.305145 omniscript-liveaction-3.0.44/src/
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2022-11-15 01:54:06.309145 omniscript-liveaction-3.0.44/src/omniscript/
--rw-rw-r--   0 gary      (1000) gary      (1000)    10896 2022-11-11 01:59:44.000000 omniscript-liveaction-3.0.44/src/omniscript/__init__.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     5951 2022-09-08 23:54:24.000000 omniscript-liveaction-3.0.44/src/omniscript/adapter.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     6533 2022-11-04 18:18:46.000000 omniscript-liveaction-3.0.44/src/omniscript/adapterinformation.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     7566 2022-09-08 23:54:24.000000 omniscript-liveaction-3.0.44/src/omniscript/alarm.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     2792 2022-09-08 23:54:24.000000 omniscript-liveaction-3.0.44/src/omniscript/analysismodule.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     2221 2022-11-02 20:21:36.000000 omniscript-liveaction-3.0.44/src/omniscript/application.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     4445 2022-11-04 19:25:28.000000 omniscript-liveaction-3.0.44/src/omniscript/authenticationtoken.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    36976 2022-11-10 02:07:17.000000 omniscript-liveaction-3.0.44/src/omniscript/capture.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    21450 2022-11-12 01:59:28.000000 omniscript-liveaction-3.0.44/src/omniscript/capturesession.py
--rw-rw-r--   0 gary      (1000) gary      (1000)   134378 2022-11-12 01:48:00.000000 omniscript-liveaction-3.0.44/src/omniscript/capturetemplate.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     2474 2022-11-03 00:13:08.000000 omniscript-liveaction-3.0.44/src/omniscript/country.py
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2022-11-15 01:54:06.309145 omniscript-liveaction-3.0.44/src/omniscript/data/
--rw-rw-r--   0 gary      (1000) gary      (1000)    12405 2022-09-08 23:54:24.000000 omniscript-liveaction-3.0.44/src/omniscript/data/_capture_template.xml
--rw-rw-r--   0 gary      (1000) gary      (1000)    12443 2022-09-08 23:54:24.000000 omniscript-liveaction-3.0.44/src/omniscript/data/_capture_template_linux.xml
--rw-rw-r--   0 gary      (1000) gary      (1000)    12405 2022-09-08 23:54:24.000000 omniscript-liveaction-3.0.44/src/omniscript/data/_capture_template_windows.xml
--rw-rw-r--   0 gary      (1000) gary      (1000)    14591 2022-11-04 01:34:59.000000 omniscript-liveaction-3.0.44/src/omniscript/data/_class_ids.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)     3879 2022-09-08 23:54:24.000000 omniscript-liveaction-3.0.44/src/omniscript/data/_co_codes.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)     7745 2022-09-12 22:54:21.000000 omniscript-liveaction-3.0.44/src/omniscript/data/_expert_problem_ids.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)    25315 2022-09-08 23:54:24.000000 omniscript-liveaction-3.0.44/src/omniscript/data/_stat_ids.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)   103212 2022-09-08 23:54:24.000000 omniscript-liveaction-3.0.44/src/omniscript/data/expertdescriptions.xml
--rw-rw-r--   0 gary      (1000) gary      (1000)   328348 2022-09-08 23:54:24.000000 omniscript-liveaction-3.0.44/src/omniscript/data/pspecs.xml
--rw-rw-r--   0 gary      (1000) gary      (1000)     1924 2022-09-15 21:46:16.000000 omniscript-liveaction-3.0.44/src/omniscript/directory.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    15763 2022-10-15 01:03:30.000000 omniscript-liveaction-3.0.44/src/omniscript/enginestatus.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     9220 2022-10-04 00:21:23.000000 omniscript-liveaction-3.0.44/src/omniscript/eventlog.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     2337 2022-09-20 22:37:42.000000 omniscript-liveaction-3.0.44/src/omniscript/fileinformation.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     8744 2022-09-27 20:48:04.000000 omniscript-liveaction-3.0.44/src/omniscript/filter.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    62369 2022-09-28 23:33:29.000000 omniscript-liveaction-3.0.44/src/omniscript/filternode.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    19210 2022-11-12 01:53:14.000000 omniscript-liveaction-3.0.44/src/omniscript/forensicsearch.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    47210 2022-10-22 00:07:04.000000 omniscript-liveaction-3.0.44/src/omniscript/forensictemplate.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     4606 2022-09-08 23:54:24.000000 omniscript-liveaction-3.0.44/src/omniscript/graphtemplate.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    17329 2022-11-11 19:27:52.000000 omniscript-liveaction-3.0.44/src/omniscript/invariant.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     1997 2022-11-04 01:30:58.000000 omniscript-liveaction-3.0.44/src/omniscript/mediainformation.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    19019 2022-11-04 18:24:32.000000 omniscript-liveaction-3.0.44/src/omniscript/omniaddress.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     2594 2022-09-08 23:54:24.000000 omniscript-liveaction-3.0.44/src/omniscript/omnidatatable.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    50433 2022-11-15 01:28:21.000000 omniscript-liveaction-3.0.44/src/omniscript/omniengine.py
--rw-rw-r--   0 gary      (1000) gary      (1000)      668 2022-09-21 00:26:47.000000 omniscript-liveaction-3.0.44/src/omniscript/omnierror.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     3423 2022-11-05 01:02:57.000000 omniscript-liveaction-3.0.44/src/omniscript/omniid.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     2650 2022-09-28 20:44:34.000000 omniscript-liveaction-3.0.44/src/omniscript/omniport.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    13903 2022-11-11 20:07:36.000000 omniscript-liveaction-3.0.44/src/omniscript/omniscript.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     9871 2022-09-27 20:45:17.000000 omniscript-liveaction-3.0.44/src/omniscript/packet.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     7740 2022-09-20 22:38:16.000000 omniscript-liveaction-3.0.44/src/omniscript/packetfileinformation.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    11260 2022-10-25 23:07:31.000000 omniscript-liveaction-3.0.44/src/omniscript/peektime.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     1335 2022-10-27 01:09:29.000000 omniscript-liveaction-3.0.44/src/omniscript/performancelogger.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     5487 2022-09-12 21:49:02.000000 omniscript-liveaction-3.0.44/src/omniscript/readstream.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     6341 2022-09-08 23:54:24.000000 omniscript-liveaction-3.0.44/src/omniscript/statslimit.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     3187 2022-09-08 23:54:24.000000 omniscript-liveaction-3.0.44/src/omniscript/voipsettings.py
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2022-11-15 01:54:06.309145 omniscript-liveaction-3.0.44/src/omniscript_liveaction.egg-info/
--rw-rw-r--   0 gary      (1000) gary      (1000)      568 2022-11-15 01:54:06.000000 omniscript-liveaction-3.0.44/src/omniscript_liveaction.egg-info/PKG-INFO
--rw-rw-r--   0 gary      (1000) gary      (1000)     1757 2022-11-15 01:54:06.000000 omniscript-liveaction-3.0.44/src/omniscript_liveaction.egg-info/SOURCES.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)        1 2022-11-15 01:54:06.000000 omniscript-liveaction-3.0.44/src/omniscript_liveaction.egg-info/dependency_links.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)       21 2022-11-15 01:54:06.000000 omniscript-liveaction-3.0.44/src/omniscript_liveaction.egg-info/requires.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)       11 2022-11-15 01:54:06.000000 omniscript-liveaction-3.0.44/src/omniscript_liveaction.egg-info/top_level.txt
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-05-11 20:42:55.059468 omniscript-liveaction-3.0.49/
+-rw-rw-r--   0 gary      (1000) gary      (1000)     1074 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/LICENSE
+-rw-rw-r--   0 gary      (1000) gary      (1000)       64 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/MANIFEST.in
+-rw-rw-r--   0 gary      (1000) gary      (1000)      567 2023-05-11 20:42:55.059468 omniscript-liveaction-3.0.49/PKG-INFO
+-rw-rw-r--   0 gary      (1000) gary      (1000)       64 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/README.md
+-rw-rw-r--   0 gary      (1000) gary      (1000)        3 2023-05-11 20:38:11.000000 omniscript-liveaction-3.0.49/build.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        7 2023-05-11 20:41:32.000000 omniscript-liveaction-3.0.49/next_version.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)      386 2023-04-18 20:30:17.000000 omniscript-liveaction-3.0.49/pyproject.toml
+-rw-rw-r--   0 gary      (1000) gary      (1000)      757 2023-05-11 20:42:55.059468 omniscript-liveaction-3.0.49/setup.cfg
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-05-11 20:42:55.055468 omniscript-liveaction-3.0.49/src/
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-05-11 20:42:55.055468 omniscript-liveaction-3.0.49/src/omniscript/
+-rw-rw-r--   0 gary      (1000) gary      (1000)    20154 2023-05-10 02:07:41.000000 omniscript-liveaction-3.0.49/src/omniscript/__init__.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     7575 2023-05-05 00:13:09.000000 omniscript-liveaction-3.0.49/src/omniscript/adapter.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     7935 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/adapterinformation.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    12703 2023-04-26 20:54:34.000000 omniscript-liveaction-3.0.49/src/omniscript/alarm.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     3293 2023-05-02 23:20:12.000000 omniscript-liveaction-3.0.49/src/omniscript/analysismodule.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     2598 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/application.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     3963 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/auditlog.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     5751 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/authenticationtoken.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    17010 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/capabilities.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    37328 2023-05-10 02:06:29.000000 omniscript-liveaction-3.0.49/src/omniscript/capture.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    24964 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/capturesession.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)   160802 2023-05-09 01:18:30.000000 omniscript-liveaction-3.0.49/src/omniscript/capturetemplate.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     2521 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/country.py
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-05-11 20:42:55.055468 omniscript-liveaction-3.0.49/src/omniscript/data/
+-rw-rw-r--   0 gary      (1000) gary      (1000)     5462 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/data/_capability_ids.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)    12405 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/data/_capture_template.xml
+-rw-rw-r--   0 gary      (1000) gary      (1000)    12443 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/data/_capture_template_linux.xml
+-rw-rw-r--   0 gary      (1000) gary      (1000)    12405 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/data/_capture_template_windows.xml
+-rw-rw-r--   0 gary      (1000) gary      (1000)    14676 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/data/_class_ids.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)     3879 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/data/_co_codes.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)     7745 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/data/_expert_problem_ids.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)    25315 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/data/_stat_ids.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)   103212 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/data/expertdescriptions.xml
+-rw-rw-r--   0 gary      (1000) gary      (1000)   404432 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/data/pspecs.xml
+-rw-rw-r--   0 gary      (1000) gary      (1000)     2724 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/decryptionkey.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     3277 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/decryptionkeytemplate.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     2726 2023-05-10 00:25:05.000000 omniscript-liveaction-3.0.49/src/omniscript/directory.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    70178 2023-04-26 20:54:26.000000 omniscript-liveaction-3.0.49/src/omniscript/dms.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    42825 2023-04-19 17:17:01.000000 omniscript-liveaction-3.0.49/src/omniscript/enginesettings.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    15583 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/enginestatus.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     9216 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/eventlog.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    30578 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/expertpreferences.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     2274 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/fileinformation.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     9735 2023-05-01 23:17:47.000000 omniscript-liveaction-3.0.49/src/omniscript/filter.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    62919 2023-05-01 23:34:25.000000 omniscript-liveaction-3.0.49/src/omniscript/filternode.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    19189 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/forensicsearch.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    48325 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/forensictemplate.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     4643 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/graphtemplate.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     3489 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/helpers.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    35455 2023-05-03 23:29:40.000000 omniscript-liveaction-3.0.49/src/omniscript/invariant.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     2974 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/license.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    34748 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/liveflow.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     1966 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/mediainformation.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     2626 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/nametable.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    33684 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/notifications.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    19481 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/omniaddress.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     2602 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/omnidatatable.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    80340 2023-05-10 18:19:42.000000 omniscript-liveaction-3.0.49/src/omniscript/omniengine.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)      671 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/omnierror.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     3500 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/omniid.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     2597 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/omniport.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    15211 2023-05-01 22:25:38.000000 omniscript-liveaction-3.0.49/src/omniscript/omniscript.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    14115 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/packet.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     7688 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/packetfileinformation.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    11196 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/peektime.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     1330 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/performancelogger.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     3055 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/protocol.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     2513 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/protocoltranslation.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     5483 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/readstream.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     8139 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/remoteengine.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     2819 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/selection.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     6184 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/omniscript/statslimit.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     5532 2023-04-19 17:17:01.000000 omniscript-liveaction-3.0.49/src/omniscript/user.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     4396 2023-05-02 22:56:48.000000 omniscript-liveaction-3.0.49/src/omniscript/voipsettings.py
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-05-11 20:42:55.055468 omniscript-liveaction-3.0.49/src/omniscript_liveaction.egg-info/
+-rw-rw-r--   0 gary      (1000) gary      (1000)      567 2023-05-11 20:42:55.000000 omniscript-liveaction-3.0.49/src/omniscript_liveaction.egg-info/PKG-INFO
+-rw-rw-r--   0 gary      (1000) gary      (1000)     2467 2023-05-11 20:42:55.000000 omniscript-liveaction-3.0.49/src/omniscript_liveaction.egg-info/SOURCES.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        1 2023-05-11 20:42:55.000000 omniscript-liveaction-3.0.49/src/omniscript_liveaction.egg-info/dependency_links.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)       21 2023-05-11 20:42:55.000000 omniscript-liveaction-3.0.49/src/omniscript_liveaction.egg-info/requires.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)       17 2023-05-11 20:42:55.000000 omniscript-liveaction-3.0.49/src/omniscript_liveaction.egg-info/top_level.txt
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-05-11 20:42:55.059468 omniscript-liveaction-3.0.49/src/tests/
+-rw-rw-r--   0 gary      (1000) gary      (1000)        0 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/tests/__init__.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     5345 2023-04-19 17:17:01.000000 omniscript-liveaction-3.0.49/src/tests/conftest.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)      261 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/tests/decrypt_file.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)      292 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/tests/encrypt_file.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     1010 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/tests/encryption_util.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)      334 2023-04-14 22:29:02.000000 omniscript-liveaction-3.0.49/src/tests/gen_key.py
```

### Comparing `omniscript-liveaction-3.0.44/LICENSE` & `omniscript-liveaction-3.0.49/LICENSE`

 * *Files identical despite different names*

### Comparing `omniscript-liveaction-3.0.44/PKG-INFO` & `omniscript-liveaction-3.0.49/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: omniscript-liveaction
-Version: 3.0.44
+Version: 3.0.49
 Summary: Automate LiveAction LiveCapture and LiveWire.
 Home-page: https://MyPeek.LiveAction.com
 Author: gvisser
 Author-email: gvisser@liveaction.com
 Project-URL: Bug Tracker, https://MyPeek.LiveAction.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Example Package
+# OmniScript 3.0
 
 Automate LiveAction LiveCapture and LiveWire.
```

### Comparing `omniscript-liveaction-3.0.44/setup.cfg` & `omniscript-liveaction-3.0.49/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = omniscript-liveaction
-version = 3.0.44
+version = 3.0.49
 author = gvisser
 author_email = gvisser@liveaction.com
 description = Automate LiveAction LiveCapture and LiveWire.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://MyPeek.LiveAction.com
 project_urls = 
@@ -15,15 +15,15 @@
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 include_package_data = True
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = 
 	requests
 	six
 	urllib3
 
 [options.packages.find]
 where = src
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/adapter.py` & `omniscript-liveaction-3.0.49/src/omniscript/adapter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 ﻿"""Adapter class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 import six
 
+from .invariant import AdapterType
 from .omniid import OmniId
 
 
-adapter_types = ['Network Interface Card', 'File Adapter', 'Plugin Adapter']
-
-adapter_find_attributes = ['name', 'id', 'device_name']
-
 _adapt_prop_dict = {
-    'AdapterFeatures' : 'features',
-    'AdapterType' : 'type',
-    'address' : 'address',
-    'channels' : 'channels',
-    'clsid' : 'class_id',
-    'defaultLinkSpeed' : 'default_link_speed',
-    'description' : 'description',
-    'DeviceName' : 'device_name',
-    'flags' : 'flags',
-    'identifier' : 'id',
-    'ids' : 'ids',
-    'InterfaceFeatures' : 'interface_features',
-    'linkSpeed' : 'link_speed',
-    'mediaSubType' : 'media_sub_type',
-    'mediaType' : 'media_type',
-    'ringBufferSize' : 'ring_buffer_size',
-    'type' : 'type',
-    'WildPacketsAPI' : 'wildpackets_api'
+    'AdapterFeatures': 'features',
+    'AdapterType': 'adapter_type',
+    'address': 'address',
+    'channels': 'channels',
+    'clsid': 'class_id',
+    'defaultLinkSpeed': 'default_link_speed',
+    'description': 'description',
+    'DeviceName': 'device_name',
+    'flags': 'flags',
+    'identifier': 'adapter_id',
+    'ids': 'ids',
+    'InterfaceFeatures': 'interface_features',
+    'linkSpeed': 'link_speed',
+    'mediaSubType': 'media_sub_type',
+    'mediaType': 'media_type',
+    'ringBufferSize': 'ring_buffer_size',
+    'type': 'adapter_type',
+    'WildPacketsAPI': 'wildpackets_api'
 }
 
 
 class Adapter(object):
     """The Adapter class has the attributes of an adapter.
-    The 
-    :func:`get_adapter_list() 
+    The
+    :func:`get_adapter_list()
     <omniscript.omniengine.OmniEngine.get_adapter_list>`
     function returns a list of Adapter objects.
     """
 
-    id = ''
-    """The adapter's identifier, on Windows is a four digit code that
-    is engine specific.
+    adapter_id = ''
+    """The adapter's identifier is a string. On Linux it's the port
+       name, for instance eth0. On Windows is a four digit code with
+       leading zeros are significant and is engine specific.
     """
 
-    features = 0
-    """Features of the adapter. Bit fields."""
-
-    adapter_type = 0
-    """The type of adapter. Any of the ADDRESS TYPE constants."""
+    adapter_type = AdapterType.UKNOWN
+    """The type of adapter. Must be an AdapteryType value."""
 
     address = '00:00:00:00:00:00'
     """The Ethernet Address of the adapter."""
 
     class_id = None
     """The adapters Class Id as a GUID."""
 
@@ -65,14 +60,17 @@
 
     description = ''
     """The decscription/name of the adapter."""
 
     device_name = ''
     """The device name of the adapter: Broadcom, Intel..."""
 
+    features = 0
+    """Features of the adapter. Bit fields."""
+
     interface_features = 0
     """Interface Features of the adapter. Bit fields."""
 
     link_speed = 0
     """The link speed of the adapter in bits per second."""
 
     media_type = 0
@@ -80,47 +78,65 @@
 
     media_sub_type = 0
     """The Media Sub Type of the adapter."""
 
     ring_buffer_size = 0
     """The size of the ring buffer in bytes."""
 
-    type = 0
-    """The type of adapter."""
-
     wildpackets_api = False
-    """Does the adapter support the WildPackets' API."""
+    """Does the adapter support the WildPackets' Wireless API."""
+
+    adapter_types = (
+        'Unknown', 'Network Interface Card', 'File Adapter', 'Plugin Adapter', 'Remote Adapter')
+
+    find_attributes = ('name', 'id', 'device_name', 'type')
+
+    _endpoint = 'Adapters'
 
     def __init__(self, engine, props):
         self._engine = engine
         self.logger = engine.logger
+        self.adapter_id = Adapter.adapter_id
+        self.adapter_type = Adapter.adapter_type
+        self.address = Adapter.address
+        self.class_id = Adapter.class_id
+        self.default_link_speed = Adapter.default_link_speed
+        self.description = Adapter.description
+        self.device_name = Adapter.device_name
+        self.features = Adapter.features
+        self.interface_features = Adapter.interface_features
+        self.link_speed = Adapter.link_speed
+        self.media_type = Adapter.media_type
+        self.media_sub_type = Adapter.media_sub_type
+        self.ring_buffer_size = Adapter.ring_buffer_size
+        self.wildpackets_api = Adapter.wildpackets_api
         self._load(props)
         if self.description is None:
             self.description = ''
-        if not self.device_name and (self.name == self.id):
+        if not self.device_name and (self.name == self.adapter_id):
             self.device_name = self.name
 
     def __repr__(self):
         return f'Adapter: {self.description}'
 
     def __str__(self):
         return f'Adapter: {self.description}'
 
     def _load(self, props):
         """Set attributes from a dictionary."""
         if isinstance(props, dict):
             if len(props) == 2:
-                config = props['configuration']
-                info = props['info']
+                config = props.get('configuration')
+                info = props.get('info')
             else:
                 config = props
                 info = None
             # Set attributes from the configuration (config) dictionary.
             if isinstance(config, dict):
-                for k,v in config.items():
+                for k, v in config.items():
                     a = _adapt_prop_dict.get(k)
                     if a is not None and hasattr(self, a):
                         if isinstance(getattr(self, a), six.string_types):
                             setattr(self, a, v if v else '')
                         elif isinstance(getattr(self, a), int):
                             setattr(self, a, int(v) if v else 0)
                         elif isinstance(getattr(self, a), list):
@@ -129,15 +145,15 @@
                             setattr(self, a, v)
                         elif getattr(self, a) is None:
                             setattr(self, a, OmniId(v))
                         else:
                             setattr(self, a, v)
             # Set attributes from the information (info) dictionary.
             if isinstance(info, dict):
-                for k,v in info.items():
+                for k, v in info.items():
                     a = _adapt_prop_dict.get(k)
                     if a is not None and hasattr(self, a):
                         if isinstance(getattr(self, a), six.string_types):
                             setattr(self, a, v if v else '')
                         elif isinstance(getattr(self, a), int):
                             setattr(self, a, int(v) if v else 0)
                         elif isinstance(getattr(self, a), list):
@@ -151,35 +167,58 @@
 
     @property
     def name(self):
         """The name/description of the adapter. (Read Only)"""
         return self.description
 
     def rename(self, new_name):
-        self._engine.rename_adapter(self.adapter_type, self.id, new_name)
+        self._engine.rename_adapter(self.adapter_type, self.adapter_id, new_name)
 
 
 def _create_adapter_list(engine, resp):
     lst = []
     adapters = resp['adapters']
     if adapters is not None:
         for props in adapters:
             lst.append(Adapter(engine, props))
     lst.sort(key=lambda x: x.description)
     return lst
 
 
-def find_adapter(adapters, value, attrib=adapter_find_attributes[0]):
-    """Finds an adapter in the list."""
-    if (not adapters) or (attrib not in adapter_find_attributes):
+def find_all_adapters(adapters, value, attrib=Adapter.find_attributes[0]):
+    """Finds all adapters that match the value in the adapters list"""
+    if (not adapters) or (attrib not in Adapter.find_attributes):
+        return None
+
+    if attrib == 'id':
+        _attrib = 'adapter_id'
+    elif attrib == 'type':
+        _attrib = 'adapter_type'
+    else:
+        _attrib = attrib
+
+    if isinstance(adapters, list):
+        return [i for i in adapters if isinstance(i, Adapter) and getattr(i, _attrib) == value]
+
+
+def find_adapter(adapters, value, attrib=Adapter.find_attributes[0]):
+    """Find the first adapter in the list that matches the criteria."""
+    if (not adapters) or (attrib not in Adapter.find_attributes):
         return None
 
     if len(adapters) == 0:
         return None
 
     if isinstance(value, Adapter):
-        _value = value.id
+        _value = value.adapter_id
         attrib = 'id'
     else:
         _value = value
 
-    return next((i for i in adapters if getattr(i, attrib) == _value), None)
+    if attrib == 'id':
+        _attrib = 'adapter_id'
+    elif attrib == 'type':
+        _attrib = 'adapter_type'
+    else:
+        _attrib = attrib
+
+    return next((i for i in adapters if getattr(i, _attrib) == _value), None)
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/adapterinformation.py` & `omniscript-liveaction-3.0.49/src/omniscript/adapterinformation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,121 +1,170 @@
 ﻿"""AdapterInfo class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
-
-import six
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
+from .invariant import AdapterType
 from .omniaddress import EthernetAddress
 from .omniid import OmniId
 
 
-adapter_types = ['Network Interface Card', 'File Adapter', 'Plugin Adapter']
-
-adapter_find_attributes = ['name', 'id', 'device_name']
-
-
 class AdapterInformation(object):
     """The Adapter Information class has the attributes of an adapter.
-    The 
-    :func:`get_adapter_info_list() 
+    The
+    :func:`get_adapter_info_list()
     <omniscript.omniengine.OmniEngine.get_adapter_info_list>`
     function returns a list of Adapter Information objects.
     """
 
-    adapter_type = 0
+    adapter_id = ''
+    """The adapter's identifier is a string. On Linux it's the port
+       name, for instance eth0. On Windows is a four digit code with
+       leading zeros are significant and is engine specific.
+    """
+
+    adapter_type = AdapterType.UKNOWN
+    """The type of Adapter."""
+
     address = None
+    """The EthernetAddress of the Adapter."""
+
     channel_list = None
+    """The list of channels this Adapter supports."""
+
     characteristics = 0
+    """The characteristics of the Adapter."""
+
     description = ''
+    """A description of the Adapter."""
+
     enumerator = ''
+    """The enumerator of the Adapter. The enumerator is a string
+    and not an integer value. Any leading zeros are significant.
+    """
+
     extended_description = ''
+    """The extended description of the Adapter."""
+
     features = None
+    """Features of the Adapter."""
+
     flags = 0
-    id = None
-    interface_fatures = None
+    """Flags of the Adapter."""
+
+    interface_features = None
+    """Interface Features of the Adapter."""
+
     interface_version = None
+    """Interface Version of the Adapter."""
+
     link_speed = 0
+    """The Adapter's link speed."""
+
     media_type = 0
+    """The media type the Adapter supports."""
+
     media_sub_type = 0
+    """The media sub-type the Adapter supports."""
+
     product_name = None
+    """The manufacterer's product name of the Adapter."""
+
     service_name = None
+    """The service name of the Adapter."""
+
     symbolic_link = None
+    """A symbolic link of the Adapter."""
+
     title = None
+    """The title of the Adapter."""
+
     versions = None
+    """The version of the Adapter."""
+
     option_hidden = False
+    """Is the Adapter hidden from the user."""
+
     option_valid = True
-    optoin_valid_advanced = True
+    """Is the Adapter a valid Adapter."""
+
+    option_valid_advanced = True
+    """Is the advanced configuration of the Adapter valid."""
+
     option_virtual = True
+    """Is this a virtual Adapter."""
+
+    adapter_types = ('Network Interface Card', 'File Adapter', 'Plugin Adapter')
+
+    find_attributes = ('name', 'id', 'device_name')
 
     def __init__(self, engine, props):
         self._engine = engine
         self.logger = engine.logger
+        self.adapter_id = AdapterInformation.adapter_id
         self.adapter_type = AdapterInformation.adapter_type
         self.address = AdapterInformation.address
         self.channel_list = AdapterInformation.channel_list
         self.characteristics = AdapterInformation.characteristics
         self.description = AdapterInformation.description
         self.enumerator = AdapterInformation.enumerator
         self.extended_description = AdapterInformation.extended_description
         self.features = AdapterInformation.features
         self.flags = AdapterInformation.flags
-        self.id = AdapterInformation.id
         self.link_speed = AdapterInformation.link_speed
         self.media_type = AdapterInformation.media_type
         self.media_sub_type = AdapterInformation.media_sub_type
         self.product_name = AdapterInformation.product_name
         self.service_name = AdapterInformation.service_name
         self.symbolic_link = AdapterInformation.symbolic_link
         self.title = AdapterInformation.title
         self.versions = AdapterInformation.versions
         self.option_hidden = AdapterInformation.option_hidden
         self.option_valid = AdapterInformation.option_valid
-        self.optoin_valid_advanced = AdapterInformation.optoin_valid_advanced
+        self.option_valid_advanced = AdapterInformation.option_valid_advanced
         self.option_virtual = AdapterInformation.option_virtual
         self._load(props)
 
     def __repr__(self):
         return f'AdapterInformation: {self.description}'
 
     def __str__(self):
         return f'Adapter: {self.description}'
 
     def _load(self, props):
         """Set attributes from a dictionary."""
         if isinstance(props, dict):
-            for k,v in props.items():
-                if k == 'type':
-                    self.adapter_type = int(v)
-                elif k == 'address':
+            for k, v in props.items():
+                if k == 'address':
                     self.address = EthernetAddress(v)
                 elif k == 'channel_list':
                     self.channel_list = []
                     if isinstance(v, dict):
+                        # TODO: Implement this.
                         if 'enumChannels' in v:
-                            ch = v.get('enumChannels')
+                            _ = v.get('enumChannels')
                         elif 'wirelessChannels' in v:
-                            wch = v.get('wirelessChannels')
+                            _ = v.get('wirelessChannels')
                 elif k == 'characteristics':
-                    self.channel_list = v
+                    self.characteristics = v
                 elif k == 'description':
                     self.description = v
                 elif k == 'enumerator':
                     self.enumerator = v
                 elif k == 'descriptionExtended':
                     self.extended_description = v
                 elif k == 'features':
                     self.features = v
                 elif k == 'flags':
                     self.flags = int(v)
                 elif k == 'id':
-                    self.id = OmniId(v)
+                    self.adapter_id = OmniId(v)
                 elif k == 'interfaceFeatures':
-                    self.interface_fatures = v
+                    self.interface_features = v
                 elif k == 'interfaceVersion':
                     self.interface_version = v
                 elif k == 'link_speed':
                     self.link_speed = int(v)
                 elif k == 'mediaType':
                     self.media_type = int(v)
                 elif k == 'mediaSubType':
@@ -124,30 +173,30 @@
                     self.product_name = v
                 elif k == 'serviceName':
                     self.service_name = v
                 elif k == 'symbolicLink':
                     self.symbolic_link = v
                 elif k == 'title':
                     self.title = v
+                elif k == 'type':
+                    self.adapter_type = int(v)
                 elif k == 'versions':
                     if v:
                         try:
                             self.versions = dict(
-                                    (x.strip(),
-                                    y.strip() if not y.strip().isnumeric() else int(y))
-                                for x,y in (e.split(':')
-                                for e in v.split(', ')))
+                                (x.strip(), y.strip() if not y.strip().isnumeric() else int(y))
+                                for x, y in (e.split(':') for e in v.split(', ')))
                         except Exception:
                             self.versions = [v]
                 elif k == 'hidden':
                     self.option_hidden = v
                 elif k == 'valid':
                     self.option_valid = v
                 elif k == 'validAdvanced':
-                    self.optoin_valid_advanced = v
+                    self.option_valid_advanced = v
                 elif k == 'supportsVirtual':
                     self.option_virtual = v
 
     @property
     def name(self):
         """The name/description of the adapter. (Read Only)"""
         return self.description
@@ -159,17 +208,17 @@
     if isinstance(adapters, list):
         for a in adapters:
             lst.append(AdapterInformation(engine, a))
     lst.sort(key=lambda x: x.description)
     return lst
 
 
-def find_adapter_information(adapters, value, attrib=adapter_find_attributes[0]):
+def find_adapter_information(adapters, value, attrib=AdapterInformation.find_attributes[0]):
     """Finds an Adapter Information in the list."""
-    if (not adapters) or (attrib not in adapter_find_attributes):
+    if (not adapters) or (attrib not in AdapterInformation.find_attributes):
         return None
 
     if len(adapters) == 0:
         return None
 
     if isinstance(value, AdapterInformation):
         _value = value.id
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/analysismodule.py` & `omniscript-liveaction-3.0.49/src/omniscript/analysismodule.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 ﻿"""AnalysisModule class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 from .omniid import OmniId
 
 
-find_attribs = ['name', 'id']
-
 _plugin_prop_dict = {
-    'Identifier':'id',
-    'Name':'name'
+    'Identifier': 'id',
+    'Name': 'name'
 }
 
 
 class AnalysisModule(object):
-    """The AnalysisModule class has the attributes of an analysis module 
-    (plugin). The 
-    :func:`get_analysis_module_list() 
+    """The AnalysisModule class has the attributes of an analysis module
+    (plugin). The
+    :func:`get_analysis_module_list()
     <omniscript.omniengine.OmniEngine.get_analysis_module_list>`
     function returns a list of AnalysisModule objects.
     """
 
     category_ids = []
     """The analysis module's list of category identifier."""
 
+    configuration = None
+    """For an instance of an Analysis Module in a CaptureTemplate, the
+    configuration information for the instance.
+    """
+
     engine = None
     """The OmniEngine of the analysis module."""
 
     file_name = None
     """The analysis module's file name on its OmniEngine."""
 
     id = None
@@ -40,62 +43,74 @@
 
     publisher = None
     """The analysis module's publisher."""
 
     version = None
     """The version of the analysis module."""
 
-    def __init__(self, engine, props):
+    find_attributes = ('name', 'id')
+
+    def __init__(self, engine, props=None, id=None):
         self.engine = engine
         self.category_ids = AnalysisModule.category_ids
+        self.configuration = AnalysisModule.configuration
         self.file_name = AnalysisModule.file_name
         self.id = AnalysisModule.id
         self.name = AnalysisModule.name
         self.publisher = AnalysisModule.publisher
         self.version = AnalysisModule.version
-        self._load(props)
+        if props is not None:
+            self._load(props)
+        elif id is not None:
+            self.id = id
 
     def __str__(self):
         return f'AnalysisModule: {self.name}'
 
     def _load(self, props):
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             if k == 'clsid':
                 self.id = OmniId(v)
             elif k == 'cagegoryIds':
                 self.category_ids = v
             elif k == 'file':
                 self.file_name = v
             elif k == 'name':
                 self.name = v
             elif k == 'publisher':
                 self.publisher = v
             elif k == 'version':
                 self.version = v
 
+    def get_configuration(self):
+        return self.configuration
+
+    def set_configuration(self, config):
+        self.configuration = config
+
 
 def _create_analysis_module_list(engine, props):
     lst = []
     if props and len(props) > 0:
         for plugin in props:
             lst.append(AnalysisModule(engine, plugin))
     lst.sort(key=lambda x: x.name)
     return lst
 
 
-def find_analysis_module(analysis_modules, value, attrib=find_attribs[0]):
+def find_analysis_module(analysis_modules, value, attrib=AnalysisModule.find_attributes[0]):
     """Finds an analysis module in the list"""
-    if (not analysis_modules) or (attrib not in find_attribs):
+    if (not analysis_modules) or (attrib not in AnalysisModule.find_attributes):
         return None
 
     if len(analysis_modules) == 0:
         return None
 
     if isinstance(value, AnalysisModule):
         _value = value.id
         attrib = 'id'
     else:
         _value = value
-    
+
     return next((i for i in analysis_modules if getattr(i, attrib) == _value), None)
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/application.py` & `omniscript-liveaction-3.0.49/src/omniscript/application.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,44 @@
 """Application class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 
 find_attribs = ['name', 'id']
 
+
 class Application(object):
-    """An Application object."""
+    """An Application object.
+    """
 
     category = ''
+    """The category of the Application."""
+
     color = 0
+    """The color of the Application."""
+
     description = ''
+    """The description of the Application."""
+
     id = ''
+    """The identifier of the Application"""
+
     name = ''
+    """The name of the Application."""
+
     productivity = 0
+    """The productivity level of the Application."""
+
     reference = ''
+    """The reference value of the Application."""
+
     risk = 0
+    """The risk level of the application."""
 
     # Tags
     _tag_category = 'category'
     _tag_color = 'color'
     _tag_description = 'description'
     _tag_id = 'id'
     _tag_name = 'name'
@@ -38,15 +55,15 @@
         self.productivity = Application.productivity
         self.reference = Application.reference
         self.risk = Application.risk
         self._load(props)
 
     def _load(self, props):
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 if k == Application._tag_category:
                     self.category = v
                 elif k == Application._tag_color:
                     self.color = int(v.strip('#'), 16)
                 elif k == Application._tag_description:
                     self.description = v
                 elif k == Application._tag_id:
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/capture.py` & `omniscript-liveaction-3.0.49/src/omniscript/capture.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ﻿"""Capture class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 import six
 import xml.etree.ElementTree as ET
 
-from .invariant import (CAPTURE_STATUS_CAPTURING, DECODE_PLAIN_TEXT, DECODE_HTML,
-    DECODE_TAG_STREAM)
+from .invariant import (
+    CAPTURE_STATUS_CAPTURING, DECODE_PLAIN_TEXT, DECODE_HTML, DECODE_TAG_STREAM)
 
 from .adapter import Adapter
 # from .callstatistic import CallStatistic
 from .capturetemplate import CaptureTemplate
 # from .expertquery import ExpertQuery
 # from .expertresult import ExpertResult
 from .invariant import EngineDataFormat as DF, EngineOperation as EO
@@ -27,35 +27,36 @@
 # from .statscontext import StatsContext
 # from .summarystatistic import SummaryStatistic
 
 # from .expertresult import _create_expert_result_list
 from .packet import _create_packet_list
 
 
-find_attribs = ['name', 'id']
-
 status_map = {
-    0 : 'Idle',
-    1 : 'Capturing',
-    256 : 'Idle Start Active',
-    257 : 'Wait Start',
-    8192 : 'Idle Stop Active',
-    8193 : 'Capturing Stop Active',
-    8448 : 'Idle Start and Stop Active',
-    8449 : 'Start Stop Active'
+    0: 'Idle',
+    1: 'Capturing',
+    256: 'Idle Start Active',
+    257: 'Wait Start',
+    8192: 'Idle Stop Active',
+    8193: 'Capturing Stop Active',
+    8448: 'Idle Start and Stop Active',
+    8449: 'Start Stop Active'
 }
 
 jtrue = 'true'
 jfalse = 'false'
 
+
 def jbool(b):
     """Returns 'true' if 'b' is True else 'false'."""
     return jtrue if b else jfalse
 
+
 def _summary_xml_to_stats_list(xml):
+    # TODO: change the inner lists to tuples.
     type_dict = [
         [''],
         ['date'],
         ['time'],
         ['duration'],
         ['packets'],
         ['bytes'],
@@ -65,115 +66,115 @@
     ]
     element = ET.fromstring(xml)
     lst = []
     snapshot = element.find('summarystats/snapshot')
     for stat in snapshot:
         stat_type = int(stat.attrib['type'])
         s = {
-            'id':stat.attrib['id'],
-            'parent':stat.attrib['parent'],
-            'type':stat_type,
-            'flags':int(stat.attrib['flags'])
+            'id': stat.attrib['id'],
+            'parent': stat.attrib['parent'],
+            'type': stat_type,
+            'flags': int(stat.attrib['flags'])
         }
         if stat_type >= 1 and stat_type <= len(type_dict):
             for t in type_dict[stat_type]:
                 s[t] = stat.attrib[t]
         # lst.append(SummaryStatistic(s))
     return lst
 
 
 _capture_prop_dict = {
-    'adapter' : 'adapter_name',
-    'adapterId' : 'adapter_id',
-    'adapterInfo' : 'adapter',
-    'adapterType' : 'adapter_type',
-    'alarmsEnabled' : 'option_alarms',
-    'alarmsInfo' : 'alarms_info',
-    'alarmsMajor' : 'alarms_major',
-    'alarmsMinor' : 'alarms_minor',
-    'alarmsSevere' : 'alarms_severe',
-    'analysisDroppedPackets' : 'analysis_dropped_packets',
-    'bufferCapacity' : 'buffer_size',
-    'capacityAvailable' : 'buffer_available',
-    'capacityUsed' : 'buffer_used',
-    'captureId' : 'group_id',
-    'captureSessionId' : 'session_id',
-    'comment' : 'comment',
-    'creationTime' : 'creation_time',
-    'creator' : 'creator',
-    'creatorSID' : 'creator_sid',
-    'ctdEnabled' : 'option_ctd',
-    'ctdIntelligent' : 'option_ctd_intelligent',
-    'ctdSize' : 'file_size',
-    'ctdStartTime' : 'ctd_start_time',
-    'ctdStopTime' : 'ctd_stop_time',
-    'dataPacketCount' : '_data_packet_count',
-    'dataPacketsDropped' : 'data_packets_dropped',
-    'dataSize' : 'data_size',
-    'dataSizeReserved' : 'data_size_reserved',
-    'dataStartTime' : 'data_start_time',
-    'dataStopTime' : 'data_stop_time',
-    'distributedCapture' : 'option_distributed',
-    'duplicatePacketsDiscarded' : 'duplicate_packets_discarded',
-    'duration' : 'duration',
-    'elkCapture' : 'option_elk',
-    'errorCondition' : 'error_code',
-    'errorConditionText' : 'error_code_text',
-    'expertEnabled' : 'option_expert',
-    'filterIdsEnabled' : 'filter_list',
-    'filterMode' : 'filter_mode',
-    'filtersEnabled' : 'option_filters',
-    'firstPacket' : 'first_packet',
-    'flowsDropped' : 'flows_dropped',
-    'graphsCount' : 'graphs_count',
-    'graphsEnabled' : 'option_graphs',
-    'groupID' : 'group_id',
-    'hardwareDeduplication' : 'option_hardware_deduplication',
-    'hardwareFiltering' : 'option_hardware_filtering',
-    'hardwareProfileID' : 'hardware_profile_id',
-    'hardwareProfileName' : 'hardware_profile',
-    'hardwareSlicing' : '',
-    'hidden' : 'option_hidden',
-    'id' : 'id',
-    'indexingEnabled' : 'option_indexing',
-    'linkSpeed' : 'link_speed',
-    'loggedOnUserSid' : 'logged_on_user_sid',
-    'mediaInfo' : 'media_information',
-    'mediaSubType' : 'media_sub_type',
-    'mediaType' : 'media_type',
-    'modificationBy' : 'modified_by',
-    'modificationTime' : 'modification_time',
-    'modificationType' : 'modification_type',
-    'multiStream' : 'option_multistream',
-    'name' : 'name',
-    'packetBufferEnabled' : 'option_packet_buffer',
-    'packetCount' : 'packet_count',
-    'packetsAnalyzed' : 'packets_analyzed',
-    'packetsDropped' : 'packets_dropped',
-    'packetsFiltered' : 'packets_filtered',
-    'packetsReceived' : 'packets_received',
-    'pluginsEnabled' : 'plugin_list',
-    'resetCount' : 'reset_count',
-    'spotlightCapture' : 'option_spotlight',
-    'startTime' : 'start_time',
-    'statsEnabled' : 'option_stats',
-    'status' : 'status',
-    'stopTime' : 'stop_time',
-    'threatEyeNVCapture' : 'option_threateye',
-    'timelineStatsEnabled' : 'option_timeline_stats',
-    'triggerCount' : 'trigger_count',
-    'triggerDuration' : 'trigger_duration',
-    'voiceEnabled' : 'option_voice',
-    'webEnabled' : 'option_web'
+    'adapter': 'adapter_name',
+    'adapterId': 'adapter_id',
+    'adapterInfo': 'adapter',
+    'adapterType': 'adapter_type',
+    'alarmsEnabled': 'option_alarms',
+    'alarmsInfo': 'alarms_info',
+    'alarmsMajor': 'alarms_major',
+    'alarmsMinor': 'alarms_minor',
+    'alarmsSevere': 'alarms_severe',
+    'analysisDroppedPackets': 'analysis_dropped_packets',
+    'bufferCapacity': 'buffer_size',
+    'capacityAvailable': 'buffer_available',
+    'capacityUsed': 'buffer_used',
+    'captureId': 'group_id',
+    'captureSessionId': 'session_id',
+    'comment': 'comment',
+    'creationTime': 'creation_time',
+    'creator': 'creator',
+    'creatorSID': 'creator_sid',
+    'ctdEnabled': 'option_ctd',
+    'ctdIntelligent': 'option_ctd_intelligent',
+    'ctdSize': 'file_size',
+    'ctdStartTime': 'ctd_start_time',
+    'ctdStopTime': 'ctd_stop_time',
+    'dataPacketCount': '_data_packet_count',
+    'dataPacketsDropped': 'data_packets_dropped',
+    'dataSize': 'data_size',
+    'dataSizeReserved': 'data_size_reserved',
+    'dataStartTime': 'data_start_time',
+    'dataStopTime': 'data_stop_time',
+    'distributedCapture': 'option_distributed',
+    'duplicatePacketsDiscarded': 'duplicate_packets_discarded',
+    'duration': 'duration',
+    'elkCapture': 'option_elk',
+    'errorCondition': 'error_code',
+    'errorConditionText': 'error_code_text',
+    'expertEnabled': 'option_expert',
+    'filterIdsEnabled': 'filter_list',
+    'filterMode': 'filter_mode',
+    'filtersEnabled': 'option_filters',
+    'firstPacket': 'first_packet',
+    'flowsDropped': 'flows_dropped',
+    'graphsCount': 'graphs_count',
+    'graphsEnabled': 'option_graphs',
+    'groupID': 'group_id',
+    'hardwareDeduplication': 'option_hardware_deduplication',
+    'hardwareFiltering': 'option_hardware_filtering',
+    'hardwareProfileID': 'hardware_profile_id',
+    'hardwareProfileName': 'hardware_profile',
+    'hardwareSlicing': '',
+    'hidden': 'option_hidden',
+    'id': 'id',
+    'indexingEnabled': 'option_indexing',
+    'linkSpeed': 'link_speed',
+    'loggedOnUserSid': 'logged_on_user_sid',
+    'mediaInfo': 'media_information',
+    'mediaSubType': 'media_sub_type',
+    'mediaType': 'media_type',
+    'modificationBy': 'modified_by',
+    'modificationTime': 'modification_time',
+    'modificationType': 'modification_type',
+    'multiStream': 'option_multistream',
+    'name': 'name',
+    'packetBufferEnabled': 'option_packet_buffer',
+    'packetCount': 'packet_count',
+    'packetsAnalyzed': 'packets_analyzed',
+    'packetsDropped': 'packets_dropped',
+    'packetsFiltered': 'packets_filtered',
+    'packetsReceived': 'packets_received',
+    'pluginsEnabled': 'plugin_list',
+    'resetCount': 'reset_count',
+    'spotlightCapture': 'option_spotlight',
+    'startTime': 'start_time',
+    'statsEnabled': 'option_stats',
+    'status': 'status',
+    'stopTime': 'stop_time',
+    'threatEyeNVCapture': 'option_threateye',
+    'timelineStatsEnabled': 'option_timeline_stats',
+    'triggerCount': 'trigger_count',
+    'triggerDuration': 'trigger_duration',
+    'voiceEnabled': 'option_voice',
+    'webEnabled': 'option_web'
 }
 
 
 class Capture(object):
     """The Capture class has the attributes of a capture.
-    The functions :func:`create_capture() 
+    The functions :func:`create_capture()
     <omniscript.omniengine.OmniEngine.create_capture>`
     and :func:`find_capture() <omniscript.omniengine.OmniEngine.find_capture>`
     return a Capture object.
     The function :func:`get_capture_list()
     <omniscript.omniengine.OmniEngine.get_capture_list>`
     returns a list of Capture objects.
     """
@@ -219,15 +220,15 @@
     buffer_used = 0
     """The number of bytes in use of the capture's buffer."""
 
     comment = ''
     """The capture's comment."""
 
     creation_time = None
-    """When the capture was created as 
+    """When the capture was created as
     :class:`PeekTime <omniscript.peektime.PeekTime>`.
     """
 
     creator = ''
     """The name of the account that created the capture."""
 
     creator_sid = ''
@@ -253,15 +254,15 @@
 
     data_size = 0
     """The size, in bytes, of the packet files when they are saved to
     disk.
     """
 
     data_size_reserved = 0
-    """The number of bytes reserved for packet files being saved to 
+    """The number of bytes reserved for packet files being saved to
     disk files. If this value is exceeded, the old file(s) will be
     deleted.
     """
 
     data_start_time = None
     """The time, as
     :class:`PeekTime <omniscript.peektime.PeekTime>`,
@@ -313,20 +314,20 @@
     group_id = 0
     """The index, as an integer, of the capture group."""
 
     hardware_profile = ''
     """The name of the Hardware Profile."""
 
     hardware_profile_id = None
-    """The Hardware Profile Id as 
+    """The Hardware Profile Id as
     :class:`OmniId <omniscript.omniid.OmniId>`
     """
 
     id = None
-    """The Identifier, as 
+    """The Identifier, as
     :class:`OmniId <omniscript.omniid.OmniId>`,
     of the Capture.
     """
 
     link_speed = 0
     """The link speed, in bits per second, of the capture's adapter."""
 
@@ -456,14 +457,16 @@
 
     option_voice = False
     """Are Voice Statistics enabled?"""
 
     option_web = False
     """Are Web Statistics enabled?"""
 
+    find_attributes = ('name', 'id')
+
     def __init__(self, engine, props=None):
         self._engine = engine
         self.logger = engine.logger
         self._context = None
 
         self.adapter = Capture.adapter
         self.adapter_id = Capture.adapter_id
@@ -566,15 +569,15 @@
     #     # DEBUG with open(r"c:\temp\stat_data.bin", 'wb') as fle:
     #     # DEBUG    fle.write(data)
     #     # self._context = StatsContext(data.raw)
 
     def _load(self, props):
         """Set attributes from a dictionary."""
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 a = _capture_prop_dict.get(k)
                 if a is None or not hasattr(self, a):
                     continue
                 if isinstance(getattr(self, a), six.string_types):
                     setattr(self, a, v if v else '')
                 elif isinstance(getattr(self, a), bool):
                     setattr(self, a, (v != 'true') if v else False)
@@ -584,17 +587,16 @@
                     if (a == 'filter_list') or (a == 'plugin_list'):
                         setattr(self, a, [OmniId(id) for id in v])
                 elif getattr(self, a) is None:
                     if a == 'adapter':
                         setattr(self, a, Adapter(self.engine, v))
                     elif a in ('group_id', 'id', 'session_id'):
                         setattr(self, a, OmniId(v))
-                    elif a in ('creation_time', 'data_start_time',
-                                'data_stop_time', 'modification_time',
-                                'start_time', 'stop_time'):
+                    elif a in ('creation_time', 'data_start_time', 'data_stop_time',
+                               'modification_time', 'start_time', 'stop_time'):
                         setattr(self, a, PeekTime(v))
                     elif a == 'media_information':
                         setattr(self, a, MediaInformation(v))
         # first_packet is a packet index (index into the capture buffer),
         #   convert it into a packet number(?).
         if self.first_packet > 0:
             self.first_packet += 1
@@ -618,36 +620,36 @@
 
     #     Args:
     #         refresh (boolean): refresh the statistics cache. Default is False.
     #     """
     #     if self._context is None or refresh:
     #         self._get_statistics()
     #     if self._context is None:
-    #         self.logger.error("Failed to get statistics context " \
-    #                           "for capture: %s.", self.name)
+    #         self.logger.error(("Failed to get statistics context "
+    #                            "for capture: %s.", self.name))
     #         return None
     #     return self._context.get_application_statistics()
 
     # def get_call_stats(self, refresh=False):
-    #     """Returns a 
+    #     """Returns a
     #     :class:`CallStatistic <omniscript.callstatistic.CallStatistic>`
     #     object.
     #     Note that only one CallStatistic object is returned.
 
     #     Args:
     #         refresh (boolean): refresh the statistics cache. Default is False.
     #     """
     #     if self._context is None or refresh:
     #         self._get_statistics()
     #     if self._context is None:
-    #         self.logger.error("Failed to get statistics context " \
-    #                           "for capture: %s.", self.name)
+    #         self.logger.error(("Failed to get statistics context "
+    #                            "for capture: %s.", self.name))
     #         return None
     #     return self._context.get_call_statistics()
-    
+
     # def get_capture_template(self):
     #     """Get the
     #     :class:`CaptureTemplate <omniscript.capturetemplate.CaptureTemplate>`
     #     of this capture.
 
     #     Returns:
     #         A :class:`CaptureTemplate <omniscript.capturetemplate.CaptureTemplate>`
@@ -663,16 +665,16 @@
     #     Args:
     #         refresh (boolean): refresh the statistics cache.
     #                            Default is False.
     #     """
     #     if self._context is None or refresh:
     #         self._get_statistics()
     #     if self._context is None:
-    #         self.logger.error("Failed to get statistics context " \
-    #                           "for capture: %s.", self.name)
+    #         self.logger.error(("Failed to get statistics context "
+    #                            "for capture: %s.", self.name))
     #         return None
     #     return self._context.get_country_statistics()
 
     # def get_node_stats(self, refresh=False):
     #     """Returns a list of
     #     :class:`NodeStatistic <omniscript.nodestatistic.NodeStatistic>`
     #     objects.
@@ -680,16 +682,16 @@
     #     Args:
     #         refresh (boolean): refresh the statistics cache.
     #                            Default is False.
     #     """
     #     if self._context is None or refresh:
     #         self._get_statistics()
     #     if self._context is None:
-    #         self.logger.error("Failed to get statistics context " \
-    #                           "for capture: %s.", self.name)
+    #         self.logger.error(("Failed to get statistics context "
+    #                            "for capture: %s.", self.name))
     #         return None
     #     return self._context.get_node_statistics()
 
     def get_options(self):
         """Returns the Capture's Options in a Capture Template object."""
         pr = self.perf('get_options')
         cmd = f'captures/{self.id.format()}/options/'
@@ -758,15 +760,15 @@
             ('packetCount', count),
             ('showLogical', jtrue),
             ('showAddressNames', jfalse),
             ('showPortNames', jfalse)
         ]
         column_dict = Packet.get_prop_dict()
         for k in column_dict.keys():
-            req_props.append( ('columns', k) )
+            req_props.append(('columns', k))
         pr = self.perf('get_packets')
         command = f'captures/{self.id.format()}/packet-list/'
         props = self._engine._issue_command(command, pr, params=req_props)
         return _create_packet_list(props)
 
     # def get_packets_old(self, indices):
     # #     """Returns a list of
@@ -812,60 +814,60 @@
     #     # for i in indexes:
     #     #     if isinstance(i, int):
     #     #         pl.append(self.get_packet(i))
     #     return pl
 
     # def get_protocol_stats(self, refresh=False):
     #     """Returns a list of
-    #     :class:`ProtocolStatistic 
+    #     :class:`ProtocolStatistic
     #     <omniscript.protocolstatistic.ProtocolStatistic>`
     #     objects.
 
     #     Args:
     #         refresh (boolean): refresh the statistics cache. Default is False.
     #     """
     #     if self._context is None or refresh:
     #         self._get_statistics()
     #     if self._context is None:
-    #         self.logger.error("Failed to get statistics context for " \
-    #                           "capture: %s.", self.name)
+    #         self.logger.error(("Failed to get statistics context for "
+    #                            "capture: %s.", self.name))
     #         return None
     #     return self._context.get_protocol_statistics()
 
     # def get_stats_context(self, refresh=False):
-    #     """Returns a 
-    #     :class:`StatsContext 
+    #     """Returns a
+    #     :class:`StatsContext
     #     <omniscript.statscontext.StatsContext>`
     #     object.
 
     #     Args:
     #         refresh (boolean): refresh the statistics context. Default is False.
     #     """
     #     if self._context is None or refresh:
     #         self._get_statistics()
     #     if self._context is None:
-    #         self.logger.error("Failed to get statistics context for " \
-    #                           "capture: %s.", self.name)
+    #         self.logger.error(("Failed to get statistics context for "
+    #                            "capture: %s.", self.name))
     #         return None
     #     return self._context
 
     # def get_summary_stats(self, refresh=False):
     #     """Returns a list of
-    #     :class:`SummaryStatistic 
+    #     :class:`SummaryStatistic
     #     <omniscript.summarystatistic.SummaryStatistic>`
     #     objects.
 
     #     Args:
     #         refresh (boolean): refresh the statistics cache. Default is False.
     #     """
     #     if self._context is None or refresh:
     #         self._get_statistics()
     #     if self._context is None:
-    #         self.logger.error("Failed to get statistics context for " \
-    #                           "capture: %s.", self.name)
+    #         self.logger.error(("Failed to get statistics context for "
+    #                            "capture: %s.", self.name))
     #         return None
     #     return self._context.get_summary_statistics()
 
     def is_capturing(self, refresh=True):
         """Returns True if the capture is capturing.
 
         Args:
@@ -958,47 +960,48 @@
     #     """
     #     if self.id is None:
     #         self.logger.error("Failed to get the id for Capture: %s", self.name)
     #         return False
     #     # <captures>
     #     #   <capture id="{xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx}" />
     #     # </captures>
-    #     request = r'<request><captures><capture id="' + str(self.id) + \
-    #               r'"/></captures></request>'
+    #     request = (r'<request><captures><capture id="' + str(self.id) +
+    #                r'"/></captures></request>')
     #     response = self._engine._issue_xml_string_result(
     #                 invariant.OMNI_CLEAR_CAPTURES, request)
     #     omniscript._parse_command_response(response)
     #     self.refresh()
 
     # def save_all_packets(self, filename):
     #     """Save the packets of the capture to a file."""
     #     return self._engine.save_all_packets(self, filename)
 
-    # def select_related(self, packets, criteria=omniscript.SELECT_BY_SOURCE_DESTINATION, unique=True):
+    # def select_related(self, packets, criteria=omniscript.SELECT_BY_SOURCE_DESTINATION,
+    #                    unique=True):
     #     """Returns a list of packet numbers for the packets and criteria specified.
     #     If unique is True then only unique packet numbers are returned. Otherwise the
     #     list may contain duplicates.
     #     Example: packet 1 matches packets 1,2,5 and packet 3 matches packets 2,3,4,6.
     #     Unique returns [1,2,3,4,5,6], non-unique returns [1,2,5,2,3,4,6].
     #     """
     #     _packets = packets if isinstance(packets, list) else [packets]
     #     magic = 0x4E8B3899
     #     version = 1
     #     logical_addr = 1
     #     packet_count = len(packets)
-    #     buf = struct.pack('=II16sIII%dQ' % packet_count, magic, version, 
+    #     buf = struct.pack('=II16sIII%dQ' % packet_count, magic, version,
     #                       self.id.bytes_le(), criteria, logical_addr,
     #                       packet_count, *packets)
     #     response = self._engine._issue_command(invariant.OMNI_SELECT_RELATED,
     #                                            buf, len(buf))
     #     try:
     #         omniscript._parse_command_response(response)
     #     except omniscript.OmniError as oe:
     #         raise oe
-    #     except:
+    #     except Exception:
     #         # Only errors are parseable.
     #         # But ET.parse(data) will throw an exception
     #         #   catch the exception and process the success.
     #         pass
     #     stream = ReadStream(response)
     #     pkt_count = stream.read_uint()
     #     if unique:
@@ -1037,17 +1040,26 @@
     if captures is not None:
         for props in captures:
             lst.append(Capture(engine, props))
     lst.sort(key=lambda x: x.name)
     return lst
 
 
-def find_capture(captures, value, attrib = find_attribs[0]):
+def find_all_captures(captures, value, attrib=Capture.find_attributes[0]):
+    """Finds all captures that match the value in the capture list."""
+    if (not captures) or (attrib not in Capture.find_attributes):
+        return None
+
+    if isinstance(captures, list):
+        return [i for i in captures if isinstance(i, Capture) and getattr(i, attrib) == value]
+
+
+def find_capture(captures, value, attrib=Capture.find_attributes[0]):
     """Finds a capture in the list"""
-    if not captures or attrib not in find_attribs:
+    if not captures or attrib not in Capture.find_attributes:
         return None
 
     if len(captures) == 0:
         return None
 
     if isinstance(value, Capture):
         _value = value.id
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/capturesession.py` & `omniscript-liveaction-3.0.49/src/omniscript/capturesession.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ﻿"""CaptureSession class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 import six
 
 from .omniid import OmniId
 from .peektime import PeekTime
 
 from .invariant import SessionDataType, SessionStatisticsType
@@ -32,103 +32,50 @@
     'top-applications',
     'top-ipv4-nodes',
     'top-ipv6-nodes',
     'top-physical-nodes',
     'top-protocols'
 )
 
-class SessionData(object): ...
-class SessionStatistics(object): ...
 
-class ApplicationsData(object): ...
-class CallQualityData(object): ...
-class CallUtilizationData(object): ...
-class MulticastData(object): ...
-class PacketsData(object): ...
-class PacketSizeData(object): ...
-class ProtocolsData(object): ...
-class UtilizationData(SessionData): ...
-class VlanMplsData(object): ...
-class WirelessData(object): ...
-
-class StatisticsEntry(object): ...
+# class SessionData(object): ...
+# class SessionStatistics(object): ...
+# class ApplicationsData(object): ...
+# class CallQualityData(object): ...
+# class CallUtilizationData(object): ...
+# class MulticastData(object): ...
+# class PacketsData(object): ...
+# class PacketSizeData(object): ...
+# class ProtocolsData(object): ...
+# class UtilizationData(SessionData): ...
+# class VlanMplsData(object): ...
+# class WirelessData(object): ...
+# class StatisticsEntry(object): ...
 
 
 def _decode_color(value):
     return int(value.strip('#'), 16)
 
 
 def _format_color(color):
     return f'#{color:6X}' if color else '#000000'
 
 
-class SessionData(object):
-    session_id = 0
-    data_type = 0
-    start_time = None
-    end_time = None
-    sample_interval = 0
-    sample_count = 0
-    data_list = None
-
-    def __init__(self, session, props):
-        self._session = session
-        self.session_id = 0
-        self.data_type = None
-        self.start_time = None
-        self.end_time = None
-        self.sample_interval = 0
-        self.sample_count = None
-        self.data_list = None
-        self._load(props)
-
-    def _load(self, props):
-        if not isinstance(props, dict):
-            return
-        self.session_id = int(props.get('sessionId', 0))
-        self.data_type = SessionDataType(props.get('viewType', 0))
-        self.start_time = PeekTime(props.get('startTime', 0))
-        self.end_time = PeekTime(props.get('startTime', 0))
-        self.sample_interval = int(props.get('sampleInterval', 0))
-        self.data_list = None
-        if self.data_type == SessionDataType.UTILIZATION_MBPS:
-            self.data_list = [UtilizationData(d) for d in props.get('data')]
-        elif self.data_type == SessionDataType.PACKETS:
-            self.data_list = [PacketsData(d) for d in props.get('data')]
-        elif self.data_type == SessionDataType.MULTICAST:
-            self.data_list = [MulticastData(d) for d in props.get('data')]
-        elif self.data_type == SessionDataType.PACKET_SIZES:
-            self.sample_count = int(props.get('sampleCount'))
-            self.data_list = [PacketSizeData(d) for d in props.get('data')]
-        elif self.data_type == SessionDataType.VLAN_MPLS:
-            self.data_list = [VlanMplsData(d) for d in props.get('data')]
-        elif self.data_type == SessionDataType.PROTOCOLS_MBPS:
-            self.data_list = [ProtocolsData(d) for d in props.get('data')]
-        elif self.data_type == SessionDataType.PROTOCOLS_PPS:
-            self.data_list = [ProtocolsData(d) for d in props.get('data')]
-        elif self.data_type == SessionDataType.CALL_QUALITY:
-            self.data_list = [CallQualityData(d) for d in props.get('data')]
-        elif self.data_type == SessionDataType.CALL_UTILIZATION:
-            self.data_list = [CallUtilizationData(d) for d in props.get('data')]
-        elif self.data_type == SessionDataType.WIRELESS_PACKETS:
-            self.data_list = [WirelessData(d) for d in props.get('data')]
-        elif self.data_type == SessionDataType.WIRELESS_RETRIES:
-            self.data_list = [WirelessData(d) for d in props.get('data')]
-        elif self.data_type == SessionDataType.APPLICATIONS_MBPS:
-            self.data_list = [ApplicationsData(d) for d in props.get('data')]
-        elif self.data_type == SessionDataType.APPLICATIONS_PPS:
-            self.data_list = [ApplicationsData(d) for d in props.get('data')]
-        else:
-            raise(ValueError('Invalid data_type'))
-
-
 class ApplicationsData(object):
+    """An Applications Data object.
+    """
+
     application_id = 0.0
+    """The identifier of the application."""
+
     others = 0.0
+    """The others of the applications."""
+
     total_packets = 0
+    """The total number of packets in the data."""
 
     def __init__(self, props):
         self.application_id = 0.0
         self.others = 0.0
         self.total_packets = 0
         if isinstance(props, dict):
             self.application_id = float(props.get('appid', 0.0))
@@ -136,20 +83,34 @@
             self.total_packets = int(props.get('totalPackets', 0))
 
     def format(self):
         return f'app id: {self.application_id}, other: {self.others}, pkts: {self.total_packets}'
 
 
 class CallQualityData(object):
+    """A Call Quality Data object.
+    """
+
     bad = 0.0
+    """The number of bad quality calls."""
+
     fair = 0.0
+    """The number of fair quality calls."""
+
     good = 0.0
+    """The number of good quality calls."""
+
     poor = 0.0
+    """The number of poor quality calls."""
+
     unknown = 0.0
+    """The number of unkown quality calls."""
+
     total_packets = 0
+    """The total number of packets."""
 
     def __init__(self, props):
         self.bad = 0.0
         self.fair = 0.0
         self.good = 0.0
         self.poor = 0.0
         self.unknown = 0.0
@@ -160,21 +121,29 @@
             self.good = float(props.get('good', 0.0))
             self.poor = float(props.get('poor', 0.0))
             self.unknown = float(props.get('unknown', 0.0))
             self.packets = int(props.get('totalPackets', 0))
 
     def format(self):
         return (f'bad: {self.bad}, fair: {self.fair}, good: {self.good}, poor: {self.poor}, '
-            f'unknown: {self.unknown}, pkts: {self.total_packets}')
+                f'unknown: {self.unknown}, pkts: {self.total_packets}')
 
 
 class CallUtilizationData(object):
+    """A Call Utilization Data object.
+    """
+
     call_mbps = 0.0
+    """The amount of traffic of the calls in megabits per second."""
+
     mbps = 0.0
+    """The speed of traffic in megabits per second."""
+
     total_packets = 0
+    """The total number of packets."""
 
     def __init__(self, props):
         self.call_mbps = 0.0
         self.mbps = 0.0
         self.total_packets = 0
         if isinstance(props, dict):
             self.call_mbps = float(props.get('callMbps', 0.0))
@@ -182,20 +151,34 @@
             self.packets = int(props.get('totalPackets', 0))
 
     def format(self):
         return f'call: {self.call_mbps}, mbps: {self.mbps}, pkts: {self.total_packets}'
 
 
 class PacketsData(object):
+    """A Packets Data object.
+    """
+
     packets = 0.0
+    """The number of packets."""
+
     dropped = 0.0
+    """The number of dropped packets."""
+
     crc = 0.0
+    """The number of crc errors."""
+
     undersize = 0.0
+    """The number of under-sized packets."""
+
     oversize = 0.0
+    """The number of over-sized packets."""
+
     total_packets = 0
+    """The total number of packets."""
 
     def __init__(self, props):
         self.packets = 0.0
         self.dropped = 0.0
         self.crc = 0.0
         self.undersize = 0.0
         self.oversize = 0.0
@@ -209,42 +192,66 @@
             self.total_packets = int(props.get('totalPackets', 0))
 
     def format(self):
         return f'pkts: {self.total_packets}'
 
 
 class PacketSizeData(object):
+    """A PacketSizeData object.
+    """
+
     size_range = ''
+    """The range of packet sizes."""
+
     packets = 0.0
+    """The packet count."""
+
     pct = 0.0
+    """The pct."""
+
     total_packets = 0
+    """The total number of packets."""
 
     def __init__(self, props):
         self.size_range = ''
         self.packets = 0.0
         self.pct = 0.0
         self.total_packets = 0
         if isinstance(props, dict):
             self.size_range = props.get('entry, 0.0')
             self.packets = float(props.get('packets', 0.0))
             self.pct = float(props.get('pct', 0.0))
             self.total_packets = int(props.get('totalPackets', 0))
 
     def format(self):
         return (f'range: {self.size_range}, p: {self.packets}, pct: {self.pct}, '
-            f'pkts: {self.total_packets}')
+                f'pkts: {self.total_packets}')
 
 
 class ProtocolsData(object):
+    """A ProtocolsData object.
+    """
+
     icmp = 0.0
+    """The number packets of the ICMP protocol."""
+
     ipv4 = 0.0
+    """The number of IPv4 packets."""
+
     ipv6 = 0.0
+    """The number of IPv6 packets."""
+
     tcp = 0.0
+    """The number packets of the TCP protocol."""
+
     udp = 0.0
+    """The number packets of the UDP protocol."""
+
     total_packets = 0
+    """The total number of packets."""
 
     def __init__(self, props):
         self.icmp = 0.0
         self.ipv4 = 0.0
         self.ipv6 = 0.0
         self.tcp = 0.0
         self.udp = 0.0
@@ -255,83 +262,126 @@
             self.ipv6 = float(props.get('ipv6', 0.0))
             self.tcp = float(props.get('tcp', 0.0))
             self.udp = float(props.get('udp', 0.0))
             self.packets = int(props.get('totalPackets', 0))
 
     def format(self):
         return (f'icmp: {self.icmp}, ipv4: {self.ipv4}, ipv6: {self.ipv6}, tcp: {self.tcp}, '
-            f'udp: {self.udp}, pkts: {self.total_packets}')
+                f'udp: {self.udp}, pkts: {self.total_packets}')
 
 
 class MulticastData(object):
+    """A MulticastData object.
+    """
+
     broadcast = 0.0
+    """The number of broadcast packets."""
+
     multicast = 0.0
+    """The number of multicast packets."""
+
     unicast = 0.0
+    """The number of unicast packets."""
+
     total_packets = 0
+    """The total number of packets."""
 
     def __init__(self, props):
         self.broadcast = 0.0
         self.multicast = 0.0
         self.unicast = 0.0
         self.total_packets = 0
         if isinstance(props, dict):
             self.broadcast = float(props.get('broadcast', 0.0))
             self.multicast = float(props.get('multicast', 0.0))
             self.unicast = float(props.get('unicast', 0.0))
             self.total_packets = int(props.get('totalPackets', 0))
 
     def format(self):
         return (f'broad: {self.broadcast}, multi: {self.multicast}, uni: {self.unicast}, '
-            f'pkts: {self.total_packets}')
+                f'pkts: {self.total_packets}')
 
 
 class UtilizationData(object):
+    """A UtilizationData object.
+    """
+
     mbps = 0.0
+    """The traffic utilization in megabits per second."""
+
     total_packets = 0
+    """The total number of packets."""
 
     def __init__(self, props):
         self.mbps = 0.0
         self.total_packets = 0
         if isinstance(props, dict):
             self.mbps = float(props.get('mbps', 0.0))
             self.total_packets = int(props.get('totalPackets', 0))
 
     def format(self):
         return f'mbps: {self.mbps}, pkts: {self.total_packets}'
 
 
 class VlanMplsData(object):
+    """A VlanMplsData object.
+    """
+
     mpls = 0.0
+    """The number of MPLS packets."""
+
     packets = 0.0
+    """The number of packets."""
+
     vlan = 0.0
+    """The number of VLAN packets."""
+
     total_packets = 0
+    """The total number of packets."""
 
     def __init__(self, props):
         self.mpls = 0.0
         self.packets = 0.0
         self.vlan = 0.0
         self.total_packets = 0
         if isinstance(props, dict):
             self.mpls = float(props.get('mpls', 0.0))
             self.packets = float(props.get('packets', 0.0))
             self.vlan = float(props.get('vlan', 0.0))
             self.total_packets = int(props.get('total_packets', 0))
 
     def format(self):
-        return f'mpls: {self.mpls}, p: {self.packets}, vlan: {self.vlan}, pkts: {self.total_packets}'
+        return (f'mpls: {self.mpls}, p: {self.packets}, vlan: {self.vlan}, '
+                f'pkts: {self.total_packets}')
 
 
 class WirelessData(object):
+    """A WirelessData object.
+    """
+
     call_mbps = 0.0
+    """The utilization of wireless data in megabits per second."""
+
     control = 0.0
+    """The number of control packets."""
+
     data = 0.0
+    """The number of data packets."""
+
     management = 0.0
+    """The number of management packets."""
+
     packets = 0.0
+    """The number of packets."""
+
     retry = 0.0
+    """The number of retry packets."""
+
     total_packets = 0
+    """The total number of packets."""
 
     def __init__(self, props):
         self.call_mbps = 0.0
         self.control = 0.0
         self.data = 0.0
         self.management = 0.0
         self.packets = 0.0
@@ -344,25 +394,115 @@
             self.management = float(props.get('management', 0.0))
             self.packets = float(props.get('packets', 0.0))
             self.retry = float(props.get('retry', 0.0))
             self.total_packets = int(props.get('totalPackets', 0))
 
     def format(self):
         return (f'call: {self.call_mbps}, ctrl: {self.control}, d: {self.data}, '
-            f'man: {self.management}, p: {self.packets}, re: {self.retry}, '
-            f'pkts: {self.total_packets}')
+                f'man: {self.management}, p: {self.packets}, re: {self.retry}, '
+                f'pkts: {self.total_packets}')
+
+
+class SessionData(object):
+    """Session Data object.
+    """
+
+    session_id = 0
+    """The session id of the data."""
+
+    data_type = 0
+    """The type of the data."""
+
+    start_time = None
+    """The timestamp of the start of the data."""
+
+    end_time = None
+    """The timestamp of the end of the data."""
+
+    sample_interval = 0
+    """The interval in seconds between samples."""
+
+    sample_count = 0
+    """"The number of samples in the data."""
+
+    data_list = None
+    """The list of samples."""
+
+    def __init__(self, session, props):
+        self._session = session
+        self.session_id = 0
+        self.data_type = None
+        self.start_time = None
+        self.end_time = None
+        self.sample_interval = 0
+        self.sample_count = None
+        self.data_list = None
+        self._load(props)
+
+    def _load(self, props):
+        if not isinstance(props, dict):
+            return
+        self.session_id = int(props.get('sessionId', 0))
+        self.data_type = SessionDataType(props.get('viewType', 0))
+        self.start_time = PeekTime(props.get('startTime', 0))
+        self.end_time = PeekTime(props.get('startTime', 0))
+        self.sample_interval = int(props.get('sampleInterval', 0))
+        self.data_list = None
+        if self.data_type == SessionDataType.UTILIZATION_MBPS:
+            self.data_list = [UtilizationData(d) for d in props.get('data')]
+        elif self.data_type == SessionDataType.PACKETS:
+            self.data_list = [PacketsData(d) for d in props.get('data')]
+        elif self.data_type == SessionDataType.MULTICAST:
+            self.data_list = [MulticastData(d) for d in props.get('data')]
+        elif self.data_type == SessionDataType.PACKET_SIZES:
+            self.sample_count = int(props.get('sampleCount'))
+            self.data_list = [PacketSizeData(d) for d in props.get('data')]
+        elif self.data_type == SessionDataType.VLAN_MPLS:
+            self.data_list = [VlanMplsData(d) for d in props.get('data')]
+        elif self.data_type == SessionDataType.PROTOCOLS_MBPS:
+            self.data_list = [ProtocolsData(d) for d in props.get('data')]
+        elif self.data_type == SessionDataType.PROTOCOLS_PPS:
+            self.data_list = [ProtocolsData(d) for d in props.get('data')]
+        elif self.data_type == SessionDataType.CALL_QUALITY:
+            self.data_list = [CallQualityData(d) for d in props.get('data')]
+        elif self.data_type == SessionDataType.CALL_UTILIZATION:
+            self.data_list = [CallUtilizationData(d) for d in props.get('data')]
+        elif self.data_type == SessionDataType.WIRELESS_PACKETS:
+            self.data_list = [WirelessData(d) for d in props.get('data')]
+        elif self.data_type == SessionDataType.WIRELESS_RETRIES:
+            self.data_list = [WirelessData(d) for d in props.get('data')]
+        elif self.data_type == SessionDataType.APPLICATIONS_MBPS:
+            self.data_list = [ApplicationsData(d) for d in props.get('data')]
+        elif self.data_type == SessionDataType.APPLICATIONS_PPS:
+            self.data_list = [ApplicationsData(d) for d in props.get('data')]
+        else:
+            raise ValueError('Invalid data_type')
 
 
 class SessionStatistics(object):
+    """A SessionStatistics object.
+    """
+
     _session = None
+    """The CaptureSession object the statistics belong to."""
+
     statistics_type = None
+    """The type of statistics."""
+
     start_time = None
+    """The timestamp of when the CaptureSession began."""
+
     end_time = None
+    """"The timestamp of when the CaptureSession ended."""
+
     total_bytes = None
+    """The total number of bytes in the CaptureSession."""
+
     entry_list = None
+    """The list of statistics objects of the CaptureSession."""
 
     def __init__(self, session, statistics_type, props):
         self._session = session
         self.statistics_type = statistics_type
         self.start_time = None
         self.end_time = None
         self.total_bytes = None
@@ -375,20 +515,34 @@
         self.start_time = PeekTime(props.get('startTime', 0))
         self.end_time = PeekTime(props.get('endTime', 0))
         self.total_bytes = int(props.get('sampleInterval', 0))
         self.entry_list = [StatisticsEntry(e) for e in props.get('entries')]
 
 
 class StatisticsEntry(object):
+    """A StatisticsEntry object.
+    """
+
     entry = ''
+    """A CaptureSession Statistics Entry object."""
+
     name = ''
+    """"The name of the StatisticsEntry."""
+
     color = 0
+    """"The color of the StatisticsEntry."""
+
     bytes = 0
+    """"The number of byte of traffic data in the StatisticsEntry."""
+
     pct = 0.0
+    """The pct of the StatisticsEntry."""
+
     total_bytes = None
+    """The total number of bytes of traffic in the StatisticsEntry."""
 
     def __init__(self, props):
         self.entry = ''
         self.name = ''
         self.color = 0
         self.bytes = 0
         self.pct = 0.0
@@ -399,15 +553,16 @@
             self.color = int(props.get('color', '0').strip('#'), 16)
             self.bytes = int(props.get('bytes', 0))
             self.pct = float(props.get('pct', 0.0))
             self.total_bytes = int(props.get('totalBytes', 0))
 
 
 class CaptureSession(object):
-    """Information about a Capture Session."""
+    """Information about a Capture Session.
+    """
 
     _engine = None
     """The engine this capture belongs to."""
 
     adapter_address = ''
     """The Ethernet address of the adapter."""
 
@@ -531,28 +686,27 @@
         self.packet_count = CaptureSession.packet_count
         self.session_id = CaptureSession.session_id
         self.session_start_time = CaptureSession.session_start_time
         self.start_time = CaptureSession.start_time
         self.storage_units = CaptureSession.storage_units
         self.stop_time = CaptureSession.stop_time
         self.total_byte_count = CaptureSession.total_byte_count
-        self.total_dropped_packet_count = \
-            CaptureSession.total_dropped_packet_count
+        self.total_dropped_packet_count = CaptureSession.total_dropped_packet_count
         self.total_packet_count = CaptureSession.total_packet_count
         self._load(props)
 
     def __str__(self):
         return f'CaptureSession: {self.name if self.name else ""}'
 
     def _load(self, props):
         """Load the CaptureSession information from the row of an
         :class:`OmniDataTable <omniscript.omnidatatabel.OmniDataTable>`.
         """
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 a = CaptureSession._capture_session_prop_dict.get(k)
                 if a is not None and hasattr(self, a):
                     if isinstance(getattr(self, a), six.string_types):
                         setattr(self, a, v if v else '')
                     elif isinstance(getattr(self, a), int):
                         setattr(self, a, int(v) if v else 0)
                     elif getattr(self, a) is None:
@@ -561,63 +715,64 @@
                         elif (a == 'session_start_time'
                               or a == 'start_time'
                               or a == 'stop_time'):
                             setattr(self, a, PeekTime(v))
 
     def _perf(self, msg):
         """Log a performance message."""
-        return self._engine._perf_logger.perf(msg) if self._engine and self._engine._perf_logger else None
+        return (self._engine._perf_logger.perf(msg)
+                if self._engine and self._engine._perf_logger else None)
 
     def get_data(self, data_type):
         """Get the a
         :class:`CaptureSession <omniscript.capturesession.CaptureSession>`.
-        
+
         Returns:
             A
             :class:`CaptureSession <omniscript.capturesession.CaptureSession>`
             object.
         """
         if not self._engine:
             raise ValueError('CaptureSession improperly initialized, no OmniEngine reference.')
 
         if isinstance(data_type, SessionDataType):
             dt = session_data_types[data_type]
         elif isinstance(data_type, int):
             dt = session_data_types[SessionDataType(data_type)]
         elif isinstance(data_type, six):
             dt = data_type.lower()
-            if not dt in session_data_types:
+            if dt not in session_data_types:
                 raise TypeError('The value of data_type is not supported')
         else:
             raise TypeError('data_type is not a supported type')
 
         pr = self._perf('get_capture_session_data')
         cmd = f'capture-sessions/{self.session_id}/{dt}/'
         props = self._engine._issue_command(cmd, pr)
         return SessionData(self, props) if props else None
 
     def get_statistics(self, statistics_type, start, end):
         """Get the a statistics from the Capture Session of the type
         specified.
-        
+
         Returns:
             A
             :class:`SessionStatistics <omniscript.capturesession.SessionStatistics>`
             object.
         """
         if not self._engine:
             raise ValueError('CaptureSession improperly initialized, no OmniEngine reference.')
 
         if isinstance(statistics_type, SessionStatisticsType):
             st = session_statistics_types[statistics_type]
         elif isinstance(statistics_type, int):
             st = session_statistics_types[SessionStatisticsType(statistics_type)]
         elif isinstance(statistics_type, six):
             st = statistics_type.lower()
-            if not st in session_statistics_types:
+            if st not in session_statistics_types:
                 raise TypeError('The value of statistics_type is not supported')
         else:
             raise TypeError('statistics_type is not a supported type')
 
         req_props = {
             'start': start.iso_time(),
             'end': end.iso_time()
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/capturetemplate.py` & `omniscript-liveaction-3.0.49/src/omniscript/capturetemplate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 ﻿"""CaptureTemplate class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 import json
 import six
 import xml.etree.ElementTree as ET
 from enum import Enum
 
 import omniscript
 
-from .invariant import (ADAPTER_TYPE_NIC, ADAPTER_TYPE_FILE, ADAPTER_TYPE_UNKNOWN,
-    SEVERITY_INFORMATIONAL, FILTER_MODE_ACCEPT_MATCHING_ANY, ADAPTER_TYPE_NIC, PROP_BAG_FALSE,
-    PROP_BAG_TRUE)
+from .invariant import (
+    AdapterType, Severity, FILTER_MODE_ACCEPT_MATCHING_ANY, PROP_BAG_FALSE, PROP_BAG_TRUE)
 
 from .adapter import Adapter
-# from .alarm import Alarm
-# from .fileadapter import FileAdapter
+from .analysismodule import AnalysisModule
 from .filter import Filter
-from .graphtemplate import GraphTemplate
 from .omniid import OmniId
 from .omnierror import OmniError
 from .peektime import PeekTime
 from .statslimit import StatsLimit
 from .voipsettings import VoIPSettings
 
+from .alarm import find_alarm
+from .analysismodule import find_analysis_module
 from .filter import find_filter
 from .graphtemplate import find_graph_template
 
-
 LOAD_FROM_NONE = 0
 LOAD_FROM_FILE = 1
 LOAD_FROM_NODE = 2
 
 SECONDS_IN_A_MINUTE = 60
 MINUTES_IN_A_HOUR = 60
 SECONDS_IN_A_HOUR = SECONDS_IN_A_MINUTE * MINUTES_IN_A_HOUR
@@ -79,15 +77,22 @@
 _tag_unknown = ''
 
 # JSON Tags
 _json_classid = 'clsid'
 _json_enabled = 'enabled'
 _json_properties = 'properties'
 
-find_attributes = [_tag_name, _tag_id]
+jtrue = 'true'
+jfalse = 'false'
+
+
+def jbool(b):
+    """Returns 'true' if 'b' is True else 'false'."""
+    return jtrue if b else jfalse
+
 
 def _to_interval_units(seconds):
     if (seconds % SECONDS_IN_A_DAY) == 0:
         return ((seconds / SECONDS_IN_A_DAY), GRAPHS_INTERVAL_DAYS)
     if (seconds % SECONDS_IN_A_HOUR) == 0:
         return ((seconds / SECONDS_IN_A_HOUR), GRAPHS_INTERVAL_HOURS)
     if (seconds % SECONDS_IN_A_MINUTE) == 0:
@@ -110,15 +115,15 @@
 
 
 def _find_properties(template):
     """Find the main Property Bag of the Capture Template."""
     # or next(e for e in template.iter() if e.tag == 'properties')
     props = template.find(_tag_props)
     if props is None:
-        #Restart Capture Template File
+        # Restart Capture Template File
         props = template.find('CaptureTemplate/properties')
     return props
 
 
 def _find_property(props, key):
     if props is None:
         return None
@@ -147,17 +152,17 @@
     if not isinstance(value, six.string_types):
         value = str(value)
     prop = _find_property(parent, key)
     if prop is not None:
         prop.text = value
         return
     if key:
-        ET.SubElement(parent, _tag_prop, {_tag_name:key, _tag_type:str(value_type)}).text = value
+        ET.SubElement(parent, _tag_prop, {_tag_name: key, _tag_type: str(value_type)}).text = value
     else:
-        ET.SubElement(parent, _tag_prop, {_tag_type:str(value_type)}).text = value
+        ET.SubElement(parent, _tag_prop, {_tag_type: str(value_type)}).text = value
 
 # def _set_label_clsid(obj, label, clsid_name):
 #     if not _tag_classid in obj.attrib:
 #         class_name_ids = omniscript.get_class_name_ids()
 #         obj.attrib[_tag_classid] = str(class_name_ids[clsid_name])
 #     if not _tag_name in obj.attrib:
 #         obj.attrib[_tag_name] = label
@@ -189,30 +194,30 @@
         'outputExpertLog': _tag_expert_log,
         'outputVoIP': _tag_voip,
         'outputExpertSummary': _tag_expert_summary,
         'outputExecutiveSummary': _tag_executive_summary
     }
 
     def __init__(self):
-        self.option_output_statistics = \
-            AdditionalReportsStatisticsSettings.option_output_statistics
-        self.option_output_statistics = \
-            AdditionalReportsStatisticsSettings.option_output_statistics
-        self.option_conversations_only = \
-            AdditionalReportsStatisticsSettings.option_conversations_only
+        self.option_output_statistics = (
+            AdditionalReportsStatisticsSettings.option_output_statistics)
+        self.option_output_statistics = (
+            AdditionalReportsStatisticsSettings.option_output_statistics)
+        self.option_conversations_only = (
+            AdditionalReportsStatisticsSettings.option_conversations_only)
         self.option_expert_log = AdditionalReportsStatisticsSettings.option_expert_log
         self.option_voip = AdditionalReportsStatisticsSettings.option_voip
         self.option_expert_summary = AdditionalReportsStatisticsSettings.option_expert_summary
-        self.option_executive_summary = \
-            AdditionalReportsStatisticsSettings.option_executive_summary
+        self.option_executive_summary = (
+            AdditionalReportsStatisticsSettings.option_executive_summary)
 
     def _load(self, props, engine):
         """Load the  Statics Settings from a Dictionairy."""
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 a = AdditionalReportsStatisticsSettings._additional_reports_stats_prop_dict.get(k)
                 if a is not None and hasattr(self, a):
                     setattr(self, a, v)
 
 
 class CaptureLimit(object):
     """The Capture Limit of a Trigger Event Object.
@@ -223,35 +228,35 @@
 
     bytes = 0
     """The number of bytes needed to trigger the Trigger."""
 
     enabled = False
     """Is the Capture Limit enabled?"""
 
-    #Tags
+    # Tags
     _json_bytes = 'bytesCaptured'
 
     _tag_class_name = 'BytesCapturedTriggerEvent'
     _tag_bytes = 'bytes'
 
     _capture_limit_prop_dict = {
-        _json_classid : _tag_classid,
-        _tag_enabled : _tag_enabled,
-        _json_bytes : _tag_bytes
+        _json_classid: _tag_classid,
+        _tag_enabled: _tag_enabled,
+        _json_bytes: _tag_bytes
     }
 
     def __init__(self, criteria=None):
         self.bytes = CaptureLimit.bytes
         self.enabled = CaptureLimit.enabled
         self._load(criteria)
 
     def _load(self, props):
         """Load the Capture Limit from a Dictionairy."""
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 a = CaptureLimit._capture_limit_prop_dict.get(k)
                 if a == _tag_classid:
                     self._class_id = OmniId(v)
                 elif a == _tag_enabled:
                     self.enabled = v
                 elif a == CaptureLimit._tag_bytes:
                     self.bytes = int(v)
@@ -263,15 +268,16 @@
         props[CaptureLimit._json_bytes] = self.bytes
         props[_json_enabled] = self.enabled
         props[_json_classid] = _get_class_id(CaptureLimit._tag_class_name)
         return props
 
 
 class DateLimit(object):
-    """The DateLimit of a Trigger Event Object."""
+    """The DateLimit of a Trigger Event Object.
+    """
 
     _class_id = None
     """The Class Identifier of the object."""
 
     elapsed_time = 0
     """The number of nanoseconds"""
 
@@ -287,15 +293,15 @@
 
     option_use_date = False
     """Use the date of the time?"""
 
     option_use_elapsed = False
     """Use the elapsed time?"""
 
-    #Tags
+    # Tags
     _json_elapsed_time = 'elapsedTime'
     _json_time = 'time'
     _json_use_date = 'useDate'
     _json_use_elapsed = 'useElapsedTime'
 
     _tag_class_name = 'TimeTriggerEvent'
     _tag_elapsed_time = 'elapsed_time'
@@ -320,15 +326,15 @@
         self.option_use_date = DateLimit.option_use_date
         self.option_use_elapsed = DateLimit.option_use_elapsed
         self._load(criteria)
 
     def _load(self, props):
         """Load the Date Limit from a Dictionairy."""
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 a = DateLimit._date_limit_prop_dict.get(k)
                 if a == _tag_classid:
                     self._class_id = OmniId(v)
                 elif a == DateLimit._tag_elapsed_time:
                     self.elapsed_time = v
                 elif a == _tag_enabled:
                     self.enabled = v
@@ -365,42 +371,42 @@
     """A list of filter Ids."""
 
     mode = 0
     """The filtering mode of the Filters."""
 
     _filter_ids = []
 
-    #XML Tags
+    # XML Tags
     _json_label = 'filterConfig'
     _json_filters = 'filters'
     _json_mode = 'mode'
 
     _tag_class_name = 'FilterTriggerEvent'
     _tag_filters = 'filters'
     _tag_mode = 'mode'
 
     _filter_limit_prop_dict = {
-        _json_classid : _tag_classid,
-        _tag_enabled : _tag_enabled,
-        _json_filters : _tag_filters,
-        _json_mode : _tag_mode
+        _json_classid: _tag_classid,
+        _tag_enabled: _tag_enabled,
+        _json_filters: _tag_filters,
+        _json_mode: _tag_mode
     }
 
     def __init__(self, criteria=None, engine=None):
         self.enabled = FilterLimit.enabled
         self.filters = []
         self.mode = FilterLimit.mode
         self._filter_ids = []
         self._load(criteria, engine)
 
     def _load(self, props, engine):
         """Load the Date Limit from a Dictionairy."""
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             a = FilterLimit._filter_limit_prop_dict.get(k)
             if a == _tag_classid:
                 self._class_id = OmniId(v)
             elif a == _tag_enabled:
                 self.enabled = v
             elif a == FilterLimit._tag_filters:
                 if isinstance(v, list):
@@ -445,15 +451,15 @@
         self.option_flows = ExpertStatisticsSettings.option_flows
         self.option_applications = ExpertStatisticsSettings.option_applications
 
     def _load(self, props, engine):
         """Load the Expert Statics Settings from a Dictionairy."""
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             a = ExpertStatisticsSettings._expert_stats_prop_dict.get(k)
             if a is not None and hasattr(self, a):
                 setattr(self, a, v)
 
 
 class GraphsStatisticsSettings(object):
     """The Graphs Statistics Settings of an
@@ -472,15 +478,15 @@
     def __init__(self):
         self.option_output_graphs = GraphsStatisticsSettings.option_output_graphs
 
     def _load(self, props, engine):
         """Load the Graphs Statics Settings from a Dictionairy."""
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             a = GraphsStatisticsSettings._graphs_stats_prop_dict.get(k)
             if a is not None and hasattr(self, a):
                 setattr(self, a, v)
 
 
 class NodeStatisticsSettings(object):
     """The Node Statistics Settings of an
@@ -568,18 +574,20 @@
         self.option_type_ip = NodeStatisticsSettings.option_type_ip
         self.option_type_ipv6 = NodeStatisticsSettings.option_type_ipv6
         self.option_type_dec = NodeStatisticsSettings.option_type_dec
         self.option_type_apple = NodeStatisticsSettings.option_type_apple
         self.option_type_ipx = NodeStatisticsSettings.option_type_ipx
 
     def _load(self, props, engine):
-        """Load the Node Statics Settings from a Dictionairy."""
+        """Load the Node Statics Settings from a Dictionairy.
+        """
+
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             a = NodeStatisticsSettings._node_stats_prop_dict.get(k)
             if a is not None and hasattr(self, a):
                 setattr(self, a, v)
                 # if a == NodeStatisticsSettings._tag_output_statistics:
                 #     self.option_output_statistics = v
                 # elif a == NodeStatisticsSettings.option_output_details:
                 #     self.option_output_details = v
@@ -644,15 +652,15 @@
         self.option_packets = ProtocolStatisticsSettings.option_packets
         self.option_path = ProtocolStatisticsSettings.option_path
 
     def _load(self, props, engine):
         """Load the Summary Statics Settings from a Dictionairy."""
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             a = ProtocolStatisticsSettings._protocol_stats_prop_dict.get(k)
             if a is not None and hasattr(self, a):
                 setattr(self, a, v)
 
 
 class SummaryStatisticsSettings(object):
     """The Summary Statistics Settings of an
@@ -691,15 +699,15 @@
         self.option_bytes_per_second = SummaryStatisticsSettings.option_bytes_per_second
         self.option_snapshots = SummaryStatisticsSettings.option_snapshots
 
     def _load(self, props, engine):
         """Load the Summary Statics Settings from a Dictionairy."""
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             a = SummaryStatisticsSettings._summary_stats_prop_dict.get(k)
             if a is not None and hasattr(self, a):
                 setattr(self, a, v)
 
 
 class WirelessChannelStatisticsSettings(object):
     """The Wireless Statistics Settings of an
@@ -878,21 +886,21 @@
         self.option_NoisedBmCurrent = WirelessChannelStatisticsSettings._tag_NoisedBmCurrent
         self.option_NoisedBmAverage = WirelessChannelStatisticsSettings._tag_NoisedBmAverage
 
     def _load(self, props, engine):
         """Load the Wireless Statics Settings from a Dictionairy."""
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             a = WirelessChannelStatisticsSettings._wireless_stats_prop_dict.get(k)
             if a is not None and hasattr(self, a):
                 self.setattr(self, a, v)
 
 
-class  WirelessDataRatesStatisticsSettings(object):
+class WirelessDataRatesStatisticsSettings(object):
     """The Wireless Data Rates Statistics Settings of an
     StatisticsOutputPreferencesSettings Object.
     """
 
     option_output_statistics = False
     option_packets = False
     option_bytes = False
@@ -905,24 +913,24 @@
     _wireless_data_rates_stats_prop_dict = {
         'outputDataRates': _tag_output_statistics,
         'dataRatesPackets': _tag_packets,
         'dataRatesBytes': _tag_bytes
     }
 
     def __init__(self):
-        self.option_output_statistics = \
-            WirelessDataRatesStatisticsSettings.option_output_statistics
+        self.option_output_statistics = (
+            WirelessDataRatesStatisticsSettings.option_output_statistics)
         self.option_packets = WirelessDataRatesStatisticsSettings.option_packets
         self.option_bytes = WirelessDataRatesStatisticsSettings.option_bytes
 
     def _load(self, props, engine):
         """Load the  Statics Settings from a Dictionairy."""
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             a = WirelessDataRatesStatisticsSettings._wireless_data_rates_stats_prop_dict.get(k)
             if a is not None and hasattr(self, a):
                 setattr(self, a, v)
 
 
 class WLANStatisticsSettings(object):
     """The WLAN Statistics Settings of an
@@ -1117,15 +1125,15 @@
         self.option_associations = WLANStatisticsSettings.option_associations
         self.option_trust = WLANStatisticsSettings.option_trust
 
     def _load(self, props, engine):
         """Load the WLAN Statics Settings from a Dictionairy."""
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             a = WLANStatisticsSettings._wlan_stats_prop_dict.get(k)
             if a is not None and hasattr(self, a):
                 setattr(self, a, v)
 
 
 class AdapterSettings(object):
     """The Adapter Settings section of a
@@ -1146,36 +1154,39 @@
 
     name = None
     """The name (or description) of the adapter."""
 
     speed = 1.0
     """The replay speed multiplier of a file adapter."""
 
-    adapter_type = ADAPTER_TYPE_NIC
+    adapter_type = AdapterType.NIC
     """The type of adapter. One of the ADAPTER TYPE constants."""
 
-    #Tags
+    # Tags
     _json_label = 'adapterSettings'
     _json_class_name = _tag_prop_bag
     _json_enumerator = 'enumerator'
     _json_name = _tag_name
     _json_type = _tag_type
     _json_limit = 'replayLimit'
     _json_mode = 'replayTimeStampMode'
     _json_speed = 'replaySpeed'
 
-    _tag_device_name = 'device_name'
     _tag_adapter_type = 'adapter_type'
+    _tag_as_type = "Type"
+    _tag_device_name = 'device_name'
     _tag_enumerator = 'enumerator'
+    _tag_label = 'AdapterSettings'
     _tag_limit = 'limit'
     _tag_mode = 'mode'
+    _tag_root_name = _tag_props
     _tag_speed = 'speed'
 
     _adapter_prop_dict = {
-        _json_classid : _tag_classid,
+        _json_classid: _tag_classid,
         _json_name: _tag_device_name,
         _json_type: _tag_adapter_type,
         _json_enumerator: _tag_enumerator,
         _json_limit: _tag_limit,
         _json_mode: _tag_mode,
         _json_speed: _tag_speed
     }
@@ -1196,15 +1207,15 @@
         """Return the name as the description of the adapter."""
         return self.name
 
     def _load(self, props):
         """Load the Adapter Settings from a Dictionairy."""
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             a = AdapterSettings._adapter_prop_dict.get(k)
             if a is None or not hasattr(self, a):
                 continue
             if a == _json_classid:
                 self._class_id = OmniId(v)
             elif a == AdapterSettings._tag_device_name:
                 self.device_name = v
@@ -1214,29 +1225,43 @@
                 self.mode = int(v)
             elif a == _tag_name:
                 self.name = v
             elif a == AdapterSettings._tag_speed:
                 self.speed = int(v)
             elif a == AdapterSettings._tag_adapter_type:
                 self.adapter_type = int(v)
-        # if self.adapter_type == ADAPTER_TYPE_FILE:
+        # if self.adapter_type == AdapterType.FILE:
         #     _find_property(props, AdapterSettings._tag_limit)
         #     _find_property(props, AdapterSettings._tag_speed)
         #     _find_property(props, AdapterSettings._tag_mode)
         # prop = _find_property(props, AdapterSettings._tag_as_name)
         # if prop is not None:
         #     self.name = prop.text
 
+    def _load_xml(self, obj):
+        """Load the Adapter Settings from an ETree SubElement."""
+        props = obj.find(AdapterSettings._tag_root_name)
+        prop_type = _find_property(props, AdapterSettings._tag_as_type)
+        if prop_type is not None:
+            self.adapter_type = int(prop_type.text)
+        #     if self.adapter_type == config.ADAPTER_TYPE_FILE:
+        #         _find_property(props, AdapterSettings._tag_limit)
+        #         _find_property(props, AdapterSettings._tag_speed)
+        #         _find_property(props, AdapterSettings._tag_mode)
+        # prop = _find_property(props, AdapterSettings._tag_as_name)
+        # if prop is not None:
+        #     self.name = prop.text
+
     def _store(self, props, engine):
         """Store the Adapter Settings into a dictionary."""
         if not isinstance(props, dict):
             return
         _props = {}
         if engine is not None:
-            if self.adapter_type == ADAPTER_TYPE_FILE:
+            if self.adapter_type == AdapterType.FILE:
                 _props[AdapterSettings._json_name] = self.name
                 _props[AdapterSettings._json_limit] = self.limit
                 _props[AdapterSettings._json_mode] = self.mode
                 _props[AdapterSettings._json_speed] = self.speed
                 _props[AdapterSettings._json_adapter_type] = self.adapter_type
             else:
                 adapter = None
@@ -1244,17 +1269,17 @@
                     adapter = engine.find_adapter(self.name)
                 elif self.device_name is not None:
                     adapter = engine.find_adapter(self.device_name, 'device_name')
 
                 if adapter is None:
                     raise OmniError('Adapter not found')
 
-                _props[AdapterSettings._json_enumerator] = adapter.id
+                _props[AdapterSettings._json_enumerator] = adapter.adapter_id
                 _props[AdapterSettings._json_name] = adapter.name
-                _props[AdapterSettings._json_type] = adapter.type
+                _props[AdapterSettings._json_type] = adapter.adapter_type
         elif self.name is not None:
             _props[AdapterSettings._json_name] = self.name
         _props[_json_classid] = _get_class_id(AdapterSettings._json_class_name)
         props[AdapterSettings._json_label] = _props
 
 
 class AlarmSettings(object):
@@ -1267,108 +1292,132 @@
 
     alarms = []
     """A list of Alarms.
     :class:`Alarm <omniscript.alarm.Alarm>` or
     :class:`OmniId <omniscript.omniid.OmniId>`
     """
 
-    #Tags
+    # Tags
     _json_label = 'alarmConfig'
     _json_class_name = 'AlarmConfig'
     _json_alarms = 'alarms'
 
-    _tag_alarms  = 'alarms'
+    _tag_alarms = 'alarms'
+    _tag_label = 'AlarmConfig'
+
+    _tag_xml_config = "AlarmConfig"
+    _tag_xml_alarm = "Alarm"
+    _tag_xml_alarms = "Alarms"
 
     _alarm_prop_dict = {
-        _json_classid : _tag_classid,
+        _json_classid: _tag_classid,
         _json_alarms: _tag_alarms
     }
 
     def __init__(self):
         self.alarms = AlarmSettings.alarms
 
     def _load(self, props, engine=None):
         """Load the Alarm Settings from a Dictionairy."""
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             a = AlarmSettings._alarm_prop_dict.get(k)
             if a is not None and hasattr(self, a):
                 if a == _tag_classid:
                     self._class_id = OmniId(v)
                 elif a == 'alarms':
                     self.alarms = []
                     for id in v:
                         self.alarms.append(OmniId(id))
 
+    def _load_xml(self, obj, engine=None):
+        """Load the Alarm from an ETree.SubElement."""
+        _config = obj.find(AlarmSettings._tag_xml_config)
+        if _config is not None:
+            alarm_list = None
+            if engine is not None:
+                alarm_list = engine.get_alarm_list()
+            alarms = _config.find(AlarmSettings._tag_xml_alarms)
+            for alarm in alarms.findall(AlarmSettings._tag_xml_alarm):
+                id = OmniId(alarm.attrib[_tag_id])
+                _alarm = None
+                if alarm_list is not None:
+                    _alarm = find_alarm(alarm_list, id)
+                if _alarm is not None:
+                    self.alarms.append(_alarm)
+                else:
+                    self.alarms.append(id)
+
     def _store(self, props):
         """Store the Alarms into a JSON props."""
         if not isinstance(props, dict) or len(self.alarms) == 0:
             return
         _props = {}
         _props[AlarmSettings._tag_alarms] = [a.format() for a in self.alarms]
         _props[_json_classid] = _get_class_id(AlarmSettings._json_class_name)
         props[AlarmSettings._json_label] = _props
 
 
 class AnalysisModules(object):
     """The Analysis Module section of a
     :class:`CaptureTemplate <omniscript.capturetemplate.CaptureTemplate>`
-    All the Analysis Modules installed on the engine and listed in 
+    All the Analysis Modules installed on the engine and listed in
     modules by name and in ids listed by
     :class:`OmniId <omniscript.omniid.OmniId>` will be enabled in the capture.
     """
 
-    _class_id = None
-    """The Class Identifier of the object."""
-
     modules = []
-    """A list of Analysis Module Names."""
-
-    ids = []
-    """A list of :class:`OmniId <omniscript.omniid.OmniId>` of enabled
-    Analysis Modules.
+    """A list of
+    :class:`AnalysisModule <omniscript.analysismodule.AnalysisModule>`
+    objects.
     """
 
     option_enable_all = False
     """When True all of the engine's Analysis Modules will be enabled.
     """
 
-    #Tags
-    _json_label = 'pluginsList'
+    # Tags
     _json_class_name = 'PropertyList'
+    _json_config_class_name = 'PluginsConfig'
+    _json_config_label = 'pluginsConfig'
     _json_ids = 'ids'
+    _json_label = 'pluginsList'
 
     _tag_ids = 'ids'
+    _tag_label = 'PluginsList'
+    _tag_options = 'options'
+    _tag_plugins = 'plugins'
+    _tag_root_name = _tag_props
+
+    _tag_xml_plugin = 'plugin'
+    _tag_xml_plugins = 'plugins'
 
     _analysis_modules_prop_list = {
-        _json_classid : _tag_classid,
-        _tag_props : _tag_ids
+        _json_classid: _tag_classid,
+        _tag_props: _tag_ids
     }
 
     def __init__(self):
         self.modules = []
-        self.ids = []
         self.option_enable_all = AnalysisModules.option_enable_all
 
     def _load(self, props, engine=None):
         """Load the Analysis Modules List from a Dictionairy."""
         self.modules = []
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             a = AnalysisModules._analysis_modules_prop_list.get(k)
             if a is not None and hasattr(self, a):
-                if a == _tag_classid:
-                    self._class_id = OmniId(v)
-                elif a == AnalysisModules._tag_ids:
+                if a == AnalysisModules._tag_ids:
                     for m in v:
                         # {'type': 8, 'value': '{9A138D11-5773-4C77-8DBF-16EAC5EFE083}'}
                         if isinstance(m, dict) and ('value' in m):
-                                self.ids.append(OmniId(m['value']))
+                            self.modules.append(AnalysisModule(id=m['value']))
         # props = obj.find(AnalysisModules._tag_root_name)
         # if props is not None:
         #     for prop in props.findall(_tag_prop):
         #         if OmniId.is_id(prop.text):
         #             id = OmniId(prop.text)
         #             module_name = None
         #             if module_list:
@@ -1383,27 +1432,80 @@
         #                     self.modules.append(module_name)
         #                 else:
         #                     self.ids.append(id)
         #         else:
         #             if prop.text not in self.modules:
         #                 self.modules.append(prop.text)
 
+    def _load_xml(self, obj, engine):
+        """Load the list of Analysis Modules from an ETree.SubElement."""
+        if self.modules is None:
+            self.modules = []
+
+        if 'null' in obj.attrib:
+            null_enabled = obj.attrib['null']
+            if null_enabled:
+                return
+
+        """ Build Analysis Module list """
+        props = obj.find(AnalysisModules._tag_root_name)
+        if props is not None:
+            for prop in props.findall(_tag_prop):
+                if OmniId.is_id(prop.text):
+                    id = OmniId(prop.text)
+                    plugin = find_analysis_module(self.modules, id, 'id')
+                    if plugin is None:
+                        self.modules.append(AnalysisModule(engine, id=id))
+
+    def _load_xml_config(self, obj, engine):
+        props = obj.find(AnalysisModules._tag_xml_plugins)
+        if props is not None:
+            for prop in props.findall(AnalysisModules._tag_xml_plugin):
+                prop_id = prop.attrib.get('clsid')
+                if prop_id:
+                    if OmniId.is_id(prop_id):
+                        id = OmniId(prop_id)
+                        plugin = find_analysis_module(self.modules, id, 'id')
+                        if plugin is None:
+                            plugin = AnalysisModule(engine, id=id)
+                            self.modules.append(plugin)
+                        if plugin is not None:
+                            plugin.set_configuration(prop)
+
     def _store(self, props):
         """Store the Analysis Module list into a JSON props."""
         if not isinstance(props, dict):
             return
         prop_list = [
-            {_tag_type: 8, _tag_value: id.format()} for id in self.ids
+            {
+                _tag_type: 8,
+                _tag_value: str(plugin.id)
+            } for plugin in self.modules
         ]
         _props = {
-            _tag_props: prop_list,
+            AnalysisModules._tag_root_name: prop_list,
             _json_classid: _get_class_id(AnalysisModules._json_class_name)
         }
         props[AnalysisModules._json_label] = _props
 
+        have_config = [m.configuration is not None for m in self.modules]
+        if any(have_config):
+            config_list = [
+                {
+                    _json_classid: str(plugin.id),
+                    _tag_name: plugin.name,
+                    AnalysisModules._tag_options: plugin.get_configuration()
+                } for plugin in self.modules
+            ]
+            config_props = {
+                AnalysisModules._tag_plugins: config_list,
+                _json_classid: _get_class_id(AnalysisModules._json_config_class_name)
+            }
+            props[AnalysisModules._json_config_label] = config_props
+
     def set_all(self, enable=True):
         """Enable or disable enabeling all of the Analysis Modules on
         the Engine.
         """
         self.option_enable_all = enable
 
 
@@ -1473,15 +1575,15 @@
 
     option_wireless_channel = False
     """Is the Wireless Channel Statistics option enabled?"""
 
     option_wireless_node = False
     """Is the Wireless Node Statistics option enabled?"""
 
-    #Tags
+    # Tags
     _json_label = 'performanceConfig'
     _json_class_name = _tag_prop_bag
     _json_alarms = 'alarms'
     _json_analysis_modules = 'analysisModules'
     _json_application = 'applicationStatistics'
     _json_compass = 'compass'
     _json_country = 'countryStatistics'
@@ -1497,38 +1599,56 @@
     _json_top_talker = 'topTalkerStatistics'
     _json_traffic = 'trafficHistoryStatistics'
     _json_voice_video = 'voiceAndVideoAnalysis'
     _json_web = 'webAnalysis'
     _json_wireless_channel = 'wirelessChannelStatistics'
     _json_wireless_node = 'wirelessNodeStatistics'
 
-    _tag_node_limit = "Node Statistics"
-    _tag_detail_limit = "Node/Protocol Detail Statistics"
-    _tag_protocol_limit = "Protocol Statistics"
-    _tag_node = 'node_limit'
-    _tag_node_protocol = 'node_protocol_detail_limit'
-    _tag_protocol = 'protocol_limit'
-    _tag_analysis_modules = 'option_analysis_modules'
     _tag_alarms = 'option_alarms'
+    _tag_analysis_modules = 'option_analysis_modules'
     _tag_application = 'option_application'
     _tag_compass = 'option_compass'
     _tag_country = 'option_country'
+    _tag_detail_limit = "Node/Protocol Detail Statistics"
     _tag_error = 'option_error'
     _tag_expert = 'option_expert'
+    _tag_label = 'PerfConfig'
     _tag_network = 'option_network'
+    _tag_node = 'node_limit'
+    _tag_node_limit = "Node Statistics"
+    _tag_node_protocol = 'node_protocol_detail_limit'
     _tag_passive = 'option_passive_name_resolution'
+    _tag_protocol = 'protocol_limit'
+    _tag_protocol_limit = "Protocol Statistics"
+    _tag_root_name = _tag_props
     _tag_size = 'option_size'
     _tag_summary = 'option_summary'
     _tag_top_talker = 'option_top_talker'
     _tag_traffic = 'option_traffic_history'
     _tag_voice_video = 'option_voice_video'
     _tag_web = 'option_web'
     _tag_wireless_channel = 'option_wireless_channel'
     _tag_wireless_node = 'option_wireless_node'
 
+    _tag_xml_alarms = "Alarms"
+    _tag_xml_analysis_modules = "Analysis Modules"
+    _tag_xml_application_stats = "Application Statistics"
+    _tag_xml_country_stats = "Country Statistics"
+    _tag_xml_detail_limit = "Node/Protocol Detail Statistics"
+    _tag_xml_error_stats = "Error Statistics"
+    _tag_xml_expert = "Expert Analysis"
+    _tag_xml_network_stats = "Network Statistics"
+    _tag_xml_node_limit = "Node Statistics"
+    _tag_xml_protocol_limit = "Protocol Statistics"
+    _tag_xml_size_stats = "Size Statistics"
+    _tag_xml_summary_stats = "Summary Statistics"
+    _tag_xml_top_talker_stats = "Top Talker Statistics"
+    _tag_xml_traffic_stats = "Traffic History Statistics"
+    _tag_xml_voice_video = "Voice and Video Analysis"
+
     _analysis_prop_dict = {
         _json_classid: _tag_classid,
         _json_alarms: _tag_alarms,
         _json_analysis_modules: _tag_analysis_modules,
         _json_application: _tag_application,
         _json_compass: _tag_compass,
         _json_country: _tag_country,
@@ -1573,15 +1693,15 @@
         self.option_wireless_channel = AnalysisSettings.option_wireless_channel
         self.option_wireless_node = AnalysisSettings.option_wireless_node
 
     def _load(self, props, engine=None):
         """Load the Analysis Settings from a Dictionairy."""
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             a = AnalysisSettings._analysis_prop_dict.get(k)
             if a is None or not hasattr(self, a):
                 continue
             if a == _tag_classid:
                 self._class_id = OmniId(v)
             # elif a == AnalysisSettings._tag_node_limit:
             #     self.node_limit = StatsLimit(AnalysisSettings._tag_node_limit)
@@ -1623,23 +1743,75 @@
             elif a == AnalysisSettings._tag_web:
                 self.option_web = v
             elif a == AnalysisSettings._tag_wireless_channel:
                 self.option_wireless_channel = v
             elif a == AnalysisSettings._tag_wireless_node:
                 self.option_wireless_node = v
 
+    def _load_xml(self, obj, engine=None):
+        """Load the Analysis Settings from an ETree.SubElement."""
+        props = obj.find(AnalysisSettings._tag_root_name)
+        if props is not None:
+            for obj in props.findall(_tag_object):
+                objName = obj.attrib[_tag_name]
+                if objName == AnalysisSettings._tag_xml_node_limit:
+                    self.node_limit.parse(obj)
+                elif objName == AnalysisSettings._tag_xml_detail_limit:
+                    self.node_protocol_detail_limit.parse(obj)
+                elif objName == AnalysisSettings._tag_xml_protocol_limit:
+                    self.protocol_limit.parse(obj)
+            for prop in props.findall(_tag_prop):
+                propName = prop.attrib[_tag_name]
+                if propName == AnalysisSettings._tag_xml_alarms:
+                    self.option_alarms = _from_prop_boolean(prop.text)
+                elif propName == AnalysisSettings._tag_xml_analysis_modules:
+                    self.option_analysis_modules = _from_prop_boolean(prop.text)
+                elif propName == AnalysisSettings._tag_xml_application_stats:
+                    self.option_application = _from_prop_boolean(prop.text)
+                elif propName == _tag_compass:
+                    self.option_compass = _from_prop_boolean(prop.text)
+                elif propName == AnalysisSettings._tag_xml_country_stats:
+                    self.option_country = _from_prop_boolean(prop.text)
+                elif propName == AnalysisSettings._tag_xml_error_stats:
+                    self.option_error = _from_prop_boolean(prop.text)
+                elif propName == AnalysisSettings._tag_xml_expert:
+                    self.option_expert = _from_prop_boolean(prop.text)
+                elif propName == AnalysisSettings._tag_xml_network_stats:
+                    self.option_network = _from_prop_boolean(prop.text)
+                elif propName == AnalysisSettings._tag_xml_size_stats:
+                    self.option_size = _from_prop_boolean(prop.text)
+                elif propName == AnalysisSettings._tag_xml_summary_stats:
+                    self.option_summary = _from_prop_boolean(prop.text)
+                elif propName == AnalysisSettings._tag_xml_top_talker_stats:
+                    self.option_top_talker = _from_prop_boolean(prop.text)
+                elif propName == AnalysisSettings._tag_xml_traffic_stats:
+                    self.option_traffic = _from_prop_boolean(prop.text)
+                elif propName == AnalysisSettings._tag_xml_voice_video:
+                    self.option_voice_video = _from_prop_boolean(prop.text)
+                elif propName == AnalysisSettings._tag_node_limit:
+                    self.node_limit = StatsLimit(AnalysisSettings._tag_xml_node_limit)
+                    self.node_limit.enabled = _from_prop_boolean(prop.text)
+                elif propName == AnalysisSettings._tag_xml_detail_limit:
+                    self.node_protocol_detail_limit = StatsLimit(
+                        AnalysisSettings._tag_xml_detail_limit)
+                    self.node_protocol_detail_limit.enabled = _from_prop_boolean(prop.text)
+                elif propName == AnalysisSettings._tag_xml_protocol_limit:
+                    self.protocol_limit = StatsLimit(AnalysisSettings._tag_xml_protocol_limit)
+                    self.protocol_limit.enabled = _from_prop_boolean(prop.text)
+
     def _store(self, props):
         """Store the Analysis Settings into the ETree.SubElement."""
         if not isinstance(props, dict):
             return
         _props = {}
         _props[AnalysisSettings._json_node] = self.node_limit.enabled
         _props[AnalysisSettings._json_protocol] = self.protocol_limit.enabled
         _props[AnalysisSettings._json_node_protocol] = self.protocol_limit.enabled
         _props[AnalysisSettings._json_alarms] = self.option_alarms
+        _props[AnalysisSettings._json_analysis_modules] = self.option_analysis_modules
         _props[AnalysisSettings._json_application] = self.option_application
         _props[AnalysisSettings._json_compass] = self.option_compass
         _props[AnalysisSettings._json_country] = self.option_country
         _props[AnalysisSettings._json_passive] = self.option_passive_name_resolution
         _props[AnalysisSettings._json_error] = self.option_error
         _props[AnalysisSettings._json_expert] = self.option_expert
         _props[AnalysisSettings._json_network] = self.option_network
@@ -1649,25 +1821,25 @@
         _props[AnalysisSettings._json_traffic] = self.option_traffic_history
         _props[AnalysisSettings._json_voice_video] = self.option_voice_video
         _props[AnalysisSettings._json_web] = self.option_web
         _props[AnalysisSettings._json_wireless_channel] = self.option_wireless_channel
         _props[AnalysisSettings._json_wireless_node] = self.option_wireless_node
 #         # If a limit is None or disabled, then set it as a bool property.
 #         if self.node_limit is None or not self.node_limit.enabled:
-#             _set_property(props, AnalysisSettings._tag_node_limit, 22, 
+#             _set_property(props, AnalysisSettings._tag_node_limit, 22,
 #                           _to_prop_boolean(False))
 #         else:
 #             props.append(self.node_limit.to_xml())
 #         if self.node_protocol_detail_limit is None or not self.node_protocol_detail_limit.enabled:
-#             _set_property(props, AnalysisSettings._tag_detail_limit, 22, 
+#             _set_property(props, AnalysisSettings._tag_detail_limit, 22,
 #                           _to_prop_boolean(False))
 #         else:
 #             props.append(self.node_protocol_detail_limit.to_xml())
 #         if self.protocol_limit is None or not self.protocol_limit.enabled:
-#             _set_property(props, AnalysisSettings._tag_protocol_limit, 22, 
+#             _set_property(props, AnalysisSettings._tag_protocol_limit, 22,
 #                           _to_prop_boolean(False))
 #         else:
 #             props.append(self.protocol_limit.to_xml())
         _props[_json_classid] = _get_class_id(AdapterSettings._json_class_name)
         props[AnalysisSettings._json_label] = _props
 
     def set_all(self, enable=True):
@@ -1716,16 +1888,18 @@
     # Tags
     _json_label = 'filterConfig'
     _json_class_name = 'FilterConfig'
     _json_filters = 'filters'
     _json_ids = 'ids'
     _json_mode = 'mode'
 
+    _tag_config = "filterconfig"
     _tag_filters = 'filters'
     _tag_ids = 'ids'
+    _tag_label = 'FilterConfig'
     _tag_mode = 'mode'
 
     _filter_prop_dict = {
         _json_classid: _tag_classid,
         _json_filters: _tag_filters,
         _json_ids: _tag_ids,
         _json_mode: _tag_mode
@@ -1737,29 +1911,47 @@
         self.mode = FilterSettings.mode
 
     def _load(self, props):
         """Load the Filter Settings from a Dictionairy."""
         self.filters = []
         self._filter_ids = []
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 a = FilterSettings._filter_prop_dict.get(k)
                 if a is not None and hasattr(self, a):
                     if a == _tag_classid:
                         self._class_id = OmniId(v)
                     elif a == FilterSettings._tag_filters:
                         if isinstance(v, list):
                             for f in v:
                                 self.ids.append(OmniId(f))
                     elif a == FilterSettings._tag_mode:
                         self.mode = int(v)
         # obj.find(FilterSettings._tag_root_name)
         # """ Build filter_list """
         # pass
 
+    def _load_xml(self, obj):
+        """Load the Filter Settings from an ETree.SubElement."""
+        self.filters = []
+        self._filter_ids = []
+
+        if 'null' in obj.attrib:
+            null_enabled = obj.attrib['null']
+            if null_enabled:
+                return
+
+        config = obj.find(FilterSettings._tag_config)
+        if config:
+            mode = config.attrib.get(FilterSettings._tag_mode)
+            self.mode = int(mode) if mode is not None else FilterSettings.mode
+
+        """ Build filter_list """
+        pass
+
     def _store(self, props, engine):
         """Store the Filter Settings into a JSON props."""
         if not isinstance(props, dict):
             return
         if not self.ids:
             fl = engine.get_filter_list()
             for fn in self.filters:
@@ -1813,23 +2005,23 @@
     id = None
     """The Global Unique Identier of the capture."""
 
     intelligent_ctd_count = 0
     """The ctd intelligent count value."""
 
     keep_last_files_count = 10
-    """The number of files to keep if 
+    """The number of files to keep if
     :func:`option_keep_last_files
     <omniscript.capturetemplate.generalsettings.option_keep_last_files>`
     is enabled.
     Default is 10.
     """
 
     max_file_age = SECONDS_IN_A_DAY
-    """The maximum number of seconds a capture file may be open until 
+    """The maximum number of seconds a capture file may be open until
     a new file is created if
     :func:`option_file_age
     <omniscript.capturetemplate.generalsettings.option_file_age>`
     is enabled. Default is 1 day.
     """
 
     max_total_file_size = 10 * BYTES_IN_A_GIGABYTE
@@ -1927,15 +2119,15 @@
     """Is the option to restrict the maximum amount of diskspace to
     a total of
     :func:`max_total_file_size
     <omniscript.capturetemplate.generalsettings.max_total_file_size>`
     bytes is enabled? Default is False.
     """
 
-    #Tags
+    # Tags
     _json_label = 'generalSettings'
     _json_class_name = _tag_prop_bag
     _json_buffer_size = 'bufferSize'
     _json_id = 'captureId'
     _json_capture_to_disk = 'captureToDisk'
     _json_comment = 'comment'
     _json_continuous_capture = 'continuousCapture'
@@ -1956,49 +2148,84 @@
     _json_voip_stats = 'enableVoIPStats'
     _json_name = 'name'
     _json_owner = 'owner'
     _json_save_as_template = 'saveAsTemplate'
     _json_slice_length = 'sliceLength'
     _json_slicing = 'slicing'
     _json_start_capture = 'startCapture'
-    _json_tap_timestamps = 'tapTimestamps' 
+    _json_tap_timestamps = 'tapTimestamps'
 
     _tag_buffer_size = 'buffer_size'
     _tag_comment = 'comment'
     _tag_directory = 'directory'
     _tag_file_pattern = 'file_pattern'
     _tag_file_size = 'file_size'
     _tag_group_id = 'group_id'
     _tag_group_name = 'group_name'
     _tag_intelligent_count = 'intelligent_ctd_count'
     _tag_keep_last_files_count = 'keep_last_files_count'
+    _tag_label = 'GeneralSettings'
     _tag_max_file_age = 'max_file_age'
     _tag_max_total_file_size = 'max_total_file_size'
     _tag_owner = 'owner'
     _tag_reserved_size = 'reserved_size'
     _tag_slice_length = 'slice_length'
     _tag_tap_timestamps = 'tap_timestamps'
     _tag_capture_to_disk = 'option_capture_to_disk'
     _tag_continuous_capture = 'option_continuous_capture'
     _tag_deduplicate = 'option_deduplicate'
     _tag_file_age = 'option_file_age'
     _tag_intelligent_ctd = 'option_intelligent_ctd'
     _tag_keep_last_files = 'option_keep_last_files'
     _tag_multistream = 'option_multistream'
     _tag_priority_ctd = 'option_priority_ctd'
+    _tag_root_name = _tag_props
     _tag_save_as_template = 'option_save_as_template'
     _tag_slicing = 'option_slicing'
     _tag_spotlight_capture = 'option_spotlight_capture'
     _tag_start_capture = 'option_start_capture'
     _tag_app_stats = 'option_timeline_app_stats'
     _tag_timeline_stats = 'option_timeline_stats'
     _tag_top_stats = 'option_timeline_top_stats'
     _tag_voip_stats = 'option_timeline_voip_stats'
     _tag_total_file_size = 'option_total_file_size'
 
+    _tag_xml_application_stats = "EnableAppStats"
+    _tag_xml_buffer_size = "BufferSize"
+    _tag_xml_capture_id = "CaptureID"
+    _tag_xml_capture_to_disk = "CaptureToDisk"
+    _tag_xml_comment = "Comment"
+    _tag_xml_continuous_capture = "ContinuousCapture"
+    _tag_xml_deduplicate = "Deduplicate"
+    _tag_xml_directory = "CtdDir"
+    _tag_xml_file_age = "CtdUseMaxFileAge"
+    _tag_xml_file_pattern = "CtdFilePattern"
+    _tag_xml_file_size = "CtdFileSize"
+    _tag_xml_group_id = "GroupID"
+    _tag_xml_group_name = "GroupName"
+    _tag_xml_keep_last_files = "CtdKeepLastFiles"
+    _tag_xml_keep_last_files_count = "CtdKeepLastFilesCount"
+    _tag_xml_max_file_age = "CtdMaxFileAge"
+    _tag_xml_max_total_file_size = "CtdMaxTotalFileSize"
+    _tag_xml_multistream = "MultiStream"
+    _tag_xml_gs_name = "Name"
+    _tag_xml_owner = "Owner"
+    _tag_xml_priority_ctd = "CtdPriority"
+    _tag_xml_reserved_size = "CtdReservedSize"
+    _tag_xml_save_as_template = "SaveAsTemplate"
+    _tag_xml_slice_length = "SliceLength"
+    _tag_xml_slicing = "Slicing"
+    _tag_xml_spotlight_capture = "SpotlightCapture"
+    _tag_xml_start_capture = "StartCapture"
+    _tag_xml_tap_timestamps = "TapTimestamps"
+    _tag_xml_timeline_stats = "EnableTimelineStats"
+    _tag_xml_timeline_top_stats = "EnableTopStats"
+    _tag_xml_total_file_size = "CtdUseMaxTotalFileSize"
+    _tag_xml_voip_stats = "EnableVoIPStats"
+
     _general_prop_dict = {
         _json_classid: _tag_classid,
         _json_buffer_size: _tag_buffer_size,
         _json_id: _tag_id,
         _json_capture_to_disk: _tag_capture_to_disk,
         _json_comment: _tag_comment,
         _json_continuous_capture: _tag_continuous_capture,
@@ -2062,30 +2289,30 @@
         self.option_timeline_voip_stats = GeneralSettings.option_timeline_voip_stats
         self.option_total_file_size = GeneralSettings.option_total_file_size
         self.option_spotlight_capture = GeneralSettings.option_spotlight_capture
 
     def _load(self, props):
         """Load the General Settings from a dictionairy."""
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 a = GeneralSettings._general_prop_dict.get(k)
                 if a is None or not hasattr(self, a):
                     continue
                 if a == _tag_classid:
                     self._class_id = OmniId(v)
                 elif a == GeneralSettings._tag_buffer_size:
                     self.buffer_size = int(v)
                 elif a == _tag_id:
                     self.id = OmniId(v)
                 elif a == GeneralSettings._tag_capture_to_disk:
                     self.option_capture_to_disk = v
                 elif a == GeneralSettings._tag_comment:
                     self.comment = v
                 elif a == GeneralSettings._tag_continuous_capture:
-                    self.option_continuous_capture =  v
+                    self.option_continuous_capture = v
                 elif a == GeneralSettings._tag_deduplicate:
                     self.option_deduplicate = v
                 elif a == GeneralSettings._tag_directory:
                     self.directory = v
                 elif a == GeneralSettings._tag_file_age:
                     self.option_file_age = v
                 elif a == GeneralSettings._tag_file_pattern:
@@ -2133,14 +2360,86 @@
                 elif a == GeneralSettings._tag_top_stats:
                     self.option_timeline_top_stats = v
                 elif a == GeneralSettings._tag_total_file_size:
                     self.option_total_file_size = v
                 elif a == GeneralSettings._tag_voip_stats:
                     self.option_timeline_voip_stats = v
 
+    def _load_xml(self, obj):
+        """Load the General Settings from an ETree.SubElement."""
+        props = obj.find(GeneralSettings._tag_root_name)
+        if props is not None:
+            for prop in props.findall(_tag_prop):
+                propName = prop.attrib[_tag_name]
+                if propName == GeneralSettings._tag_buffer_size:
+                    self.buffer_size = int(prop.text)
+                elif propName == GeneralSettings._tag_xml_capture_id:
+                    self.id = OmniId(prop.text)
+                elif propName == GeneralSettings._tag_xml_capture_to_disk:
+                    self.option_capture_to_disk = _from_prop_boolean(prop.text)
+                elif propName == GeneralSettings._tag_xml_comment:
+                    self.comment = prop.text
+                elif propName == GeneralSettings._tag_xml_continuous_capture:
+                    self.option_continuous_capture = \
+                        _from_prop_boolean(prop.text)
+                elif propName == GeneralSettings._tag_xml_deduplicate:
+                    self.option_deduplicate = _from_prop_boolean(prop.text)
+                elif propName == GeneralSettings._tag_xml_directory:
+                    self.directory = prop.text
+                elif propName == GeneralSettings._tag_xml_file_age:
+                    self.option_file_age = _from_prop_boolean(prop.text)
+                elif propName == GeneralSettings._tag_xml_file_pattern:
+                    self.file_pattern = prop.text
+                elif propName == GeneralSettings._tag_xml_file_size:
+                    self.file_size = int(prop.text)
+                elif propName == GeneralSettings._tag_xml_group_id:
+                    self.group_id = OmniId(prop.text)
+                elif propName == GeneralSettings._tag_xml_group_name:
+                    self.group_name = prop.text
+                elif propName == GeneralSettings._tag_xml_keep_last_files:
+                    self.option_keep_last_files = _from_prop_boolean(prop.text)
+                elif propName == GeneralSettings._tag_xml_keep_last_files_count:
+                    self.keep_last_files_count = int(prop.text)
+                elif propName == GeneralSettings._tag_xml_max_file_age:
+                    self.max_file_age = int(prop.text)
+                elif propName == GeneralSettings._tag_xml_max_total_file_size:
+                    self.max_total_file_size = int(prop.text)
+                elif propName == GeneralSettings._tag_xml_multistream:
+                    self.option_multistream = _from_prop_boolean(prop.text)
+                elif propName == GeneralSettings._tag_xml_gs_name:
+                    self.name = prop.text
+                elif propName == GeneralSettings._tag_xml_owner:
+                    self.owner = prop.text
+                elif propName == GeneralSettings._tag_xml_priority_ctd:
+                    self.option_priority_ctd = _from_prop_boolean(prop.text)
+                elif propName == GeneralSettings._tag_xml_reserved_size:
+                    self.reserved_size = int(prop.text)
+                elif propName == GeneralSettings._tag_xml_save_as_template:
+                    self.option_save_as_template = _from_prop_boolean(prop.text)
+                elif propName == GeneralSettings._tag_xml_slice_length:
+                    self.slice_length = int(prop.text)
+                elif propName == GeneralSettings._tag_xml_spotlight_capture:
+                    self.option_spotlight_capture = _from_prop_boolean(prop.text)
+                elif propName == GeneralSettings._tag_xml_slicing:
+                    self.option_slicing = _from_prop_boolean(prop.text)
+                elif propName == GeneralSettings._tag_xml_start_capture:
+                    self.option_start_capture = _from_prop_boolean(prop.text)
+                elif propName == GeneralSettings._tag_xml_tap_timestamps:
+                    self.tap_timestamps = int(prop.text)
+                elif propName == GeneralSettings._tag_xml_timeline_stats:
+                    self.option_timeline_stats = _from_prop_boolean(prop.text)
+                elif propName == GeneralSettings._tag_xml_application_stats:
+                    self.option_timeline_app_stats = _from_prop_boolean(prop.text)
+                elif propName == GeneralSettings._tag_xml_timeline_top_stats:
+                    self.option_timeline_top_stats = _from_prop_boolean(prop.text)
+                elif propName == GeneralSettings._tag_xml_total_file_size:
+                    self.option_total_file_size = _from_prop_boolean(prop.text)
+                elif propName == GeneralSettings._tag_xml_voip_stats:
+                    self.option_timeline_voip_stats = _from_prop_boolean(prop.text)
+
     def _store(self, props, new):
         """Store the General Settings into the ETree.SubElement."""
         if not isinstance(props, dict):
             return
         if new:
             self.id = OmniId(True)
         _props = {}
@@ -2187,18 +2486,18 @@
     :class:`CaptureTemplate <omniscript.capturetemplate.CaptureTemplate>`
     """
 
     _class_id = None
     """The Class Identifier of the object."""
 
     graphs = []
-    """A list of 
+    """A list of
     :class:`GraphTemplate <omniscript.graphtemplate.GraphTemplate>`,
     or OmniId or OmniId as a string.
-    
+
     The function :func:`get_graph_template_list()
     <omniscript.omniengine.OmniEngine.get_graph_template_list>`
     returns a list of GraphTemplate objects.
     """
 
     enabled = False
     """Are graphs enabled."""
@@ -2211,37 +2510,48 @@
     file_buffer_size = 50
 
     hours_to_keep = 1
     """Keep most recent in hours."""
 
     option_preserve_files = False
 
-    #XML Tags
+    # XML Tags
     _json_label = 'graphSettings'
     _json_class_name = 'GraphSettings'
     _json_graphs = 'graphs'
     _json_interval = 'interval'
     _json_interval_units = 'intervalUnit'
     _json_file_count = 'fileCount'
     _json_file_buffer_size = 'fileBufferSize'
     _json_hours_to_keep = 'hoursToKeep'
     _json_memory = 'memory'
     _json_preserve_files = 'preserveFiles'
     _json_templates = 'templates'
 
+    _tag_file_buffer_size = 'file_buffer_size'
+    _tag_file_count = 'file_count'
     _tag_graphs = 'graphs'
+    _tag_hours_to_keep = 'hours_to_keep'
     _tag_interval = 'interval'
     _tag_interval_units = 'interval_units'
-    _tag_file_count = 'file_count'
-    _tag_file_buffer_size = 'file_buffer_size'
-    _tag_hours_to_keep = 'hours_to_keep'
+    _tag_label = 'GraphSettings'
     _tag_memory = 'memory'
     _tag_preserve_files = 'option_preserve_files'
     _tag_templates = 'templates'
 
+    _tag_xml_graphdata = "graphdata"
+    _tag_xml_interval = "Interval"
+    _tag_xml_file_count = "FileCnt"
+    _tag_xml_file_buffer_size = "FileBufferSize"
+    _tag_xml_preserve_files = "PreserveFiles"
+    _tag_xml_hours_to_keep = "memory"
+    _tag_xml_templates = "templates"
+    _tag_xml_template = "template"
+    _tag_xml_units = "IntervalUnit"
+
     _graphs_prop_dict = {
         _json_classid: _tag_classid,
         _json_enabled: _tag_enabled,
         _json_file_buffer_size: _tag_file_buffer_size,
         _json_file_count: _tag_file_count,
         _json_interval: _tag_interval,
         _json_interval_units: _tag_interval_units,
@@ -2258,28 +2568,29 @@
         self.file_count = GraphsSettings.file_count
         self.file_buffer_size = GraphsSettings.file_buffer_size
         self.hours_to_keep = GraphsSettings.hours_to_keep
         self.option_preserve_files = GraphsSettings.option_preserve_files
 
     def _load(self, props, engine=None):
         """Load the Graph Settings from a Dictionairy."""
-        _interval = 1
-        _interval_units = 1
+        # TODO: Implement this.
+        # _interval = 1
+        # _interval_units = 1
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 a = GraphsSettings._graphs_prop_dict.get(k)
                 if a is not None and hasattr(self, a):
                     if a == _tag_classid:
                         self._class_id = OmniId(v)
                     elif a == _tag_enabled:
                         self.enabled = v
-                    elif a == GraphsSettings._tag_interval:
-                        _interval = int(v)
-                    elif a == GraphsSettings._tag_interval_units:
-                        _interval_unit = int(v)
+                    # elif a == GraphsSettings._tag_interval:
+                    #     _interval = int(v)
+                    # elif a == GraphsSettings._tag_interval_units:
+                    #     _interval_units = int(v)
                     elif a == GraphsSettings._tag_file_count:
                         self.file_count = int(v)
                     elif a == GraphsSettings._tag_file_buffer_size:
                         self.file_buffer_size = int(v)
                     elif a == GraphsSettings._tag_hours_to_keep:
                         self.hours_to_keep = int(v)
                     elif a == GraphsSettings._tag_preserve_files:
@@ -2296,14 +2607,47 @@
         #             self.graphs.append(template)
         #         # else:
         #         #     name = id
         # if (_units < GRAPHS_INTERVAL_SECONDS) or (_units > GRAPHS_INTERVAL_DAYS):
         #     _units = GRAPHS_INTERVAL_SECONDS
         # self.interval = _interval * interval_multiplier[_units]
 
+    def _load_xml(self, obj, engine=None):
+        """Load the Graph Settings from an ETree.SubElement."""
+        graph_data = obj.find(GraphsSettings._tag_xml_graphdata)
+        self.enabled = _is_attribute_enabled(graph_data, _tag_alt_enabled)
+        self.file_count = int(graph_data.attrib.get(
+            GraphsSettings._tag_xml_file_count, str(GraphsSettings.file_count)))
+        self.file_buffer_size = int(graph_data.attrib.get(
+            GraphsSettings._tag_xml_file_buffer_size, str(GraphsSettings.file_buffer_size)))
+        self.hours_to_keep = int(graph_data.attrib.get(
+            GraphsSettings._tag_xml_hours_to_keep, str(GraphsSettings.hours_to_keep)))
+        self.option_preserve_files = _is_attribute_enabled(
+            graph_data, GraphsSettings._tag_xml_preserve_files)
+        _interval = int(graph_data.attrib.get(
+            GraphsSettings._tag_xml_interval, str(GraphsSettings.interval)))
+        _units = int(graph_data.attrib.get(GraphsSettings._tag_xml_units, '1'))
+
+        graph_template_list = []
+        if engine is not None:
+            graph_template_list = engine.get_graph_template_list()
+        if graph_data is not None:
+            templates = graph_data.find(GraphsSettings._tag_xml_templates)
+            for template in templates.findall(GraphsSettings._tag_xml_template):
+                id = OmniId(template.attrib[_tag_id])
+                template = find_graph_template(graph_template_list, id, 'id')
+                if template:
+                    self.graphs.append(template)
+                # else:
+                #     name = id
+
+        if (_units < GRAPHS_INTERVAL_SECONDS) or (_units > GRAPHS_INTERVAL_DAYS):
+            _units = GRAPHS_INTERVAL_SECONDS
+        self.interval = _interval * interval_multiplier[_units]
+
     def _store(self, props):
         """Store the Graphs Data in a JSON props."""
         if not isinstance(props, dict) or not self.enabled:
             return
         _interval, _units = _to_interval_units(self.interval)
         _props = {}
         _props[_json_enabled] = self.enabled
@@ -2323,15 +2667,15 @@
     """
 
     _class_id = OmniId('6F3377D6-FBD7-4CBD-A740-2EAE63DBF639')
     """The Class Identifier of the object."""
 
     profile_list = []
 
-    #Tags
+    # Tags
     _json_label = 'hardwareConfig'
     _json_class_name = 'HardwareConfig'
     _json_profile_list = 'hardwareProfiles'
 
     _tag_profile_list = 'profile_list'
 
     _hardware_prop_dict = {
@@ -2342,15 +2686,15 @@
     def __init__(self):
         self._class_id = None
         self.profile_list = []
 
     def _load(self, props, engine=None):
         """Load the Hardware Configuration from a Dictionairy."""
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 a = HardwareConfig._hardware_prop_dict.get(k)
                 if a is not None and hasattr(self, a):
                     if a == _tag_classid:
                         self._class_id = OmniId(v)
                     elif a == 'profiles':
                         for p in v:
                             self.profile_list.append(OmniId(p))
@@ -2396,19 +2740,22 @@
 
     option_protospec = False
     """Is Protospec indexing enabled?"""
 
     option_vlan = False
     """Is VLAN indexing enabled?"""
 
-    #Tags
+    # Tags
     _json_label = 'indexingSettings'
     _json_class_name = 'PropertyList'
 
-    #Options list of tuples(attribute, name)
+    _tag_label = 'IndexingSettings'
+    _tag_root_name = _tag_props
+
+    # Options list of tuples(attribute, name)
     _options = [
         ('option_ipv4', 'Indexing IPv4'),
         ('option_ipv6', 'Indexing IPv6'),
         ('option_ethernet', 'Indexing Ethernet'),
         ('option_port', 'Indexing Port'),
         ('option_protospec', 'Indexing Protospec'),
         ('option_application', 'Indexing Application'),
@@ -2432,32 +2779,48 @@
         self.option_port = IndexingSettings.option_port
         self.option_protospec = IndexingSettings.option_protospec
         self.option_vlan = IndexingSettings.option_vlan
 
     def _load(self, props):
         """Load the Indexing Settings from a Dictionairy."""
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 a = IndexingSettings._indexing_prop_dict.get(k)
                 if a == _tag_classid:
                     self._class_id = OmniId(v)
                 elif a == _tag_props:
                     for p in v:
                         if isinstance(p, dict) and (_tag_value in p):
-                            i = int(p[_tag_value])
+                            # TODO: implement this.
+                            # i = int(p[_tag_value])
                             pass
         # self.set_all(False)
         # props = obj.find(IndexingSettings._tag_root_name)
         # if props is not None:
         #     for prop in props.findall(_tag_prop):
         #         _index = int(prop.text)
-        #         if _index < len(IndexingSettings._options) and \
-        #                 hasattr(self, IndexingSettings._options[_index]):
+        #         if (_index < len(IndexingSettings._options)
+        #             and hasattr(self, IndexingSettings._options[_index])):
         #             setattr(self, IndexingSettings._options[_index], True)
 
+    def _load_xml(self, obj):
+        """Load the Indexing Settings from an ETree.SubElement."""
+        if 'null' in obj.attrib:
+            null_enabled = obj.attrib['null']
+            if null_enabled:
+                return
+        self.set_all(False)
+        props = obj.find(IndexingSettings._tag_root_name)
+        if props is not None:
+            for prop in props.findall(_tag_prop):
+                _index = int(prop.text)
+                if _index < len(IndexingSettings._options) and \
+                        hasattr(self, IndexingSettings._options[_index]):
+                    setattr(self, IndexingSettings._options[_index], True)
+
     def _store(self, props):
         """Store the Indexing Data in a JSON props."""
         if not isinstance(props, dict):
             return
         _props = {}
         _props[_tag_props] = []
         if self.option_ipv4:
@@ -2542,15 +2905,15 @@
 
     option_keep_files = False
     """Is the keep files option enabled?"""
 
     option_reset_output = False
     """Is the reset output option enabled?"""
 
-    #Tags
+    # Tags
     _json_label = 'statsOutput'
     _json_class_name = 'StatsOutput'
     _json_files_to_keep = 'keep'
     _json_interval = 'outputInterval'
     _json_interval_units = 'outputIntervalUnit'
     _json_new_set_interval = 'newSetInterval'
     _json_new_set_units = 'newSetIntervalUnit'
@@ -2564,27 +2927,45 @@
     _json_scheduled = 'scheduled'
     _json_keep_files = 'keepFiles'
     _json_reset_output = 'resetOutput'
 
     _tag_files_to_keep = 'files_to_keep'
     _tag_interval = 'interval'
     _tag_interval_units = 'interval_units'
+    _tag_label = 'StatsOutput'
     _tag_new_set_interval = 'new_set_interval'
     _tag_new_set_units = 'new_set_interval_units'
     _tag_report_path = 'report_path'
     _tag_report_type = 'report_type'
     _tag_user_path = 'user_path'
     _tag_notify = 'option_notify'
     _tag_align_new_set = 'option_align_new_set'
     _tag_align_output = 'option_align_output'
     _tag_new_set = 'option_new_set'
     _tag_scheduled = 'option_scheduled'
     _tag_keep_files = 'option_keep_files'
     _tag_reset_output = 'option_reset_output'
 
+    _tag_xml_align_new_set = "alignNewSet"
+    _tag_xml_align_output = "alignOutput"
+    _tag_xml_files_to_keep = "keep"
+    _tag_xml_keep_files = "keepEnabled"
+    _tag_xml_new_set = "newSetEnabled"
+    _tag_xml_new_set_interval = "newSetInterval"
+    _tag_xml_new_set_units = "newSetIntervalUnit"
+    _tag_xml_notify = "notify"
+    _tag_xml_interval = "outputInterval"
+    _tag_xml_report_path = "reportPath"
+    _tag_xml_report_type = "outputType"
+    _tag_xml_reset_output = "ResetOutput"
+    _tag_xml_root_name = "statsoutput"
+    _tag_xml_scheduled = "scheduled"
+    _tag_xml_units = "outputIntervalUnit"
+    _tag_xml_user_path = "userPath"
+
     _statistics_output_prop_dict = {
         _json_classid: _tag_classid,
         _tag_enabled: _tag_enabled,
         _json_files_to_keep: _tag_files_to_keep,
         _json_interval: _tag_interval,
         _json_interval_units: _tag_interval_units,
         _json_new_set_interval: _tag_new_set_interval,
@@ -2620,15 +3001,15 @@
     def _load(self, props):
         """Load the Statistics Output Settings from a Dictionairy."""
         if isinstance(props, dict):
             _interval = 0
             _interval_units = 0
             _new_set_interval = 0
             _new_set_units = 0
-            for k,v in props.items():
+            for k, v in props.items():
                 a = StatisticsOutputSettings._statistics_output_prop_dict.get(k)
                 if a is None or not hasattr(self, a):
                     continue
                 if a == _tag_classid:
                     self._class_id = OmniId(v)
                 elif a == _tag_enabled:
                     self.enabled = v
@@ -2659,20 +3040,66 @@
                 elif a == StatisticsOutputSettings._tag_scheduled:
                     self.option_scheduled = v
                 elif a == StatisticsOutputSettings._tag_keep_files:
                     self.option_keep_files = v
                 elif a == StatisticsOutputSettings._tag_reset_output:
                     self.option_reset_output = v
 
-            if ( (_interval_units < GRAPHS_INTERVAL_SECONDS)
-                 or (_interval_units > GRAPHS_INTERVAL_DAYS) ):
+            if ((_interval_units < GRAPHS_INTERVAL_SECONDS)
+                    or (_interval_units > GRAPHS_INTERVAL_DAYS)):
                 _interval_units = GRAPHS_INTERVAL_SECONDS
             self.interval = _interval * interval_multiplier[_interval_units]
-            if ( (_new_set_units < GRAPHS_INTERVAL_SECONDS)
-                 or (_new_set_units > GRAPHS_INTERVAL_DAYS) ):
+            if ((_new_set_units < GRAPHS_INTERVAL_SECONDS)
+                    or (_new_set_units > GRAPHS_INTERVAL_DAYS)):
+                _new_set_units = GRAPHS_INTERVAL_SECONDS
+            self.new_set_interval = _new_set_interval * interval_multiplier[_new_set_units]
+
+    def _load_xml(self, obj):
+        """Load the Statistics Output Settings from an ETree.SubElement."""
+        settings = obj.find(StatisticsOutputSettings._tag_xml_root_name)
+        if settings is not None:
+            self.enabled = _is_attribute_enabled(settings, StatisticsOutputSettings.enabled)
+            self.files_to_keep = int(settings.attrib.get(
+                StatisticsOutputSettings._tag_xml_files_to_keep,
+                StatisticsOutputSettings.files_to_keep))
+            self.report_path = settings.attrib.get(
+                StatisticsOutputSettings._tag_xml_report_path,
+                StatisticsOutputSettings.report_path)
+            self.report_type = settings.attrib.get(
+                StatisticsOutputSettings._tag_xml_report_type,
+                StatisticsOutputSettings.report_type)
+            self.user_path = settings.attrib.get(
+                StatisticsOutputSettings._tag_xml_user_path,
+                StatisticsOutputSettings.user_path)
+            self.option_notify = _is_attribute_enabled(
+                settings, StatisticsOutputSettings._tag_xml_notify)
+            self.option_align_new_set = _is_attribute_enabled(
+                settings, StatisticsOutputSettings._tag_xml_align_new_set)
+            self.option_align_output = _is_attribute_enabled(
+                settings, StatisticsOutputSettings._tag_xml_align_output)
+            self.option_new_set = _is_attribute_enabled(
+                settings, StatisticsOutputSettings._tag_xml_new_set)
+            self.option_scheduled = _is_attribute_enabled(
+                settings, StatisticsOutputSettings._tag_xml_scheduled)
+            self.option_keep_files = _is_attribute_enabled(
+                settings, StatisticsOutputSettings._tag_xml_keep_files)
+            self.option_reset_output = _is_attribute_enabled(
+                settings, StatisticsOutputSettings._tag_xml_reset_output)
+
+            _interval = int(settings.attrib.get(StatisticsOutputSettings._tag_xml_interval, 1))
+            _units = int(settings.attrib.get(StatisticsOutputSettings._tag_xml_units, 3))
+            if _units < GRAPHS_INTERVAL_SECONDS or _units > GRAPHS_INTERVAL_DAYS:
+                _units = GRAPHS_INTERVAL_SECONDS
+            self.interval = _interval * interval_multiplier[_units]
+
+            _new_set_interval = int(
+                settings.attrib.get(StatisticsOutputSettings._tag_xml_new_set_interval, 1))
+            _new_set_units = int(
+                settings.attrib.get(StatisticsOutputSettings._tag_xml_new_set_units, 4))
+            if _new_set_units < GRAPHS_INTERVAL_SECONDS or _new_set_units > GRAPHS_INTERVAL_DAYS:
                 _new_set_units = GRAPHS_INTERVAL_SECONDS
             self.new_set_interval = _new_set_interval * interval_multiplier[_new_set_units]
 
     def _store(self, props):
         """Store the Statistics Output Settings in a JSON props."""
         if not isinstance(props, dict) or not self.enabled:
             return
@@ -2709,45 +3136,56 @@
 
     enabled = False
     """Are the Statistics Output Preferences Settings enabled?"""
 
     report_type = 3
     """The Report type. One of the REPORT TYPE constances."""
 
-    #Tags
+    # Tags
     _json_label = 'statsOutputPrefs'
     _json_class_name = 'StatsOutputPrefs'
     _json_report_type = 'reportType'
 
+    _tag_label = 'StatsOutputPrefs'
     _tag_report_type = 'report_type'
 
     _stats_out_prefs_prop_dict = {
-          _json_classid: _tag_classid,
+        _json_classid: _tag_classid,
         _tag_enabled: _tag_enabled,
         _json_report_type: _tag_report_type
     }
 
     def __init__(self):
         self.enabled = StatisticsOutputPreferencesSettings.enabled
         self.report_type = StatisticsOutputPreferencesSettings.report_type
 
     def _load(self, props):
         """Load the Statistics Output Preferences Settings from a
         Dictionairy.
         """
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 a = StatisticsOutputPreferencesSettings._stats_out_prefs_prop_dict.get(k)
                 if a == _tag_classid:
                     self._class_id = OmniId(v)
                 elif a == _tag_enabled:
                     self.enabled = v
                 elif a == StatisticsOutputPreferencesSettings._tag_report_type:
                     self.report_type = int(v)
 
+    def _load_xml(self, obj):
+        """Load the Statistics Output Preferences Settings from an ETree.SubElement."""
+        settings = obj.find(StatisticsOutputPreferencesSettings._tag_root_name)
+        if settings is not None:
+            self.enabled = _is_attribute_enabled(settings,
+                                                 StatisticsOutputPreferencesSettings.enabled)
+            self.report_type = int(settings.attrib.get(
+                StatisticsOutputPreferencesSettings._tag_report_type,
+                StatisticsOutputPreferencesSettings.report_type))
+
     def _store(self, props):
         """Store the Statistics Output Preferences Settings in a JSON
         props.
         """
         if not isinstance(props, dict) or not self.enabled:
             return
         _props = {}
@@ -2757,20 +3195,20 @@
         props[StatisticsOutputPreferencesSettings._json_label] = _props
 
 
 class TriggerSettings(object):
     """The Trigger Settings section of a
     :class:`CaptureTemplate <omniscript.capturetemplate.CaptureTemplate>`
     """
- 
+
     class TriggerType(Enum):
         START = 1
         STOP = 2
         REPEAT = 3
-    
+
     _class_id = None
     """The Class Identifier of the object."""
 
     _type = None
     """The type of Trigger: 0: Start, 1: Stop, 3: Repeat"""
 
     captured = None
@@ -2784,15 +3222,15 @@
 
     filter = None
     """The Filter Limit of the Trigger. Initialized to a
     :class:`FilterLimit <omniscript.capturetemplate.FilterLimit>`
     object.
     """
 
-    severity = SEVERITY_INFORMATIONAL
+    severity = Severity.INFORMATIONAL
     """The Severity of the the notification. One of the SEVERITY
     constants
     """
 
     time = None
     """The Date Limit of the Trigger. Initialized to a
     :class:`DateLimit <omniscript.capturetemplate.DateLimit>`
@@ -2807,32 +3245,47 @@
 
     _label = None
     """The label of Trigger: either Start, Stop or Repeat Trigger."""
 
     _label_json = None
     """The json label of Trigger: either Start, Stop or Repeat Trigger."""
 
-    #Tags
+    # Tags
     _json_repeat = 'repeatTrigger'
     _json_start = 'startTrigger'
     _json_stop = 'stopTrigger'
     _json_notify = 'notify'
     _json_severity = 'severity'
     _json_toggle_capture = 'toggleCapture'
     _json_trigger_events = 'triggerEvents'
 
     _tag_class_name = 'Trigger'
+    _tag_label_repeat = 'RepeatTrigger'
+    _tag_label_start = 'StartTrigger'
+    _tag_label_stop = 'StopTrigger'
     _tag_repeat = 'repeat'
     _tag_start = 'start'
     _tag_stop = 'stop'
     _tag_severity = 'severity'
     _tag_trigger_events = 'trigger_events'
     _tag_notify = 'option_notify'
     _tag_toggle_capture = 'option_toggle_capture'
 
+    _tag_xml_events = "triggerevents"
+    _tag_xml_event_obj = "triggereventobj"
+    _tag_xml_notify = "notify"
+    _tag_xml_root_name = "trigger"
+    _tag_xml_severity = "severity"
+    _tag_xml_toggle = "togglecapture"
+
+    # Trigger Event Names
+    _class_bytes_captured = "BytesCapturedTriggerEvent"
+    _class_time = "TimeTriggerEvent"
+    _class_flter = "FilterTriggerEvent"
+
     _trigger_prop_dict = {
         _json_classid: _tag_classid,
         _tag_enabled: _tag_enabled,
         _json_notify: _tag_notify,
         _json_severity: _tag_severity,
         _json_toggle_capture: _tag_toggle_capture,
         _json_trigger_events: _tag_trigger_events
@@ -2860,46 +3313,71 @@
         self.option_toggle_capture = TriggerSettings.option_toggle_capture
         self._label = TriggerSettings._label_tag[trigger_type]
         self._label_json = TriggerSettings._label_json[trigger_type]
 
     def _load(self, props, engine):
         """Load the Trigger Settings from a dictionairy."""
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 a = TriggerSettings._trigger_prop_dict.get(k)
                 if a == _tag_classid:
                     self._class_id = OmniId(v)
                 elif a == _tag_enabled:
                     self.enabled = v
                 elif a == TriggerSettings._tag_severity:
-                    self.severity = v
+                    self.severity = Severity(v) if v in Severity else Severity.INFORMATIONAL
                 elif a == TriggerSettings._tag_notify:
                     self.option_notify = v
                 elif a == TriggerSettings._tag_toggle_capture:
                     self.option_toggle_capture = v
                 elif a == TriggerSettings._tag_trigger_events:
                     if not isinstance(v, list):
                         continue
                     capture_class_id = _get_class_id(CaptureLimit._tag_class_name)
                     date_class_id = _get_class_id(DateLimit._tag_class_name)
                     filter_class_id = _get_class_id(FilterLimit._tag_class_name)
                     for limit in v:
-                            if not isinstance(limit, dict):
-                                continue
-                            class_id = limit.get(_json_classid)
-                            if class_id:
-                                id = OmniId(class_id)
-                                if id == capture_class_id:
-                                    self.captured._load(limit)
-                                elif id == date_class_id:
-                                    self.time._load(limit)
-                                elif id == filter_class_id:
-                                    self.filter._load(limit, engine)
-                                else:
-                                    pass
+                        if not isinstance(limit, dict):
+                            continue
+                        class_id = limit.get(_json_classid)
+                        if class_id:
+                            id = OmniId(class_id)
+                            if id == capture_class_id:
+                                self.captured._load(limit)
+                            elif id == date_class_id:
+                                self.time._load(limit)
+                            elif id == filter_class_id:
+                                self.filter._load(limit, engine)
+                            else:
+                                pass
+
+    def _load_xml(self, obj, engine):
+        """Load the Trigger Settings from an ETree SubElement."""
+        self._name = obj.attrib[_tag_name]
+        trigger = obj.find(TriggerSettings._tag_xml_root_name)
+        self.enabled = _is_prop_enabled(trigger)
+        self.option_notify = _is_attribute_enabled(
+            trigger, TriggerSettings._tag_xml_notify)
+        self.severity = int(trigger.attrib.get(
+            TriggerSettings._tag_xml_severity, str(TriggerSettings.severity)))
+        self.option_toggle_capture = _is_attribute_enabled(
+            trigger, TriggerSettings._tag_xml_toggle)
+        events = trigger.find(TriggerSettings._tag_xml_events)
+        for ev_obj in events.findall(TriggerSettings._tag_xml_event_obj):
+            class_name_ids = omniscript.get_class_name_ids()
+            id = OmniId(ev_obj.attrib.get(_tag_classid))
+            if id == class_name_ids[TriggerSettings._class_bytes_captured]:
+                self.captured = CaptureLimit()
+                self.captured._load(ev_obj)
+            elif id == class_name_ids[TriggerSettings._class_time]:
+                self.time = DateLimit()
+                self.time._load(ev_obj)
+            elif id == class_name_ids[TriggerSettings._class_flter]:
+                self.filter = FilterLimit()
+                self.filter._load(ev_obj, engine)
 
     def _store(self, props, engine):
         """Store the Trigger Settings into the ETree SubElement"""
         if not isinstance(props, dict):
             return
         _props = {}
         _props[_json_enabled] = self.enabled
@@ -3023,20 +3501,21 @@
 
     voip = None
     """The VoIP configuration
     :class:`VoIP Settings <omniscript.capturetemplate.VoIPSettings>`
     object.
     """
 
+    find_attributes = ('name', 'id')
+
     _default_filename = False
     """Is the default capture template being used?"""
 
     _load_from = LOAD_FROM_NONE
 
-
     # Tags
     _json_plugins_config = 'pluginsConfig'
 
     _tag_adapter = 'adapter'
     _tag_template = 'template'
     _tag_alarms = 'alarms'
     _tag_analysis = 'analysis'
@@ -3051,14 +3530,16 @@
     _tag_repeat_trigger = 'repeat_trigger'
     _tag_start_trigger = 'start_trigger'
     _tag_statistics_output = 'statistics_output'
     _tag_statistics_output_preferences = 'statistics_output_preferences'
     _tag_stop_trigger = 'stop_trigger'
     _tag_voip = 'voip'
 
+    _tag_xml_plugins_config = 'PluginsConfig'
+
     _template_prop_dict = {
         _json_classid: _tag_classid,
         AdapterSettings._json_label: _tag_adapter,
         AlarmSettings._json_label: _tag_alarms,
         AnalysisModules._json_label: _tag_plugins,
         AnalysisSettings._json_label: _tag_analysis,
         FilterSettings._json_label: _tag_filter,
@@ -3097,21 +3578,21 @@
         self.start_trigger = TriggerSettings(TriggerSettings.TriggerType.START)
         self.statistics_output = StatisticsOutputSettings()
         self.statistics_output_preferences = StatisticsOutputPreferencesSettings()
         self.stop_trigger = TriggerSettings(TriggerSettings.TriggerType.STOP)
         self.voip = VoIPSettings()
         # if not self.filename:
         #     _dirname = os.path.dirname(omniscript.__file__)
-        #     self.filename = os.path.join(_dirname, '_capture_template.xml')
+        #     self.filename = os.path.join(_dirname, 'data', '_capture_template.xml')
         #     self._default_filename = True
-        # if self.filename is not None:
-        #     tree = ET.parse(self.filename)
-        #     props = _find_properties(tree)
-        #     self._load(props, engine)
-        #     self._load_from = LOAD_FROM_FILE
+        if self.filename is not None:
+            tree = ET.parse(self.filename)
+            file_props = _find_properties(tree)
+            self.load_xml(file_props, engine)
+            self._load_from = LOAD_FROM_FILE
         if props is not None:
             self._load(props, engine)
             self._load_from = LOAD_FROM_NODE
 
     def __repr__(self) -> str:
         return f'CaptureTemplate: {self.general.name} {self.id.format()}'
 
@@ -3124,15 +3605,15 @@
         self.id = OmniId(props['id']) if 'id' in props else None
         self.type = props['type'] if 'type' in props else None
         self.clsid = props[_json_classid] if _json_classid in props else None
         template = (props[CaptureTemplate._tag_template]
                     if CaptureTemplate._tag_template in props
                     else props)
         if isinstance(template, dict):
-            for k,v in template.items():
+            for k, v in template.items():
                 a = CaptureTemplate._template_prop_dict.get(k)
                 if a is None or not hasattr(self, a):
                     continue
                 if a == _tag_classid:
                     self._class_id = OmniId(v)
                 elif a == CaptureTemplate._tag_adapter:
                     self.adapter._load(v)
@@ -3188,30 +3669,71 @@
     #     for item in filters:
     #         if isinstance(item, (list, tuple)):
     #             for f in item:
     #                 self.add_filters(f)
     #         else:
     #             self.add_filter(item)
 
+    def load_xml(self, props, engine):
+        if props is not None:
+            for obj in props.findall(_tag_object):
+                objName = obj.attrib[_tag_name]
+                if objName == AdapterSettings._tag_label:
+                    self.adapter._load_xml(obj)
+                elif objName == AlarmSettings._tag_label:
+                    self.alarms._load_xml(obj)
+                elif objName == AnalysisSettings._tag_label:
+                    self.analysis._load_xml(obj)
+                elif objName == FilterSettings._tag_label:
+                    self.filter._load_xml(obj)
+                elif objName == GeneralSettings._tag_label:
+                    self.general._load_xml(obj)
+                elif objName == GraphsSettings._tag_label:
+                    self.graphs._load_xml(obj)
+                elif objName == IndexingSettings._tag_label:
+                    self.indexing._load_xml(obj)
+                elif objName == AnalysisModules._tag_label:
+                    self.plugins._load_xml(obj, engine)
+                elif objName == AnalysisSettings._tag_label:
+                    self.plugins_config = None
+                elif objName == TriggerSettings._tag_label_start:
+                    if self.start_trigger is None:
+                        self.start_trigger = TriggerSettings(CaptureTemplate._tag_start)
+                    self.start_trigger._load_xml(obj, engine)
+                elif objName == StatisticsOutputSettings._tag_label:
+                    self.statistics_output._load_xml(obj)
+                elif objName == TriggerSettings._tag_label_stop:
+                    if self.stop_trigger is None:
+                        self.stop_trigger = TriggerSettings(CaptureTemplate._tag_stop)
+                    self.stop_trigger._load_xml(obj, engine)
+                elif objName == VoIPSettings.get_label():
+                    self.voip._load_xml(obj)
+                elif objName == CaptureTemplate._tag_xml_plugins_config:
+                    self.plugins._load_xml_config(obj, engine)
+            for prop in props.findall(_tag_prop):
+                propName = prop.attrib[_tag_name]
+                if propName == TriggerSettings._tag_label_repeat:
+                    self.repeat_trigger = int(prop.text)
+
     # def save(self, filename, engine=None):
     #     """Save the capture template to file."""
     #     f = open(filename, 'w')
     #     f.write(self.to_xml(engine, True))   #True: pretty print.
     #     f.close
 
     def set_adapter(self, value):
         """Set the adapter; only it's name/description is stored."""
         if isinstance(value, six.string_types):
-            self.adapter.adapter_type = ADAPTER_TYPE_UNKNOWN
+            self.adapter.adapter_type = AdapterType.UNKNOWN
             self.adapter.name = value
         elif isinstance(value, Adapter):
             self.adapter.adapter_type = value.adapter_type
             self.adapter.name = value.name
         # elif isinstance(value, FileAdapter):
-        #     self.adapter.adapter_type = ADAPTER_TYPE_FILE
+        #     self.adapter.adapter_type = AdapterType.FILE
         #     self.adapter.name = value.filename
         #     self.adapter.limit = value.limit
         #     self.adapter.mode = value.mode
         #     self.adapter.speed = value.speed
 
     def set_all(self, enable=True):
         """Set all analysis options, default is True.
@@ -3224,15 +3746,15 @@
         self.general.set_timeline(enable)
 
     # def set_filters(self, filter_list):
     #     """Set the filters of the capture."""
     #     self.filter.filters = []
     #     self.add_filters(filter_list)
 
-	# def set_multistream(self, enable=False):
+    # def set_multistream(self, enable=False):
     #     """Set the capture multistream."""
     #     self.general.set_multistream(enable)
 
     def set_repeat_trigger(self, value):
         """Set the Repeat Trigger option.
 
         Args:
@@ -3317,22 +3839,20 @@
     #             self.general._store(obj)
     #         elif objName == CaptureTemplate._tag_graphs:
     #             self.graphs._store(obj)
     #         elif objName == CaptureTemplate._tag_indexing:
     #             self.indexing._store(obj)
     #         elif objName == CaptureTemplate._tag_plugins:
     #             self.plugins._store(obj, engine, self.analysis.option_compass)
-    #         elif objName == CaptureTemplate._tag_start and \
-    #                 self.start_trigger is not None:
+    #         elif objName == CaptureTemplate._tag_start and self.start_trigger is not None:
     #             self.start_trigger._store(obj, engine)
-    #         elif objName == CaptureTemplate._tag_stop and \
-    #                 self.stop_trigger is not None:
+    #         elif objName == CaptureTemplate._tag_stop and self.stop_trigger is not None:
     #             self.stop_trigger._store(obj, engine)
     #     if self.repeat_trigger is not None:
-    #         _set_property(props, CaptureTemplate._tag_repeat, 22, 
+    #         _set_property(props, CaptureTemplate._tag_repeat, 22,
     #                 int(self.repeat_trigger))
 
     #     #template = ET.Element('capturetemplate', {'version':'1.0'})
     #     #props = ET.SubElement(template, 'properties')
     #     #self.adapter._store(ET.SubElement(props, 'obj'), engine)
     #     #self.alarms._store(ET.SubElement(props, 'obj'))
     #     #self.analysis._store(ET.SubElement(props, 'obj'))
@@ -3365,17 +3885,18 @@
     templates = resp['templates']
     if templates is not None:
         for props in templates:
             lst.append(CaptureTemplate(None, props, engine))
     # lst.sort(key=lambda x: x.description)
     return lst
 
-def find_capture_template(templates, value, attrib = find_attributes[0]):
+
+def find_capture_template(templates, value, attrib=CaptureTemplate.find_attributes[0]):
     """Finds a Capture Template in the list"""
-    if (not templates) or (attrib not in find_attributes):
+    if (not templates) or (attrib not in CaptureTemplate.find_attributes):
         return None
 
     if len(templates) == 0:
         return None
 
     if isinstance(value, CaptureTemplate):
         _value = value.id
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/country.py` & `omniscript-liveaction-3.0.49/src/omniscript/country.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 """Country class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 
-find_attribs = ['name', 'code']
-
 class Country(object):
-    """An Country object."""
+    """An Country object.
+    """
 
     code = ''
+    """The country code of the Country."""
+
     name = ''
+    """The name of the Country."""
 
     # Tags
     _tag_code = 'code'
     _tag_name = 'name'
 
     def __init__(self, props):
         self.code = Country.code
         self.name = Country.name
         self._load(props)
 
     def _load(self, props):
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 if k == Country._tag_code:
                     self.code = v
                 elif k == Country._tag_name:
                     self.name = v
 
 
 def _create_country_list(props):
@@ -41,15 +43,15 @@
                     lst.append(Country(c))
     return lst
 
 
 def create_country_name_dictionary(countries):
     """Create a diction with the country name as the key
     and the country code as the value.
-    
+
     Input:
         countries as a dictionary of with one element 'countries', a list
         of 'code' and 'name' dictionary elements.
         Or as a list of Country objects.
     """
     dct = {}
     if isinstance(countries, dict):
@@ -63,15 +65,15 @@
             dct[c.name] = c.code
     return dct
 
 
 def create_country_code_dictionary(countries):
     """Create a diction with the country code as the key
     and the country code as the value.
-    
+
     Input:
         countries as a dictionary of with one element 'countries', a list
         of 'code' and 'name' dictionary elements.
         Or as a list of Country objects.
     """
     dct = {}
     if isinstance(countries, dict):
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/data/_capture_template.xml` & `omniscript-liveaction-3.0.49/src/omniscript/data/_capture_template.xml`

 * *Files identical despite different names*

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/data/_capture_template_linux.xml` & `omniscript-liveaction-3.0.49/src/omniscript/data/_capture_template_linux.xml`

 * *Files identical despite different names*

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/data/_capture_template_windows.xml` & `omniscript-liveaction-3.0.49/src/omniscript/data/_capture_template_windows.xml`

 * *Files identical despite different names*

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/data/_class_ids.txt` & `omniscript-liveaction-3.0.49/src/omniscript/data/_class_ids.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 {F2A9D611-F285-4895-8891-104D5937C3CC} CaptureTemplateCollection
 {BD360857-1394-47DD-9E11-340781664ED7} CaptureTemplateItem
 {0FCC314A-DF4F-4535-A69A-5D42B29D7267} ChannelFilterNode
 {1BABAFF2-64C1-4636-AF25-CBF7DA8D8018} ChannelManager
 {9E6F756E-4BE7-4E14-AD2A-72C81C8DDC6C} ChannelStats
 {EF3D3547-AECB-4CCD-A8BE-82E7BBF12AB2} Compass
 {977000CD-2261-4294-963C-AD6FC396C761} Configuration: Configure engine settings
+{B5405600-33F6-4D63-9AA9-30F5DDFDC58B} Configuration: Delete files created by others
 {0D4BE720-1B4D-4FE8-BC99-3C78A8C63971} Configuration: Download files
 {CB24BECC-5E6C-46FB-9E73-903C57706E31} Configuration: Upload files
 {1A6CDC94-4896-42ee-8195-E68B72B050D7} Configuration: View/modify matrix switch settings
 {9482DD9B-6E9B-4595-8F4A-398C7A6BAB20} Configuration: View the audit log
 {5C91C7DE-D4EB-4AC2-84F5-84829A8837BF} ConversationStats
 {0866D6FD-0DBC-47A9-AD9E-927A6489D01C} CountryFilterNode
 {BAC56A49-681B-47EC-81B6-923A9392DFD1} CountryStats
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/data/_co_codes.txt` & `omniscript-liveaction-3.0.49/src/omniscript/data/_co_codes.txt`

 * *Files identical despite different names*

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/data/_expert_problem_ids.txt` & `omniscript-liveaction-3.0.49/src/omniscript/data/_expert_problem_ids.txt`

 * *Files identical despite different names*

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/data/_stat_ids.txt` & `omniscript-liveaction-3.0.49/src/omniscript/data/_stat_ids.txt`

 * *Files identical despite different names*

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/data/expertdescriptions.xml` & `omniscript-liveaction-3.0.49/src/omniscript/data/expertdescriptions.xml`

 * *Files identical despite different names*

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/data/pspecs.xml` & `omniscript-liveaction-3.0.49/src/omniscript/data/pspecs.xml`

 * *Files 8% similar despite different names*

#### Comparing `omniscript-liveaction-3.0.44/src/omniscript/data/pspecs.xml` & `omniscript-liveaction-3.0.49/src/omniscript/data/pspecs.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file should be saved with utf-8 encoding without BOM -->
-<ProtoSpecTable Version="2.4.28">
+<ProtoSpecTable Version="2.4.61">
   <ColorTable>
     <ColorDef Name="none" RGB="0x000000"/>
     <ColorDef Name="1" RGB="0x000055"/>
     <ColorDef Name="2" RGB="0x003f55"/>
     <ColorDef Name="3" RGB="0x843d00"/>
     <ColorDef Name="4" RGB="0x007f00"/>
     <ColorDef Name="5" RGB="0x557f00"/>
@@ -31,14 +31,15 @@
     <Translation From="41" To="38"/>
     <Translation From="42" To="39"/>
     <Translation From="520" To="500"/>
     <Translation From="1455" To="1400"/>
     <Translation From="1465" To="1400"/>
     <Translation From="1469" To="1500"/>
     <Translation From="1481" To="2476"/>
+    <Translation From="1914" To="2390"/>
     <Translation From="4700" To="4500"/>
     <Translation From="2488" To="1400"/>
     <Translation From="2530" To="1479"/>
     <Translation From="6101" To="6100"/>
     <Translation From="6102" To="6100"/>
     <Translation From="6103" To="6100"/>
     <Translation From="6104" To="6100"/>
@@ -218,16 +219,17 @@
       <Desc>VINES is a complete networking implementation sold by Banyan Systems Incorporated. It runs on many different computer platforms. It has multiple layers comprised of packet routing, network, session and application control.</Desc>
       <Color>15</Color>
       <CondSwitch>0x0bad</CondSwitch>
       <CondSwitch>0x80c4</CondSwitch>
       <Link Name="VINES Children"/>
     </PSpec>
     <PSpec Name="PPPoE">
-      <PSpecID>20</PSpecID>
       <NotChild Name="PPPoE"/>
+      <NotChild Name="GENEVE"/>
+      <PSpecID>20</PSpecID>
       <LName>PPP over Ethernet</LName>
       <Desc>The Point-to-Point Protocol (PPP) provides a standard method for transporting multi-protocol datagrams over point-to-point links. PPPoE provides a method for building PPP sessions and encapsulating PPP packets over Ethernet.</Desc>
       <Color>3</Color>
       <CondSwitch>0x8863</CondSwitch>
       <CondSwitch>0x8864</CondSwitch>
       <PSpec Name="Discovery">
         <PSpecID>21</PSpecID>
@@ -511,14 +513,60 @@
       <LName>Media Redundancy Protocol</LName>
       <Desc>Media Redundancy Protocol (IEC62439-2).</Desc>
       <Color>1</Color>
       <ParentSpecific Parent="Ethernet Type 2">
         <CondSwitch>0x88e3</CondSwitch>
       </ParentSpecific>
     </PSpec>
+    <PSpec Name="NHRP">
+      <PSpecID>8331</PSpecID>
+      <LName>NBMA Next Hop Resolution Protocol</LName>
+      <Desc>The Next Hop Resolution Protocol (NHRP) is an extension of the ATM ARP routing mechanism that is sometimes used to improve the efficiency of routing computer network traffic over Non-Broadcast, Multiple Access (NBMA) Networks.</Desc>
+      <Color>13</Color>
+      <ParentSpecific Parent="Ethernet Type 2">
+        <CondSwitch>0x2001</CondSwitch>
+      </ParentSpecific>
+    </PSpec>
+    <PSpec Name="MDP">
+      <PSpecID>8817</PSpecID>
+      <LName>Cisco Meraki Discovery Protocol</LName>
+      <Desc>Cisco Meraki propriatary provisioning protocol for Meraki Access Points.</Desc>
+      <Color>2</Color>
+      <ParentSpecific Parent="Ethernet Type 2">
+        <CondSwitch>0x0712</CondSwitch>
+        <CondSwitch>0x0713</CondSwitch>
+      </ParentSpecific>
+    </PSpec>
+    <PSpec Name="HomePlug AV">
+      <PSpecID>8818</PSpecID>
+      <Desc>HomePlug AV is a subversion of the HomePlug Protocol Family. Some HomePlug specifications target broadband applications via power-line communication technology.</Desc>
+      <Color>3</Color>
+      <ParentSpecific Parent="Ethernet Type 2">
+        <CondSwitch>0x88E1</CondSwitch>
+      </ParentSpecific>
+    </PSpec>
+    <PSpec Name="EtherCAT">
+      <PSpecID>8819</PSpecID>
+      <LName>Ethernet for Control Automation Technology</LName>
+      <Desc>EtherCAT (Ethernet for Control Automation Technology) is an Ethernet-based fieldbus system invented by Beckhoff Automation. The protocol is standardized in IEC 61158 and is suitable for both hard and soft real-time computing requirements in automation technology.</Desc>
+      <Color>1</Color>
+      <ParentSpecific Parent="Ethernet Type 2">
+        <CondSwitch>0x88A4</CondSwitch>
+      </ParentSpecific>
+    </PSpec>
+    <PSpec Name="Palo Alto Heartbeat Backup">
+      <PSpecID>8820</PSpecID>
+      <SName>PAHB</SName>
+      <LName>Palo Alto Heartbeat Backup</LName>
+      <Desc>Palo Alto Heartbeat Backup uses the management ports on the HA devices to provide a backup path for heartbeat and hello messages. The management port IP address will be shared with the HA peer through the HA1 control link.</Desc>
+      <Color>1</Color>
+      <ParentSpecific Parent="Ethernet Type 2">
+        <CondSwitch>0x8988</CondSwitch>
+      </ParentSpecific>
+    </PSpec>
   </PSpec>
   <PSpec Name="IPv6 Children" Type="CommonTable">
     <Switch Name="IP ProtocolID Switch">
       <On>ProtocolID</On>
       <Link Name="IP Children"/>
     </Switch>
   </PSpec>
@@ -761,27 +809,32 @@
         <LName>IP EIGRP Ack</LName>
         <SName>EIGRP Ack</SName>
         <Desc>EIGRP Ack. They are unicast, and use unreliable delivery.</Desc>
         <CondExp><![CDATA[(MLD8[1] == 5) && (MLD32[12] != 0)]]></CondExp>
       </PSpec>
     </PSpec>
     <PSpec Name="SCTP">
+      <NotChild Name="IPv6"/>
+      <NotChild Name="IPinIP"/>
+      <NotChild Name="GRE"/>
+      <NotChild Name="GTP"/>
+      <NotChild Name="GENEVE"/>
       <PSpecID>1900</PSpecID>
       <LName>Stream Control Transmission Protocol</LName>
       <Desc>The basic service offered by SCTP is the reliable transfer of user messages between peer SCTP users. It performs this service within the context of an association between two SCTP endpoints.</Desc>
       <Color>7</Color>
       <CondSwitch>132</CondSwitch>
       <Definitions>
         <Define>
           <Name>SrcPort</Name>
-          <Value><![CDATA[PLD16[0]]]></Value>
+          <Value><![CDATA[MLD16[0]]]></Value>
         </Define>
         <Define>
           <Name>DestPort</Name>
-          <Value><![CDATA[PLD16[2]]]></Value>
+          <Value><![CDATA[MLD16[2]]]></Value>
         </Define>
       </Definitions>
       <NextLayer>
         <Exp><![CDATA[12]]></Exp>
       </NextLayer>
       <Link Name="SCTP Chunks"/>
     </PSpec>
@@ -804,19 +857,26 @@
           <Value><![CDATA[PLD16[2]]]></Value>
         </Define>
       </Definitions>
       <Switch Name="TCP Port Switch">
         <On>SrcPort</On>
         <On>DestPort</On>
         <Link Name="TCP/UDP" Sort="Last"/>
+        <PSpec Name="Firebird">
+          <PSpecID>3050</PSpecID>
+          <LName>Firebird Database</LName>
+          <Desc>Firebird Database protocol is used to communicate with the Open Source Firebird Database Server.</Desc>
+          <Color>14</Color>
+          <CondSwitch>3050</CondSwitch>
+        </PSpec>
         <PSpec Name="HTTP">
           <PSpecID>1418</PSpecID>
           <LName>World Wide Web HTTP Protocol</LName>
           <Desc>The HTTP protocol is used to implement the World-Wide-Web (WWW) on the Internet and in that context normally runs as a sub-protocol of TCP/IP. HTTP has low overhead and hence high efficiency and was designed as a communication method for a distributed hypermedia information system. HTTP is stateless and object-oriented and contains a method for negotiating data representations which allows it to be easily extended to the development of new, more advanced, highly complex data representations.</Desc>
-          <Color>14</Color>
+          <Color>8</Color>
           <CondSwitch>80</CondSwitch>
         </PSpec>
         <PSpec Name="FTP">
           <PSpecID>1402</PSpecID>
           <LName>File Transfer Protocol</LName>
           <Desc>FTP is the TCP/IP standard, high-level protocol for transferring files from one machine to another. It is usually implemented as a part of an application level program expressly for this purpose. FTP uses two well-known sockets, one for transferring the data between the machines (Data) and one for controlling and maintaining the connection (Control).</Desc>
           <Color>1</Color>
@@ -859,38 +919,42 @@
           <Color>8</Color>
           <CondSwitch>25</CondSwitch>
         </PSpec>
         <PSpec Name="SMPP">
           <PSpecID>1620</PSpecID>
           <LName>Short Message Peer to Peer Protocol</LName>
           <Desc>Short Message Peer to Peer (SMPP) protocol is an open, industry standard protocol designed to provide a flexible data communications interface for transfer of short message data between a Message Center, such as a Short Message Service Centre (SMSC), GSM Unstructured Supplementary Services Data (USSD) Server or other type of Message Center and a SMS application system, such as a WAP Proxy Server, EMail Gateway or other Messaging Gateway. Default Port Number (2775).</Desc>
+          <Color>9</Color>
           <CondSwitch>2775</CondSwitch>
         </PSpec>
         <PSpec Name="WhoIs">
           <PSpecID>1448</PSpecID>
           <Desc>WhoIs is a simple TCP transaction based query/response server that provides rudimentary directory services to internet users. Typically, a WhoIs server running on a host maintains a database of information on users of that server. Clients then connect to this server to request information on a particular user. WhoIs uses IP port 43.</Desc>
+          <Color>10</Color>
           <CondSwitch>43</CondSwitch>
         </PSpec>
         <PSpec Name="IMAP">
           <PSpecID>1450</PSpecID>
           <LName>Internet Message Access Protocol</LName>
           <Desc>IMAP may be thought of as a functional superset of Post Office Protocol version 2 (POP2). Like POP2, IMAP specifies a means of accessing stored electronic mail from a server. IMAP version 2 and 4 servers listen on TCP port 143. IMAP 3 uses TCP port 220.</Desc>
+          <Color>11</Color>
           <CondSwitch>143</CondSwitch>
         </PSpec>
         <PSpec Name="BGP">
           <PSpecID>1451</PSpecID>
           <LName>Border Gateway Protocol</LName>
           <Desc>The Border Gateway Protocol (BGP) is an inter-Autonomous System routing protocol. The primary function of a BGP speaking system is to exchange network reachability information with other BGP systems. BGP uses TCP port 179.</Desc>
+          <Color>12</Color>
           <CondSwitch>179</CondSwitch>
-          <CondExp><![CDATA[MLD16[0] != 0]]></CondExp>
         </PSpec>
         <PSpec Name="IMAP3">
           <PSpecID>1452</PSpecID>
           <LName>Internet Message Access Protocol 3</LName>
           <Desc>IMAP may be thought of as a functional superset of Post Office Protocol version 2 (POP2). Like POP2, IMAP specifies a means of accessing stored electronic mail from a server. IMAP version 2 and 4 servers listen on TCP port 143. IMAP 3 uses TCP port 220.</Desc>
+          <Color>13</Color>
           <CondSwitch>220</CondSwitch>
         </PSpec>
         <PSpec Name="GOPHER">
           <PSpecID>1416</PSpecID>
           <LName>GOPHER Protocol</LName>
           <Desc>GOPHER is a TCP/IP standard protocol for locating information on an IP internet and is most frequently found in use on the Internet. The GOPHER protocol is designed primarily to act as a distributed document delivery system. While documents and services reside on many different servers, GOPHER client software presents users with a hierarchy of items and directories much like a file system. The GOPHER protocol allows some facility for performing remote searches in the document database at its disposal.</Desc>
           <Color>12</Color>
@@ -981,16 +1045,23 @@
           <LName>X-Windows Server</LName>
           <Desc>X Windows operates over TCP, typically using server port numbers starting with 6000.</Desc>
           <CondSwitch>6000</CondSwitch>
         </PSpec>
         <PSpec Name="MySQL">
           <PSpecID>1487</PSpecID>
           <Desc>MySQL Protocol is part of the MySQL Database Management System.</Desc>
+          <Color>7</Color>
           <CondSwitch>3306</CondSwitch>
         </PSpec>
+        <PSpec Name="PostgreSQL">
+          <PSpecID>1496</PSpecID>
+          <Desc>PostgreSQL Protocol is part of the [PostgreSQL](https://www.postgresql.org/) relational database system.</Desc>
+          <Color>8</Color>
+          <CondSwitch>5432</CondSwitch>
+        </PSpec>
         <PSpec Name="IAPP">
           <PSpecID>1490</PSpecID>
           <LName>Inter-Access Point Protocol</LName>
           <Desc>Inter-Access Point Protocol (IAPP) is designed for the enforcement of unique association throughout an Extended Service Set and for secure exchange of station's security context between the current AP and the new AP during the handoff period.</Desc>
           <CondExp><![CDATA[(SrcPort == 3517) && (DestPort == 3517)]]></CondExp>
         </PSpec>
         <PSpec Name="iTunes Sharing">
@@ -1058,15 +1129,15 @@
         </PSpec>
         <PSpec Name="PPTP">
           <PSpecID>2472</PSpecID>
           <LName>Point-to-Point Tunneling Protocol</LName>
           <Desc>Point-to-Point Tunneling Protocol (PPTP) allows existing Network Access Server (NAS) functions to be separated using a client-server architecture. PPTP uses an extended version of GRE to carry user PPP packets. These enhancements allow for low-level congestion and flow control to be provided on the tunnels used to carry user data. This mechanism allows for efficient use of the bandwidth available for the tunnels and avoids unnecessary retransmissions and buffer overruns.</Desc>
           <CondSwitch>1723</CondSwitch>
         </PSpec>
-        <PSpec Name="SCCP">
+        <PSpec Name="Skinny">
           <PSpecID>2495</PSpecID>
           <LName>Skinny Client Control Protocol</LName>
           <Desc>A proprietary protocol from Cisco Systems. An H.323 proxy can be used to communicate with a Skinny Client using the SCCP. The Skinny Client (i.e. an Ethernet Phone) uses TCP/IP to transmit and receive calls and RTP/UDP/IP to/from a Skinny Client or H.323 terminal for audio. Skinny messages are carried over TCP and use port 2000.</Desc>
           <CondSwitch>2000</CondSwitch>
         </PSpec>
         <PSpec Name="Gnutella">
           <PSpecID>2496</PSpecID>
@@ -1088,22 +1159,28 @@
         </PSpec>
         <PSpec Name="LPD">
           <PSpecID>2499</PSpecID>
           <LName>Line Printer Daemon</LName>
           <Desc>The LPR/LPD printing protocol [LPD] is used with BSD UNIX systems in the client-server-printer configuration. Usage of the Job Monitoring MIB with LPR/LPD will most likely conform to Configuration 3, where the monitor application or the server uses SNMP to obtain job information from the printer. The client communicates with the UNIX server using the existing LPD protocol to obtain job information. The LPR/LPD protocol is also used in the Windows environment to implement peer-to-peer printing.</Desc>
           <CondSwitch>515</CondSwitch>
         </PSpec>
-        <PSpec Name="ISO-8073">
+        <PSpec Name="ISO 8073">
           <PSpecID>2505</PSpecID>
           <LName>ISO Transport Protocol 8073</LName>
           <SName>ISO-TP-8073</SName>
           <Desc>The ISO 8073 standard describes the ISO Transport Protocol Specification (TP). The ISO Transport Protocol specifies common encoding rules and a number of classes of transport protocol procedure which can be used with different network Quality of Service.</Desc>
           <CondSwitch>0x66</CondSwitch>
           <CondExp><![CDATA[(MLD16[0] != 0)]]></CondExp>
         </PSpec>
+        <PSpec Name="ISO 8583-1">
+          <PSpecID>2506</PSpecID>
+          <Color>5</Color>
+          <Desc>ISO 8583 is an international standard for exchanging electronic financial transactions initiated by cardholders using payment cards.</Desc>
+          <!-- No port is assigned - must use port translations-->
+        </PSpec>
         <PSpec Name="DCE">
           <PSpecID>2510</PSpecID>
           <LName>Distributed Computing Environment</LName>
           <Color>8</Color>
           <Desc>DCE provides tools and services that support distributed applications. DCE is based on three distributed computing models - client/server, remote procedure call, and data sharing.</Desc>
           <CondSwitch>0x87</CondSwitch>
           <CondExp><![CDATA[(((MLD16[0] == 0x0500) && (MLD8[2] < 20))) && (MLD16[0] != 0)]]></CondExp>
@@ -1114,17 +1191,17 @@
           <Color>8</Color>
           <Desc>FCIP mechanisms enable the transmission of Fibre Channel (FC) information by tunneling data between storage area network (SAN) facilities over IP networks; this capacity facilitates data sharing over a geographically distributed enterprise. Fibre Channel is suited for connecting servers to shared storage devices and for interconnecting storage controllers and drives.</Desc>
           <CondSwitch>0xc99</CondSwitch>
           <CondExp><![CDATA[(MLD16[0] != 0) && (MLD8[0] == 1)]]></CondExp>
         </PSpec>
         <PSpec Name="Omnipeek">
           <PSpecID>2521</PSpecID>
-          <LName>Savvius Omnipeek</LName>
+          <LName>LiveAction Omnipeek</LName>
           <Color>9</Color>
-          <Desc>Savvius Omnipeek uses this protocol for communications between the server and the client.</Desc>
+          <Desc>LiveAction Omnipeek uses this protocol for communications between the server and the client.</Desc>
           <CondSwitch>6367</CondSwitch>
         </PSpec>
         <PSpec Name="POP3s">
           <PSpecID>6701</PSpecID>
           <LName>POP3 over TLS/SSL</LName>
           <DescID>1422</DescID>
           <Color>14</Color>
@@ -1167,15 +1244,89 @@
           <PSpecID>2674</PSpecID>
           <LName>Access Node Control Protocol</LName>
           <Color>8</Color>
           <Desc>ANCP operates between a Network Access Server (NAS) and an Access Node (e.g., a Digital Subscriber Line Access Multiplexer (DSLAM)) in a multi-service reference architecture in order to perform operations related to Quality of Service, service, and subscribers. ANCP is documented in [RFC 6320](https://tools.ietf.org/html/rfc6320).</Desc>
           <CondSwitch>6068</CondSwitch>
           <CondExp><![CDATA[MLD16[0] == 0x880c]]></CondExp>
         </PSpec>
+        <PSpec Name="Elasticsearch API">
+          <PSpecID>2675</PSpecID>
+          <LName>Elasticsearch TCP HTTP RESTful Interface</LName>
+          <Color>3</Color>
+          <Desc>Elasticsearch REST API. [Elasticsearch](https://www.elastic.co) is a distributed search and analytics engine.</Desc>
+          <CondSwitch>9200</CondSwitch>
+        </PSpec>
+        <PSpec Name="Elasticsearch Cluster">
+          <PSpecID>2676</PSpecID>
+          <LName>Elasticsearch TCP Binary API and Node-Node Communications</LName>
+          <Color>4</Color>
+          <Desc>Elasticsearch cluster communications. [Elasticsearch](https://www.elastic.co) is a distributed search and analytics engine.</Desc>
+          <CondSwitch>9300</CondSwitch>
+        </PSpec>
+        <PSpec Name="STT">
+          <PSpecID>2677</PSpecID>
+          <LName>Stateless Transport Tunneling Protocol</LName>
+          <Color>4</Color>
+          <Desc>STT is an encapsulation format for network virtualization. Unlike other protocols in this space (namely VXLAN and NVGRE), it was designed to be used with soft switching within the server (generally in the vswitch in the hypervisor) while taking advantage of hardware acceleration at the NIC.</Desc>
+          <CondSwitch>7471</CondSwitch>
+        </PSpec>
       </Switch>
+      <PSpec Name="SSL">
+        <PSpecID>8926</PSpecID>
+        <LName>Secure Sockets Layer</LName>
+        <Color>3</Color>
+        <Desc>Secure Sockets Layer (SSL) is an encryption protocol that protects Internet communications. It is the precursor to TLS and is now considered weak security.</Desc>
+        <PSpec Name="SSLv3.0">
+          <PSpecID>8937</PSpecID>
+          <Color>4</Color>
+          <PSpec Name="SSLv3.0 Data">
+            <PSpecID>8930</PSpecID>
+            <Color>5</Color>
+          </PSpec>
+        </PSpec>
+        <PSpec Name="SSLv2.0">
+          <PSpecID>8923</PSpecID>
+          <Color>6</Color>
+          <Desc>SSLv2.0</Desc>
+        </PSpec>
+      </PSpec>
+      <PSpec Name="TLS">
+        <PSpecID>8938</PSpecID>
+        <LName>Transport Layer Security</LName>
+        <Color>7</Color>
+        <Desc>Transport Layer Security (TLS) is an encryption protocol that protects Internet communications.</Desc>
+        <PSpec Name="TLSv1.2">
+          <PSpecID>8934</PSpecID>
+          <Color>8</Color>
+          <PSpec Name="TLSv1.2 Data">
+            <PSpecID>8943</PSpecID>
+            <Color>9</Color>
+          </PSpec>
+        </PSpec>
+        <PSpec Name="TLSv1.1">
+          <PSpecID>8944</PSpecID>
+          <Color>7</Color>
+          <PSpec Name="TLSv1.1 Data">
+            <PSpecID>8945</PSpecID>
+            <Color>10</Color>
+          </PSpec>
+        </PSpec>
+        <PSpec Name="TLSv1.0">
+          <PSpecID>8936</PSpecID>
+          <Color>9</Color>
+          <PSpec Name="TLSv1.0 Data">
+            <PSpecID>8946</PSpecID>
+            <Color>11</Color>
+          </PSpec>
+        </PSpec>
+      </PSpec>
+      <PSpec Name="STUN">
+        <PSpecID>1488</PSpecID>
+        <CondExp><![CDATA[MLD32[6] == 0x2112A442]]></CondExp>
+      </PSpec>
     </PSpec>
     <PSpec Name="UDP">
       <PSpecID>1500</PSpecID>
       <LName>Internet User Datagram Protocol</LName>
       <Desc>Using 16-bit port numbers, UDP provides a method to distinguish between multiple application and process destinations inside a single IP node. Unlike TCP, UDP does not add any functionality to basic IP datagrams, but simply helps to identify the application which should be handling the UDP packets that are received.</Desc>
       <Color>7</Color>
       <CondSwitch>17</CondSwitch>
@@ -1192,33 +1343,85 @@
           <Value><![CDATA[PLD16[2]]]></Value>
         </Define>
       </Definitions>
       <Switch Name="UDP Port Switch">
         <On>SrcPort</On>
         <On>DestPort</On>
         <Link Name="TCP/UDP"/>
+        <PSpec Name="GENEVE">
+          <NotChild Name="GENEVE"/>
+          <NotChild Name="IPv6"/>
+          <NotChild Name="IEEE 802.3"/>
+          <NotChild Name="802.11 Data"/>
+          <NotChild Name="PPPoE"/>
+          <NotChild Name="802.1ah"/>
+          <NotChild Name="MPLS"/>
+          <NotChild Name="VLAN"/>
+          <NotChild Name="GRE"/>
+          <NotChild Name="GTP"/>
+          <NotChild Name="IPinIP"/>
+          <NotChild Name="iVXLAN"/>
+          <PSpecID>2673</PSpecID>
+          <LName>Generic Network Virtualization Encapsulation</LName>
+          <Desc>Generic Network Virtualization Encapsulation is an encapsulation protocol designed to recognize and accommodate modern and flexible changing capabilities and needs.</Desc>
+          <Color>8</Color>
+          <CondSwitch>6081</CondSwitch>
+          <Definitions>
+            <Define>
+              <Name>EthernetType</Name>
+              <Value><![CDATA[MLD16[2]]]></Value>
+            </Define>
+          </Definitions>
+          <NextLayer>
+            <Exp><![CDATA[((MLD8[0] & 0x3F) * 4) + 8]]></Exp>
+          </NextLayer>
+          <PSpec Name="IP">
+            <PSpecID>1000</PSpecID>
+            <DescID>8300</DescID>
+            <CondExp><![CDATA[(MLD8[0] & 0xf0) == 0x40]]></CondExp>
+            <NextLayer>
+              <Exp><![CDATA[(MLD8[0] & 0x0f) * 4]]></Exp>
+            </NextLayer>
+            <Switch Name="IP ProtocolID Switch">
+              <On><![CDATA[PLD8[9]]]></On>
+              <Link Name="IP Children"/>
+            </Switch>
+            <PSpec Name="IP Fragment" Sort="First">
+              <PSpecID>1001</PSpecID>
+              <LName>Fragmented IP</LName>
+              <CondExp><![CDATA[(PLD16[6] & 0x1fff) != 0]]></CondExp>
+            </PSpec>
+          </PSpec>
+          <!--<Switch Name="EType2 EthernetType Switch">
+						<On>EthernetType</On>
+						<Link Name="Ethernet Type 2 Children"/>
+					</Switch>-->
+        </PSpec>
         <PSpec Name="VXLAN">
-          <PSpecID>4789</PSpecID>
           <NotChild Name="VXLAN"/>
+          <NotChild Name="VXLAN GBP"/>
           <NotChild Name="IPv6"/>
           <NotChild Name="IEEE 802.3"/>
           <NotChild Name="802.11 Data"/>
           <NotChild Name="PPPoE"/>
           <NotChild Name="802.1ah"/>
           <NotChild Name="MPLS"/>
           <NotChild Name="VLAN"/>
           <NotChild Name="GRE"/>
           <NotChild Name="GTP"/>
           <NotChild Name="IPinIP"/>
+          <NotChild Name="iVXLAN"/>
+          <NotChild Name="GENEVE"/>
+          <PSpecID>4789</PSpecID>
           <LName>Virtual Extensible LAN</LName>
           <Desc>Virtual Extensible LAN (VXLAN) is a network virtualization technology that attempts to ameliorate the scalability problems associated with large cloud computing deployments. It uses a VLAN-like encapsulation technique to encapsulate MAC-based OSI layer 2 Ethernet frames within layer 4 UDP packets.</Desc>
           <Color>5</Color>
           <CondSwitch>4789</CondSwitch>
           <CondSwitch>8472</CondSwitch>
-          <CondExp><![CDATA[((MLD8[0] & 0x08) == 0x08) && (MLD8[7] == 0)]]></CondExp>
+          <CondExp><![CDATA[((MLD8[0] & 0x88) == 0x08) && (MLD8[7] == 0)]]></CondExp>
           <NextLayer>
             <Exp><![CDATA[8]]></Exp>
           </NextLayer>
           <PSpec Name="VXLAN EType2">
             <PSpecID>42</PSpecID>
             <DescID>2</DescID>
             <NextLayer>
@@ -1245,17 +1448,156 @@
                 <PSpecID>1001</PSpecID>
                 <LName>Fragmented IP</LName>
                 <CondExp><![CDATA[(PLD16[6] & 0x1fff) != 0]]></CondExp>
               </PSpec>
             </PSpec>
           </PSpec>
         </PSpec>
+        <PSpec Name="iVXLAN">
+          <NotChild Name="VXLAN"/>
+          <NotChild Name="VXLAN GBP"/>
+          <NotChild Name="IPv6"/>
+          <NotChild Name="IEEE 802.3"/>
+          <NotChild Name="802.11 Data"/>
+          <NotChild Name="PPPoE"/>
+          <NotChild Name="802.1ah"/>
+          <NotChild Name="MPLS"/>
+          <NotChild Name="VLAN"/>
+          <NotChild Name="GRE"/>
+          <NotChild Name="GTP"/>
+          <NotChild Name="IPinIP"/>
+          <NotChild Name="iVXLAN"/>
+          <NotChild Name="GENEVE"/>
+          <PSpecID>4791</PSpecID>
+          <LName>identifiable Virtual Extensible LAN</LName>
+          <Desc>In addition to differentiating traffic based on VNID with VXLAN, iVXLAN allows the source EPG of traffic to be identified by the Source Group (PCTAG) bits and to determine if policy was applied by source (SP) / destination (DP).</Desc>
+          <Color>5</Color>
+          <CondSwitch>48879</CondSwitch>
+          <CondSwitch>57005</CondSwitch>
+          <NextLayer>
+            <Exp><![CDATA[8]]></Exp>
+          </NextLayer>
+          <PSpec Name="VXLAN EType2">
+            <PSpecID>42</PSpecID>
+            <DescID>2</DescID>
+            <NextLayer>
+              <Exp><![CDATA[14]]></Exp>
+            </NextLayer>
+            <Definitions>
+              <Define>
+                <Name>EthernetType</Name>
+                <Value><![CDATA[PLD16[12]]]></Value>
+              </Define>
+            </Definitions>
+            <PSpec Name="IP">
+              <PSpecID>1000</PSpecID>
+              <DescID>8300</DescID>
+              <CondExp><![CDATA[(MLD8[0] == 0x45)]]></CondExp>
+              <NextLayer>
+                <Exp><![CDATA[(MLD8[0] & 0x0f) * 4]]></Exp>
+              </NextLayer>
+              <Switch Name="IP ProtocolID Switch">
+                <On><![CDATA[PLD8[9]]]></On>
+                <Link Name="IP Children"/>
+              </Switch>
+              <PSpec Name="IP Fragment" Sort="First">
+                <PSpecID>1001</PSpecID>
+                <LName>Fragmented IP</LName>
+                <CondExp><![CDATA[(PLD16[6] & 0x1fff) != 0]]></CondExp>
+              </PSpec>
+            </PSpec>
+          </PSpec>
+        </PSpec>
+        <PSpec Name="VXLAN GBP">
+          <NotChild Name="VXLAN"/>
+          <NotChild Name="VXLAN GBP"/>
+          <NotChild Name="IPv6"/>
+          <NotChild Name="IEEE 802.3"/>
+          <NotChild Name="802.11 Data"/>
+          <NotChild Name="PPPoE"/>
+          <NotChild Name="802.1ah"/>
+          <NotChild Name="MPLS"/>
+          <NotChild Name="VLAN"/>
+          <NotChild Name="GRE"/>
+          <NotChild Name="GTP"/>
+          <NotChild Name="IPinIP"/>
+          <NotChild Name="iVXLAN"/>
+          <NotChild Name="GENEVE"/>
+          <PSpecID>9004</PSpecID>
+          <LName>Group Policy Option for Virtual Extensible LAN</LName>
+          <Desc>Virtual Extensible LAN (VXLAN) is a network virtualization technology that attempts to ameliorate the scalability problems associated with large cloud computing deployments. It uses a VLAN-like encapsulation technique to encapsulate MAC-based OSI layer 2 Ethernet frames within layer 4 UDP packets. The VXLAN GBP model defines an application-centric policy model where the application connectivity requirements are specified in a manner that is independent of the underlying network topology.</Desc>
+          <Color>4</Color>
+          <CondSwitch>4789</CondSwitch>
+          <CondSwitch>8472</CondSwitch>
+          <CondExp><![CDATA[((MLD8[0] & 0x88) == 0x88) && (MLD8[7] == 0)]]></CondExp>
+          <NextLayer>
+            <Exp><![CDATA[8]]></Exp>
+          </NextLayer>
+          <PSpec Name="VXLAN EType2">
+            <PSpecID>42</PSpecID>
+            <DescID>2</DescID>
+            <NextLayer>
+              <Exp><![CDATA[14]]></Exp>
+            </NextLayer>
+            <Definitions>
+              <Define>
+                <Name>EthernetType</Name>
+                <Value><![CDATA[PLD16[12]]]></Value>
+              </Define>
+            </Definitions>
+            <PSpec Name="IP">
+              <PSpecID>1000</PSpecID>
+              <DescID>8300</DescID>
+              <CondExp><![CDATA[(MLD8[0] == 0x45)]]></CondExp>
+              <NextLayer>
+                <Exp><![CDATA[(MLD8[0] & 0x0f) * 4]]></Exp>
+              </NextLayer>
+              <Switch Name="IP ProtocolID Switch">
+                <On><![CDATA[PLD8[9]]]></On>
+                <Link Name="IP Children"/>
+              </Switch>
+              <PSpec Name="IP Fragment" Sort="First">
+                <PSpecID>1001</PSpecID>
+                <LName>Fragmented IP</LName>
+                <CondExp><![CDATA[(PLD16[6] & 0x1fff) != 0]]></CondExp>
+              </PSpec>
+            </PSpec>
+          </PSpec>
+        </PSpec>
+        <PSpec Name="VXLAN GPE">
+          <PSpecID>4790</PSpecID>
+          <LName>Generic Protocol Extension for Virtual Extensible LAN</LName>
+          <Color>3</Color>
+          <Desc>Virtual Extensible LAN (VXLAN) is a network virtualization technology that attempts to ameliorate the scalability problems associated with large cloud computing deployments. It uses a VLAN-like encapsulation technique to encapsulate MAC-based OSI layer 2 Ethernet frames within layer 4 UDP packets. VXLAN GPE is intended to extend the existing VXLAN protocol to provide protocol typing, OAM, and versioning capabilities.</Desc>
+          <CondSwitch>4790</CondSwitch>
+          <PSpec Name="vBNG">
+            <PSpecID>9001</PSpecID>
+            <LName>Virtual Broadband Network Gateway (vBNG)</LName>
+            <Color>1</Color>
+            <Desc>PPPoE/IPoE dialup packets exchange between control plane and user plane.</Desc>
+            <CondExp><![CDATA[(((MLD8[0] & 0x04) == 0x04) && (MLD8[3] == 0x07))]]></CondExp>
+          </PSpec>
+          <PSpec Name="GBP">
+            <PSpecID>9002</PSpecID>
+            <LName>Group-Based Policy (GBP)</LName>
+            <Color>2</Color>
+            <Desc>The GBP sub-header carries a 16-bit group policy ID that is semantically equivalent to the 16-bit group policy ID defined in VXLAN GPE.</Desc>
+            <CondExp><![CDATA[(((MLD8[0] & 0x04) == 0x04) && (MLD8[3] == 0x80))]]></CondExp>
+          </PSpec>
+          <PSpec Name="iOAM">
+            <PSpecID>9003</PSpecID>
+            <LName>In-situ OAM Data (iOAM)</LName>
+            <Color>6</Color>
+            <Desc>In-situ OAM (IOAM) records OAM information within the packet while the packet traverses a particular network domain.</Desc>
+            <CondExp><![CDATA[(((MLD8[0] & 0x04) == 0x04) && (MLD8[3] == 0x81))]]></CondExp>
+          </PSpec>
+        </PSpec>
         <PSpec Name="DHCPv6">
-          <PSpecID>1517</PSpecID>
           <NotChild Name="IP"/>
+          <PSpecID>1517</PSpecID>
           <LName>Dynamic Host Configuration Protocol v6</LName>
           <Desc>DHCPv6 is the Dynamic Host Configuration Protocol for IPv6. It uses UDP ports 546 and 547.</Desc>
           <Color>5</Color>
           <CondSwitch>546</CondSwitch>
           <CondSwitch>547</CondSwitch>
         </PSpec>
         <PSpec Name="PTP">
@@ -1335,14 +1677,15 @@
           <Desc>The Hot Standby Router Protocol, HSRP, provides a mechanism which is designed to support non-disruptive failover of IP traffic in certain circumstances. In particular, the protocol protects against the failure of the first hop router when the source host cannot learn the IP address of the first hop router dynamically. Using HSRP, a set of routers work in concert to present the illusion of a single virtual router to the hosts on the LAN. A single router (known as the active router) is elected by the group, and is responsible for forwarding the packets that hosts send to the virtual router. HSRP is patented by Cisco Systems, Inc. HSRP uses UDP port 1985.</Desc>
           <CondExp><![CDATA[(SrcPort == 1985) && (DestPort == 1985)]]></CondExp>
         </PSpec>
         <PSpec Name="STUN">
           <PSpecID>1488</PSpecID>
           <LName>Simple Traversal of UDP through NAT</LName>
           <Desc>STUN (Simple Traversal of UDP (User Datagram Protocol) through NATs (Network Address Translators)) is a network protocol allowing a client behind a NAT (or multiple NATs) to find out its public address, the type of NAT it is behind and the internet side port associated by the NAT with a particular local port.</Desc>
+          <Color>9</Color>
           <CondSwitch>3478</CondSwitch>
         </PSpec>
         <PSpec Name="L2F">
           <PSpecID>1564</PSpecID>
           <LName>Layer Two Forwarding</LName>
           <Desc>L2F permits the tunneling of the link layer (i.e., HDLC, or SLIP frames) of higher level protocols. Using such tunnels, it is possible to divorce the location of the initial dial-up server from the location at which the dial-up protocol connection is terminated and access to the network provided. L2F uses IP port 1701.</Desc>
           <CondSwitch>1701</CondSwitch>
@@ -1488,29 +1831,14 @@
         </PSpec>
         <PSpec Name="TiVo">
           <PSpecID>1472</PSpecID>
           <LName>TiVo Connect Automatic Machine Discovery Protocol</LName>
           <Desc>The TiVo Connect Automatic Machine Discovery Protocol allows two or more machines running TiVo Connect software to discover each other by periodically exchanging UDP and/or TCP packets of TiVo-defined identifying information. Default Port Number (2190).</Desc>
           <CondSwitch>2190</CondSwitch>
         </PSpec>
-        <PSpec Name="NetFlow">
-          <PSpecID>1495</PSpecID>
-          <LName>Cisco NetFlow</LName>
-          <Desc>NetFlow is a protocol introduced by Cisco and used by network devices (primarily switches and routers) to export IP flow statistics for analysis.</Desc>
-          <CondSwitch>2055</CondSwitch>
-          <CondSwitch>9995</CondSwitch>
-        </PSpec>
-        <PSpec Name="IPFIX">
-          <PSpecID>4739</PSpecID>
-          <LName>IPFIX</LName>
-          <Desc>Internet Protocol Flow Information Export (IPFIX) is an IETF protocol, which was created based on the need for a common, universal standard of export for Internet Protocol flow information from routers, probes and other devices that are used by mediation systems, accounting/billing systems and network management systems to facilitate services such as measurement, accounting and billing. The IPFIX standard defines how IP flow information is to be formatted and transferred from an exporter to a collector.</Desc>
-          <CondSwitch>4739</CondSwitch>
-          <CondSwitch>4740</CondSwitch>
-          <CondSwitch>5229</CondSwitch>
-        </PSpec>
         <PSpec Name="AppleTalk Tunnel">
           <PSpecID>7700</PSpecID>
           <LName>AppleTalk over IP</LName>
           <SName>ATalk</SName>
           <Desc>In environments where all protocol traffic must be IP datagrams, several methods have been developed to embed or tunnel other protocols inside of IP datagrams. Many of these methods were developed by Apple Computer.</Desc>
           <Color>14</Color>
           <CondSwitch>201</CondSwitch>
@@ -1934,15 +2262,66 @@
               <PSpecID>2540</PSpecID>
               <LName>Universal Alcatel Protocol</LName>
               <Desc>Universal Alcatel (UA) is a protocol for managing the identity of station owners in an Alcatel-Lucent PBX.</Desc>
               <Color>4</Color>
             </PSpec>
           </PSpec>
         </PSpec>
+        <PSpec Name="AllJoyn">
+          <PSpecID>1799</PSpecID>
+          <LName>AllJoyn Name Service Protocol</LName>
+          <Color>10</Color>
+          <Desc>AllJoyn is an open source software framework that allows devices to communicate with other devices around them.</Desc>
+          <CondSwitch>9956</CondSwitch>
+        </PSpec>
       </Switch>
+      <PSpec Name="DTLS">
+        <PSpecID>8941</PSpecID>
+        <LName>Datagram Transport Layer Security</LName>
+        <Color>6</Color>
+        <Desc>Datagram Transport Layer Security (DTLS) provides security for UDP-based applications similar to TLS</Desc>
+        <PSpec Name="DTLSv1.0">
+          <PSpecID>8940</PSpecID>
+          <Color>7</Color>
+          <PSpec Name="DTLSv1.0 Data">
+            <PSpecID>8928</PSpecID>
+            <Color>8</Color>
+          </PSpec>
+        </PSpec>
+        <PSpec Name="DTLSv1.2">
+          <PSpecID>8939</PSpecID>
+          <Color>9</Color>
+          <PSpec Name="DTLSv1.2 Data">
+            <PSpecID>8927</PSpecID>
+            <Color>10</Color>
+          </PSpec>
+        </PSpec>
+      </PSpec>
+      <PSpec Name="GQUIC">
+        <PSpecID>8932</PSpecID>
+        <LName>Google QUIC</LName>
+        <Color>10</Color>
+        <Desc>Google QUIC - the original QUIC designed and implemented at Google</Desc>
+      </PSpec>
+      <PSpec Name="Facebook QUIC">
+        <PSpecID>8948</PSpecID>
+        <Color>11</Color>
+        <Desc>QUIC Facebook mvfst</Desc>
+      </PSpec>
+      <PSpec Name="QUIC">
+        <PSpecID>8931</PSpecID>
+        <Color>12</Color>
+        <Desc>QUIC improves performance of web applications currently using TCP/TLS by using UDP with stream-multiplexing, fast connection establishment and low latency. [IETF QUIC](https://datatracker.ietf.org/wg/quic/about/)</Desc>
+      </PSpec>
+      <PSpec Name="QUIC Draft Version">
+        <PSpecID>8929</PSpecID>
+        <LName>IETF QUIC Draft Version</LName>
+        <Color>13</Color>
+        <Desc>IETF QUIC Draft Version</Desc>
+      </PSpec>
       <PSpec Name="CiscoAP">
         <NotChild Name="CiscoAP"/>
         <PSpecID>8260</PSpecID>
         <LName>Cisco AP Protocol</LName>
         <SName>CiscoAP</SName>
         <Desc>Cisco AP Protocol.</Desc>
         <Color>5</Color>
@@ -1974,77 +2353,90 @@
         <DescID>2670</DescID>
         <CondExp><![CDATA[(MLD8[0] == 0x47) && (MLD8[188] == 0x47)]]></CondExp>
       </PSpec>
       <PSpec Name="RTP" Sort="Last">
         <PSpecID>2670</PSpecID>
         <LName>Real-Time Transport Protocol</LName>
         <Desc>RTP provides end-to-end network transport functions suitable for applications transmitting real-time data, such as audio, video or simulation data, over multicast or unicast network services.</Desc>
+        <Color>8</Color>
         <CondExp><![CDATA[(((MLD8[0] & 0xc0) == 0x80) && (((MLD8[1] & 0x7f) == 0) || (((MLD8[1] & 0x7f) >= 2) && ((MLD8[1] & 0x7f) <= 18)) || ((MLD8[1] & 0x7f) == 25) || ((MLD8[1] & 0x7f) == 26) || ((MLD8[1] & 0x7f) == 28) || (((MLD8[1] & 0x7f) >= 31) && ((MLD8[1] & 0x7f) <= 34)) || ((MLD8[1] & 0x7f) >= 96)))]]></CondExp>
         <PSpec Name="G.711">
           <PSpecID>2680</PSpecID>
           <DescID>2670</DescID>
           <CondExp><![CDATA[((MLD8[1] & 0x7f) == 0) || ((MLD8[1] & 0x7f) == 8)]]></CondExp>
+          <Color>3</Color>
         </PSpec>
         <PSpec Name="G.723.1">
           <PSpecID>2681</PSpecID>
           <DescID>2670</DescID>
           <CondExp><![CDATA[(MLD8[1] & 0x7f) == 4]]></CondExp>
+          <Color>5</Color>
         </PSpec>
         <PSpec Name="G.722">
           <PSpecID>2690</PSpecID>
           <DescID>2670</DescID>
           <CondExp><![CDATA[(MLD8[1] & 0x7f) == 9]]></CondExp>
+          <Color>4</Color>
         </PSpec>
         <PSpec Name="G.726">
           <PSpecID>2686</PSpecID>
           <DescID>2670</DescID>
           <CondExp><![CDATA[(MLD8[1] & 0x7f) == 2]]></CondExp>
+          <Color>6</Color>
         </PSpec>
         <PSpec Name="G.728">
           <PSpecID>2682</PSpecID>
           <DescID>2670</DescID>
           <CondExp><![CDATA[(MLD8[1] & 0x7f) == 15]]></CondExp>
+          <Color>7</Color>
         </PSpec>
         <PSpec Name="G.729">
           <PSpecID>2683</PSpecID>
           <DescID>2670</DescID>
           <CondExp><![CDATA[(MLD8[1] & 0x7f) == 18]]></CondExp>
+          <Color>5</Color>
         </PSpec>
         <PSpec Name="H.261">
           <PSpecID>2684</PSpecID>
           <DescID>2670</DescID>
           <CondExp><![CDATA[(MLD8[1] & 0x7f) == 31]]></CondExp>
+          <Color>14</Color>
         </PSpec>
         <PSpec Name="MPV">
           <PSpecID>2691</PSpecID>
           <LName>MPEG1/MPEG2 Video</LName>
           <DescID>2670</DescID>
           <CondExp><![CDATA[(MLD8[1] & 0x7f) == 32]]></CondExp>
+          <Color>1</Color>
         </PSpec>
         <PSpec Name="H.222">
           <PSpecID>2689</PSpecID>
           <LName>ISO/IEC 13818-1- MPEG2 Protocol</LName>
           <DescID>2670</DescID>
           <CondExp><![CDATA[(MLD8[1] & 0x7f) == 33]]></CondExp>
+          <Color>3</Color>
         </PSpec>
         <PSpec Name="H.263">
           <PSpecID>2685</PSpecID>
           <DescID>2670</DescID>
           <CondExp><![CDATA[(MLD8[1] & 0x7f) == 34]]></CondExp>
+          <Color>12</Color>
         </PSpec>
         <PSpec Name="GSM">
           <PSpecID>2687</PSpecID>
           <DescID>2670</DescID>
           <CondExp><![CDATA[(MLD8[1] & 0x7f) == 3]]></CondExp>
+          <Color>5</Color>
         </PSpec>
         <PSpec Name="RTP Dynamic">
           <PSpecID>2688</PSpecID>
           <LName>RTP Dynamic Payload Type</LName>
           <DescID>2670</DescID>
           <CondExp><![CDATA[(MLD8[1] & 0x7f) >= 96]]></CondExp>
+          <Color>7</Color>
         </PSpec>
       </PSpec>
       <PSpec Name="RTCP" Sort="Last">
         <PSpecID>2671</PSpecID>
         <LName>Real-Time Transport Control Protocol</LName>
         <Desc>RTP's data transport is augmented by a control protocol (RTCP) to allow monitoring of the data delivery in a manner scalable to large multicast networks, and to provide minimal control and identification functionality.</Desc>
         <CondExp><![CDATA[((MLD8[0] & 0xc0) == 0x80) && (MLD8[1] >= 200 && MLD8[1] <= 209)]]></CondExp>
@@ -2131,14 +2523,15 @@
       <Color>15</Color>
       <CondSwitch>51</CondSwitch>
     </PSpec>
     <PSpec Name="GRE">
       <NotChild Name="GRE"/>
       <NotChild Name="IPv6"/>
       <NotChild Name="IPinIP"/>
+      <NotChild Name="GENEVE"/>
       <PSpecID>2213</PSpecID>
       <LName>Generic Routing Encapsulation</LName>
       <Desc>Generic Routing Encapsulation (GRE) protocol allows an arbitrary network protocol to be transmitted over any other arbitrary network protocol by encapsulating the packets of the encapsulated protocol within GRE packets, and then transmitting the GRE packets over the base network protocol.</Desc>
       <Color>15</Color>
       <CondSwitch>47</CondSwitch>
       <NextLayer>
         <Special>GRE</Special>
@@ -2163,14 +2556,15 @@
       <CondSwitch>103</CondSwitch>
     </PSpec>
     <PSpec Name="IPinIP">
       <NotChild Name="IPinIP"/>
       <NotChild Name="IPv6"/>
       <NotChild Name="GRE"/>
       <NotChild Name="GTP"/>
+      <NotChild Name="GENEVE"/>
       <PSpecID>1000</PSpecID>
       <CondSwitch>4</CondSwitch>
       <NextLayer>
         <Exp><![CDATA[(MLD8[0] & 0x0f) * 4]]></Exp>
       </NextLayer>
       <Definitions>
         <Define>
@@ -2186,14 +2580,15 @@
         <PSpecID>1001</PSpecID>
         <LName>Fragmented IP</LName>
         <CondExp><![CDATA[(PLD16[6] & 0x1fff) != 0]]></CondExp>
       </PSpec>
     </PSpec>
     <PSpec Name="IPv6">
       <NotChild Name="IPv6"/>
+      <NotChild Name="GENEVE"/>
       <PSpecID>8300</PSpecID>
       <LName>Internet Protocol Version 6</LName>
       <Desc>An IP datagram is the basic unit of information passed across the internet which provides the basis for connectionless, best-effort packet delivery service. The entire protocol stack which is built on top of IP is frequently called TCP/IP because TCP and IP are the two most fundamental protocols in the stack. As a non-proprietary standard, IP is the most prevalent networking protocol among heterogeneous computer systems.</Desc>
       <Color>13</Color>
       <CondSwitch>41</CondSwitch>
       <NextLayer>
         <Exp><![CDATA[MLD8[6] == 0 || MLD8[6] == 0x2B ? (((MLD8[41] + 1) * 8) + 40) : 40]]></Exp>
@@ -2209,101 +2604,123 @@
     <PSpec Name="L2TPv3">
       <PSpecID>2216</PSpecID>
       <LName>Layer Two Tunneling Protocol v3</LName>
       <Desc>L2TP facilitates the tunneling of packets across an intervening network in a way that is as transparent as possible to both end users and applications. L2TP v3 provides additional security features, improved encapsulation, and additional link types over L2TP v2. L2TP v3 may be carried over IP or UDP port 1701.</Desc>
       <Color>3</Color>
       <CondSwitch>115</CondSwitch>
     </PSpec>
-    <!--
-		<PSpec Name="EtherIP">
-			<NotChild Name="IPinIP"/>
-			<NotChild Name="EtherIP"/>
-			<NotChild Name="IPv6"/>
-			<NotChild Name="GRE"/>
-			<NotChild Name="GTP"/>
-			<PSpecID>8700</PSpecID>
-			<Color>13</Color>
-			<CondSwitch>97</CondSwitch>
-			<NextLayer>
-				<Exp><![CDATA[2]]></Exp>
-			</NextLayer>
-			<PSpec Name="EtherIP EType2">
-				<PSpecID>8701</PSpecID>
-				<DescID>2</DescID>
-				<CondExp><![CDATA[(MLD16[12] > 1500)]]></CondExp>
-				<NextLayer>
-					<Exp><![CDATA[14]]></Exp>
-				</NextLayer>
-				<PSpec Name="VLAN">
-					<NotChild Name="VLAN" Depth="2"/>
-					<NotChild Name="MPLS"/>
-					<PSpecID>40</PSpecID>
-					<LName>IEEE 802.1Q VLAN</LName>
-					<DescID>40</DescID>
-					<Color>17</Color>
-					<CondExp><![CDATA[PLD16[12] == 0x8100 || PLD16[12] == 0x88a8 || PLD16[12] == 0x9100]]></CondExp>
-					<NextLayer>
-						<Exp><![CDATA[4]]></Exp>
-					</NextLayer>
-					<PSpec Name="IP">
-						<PSpecID>1000</PSpecID>
-						<LName>Internet Protocol</LName>
-						<Color>4</Color>
-							<CondExp><![CDATA[(PLD16[2] == 0x0800)]]></CondExp>
-						<NextLayer>
-							<Exp><![CDATA[(MLD8[0] & 0x0f) * 4]]></Exp>
-						</NextLayer>
-						<Definitions>
-							<Define>
-								<Name>ProtocolID</Name>
-								<Value><![CDATA[PLD8[9]]]></Value>
-							</Define>
-						</Definitions>
-						<Switch Name="IP ProtocolID Switch">
-							<On>ProtocolID</On>
-							<Link Name="IP Children"/>
-						</Switch>
-						<PSpec Name="IP Fragment" Sort="First">
-							<PSpecID>1001</PSpecID>
-							<LName>Fragmented IP</LName>
-							<CondExp><![CDATA[(PLD16[6] & 0x1fff) != 0]]></CondExp>
-						</PSpec>
-					</PSpec>
-				</PSpec>
-			</PSpec>
-		</PSpec>
-		-->
+    <PSpec Name="HIP">
+      <PSpecID>2217</PSpecID>
+      <LName>Host Identity Protocol</LName>
+      <Desc>The Host Identity Protocol (HIP) is a host identification technology for use on Internet Protocol (IP) networks, such as the Internet.</Desc>
+      <Color>4</Color>
+      <CondSwitch>139</CondSwitch>
+      <PSpec Name="HIPv1">
+        <PSpecID>2218</PSpecID>
+        <LName>Host Identity Protocol Version 1</LName>
+        <DescID>2217</DescID>
+        <Color>5</Color>
+        <CondExp><![CDATA[((MLD8[3] & 0xf0) >> 4) == 1]]></CondExp>
+      </PSpec>
+      <PSpec Name="HIPv2">
+        <PSpecID>2219</PSpecID>
+        <LName>Host Identity Protocol Version 2</LName>
+        <DescID>2217</DescID>
+        <Color>6</Color>
+        <CondExp><![CDATA[((MLD8[3] & 0xf0) >> 4) == 2]]></CondExp>
+      </PSpec>
+    </PSpec>
+    <PSpec Name="EtherIP">
+      <PSpecID>8700</PSpecID>
+      <Desc>EtherIP is used to tunnel Ethernet frames across an IP internet. See [RFC 3378](https://tools.ietf.org/html/rfc3378)</Desc>
+      <Color>16</Color>
+      <CondSwitch>97</CondSwitch>
+      <NextLayer>
+        <Exp><![CDATA[2]]></Exp>
+      </NextLayer>
+    </PSpec>
   </PSpec>
   <PSpec Name="SCTP Chunks" Type="CommonTable">
     <PSpec Name="SCTP DATA Chunk">
       <PSpecID>1999</PSpecID>
       <SName>SCTP DATA</SName>
       <Desc>Transports payload.</Desc>
-      <Color>7</Color>
+      <Color>6</Color>
       <CondExp><![CDATA[MLD8[0] == 0x00]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[16]]></Exp>
       </NextLayer>
+      <Definitions>
+        <Define>
+          <Name>SCTPSrcPort</Name>
+          <Value><![CDATA[PLD16[-12]]]></Value>
+        </Define>
+        <Define>
+          <Name>SCTPDestPort</Name>
+          <Value><![CDATA[PLD16[-10]]]></Value>
+        </Define>
+        <Define>
+          <Name>SCTPPayloadID</Name>
+          <Value><![CDATA[PLD32[12]]]></Value>
+        </Define>
+        <Define>
+          <Name>SCTPDataChunkFlags</Name>
+          <Value><![CDATA[PLD8[1]]]></Value>
+        </Define>
+      </Definitions>
+      <!--
+			<PSpec Name="SCTP Non-Complete Packet">
+				<PSpecID>2280</PSpecID>
+				<LName>SCTP Non-Complete Packet</LName>
+				<Desc>A fragmented SCTP Packet</Desc>
+				<Color>14</Color>
+				<CondExp><![CDATA[SCTPDataChunkFlags & 0x03 != 0x03 && MLD16[2] != 16 ]]></CondExp>
+				<PSpec Name="SCTP Fragmented Beginning Packet">
+					<PSpecID>2281</PSpecID>
+					<LName>SCTP Fragmented Beginning Packet</LName>
+					<Desc>A fragmented SCTP Beginning Packet</Desc>
+					<Color>14</Color>
+					<CondExp><![CDATA[SCTPDataChunkFlags & 0x01 != 0x01 && SCTPDataChunkFlags & 0x02 == 0x02]]></CondExp>
+					<Link Name="SCTP Children"/>
+				</PSpec>
+				<PSpec Name="SCTP Fragmented Ending Packet">
+					<PSpecID>2282</PSpecID>
+					<LName>SCTP Fragmented Ending Packet</LName>
+					<Desc>A fragmented SCTP Ending Packet</Desc>
+					<Color>14</Color>
+					<CondExp><![CDATA[SCTPDataChunkFlags & 0x01 == 0x01 && SCTPDataChunkFlags & 0x02 != 0x02]]></CondExp>
+					<Link Name="SCTP Children"/>
+				</PSpec>
+				<PSpec Name="SCTP Fragmented Packet">
+					<PSpecID>2284</PSpecID>
+					<LName>SCTP Fragmented Fragmented Packet</LName>
+					<Desc>A fragmented SCTP Fragmented Packet</Desc>
+					<Color>14</Color>
+					<CondExp><![CDATA[SCTPDataChunkFlags & 0x01 == 0x00 && SCTPDataChunkFlags & 0x02 == 0x00]]></CondExp>
+					<Link Name="SCTP Children"/>
+				</PSpec>
+			</PSpec>
+			-->
       <Link Name="SCTP Children"/>
     </PSpec>
     <PSpec Name="SCTP INIT Chunk">
       <PSpecID>8501</PSpecID>
       <SName>SCTP INIT</SName>
       <LName>SCTP Initiation (INIT)</LName>
-      <Color>7</Color>
+      <Color>8</Color>
       <CondExp><![CDATA[MLD8[0] == 0x01]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP INIT ACK Chunk">
       <PSpecID>8502</PSpecID>
       <SName>SCTP INIT ACK</SName>
       <LName>SCTP Initiation Acknowledgement (INIT ACK)</LName>
-      <Color>7</Color>
+      <Color>9</Color>
       <CondExp><![CDATA[MLD8[0] == 0x02]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP SACK Chunk">
       <PSpecID>8503</PSpecID>
@@ -2313,542 +2730,1708 @@
       <CondExp><![CDATA[MLD8[0] == 0x03]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[16]]></Exp>
       </NextLayer>
       <PSpec Name="SCTP DATA Chunk">
         <PSpecID>1999</PSpecID>
         <SName>SCTP DATA</SName>
-        <Color>7</Color>
-        <CondExp><![CDATA[MLD8[0] == 0x00]]></CondExp>
+        <Color>6</Color>
+        <CondExp><![CDATA[(MLD8[0] == 0x00) && (MLD16[2] != 0)]]></CondExp>
         <NextLayer>
-          <Exp><![CDATA[(16)]]></Exp>
+          <Exp><![CDATA[16]]></Exp>
         </NextLayer>
+        <Definitions>
+          <Define>
+            <Name>SCTPSrcPort</Name>
+            <Value><![CDATA[PLD16[-28]]]></Value>
+          </Define>
+          <Define>
+            <Name>SCTPDestPort</Name>
+            <Value><![CDATA[PLD16[-26]]]></Value>
+          </Define>
+          <Define>
+            <Name>SCTPPayloadID</Name>
+            <Value><![CDATA[PLD32[12]]]></Value>
+          </Define>
+          <Define>
+            <Name>SCTPDataChunkFlags</Name>
+            <Value><![CDATA[PLD8[1]]]></Value>
+          </Define>
+        </Definitions>
+        <!--
+				<PSpec Name="SCTP Non-Complete Packet">
+					<PSpecID>2280</PSpecID>
+					<LName>SCTP Non-Complete Packet</LName>
+					<Desc>A fragmented SCTP Packet</Desc>
+					<Color>14</Color>
+					<CondExp><![CDATA[SCTPDataChunkFlags & 0x03 != 0x03 && MLD16[2] != 16 ]]></CondExp>
+					<PSpec Name="SCTP Fragmented Beginning Packet">
+						<PSpecID>2281</PSpecID>
+						<LName>SCTP Fragmented Beginning Packet</LName>
+						<Desc>A fragmented SCTP Beginning Packet</Desc>
+						<Color>14</Color>
+						<CondExp><![CDATA[SCTPDataChunkFlags & 0x01 != 0x01 && SCTPDataChunkFlags & 0x02 == 0x02]]></CondExp>
+						<Link Name="SCTP Children"/>
+					</PSpec>
+					<PSpec Name="SCTP Fragmented Ending Packet">
+						<PSpecID>2282</PSpecID>
+						<LName>SCTP Fragmented Ending Packet</LName>
+						<Desc>A fragmented SCTP Ending Packet</Desc>
+						<Color>14</Color>
+						<CondExp><![CDATA[SCTPDataChunkFlags & 0x01 == 0x01 && SCTPDataChunkFlags & 0x02 != 0x02]]></CondExp>
+						<Link Name="SCTP Children"/>
+					</PSpec>
+					<PSpec Name="SCTP Fragmented Packet">
+						<PSpecID>2284</PSpecID>
+						<LName>SCTP Fragmented Fragmented Packet</LName>
+						<Desc>A fragmented SCTP Fragmented Packet</Desc>
+						<Color>14</Color>
+						<CondExp><![CDATA[SCTPDataChunkFlags & 0x01 == 0x00 && SCTPDataChunkFlags & 0x02 == 0x00]]></CondExp>
+						<Link Name="SCTP Children"/>
+					</PSpec>
+				</PSpec>
+				-->
         <Link Name="SCTP Children"/>
       </PSpec>
     </PSpec>
     <PSpec Name="SCTP HEARTBEAT Chunk">
       <PSpecID>8504</PSpecID>
       <SName>SCTP HEARTBEAT</SName>
       <LName>SCTP Heartbeat Request (HEARTBEAT)</LName>
-      <Color>7</Color>
+      <Color>10</Color>
       <CondExp><![CDATA[MLD8[0] == 0x04]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP HEARTBEAT ACK Chunk">
       <PSpecID>8505</PSpecID>
       <SName>SCTP HEARTBEAT ACK</SName>
       <LName>SCTP Heartbeat Acknowledgement (HEARTBEAT)</LName>
-      <Color>7</Color>
+      <Color>11</Color>
       <CondExp><![CDATA[MLD8[0] == 0x05]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP ABORT Chunk">
       <PSpecID>8506</PSpecID>
       <SName>SCTP ABORT</SName>
       <LName>SCTP Abort (ABORT)</LName>
-      <Color>7</Color>
+      <Color>12</Color>
       <CondExp><![CDATA[MLD8[0] == 0x06]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP SHUTDOWN Chunk">
       <PSpecID>8507</PSpecID>
       <SName>SCTP SHUTDOWN</SName>
       <LName>SCTP Shutdown (SHUTDOWN)</LName>
-      <Color>7</Color>
+      <Color>13</Color>
       <CondExp><![CDATA[MLD8[0] == 0x07]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP SHUTDOWN ACK Chunk">
       <PSpecID>8508</PSpecID>
       <SName>SCTP SHUTDOWN ACK</SName>
       <LName>SCTP Shutdown Acknowledgement (SHUTDOWN ACK)</LName>
-      <Color>7</Color>
+      <Color>14</Color>
       <CondExp><![CDATA[MLD8[0] == 0x08]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP ERROR Chunk">
       <PSpecID>8509</PSpecID>
       <SName>SCTP ERROR</SName>
       <LName>SCTP Operation Error (ERROR)</LName>
-      <Color>7</Color>
+      <Color>15</Color>
       <CondExp><![CDATA[MLD8[0] == 0x09]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP COOKIE ECHO Chunk">
       <PSpecID>8510</PSpecID>
       <SName>SCTP COOKIE ECHO</SName>
       <LName>SCTP State Cookie (COOKIE ECHO)</LName>
-      <Color>7</Color>
+      <Color>16</Color>
       <CondExp><![CDATA[MLD8[0] == 0x0a]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP COOKIE ACK Chunk">
       <PSpecID>8511</PSpecID>
       <SName>SCTP COOKIE ACK</SName>
       <LName>SCTP Cookie Acknowledgement (COOKIE ACK)</LName>
-      <Color>7</Color>
+      <Color>17</Color>
       <CondExp><![CDATA[MLD8[0] == 0x0b]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP ECNE Chunk">
       <PSpecID>8512</PSpecID>
       <SName>SCTP ECNE</SName>
       <LName>Reserved for Explicit Congestion Notification Echo (ECNE)</LName>
-      <Color>7</Color>
+      <Color>18</Color>
       <CondExp><![CDATA[MLD8[0] == 0x0c]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP CWR Chunk">
       <PSpecID>8513</PSpecID>
       <SName>SCTP CWR</SName>
       <LName>SCTP Reserved for Congestion Window Reduced (CWR)</LName>
-      <Color>7</Color>
+      <Color>19</Color>
       <CondExp><![CDATA[MLD8[0] == 0x0d]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP SHUTDOWN COMPLETE Chunk">
       <PSpecID>8514</PSpecID>
       <SName>SCTP SHUTDOWN COMPLETE</SName>
       <LName>SCTP Shutdown Complete (SHUTDOWN COMPLETE)</LName>
-      <Color>7</Color>
+      <Color>20</Color>
       <CondExp><![CDATA[MLD8[0] == 0x0e]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP AUTHENTICATION Chunk">
       <PSpecID>8516</PSpecID>
       <SName>SCTP AUTHENTICATION</SName>
       <LName>SCTP AUTHENTICATION Chunk (AUTH)</LName>
-      <Color>7</Color>
+      <Color>21</Color>
       <CondExp><![CDATA[MLD8[0] == 0x0f]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP ADDRESS CONFIGURATION ACKNOWLEDGEMENT Chunk">
       <PSpecID>8517</PSpecID>
       <SName>SCTP ADDRESS CONFIGURATION ACKNOWLEDGEMENT</SName>
       <LName>SCTP ADDRESS CONFIGURATION ACKNOWLEDGEMENT Chunk (ASCONF-ACK)</LName>
-      <Color>7</Color>
+      <Color>22</Color>
       <CondExp><![CDATA[MLD8[0] == 0x80]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP RECONFIGURATION Chunk">
       <PSpecID>8518</PSpecID>
       <SName>SCTP RECONFIGURATION</SName>
       <LName>SCTP RECONFIGURATION Chunk (RE-CONFIG)</LName>
-      <Color>7</Color>
+      <Color>23</Color>
       <CondExp><![CDATA[MLD8[0] == 0x82]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP PADDING Chunk">
       <PSpecID>8519</PSpecID>
       <SName>SCTP PADDING Chunk (PAD)</SName>
       <LName>SCTP PADDING Chunk (PAD)</LName>
-      <Color>7</Color>
+      <Color>1</Color>
       <CondExp><![CDATA[MLD8[0] == 0x84]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP Forward Cumulative TSN Chunk">
       <PSpecID>8515</PSpecID>
       <SName>SCTP Fwrd. Cum. TSN</SName>
       <LName>SCTP Forward Cumulative TSN</LName>
-      <Color>7</Color>
+      <Color>2</Color>
       <CondExp><![CDATA[MLD8[0] == 0xc0]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="SCTP ADDRESS CONFIGURATION CHANGE Chunk (ASCONF)">
       <PSpecID>8520</PSpecID>
       <SName>SCTP ADDRESS CONFIGURATION CHANGE Chunk (ASCONF)</SName>
       <LName>SCTP ADDRESS CONFIGURATION CHANGE Chunk (ASCONF)</LName>
-      <Color>7</Color>
+      <Color>3</Color>
       <CondExp><![CDATA[MLD8[0] == 0xc1]]></CondExp>
       <NextLayer>
         <Exp><![CDATA[MLD16[2]]]></Exp>
       </NextLayer>
     </PSpec>
   </PSpec>
   <PSpec Name="SCTP Children" Type="CommonTable">
     <PSpec Name="Diameter">
       <PSpecID>6726</PSpecID>
-      <Desc>Diameter is an authentication, authorization and accounting protocol for computer networks, and a successor to RADIUS.</Desc>
-      <Color>15</Color>
-      <CondExp><![CDATA[((PLD32[12] == 0x00) && (PLD16[-12] == 3868)) || ( (PLD32[12] == 0x00) && (PLD16[-10] == 3868)) || ((PLD32[12] == 0x00) && (PLD16[-28] == 3868)) || ( (PLD32[12] == 0x00) && (PLD16[-26] == 3868))]]></CondExp>
+      <Color>14</Color>
+      <CondExp><![CDATA[SCTPSrcPort == 3868 || SCTPDestPort == 3868 || SCTPPayloadID == 0x46]]></CondExp>
     </PSpec>
     <PSpec Name="SIP">
       <PSpecID>2474</PSpecID>
-      <LName>Session Initiation Protocol</LName>
-      <Desc>The Session Initiation Protocol (SIP) is an application-layer control (signaling) protocol for creating, modifying and terminating sessions with one or more participants. These sessions include Internet multimedia conferences, Internet telephone calls and multimedia distribution. Members in a session can communicate via multicast or via a mesh of unicast relations, or a combination of these.</Desc>
       <Color>15</Color>
-      <CondExp><![CDATA[(((MLD8[0] & 0xc0) != 0x80) && ((PLD16[-12] == 5060) || (PLD16[-10] == 5060) || (PLD16[-28] == 5060) || (PLD16[-26] == 5060))) || ((MLD32[0] == 0x5349502F) || (MLD32[0] == 0x494E5649) || (MLD32[0] == 0x41434B20) || (MLD32[0] == 0x42594520) || (MLD32[0] == 0x43414E43) || (MLD32[0] == 0x4F505449) || (MLD32[0] == 0x52454749) || (MLD32[0] == 0x50524143) || (MLD32[0] == 0x53554253) || (MLD32[0] == 0x4E4F5449) || (MLD32[0] == 0x5055424C) || (MLD32[0] == 0x494e464f) || (MLD32[0] == 0x52454645) || (MLD32[0] == 0x4D455353) || (MLD32[0] == 0x55504441))]]></CondExp>
+      <CondExp><![CDATA[(MLD8[0] != 0x00 && SCTPSrcPort == 5060 || SCTPDestPort == 5060) || (MLD32[0] == 0x5349502F || MLD32[0] == 0x494E5649 || MLD32[0] == 0x41434B20 || MLD32[0] == 0x42594520 || MLD32[0] == 0x43414E43 || MLD32[0] == 0x4F505449 || MLD32[0] == 0x52454749 || MLD32[0] == 0x50524143 || MLD32[0] == 0x53554253 || MLD32[0] == 0x4E4F5449 || MLD32[0] == 0x5055424C || MLD32[0] == 0x494e464f || MLD32[0] == 0x52454645 || MLD32[0] == 0x4D455353 || MLD32[0] == 0x55504441)]]></CondExp>
+    </PSpec>
+    <PSpec Name="SIP over TLS">
+      <PSpecID>2475</PSpecID>
+      <Color>14</Color>
+      <CondExp><![CDATA[SCTPSrcPort == 5061 || SCTPDestPort == 5061]]></CondExp>
     </PSpec>
     <PSpec Name="SGSAP">
       <PSpecID>6729</PSpecID>
       <Desc>SGs Application Part.</Desc>
       <Color>15</Color>
-      <CondExp><![CDATA[((PLD32[12] == 0x00) && (PLD16[-12] == 29118)) || ( (PLD32[12] == 0x00) && (PLD16[-10] == 29118)) || ((PLD32[12] == 0x00) && (PLD16[-28] == 29118)) || ( (PLD32[12] == 0x00) && (PLD16[-26] == 29118))]]></CondExp>
+      <CondExp><![CDATA[SCTPSrcPort == 29118 || SCTPDestPort == 29118]]></CondExp>
     </PSpec>
-    <PSpec Name="Res. by SCTP">
-      <PSpecID>1901</PSpecID>
-      <LName>Reserved by SCTP</LName>
-      <Color>7</Color>
-      <CondExp><![CDATA[((PLD32[12] == 0x00) && (SrcPort != 3868)) || ((PLD32[12] == 0x00) && (DestPort != 3868))]]></CondExp>
+    <PSpec Name="FTP">
+      <PSpecID>1402</PSpecID>
+      <Color>1</Color>
+      <CondExp><![CDATA[SCTPSrcPort == 20 || SCTPDestPort == 20 || SCTPSrcPort == 21 || SCTPDestPort == 21]]></CondExp>
+      <PSpec Name="Data">
+        <PSpecID>1408</PSpecID>
+        <CondExp><![CDATA[SCTPSrcPort == 20 || SCTPDestPort == 20]]></CondExp>
+      </PSpec>
+      <PSpec Name="Control">
+        <PSpecID>1407</PSpecID>
+        <CondExp><![CDATA[SCTPSrcPort == 21 || SCTPDestPort == 21]]></CondExp>
+      </PSpec>
     </PSpec>
-    <PSpec Name="IUA">
-      <PSpecID>1902</PSpecID>
+    <PSpec Name="HTTP">
+      <PSpecID>1418</PSpecID>
       <Color>8</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x01]]></CondExp>
+      <CondExp><![CDATA[SCTPSrcPort == 80 || SCTPDestPort == 80]]></CondExp>
+    </PSpec>
+    <PSpec Name="BGP">
+      <PSpecID>1451</PSpecID>
+      <Color>12</Color>
+      <CondExp><![CDATA[SCTPSrcPort == 179 || SCTPDestPort == 179]]></CondExp>
+    </PSpec>
+    <PSpec Name="HTTPS">
+      <PSpecID>1454</PSpecID>
+      <LName>Secure HTTP Protocol</LName>
+      <Color>14</Color>
+      <CondExp><![CDATA[SCTPSrcPort == 443 || SCTPDestPort == 443]]></CondExp>
     </PSpec>
     <PSpec Name="M2UA">
       <PSpecID>1903</PSpecID>
+      <LName>Message Transfer Part Level 2 User Adaptation</LName>
+      <Desc>Message Transfer Part Level 2 User Adaptation is SIGTRAN protocol that provides an SCTP adaptation layer for the seamless backhaul of Message Transfer Part (MTP) Level 2 user messages and service interface across an IP network. See RFC 3331 for more details.</Desc>
       <Color>11</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x02]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x02 || SCTPSrcPort == 2904 || SCTPDestPort == 2904]]></CondExp>
       <NextLayer>
-        <Exp><![CDATA[16]]></Exp>
+        <Exp><![CDATA[20]]></Exp>
       </NextLayer>
-    </PSpec>
-    <PSpec Name="M3UA">
-      <PSpecID>1904</PSpecID>
-      <Color>12</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x03]]></CondExp>
-      <NextLayer>
-        <Exp><![CDATA[8]]></Exp>
-      </NextLayer>
-      <PSpec Name="M3UA NA">
-        <PSpecID>1997</PSpecID>
-        <LName>Network Appearance</LName>
-        <Color>13</Color>
-        <CondExp><![CDATA[MLD16[0] == 0x00000200]]></CondExp>
-        <NextLayer>
-          <Exp><![CDATA[8]]></Exp>
-        </NextLayer>
-        <PSpec Name="M3UA PD">
-          <PSpecID>1998</PSpecID>
-          <LName>Payload Data</LName>
-          <Color>14</Color>
-          <CondExp><![CDATA[MLD16[0] == 0x00000210]]></CondExp>
-          <NextLayer>
-            <Exp><![CDATA[16]]></Exp>
-          </NextLayer>
-          <Link Name="SigTran Children"/>
-        </PSpec>
-        <PSpec Name="M3UA RC">
-          <PSpecID>1996</PSpecID>
-          <LName>Routing Context</LName>
-          <Color>15</Color>
-          <CondExp><![CDATA[MLD16[0] == 0x00000006]]></CondExp>
-          <NextLayer>
-            <Exp><![CDATA[8]]></Exp>
-          </NextLayer>
-          <PSpec Name="M3UA PD">
-            <PSpecID>1998</PSpecID>
-            <LName>Payload Data</LName>
-            <Color>14</Color>
-            <CondExp><![CDATA[MLD16[0] == 0x00000210]]></CondExp>
-            <NextLayer>
-              <Exp><![CDATA[16]]></Exp>
-            </NextLayer>
-            <Link Name="SigTran Children"/>
-          </PSpec>
-        </PSpec>
-      </PSpec>
-      <PSpec Name="M3UA RC">
-        <PSpecID>1996</PSpecID>
-        <LName>Routing Context</LName>
-        <Color>15</Color>
-        <CondExp><![CDATA[MLD16[0] == 0x00000006]]></CondExp>
-        <NextLayer>
-          <Exp><![CDATA[8]]></Exp>
-        </NextLayer>
-        <PSpec Name="M3UA PD">
-          <PSpecID>1998</PSpecID>
-          <LName>Payload Data</LName>
-          <Color>14</Color>
-          <CondExp><![CDATA[MLD16[0] == 0x00000210]]></CondExp>
-          <NextLayer>
-            <Exp><![CDATA[16]]></Exp>
-          </NextLayer>
-          <Link Name="SigTran Children"/>
-        </PSpec>
-      </PSpec>
-      <PSpec Name="M3UA PD">
-        <PSpecID>1998</PSpecID>
-        <Color>14</Color>
-        <CondExp><![CDATA[MLD16[0] == 0x00000210]]></CondExp>
+      <PSpec Name="MTP3">
+        <PSpecID>1955</PSpecID>
+        <LName>Message Transfer Part 3</LName>
+        <Desc>Message Transfer Part 3 User Adaptation Layer is the User Adaptation protocol under the SIGTRAN family of protocols and provides an SCTP adaptation layer for the seamless backhaul or peering of Message Transfer Part (MTP) Level 3 user messages and service interface across an IP network. See RFC 4666 for more details.</Desc>
+        <Color>12</Color>
+        <CondExp><![CDATA[MLD16[0] != 0]]></CondExp>
+        <Definitions>
+          <Define>
+            <Name>ServiceIndicator</Name>
+            <Value><![CDATA[PLD8[0] & 0x0f]]></Value>
+          </Define>
+        </Definitions>
         <NextLayer>
-          <Exp><![CDATA[16]]></Exp>
+          <Exp><![CDATA[5]]></Exp>
         </NextLayer>
         <Link Name="SigTran Children"/>
       </PSpec>
     </PSpec>
     <PSpec Name="SUA">
       <PSpecID>1905</PSpecID>
+      <LName>SCCP User Adaptation</LName>
+      <Desc>SUA provides an SCTP adaptation layer for the seamless backhaul or peering of Signaling Connection Control Part user messages and service interface across an IP network. It is specified in RFC 3868.</Desc>
       <Color>16</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x04]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x04 || SCTPSrcPort == 14001 || SCTPDestPort == 14001]]></CondExp>
     </PSpec>
     <PSpec Name="M2PA">
       <PSpecID>1906</PSpecID>
+      <Desc/>
       <Color>17</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x05]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x05 || SCTPSrcPort == 3565 || SCTPDestPort == 3565]]></CondExp>
       <NextLayer>
-        <Exp><![CDATA[16]]></Exp>
+        <Exp><![CDATA[17]]></Exp>
       </NextLayer>
+      <PSpec Name="MTP3">
+        <PSpecID>1955</PSpecID>
+        <LName>Message Transfer Part Level 3</LName>
+        <Desc>Message Transfer Part Level 3 (MTP3) is part of the SS7 stack used for communication in Public Switched Telephone Networks and is responsible for reliable, unduplicated and in-sequence transport of SS7 messages between communication partners.</Desc>
+        <Color>12</Color>
+        <CondExp><![CDATA[MLD16[0] != 0 && PLD32[4] >= 17]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[5]]></Exp>
+        </NextLayer>
+        <Definitions>
+          <Define>
+            <Name>ServiceIndicator</Name>
+            <Value><![CDATA[PLD8[0] & 0x0f]]></Value>
+          </Define>
+        </Definitions>
+        <Link Name="SigTran Children"/>
+      </PSpec>
     </PSpec>
     <PSpec Name="V5UA">
       <PSpecID>1907</PSpecID>
+      <LName>V5 User Adaptation</LName>
+      <Desc>V5 User Adaptation provides an SCTP adaptation layer for the seamless backhaul of V5.2 user messages and service interface across an IP network. It is a variation of IUA.See RFC 3807 for more details.</Desc>
       <Color>18</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x06]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x06 || SCTPSrcPort == 5675 || SCTPDestPort == 5675]]></CondExp>
     </PSpec>
     <PSpec Name="MEGACO">
       <PSpecID>7800</PSpecID>
       <LName>MEGACO Text / H.248</LName>
-      <Desc>MEGACO is the protocol used for interfacing between external call agents called Media Gateway Controllers and Media Gateways.</Desc>
       <Color>13</Color>
-      <CondExp><![CDATA[(PLD32[12] == 0x07) && (PLD32[16] == 0x4d454741)]]></CondExp>
+      <CondExp><![CDATA[(SCTPPayloadID == 0x07 && PLD32[16] == 0x4d454741) || SCTPSrcPort == 2944 || SCTPDestPort == 2944]]></CondExp>
     </PSpec>
     <PSpec Name="H.248">
       <PSpecID>1908</PSpecID>
       <Color>8</Color>
-      <CondExp><![CDATA[(PLD32[12] == 0x07) && (PLD32[16] != 0x4d454741)]]></CondExp>
+      <CondExp><![CDATA[(SCTPPayloadID == 0x07 && PLD32[16] != 0x4d454741) || SCTPSrcPort == 2945 || SCTPDestPort == 2945]]></CondExp>
     </PSpec>
     <PSpec Name="BICC/Q.2150.3">
       <PSpecID>1909</PSpecID>
+      <Desc/>
       <Color>9</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x08]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x08 || SCTPSrcPort == 3097 || SCTPDestPort == 3097]]></CondExp>
     </PSpec>
     <PSpec Name="TALI">
       <PSpecID>1910</PSpecID>
+      <Desc/>
       <Color>10</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x09]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x09]]></CondExp>
     </PSpec>
     <PSpec Name="DUA">
       <PSpecID>1911</PSpecID>
+      <Desc>DPNSS 1/DASS 2 User Adaptation (DUA), as defined in RFC 4129, is a mechanism for backhauling Digital Private Network Signaling System 1 (DPNSS 1) and Digital Access Signaling System 2 (DASS 2) messages over IP.</Desc>
       <Color>11</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x0a]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x0a]]></CondExp>
     </PSpec>
     <PSpec Name="ASAP">
       <PSpecID>1912</PSpecID>
+      <Desc/>
       <Color>12</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x0b]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x0b || SCTPSrcPort == 3863 || SCTPDestPort == 3863 || SCTPSrcPort == 3864 || SCTPDestPort == 3864]]></CondExp>
     </PSpec>
     <PSpec Name="ENRP">
       <PSpecID>1913</PSpecID>
+      <Desc/>
       <Color>13</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x0c]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x0c]]></CondExp>
     </PSpec>
     <PSpec Name="H.323">
-      <PSpecID>1914</PSpecID>
+      <PSpecID>2490</PSpecID>
+      <LName>H.323 Host Call</LName>
       <Color>2</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x0d]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x0d || SCTPSrcPort == 1720 || SCTPDestPort == 1720 || SCTPSrcPort == 1721 || SCTPDestPort == 1721]]></CondExp>
+      <PSpec Name="H.225: Q.931 Basic Call Control">
+        <PSpecID>2501</PSpecID>
+        <SName>H.225/Q.931</SName>
+        <CondExp><![CDATA[((MLD16[0] == 0x300) && ((MLD8[4] == 8)) || (MLD8[0] == 8))]]></CondExp>
+      </PSpec>
     </PSpec>
     <PSpec Name="Q.IPC/Q.2150.3">
       <PSpecID>1915</PSpecID>
+      <Desc/>
       <Color>3</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x0e]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x0e || SCTPSrcPort == 3097 || SCTPDestPort == 3097]]></CondExp>
     </PSpec>
     <PSpec Name="SIMCO">
       <PSpecID>1916</PSpecID>
+      <Desc/>
       <Color>4</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x0f]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x0f || SCTPSrcPort == 7626 || SCTPDestPort == 7626]]></CondExp>
     </PSpec>
     <PSpec Name="DDP Seg Chunk">
       <PSpecID>1917</PSpecID>
       <SName>DDPSC</SName>
       <LName>DDP Segment Chunk</LName>
+      <Desc/>
       <Color>5</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x10]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x10]]></CondExp>
     </PSpec>
     <PSpec Name="DDP SSC">
       <PSpecID>1918</PSpecID>
       <SName>DDPSSC</SName>
       <LName>DDP Stream Session Control</LName>
+      <Desc/>
       <Color>6</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x11]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x11]]></CondExp>
     </PSpec>
     <PSpec Name="S1AP">
       <PSpecID>1919</PSpecID>
       <LName>S1 Application Protocol</LName>
+      <Desc/>
       <Color>19</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x12]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x12]]></CondExp>
     </PSpec>
     <PSpec Name="RUA">
       <PSpecID>1920</PSpecID>
+      <Desc/>
       <Color>20</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x13]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x13]]></CondExp>
+      <!--here should be a filter on IE Type 4 == Ranap Message which links to RANAP, this can stand on several points inside RUA-->
     </PSpec>
     <PSpec Name="HNBAP">
       <PSpecID>1921</PSpecID>
+      <Desc/>
       <Color>21</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x14]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x14]]></CondExp>
     </PSpec>
     <PSpec Name="ForCES-HP">
       <PSpecID>1922</PSpecID>
+      <Desc/>
       <Color>22</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x15]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x15 || SCTPSrcPort == 6704 || SCTPDestPort == 6704]]></CondExp>
     </PSpec>
     <PSpec Name="ForCES-MP">
       <PSpecID>1923</PSpecID>
+      <Desc/>
       <Color>23</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x16]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x16 || SCTPSrcPort == 6705 || SCTPDestPort == 6705]]></CondExp>
     </PSpec>
     <PSpec Name="ForCES-LP">
       <PSpecID>1924</PSpecID>
+      <Desc/>
       <Color>1</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x17]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x17 || SCTPSrcPort == 6706 || SCTPDestPort == 6706]]></CondExp>
     </PSpec>
     <PSpec Name="SBc-AP">
       <PSpecID>1925</PSpecID>
+      <Desc/>
       <Color>2</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x18]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x18 || SCTPSrcPort == 29169 || SCTPDestPort == 29169]]></CondExp>
     </PSpec>
     <PSpec Name="NBAP">
       <PSpecID>1926</PSpecID>
+      <Desc/>
       <Color>3</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x19]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x19]]></CondExp>
     </PSpec>
     <PSpec Name="X2AP">
       <PSpecID>1928</PSpecID>
+      <Desc/>
       <Color>4</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x1b]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x1b]]></CondExp>
     </PSpec>
     <PSpec Name="IRCP">
       <PSpecID>1929</PSpecID>
       <LName>IRCP - Inter Router Capability Protocol</LName>
+      <Desc/>
       <Color>8</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x1c]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x1c]]></CondExp>
     </PSpec>
     <PSpec Name="LCS-AP">
       <PSpecID>1930</PSpecID>
+      <Desc/>
       <Color>5</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x1d]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x1d]]></CondExp>
     </PSpec>
     <PSpec Name="MPICH2">
       <PSpecID>1932</PSpecID>
+      <Desc/>
       <Color>6</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x1e]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x1e]]></CondExp>
     </PSpec>
     <PSpec Name="SABP">
       <PSpecID>1933</PSpecID>
       <LName>Service Area Broadcast Protocol</LName>
+      <Desc/>
       <Color>7</Color>
-      <CondExp><![CDATA[PLD32[12] == 0x1f]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 0x1f]]></CondExp>
     </PSpec>
-  </PSpec>
-  <PSpec Name="SigTran Children" Type="CommonTable">
-    <PSpec Name="SCCP">
-      <PSpecID>1943</PSpecID>
-      <LName>Signaling Connection Control Part</LName>
+    <PSpec Name="Fractal Generator">
+      <PSpecID>2033</PSpecID>
+      <LName>Fractal Generator Protocol</LName>
+      <Desc/>
+      <Color>8</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 32]]></CondExp>
+    </PSpec>
+    <PSpec Name="Ping Pong">
+      <PSpecID>2034</PSpecID>
+      <LName>Ping Pong Protocol</LName>
+      <Desc/>
+      <Color>9</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 33]]></CondExp>
+    </PSpec>
+    <PSpec Name="CalcApp">
+      <PSpecID>2035</PSpecID>
+      <LName>CalcApp Protocol</LName>
+      <Desc/>
+      <Color>10</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 34]]></CondExp>
+    </PSpec>
+    <PSpec Name="Scripting Service">
+      <PSpecID>2036</PSpecID>
+      <LName>Scripting Service Protocol (SSP)</LName>
+      <Desc/>
+      <Color>11</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 35]]></CondExp>
+    </PSpec>
+    <PSpec Name="NetPerfMeter Ctl Chan">
+      <PSpecID>2037</PSpecID>
+      <LName>NetPerfMeter Protocol Control Channel (NPMP-CONTROL)</LName>
+      <Desc/>
+      <Color>12</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 36]]></CondExp>
+    </PSpec>
+    <PSpec Name="NetPerfMeter Data Chan">
+      <PSpecID>2038</PSpecID>
+      <LName>NetPerfMeter Protocol DATA Channel (NPMP-DATA)</LName>
+      <Desc/>
+      <Color>13</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 37]]></CondExp>
+    </PSpec>
+    <PSpec Name="Echo">
+      <PSpecID>2039</PSpecID>
+      <Desc/>
+      <Color>14</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 38]]></CondExp>
+    </PSpec>
+    <PSpec Name="Discard">
+      <PSpecID>2040</PSpecID>
+      <Desc/>
+      <Color>15</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 39]]></CondExp>
+    </PSpec>
+    <PSpec Name="DAYTIME">
+      <PSpecID>2041</PSpecID>
+      <Desc/>
+      <Color>16</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 40]]></CondExp>
+    </PSpec>
+    <PSpec Name="Chargen">
+      <PSpecID>2042</PSpecID>
+      <LName>Character Generator (CHARGEN)</LName>
+      <Desc/>
+      <Color>17</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 41]]></CondExp>
+    </PSpec>
+    <PSpec Name="3GPP RNA">
+      <PSpecID>2043</PSpecID>
+      <SName>RNA</SName>
+      <Desc/>
+      <Color>18</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 42]]></CondExp>
+    </PSpec>
+    <PSpec Name="3GPP M2AP">
+      <PSpecID>2044</PSpecID>
+      <SName>M2AP</SName>
+      <Desc/>
+      <Color>19</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 43 || SCTPSrcPort == 36443 || SCTPDestPort == 36443]]></CondExp>
+    </PSpec>
+    <PSpec Name="3GPP M3AP">
+      <PSpecID>2045</PSpecID>
+      <SName>M3AP</SName>
+      <Desc/>
+      <Color>20</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 44 || SCTPSrcPort == 36444 || SCTPDestPort == 36444]]></CondExp>
+    </PSpec>
+    <PSpec Name="SSH">
+      <PSpecID>1459</PSpecID>
+      <Color>5</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 45 || SCTPSrcPort == 22 || SCTPDestPort == 22]]></CondExp>
+    </PSpec>
+    <PSpec Name="Diameter in a DTLS/SCTP DATA chunk">
+      <PSpecID>2046</PSpecID>
+      <LName>Diameter in a DTLS/SCTP DATA chunk</LName>
+      <Desc/>
+      <Color>7</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 47]]></CondExp>
+    </PSpec>
+    <PSpec Name="R14P. BER Encoded ASN.1 over SCTP">
+      <PSpecID>2047</PSpecID>
+      <LName>R14P. BER Encoded ASN.1 over SCTP</LName>
+      <Desc/>
+      <Color>8</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 48]]></CondExp>
+    </PSpec>
+    <PSpec Name="WebRTC Control">
+      <PSpecID>2050</PSpecID>
+      <Desc/>
       <Color>9</Color>
-      <CondExp><![CDATA[MLD8[-4] == 0x03]]></CondExp>
+      <CondExp><![CDATA[SCTPPayloadID == 50]]></CondExp>
+    </PSpec>
+    <PSpec Name="DOMString Last">
+      <PSpecID>2051</PSpecID>
+      <Desc/>
+      <Color>10</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 51]]></CondExp>
+    </PSpec>
+    <PSpec Name="Binary Data Partial">
+      <PSpecID>2052</PSpecID>
+      <Desc/>
+      <Color>11</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 52]]></CondExp>
+    </PSpec>
+    <PSpec Name="Binary Data Last">
+      <PSpecID>2053</PSpecID>
+      <Desc/>
+      <Color>12</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 53]]></CondExp>
+    </PSpec>
+    <PSpec Name="DOMString Partial">
+      <PSpecID>2054</PSpecID>
+      <Desc/>
+      <Color>13</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 54]]></CondExp>
+    </PSpec>
+    <PSpec Name="3GPP PUA">
+      <PSpecID>2055</PSpecID>
+      <Desc/>
+      <Color>14</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 55]]></CondExp>
+    </PSpec>
+    <PSpec Name="WebRTC String Empty">
+      <PSpecID>2056</PSpecID>
+      <Desc/>
+      <Color>15</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 56]]></CondExp>
+    </PSpec>
+    <PSpec Name="WebRTC Binary Empty">
+      <PSpecID>2057</PSpecID>
+      <Desc/>
+      <Color>16</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 57]]></CondExp>
+    </PSpec>
+    <PSpec Name="3GPP XwAP">
+      <PSpecID>2058</PSpecID>
+      <SName>XwAP</SName>
+      <Desc/>
+      <Color>17</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 58]]></CondExp>
+    </PSpec>
+    <PSpec Name="3GPP Xw-Control Plane">
+      <PSpecID>2059</PSpecID>
+      <SName>XwCP</SName>
+      <Desc/>
+      <Color>18</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 59]]></CondExp>
+    </PSpec>
+    <PSpec Name="3GPP NG Application Protocol">
+      <PSpecID>2060</PSpecID>
+      <LName>3GPP NG Application Protocol (NGAP)</LName>
+      <SName>NGAP</SName>
+      <Desc/>
+      <Color>19</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 60]]></CondExp>
+    </PSpec>
+    <PSpec Name="3GPP Xn Application Protocol">
+      <PSpecID>2061</PSpecID>
+      <LName>3GPP Xn Application Protocol (XnAP)</LName>
+      <SName>XnAP</SName>
+      <Desc/>
+      <Color>20</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 61]]></CondExp>
+    </PSpec>
+    <PSpec Name="3GPP F1 Application Protocol">
+      <PSpecID>2062</PSpecID>
+      <LName>3GPP F1 Application Protocol (F1AP)</LName>
+      <SName>F1AP</SName>
+      <Desc/>
+      <Color>21</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 62]]></CondExp>
+    </PSpec>
+    <PSpec Name="Res. by SCTP">
+      <PSpecID>1901</PSpecID>
+      <LName>Reserved by SCTP</LName>
+      <Desc/>
+      <Color>7</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 0x00 && (SCTPSrcPort != 3868 || SCTPDestPort != 3868)]]></CondExp>
+      <Link Name="SCTP Port Children"/>
+    </PSpec>
+    <PSpec Name="M3UA">
+      <PSpecID>1904</PSpecID>
+      <Desc>M3UA (MTP-3 User Adaptation Layer) is a protocol for supporting the transport of SS7 MTP-3 User Signaling (e.g. ISUP or SCCP messages) over IP using the services of the Stream Control Transmission Protocol (SCTP). Also, provision is made for protocol elements that enable a seamless operation of the MTP-3 User peers in the SS7 and IP domains. This protocol would be used between Signaling Gateway (SG) and Media Gateway Controller (MGC) or IP-Resident Database, or between two IP-based applications. It is assumed that SG receives SS7 signaling over a standard SS7 interface using the SS7 message Transfer Part (MTP) to provide transport.</Desc>
+      <Color>12</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 0x03 || SCTPSrcPort == 2905 || SCTPDestPort == 2905]]></CondExp>
+      <NextLayer>
+        <Exp><![CDATA[8]]></Exp>
+      </NextLayer>
+      <PSpec Name="M3UA NA">
+        <PSpecID>1997</PSpecID>
+        <LName>Network Appearance</LName>
+        <Desc/>
+        <Color>12</Color>
+        <CondExp><![CDATA[MLD16[0] == 0x00000200]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[8]]></Exp>
+        </NextLayer>
+        <PSpec Name="M3UA PD">
+          <PSpecID>1998</PSpecID>
+          <LName>Payload Data</LName>
+          <Desc/>
+          <Color>12</Color>
+          <CondExp><![CDATA[MLD16[0] == 0x00000210]]></CondExp>
+          <NextLayer>
+            <Exp><![CDATA[16]]></Exp>
+          </NextLayer>
+          <Definitions>
+            <Define>
+              <Name>ServiceIndicator</Name>
+              <Value><![CDATA[PLD8[12] & 0x0f]]></Value>
+            </Define>
+          </Definitions>
+          <Link Name="SigTran Children"/>
+        </PSpec>
+        <PSpec Name="M3UA RC">
+          <PSpecID>1996</PSpecID>
+          <LName>Routing Context</LName>
+          <Desc/>
+          <Color>12</Color>
+          <CondExp><![CDATA[MLD16[0] == 0x00000006]]></CondExp>
+          <NextLayer>
+            <Exp><![CDATA[8]]></Exp>
+          </NextLayer>
+          <PSpec Name="M3UA PD">
+            <PSpecID>1998</PSpecID>
+            <LName>Payload Data</LName>
+            <Color>12</Color>
+            <CondExp><![CDATA[MLD16[0] == 0x00000210]]></CondExp>
+            <NextLayer>
+              <Exp><![CDATA[16]]></Exp>
+            </NextLayer>
+            <Definitions>
+              <Define>
+                <Name>ServiceIndicator</Name>
+                <Value><![CDATA[PLD8[12] & 0x0f]]></Value>
+              </Define>
+            </Definitions>
+            <Link Name="SigTran Children"/>
+          </PSpec>
+        </PSpec>
+      </PSpec>
+      <PSpec Name="M3UA RC">
+        <PSpecID>1996</PSpecID>
+        <LName>Routing Context</LName>
+        <Color>12</Color>
+        <CondExp><![CDATA[MLD16[0] == 0x00000006]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[8]]></Exp>
+        </NextLayer>
+        <PSpec Name="M3UA PD">
+          <PSpecID>1998</PSpecID>
+          <LName>Payload Data</LName>
+          <Color>12</Color>
+          <CondExp><![CDATA[MLD16[0] == 0x00000210]]></CondExp>
+          <NextLayer>
+            <Exp><![CDATA[16]]></Exp>
+          </NextLayer>
+          <Definitions>
+            <Define>
+              <Name>ServiceIndicator</Name>
+              <Value><![CDATA[PLD8[12] & 0x0f]]></Value>
+            </Define>
+          </Definitions>
+          <Link Name="SigTran Children"/>
+        </PSpec>
+      </PSpec>
+      <PSpec Name="M3UA PD">
+        <PSpecID>1998</PSpecID>
+        <Color>12</Color>
+        <CondExp><![CDATA[MLD16[0] == 0x00000210]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[16]]></Exp>
+        </NextLayer>
+        <Definitions>
+          <Define>
+            <Name>ServiceIndicator</Name>
+            <Value><![CDATA[PLD8[12] & 0x0f]]></Value>
+          </Define>
+        </Definitions>
+        <Link Name="SigTran Children"/>
+      </PSpec>
+    </PSpec>
+    <PSpec Name="IUA">
+      <PSpecID>1902</PSpecID>
+      <Desc/>
+      <Color>8</Color>
+      <CondExp><![CDATA[SCTPPayloadID == 0x01 || SCTPSrcPort == 9900 || SCTPDestPort == 9900]]></CondExp>
+    </PSpec>
+    <Link Name="SCTP Port Children"/>
+  </PSpec>
+  <PSpec Name="SCTP Port Children" Type="CommonTable">
+    <PSpec Name="Diameter">
+      <PSpecID>6726</PSpecID>
+      <Color>14</Color>
+      <CondExp><![CDATA[(SCTPSrcPort >= 4894 && SCTPSrcPort <= 4910) || (SCTPDestPort >= 4894 && SCTPDestPort <= 4910) || SCTPDestPort == 2909 || SCTPDestPort == 2010 || SCTPDestPort == 4415 || SCTPDestPort == 4415]]></CondExp>
+    </PSpec>
+    <PSpec Name="SIP">
+      <PSpecID>2474</PSpecID>
+      <Color>15</Color>
+      <CondExp><![CDATA[SCTPSrcPort == 5730 || SCTPDestPort == 5730 || MLD32[0] == 0x5349502F || MLD32[0] == 0x494E5649 || MLD32[0] == 0x41434B20 || MLD32[0] == 0x42594520 || MLD32[0] == 0x43414E43 || MLD32[0] == 0x4F505449 || MLD32[0] == 0x52454749 || MLD32[0] == 0x50524143 || MLD32[0] == 0x53554253 || MLD32[0] == 0x4E4F5449 || MLD32[0] == 0x5055424C || MLD32[0] == 0x494e464f || MLD32[0] == 0x52454645 || MLD32[0] == 0x4D455353 || MLD32[0] == 0x55504441]]></CondExp>
     </PSpec>
+  </PSpec>
+  <PSpec Name="SigTran Children" Type="CommonTable">
     <PSpec Name="SNMM">
       <PSpecID>1940</PSpecID>
       <LName>Signaling Network Management Messages</LName>
+      <Desc/>
       <Color>9</Color>
-      <CondExp><![CDATA[MLD8[-4] == 0x00]]></CondExp>
+      <CondExp><![CDATA[ServiceIndicator == 0x00]]></CondExp>
     </PSpec>
     <PSpec Name="SNTMM">
       <PSpecID>1941</PSpecID>
       <LName>Signaling Network Testing and Maintenance Messages</LName>
+      <Desc/>
       <Color>10</Color>
-      <CondExp><![CDATA[MLD8[-4] == 0x01]]></CondExp>
+      <CondExp><![CDATA[ServiceIndicator == 0x01]]></CondExp>
     </PSpec>
     <PSpec Name="SNTMSM">
       <PSpecID>1942</PSpecID>
       <LName>Signaling Network Testing and Maintenance Special Messages</LName>
+      <Desc/>
       <Color>11</Color>
-      <CondExp><![CDATA[MLD8[-4] == 0x02]]></CondExp>
+      <CondExp><![CDATA[ServiceIndicator == 0x02]]></CondExp>
     </PSpec>
     <PSpec Name="TUP">
       <PSpecID>1944</PSpecID>
       <LName>Telephone User Part</LName>
+      <Desc/>
       <Color>12</Color>
-      <CondExp><![CDATA[MLD8[-4] == 0x04]]></CondExp>
+      <CondExp><![CDATA[ServiceIndicator == 0x04]]></CondExp>
     </PSpec>
     <PSpec Name="ISUP">
       <PSpecID>1945</PSpecID>
       <LName>ISDN User Part</LName>
+      <Desc>The ISDN (Integrated Services Digital Network) User Part is part of Signaling System 7 (SS7), and is used to set up and tear down telephone calls on the Public Switched Telephone Network (PSTN).</Desc>
       <Color>13</Color>
-      <CondExp><![CDATA[MLD8[-4] == 0x05]]></CondExp>
+      <CondExp><![CDATA[ServiceIndicator == 0x05]]></CondExp>
     </PSpec>
-    <PSpec Name="DUPCCM">
+    <PSpec Name="DUP CCM">
       <PSpecID>1946</PSpecID>
-      <SName>DUP Call Circ Msg</SName>
       <LName>Data User Part (call and circuit-related messages)</LName>
+      <Desc/>
       <Color>14</Color>
-      <CondExp><![CDATA[MLD8[-4]== 0x06]]></CondExp>
+      <CondExp><![CDATA[ServiceIndicator == 0x06]]></CondExp>
     </PSpec>
     <PSpec Name="DUP FRCM">
       <PSpecID>1947</PSpecID>
-      <SName>DUP fac reg canc Msg</SName>
       <LName>Data User Part (facility registration and cancellation messages)</LName>
+      <Desc/>
       <Color>15</Color>
-      <CondExp><![CDATA[MLD8[-4] == 0x07]]></CondExp>
+      <CondExp><![CDATA[ServiceIndicator == 0x07]]></CondExp>
     </PSpec>
-    <PSpec Name="MTPTUP">
+    <PSpec Name="MTP TUP">
       <PSpecID>1948</PSpecID>
-      <SName>MTP TUP</SName>
       <LName>Reserved for MTP Testing User Part</LName>
+      <Desc/>
       <Color>16</Color>
-      <CondExp><![CDATA[MLD8[-4] == 0x08]]></CondExp>
+      <CondExp><![CDATA[ServiceIndicator == 0x08]]></CondExp>
     </PSpec>
     <PSpec Name="BISUP">
       <PSpecID>1949</PSpecID>
       <LName>Broadband ISDN User Part</LName>
+      <Desc/>
       <Color>9</Color>
-      <CondExp><![CDATA[MLD8[-4] == 0x09]]></CondExp>
+      <CondExp><![CDATA[ServiceIndicator == 0x09]]></CondExp>
     </PSpec>
     <PSpec Name="SISUP">
       <PSpecID>1950</PSpecID>
       <LName>Satellite ISDN User Part</LName>
+      <Desc/>
       <Color>9</Color>
-      <CondExp><![CDATA[MLD8[-4] == 0x0a]]></CondExp>
+      <CondExp><![CDATA[ServiceIndicator == 0x0a]]></CondExp>
     </PSpec>
     <PSpec Name="BICC">
       <PSpecID>1951</PSpecID>
       <LName>Bearer Independent Call Control Protocol</LName>
+      <Desc>The Bearer-Independent Call Control (BICC) is a signaling protocol based on N-ISUP that is used for supporting the narrowband Integrated Services Digital Network (ISDN) service over a broadband backbone network. The BICC is designed to interwork with existing transport technologies and is specified in ITU-T recommendation Q.1901.</Desc>
       <Color>9</Color>
-      <CondExp><![CDATA[MLD8[-4] == 0x0d]]></CondExp>
+      <CondExp><![CDATA[ServiceIndicator == 0x0d]]></CondExp>
     </PSpec>
     <PSpec Name="MEGACO">
       <PSpecID>7800</PSpecID>
       <LName>MEGACO Text / H.248</LName>
-      <Desc>MEGACO is the protocol used for interfacing between external call agents called Media Gateway Controllers and Media Gateways.</Desc>
-      <Color>13</Color>
+      <Color>9</Color>
       <CondExp><![CDATA[MLD8[-4] == 0x0e]]></CondExp>
     </PSpec>
+    <PSpec Name="SCCP">
+      <PSpecID>1943</PSpecID>
+      <LName>Signaling Connection Control Part</LName>
+      <Desc>Provides extended routing, flow control, segmentation, connection-orientation and error correction facilities in Signaling System 7 networks.</Desc>
+      <Color>11</Color>
+      <CondExp><![CDATA[ServiceIndicator == 0x03]]></CondExp>
+      <PSpec Name="SCCP Conn Req">
+        <PSpecID>1960</PSpecID>
+        <LName>SCCP Connection Request</LName>
+        <Color>2</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x01]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[MLD8[6] + 7 + 7]]></Exp>
+        </NextLayer>
+        <Definitions>
+          <Define>
+            <Name>SCCPSSN</Name>
+            <Value><![CDATA[((PLD8[8] & 0x01) == 0x01) ? PLD8[11] : PLD8[9]]]></Value>
+          </Define>
+        </Definitions>
+        <Switch Name="SCCP Conn Req Switch">
+          <On>SCCPSSN</On>
+          <Link Name="SCCP Children"/>
+        </Switch>
+      </PSpec>
+      <PSpec Name="SCCP Conn Conf">
+        <PSpecID>1961</PSpecID>
+        <LName>SCCP Connection Confirm</LName>
+        <Color>3</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x02]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[MLD8[9] + 9]]></Exp>
+        </NextLayer>
+      </PSpec>
+      <PSpec Name="SCCP Conn Ref">
+        <PSpecID>1962</PSpecID>
+        <LName>SCCP Connection Refused</LName>
+        <Color>4</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x03]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[20]]></Exp>
+        </NextLayer>
+      </PSpec>
+      <PSpec Name="SCCP Conn Rel">
+        <PSpecID>1963</PSpecID>
+        <LName>SCCP Connection Released</LName>
+        <Color>5</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x04]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[20]]></Exp>
+        </NextLayer>
+      </PSpec>
+      <PSpec Name="SCCP Conn Rel Comp">
+        <PSpecID>1964</PSpecID>
+        <LName>SCCP Connection Released Complete</LName>
+        <Color>6</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x05]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[7]]></Exp>
+        </NextLayer>
+      </PSpec>
+      <PSpec Name="SCCP Data Ack">
+        <PSpecID>1965</PSpecID>
+        <LName>SCCP Data Acknowledgment</LName>
+        <Color>7</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x08]]></CondExp>
+      </PSpec>
+      <PSpec Name="SCCP Unitdata">
+        <PSpecID>1966</PSpecID>
+        <LName>SCCP Unitdata</LName>
+        <Color>8</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x09]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[MLD8[4] + 5]]></Exp>
+        </NextLayer>
+        <Definitions>
+          <Define>
+            <Name>SCCPSSN</Name>
+            <Value><![CDATA[((PLD8[6] & 0x01) == 0x01) ? PLD8[9] : PLD8[7]]]></Value>
+          </Define>
+        </Definitions>
+        <Switch Name="SCCP Unitdata Switch">
+          <On>SCCPSSN</On>
+          <Link Name="SCCP Children"/>
+        </Switch>
+      </PSpec>
+      <PSpec Name="SCCP Unitdata Svc">
+        <PSpecID>1967</PSpecID>
+        <LName>SCCP Unitdata Service</LName>
+        <Color>9</Color>
+        <CondExp><![CDATA[MLD8[0] == 0xa]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[MLD8[4] + 5]]></Exp>
+        </NextLayer>
+        <Definitions>
+          <Define>
+            <Name>SCCPSSN</Name>
+            <Value><![CDATA[PLD8[7]]]></Value>
+          </Define>
+        </Definitions>
+        <Switch Name="SCCP Unitdata Svc Switch">
+          <On>SCCPSSN</On>
+          <Link Name="SCCP Children"/>
+        </Switch>
+      </PSpec>
+      <PSpec Name="SCCP Data Form">
+        <PSpecID>1968</PSpecID>
+        <LName>SCCP Data Form</LName>
+        <Color>10</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x06 || MLD8[0] == 0x07]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[7]]></Exp>
+        </NextLayer>
+        <Link Name="SCCP NON SSN Children"/>
+      </PSpec>
+      <PSpec Name="SCCP Exp Data">
+        <PSpecID>1969</PSpecID>
+        <LName>SCCP Expedited Data</LName>
+        <Color>11</Color>
+        <CondExp><![CDATA[MLD8[0] == 0xb]]></CondExp>
+      </PSpec>
+      <PSpec Name="SCCP Exp Data Ack">
+        <PSpecID>1970</PSpecID>
+        <LName>SCCP Expedited Data Acknowledgment</LName>
+        <Color>12</Color>
+        <CondExp><![CDATA[MLD8[0] == 0xc]]></CondExp>
+      </PSpec>
+      <PSpec Name="SCCP Reset Req">
+        <PSpecID>1971</PSpecID>
+        <LName>SCCP Reset Request</LName>
+        <Color>13</Color>
+        <CondExp><![CDATA[MLD8[0] == 0xd]]></CondExp>
+      </PSpec>
+      <PSpec Name="SCCP Reset Conf">
+        <PSpecID>1972</PSpecID>
+        <LName>SCCP Reset Confirmation</LName>
+        <Color>14</Color>
+        <CondExp><![CDATA[MLD8[0] == 0xe]]></CondExp>
+      </PSpec>
+      <PSpec Name="SCCP PDU Err">
+        <PSpecID>1973</PSpecID>
+        <LName>SCCP Protocol Data Unit Error</LName>
+        <Color>15</Color>
+        <CondExp><![CDATA[MLD8[0] == 0xf]]></CondExp>
+      </PSpec>
+      <PSpec Name="SCCP Inactivity Test">
+        <PSpecID>1974</PSpecID>
+        <LName>SCCP Inactivity Test</LName>
+        <Color>16</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x10]]></CondExp>
+      </PSpec>
+      <PSpec Name="SCCP Ext Unitdata">
+        <PSpecID>1975</PSpecID>
+        <LName>SCCP Extended Unitdata</LName>
+        <Color>5</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x11]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[MLD8[5] + 5]]></Exp>
+        </NextLayer>
+        <Definitions>
+          <Define>
+            <Name>SCCPSSN</Name>
+            <Value><![CDATA[((PLD8[8] & 0x01) == 0x01) ? PLD8[11] : PLD8[9]]]></Value>
+          </Define>
+        </Definitions>
+        <Switch Name="SCCP Ext Unitdata Switch">
+          <On>SCCPSSN</On>
+          <Link Name="SCCP Children"/>
+        </Switch>
+      </PSpec>
+      <PSpec Name="SCCP Ext Unitdata Svc">
+        <PSpecID>1976</PSpecID>
+        <LName>SCCP Extended Unitdata Service</LName>
+        <Color>6</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x12]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[MLD8[5] + 5]]></Exp>
+        </NextLayer>
+        <Definitions>
+          <Define>
+            <Name>SCCPSSN</Name>
+            <Value><![CDATA[((PLD8[8] & 0x01) == 0x01) ? PLD8[11] : PLD8[9]]]></Value>
+          </Define>
+        </Definitions>
+        <Switch Name="SCCP Ext Unitdata Svc Switch">
+          <On>SCCPSSN</On>
+          <Link Name="SCCP Children"/>
+        </Switch>
+      </PSpec>
+      <PSpec Name="SCCP Long Unitdata">
+        <PSpecID>1977</PSpecID>
+        <LName>SCCP Long Unitdata</LName>
+        <Color>7</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x13]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[MLD16[7] + 10]]></Exp>
+        </NextLayer>
+        <Definitions>
+          <Define>
+            <Name>SCCPSSN</Name>
+            <Value><![CDATA[((PLD8[12] & 0x01) == 0x01) ? PLD8[15] : PLD8[13]]]></Value>
+          </Define>
+        </Definitions>
+        <Switch Name="SCCP Long Unitdata Switch">
+          <On>SCCPSSN</On>
+          <Link Name="SCCP Children"/>
+        </Switch>
+      </PSpec>
+      <PSpec Name="SCCP Long Unitdata Svc">
+        <PSpecID>1978</PSpecID>
+        <LName>SCCP Long Unitdata Service</LName>
+        <Color>8</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x14]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[MLD16[7] + 10]]></Exp>
+        </NextLayer>
+        <Definitions>
+          <Define>
+            <Name>SCCPSSN</Name>
+            <Value><![CDATA[((PLD8[12] & 0x01) == 0x01) ? PLD8[15] : PLD8[13]]]></Value>
+          </Define>
+        </Definitions>
+        <Switch Name="SCCP Long Unitdata Svc Switch">
+          <On>SCCPSSN</On>
+          <Link Name="SCCP Children"/>
+        </Switch>
+      </PSpec>
+    </PSpec>
+  </PSpec>
+  <PSpec Name="SCCP Children" Type="CommonTable">
+    <PSpec Name="SCCP Management">
+      <PSpecID>2014</PSpecID>
+      <Desc/>
+      <Color>15</Color>
+      <CondSwitch>1</CondSwitch>
+    </PSpec>
+    <PSpec Name="Reserved by SCCP">
+      <PSpecID>2013</PSpecID>
+      <LName>Reserved for ITU-T Allocation</LName>
+      <Desc/>
+      <Color>22</Color>
+      <CondSwitch>2</CondSwitch>
+    </PSpec>
+    <PSpec Name="ISUP">
+      <PSpecID>1945</PSpecID>
+      <Desc/>
+      <Color>13</Color>
+      <CondSwitch>3</CondSwitch>
+    </PSpec>
+    <PSpec Name="TUP">
+      <PSpecID>1944</PSpecID>
+      <LName>Telephone User Part</LName>
+      <Desc/>
+      <Color>9</Color>
+      <CondSwitch>4</CondSwitch>
+    </PSpec>
+    <PSpec Name="MAP">
+      <PSpecID>2029</PSpecID>
+      <LName>Mobile Application Part</LName>
+      <Desc/>
+      <Color>4</Color>
+      <CondSwitch>5</CondSwitch>
+      <!-- <Link Name="TCAP Child"/> if this is uncommented pspecs stops working -->
+    </PSpec>
+    <PSpec Name="HLR">
+      <PSpecID>2016</PSpecID>
+      <Desc>The Home Location Register is the main database of permanent subscriber information for a mobile network. The HLR is an integral component of CDMA (code division multiple access), TDMA (time division multiple access), and GSM (Global System for Mobile communications) networks.</Desc>
+      <LName>Home Location Register</LName>
+      <Color>5</Color>
+      <Desc/>
+      <CondSwitch>6</CondSwitch>
+      <Link Name="TCAP Child"/>
+    </PSpec>
+    <PSpec Name="VLR">
+      <PSpecID>2025</PSpecID>
+      <LName>VLR-MAP</LName>
+      <Desc>The Visitor Location Register Mobile Application Part (VLR-MAP) is an SS7 application layer protocol that gives access to the Visitor Location Register (VLR). The VLR is a database that contains information about subscribers roaming within a mobile switching center's location area. Its primary role is to minimize the number of queries that MSCs have to make to the Home Location Register (HLR).</Desc>
+      <Color>6</Color>
+      <CondSwitch>7</CondSwitch>
+      <Link Name="TCAP Child"/>
+    </PSpec>
+    <PSpec Name="MSC">
+      <PSpecID>2017</PSpecID>
+      <LName>Mobile Switching Center</LName>
+      <Desc>Mobile Switching Center is the centerpiece of the Network Switching System (NSS), handling tasks such as call setup, release, and routing.</Desc>
+      <Color>7</Color>
+      <CondSwitch>8</CondSwitch>
+      <Link Name="TCAP Child"/>
+    </PSpec>
+    <PSpec Name="Equip Id Centre">
+      <PSpecID>2026</PSpecID>
+      <LName>Equipment Identifier Centre</LName>
+      <Desc/>
+      <Color>8</Color>
+      <CondSwitch>9</CondSwitch>
+    </PSpec>
+    <PSpec Name="Auth Centre">
+      <PSpecID>2015</PSpecID>
+      <LName>Authentication Centre</LName>
+      <Desc/>
+      <Color>9</Color>
+      <CondSwitch>10</CondSwitch>
+    </PSpec>
+    <PSpec Name="ISDN Sup Svcs">
+      <PSpecID>2028</PSpecID>
+      <LName>ISDN Supplementary Services</LName>
+      <Desc/>
+      <Color>10</Color>
+      <CondSwitch>11</CondSwitch>
+    </PSpec>
+    <PSpec Name="Res. Intl Use">
+      <PSpecID>2030</PSpecID>
+      <LName>Reserved for International Use</LName>
+      <Desc/>
+      <Color>11</Color>
+      <CondSwitch>12</CondSwitch>
+    </PSpec>
+    <PSpec Name="Bband ISDN E2E Apps">
+      <PSpecID>2031</PSpecID>
+      <LName>Broadband ISDN Edge-to-Edge Applications</LName>
+      <Desc/>
+      <Color>12</Color>
+      <CondSwitch>13</CondSwitch>
+    </PSpec>
+    <PSpec Name="TC Test Resp">
+      <PSpecID>2032</PSpecID>
+      <LName>TC Test Responder</LName>
+      <Desc/>
+      <Color>13</Color>
+      <CondSwitch>14</CondSwitch>
+    </PSpec>
+    <PSpec Name="RANAP">
+      <PSpecID>1952</PSpecID>
+      <LName>RANAP</LName>
+      <Desc>The Radio Access Network Application Part protocol is used in Universal Mobile Telecommunications System (UMTS) messaging for signaling between the Core Network, which can be a Mobile Switching Center (MSC) or the Universal Terrestrial Radio Access Network (UTRAN). For further details see 3GPP in TS 25.413</Desc>
+      <Color>14</Color>
+      <CondSwitch>142</CondSwitch>
+      <NextLayer>
+        <!--<Exp><![CDATA[MLD16[7] == 0x0010 ? 38 : 11]]></Exp> This does not work with Long Unitdata! Why? -->
+        <Exp><![CDATA[11]]></Exp>
+      </NextLayer>
+      <Link Name="SS7 Children"/>
+    </PSpec>
+    <PSpec Name="RNSAP">
+      <PSpecID>2019</PSpecID>
+      <LName>RNSAP</LName>
+      <Desc/>
+      <Color>16</Color>
+      <CondSwitch>143</CondSwitch>
+    </PSpec>
+    <PSpec Name="CAP">
+      <PSpecID>1957</PSpecID>
+      <Desc>The CAMEL Application Part is a signaling protocol. Specifically, a Remote Operations Service Element (ROSE) user protocol, used as part of the CAMEL framework, which provides tools for operators to define additional features for standard GSM services/UMTS services, and is layered on top of the Transaction Capabilities Application Part (TCAP).</Desc>
+      <Color>17</Color>
+      <CondSwitch>146</CondSwitch>
+      <PSpec Name="Camel">
+        <PSpecID>2065</PSpecID>
+        <Desc>Camel is a signaling protocol used in the Intelligent Network (IN) architecture which provides tools for operators to define additional features for standard GSM services/UMTS services.</Desc>
+        <Color>9</Color>
+      </PSpec>
+    </PSpec>
+    <PSpec Name="PCAP">
+      <PSpecID>2009</PSpecID>
+      <Desc/>
+      <Color>18</Color>
+      <CondSwitch>249</CondSwitch>
+    </PSpec>
+    <PSpec Name="BSC BSSAP-LE">
+      <PSpecID>2020</PSpecID>
+      <Desc/>
+      <Color>19</Color>
+      <CondSwitch>250</CondSwitch>
+      <!-- <Link Name="BSSAP Children"/>  if this is uncommented pspecs stops working -->
+    </PSpec>
+    <PSpec Name="BSSAP-LE">
+      <PSpecID>2021</PSpecID>
+      <LName>BSSAP-LE</LName>
+      <Desc>The Base Station System Application Part LE is an extension to the BSSAP (Base Station System Application Part) that contains messages and parameters specific in the support of LCS (Location Services).</Desc>
+      <Color>20</Color>
+      <CondSwitch>251</CondSwitch>
+      <Link Name="BSSAP Children"/>
+    </PSpec>
+    <PSpec Name="SMLC BSSAP-LE">
+      <PSpecID>2022</PSpecID>
+      <LName>SMLC</LName>
+      <Desc/>
+      <Color>21</Color>
+      <CondSwitch>252</CondSwitch>
+      <!-- <Link Name="BSSAP Children"/>  if this is uncommented pspecs stops working -->
+    </PSpec>
+    <PSpec Name="BSS O/M-A">
+      <PSpecID>2023</PSpecID>
+      <LName>BSS O/M-A-Interface</LName>
+      <Desc/>
+      <Color>22</Color>
+      <CondSwitch>253</CondSwitch>
+    </PSpec>
+    <PSpec Name="TCAP-A">
+      <PSpecID>2018</PSpecID>
+      <LName>Transaction Capabilities Application Part - A Interface</LName>
+      <Desc>The Transaction Capabilities Application Part - A Interface is the protocol used to communicate between the Base Station Control (BSC) and the Mobile Switching Center (MSC).</Desc>
+      <Color>3</Color>
+      <CondSwitch>254</CondSwitch>
+      <Link Name="BSSAP Children"/>
+    </PSpec>
+  </PSpec>
+  <PSpec Name="SCCP NON SSN Children" Type="CommonTable">
+    <PSpec Name="RANAP">
+      <PSpecID>1952</PSpecID>
+      <Color>14</Color>
+      <CondExp><![CDATA[((MLD8[0] & 0xc0 == 0xc0 || MLD8[0] & 0xc0 == 0x80 || MLD8[0] & 0xc0 == 0x40 || MLD8[0] & 0xc0 == 0x00) && MLD8[0] & 0x3f == 0 && MLD8[2] & 0x3f == 0 && MLD8[1] <= 49 && MLD8[3] >= 0) || (MLD8[0] == 0x20 && MLD8[2] == 0) || (MLD8[0] == 0x60 && MLD8[2] == 0)]]></CondExp>
+      <NextLayer>
+        <Exp><![CDATA[MLD16[7] == 0x0010 ? 38 : 11]]></Exp>
+      </NextLayer>
+      <Link Name="SS7 Children"/>
+    </PSpec>
+    <PSpec Name="BSSAP">
+      <PSpecID>1953</PSpecID>
+      <LName>Base Station Subsystem Application Part</LName>
+      <Desc>The Base Station Subsystem Application Part is a protocol in Signaling system 7 used by the Mobile Switching Center (MSC) and the Base station subsystem (BSS) to communicate with each other using signaling messages supported by the MTP and connection-oriented services of the SCCP.</Desc>
+      <Color>15</Color>
+      <CondExp><![CDATA[(MLD8[0] == 0 && MLD8[2] <= 0x79) || (MLD8[0] == 1 && MLD8[1] >= 0 && MLD8[2] != 0 && MLD8[3] & 0x0f <= 0x0f && MLD8[4] & 0x3f != 0)]]></CondExp>
+      <NextLayer>
+        <Exp><![CDATA[2]]></Exp>
+      </NextLayer>
+      <Link Name="SS7 Children"/>
+    </PSpec>
+  </PSpec>
+  <PSpec Name="TCAP Child" Type="CommonTable">
+    <PSpec Name="TCAP">
+      <PSpecID>2070</PSpecID>
+      <LName>Transaction Capabilities Application Part</LName>
+      <Desc>The Transaction Capabilities Application Part is a protocol that enables the deployment of advanced intelligent network services by supporting non-circuit related information exchange between signaling points using the SCCP connectionless service. Its primary purpose is to facilitate multiple concurrent dialogs between the same sub-systems on the same machines, using Transaction IDs to differentiate these, similar to the way TCP ports facilitate multiplexing connections between the same IP addresses on the Internet. See the ITU Q.771-Q.775 recommendations for more details</Desc>
+      <Color>2</Color>
+      <Link Name="TCAP Messages"/>
+    </PSpec>
+  </PSpec>
+  <PSpec Name="TCAP Messages" Type="CommonTable">
+    <PSpec Name="Unidir TCAP">
+      <PSpecID>2071</PSpecID>
+      <LName>Unidirectional - TCAP</LName>
+      <Color>3</Color>
+      <CondExp><![CDATA[MLD8[0] == 0x61]]></CondExp>
+      <NextLayer>
+        <Exp><![CDATA[20]]></Exp>
+      </NextLayer>
+      <!-- <Link Name="TCAP Children"/>makes problems when uncommented -->
+    </PSpec>
+    <PSpec Name="Begin TCAP">
+      <PSpecID>2072</PSpecID>
+      <LName>Begin - TCAP</LName>
+      <Desc>The Begin Transaction Capabilities Application Part is the first primitive of the TCAP protocol sent between the application and the local TCAP stack that starts a dialog.</Desc>
+      <Color>4</Color>
+      <CondExp><![CDATA[MLD8[0] == 0x62]]></CondExp>
+      <NextLayer>
+        <Exp><![CDATA[38]]></Exp>
+      </NextLayer>
+      <!-- <Link Name="TCAP Children"/>-->
+      <!--makes problems when uncommented -->
+      <PSpec Name="GSM Mobile App">
+        <PSpecID>2076</PSpecID>
+        <LName>GSM Mobile Application Part</LName>
+        <SName>GSM MAP</SName>
+        <Desc>The GSM Mobile Application Part is a Signaling System No.7 (SS7) protocol providing an application layer for GSM nodes to allow communication between them.</Desc>
+        <Color>3</Color>
+        <CondExp><![CDATA[MLD8[0] & 0xf0 == 0xa0]]></CondExp>
+      </PSpec>
+    </PSpec>
+    <PSpec Name="End TCAP">
+      <PSpecID>2073</PSpecID>
+      <Desc>The End Transaction Capabilities Application Part is the last primitive of the TCAP protocol sent between the application and the local TCAP stack on an existing dialog.</Desc>
+      <LName>End - TCAP</LName>
+      <Color>5</Color>
+      <CondExp><![CDATA[MLD8[0] == 0x64]]></CondExp>
+      <NextLayer>
+        <Exp><![CDATA[50]]></Exp>
+      </NextLayer>
+      <!-- <Link Name="TCAP Children"/>-->
+      <!--makes problems when uncommented -->
+      <PSpec Name="GSM Mobile App">
+        <PSpecID>2076</PSpecID>
+        <LName>GSM Mobile Application Part</LName>
+        <SName>GSM MAP</SName>
+        <Color>3</Color>
+        <CondExp><![CDATA[MLD8[0] & 0xf0 == 0xa0]]></CondExp>
+      </PSpec>
+    </PSpec>
+    <PSpec Name="Continue TCAP">
+      <PSpecID>2074</PSpecID>
+      <Desc>The Continue Transaction Capabilities Application Part is a primitive of the TCAP protocol sent between the application and the local TCAP stack that sends a subsequent primitive on an existing dialog.</Desc>
+      <LName>Continue - TCAP</LName>
+      <Color>6</Color>
+      <CondExp><![CDATA[MLD8[0] == 0x65]]></CondExp>
+      <NextLayer>
+        <Exp><![CDATA[(MLD8[1] & 0x80 == 0x80) ? 3 : 2]]></Exp>
+      </NextLayer>
+      <Link Name="TCAP Children"/>
+    </PSpec>
+    <PSpec Name="Abort TCAP">
+      <PSpecID>2075</PSpecID>
+      <Desc>The Abort Transaction Capabilities Application Part is a primitive sent between the application and the local TCAP stack that closes the dialog due to an error.</Desc>
+      <LName>Abort - TCAP</LName>
+      <Color>7</Color>
+      <CondExp><![CDATA[MLD8[0] == 0x67]]></CondExp>
+      <NextLayer>
+        <Exp><![CDATA[(MLD8[1] & 0x80 == 0x80) ? ((MLD8[1] & 0x3f << 7) + (MLD8[2] & 0x3f)) : MLD8[1]]]></Exp>
+      </NextLayer>
+    </PSpec>
+  </PSpec>
+  <PSpec Name="TCAP Children" Type="CommonTable">
+    <PSpec Name="TCAP-OrigTransID TLV">
+      <PSpecID>2078</PSpecID>
+      <LName>TCAP - OrigTransactionID</LName>
+      <SName>TCAP-OTID</SName>
+      <Color>9</Color>
+      <CondExp><![CDATA[MLD8[0] & 0x3f == 0x08]]></CondExp>
+      <NextLayer>
+        <Exp><![CDATA[MLD8[1] + 2]]></Exp>
+      </NextLayer>
+      <PSpec Name="TCAP-DestTransID TLV">
+        <PSpecID>2079</PSpecID>
+        <LName>TCAP - DestTransactionID</LName>
+        <SName>TCAP-DTID</SName>
+        <Color>10</Color>
+        <CondExp><![CDATA[MLD8[0] & 0x3f == 0x09]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[MLD8[1] + 2]]></Exp>
+        </NextLayer>
+        <PSpec Name="TCAP-ComponentPortion TLV">
+          <PSpecID>2081</PSpecID>
+          <LName>TCAP - ComponentPortion</LName>
+          <SName>TCAP-CP</SName>
+          <Color>11</Color>
+          <CondExp><![CDATA[MLD8[0] == 0x6c]]></CondExp>
+          <NextLayer>
+            <Exp><![CDATA[MLD8[1] & 0x80 == 0x80 ? 3 : 2]]></Exp>
+          </NextLayer>
+          <Link Name="SS7 Children"/>
+          <!--<PSpec Name="GSM Mobile Application">
+						<PSpecID>2068</PSpecID>
+						<LName>GSM Mobile Application Part</LName>
+						<SName>GSM MAP</SName>
+						<Color>9</Color>
+						<CondExp><![CDATA[MLD8[0] & 0xf0 == 0xa0]]></CondExp>
+					</PSpec>-->
+        </PSpec>
+        <PSpec Name="TCAP-DialoguePortion TLV">
+          <PSpecID>2080</PSpecID>
+          <LName>TCAP - DialoguePortion</LName>
+          <SName>TCAP-DP</SName>
+          <Color>12</Color>
+          <CondExp><![CDATA[MLD8[0] == 0x6b]]></CondExp>
+          <NextLayer>
+            <Exp><![CDATA[MLD8[1] + 2]]></Exp>
+          </NextLayer>
+          <PSpec Name="TCAP-ComponentPortion TLV">
+            <PSpecID>2081</PSpecID>
+            <LName>TCAP - ComponentPortion</LName>
+            <SName>TCAP-CP</SName>
+            <Color>11</Color>
+            <CondExp><![CDATA[MLD8[0] == 0x6c]]></CondExp>
+            <NextLayer>
+              <Exp><![CDATA[MLD8[1] & 0x80 == 0x80 ? 3 : 2]]></Exp>
+            </NextLayer>
+            <Link Name="SS7 Children"/>
+            <!--<PSpec Name="GSM Mobile Application">
+							<PSpecID>2068</PSpecID>
+							<LName>GSM Mobile Application Part</LName>
+							<SName>GSM MAP</SName>
+							<Color>9</Color>
+							<CondExp><![CDATA[MLD8[0] & 0xf0 == 0xa0]]></CondExp>
+						</PSpec>-->
+          </PSpec>
+        </PSpec>
+      </PSpec>
+      <PSpec Name="TCAP-DialoguePortion TLV">
+        <PSpecID>2082</PSpecID>
+        <LName>TCAP - DialoguePortion</LName>
+        <SName>TCAP-DP</SName>
+        <Color>12</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x6b]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[MLD8[1] + 2]]></Exp>
+        </NextLayer>
+        <PSpec Name="TCAP-ComponentPortion TLV">
+          <PSpecID>2083</PSpecID>
+          <LName>TCAP - ComponentPortion</LName>
+          <SName>TCAP-CP</SName>
+          <Color>11</Color>
+          <CondExp><![CDATA[MLD8[0] == 0x6c]]></CondExp>
+          <NextLayer>
+            <Exp><![CDATA[MLD8[1] & 0x80 == 0x80 ? 3 : 2]]></Exp>
+          </NextLayer>
+        </PSpec>
+        <!-- <Link Name="TCAP Children"/>-->
+        <!--makes problems when uncommented -->
+      </PSpec>
+      <PSpec Name="TCAP-ComponentPortion TLV">
+        <PSpecID>2083</PSpecID>
+        <LName>TCAP - ComponentPortion</LName>
+        <SName>TCAP-CP</SName>
+        <Color>11</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x6c]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[MLD8[1] & 0x80 == 0x80 ? 3 : 2]]></Exp>
+        </NextLayer>
+        <!-- <Link Name="TCAP Children"/>-->
+        <!--makes problems when uncommented -->
+      </PSpec>
+    </PSpec>
+    <PSpec Name="TCAP-DestTransID TLV">
+      <PSpecID>2086</PSpecID>
+      <LName>TCAP - DestTransactionID</LName>
+      <SName>TCAP-DTID</SName>
+      <Color>10</Color>
+      <CondExp><![CDATA[MLD8[0] & 0x3f == 0x09]]></CondExp>
+      <NextLayer>
+        <Exp><![CDATA[MLD8[1] + 2]]></Exp>
+      </NextLayer>
+      <PSpec Name="TCAP-DialoguePortion TLV">
+        <PSpecID>2084</PSpecID>
+        <LName>TCAP - DialoguePortion</LName>
+        <SName>TCAP-DP</SName>
+        <Color>12</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x6b]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[MLD8[1] + 2]]></Exp>
+        </NextLayer>
+        <PSpec Name="TCAP-ComponentPortion TLV">
+          <PSpecID>2085</PSpecID>
+          <LName>TCAP - ComponentPortion</LName>
+          <SName>TCAP-CP</SName>
+          <Color>11</Color>
+          <CondExp><![CDATA[MLD8[0] == 0x6c]]></CondExp>
+          <NextLayer>
+            <Exp><![CDATA[MLD8[1] & 0x80 == 0x80 ? 3 : 2]]></Exp>
+          </NextLayer>
+          <!-- <Link Name="TCAP Children"/>-->
+          <!--makes problems when uncommented -->
+        </PSpec>
+      </PSpec>
+      <PSpec Name="TCAP-ComponentPortion TLV">
+        <PSpecID>2085</PSpecID>
+        <LName>TCAP - ComponentPortion</LName>
+        <SName>TCAP-CP</SName>
+        <Color>11</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x6c]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[MLD8[1] & 0x80 == 0x80 ? 3 : 2]]></Exp>
+        </NextLayer>
+        <!-- <Link Name="TCAP Children"/>-->
+        <!--makes problems when uncommented -->
+      </PSpec>
+    </PSpec>
+    <PSpec Name="TCAP-DialoguePortion TLV">
+      <PSpecID>2087</PSpecID>
+      <LName>TCAP - DialoguePortion</LName>
+      <SName>TCAP-DP</SName>
+      <Color>12</Color>
+      <CondExp><![CDATA[MLD8[0] == 0x6b]]></CondExp>
+      <NextLayer>
+        <Exp><![CDATA[MLD8[1] + 2]]></Exp>
+      </NextLayer>
+      <PSpec Name="TCAP-ComponentPortion TLV">
+        <PSpecID>2088</PSpecID>
+        <LName>TCAP - ComponentPortion</LName>
+        <SName>TCAP-CP</SName>
+        <Color>11</Color>
+        <CondExp><![CDATA[MLD8[0] == 0x6c]]></CondExp>
+        <NextLayer>
+          <Exp><![CDATA[MLD8[1] & 0x80 == 0x80 ? 3 : 2]]></Exp>
+        </NextLayer>
+        <!-- <Link Name="TCAP Children"/>-->
+        <!--makes problems when uncommented -->
+      </PSpec>
+    </PSpec>
+    <PSpec Name="TCAP-ComponentPortion TLV">
+      <PSpecID>2088</PSpecID>
+      <LName>TCAP - ComponentPortion</LName>
+      <SName>TCAP-CP</SName>
+      <Color>11</Color>
+      <CondExp><![CDATA[MLD8[0] == 0x6c]]></CondExp>
+      <NextLayer>
+        <Exp><![CDATA[MLD8[1] & 0x80 == 0x80 ? 3 : 2]]></Exp>
+      </NextLayer>
+      <!-- <Link Name="TCAP Children"/>-->
+      <!--makes problems when uncommented -->
+    </PSpec>
+  </PSpec>
+  <PSpec Name="BSSAP Children" Type="CommonTable">
+    <PSpec Name="BSSAP">
+      <PSpecID>1953</PSpecID>
+      <Desc>BSSAP is a protocol in Signaling System 7 used by the Mobile Switching Center (MSC) and the Base Station Subsystem (BSS) to communicate with each other using signaling messages supported by the MTP and connection-oriented services of the SCCP.</Desc>
+      <Color>15</Color>
+      <NextLayer>
+        <Exp><![CDATA[2]]></Exp>
+      </NextLayer>
+      <Link Name="SS7 Children"/>
+    </PSpec>
+  </PSpec>
+  <PSpec Name="SS7 Children" Type="CommonTable">
+    <PSpec Name="GSM A DTAP">
+      <PSpecID>2063</PSpecID>
+      <LName>GSM A Interface DTAP</LName>
+      <Desc>GSM A DTAP is one part of the GSM specific protocol BSSAP. It is designed to signal over the A interface, which is the interface between the MSC and the BSC. DTAP carries messages related to call control and mobility management between two users.</Desc>
+      <Color>1</Color>
+      <ParentSpecific Parent="RANAP">
+        <CondExp><![CDATA[PLD8[1] == 0x14 || PLD8[1] == 0x13]]></CondExp>
+      </ParentSpecific>
+      <ParentSpecific Parent="BSSAP">
+        <CondExp><![CDATA[PLD8[0] == 0x01]]></CondExp>
+      </ParentSpecific>
+      <ParentSpecific Parent="TCAP-ComponentPortion TLV">
+        <CondExp><![CDATA[PLD8[1] > 256]]></CondExp>
+      </ParentSpecific>
+      <NextLayer>
+        <Exp><![CDATA[4]]></Exp>
+      </NextLayer>
+      <Link Name="GSM DTAP Children"/>
+    </PSpec>
+    <PSpec Name="GSM A BSSMAP">
+      <PSpecID>2066</PSpecID>
+      <LName>GSM A Interface BSSMAP</LName>
+      <Desc>GSM A BSSMAP is one part of the GSM-specific protocol BSSAP. It is designed to signal over the A interface, which is the interface between the MSC and the BSC. BSSMAP carries messages related to radio resource and the Base Station Controller (BSC) management.</Desc>
+      <Color>2</Color>
+      <ParentSpecific Parent="RANAP">
+        <CondExp><![CDATA[PLD8[1] > 256]]></CondExp>
+      </ParentSpecific>
+      <ParentSpecific Parent="BSSAP">
+        <CondExp><![CDATA[PLD8[0] == 0x00]]></CondExp>
+      </ParentSpecific>
+      <ParentSpecific Parent="TCAP-ComponentPortion TLV">
+        <CondExp><![CDATA[PLD8[1] > 256]]></CondExp>
+      </ParentSpecific>
+      <NextLayer>
+        <Exp><![CDATA[13]]></Exp>
+      </NextLayer>
+      <!-- <Link Name="GSM BSSMAP Children"/> if this is uncommented pspecs stops working-->
+    </PSpec>
+    <PSpec Name="GSM Mobile App">
+      <PSpecID>2089</PSpecID>
+      <LName>GSM Mobile Application Part</LName>
+      <SName>GSM MAP</SName>
+      <Desc>Global System for Mobile communications Mobile Application Part provides an application layer for the various nodes in the GSM to communicate with each other in order to provide services to users.</Desc>
+      <Color>3</Color>
+      <ParentSpecific Parent="RANAP">
+        <CondExp><![CDATA[PLD8[1] > 256]]></CondExp>
+      </ParentSpecific>
+      <ParentSpecific Parent="BSSAP">
+        <CondExp><![CDATA[PLD8[0] > 256]]></CondExp>
+      </ParentSpecific>
+      <ParentSpecific Parent="TCAP-ComponentPortion TLV">
+        <CondExp><![CDATA[MLD8[0] & 0xf0 == 0xa0]]></CondExp>
+      </ParentSpecific>
+    </PSpec>
+  </PSpec>
+  <PSpec Name="GSM BSSMAP Children" Type="CommonTable">
+    <PSpec Name="GSM A DTAP">
+      <PSpecID>2063</PSpecID>
+      <LName>GSM A-Interface DTAP</LName>
+      <Desc>The Global System for Mobile communications A-Interface Direct Transfer Application Part protocol is used to transfer call control and mobility management layer 3 messages between the Base Station Controller (BSC) and the Mobile Switching Center (MSC) without any analysis of message content.</Desc>
+      <Color>4</Color>
+      <CondExp><![CDATA[PLD8[0] == 0x57]]></CondExp>
+      <NextLayer>
+        <Exp><![CDATA[4]]></Exp>
+      </NextLayer>
+      <Link Name="GSM DTAP Children"/>
+    </PSpec>
+  </PSpec>
+  <PSpec Name="GSM DTAP Children" Type="CommonTable">
+    <PSpec Name="GSM A RP">
+      <PSpecID>2064</PSpecID>
+      <LName>GSM A-Interface RP</LName>
+      <Desc>Global System for Mobile communication A-Interface Relay Protocol sends short messages in the Global System for Mobile communications network between the Mobile Switching Center (MSC) and Base Station Controller (BSC).</Desc>
+      <Color>5</Color>
+      <CondExp><![CDATA[PLD8[1] == 0x01]]></CondExp>
+    </PSpec>
   </PSpec>
   <PSpec Name="GRE Children" Type="CommonTable">
     <PSpec Name="IP">
       <PSpecID>1000</PSpecID>
       <DescID>8300</DescID>
       <CondSwitch>0x0800</CondSwitch>
       <CondSwitch>0xFFFF</CondSwitch>
@@ -2862,17 +4445,17 @@
       <PSpec Name="IP Fragment" Sort="First">
         <PSpecID>1001</PSpecID>
         <LName>Fragmented IP</LName>
         <CondExp><![CDATA[(PLD16[6] & 0x1fff) != 0]]></CondExp>
       </PSpec>
     </PSpec>
     <PSpec Name="GRE EType2">
-      <PSpecID>43</PSpecID>
       <NotChild Name="IEEE 802.3"/>
       <NotChild Name="802.11 Data"/>
+      <PSpecID>43</PSpecID>
       <DescID>2</DescID>
       <CondSwitch>0x6558</CondSwitch>
       <NextLayer>
         <Exp><![CDATA[14]]></Exp>
       </NextLayer>
       <Definitions>
         <Define>
@@ -2940,14 +4523,15 @@
       <CondSwitch>0x8360</CondSwitch>
       <CondSwitch>0x8370</CondSwitch>
       <NextLayer>
         <Exp><![CDATA[24]]></Exp>
       </NextLayer>
     </PSpec>
     <PSpec Name="WCCP FWD">
+      <NotChild Name="GENEVE"/>
       <PSpecID>5901</PSpecID>
       <LName>Web Cache Communication Protocol GRE Forwarding</LName>
       <SName>WCCP GRE FWD</SName>
       <Desc>Web Cache Communication Protocol (WCCP) is a Cisco-developed content-routing protocol that provides a mechanism to redirect traffic flows in real-time.</Desc>
       <Color>14</Color>
       <CondSwitch>0x883E</CondSwitch>
       <NextLayer>
@@ -2968,19 +4552,20 @@
           <PSpecID>1001</PSpecID>
           <LName>Fragmented IP</LName>
           <CondExp><![CDATA[(PLD16[6] & 0x1fff) != 0]]></CondExp>
         </PSpec>
       </PSpec>
     </PSpec>
     <PSpec Name="ERSPAN">
-      <PSpecID>5902</PSpecID>
       <NotChild Name="ERSPAN"/>
       <NotChild Name="GTP"/>
       <NotChild Name="IEEE 802.3"/>
       <NotChild Name="802.11 Data"/>
+      <NotChild Name="GENEVE"/>
+      <PSpecID>5902</PSpecID>
       <LName>ERSPAN</LName>
       <SName>ERSPAN</SName>
       <Desc>ERSPAN transports mirrored traffic over an IP network. The traffic is encapsulated at the source router and is transferred across the network. The packet is unencapsulated at the destination router and then sent to the destination interface.</Desc>
       <Color>10</Color>
       <CondSwitch>0x88BE</CondSwitch>
       <CondSwitch>0x22EB</CondSwitch>
       <NextLayer>
@@ -3001,14 +4586,90 @@
         </Definitions>
         <Switch Name="EType2 EthernetType Switch">
           <On>EthernetType</On>
           <Link Name="Ethernet Type 2 Children"/>
         </Switch>
       </PSpec>
     </PSpec>
+    <PSpec Name="MPLS">
+      <PSpecID>8330</PSpecID>
+      <NotChild Name="MPLS"/>
+      <NotChild Name="GENEVE"/>
+      <LName>Multi-Protocol Label Switching</LName>
+      <Desc>In a Multi-Protocol Label Switching (MPLS) network, incoming packets are assigned a label by a label edge router (LER). Packets are forwarded along a label switch path (LSP) where each label switch router (LSR) makes forwarding decisions based solely on the contents of the label. At each hop, the LSR strips off the existing label and applies a new label which tells the next hop how to forward the packet.</Desc>
+      <Color>3</Color>
+      <CondSwitch>0x8847</CondSwitch>
+      <CondSwitch>0x8848</CondSwitch>
+      <NextLayer>
+        <Exp><![CDATA[4]]></Exp>
+      </NextLayer>
+      <PSpec Name="Ethernet Type 2">
+        <NotChild Name="IEEE 802.3"/>
+        <NotChild Name="802.11 Data"/>
+        <NotChild Name="SNAP"/>
+        <NotChild Name="VXLAN"/>
+        <NotChild Name="IPv6"/>
+        <NotChild Name="PPPoE"/>
+        <NotChild Name="802.1ah"/>
+        <NotChild Name="VLAN"/>
+        <NotChild Name="IPinIP"/>
+        <NotChild Name="iVXLAN"/>
+        <PSpecID>34</PSpecID>
+        <LName>MPLS Ethernet Type 2</LName>
+        <SName>MPLS EType2</SName>
+        <DescID>2</DescID>
+        <CondExp><![CDATA[MLD16[12] > 1500]]></CondExp>
+        <Switch Name="EType2 EthernetType Switch">
+          <On>EthernetType</On>
+          <Link Name="Ethernet Type 2 Children"/>
+        </Switch>
+        <Definitions>
+          <Define>
+            <Name>EthernetType</Name>
+            <Value><![CDATA[PLD16[12]]]></Value>
+          </Define>
+        </Definitions>
+        <NextLayer>
+          <Exp><![CDATA[14]]></Exp>
+        </NextLayer>
+      </PSpec>
+      <PSpec Name="IEEE 802.3">
+        <NotChild Name="802.11 Data"/>
+        <NotChild Name="SNAP"/>
+        <NotChild Name="VXLAN"/>
+        <NotChild Name="IPv6"/>
+        <NotChild Name="PPPoE"/>
+        <NotChild Name="802.1ah"/>
+        <NotChild Name="VLAN"/>
+        <NotChild Name="IPinIP"/>
+        <NotChild Name="iVXLAN"/>
+        <PSpecID>35</PSpecID>
+        <LName>MPLS IEEE 802.3</LName>
+        <SName>MPLS 802.3</SName>
+        <DescID>1</DescID>
+        <CondExp><![CDATA[MLD16[12] <= 1500]]></CondExp>
+        <Definitions>
+          <Define>
+            <Name>EthernetType</Name>
+            <Value><![CDATA[PLD16[12]]]></Value>
+          </Define>
+        </Definitions>
+        <Link Name="802.2 LLC"/>
+        <NextLayer>
+          <Exp><![CDATA[14]]></Exp>
+        </NextLayer>
+      </PSpec>
+    </PSpec>
+    <PSpec Name="NHRP">
+      <PSpecID>8331</PSpecID>
+      <LName>NBMA Next Hop Resolution Protocol</LName>
+      <Desc>The Next Hop Resolution Protocol (NHRP) is an extension of the ATM ARP routing mechanism that is sometimes used to improve the efficiency of routing computer network traffic over Non-Broadcast, Multiple Access (NBMA) Networks.</Desc>
+      <Color>13</Color>
+      <CondSwitch>0x2001</CondSwitch>
+    </PSpec>
   </PSpec>
   <PSpec Name="Ethernet" Type="CommonTable">
     <PSpec Name="ARP">
       <PSpecID>500</PSpecID>
       <LName>Internet Protocol Address Resolution Protocol</LName>
       <Desc>ARP packets are used to create a link between IP logical addresses and data link physical addresses (i.e. an Ethernet address). Given an IP logical address, ARP tries to discover the underlying data link physical address. Address resolution is a normal process of higher level protocols as they are established on different types of networking media.</Desc>
       <Color>5</Color>
@@ -3040,23 +4701,24 @@
         <CondSwitch>0x88cc</CondSwitch>
       </ParentSpecific>
       <ParentSpecific Parent="SNAP">
         <CondExp><![CDATA[PLD16[6] == 0x88cc]]></CondExp>
       </ParentSpecific>
     </PSpec>
     <PSpec Name="802.1ah">
-      <PSpecID>6670</PSpecID>
       <NotChild Name="802.1ah"/>
       <NotChild Name="SNAP"/>
       <NotChild Name="WAN PPP"/>
       <NotChild Name="WAN Frame Relay"/>
       <NotChild Name="WAN X25"/>
       <NotChild Name="GRE"/>
       <NotChild Name="GTP"/>
       <NotChild Name="PPPoE"/>
+      <NotChild Name="GENEVE"/>
+      <PSpecID>6670</PSpecID>
       <LName>802.1ah (mac-in-mac)</LName>
       <Desc>Provider Backbone Bridges (PBB, known as &quot;mac-in-mac&quot;) is a set of architecture and protocols for routing over a provider's network allowing interconnection of multiple Provider Bridge Networks without losing each customer's individually defined VLANs.</Desc>
       <Color>18</Color>
       <CondSwitch>0x88e7</CondSwitch>
       <Color>4</Color>
       <NextLayer>
         <Exp><![CDATA[18]]></Exp>
@@ -3170,17 +4832,17 @@
             <Name>ProtocolID</Name>
             <Value><![CDATA[PLD8[6] == 0 || PLD8[6] == 0x2B ? PLD8[40] : PLD8[6]]]></Value>
           </Define>
         </Definitions>
         <Link Name="IPv6 Children"/>
       </PSpec>
       <PSpec Name="Ethernet Type 2">
-        <PSpecID>34</PSpecID>
         <NotChild Name="IEEE 802.3"/>
         <NotChild Name="802.11 Data"/>
+        <PSpecID>34</PSpecID>
         <LName>MPLS Ethernet Type 2</LName>
         <SName>MPLS EType2</SName>
         <DescID>2</DescID>
         <CondExp><![CDATA[MLD16[12] > 1500]]></CondExp>
         <Switch Name="EType2 EthernetType Switch">
           <On>EthernetType</On>
           <Link Name="Ethernet Type 2 Children"/>
@@ -3192,16 +4854,16 @@
           </Define>
         </Definitions>
         <NextLayer>
           <Exp><![CDATA[14]]></Exp>
         </NextLayer>
       </PSpec>
       <PSpec Name="IEEE 802.3">
-        <PSpecID>35</PSpecID>
         <NotChild Name="Ethernet Type 2"/>
+        <PSpecID>35</PSpecID>
         <LName>MPLS IEEE 802.3</LName>
         <SName>MPLS 802.3</SName>
         <DescID>1</DescID>
         <CondExp><![CDATA[MLD16[12] <= 1500]]></CondExp>
         <Definitions>
           <Define>
             <Name>EthernetType</Name>
@@ -3332,14 +4994,15 @@
         <DescID>513</DescID>
         <CondExp><![CDATA[MLD16[6] == 0x0004]]></CondExp>
       </PSpec>
     </PSpec>
     <PSpec Name="VLAN">
       <NotChild Name="VLAN"/>
       <NotChild Name="MPLS"/>
+      <NotChild Name="GENEVE"/>
       <PSpecID>40</PSpecID>
       <LName>IEEE 802.1Q VLAN</LName>
       <Desc>IEEE 802.1Q uses an internal tagging mechanism that inserts a 4-byte tag field in the original Ethernet frame itself between the Source Address and Type/Length fields.</Desc>
       <Color>17</Color>
       <ParentSpecific Parent="SNAP">
         <CondExp><![CDATA[(PLD16[2] == 0x0300) && (PLD32[4] == 0x00008100 || PLD32[4] == 0x00f88100 || PLD32[4] == 0x000088a8 || PLD32[4] == 0x00f888a8)]]></CondExp>
       </ParentSpecific>
@@ -3354,17 +5017,17 @@
       <Definitions>
         <Define>
           <Name>EthernetType</Name>
           <Value><![CDATA[MLD16[-2]]]></Value>
         </Define>
       </Definitions>
       <PSpec Name="VLAN EType2">
-        <PSpecID>38</PSpecID>
         <NotChild Name="IEEE 802.3"/>
         <NotChild Name="802.11 Data"/>
+        <PSpecID>38</PSpecID>
         <DescID>2</DescID>
         <CondExp><![CDATA[EthernetType > 1500]]></CondExp>
         <Switch Name="EType2 EthernetType Switch">
           <On>EthernetType</On>
           <Link Name="Ethernet Type 2 Children"/>
         </Switch>
       </PSpec>
@@ -3840,14 +5503,29 @@
       <PSpec Name="VTP">
         <PSpecID>2003</PSpecID>
         <LName>VLAN Trunking Protocol</LName>
         <Desc>VLAN Trunking Protocol (VTP) is a proprietary protocol from Cisco Systems that propagates the definition of Virtual Local Area Networks (VLAN) on the whole local area network.</Desc>
         <Color>3</Color>
         <CondExp><![CDATA[PLD16[6] == 0x2003]]></CondExp>
       </PSpec>
+      <PSpec Name="UDLD">
+        <PSpecID>2004</PSpecID>
+        <LName>Unidirectional Link Detection</LName>
+        <Desc>Unidirectional Link Detection (UDLD) is a data link layer protocol from Cisco Systems to monitor the physical configuration of the cables and detect unidirectional links. UDLD complements the Spanning Tree Protocol which is used to eliminate switching loops.</Desc>
+        <Color>15</Color>
+        <CondExp><![CDATA[PLD16[6] == 0x0111]]></CondExp>
+      </PSpec>
+      <PSpec Name="Miscabling Protocol">
+        <PSpecID>313</PSpecID>
+        <LName>Cisco Miscabling Protocol</LName>
+        <SName>MCP</SName>
+        <Desc>MCP provides additional protection against misconfigurations that would otherwise result in loops.</Desc>
+        <Color>15</Color>
+        <CondExp><![CDATA[PLD16[6] == 0x0139]]></CondExp>
+      </PSpec>
     </PSpec>
     <PSpec Name="LSAP">
       <PSpecID>10</PSpecID>
       <Desc>IEEE 802.2 LLC SAP Layer</Desc>
       <Color>1</Color>
       <CondExp><![CDATA[MLD16[0] != 0xaaaa]]></CondExp>
       <NextLayer>
@@ -4310,38 +5988,41 @@
       <Color>13</Color>
       <CondSwitch>9</CondSwitch>
     </PSpec>
     <PSpec Name="SSH">
       <PSpecID>1459</PSpecID>
       <LName>Secure Shell Protocol</LName>
       <Desc>SSH (Secure Shell) is a program to log into another computer over a network, to execute commands on a remote machine, and to move files from one machine to another. It provides strong authentication and secure communications over unsecured channels. It is intended as a replacement for rlogin, rsh, and rcp.</Desc>
+      <Color>5</Color>
       <CondSwitch>22</CondSwitch>
     </PSpec>
     <PSpec Name="Kerberos">
       <PSpecID>1449</PSpecID>
       <Desc>Kerberos is a network authentication protocol, developed by the Massachusetts Institute of Technology, which provides strong authentication for client-server applications by using secret-key cryptography. It uses IP port 88.</Desc>
+      <Color>6</Color>
       <CondSwitch>88</CondSwitch>
     </PSpec>
     <PSpec Name="DNS">
       <PSpecID>1413</PSpecID>
       <LName>Domain Name System Protocol</LName>
       <Desc>DNS is the TCP/IP standard protocol for mapping human-readable names into IP logical addresses. DNS servers maintain a database of associations between hierarchical names and the corresponding addresses so that people and processes may locate each other without needing to know a logical or physical address. This also allows sites to change their underlying IP address scheme without having to reconfigure every other machine on the network.</Desc>
       <Color>9</Color>
       <CondSwitch>53</CondSwitch>
       <CondSwitch>5353</CondSwitch>
     </PSpec>
     <PSpec Name="RTPS">
       <PSpecID>1494</PSpecID>
       <LName>Real-Time Publish-Subscribe</LName>
       <Desc>The Real-Time Publish-Subscribe (RTPS) Wire Protocol provides two main communication models: the publish-subscribe protocol, which transfers data from publishers to subscribers; and the Composite State Transfer (CST) protocol, which transfers state. The RTPS protocol is designed to run over an unreliable transport such as UDP/IP.</Desc>
+      <Color>8</Color>
       <CondExp><![CDATA[MLD32[0] == 0x52545053]]></CondExp>
     </PSpec>
     <PSpec Name="BOOTP">
-      <PSpecID>1414</PSpecID>
       <NotChild Name="IPv6"/>
+      <PSpecID>1414</PSpecID>
       <LName>Boot Protocol</LName>
       <Desc>BOOTP is used by BOOTP clients to notify BOOTP servers that a machine needs some configuration and an executable image to begin running. A BOOTP server typically sends an IP address for the machine to use and other configuration information including the name and location of an image file that the client should fetch into its memory in order to execute. TFTP is typically used to fetch such an image. BOOTP is most often used in diskless workstation environments.</Desc>
       <Color>10</Color>
       <CondSwitch>67</CondSwitch>
       <NextLayer>
         <Exp><![CDATA[236]]></Exp>
       </NextLayer>
@@ -4470,14 +6151,36 @@
     </PSpec>
     <PSpec Name="Lotus Notes">
       <PSpecID>1457</PSpecID>
       <Desc>Lotus Notes is a client-server groupware product sold by Lotus. It uses IP port 1352.</Desc>
       <Color>13</Color>
       <CondSwitch>1352</CondSwitch>
     </PSpec>
+    <PSpec Name="NetFlow">
+      <PSpecID>1495</PSpecID>
+      <LName>Cisco NetFlow</LName>
+      <Desc>NetFlow is a protocol introduced by Cisco and used by network devices (primarily switches and routers) to export IP flow statistics for analysis.</Desc>
+      <CondSwitch>2055</CondSwitch>
+      <CondSwitch>4739</CondSwitch>
+      <CondSwitch>4740</CondSwitch>
+      <CondSwitch>5229</CondSwitch>
+      <CondSwitch>9995</CondSwitch>
+      <CondExp><![CDATA[ MLD16[0] <= 9 ]]></CondExp>
+    </PSpec>
+    <PSpec Name="IPFIX">
+      <PSpecID>4739</PSpecID>
+      <LName>IPFIX</LName>
+      <Desc>Internet Protocol Flow Information Export (IPFIX) is an IETF protocol, which was created based on the need for a common, universal standard of export for Internet Protocol flow information from routers, probes and other devices that are used by mediation systems, accounting/billing systems and network management systems to facilitate services such as measurement, accounting and billing. The IPFIX standard defines how IP flow information is to be formatted and transferred from an exporter to a collector.</Desc>
+      <CondSwitch>2055</CondSwitch>
+      <CondSwitch>4739</CondSwitch>
+      <CondSwitch>4740</CondSwitch>
+      <CondSwitch>5229</CondSwitch>
+      <CondSwitch>9995</CondSwitch>
+      <CondExp><![CDATA[ MLD16[0] == 10 ]]></CondExp>
+    </PSpec>
     <PSpec Name="AOL">
       <PSpecID>1460</PSpecID>
       <LName>America Online</LName>
       <Desc>AOL (America Online) provides Internet online services such as e-mail, software downloading, and chat rooms. AOL uses IP port 5190.</Desc>
       <Color>10</Color>
       <CondSwitch>5190</CondSwitch>
     </PSpec>
@@ -4596,14 +6299,15 @@
     </PSpec>
     <PSpec Name="GTP">
       <NotChild Name="GTP"/>
       <NotChild Name="WAN PPP"/>
       <NotChild Name="WAN Frame Relay"/>
       <NotChild Name="WAN X25"/>
       <NotChild Name="IPv6"/>
+      <NotChild Name="GENEVE"/>
       <PSpecID>2498</PSpecID>
       <LName>GPRS Tunneling Protocol</LName>
       <Desc>In General Packet Radio Service (GPRS) backbone network GPRS Tunneling Protocol (GTP) is a high level tunneling protocol used to carry signaling and data. GPRS backbone network contains several nodes of GPRS Support Node (GSN), which communicate with each other using IP. GSNs are used to communicate with Mobile Terminal equipment and relay data inside the backbone network to outside connections which in turn are controlled by Gateway GPRS Support Nodes. This relaying is implemented in the backbone network using GTP on top of UDP or TCP.</Desc>
       <Color>14</Color>
       <CondSwitch>3386</CondSwitch>
       <CondSwitch>2123</CondSwitch>
       <CondSwitch>2152</CondSwitch>
@@ -4677,20 +6381,25 @@
     </PSpec>
     <PSpec Name="Aruba ERM">
       <NotChild Name="Aruba ERM"/>
       <PSpecID>6727</PSpecID>
       <LName>Aruba ERM</LName>
       <SName>Aruba ERM</SName>
       <Desc>Aruba ERM Radio format for remote packet capture.</Desc>
-      <Color>14</Color>
+      <Color>15</Color>
       <CondSwitch>5555</CondSwitch>
       <NextLayer>
         <Exp><![CDATA[16]]></Exp>
       </NextLayer>
     </PSpec>
+    <PSpec Name="PEEK Remote">
+      <PSpecID>6728</PSpecID>
+      <Desc>Omnipeek/AiroPeek encapsulated IEEE 802.11 for remote packet capture.</Desc>
+      <Color>16</Color>
+    </PSpec>
     <PSpec Name="Diameter">
       <PSpecID>6726</PSpecID>
       <Desc>Diameter is an authentication, authorization and accounting protocol for computer networks, and a successor to RADIUS.</Desc>
       <Color>14</Color>
       <CondExp><![CDATA[(SrcPort == 3868) || (DestPort == 3868)]]></CondExp>
     </PSpec>
     <PSpec Name="UNIStim">
@@ -4795,24 +6504,119 @@
     <PSpec Name="ZEP">
       <PSpecID>7754</PSpecID>
       <SName>ZEP</SName>
       <LName>ZigBee Encapsulation Protocol</LName>
       <Desc>ZigBee Encapsulation Protocol for IoT Devices</Desc>
       <Color>7</Color>
       <CondSwitch>17754</CondSwitch>
-      <CondExp><![CDATA[(MLD16[0] == 0x4558)]]></CondExp>
+      <CondExp><![CDATA[MLD16[0] == 0x4558]]></CondExp>
+      <NextLayer>
+        <Exp><![CDATA[32]]></Exp>
+      </NextLayer>
+      <PSpec Name="802.15.4 Data">
+        <PSpecID>7756</PSpecID>
+        <LName>IEEE 802.15.4 Data Frame</LName>
+        <Color>9</Color>
+        <CondExp><![CDATA[(MLD8[0] & 0x03) == 0x01]]></CondExp>
+      </PSpec>
+      <PSpec Name="802.15.4 Cmd">
+        <PSpecID>7755</PSpecID>
+        <LName>IEEE 802.15.4 MAC Command Frame</LName>
+        <Color>8</Color>
+        <CondExp><![CDATA[(MLD8[0] & 0x03) == 0x03]]></CondExp>
+      </PSpec>
     </PSpec>
     <PSpec Name="MQTT">
       <PSpecID>1883</PSpecID>
       <SName>MQTT</SName>
       <LName>Message Queue Telemetry Transport</LName>
       <Desc>Message Queue Telemetry Transport is an ISO standard publish-subscribe-based &quot;lightweight&quot; messaging protocol for use on top of the TCP/IP protocol.</Desc>
       <Color>7</Color>
       <CondSwitch>1883</CondSwitch>
     </PSpec>
+    <PSpec Name="IEC 60870-5-104">
+      <PSpecID>2404</PSpecID>
+      <SName>IEC 60870-5-104</SName>
+      <Desc>IEC 60870 part 5 is one of the IEC 60870 set of standards which define systems used for telecontrol (supervisory control and data acquisition) in electrical engineering and power system automation applications. Part 5 provides a communication profile for sending basic telecontrol messages between two systems, which uses permanent directly connected data circuits between the systems.</Desc>
+      <Color>8</Color>
+      <CondSwitch>2404</CondSwitch>
+    </PSpec>
+    <PSpec Name="ANSI C12.22">
+      <PSpecID>1155</PSpecID>
+      <Desc>Protocol for transporting ANSI C12.19 table data over networks, for the purpose of interoperability among communications modules and meters.</Desc>
+      <Color>7</Color>
+      <CondSwitch>1153</CondSwitch>
+    </PSpec>
+    <PSpec Name="OpenVPN">
+      <PSpecID>1194</PSpecID>
+      <Desc>OpenVPN</Desc>
+      <Color>7</Color>
+      <CondSwitch>1194</CondSwitch>
+    </PSpec>
+    <PSpec Name="Bitcoin RPC">
+      <PSpecID>8332</PSpecID>
+      <LName>Bitcoin Remote Procedure Call Protocol</LName>
+      <Desc>Bitcoin Core provides a remote procedure call (RPC) interface for various administrative tasks, wallet operations, and queries about network and block chain data.</Desc>
+      <Color>12</Color>
+      <CondSwitch>8332</CondSwitch>
+    </PSpec>
+    <PSpec Name="Bitcoin">
+      <PSpecID>8333</PSpecID>
+      <LName>Bitcoin Protocol</LName>
+      <Desc>Bitcoin uses a simple broadcast network to propagate transactions and blocks. All communications are done over TCP. Bitcoin is fully able to use ports other than 8333 via the -port parameter. IPv6 is supported with Bitcoind/Bitcoin-Qt v0.7. Using bitcoin over tor is also supported.</Desc>
+      <Color>11</Color>
+      <CondSwitch>8333</CondSwitch>
+    </PSpec>
+    <PSpec Name="LISP">
+      <PSpecID>4340</PSpecID>
+      <LName>Locator/Identifier Separation Protocol</LName>
+      <Desc>The Locator/ID Separation Protocol (LISP) is a network-layer-based protocol which allows separating IP addresses into Endpoint Identifiers (EIDs) and Routing Locators (RLOCs). It is described in [RFC 6830](https://tools.ietf.org/html/rfc6830).</Desc>
+      <Color>5</Color>
+      <CondSwitch>4341</CondSwitch>
+      <CondSwitch>4342</CondSwitch>
+      <PSpec Name="LISP Data">
+        <PSpecID>4341</PSpecID>
+        <LName>Locator/Identifier Separation Protocol - Data</LName>
+        <CondExp><![CDATA[(SrcPort == 4341) || (DestPort == 4341)]]></CondExp>
+      </PSpec>
+      <PSpec Name="LISP Control">
+        <PSpecID>4342</PSpecID>
+        <LName>Locator/Identifier Separation Protocol - Control</LName>
+        <CondExp><![CDATA[(SrcPort == 4342) || (DestPort == 4342)]]></CondExp>
+      </PSpec>
+    </PSpec>
+    <PSpec Name="UMA">
+      <PSpecID>1797</PSpecID>
+      <LName>Unlicensed Mobile Access</LName>
+      <Color>2</Color>
+      <Desc>Unlicensed Mobile Access (UMA) (aka Generic Access Network) allows seamless transition between wireless wide-area networks (e.g. GSM, GPRS) and local area networks (e.g. Wi-Fi, Bluetooth).</Desc>
+      <CondSwitch>1797</CondSwitch>
+    </PSpec>
+    <PSpec Name="DNP3">
+      <PSpecID>1798</PSpecID>
+      <LName>Distributed Network Protocol v3</LName>
+      <Color>15</Color>
+      <Desc>Distributed Network Protocol 3 (DNP3) is a set of communications protocols used between components in process automation systems. Its main use is in utilities such as electric and water companies.</Desc>
+      <CondSwitch>20000</CondSwitch>
+      <CondExp><![CDATA[MLD16[0] == 0x0564]]></CondExp>
+    </PSpec>
+    <PSpec Name="CoAP">
+      <PSpecID>1800</PSpecID>
+      <LName>Constrained Application Protocol</LName>
+      <Color>15</Color>
+      <Desc>Constrained Application Protocol (CoAP) is a specialized Internet application protocol for constrained devices, as defined in [RFC 7252](https://tools.ietf.org/html/rfc7252). It enables those constrained devices called &quot;nodes&quot; to communicate with the wider Internet using similar protocols.</Desc>
+      <CondSwitch>5683</CondSwitch>
+    </PSpec>
+    <PSpec Name="DLEP">
+      <PSpecID>1801</PSpecID>
+      <LName>Dynamic Link Exchange Protocol</LName>
+      <Color>8</Color>
+      <Desc>The DLEP protocol deals with communication between a router and a local radio, attached over an IP network.</Desc>
+      <CondSwitch>854</CondSwitch>
+    </PSpec>
   </PSpec>
   <PSpec Name="IPX Children" Type="CommonTable">
     <PSpec Name="RIP">
       <PSpecID>3002</PSpecID>
       <LName>NetWare IPX Routing Information Protocol</LName>
       <SName>NW RIP</SName>
       <Desc>NetWare RIP is a distance-vector routing protocol. Distance-vector routing protocols typically exchange information about the network's topology through periodic broadcasts with their immediate router neighbors. RIP packets use the IPX protocol for transport and designate the value 0x0453 in the IPX socket field. RIP broadcasts are restricted to the local network only and allow routers to propagate the routing information onto other networks. Each router maintains a table of known routes and broadcasts this information on each locally attached segment. Other routers receive this information, update their routing tables, and send an up-to-date routing information packet. RIP packets are not allowed to cross routers.</Desc>
@@ -5669,14 +7473,20 @@
   </PSpec>
   <PSpec Name="Cisco FabricPath">
     <PSpecID>6668</PSpecID>
     <LName>Cisco FabricPath</LName>
     <Color>1</Color>
     <Desc>Cisco FabricPath is a proprietary implementation of TRILL (Transparent Interconnection of Lots of Links) that utilizes IS-IS for Layer 2 routing that is an alternative to Spanning Tree Protocol (STP).</Desc>
   </PSpec>
+  <PSpec Name="Cisco Meta Data">
+    <PSpecID>6669</PSpecID>
+    <LName>Cisco Meta Data</LName>
+    <Color>1</Color>
+    <Desc>Cisco Meta Data is a component of Cisco TrustSec security architecture.</Desc>
+  </PSpec>
   <PSpec Name="IEEE 802.3">
     <PSpecID>1</PSpecID>
     <LName>IEEE 802.3 CSMA/CD Ethernet</LName>
     <SName>802.3</SName>
     <Color>1</Color>
     <Desc>802.3 is a comprehensive standard for Local Area Networks employing the Carrier Sense Multiple Access with Collision Detection (CSMA/CD) access method. Under the International Standards Organization (ISO) the 10 megabits per second transmission speed is specified by ISO/DIS 8802/3. The definition of Ethernet under 802.3 supersedes the previous Ethernet standard known as Ethernet Type 2. In terms of data bytes in the protocol stack, 802.3 uses bytes 13 and 14 as a length field, whereas the earlier standard used these bytes as a protocol definition field.</Desc>
     <CondExp><![CDATA[MLD16[12] <= 1500]]></CondExp>
@@ -5690,30 +7500,30 @@
     <LName>IEEE 802.11 CSMA/CA WLAN</LName>
     <SName>802.11</SName>
     <Desc>802.11 is a comprehensive standard for Wireless Local Area Networks employing the Carrier Sense Multiple Access with Collision Avoidance (CSMA/CA) access method.</Desc>
     <Color>12</Color>
     <Definitions>
       <Define>
         <Name>PacketBits</Name>
-        <Value><![CDATA[(MLD8[0] & 0x0c)]]></Value>
+        <Value><![CDATA[MLD8[0] & 0x0c]]></Value>
       </Define>
       <Define>
         <Name>FragmentNumber</Name>
-        <Value><![CDATA[(PLD8[22] & 0x0f)]]></Value>
+        <Value><![CDATA[PLD8[22] & 0x0f]]></Value>
       </Define>
     </Definitions>
     <PSpec Name="802.11 Control">
       <PSpecID>200</PSpecID>
-      <Desc>There are six control frame subtypes in 802.11: request to send (RTS), clear to send (CTS), acknowledge (ACK), power save poll (PS-Poll), contention-free end (CF-End), and contention-free end plus ACK (CF-End+CF-Ack).</Desc>
+      <Desc>802.11 Control Frames assist with the delivery of Data &amp; Management frames.</Desc>
       <Color>14</Color>
       <CondExp><![CDATA[PacketBits == 0x04]]></CondExp>
       <Definitions>
         <Define>
           <Name>ControlBits</Name>
-          <Value><![CDATA[(MLD8[0] & 0xfc)]]></Value>
+          <Value><![CDATA[MLD8[0] & 0xfc]]></Value>
         </Define>
       </Definitions>
       <PSpec Name="Block Ack Request">
         <PSpecID>216</PSpecID>
         <SName>802.11 BAR</SName>
         <Desc>At the end of a burst the sender transmits a block-ACK Request frame, the receiver replies with a Block ACK frame containing the status of reception.</Desc>
         <Color>3</Color>
@@ -5758,27 +7568,157 @@
         <Desc>Acknowledges receipt of transmitted data.</Desc>
         <Color>17</Color>
         <CondExp><![CDATA[ControlBits == 0xd4]]></CondExp>
       </PSpec>
       <PSpec Name="Contention-Free End">
         <PSpecID>214</PSpecID>
         <LName>802.11 Control Contention-Free End</LName>
-        <SName>802.11 CFE</SName>
+        <SName>802.11 CF End</SName>
         <Desc>Signals the end of Contention Free period.</Desc>
         <Color>11</Color>
         <CondExp><![CDATA[ControlBits == 0xe4]]></CondExp>
       </PSpec>
       <PSpec Name="CF-End+CF-Ack">
         <PSpecID>215</PSpecID>
         <LName>802.11 Control CF-End+CF-Ack</LName>
         <SName>802.11 CFE+CFA</SName>
         <Desc>Signals the end of the Contention Free period and Acknowledges the receipt of transmitted data in a single message.</Desc>
         <Color>2</Color>
         <CondExp><![CDATA[ControlBits == 0xf4]]></CondExp>
       </PSpec>
+      <PSpec Name="Beamforming Report Poll">
+        <PSpecID>258</PSpecID>
+        <LName>802.11 Beamforming Report Poll</LName>
+        <SName>802.11 BRP</SName>
+        <Desc>To retrieve additional feedback from the second and subsequent beamformees, the beamformer must use a Beamforming Report Poll frame</Desc>
+        <Color>1</Color>
+        <CondExp><![CDATA[ControlBits == 0x44]]></CondExp>
+      </PSpec>
+      <PSpec Name="VHT/HE NDP Announcement">
+        <PSpecID>257</PSpecID>
+        <LName>802.11 VHT/HE NDP Announcement</LName>
+        <SName>802.11 VHT/HE NDP Ann</SName>
+        <Color>2</Color>
+        <CondExp><![CDATA[ControlBits == 0x54]]></CondExp>
+      </PSpec>
+      <PSpec Name="Control Frame Extension">
+        <PSpecID>256</PSpecID>
+        <LName>802.11 Control Frame Extension</LName>
+        <SName>802.11 CFE</SName>
+        <Color>3</Color>
+        <CondExp><![CDATA[ControlBits == 0x64]]></CondExp>
+        <Definitions>
+          <Define>
+            <Name>ControlExtBits</Name>
+            <Value><![CDATA[(MLD8[1] & 0x0f)]]></Value>
+          </Define>
+        </Definitions>
+        <PSpec Name="Reserved Control Frame Extension">
+          <PSpecID>261</PSpecID>
+          <LName>802.11 Control Frame Extension Reserved</LName>
+          <SName>802.11 CFE Res</SName>
+          <Desc>IEEE 802.11 reserved frame type.</Desc>
+          <Color>1</Color>
+          <CondExp><![CDATA[ControlExtBits == 0x00]]></CondExp>
+          <CondExp><![CDATA[ControlExtBits == 0x01]]></CondExp>
+          <CondExp><![CDATA[ControlExtBits == 0x0b]]></CondExp>
+          <CondExp><![CDATA[ControlExtBits == 0x0c]]></CondExp>
+          <CondExp><![CDATA[ControlExtBits == 0x0d]]></CondExp>
+          <CondExp><![CDATA[ControlExtBits == 0x0e]]></CondExp>
+          <CondExp><![CDATA[ControlExtBits == 0x0f]]></CondExp>
+        </PSpec>
+        <PSpec Name="Poll">
+          <PSpecID>262</PSpecID>
+          <LName>802.11 Control Frame Extension - Poll</LName>
+          <SName>802.11 CFE Poll</SName>
+          <Desc>IEEE 802.11 Control Extension Poll Frame.</Desc>
+          <Color>2</Color>
+          <CondExp><![CDATA[ControlExtBits == 0x02]]></CondExp>
+        </PSpec>
+        <PSpec Name="SPR">
+          <PSpecID>263</PSpecID>
+          <LName>802.11 Control Frame Extension - SPR</LName>
+          <SName>802.11 CFE SPR</SName>
+          <Desc>A IEEE 802.11 Control Extension SPR Frame.</Desc>
+          <Color>3</Color>
+          <CondExp><![CDATA[ControlExtBits == 0x03]]></CondExp>
+        </PSpec>
+        <PSpec Name="Grant">
+          <PSpecID>264</PSpecID>
+          <LName>802.11 Control Frame Extension - Grant</LName>
+          <SName>802.11 CFE Grant</SName>
+          <Desc>IEEE 802.11 Control Extension Grant Frame.</Desc>
+          <Color>4</Color>
+          <CondExp><![CDATA[ControlExtBits == 0x04]]></CondExp>
+        </PSpec>
+        <PSpec Name="DMG CTS">
+          <PSpecID>265</PSpecID>
+          <LName>802.11 Control Frame Extension - DMG Clear To Send</LName>
+          <SName>802.11 DMG CTS</SName>
+          <Desc>IEEE 802.11 Control Extension DMG Clear To Send Frame.</Desc>
+          <Color>5</Color>
+          <CondExp><![CDATA[ControlExtBits == 0x05]]></CondExp>
+        </PSpec>
+        <PSpec Name="DMG DTS">
+          <PSpecID>266</PSpecID>
+          <LName>802.11 Control Frame Extension - DMG DTS</LName>
+          <SName>802.11 DMG DTS</SName>
+          <Desc>IEEE 802.11 Control Extension DMG DTS Frame.</Desc>
+          <Color>6</Color>
+          <CondExp><![CDATA[ControlExtBits == 0x06]]></CondExp>
+        </PSpec>
+        <PSpec Name="Grant Ack">
+          <PSpecID>267</PSpecID>
+          <LName>802.11 Control Frame Extension - Grant Acknowledge</LName>
+          <SName>802.11 Grant Ack</SName>
+          <Desc>IEEE 802.11 Control Extension Grant Ack Frame.</Desc>
+          <Color>7</Color>
+          <CondExp><![CDATA[ControlExtBits == 0x07]]></CondExp>
+        </PSpec>
+        <PSpec Name="SSW">
+          <PSpecID>268</PSpecID>
+          <LName>802.11 Control Frame Extension - Sector Sweep</LName>
+          <SName>802.11 SSW</SName>
+          <Desc>IEEE 802.11 Control Extension Sector Sweep Frame.</Desc>
+          <Color>8</Color>
+          <CondExp><![CDATA[ControlExtBits == 0x08]]></CondExp>
+        </PSpec>
+        <PSpec Name="SSW-Feedback">
+          <PSpecID>269</PSpecID>
+          <LName>802.11 Control Frame Extension - Sector Sweep-Feedback</LName>
+          <SName>802.11 SSW-Feedback</SName>
+          <Desc>IEEE 802.11 Control Extension Sector Sweep-Feedback Frame.</Desc>
+          <Color>9</Color>
+          <CondExp><![CDATA[ControlExtBits == 0x09]]></CondExp>
+        </PSpec>
+        <PSpec Name="SSW-Ack">
+          <PSpecID>270</PSpecID>
+          <LName>802.11 Control Frame Extension - Sector Sweep-Ack</LName>
+          <SName>802.11 SSW-Ack</SName>
+          <Desc>IEEE 802.11 Control Extension Sector Sweep-Ack Frame.</Desc>
+          <Color>10</Color>
+          <CondExp><![CDATA[ControlExtBits == 0x0a]]></CondExp>
+        </PSpec>
+      </PSpec>
+      <PSpec Name="Control Wrapper">
+        <PSpecID>255</PSpecID>
+        <LName>802.11 Control Wrapper</LName>
+        <SName>802.11 CW</SName>
+        <Desc>The Control Wrapper frame is used to carry any other control frame, other than another Control Wrapper frame together with a HT Control field.</Desc>
+        <Color>4</Color>
+        <CondExp><![CDATA[ControlBits == 0x74]]></CondExp>
+      </PSpec>
+      <PSpec Name="Trigger">
+        <PSpecID>300</PSpecID>
+        <LName>802.11 Trigger</LName>
+        <SName>802.11 Trigger</SName>
+        <Desc>A Trigger frame allocates resources for and solicits one or more HE TB PPDU transmissions. The Trigger frame also carries other information required by the responding STA to send an HE TB PPDU.</Desc>
+        <Color>6</Color>
+        <CondExp><![CDATA[ControlBits == 0x24]]></CondExp>
+      </PSpec>
     </PSpec>
     <PSpec Name="802.11 Management">
       <PSpecID>201</PSpecID>
       <Desc>There are 11 distinct management frame types. All management frames include fields: frame control duration address 1, 2, and 3, sequence control, frame body and frame check sequence. The frame body carries information in both fixed fields and in variable length information elements. Management frames in 802.11: beacon, probe request and response, authentication, deauthentication, association request and response, reassociation request and response, disassociation, and announcement traffic indication message.</Desc>
       <Color>1</Color>
       <CondExp><![CDATA[PacketBits == 0x00]]></CondExp>
       <Definitions>
@@ -5831,14 +7771,22 @@
         <PSpecID>225</PSpecID>
         <LName>802.11 Management Probe Response</LName>
         <SName>802.11 Probe Rsp</SName>
         <Desc>A Probe Response is a reply to a Probe Request with station parameters and supported data rates.</Desc>
         <Color>12</Color>
         <CondExp><![CDATA[ManagementBits == 0x50]]></CondExp>
       </PSpec>
+      <PSpec Name="Timing Adv">
+        <PSpecID>253</PSpecID>
+        <LName>802.11 Management Timing Advertisement</LName>
+        <SName>802.11 Timing Advertisement</SName>
+        <Desc>A Timing Advertisement.</Desc>
+        <Color>10</Color>
+        <CondExp><![CDATA[ManagementBits == 0x60]]></CondExp>
+      </PSpec>
       <PSpec Name="Beacon">
         <PSpecID>226</PSpecID>
         <LName>802.11 Management Beacon</LName>
         <SName>802.11 Beacon</SName>
         <Desc>Beacon packets are sent by the access point in a BSS (or its equivalent in an IBSS) to announce the beginning of a Contention Free period (CF), during which the right to transmit is conferred by the access point by polling. Beacon management packets carry BSS timestamps to help synchronize member stations with the BSS, and other information to help them locate and choose the BSS with the best signal and availability.</Desc>
         <Color>14</Color>
         <CondExp><![CDATA[ManagementBits == 0x80]]></CondExp>
@@ -5887,14 +7835,22 @@
         <PSpecID>231</PSpecID>
         <LName>802.11 Management Action</LName>
         <SName>802.11 Action</SName>
         <Desc>The Action field provides a mechanism for specifying extended management actions.</Desc>
         <Color>13</Color>
         <CondExp><![CDATA[ManagementBits == 0xd0]]></CondExp>
       </PSpec>
+      <PSpec Name="Action No Ack">
+        <PSpecID>254</PSpecID>
+        <LName>802.11 Management Action No Ack</LName>
+        <SName>802.11 Action No Ack</SName>
+        <Desc>The Action field provides a mechanism for specifying extended management actions.</Desc>
+        <Color>16</Color>
+        <CondExp><![CDATA[ManagementBits == 0xe0]]></CondExp>
+      </PSpec>
     </PSpec>
     <PSpec Name="802.11 Data">
       <PSpecID>202</PSpecID>
       <Desc>The simple data frame encapsulates the upper layer protocol packets delivering them from one IEEE 802.11 station to another. It may appear in both the contention period and the contention-free period.</Desc>
       <Color>4</Color>
       <CondExp><![CDATA[PacketBits == 0x08]]></CondExp>
       <NextLayer>
@@ -5988,14 +7944,41 @@
       <PSpec Name="802.11 QoS CF-Ack + CF-Poll">
         <PSpecID>247</PSpecID>
         <Desc>802.11 CF-Ack + CF-Poll.</Desc>
         <Color>15</Color>
         <CondExp><![CDATA[(PLD8[0] & 0xfc) == 0xf8]]></CondExp>
       </PSpec>
     </PSpec>
+    <PSpec Name="802.11 Extension">
+      <PSpecID>259</PSpecID>
+      <Color>4</Color>
+      <CondExp><![CDATA[PacketBits == 0x0c]]></CondExp>
+      <Definitions>
+        <Define>
+          <Name>ExtensionBits</Name>
+          <Value><![CDATA[MLD8[0] & 0xfc]]></Value>
+        </Define>
+      </Definitions>
+      <PSpec Name="DMG Beacon">
+        <PSpecID>260</PSpecID>
+        <LName>802.11 DMG Beacon</LName>
+        <SName>802.11 DMG Beacon</SName>
+        <Desc>DMG Beacon.</Desc>
+        <Color>8</Color>
+        <CondExp><![CDATA[ExtensionBits == 0x0c]]></CondExp>
+      </PSpec>
+      <PSpec Name="S1G Beacon">
+        <PSpecID>273</PSpecID>
+        <LName>802.11 S1G Beacon</LName>
+        <SName>802.11 S1G Beacon</SName>
+        <Desc>S1G Beacon.</Desc>
+        <Color>8</Color>
+        <CondExp><![CDATA[ExtensionBits == 0x0d]]></CondExp>
+      </PSpec>
+    </PSpec>
   </PSpec>
   <PSpec Name="Ethernet Type 2">
     <PSpecID>2</PSpecID>
     <SName>EType2</SName>
     <Desc>Ethernet Type 2 is the second version of Ethernet that was defined by Xerox Parc, Digital Equipment Corporation and other industry leaders around 1980 and was subsequently superseded by the international standard 802.3. Some protocols, such as IP and DECnet were originally defined under Ethernet Type 2, and have never successfully (in terms of widespread usage) migrated to the newer standard on Ethernet. In terms of data bytes on the wire, Ethernet Type 2 uses bytes 13 and 14 as a protocol definition field, whereas the later standard used these bytes as a length field.</Desc>
     <Color>6</Color>
     <CondExp><![CDATA[MLD16[12] > 1500]]></CondExp>
@@ -6250,8 +8233,14 @@
     <PSpec Name="Q931">
       <PSpecID>31</PSpecID>
       <LName>WAN Q.931</LName>
       <SName>WAN Q.931</SName>
       <CondExp><![CDATA[(MLD8[0] == 0x08) && ((MLD8[1] & 0xf0) == 0) && (PLD8[0] != 0xff)]]></CondExp>
     </PSpec>
   </PSpec>
+  <PSpec Name="NSH">
+    <PSpecID>9000</PSpecID>
+    <LName>Network Service Header (NSH)</LName>
+    <Color>5</Color>
+    <Desc>Imposed on packets or frames to realize Service Function Paths (SFPs). The NSH also provides a mechanism for metadata exchange along the instantiated service paths.</Desc>
+  </PSpec>
 </ProtoSpecTable>
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/enginestatus.py` & `omniscript-liveaction-3.0.49/src/omniscript/enginestatus.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,76 @@
 ﻿"""EngineStatus class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 import six
 
-from .capture import Capture
 from .omniid import OmniId
-
-from .invariant import BYTES_PER_KILOBYTE, KILOBYTES_PER_MEGABYTE, \
-    KILOBYTES_PER_GIGABYTE, KILOBYTES_PER_TERABYTE
-
 from .peektime import PeekTime
 
 
 _engine_prop_dict = {
-    'adapterCount' : 'adapter_count',
-    'address' : 'address',
-    'alarmCount' : 'alarm_count',
-    'alarmsModificationTime' : 'alarm_modification_time',
-    'captureInfo' : 'capture_info_list',
-    'captures' : 'capture_count',
-    'captureSessionCount' : 'capture_session_count',
-    'cpuCount' : 'cpu_count',
-    'cpuType' : 'cpu_type',
-    'customSettings' : 'custom_settings',
-    'dataDriveFormat' : 'data_drive_format',
-    'dataFolder' : 'data_directory',
+    'adapterCount': 'adapter_count',
+    'address': 'address',
+    'alarmCount': 'alarm_count',
+    'alarmsModificationTime': 'alarm_modification_time',
+    'captureInfo': 'capture_info_list',
+    'captures': 'capture_count',
+    'captureSessionCount': 'capture_session_count',
+    'cpuCount': 'cpu_count',
+    'cpuType': 'cpu_type',
+    'customSettings': 'custom_settings',
+    'dataDriveFormat': 'data_drive_format',
+    'dataFolder': 'data_directory',
     'decryptionKeyCount': 'decryption_key_count',
-    'diskReservedSpace' : 'disk_reserved_space',
-    'enginesModificationTime' : 'modification_time',
-    'engineType' : 'engine_type',
-    'fileCount' : 'file_count',
-    'fileVersion' : 'file_version',
-    'filterCount' : 'filter_count',
-    'filtersModificationTime' : 'filters_modification_time',
-    'forensicSearches' : 'forensic_search_count',
-    'forensicSearchReservedSpace' : 'forensic_search_reserved_space',
-    'graphCount' : 'graph_count',
-    'hardwareProfileCount' : 'hardware_profile_count',
-    'hardwareType' : 'hardware_type',
-    'hostName' : 'host',
-    'ipmiAddr' : 'ipmi_address',
-    'licensed' : 'is_licensed',
-    'licenseExpirationDate' : 'license_expiration_date',
-    'licenseExpired' : 'is_license_expired',
-    'licenseType' : 'license_type',
-    'logTotalCount' : 'log_total_count',
-    'memoryAvailablePhysical' : 'memory_available_physical',
-    'memoryTotalPhysical' : 'memory_total_physical',
-    'name' : 'name',
-    'nameCount' : 'name_table_count',
-    'namesModificationTime' : 'names_modification_time',
-    'nativeProtospecsEnabled' : 'is_native_protospecs_enabled',
-    'notificationCount' : 'notification_count',
-    'notificationsModificationTime' : 'notifications_modification_time',
-    'operatingSystem' : 'operating_system',
-    'os' : 'os',
-    'platform' : 'platform',
-    'productVersion' : 'product_version',
-    'protocolTranslationCount' : 'protocol_translation_count',
-    'protospecsVersion' : 'protospecs_version',
-    'securityEventsTotalCount' : 'security_events_total_count',
-    'serialNumber' : 'serial_number',
-    'storageTotal' : 'storage_total',
-    'storageUsed' : 'storage_used',
-    'time' : 'time',
-    'timeZoneBias' : 'time_zone_bias',
-    'uptime' : 'uptime',
-    'userDomain' : 'user_domain',
-    'userId' : 'user_id',
-    'userName' : 'user_name'
+    'diskReservedSpace': 'disk_reserved_space',
+    'enginesModificationTime': 'modification_time',
+    'engineType': 'engine_type',
+    'fileCount': 'file_count',
+    'fileVersion': 'file_version',
+    'filterCount': 'filter_count',
+    'filtersModificationTime': 'filters_modification_time',
+    'forensicSearches': 'forensic_search_count',
+    'forensicSearchReservedSpace': 'forensic_search_reserved_space',
+    'graphCount': 'graph_count',
+    'hardwareProfileCount': 'hardware_profile_count',
+    'hardwareType': 'hardware_type',
+    'hostName': 'host',
+    'ipmiAddr': 'ipmi_address',
+    'licensed': 'is_licensed',
+    'licenseExpirationDate': 'license_expiration_date',
+    'licenseExpired': 'is_license_expired',
+    'licenseType': 'license_type',
+    'logTotalCount': 'log_total_count',
+    'memoryAvailablePhysical': 'memory_available_physical',
+    'memoryTotalPhysical': 'memory_total_physical',
+    'name': 'name',
+    'nameCount': 'name_table_count',
+    'namesModificationTime': 'names_modification_time',
+    'nativeProtospecsEnabled': 'is_native_protospecs_enabled',
+    'notificationCount': 'notification_count',
+    'notificationsModificationTime': 'notifications_modification_time',
+    'operatingSystem': 'operating_system',
+    'os': 'os',
+    'platform': 'platform',
+    'productVersion': 'product_version',
+    'protocolTranslationCount': 'protocol_translation_count',
+    'protospecsVersion': 'protospecs_version',
+    'securityEventsTotalCount': 'security_events_total_count',
+    'serialNumber': 'serial_number',
+    'storageTotal': 'storage_total',
+    'storageUsed': 'storage_used',
+    'time': 'time',
+    'timeZoneBias': 'time_zone_bias',
+    'uptime': 'uptime',
+    'userDomain': 'user_domain',
+    'userId': 'user_id',
+    'userName': 'user_name'
 }
 
 
 # def _ parse _ prop (a, v):
 #     result = None
 #     if a == 'storage_free_space':
 #         result = []
@@ -113,15 +108,15 @@
         self._load(props)
 
     def _load(self, props):
         """Set attributes from a dictionary."""
         if isinstance(props, dict):
             value = props.get('value')
             if isinstance(value, dict):
-                for k,v in value.items():
+                for k, v in value.items():
                     if k == 'id':
                         setattr(self, k, OmniId(v))
                     elif k == 'allocated':
                         setattr(self, k, v)
                     elif k == 'used':
                         setattr(self, k, v)
 
@@ -138,16 +133,16 @@
     address = None
     """The OmniEngine's IP Address or host name."""
 
     alarm_count = 0
     """The number of alarms configured on the OmniEngine."""
 
     alarm_modification_time = None
-    """The time, as 
-    :class:`PeekTime <omniscript.peektime.PeekTime>`, 
+    """The time, as
+    :class:`PeekTime <omniscript.peektime.PeekTime>`,
     of the last modification to the alarms."""
 
     capture_info_list = []
     """Information about the captures on the Engine."""
 
     capture_count = 0
     """The number of Captures created on the OmniEngine."""
@@ -187,16 +182,16 @@
     file_version = ''
     """The File Version property of the OmniEngine."""
 
     filter_count = 0
     """The number of Filters on the OmniEngine."""
 
     filters_modification_time = None
-    """The last time, as a 
-    :class:`PeekTime <omniscript.peektime.PeekTime>`, 
+    """The last time, as a
+    :class:`PeekTime <omniscript.peektime.PeekTime>`,
     the Filters where modified."""
 
     forensic_search_count = 0
     """The number of Forensic Searches on the OmniEngine."""
 
     forensic_search_reserved_space = 0
     """The amount of disk space, in bytes, reserved for
@@ -224,16 +219,16 @@
     is_licensed = False
     """Is the engine licensed?"""
 
     is_native_protospecs_enabled = False
     """Are the Native Protospecs Enabled?"""
 
     license_expiration_date = None
-    """The date, as 
-    :class:`PeekTime <omniscript.peektime.PeekTime>`, 
+    """The date, as
+    :class:`PeekTime <omniscript.peektime.PeekTime>`,
     the OmniEngine's license expires."""
 
     license_type = 0
     """The index of the OmniEngines license type."""
 
     log_total_count = 0
     """The total number of Log entires in the OmniEngine Event Log."""
@@ -253,24 +248,24 @@
     """The name of the OmniEngine."""
 
     name_table_count = 0
     """The number of Name Table entires (need to confirm) on the
     OmniEngine."""
 
     name_table_modification_time = None
-    """The time, as 
-    :class:`PeekTime <omniscript.peektime.PeekTime>`, 
+    """The time, as
+    :class:`PeekTime <omniscript.peektime.PeekTime>`,
     the Names Table was modified."""
 
     notification_count = 0
     """The number of Notifications on the OmniEngine."""
 
     notifications_modification_time = None
-    """The last time, as 
-    :class:`PeekTime <omniscript.peektime.PeekTime>`, 
+    """The last time, as
+    :class:`PeekTime <omniscript.peektime.PeekTime>`,
     the Notifications were modified."""
 
     operating_system = ''
     """The full name of the Operating System that the OmniEngine is
     running on.
     """
 
@@ -386,21 +381,21 @@
         self.time = EngineStatus.time
         self.time_zone_bias = EngineStatus.time_zone_bias
         self.uptime = EngineStatus.uptime
         self.user_domain = EngineStatus.user_domain
         self.user_id = EngineStatus.user_id
         self.user_name = EngineStatus.user_name
 
-        #Initialize calculated values
+        # Initialize calculated values
         self.storage_available = EngineStatus.storage_available
 
-        #Set provided values
+        # Set provided values
         self.host = engine.host
         self.port = engine.port
-        #Parse the dictionary.
+        # Parse the dictionary.
         self._load(props)
 
     def __str__(self):
         return f'EngineStatus: {self.name}'
 
     def _create_capture_info_list(self, props):
         """Return a list of CaptureInfo objects."""
@@ -411,15 +406,15 @@
                 for ci in capture_list:
                     lst.append(CaptureInfo(ci))
         return lst
 
     def _load(self, props):
         """Set attributes from a dictionary."""
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 a = _engine_prop_dict.get(k)
                 if a is not None and hasattr(self, a):
                     if isinstance(getattr(self, a), six.string_types):
                         setattr(self, a, v if v else '')
                     elif isinstance(getattr(self, a), int):
                         setattr(self, a, int(v) if v else 0)
                     elif isinstance(getattr(self, a), list):
@@ -427,24 +422,24 @@
                             setattr(self, a, self._create_capture_info_list(v))
                     elif isinstance(getattr(self, a), dict):
                         setattr(self, a, v)
                     elif getattr(self, a) is None:
                         if a in ('address'):
                             setattr(self, a, v)
                         elif a in ('alarm_modification_time', 'filters_modification_time',
-                                'modification_time', 'license_expiration_date',
-                                'notifications_modification_time', 'time'):
+                                   'modification_time', 'license_expiration_date',
+                                   'notifications_modification_time', 'time'):
                             setattr(self, a, PeekTime(v))
                         else:
                             setattr(self, a, v)
                     else:
                         setattr(self, a, v)
             self.cpu_type = ' '.join(self.cpu_type.split())
             self.storage_available = (self.storage_total - self.storage_used
-                if self.storage_total > self.storage_used else 0)
+                                      if self.storage_total > self.storage_used else 0)
 
     def refresh(self):
         """Refresh the attributes of this object."""
         props = self._engine._issue_command("status/")
         if props:
             self.__init__(self._engine, props)
             return True
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/eventlog.py` & `omniscript-liveaction-3.0.49/src/omniscript/eventlog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """EventLog class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 import six
 
 from .omniid import OmniId
 from .omnierror import OmniError
 from .peektime import PeekTime
 
@@ -34,15 +34,15 @@
 
     source_key = 0
     """The GUID of the source of the log entry."""
 
     timestamp = None
     """The date and time when the log entry was generated."""
 
-    #XML Tags
+    # XML Tags
     _json_capture_id = "contextId"
     _json_index = "messageId"
     _json_message = "shortMessage"
     _json_severity = "severity"
     _json_source_id = "sourceId"
     _json_source_key = "sourceKey"
     _json_timestamp = "timestamp"
@@ -78,52 +78,52 @@
         self.severity = EventLogEntry.severity
         self.source_id = EventLogEntry.source_id
         self.source_key = EventLogEntry.source_key
         self.timestamp = EventLogEntry.timestamp
         self._load(props)
 
     def __str__(self):
-        return f'AuditLogEntry: {self.message}'
+        return f'EventLogEntry: {self.message}'
 
     def _load(self, props):
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 a = EventLogEntry._event_log_entry_prop_dict.get(k)
                 if hasattr(self, a):
                     if isinstance(getattr(self, a), six.string_types):
                         setattr(self, a, v if v else '')
                     elif isinstance(getattr(self, a), int):
                         setattr(self, a, int(v) if v else 0)
                     elif getattr(self, a) is None:
-                        if (a == EventLogEntry._tag_capture_id) \
-                            or (a == EventLogEntry._tag_source_id):
+                        if (a == EventLogEntry._tag_capture_id
+                                or a == EventLogEntry._tag_source_id):
                             setattr(self, a, OmniId(v))
                         elif a == EventLogEntry._tag_timestamp:
                             setattr(self, a, PeekTime(v))
 
     def _key(self):
         return self.index
 
 
 class EventLog(object):
     """The EventLog class.
     """
-    
+
     context_id = None
     """The id of the context (Capture)."""
 
     count = 0
     """The total number of entries in the log."""
 
     engine = None
     """The OmniEngine object the Audit Log is from."""
 
     first = None
     """The timestamp of the first log entry."""
-    
+
     informational = 0
     """The number of informational (0) events."""
 
     last = None
     """The timestamp of the last log entry."""
 
     major = 0
@@ -135,15 +135,15 @@
     query = None
     """The query string for this EventLog."""
 
     severe = 0
     """The number of severe (3) events."""
 
     entries = None
-    """The list of 
+    """The list of
     :class:`EventLogEntry <omniscript.eventlog.EventLogEntry>`
     Entries.
     """
 
     # Tags
     _json_count = 'total'
     _json_first = 'firstTimestamp'
@@ -197,15 +197,15 @@
         else:
             return 'EventLog'
 
     def _load_counts(self, props):
         if isinstance(props, dict):
             counts = props.get('counts')
             if isinstance(counts, dict):
-                for k,v in counts.items():
+                for k, v in counts.items():
                     a = EventLog._event_log_prop_dict[k]
                     if a == EventLog._tag_count:
                         self.count = max(self.count, int(v))
                     elif a == EventLog._tag_informational:
                         self.informational = max(self.informational, int(v))
                     elif a == EventLog._tag_major:
                         self.major = max(self.major, int(v))
@@ -248,15 +248,15 @@
             _first = (self.count - first) if (first < self.count) else 0
         _el = self.engine.get_event_log(
             _first, _count, self.context_id, self.query)
         self.update(_el)
 
     def get_next(self, count=None):
         """Retrieve the next count entries of the EventLog or the last
-        count entries if count is negative. If count is not specified, 
+        count entries if count is negative. If count is not specified,
         then the remaining entries are retrieved.
         """
         if not self.engine:
             raise OmniError('EventLog does not have an OmniEngine.')
         if isinstance(count, int) and count == 0:
             return
         if count > 0:
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/fileinformation.py` & `omniscript-liveaction-3.0.49/src/omniscript/fileinformation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 ﻿"""FileInformation class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
-
-import xml.etree.ElementTree as ET
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 from .invariant import FILE_FLAGS_DIRECTORY
-from .peektime import PeekTime
 
 
 class FileInformation(object):
     """Information about a file.
     """
 
     flags = 0
@@ -26,15 +23,15 @@
 
     name = ''
     """The fully qualified name of the file."""
 
     size = 0
     """The size of the file in bytes."""
 
-    #XML Tags
+    # XML Tags
     _json_path = 'dir'
     _json_file_name = 'files'
 
     _tag_root_name = "file"
     _tag_name = "name"
 
     def __init__(self, name='', flags=0, props=None):
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/filter.py` & `omniscript-liveaction-3.0.49/src/omniscript/filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 ﻿"""Filter class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 import json
 import xml.etree.ElementTree as ET
 
 import omniscript
 
 from .omniid import OmniId
 from .peektime import PeekTime
 
 from .invariant import TIME_FLAGS_NANOSECONDS
 
 from .filternode import parse_console_filter, parse_omni_filter, store_omni_filter
 
 
-find_attribs = ['name', 'id']
 _attrib_props = ['Name', 'ID']
 
 
 class Filter(object):
     """The Filter class.
     """
-    
+
     _class_id = None
     """The Class Identifier of the object."""
 
     _engine = False
     """Is this an Engine Filter. Or a OmniPeek Console Filter."""
-    
+
     color = None
     """The color of the filter."""
 
     comment = None
     """The filter's comment."""
 
     created = None
@@ -58,15 +57,17 @@
 
     criteria = None
     """The criteria of the the filter. A hierarchy of
     objectes that are sub-classed from
     :class:`FilterNode <omniscript.filternode.FilterNode>`.
     """
 
-    #Tags
+    find_attributes = ('name', 'id', 'code')
+
+    # Tags
     _json_classid = 'clsid'
     _json_filters = 'filters'
     _json_classid_name = 'Filter'
     _json_id = 'id'
     _json_name = 'name'
     _json_comment = 'comment'
     _json_color = 'color'
@@ -93,45 +94,53 @@
         _json_group: _tag_group,
         _json_id: _tag_id,
         _json_modified: _tag_modified,
         _json_name:  _tag_name,
         _json_criteria: _tag_criteria
     }
 
+    endpoint = 'filters/'
+
     def __init__(self, name=None, criteria=None):
         class_name_ids = omniscript.get_class_name_ids()
         self._class_id = class_name_ids[Filter._json_classid_name]
         self.id = OmniId(True) if criteria is None else Filter.id
         self.name = name
         self.color = Filter.color
         self.comment = Filter.comment
         self.group = Filter.group
         self.created = Filter.created
         self.modified = Filter.modified
         self.criteria = Filter.criteria
+        self.props = criteria if isinstance(criteria, dict) else {}
         self._load(criteria)
 
     def __repr__(self) -> str:
         return f'Filter: {self.name}'
 
     def __str__(self) -> str:
         return f'Filter: {self.name}'
 
+    def __eq__(self, other) -> bool:
+        return (self._class_id, self.id, self.name, self.color, self.comment, self.group,
+                self.created) == (other._class_id, other.id, other.name, other.color,
+                                  other.comment, other.group, other.created)
+
     def _load(self, criteria):
         """Load the Filter from a Dictionairy."""
         if isinstance(criteria, dict):
             self._load_dict(criteria)
         elif isinstance(criteria, ET.Element):
             self._load_xml(criteria)
- 
+
     def _load_dict(self, props):
         """Load the Filter from a Dictionairy."""
         if isinstance(props, dict):
-            self._engine = True # Do the props contain an Engine Filter?
-            for k,v in props.items():
+            self._engine = True  # Do the props contain an Engine Filter?
+            for k, v in props.items():
                 a = Filter._filter_prop_dict.get(k)
                 if a is not None and hasattr(self, a):
                     if a == Filter._tag_classid:
                         self._class_id = OmniId(v)
                     elif a == Filter._tag_color:
                         self.color = int(v.strip('#'), 16)
                     elif a == Filter._tag_comment:
@@ -147,18 +156,18 @@
                     elif a == Filter._tag_name:
                         self.name = v
                     elif a == Filter._tag_criteria:
                         self.criteria = parse_omni_filter(v)
 
     def _load_xml(self, element):
         """Load the Filter from XML."""
-        engine = True # Does element contain an Engine Filter?
+        engine = True  # Does element contain an Engine Filter?
         filter_obj = element.find('filter')
         if filter_obj is None:
-            filter_obj = element.find('filterobj') #from Filter List.
+            filter_obj = element.find('filterobj')  # from Filter List.
         if filter_obj is not None:
             for attrib in filter_obj.items():
                 if attrib[0] == 'id':
                     engine = OmniId.is_id(attrib[1])
                     self.id = OmniId(attrib[1]) if engine else OmniId(True)
                 elif attrib[0] == 'color':
                     self.color = int(attrib[1])
@@ -173,42 +182,49 @@
                 elif attrib[0] == 'name':
                     self.name = attrib[1]
             if self.id is None:
                 self.id = OmniId(None)
             root_node = filter_obj.find('rootnode')
             if root_node is not None:
                 self.criteria = (parse_omni_filter(root_node)
-                    if engine else parse_console_filter(root_node))
+                                 if engine else parse_console_filter(root_node))
 
     def _store(self):
         """Returns the Filter as a Dictionairy."""
         props = {}
         props[Filter._json_id] = self.id.format()
         props[Filter._json_name] = self.name
         if self.comment:
             props[Filter._json_comment] = self.comment
         props[Filter._json_color] = f'#{self.color:6X}' if self.color else '#000000'
         if self.created:
-            props[Filter._json_created] = self.created.iso_time(TIME_FLAGS_NANOSECONDS)
+            props[Filter._json_created] = self.created.iso_time(
+                TIME_FLAGS_NANOSECONDS)
         if self.modified:
-            props[Filter._json_modified] = self.modified.iso_time(TIME_FLAGS_NANOSECONDS)
+            props[Filter._json_modified] = self.modified.iso_time(
+                TIME_FLAGS_NANOSECONDS)
         if self.group:
             props[Filter._json_group] = self.group
         if self.criteria:
             store_omni_filter(props, Filter._json_criteria, self.criteria)
         props[Filter._json_classid] = self._class_id.format()
         return json.dumps(props)
 
     def to_string(self, pad):
         text = str(self) + '\n'
         if self.criteria:
             operation = 'or: ' if self.criteria.or_node is not None else ''
             text += self.criteria.to_string((pad+1), operation)
         return text
 
+    @property
+    def UUID(self) -> str:
+        """ Return the UUID in string format """
+        return str(self.id.get_id()).upper() if self.id is not None else ''
+
     # def to_xml(self, pretty=False):
     #     """Return the Filter encoded in XML as a string."""
     #     class_name_ids = omniscript.get_class_name_ids()
     #     filter_obj = ET.Element('filterobj',
     #                             {'clsid':str(class_name_ids['Filter'])})
     #     self._store(filter_obj)
     #     return ET.tostring(filter_obj).replace('\n', '')
@@ -219,17 +235,26 @@
     if isinstance(resp, dict) and Filter._json_filters in resp:
         for props in resp[Filter._json_filters]:
             lst.append(Filter(criteria=props))
     lst.sort(key=lambda x: x.name)
     return lst
 
 
-def find_filter(filters, value, attrib=find_attribs[0]):
+def find_all_filters(filters, value, attrib=Filter.find_attributes[0]):
+    """Finds all filters that match the value in the filters list"""
+    if (not filters) or (attrib not in Filter.find_attributes):
+        return None
+
+    if isinstance(filters, list):
+        return [i for i in filters if isinstance(i, Filter) and getattr(i, attrib) == value]
+
+
+def find_filter(filters, value, attrib=Filter.find_attributes[0]):
     """Finds a filter in the list"""
-    if (not filters) or (attrib not in find_attribs):
+    if (not filters) or (attrib not in Filter.find_attributes):
         return None
 
     if isinstance(filters[0], Filter):
         return next((i for i in filters if getattr(i, attrib) == value), None)
 
 
 def read_filter_file(filename):
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/filternode.py` & `omniscript-liveaction-3.0.49/src/omniscript/filternode.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 ﻿"""FilterNode class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 import six
 import xml.etree.ElementTree as ET
 
 import omniscript
 
 from .analysismodule import AnalysisModule
-from .omniaddress import OmniAddress
+from .omniaddress import OmniAddress, BaseAddress
 from .omniport import OmniPort
 from .omniid import OmniId
 from .peektime import PeekTime
 
-from .invariant import (PATTERN_TYPE_ASCII, VALUE_FLAG_NETWORK_BYTE_ORDER, VALUE_OPERATOR_EQUAL,
-    WIRELESS_BAND_ALL, WAN_DIRECTION_UNDEFINED)
-
+from .invariant import (
+    PATTERN_TYPE_ASCII, VALUE_FLAG_NETWORK_BYTE_ORDER, VALUE_OPERATOR_EQUAL, WIRELESS_BAND_ALL,
+    WAN_DIRECTION_UNDEFINED)
 
 _json_classid = 'clsid'
 _json_andnode = 'andNode'
 _json_ornode = 'orNode'
 _json_accept_1_to_2 = 'accept1To2'
 _json_accept_2_to_1 = 'accept2To1'
 _json_data = 'data'
@@ -36,15 +36,15 @@
 def _build_class_id():
     global _filter_id_to_class
     class_name_ids = omniscript.get_class_name_ids()
     _filter_id_to_class = (dict((class_name_ids[name_], class_)
                            for (name_, class_) in _filter_name_class))
     # Add the duplicate AddressFilterNode.
     id_class_names = omniscript.get_id_class_names()
-    for k,v in id_class_names.items():
+    for k, v in id_class_names.items():
         if v == 'AddressFilterNode':
             if k not in _filter_id_to_class:
                 _filter_id_to_class[k] = _filter_name_class[1][1]
                 return
 
 
 def get_id_to_class():
@@ -62,16 +62,16 @@
     return None
 
 
 def parse_omni_filter_dict(element):
     if not isinstance(element, dict) and (_json_classid not in element):
         return None
     id_to_class = get_id_to_class()
-    node = id_to_class[OmniId(element[_json_classid])] #2 lines for debugging.
-    root = node(element) # step right into the __init__ function.
+    node = id_to_class[OmniId(element[_json_classid])]  # 2 lines for debugging.
+    root = node(element)  # step right into the __init__ function.
     if not root:
         return None
     if (_json_andnode in element) and (element[_json_andnode] is not None):
         root.and_node = parse_omni_filter_dict(element[_json_andnode])
     if (_json_ornode in element) and (element[_json_ornode] is not None):
         root.or_node = parse_omni_filter_dict(element[_json_ornode])
     return root
@@ -161,56 +161,56 @@
         mask = (mask << 1) | 1
     return mask << (bit_length - byte_count)
 
 
 def _bytes_to_hex_string(bytes):
     """Return a string of hex characters from a list of
     integers (bytes).
-    
+
     Args:
         bytes ([int]): list of integers:  [18, 52, 86, 120]
 
     Returns:
-        String: '12345678' 
+        String: '12345678'
     """
     return ''.join(hex(n)[2:] for n in bytes)
 
 
 def _hex_string_to_bytes(value):
     """Return a list of single byte intergers from each pair of
     hex characters.
 
     Args:
         value (string): string of hex characters: '12345678'
-    
+
     Returns:
         List of integers: [18, 52, 86, 120]
     """
     return [int(value[i:i+2], 16) for i in range(0, len(value), 2)]
 
 
 def _hex_string_to_shorts(value):
     """Return a list of short intergers from each four hex characters.
     Used to parse IPv6 hex strings into list of 16-bit values.
 
     Args:
         value (string): string of hex characters: '12345678'
-    
+
     Returns:
         List of integers: [4660, 22136]
     """
     return [int(value[i:i+4], 16) for i in range(0, len(value), 4)]
 
 
 def _hex_string_to_string(value):
     """Return a string from each pair of hex characters.
 
     Args:
         value (string): string of hex characters: '48656C6C6F'
-    
+
     Returns:
         String: 'Hello'
     """
     return ''.join(chr(int(value[i:i+2], 16)) for i in range(0, len(value), 2)).strip('\0')
 
 
 def parse_port_list(value):
@@ -224,26 +224,27 @@
 
 def _string_to_hex_string(value, pad=0):
     """Return a string of hex characters from a string.
 
     Args:
         value (string): string of hex characters: 'Hello'
         pad: min length of the resulting string.: 8
-    
+
     Returns:
         String: '48656C6C6F000000'
     """
     result = ''.join('%X' % ord(i) for i in value)
     if len(value) < pad:
         result += ''.join('00' for i in range(8 - len(value)))
     return result
 
 
 class DataIdType(object):
-    """Data Id Type"""
+    """Data Id Type object.
+    """
 
     id = None
     """The GUID of the type as a
     :class:`OmniId <omniscript.omniid.OmniId>` object.
     """
 
     data_type = DATA_TYPE_UNDEFINED
@@ -251,29 +252,31 @@
 
     def __init(self):
         self.id = DataIdType.id
         self.data_type = DataIdType.data_type
 
 
 class NamedDataType(object):
-    """The Named Data Type class."""
+    """The Named Data Type class.
+    """
 
     name = ''
     """The name of the type."""
 
     data_type = DATA_TYPE_UNDEFINED
     """The type of data/node. One of the DATA TYPE constants."""
 
     def __init__(self):
         self.name = NamedDataType.name
         self.data_type = NamedDataType.data_type
 
 
 class WirelessChannel(object):
-    """A wireless channel."""
+    """A wireless channel.
+    """
 
     channel = 0
     """The channel number."""
 
     frequency = 0
     """The channel's frequency."""
 
@@ -287,15 +290,15 @@
     def __init__(self):
         self.channel = WirelessChannel.channel
         self.frequency = WirelessChannel.frequency
         self.band = WirelessChannel.band
 
     def _load(self, props):
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 if k == WirelessChannel._tag_number:
                     self.channel_number = int(v)
                 elif k == WirelessChannel._tag_frequency:
                     self.channel_frequency = int(v)
                 elif k == WirelessChannel._tag_band:
                     self.channel_band = int(v)
 
@@ -319,29 +322,29 @@
     """The AND node."""
 
     or_node = None
     """The OR node."""
 
     comment = None
     """User supplied comment for this node."""
-    
+
     protospec_path = ''
     """The path of the protospec."""
 
     option_inverted = False
     """Is the logic of this node inverted?
     Default is False.
     """
 
     option_slice_to_header = False
     """Slice the packet to header?
     Default is False.
     """
 
-    #Tags
+    # Tags
     _json_comment = 'comment'
     _json_inverted = 'inverted'
     _json_slice_to_header = 'sliceToHeader'
     _json_protospec_path = 'protospecPath'
 
     _tag_comment = 'comment'
     _tag_inverted = 'option_inverted'
@@ -364,15 +367,15 @@
         self.protospec_path = FilterNode.protospec_path
         self.option_inverted = FilterNode.option_inverted
         self.option_slice_to_header = FilterNode.option_slice_to_header
 
     def _load(self, props):
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             a = FilterNode._filter_node_prop_dict.get(k)
             if a is not None and hasattr(self, a):
                 if a == FilterNode._tag_comment:
                     self.comment = v
                 elif a == FilterNode._tag_protospec_path:
                     self.protospec_path = v
                 elif a == FilterNode._tag_inverted:
@@ -382,15 +385,15 @@
 
     def _store(self, props):
         if not isinstance(props, dict):
             return
         props[FilterNode._json_inverted] = self.option_inverted
         if self.comment:
             props[FilterNode._json_comment] = self.comment
-        
+
     def to_string(self, pad, operation=""):
         text = ''
         if self.and_node:
             text += "\n" + self.and_node.to_string((pad+1), "and: ")
         if self.or_node:
             text += "\n" + self.or_node.to_string(pad, "or: ")
         return text
@@ -429,39 +432,47 @@
     def _store(self, props):
         if not isinstance(props, dict):
             return
         props[ApplicationNode._json_names] = ' '.join(self.names)
         super(ApplicationNode, self)._store(props)
 
     def to_string(self, pad, operation=""):
-        criteria  = '%s%s%s: %s%s' % (
+        criteria = '%s%s%s: %s%s' % (
             ''.ljust(pad * FilterNode.pad_depth),
             operation,
             ApplicationNode._display_name,
             _invert_string(self.option_inverted),
             self.names)
         return criteria + FilterNode.to_string(self, pad)
 
 
 class AddressNode(FilterNode):
     """The AddressNode class, subclass of the
     :class:`FilterNode <omniscript.filternode.FilterNode>` class.
     """
 
+    address_1 = None
+    """The address of the Node as a
+    :class:`OmniAddress <omniscript.omniaddress.OmniAddress>` object."""
+
+    address_2 = None
+    """The other address 2 of the Node as a
+    :class:`OmniAddress <omniscript.omniaddress.OmniAddress>` object."""
+
     address_list_1 = None
     """The first address as a list of
     :class:`OmniAddress <omniscript.omniaddress.OmniAddress>` object."""
 
     address_list_2 = None
     """The second address as a list of
     :class:`OmniAddress <omniscript.omniaddress.OmniAddress>` object."""
-    
+
     option_accept_1_to_2 = False
     """Accept traffic from the first to the second address."""
-    
+
     option_accept_2_to_1 = False
     """Accept traffic from the second to the first address."""
 
     _class_id = OmniId('D2ED5346-496C-4EA0-948E-21CDDA1ED723')
     _class_name = 'AddressFilterNode'
     _display_name = 'Address'
 
@@ -481,14 +492,16 @@
         _json_address_type: _tag_address_type,
         _json_accept_1_to_2: _tag_accept_1_to_2,
         _json_accept_2_to_1: _tag_accept_2_to_1
     }
 
     def __init__(self, props=None):
         super(AddressNode, self).__init__()
+        self.address_1 = AddressNode.address_1
+        self.address_2 = AddressNode.address_2
         self.address_list_1 = AddressNode.address_list_1
         self.address_list_2 = AddressNode.address_list_2
         self.option_accept_1_to_2 = AddressNode.option_accept_1_to_2
         self.option_accept_2_to_1 = AddressNode.option_accept_2_to_1
         self._load(props)
 
     def __str__(self):
@@ -496,37 +509,37 @@
                 f'{self.address_list_1} '
                 f'{_direction_string(self.option_accept_1_to_2, self.option_accept_2_to_1)} '
                 f'{self.address_list_2}')
 
     @property
     def accept_1_to_2(self):
         return self.option_accept_1_to_2
-    
+
     @accept_1_to_2.setter
     def accept_1_to_2(self, value):
         self.option_accept_1_to_2 = bool(value)
 
     @property
     def accept_2_to_1(self):
         return self.option_accept_2_to_1
-    
+
     @accept_2_to_1.setter
     def accept_2_to_1(self, value):
         self.option_accept_2_to_1 = bool(value)
 
     def _load(self, props):
         if not isinstance(props, dict):
             return
         super(AddressNode, self)._load(props)
         _address_1 = None
         _address_2 = None
         _address_type = None
-        for k,v in props.items():
+        for k, v in props.items():
             a = AddressNode._address_node_prop_dict.get(k)
-            #if a is None, then simply no match.
+            # if a is None, then simply no match.
             if a == AddressNode._tag_address_1:
                 _address_1 = v
             elif a == AddressNode._tag_address_2:
                 _address_2 = v
             elif a == AddressNode._tag_address_type:
                 _address_type = int(v)
             elif a == AddressNode._tag_accept_1_to_2:
@@ -535,18 +548,22 @@
                 self.option_accept_2_to_1 = v
         self.address_list_1 = OmniAddress('addr1', _address_1, _address_type).address_list
         self.address_list_2 = OmniAddress('addr2', _address_2, _address_type).address_list
 
     def _store(self, props):
         if not isinstance(props, dict):
             return
+        if isinstance(self.address_1, BaseAddress) and self.address_list_1 is None:
+            self.address_list_1 = [self.address_1]
+        if isinstance(self.address_2, BaseAddress) and self.address_list_2 is None:
+            self.address_list_2 = [self.address_2]
         addr_1 = [str(a) for a in self.address_list_1] if self.address_list_1 else []
         addr_2 = [str(a) for a in self.address_list_2] if self.address_list_2 else []
         _type = (self.address_list_1[0].address_type if self.address_list_1
-            else self.address_list_2[0].address_type if self.address_list_1 else 0)
+                 else self.address_list_2[0].address_type if self.address_list_1 else 0)
         props[_json_type] = _type
         props[AddressNode._json_address_1] = ' '.join(addr_1) if addr_1 else ''
         props[AddressNode._json_address_2] = ' '.join(addr_2) if addr_2 else ''
         props[_json_accept_1_to_2] = self.option_accept_1_to_2
         props[_json_accept_2_to_1] = self.option_accept_2_to_1
         super(AddressNode, self)._store(props)
 
@@ -594,15 +611,15 @@
     def _store(self, props):
         if not isinstance(props, dict):
             return
         props[BpfNode._json_filter] = self.filter
         super(BpfNode, self)._store(props)
 
     def to_string(self, pad, operation=""):
-        criteria  = '%s%s%s: %s%s' % (
+        criteria = '%s%s%s: %s%s' % (
             ''.ljust(pad * FilterNode.pad_depth),
             operation,
             BpfNode._display_name,
             _invert_string(self.option_inverted),
             self.filter)
         return criteria + FilterNode.to_string(self, pad)
 
@@ -638,15 +655,15 @@
     def _store(self, props):
         if not isinstance(props, dict):
             return
         props[ChannelNode._json_channel] = self.channel
         super(ChannelNode, self)._store(props)
 
     def to_string(self, pad, operation=""):
-        criteria  = '%s%s%s: %s%d' % (
+        criteria = '%s%s%s: %s%d' % (
             ''.ljust(pad * FilterNode.pad_depth),
             operation,
             ChannelNode._display_name,
             _invert_string(self.option_inverted),
             self.channel)
         return criteria + FilterNode.to_string(self, pad)
 
@@ -657,18 +674,18 @@
     """
 
     country_1 = None
     """The first country as a String."""
 
     country_2 = None
     """The second Country as a string."""
-    
+
     option_accept_1_to_2 = False
     """Accept traffic from the first to the second country."""
-    
+
     option_accept_2_to_1 = False
     """Accept traffic from the second to the first coutry."""
 
     _class_name = 'CountryFilterNode'
     _display_name = 'Country'
 
     country_1 = None
@@ -703,15 +720,15 @@
                 f'{_direction_string(self.option_accept_1_to_2, self.option_accept_2_to_1)} '
                 f'{self.country_2}')
 
     def _load(self, props):
         if not isinstance(props, dict):
             return
         super(CountryNode, self)._load(props)
-        for k,v in props.items():
+        for k, v in props.items():
             a = CountryNode._country_node_prop_dict.get(k)
             if a == CountryNode._tag_country_1:
                 self.country_1 = v
             elif a == CountryNode._tag_country_2:
                 self.country_2 = v
             elif a == CountryNode._tag_accept_1_to_2:
                 self.option_accept_1_to_2 = v
@@ -724,23 +741,21 @@
         props[CountryNode._json_country_1] = self.country_1
         props[CountryNode._json_country_2] = self.country_2
         props[_json_accept_1_to_2] = self.option_accept_1_to_2
         props[_json_accept_2_to_1] = self.option_accept_2_to_1
         super(CountryNode, self)._store(props)
 
     def to_string(self, pad, operation=""):
-        criteria  = '%s%s%s: %s%s %s %s' % (
+        criteria = '%s%s%s: %s%s %s %s' % (
             ''.ljust(pad * FilterNode.pad_depth),
             operation,
             CountryNode._display_name,
-            _invert_string(self.option_inverted),
-            self.country_1,
-            _direction_string(
-                self.option_accept_1_to_2, self.option_accept_2_to_1),
-                self.country_2)
+            _invert_string(self.option_inverted), self.country_1,
+            _direction_string(self.option_accept_1_to_2, self.option_accept_2_to_1),
+            self.country_2)
         return criteria + FilterNode.to_string(self, pad)
 
 
 class ErrorNode(FilterNode):
     """The ErrorNode class, subclass of the
     :class:`FilterNode <omniscript.filternode.FilterNode>` class.
     """
@@ -793,15 +808,15 @@
         errorflags |= [0, ERROR_FLAG_CRC][self.option_crc_errors]
         errorflags |= [0, ERROR_FLAG_FRAME][self.option_frame_errors]
         errorflags |= [0, ERROR_FLAG_OVERSIZE][self.option_oversize_errors]
         errorflags |= [0, ERROR_FLAG_RUNT][self.option_runt_errors]
         props[ErrorNode._json_flags] = errorflags
 
     def to_string(self, pad, operation=""):
-        criteria  = '%s%s%s: %scrc:%s frame:%s oversize:%s runt:%s' % (
+        criteria = '%s%s%s: %scrc:%s frame:%s oversize:%s runt:%s' % (
             ''.ljust(pad * FilterNode.pad_depth),
             operation,
             ErrorNode._display_name,
             _invert_string(self.option_inverted),
             ['F', 'T'][self.option_crc_errors],
             ['F', 'T'][self.option_frame_errors],
             ['F', 'T'][self.option_oversize_errors],
@@ -848,30 +863,30 @@
     def __str__(self):
         return f'{LengthNode._class_name}: {self.minimum} to {self.maximum}'
 
     def _load(self, props):
         if not isinstance(props, dict):
             return
         super(LengthNode, self)._load(props)
-        for k,v in props.items():
+        for k, v in props.items():
             a = LengthNode._length_node_prop_dict.get(k)
             if a == LengthNode._tag_minimum:
                 self.minimum = int(v)
             elif a == LengthNode._tag_maximum:
                 self.maximum = int(v)
 
     def _store(self, props):
         if not isinstance(props, dict):
             return
         props[LengthNode._json_minimum] = self.minimum
         props[LengthNode._json_maximum] = self.maximum
         super(LengthNode, self)._store(props)
 
     def to_string(self, pad, operation=""):
-        criteria  = '%s%s%s: %smin:%d max:%d' % (
+        criteria = '%s%s%s: %smin:%d max:%d' % (
             ''.ljust(pad * FilterNode.pad_depth),
             operation,
             LengthNode._display_name,
             _invert_string(self.option_inverted),
             self.minimum,
             self.maximum)
         return criteria + FilterNode.to_string(self, pad)
@@ -938,17 +953,17 @@
             _right = {}
             self.left.store(_right)
             props[LogicalNode._json_right] = _right
         super(LogicalNode, self)._store(props)
 
     def to_string(self, pad, operation=""):
         _padding = ''.ljust(pad * FilterNode.pad_depth)
-        _padding_plus = ''.ljust((pad+1)* FilterNode.pad_depth)
+        _padding_plus = ''.ljust((pad+1) * FilterNode.pad_depth)
 
-        criteria  = '%s%s%s: %s %s\n%sleft:%s\n%sright:%s' % (
+        criteria = '%s%s%s: %s %s\n%sleft:%s\n%sright:%s' % (
             _padding,
             operation,
             LogicalNode._display_name,
             _invert_string(self.option_inverted),
             LogicalNode._op_names[self.operator],
             _padding_plus,
             self.left.to_string(pad+1),
@@ -1032,31 +1047,31 @@
     def __str__(self):
         return f'{PatternNode._class_name}: {self.pattern}'
 
     def _load(self, props):
         if not isinstance(props, dict):
             return
         super(PatternNode, self)._load(props)
-        for k,v in props.items():
+        for k, v in props.items():
             a = PatternNode._pattern_node_prop_dict.get(k)
-            if a ==PatternNode._tag_pattern_type:
+            if a == PatternNode._tag_pattern_type:
                 self.pattern_type = int(v)
-            elif a ==PatternNode._tag_pattern:
+            elif a == PatternNode._tag_pattern:
                 self.pattern = v
-            elif a ==PatternNode._tag_case_sensitive:
+            elif a == PatternNode._tag_case_sensitive:
                 self.option_case_sensitive = v
-            elif a ==PatternNode._tag_code_page:
+            elif a == PatternNode._tag_code_page:
                 self.code_page = int(v)
-            elif a ==PatternNode._tag_start_offset:
+            elif a == PatternNode._tag_start_offset:
                 self.start_offset = int(v)
-            elif a ==PatternNode._tag_end_offset:
+            elif a == PatternNode._tag_end_offset:
                 self.end_offset = int(v)
-            elif a ==PatternNode._tag_protocol_specification:
+            elif a == PatternNode._tag_protocol_specification:
                 self.protocol_specification = int(v)
-            elif a ==PatternNode._tag_flags:
+            elif a == PatternNode._tag_flags:
                 self.flags = int(v)
 
     def _store(self, props):
         if not isinstance(props, dict):
             return
         props[PatternNode._json_pattern_type] = self.pattern_type
         props[PatternNode._json_pattern] = self.pattern
@@ -1076,15 +1091,15 @@
             self.pattern = ''.join(("%02X" % ord(x)) for x in value)
             self.pattern_type = PATTERN_TYPE_ASCII
         else:
             self.pattern = str(value)
             self.pattern_type = PATTERN_TYPE_ASCII
 
     def to_string(self, pad, operation=""):
-        criteria  = '%s%s%s: %s%s begin:%d end:%d' % (
+        criteria = '%s%s%s: %s%s begin:%d end:%d' % (
             ''.ljust(pad * FilterNode.pad_depth),
             operation,
             PatternNode._display_name,
             _invert_string(self.option_inverted),
             self.pattern,
             self.start_offset,
             self.end_offset)
@@ -1093,15 +1108,15 @@
 
 class PluginNode(FilterNode):
     """The PluginNode class, subclass of the
     :class:`FilterNode <omniscript.filternode.FilterNode>` class.
     """
 
     ids = []
-    """A list of plugin ids as a list of 
+    """A list of plugin ids as a list of
     :class:`OmniId <omniscript.omniid.OmniId>` objects.
     Use the add_analysis_module function to add items to the list.
     """
 
     _class_name = 'PluginFilterNode'
     _display_name = 'Plugin'
 
@@ -1135,15 +1150,15 @@
             self.ids.append(clsid)
         elif isinstance(clsid, six.string_types):
             self.ids.append(OmniId(clsid))
         elif isinstance(clsid, AnalysisModule):
             self.ids.append(clsid.id)
 
     def to_string(self, pad, operation=""):
-        criteria  = '%s%s%s: %s%s' % (
+        criteria = '%s%s%s: %s%s' % (
             ''.ljust(pad * FilterNode.pad_depth),
             operation,
             PluginNode._display_name,
             _invert_string(self.option_inverted),
             f'{" ".join(i.format() for i in self.ids)}')
         return criteria + FilterNode.to_string(self, pad)
 
@@ -1156,18 +1171,18 @@
     port_list_1 = None
     """The first list of
     :class:`OmniPort <omniscript.omniport.OmniPort>` object."""
 
     port_list_2 = None
     """The second list of
     :class:`OmniPort <omniscript.omniport.OmniPort>` object."""
-    
+
     option_accept_1_to_2 = False
     """Accept traffic from the first to the second address."""
-    
+
     option_accept_2_to_1 = False
     """Accept traffic from the second to the first address."""
 
     _class_name = 'PortFilterNode'
     _display_name = 'Port'
 
     _json_port_1 = 'port1'
@@ -1199,25 +1214,25 @@
                 f'{_direction_string(self.option_accept_1_to_2, self.option_accept_2_to_1)} '
                 f'{self.port_2}')
 
     def _load(self, props):
         if not isinstance(props, dict):
             return
         super(PortNode, self)._load(props)
-        for k,v in props.items():
+        for k, v in props.items():
             a = PortNode._port_node_prop_dict.get(k)
             if a == PortNode._tag_port_1:
                 self.port_list_1 = parse_port_list(v)
             elif a == PortNode._tag_port_2:
                 self.port_list_2 = parse_port_list(v)
             elif a == PortNode._tag_accept_1_to_2:
                 self.option_accept_1_to_2 = v
             elif a == PortNode._tag_accept_2_to_1:
                 self.option_accept_2_to_1 = v
-        
+
     def _store(self, props):
         if not isinstance(props, dict):
             return
         port_1 = [str(a) for a in self.port_list_1] if self.port_list_1 else []
         port_2 = [str(a) for a in self.port_list_2] if self.port_list_2 else []
         _type = (self.port_list_1[0].port_type if self.port_list_1
                  else self.port_list_2[0].port_type if self.port_list_2 else 0)
@@ -1290,15 +1305,15 @@
         super(ProtocolNode, self)._store(props)
 
     def set_protocol(self, name):
         name_ids = omniscript.get_protocol_short_name_ids()
         self.protocol = name_ids.get(name, 0)
 
     def to_string(self, pad, operation=""):
-        criteria  = '%s%s%s: %s%d' % (
+        criteria = '%s%s%s: %s%d' % (
             ''.ljust(pad * FilterNode.pad_depth),
             operation,
             ProtocolNode._display_name,
             _invert_string(self.option_inverted),
             self.protocol)
         return criteria + FilterNode.to_string(self, pad)
 
@@ -1348,15 +1363,15 @@
         if self.start:
             props[TimeRangeNode._json_start] = self.start
         if self.end:
             props[TimeRangeNode._json_end] = self.end
         super(TimeRangeNode, self)._store(props)
 
     def to_string(self, pad, operation=""):
-        criteria  = '%s%s%s: %sstart: %s end: %s' % (
+        criteria = '%s%s%s: %sstart: %s end: %s' % (
             ''.ljust(pad * FilterNode.pad_depth),
             operation,
             TimeRangeNode._display_name,
             _invert_string(self.option_inverted),
             str(self.start),
             str(self.end))
         return criteria + FilterNode.to_string(self, pad)
@@ -1436,15 +1451,15 @@
                 f'off:{self.offset} '
                 f'len:{self.length}')
 
     def _load(self, props):
         if not isinstance(props, dict):
             return
         super(ValueNode, self)._load(props)
-        for k,v in props.items():
+        for k, v in props.items():
             a = ValueNode._value_node_prop_dict.get(k)
             if a == ValueNode._tag_value:
                 if isinstance(v, dict) and (_json_data in v):
                     self.value = int(v[_json_data])
             elif a == ValueNode._tag_mask:
                 if isinstance(v, dict) and (_json_data in v):
                     self.mask = int(v[_json_data])
@@ -1472,15 +1487,15 @@
             'pspec': 1000
         }
         props[ValueNode._json_operator] = self.operator
         props[ValueNode._json_flags] = self.flags
         super(ValueNode, self)._store(props)
 
     def to_string(self, pad, operation=""):
-        criteria  = '%s%s%s: %s%s' % (
+        criteria = '%s%s%s: %s%s' % (
             ''.ljust(pad * FilterNode.pad_depth),
             operation,
             ValueNode._display_name,
             _invert_string(self.option_inverted),
             self.value)
         return criteria + FilterNode.to_string(self, pad)
 
@@ -1488,18 +1503,18 @@
 class VlanMplsNode(FilterNode):
     """The VlanMplsNode class, subclass of the
     :class:`FilterNode <omniscript.filternode.FilterNode>` class.
     """
 
     ids = None
     """A list of VLAN Ids and Id ranges."""
-    
+
     labels = None
     """A list of MPLS Labels and Label ranges."""
-    
+
     _class_name = 'VlanFilterNode'
     _display_name = 'Vlan-Mpls'
 
     _json_ids = 'ids'
     _json_labels = 'labels'
 
     def __init__(self, props=None):
@@ -1532,15 +1547,15 @@
         props[VlanMplsNode._json_ids] = ''
         props[VlanMplsNode._json_labels] = ''
         if self.ids:
             props[VlanMplsNode._json_ids] = (' '.join(str(id) if isinstance(id, int)
                                              else '-'.join(str(i) for i in id) for id in self.ids))
         if self.labels:
             props[VlanMplsNode._json_labels] = (' '.join(str(lb) if isinstance(lb, int)
-                                                else '-'.join(str(l) for l in lb)
+                                                else '-'.join(str(i) for i in lb)
                                                 for lb in self.labels))
         super(VlanMplsNode, self)._store(props)
 
     def add_id(self, id):
         """Add a VLAN Id or Id range."""
         if isinstance(id, int):
             self.ids.append(id)
@@ -1550,15 +1565,15 @@
                 if len(items) == 1:
                     self.ids.append(int(items[0]))
                 elif len(items) > 1:
                     self.ids.append((int(items[0]), int(items[1])))
 
     def add_ids(self, *ids):
         """Add multiple VLAN Ids and/or Id ranges.
-        Either as a string: '10 100-110 256' or a list: 
+        Either as a string: '10 100-110 256' or a list:
         (10, '100-110', 256).
         If the list contains a range, the range must be quoted.
         """
         if isinstance(ids, list) or isinstance(ids, tuple):
             for id in ids:
                 if isinstance(id, int) or isinstance(id, six.string_types):
                     self.add_id(id)
@@ -1593,15 +1608,15 @@
                 else:
                     self.add_labels(label)
         elif isinstance(labels, six.string_types):
             for label in labels:
                 self.add_label(label)
 
     def to_string(self, pad, operation=""):
-        criteria  = '%s%s%s: %sIds:%s Labels:%s' % (
+        criteria = '%s%s%s: %sIds:%s Labels:%s' % (
             ''.ljust(pad * FilterNode.pad_depth),
             operation,
             VlanMplsNode._display_name,
             _invert_string(self.option_inverted),
             self.ids,
             self.labels)
         return criteria + FilterNode.to_string(self, pad)
@@ -1610,15 +1625,15 @@
 class WANDirectionNode(FilterNode):
     """The WANDirectionNode class, subclass of the
     :class:`FilterNode <omniscript.filternode.FilterNode>` class.
     """
 
     direction = WAN_DIRECTION_UNDEFINED
     """Direction: to the DCE (1) or to the DTE (2)."""
-    
+
     _class_name = 'DirectionFilterNode'
     _display_name = 'WAN Direction'
 
     _json_direction = 'direction'
 
     def __init__(self, props=None):
         super(WANDirectionNode, self).__init__()
@@ -1640,15 +1655,15 @@
         if not isinstance(props, dict):
             return
         if self.direction != WAN_DIRECTION_UNDEFINED:
             props[WANDirectionNode._json_direction] = self.direction
         super(WANDirectionNode, self)._store(props)
 
     def to_string(self, pad, operation=""):
-        criteria  = '%s%s%s: %s%s' % (
+        criteria = '%s%s%s: %s%s' % (
             ''.ljust(pad * FilterNode.pad_depth),
             operation,
             WANDirectionNode._display_name,
             _invert_string(self.option_inverted),
             ['Unknown', 'to DCE', 'to DTE'][self.direction])
         return criteria + FilterNode.to_string(self, pad)
 
@@ -1672,15 +1687,15 @@
     data_rate = None
     """The Data Rate, in megabits per second, to filter as a floating point
     value.
     """
 
     flags = None
     """The flags. A set of the WIRELESS FLAG constants."""
-    
+
     signal_minimum = None
     """The Minumum Signal to filter on."""
 
     signal_maximum = None
     """The Maximum Signal to filter on."""
 
     noise_minimum = None
@@ -1736,15 +1751,15 @@
         self.signal_minimum = WirelessNode.signal_minimum
         self.signal_maximum = WirelessNode.signal_maximum
         self.noise_minimum = WirelessNode.noise_minimum
         self.noise_maximum = WirelessNode.noise_maximum
         self.encryption = WirelessNode.encryption
         self.decryption = WirelessNode.decryption
         self.bssid = WirelessNode.bssid
-        self.mask_bssid = WirelessNode.mask_bssid 
+        self.mask_bssid = WirelessNode.mask_bssid
         self._load(props)
 
     def __str__(self):
         return (f'{WirelessNode._class_name}: '
                 f'ch:{self.channel_number} '
                 f'Hz:{self.channel_frequency} '
                 f'band:{self.channel_band}')
@@ -1752,28 +1767,28 @@
     def _load(self, props):
         if not isinstance(props, dict):
             return
         super(WirelessNode, self)._load(props)
         if WirelessNode._json_channel in props:
             channel = props[WirelessNode._json_channel]
             if isinstance(channel, dict):
-                for k,v in channel.items():
+                for k, v in channel.items():
                     a = WirelessNode._wireless_node_prop_dict.get(k)
                     if a == WirelessNode._tag_channel_number:
                         self.channel_number = int(v)
                     elif a == WirelessNode._tag_channel_frequency:
                         self.channel_frequency = int(v)
                     elif a == WirelessNode._tag_channel_band:
                         self.channel_band = int(v)
         # if 'dataRate' in props:
         #     datarate = props['datarate']
         #     if datarate is not None:
         #         data_rate = int(datarate.get('data', '0'))
         #         self.data_rate = data_rate / 2.0
-        
+
         # signal = props.find('signal')
         # if signal is not None:
         #     self.signal_minimum = int(signal.get('min', '0'))
         #     self.signal_maximum = int(signal.get('max', '0'))
         # noise = props.find('noise')
         # if noise is not None:
         #     self.noise_minimum = int(noise.get('min', '0'))
@@ -1815,15 +1830,15 @@
         #                   {'data':['0', '1'][self.decryption]})
         # if self.bssid is not None:
         #     self.bssid._store(props)
         # if self.flags is not None:
         #     ET.SubElement(props, 'flagsn', {'data':str(self.flags)})
 
     def to_string(self, pad, operation=""):
-        criteria  = '%s%s%s: %s%s' % (
+        criteria = '%s%s%s: %s%s' % (
             ''.ljust(pad * FilterNode.pad_depth),
             operation,
             WirelessNode._display_name,
             _invert_string(self.option_inverted),
             int(self.channel_number) if self.channel_number else '')
         return criteria + FilterNode.to_string(self, pad)
 
@@ -1843,15 +1858,15 @@
     ('PortFilterNode', PortNode),
     ('ProtocolFilterNode', ProtocolNode),
     ('TimeRangeFilterNode', TimeRangeNode),
     ('ValueFilterNode', ValueNode),
     ('VlanFilterNode', VlanMplsNode),
     ('DirectionFilterNode', WANDirectionNode),
     ('WirelessFilterNode', WirelessNode)
-    ]
+]
 
 _console_filter_id_class = {
     OmniId('{B4298A64-5A40-4F5F-ABCD-B14BA0F8D9EB}'): None,
     OmniId('{2D2D9B91-08BF-44CF-B240-F0BBADBF21B5}'): AddressNode,
     OmniId('{8C7C9172-82B2-43DC-AAF1-41ED80CE828F}'): ApplicationNode,
     OmniId('{11FC8E5E-B21E-446B-8024-39E41E6865E1}'): BpfNode,
     OmniId('{6E8DAF74-AF0D-4CD3-865D-D559A5798C5B}'): ChannelNode,
@@ -1864,8 +1879,8 @@
     OmniId('{297D404D-3610-4A18-95A2-22768B554BED}'): PortNode,
     OmniId('{F4342DAD-4A56-4ABA-9436-6E3C30DAB1C8}'): ProtocolNode,
     OmniId('{85F2216E-6E65-4AE9-B14B-CC8DF48CAE6A}'): TimeRangeNode,
     OmniId('{838F0E57-0D9F-4095-9C12-F1040C84E428}'): ValueNode,
     OmniId('{1999CC65-01DA-4256-81B4-C303BDE88BDA}'): VlanMplsNode,
     OmniId('{90BAE500-B97B-42B0-9886-0947F34001EF}'): WANDirectionNode,
     OmniId('{899E11AD-1849-40BA-9454-9F03798B3A6C}'): WirelessNode
-    }
+}
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/forensicsearch.py` & `omniscript-liveaction-3.0.49/src/omniscript/forensicsearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 ﻿"""ForensicSearch class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
-from ast import For
 import six
-import struct
 import xml.etree.ElementTree as ET
 
 import omniscript
 
-from .invariant import (DECODE_PLAIN_TEXT, DECODE_HTML, DECODE_TAG_STREAM,
-    MEDIA_TYPE_802_3, MEDIA_SUB_TYPE_NATIVE, OMNI_GET_STATS, OMNI_EXPERT_EXECUTE_QUERY,
-    OMNI_GET_STATS_CONTEXT)
+from .invariant import (
+    DECODE_PLAIN_TEXT, DECODE_HTML, DECODE_TAG_STREAM, MEDIA_TYPE_802_3, MEDIA_SUB_TYPE_NATIVE,
+    OMNI_EXPERT_EXECUTE_QUERY)
 
 # from expertresult import _create_expert_result_list
 from .invariant import EngineDataFormat as DF
 from .mediainformation import MediaInformation
 # from nodestatistic import NodeStatistic
 from .omnierror import OmniError
 from .omniid import OmniId
 from .peektime import PeekTime
 # from protocolstatistic import ProtocolStatistic
 # from statscontext import StatsContext
 # from summarystatistic import SummaryStatistic
 
 
-find_attribs = ['name', 'id']
-
 _forensic_prop_dict = {
     'id': 'id',
     'name': 'name',
     'adapter': 'adapter',
     'pluginsEnabled': 'analysis_modules',
     'captureName': 'capture_name',
     'captureSessionId': 'session_id',
@@ -69,15 +65,16 @@
     'statsEnabled': 'option_statistics',
     'voiceEnabled': 'option_voice',
     'webEnabled': 'option_web'
 }
 
 
 class ForensicSearch(object):
-    """Forensic Search class"""
+    """Forensic Search class.
+    """
 
     id = None
     """The identifier of the search as an OmniId."""
 
     name = ''
     """The name of the search."""
 
@@ -173,15 +170,15 @@
     status = 0
     """The status of the search: loading = 0, processing = 1, complete = 2."""
 
     statistics = []
     """The ids of the Statistics used by the Forensic Search."""
 
     stop_time = None
-    """The ending of the time range, as 
+    """The ending of the time range, as
     :class:`PeekTime <omniscript.peektime.PeekTime>`,
     of packets to search."""
 
     user = ''
     """The currently logged on User Account."""
 
     option_expert = False
@@ -200,15 +197,17 @@
     """Is the Packet Buffer option enabled."""
 
     option_voice = False
     """Is the Voice and Video Statistics option enabled."""
 
     option_web = False
     """Is the Web Statistics option enabled."""
-    
+
+    find_attributes = ('name', 'id')
+
     def __init__(self, props, engine):
         self._engine = engine
 
         self.id = ForensicSearch.id
         self.name = ForensicSearch.name
         self.adapter = ForensicSearch.adapter
         self.analysis_modules = ForensicSearch.analysis_modules
@@ -251,19 +250,19 @@
 
     # def _get_statistics(self):
     #     """Get the Statistics, a binary blob of data."""
     #     if self.id is None:
     #         self.logger.error("Failed to get the id for Capture: %s",
     #                           self.name)
     #         return None
-    #     #self._context = self._engine._api_issue_command(
+    #     # self._context = self._engine._api_issue_command(
     #     #                   OMNI_GET_STATS_CONTEXT, str(self.id), 0)
     #     request = struct.pack('16sQ', self.id.bytes_le(), 0)
     #     data = self._engine._issue_command(OMNI_GET_STATS, request, 24)
-    #     #with open(r"c:\temp\stat_data.bin", 'wb') as fle:
+    #     # with open(r"c:\temp\stat_data.bin", 'wb') as fle:
     #     #    fle.write(data)
     #     self._context = StatsContext(data.raw)
 
     def get_application_stats(self, refresh=False):
         """Returns a list of
         :class:`ApplicationStatistic <omniscript.applicationstatistic.ApplicationStatistic>`
         objects.
@@ -276,15 +275,15 @@
         if self._context is None:
             self.logger.error(
                 f'Failed to get statistics context for forensic search: {self.name}.')
             return None
         return self._context.get_application_statistics()
 
     def get_call_stats(self, refresh=False):
-        """Returns a 
+        """Returns a
         :class:`CallStatistic <omniscript.callstatistic.CallStatistic>`
         object.
         Note that only one CallStatistic object is returned.
 
         Args:
             refresh (boolean): refresh the statistics cache. Default is False.
         """
@@ -318,19 +317,19 @@
         objects.
         """
         if self._context is None:
             self._get_statistics()
         if self._context is None:
             self.logger.error(f'Failed to get statistics context for capture: {self.name}.')
             return None
-        #node_stats = self._engine._get_stats(self._context, STATS_NODE)
-        #lst = []
-        #for ns in node_stats:
+        # node_stats = self._engine._get_stats(self._context, STATS_NODE)
+        # lst = []
+        # for ns in node_stats:
         #    lst.append(NodeStatistic(ns))
-        #return lst
+        # return lst
         return self._context.get_node_statistics()
 
     def get_packet_data(self, number):
         """Returns a bytearry of the packet data.
 
         Notes:
             The first packet number is 1.
@@ -369,33 +368,33 @@
 
         command = f'forensic-searches/{self.id.format()}/packets/{number}/'
         resp = self._engine._issue_command(command, format=decode)
         return resp
 
     def get_protocol_stats(self):
         """Returns a list of
-        :class:`ProtocolStatistic 
+        :class:`ProtocolStatistic
         <omniscript.protocolstatistic.ProtocolStatistic>`
         objects.
         """
         if self._context is None:
             self._get_statistics()
         if self._context is None:
             self.logger.error(f'Failed to get statistics context for capture: {self.name}.')
             return None
-        #protocol_stats = self._engine._get_stats(self._context, STATS_PROTOCOL)
-        #lst = []
-        #for ps in protocol_stats:
+        # protocol_stats = self._engine._get_stats(self._context, STATS_PROTOCOL)
+        # lst = []
+        # for ps in protocol_stats:
         #    lst.append(ProtocolStatistic(ps))
-        #return lst
+        # return lst
         return self._context.get_protocol_statistics()
 
     def get_stats_context(self, refresh=False):
-        """Returns a 
-        :class:`StatsContext 
+        """Returns a
+        :class:`StatsContext
         <omniscript.statscontext.StatsContext>`
         object.
 
         Args:
             refresh (boolean): refresh the statistics context. Default is False.
         """
         if self._context is None or refresh:
@@ -404,31 +403,31 @@
             self.logger.error(
                 f'Failed to get statistics context for forensic search: {self.name}.')
             return None
         return self._context
 
     def get_summary_stats(self):
         """Returns a list of
-        :class:`SummaryStatistic 
+        :class:`SummaryStatistic
         <omniscript.summarystatistic.SummaryStatistic>`
         objects.
         """
         if self._context is None:
             self._get_statistics()
         if self._context is None:
             self.logger.error(f'Failed to get statistics context for capture: {self.name}.')
             return None
-        #summary_stats = self._engine._get_stats(self._context, STATS_SUMMARY)
-        #return _summary_xml_to_stats_list(summary_xml)
+        # summary_stats = self._engine._get_stats(self._context, STATS_SUMMARY)
+        # return _summary_xml_to_stats_list(summary_xml)
         return self._context.get_summary_statistics()
 
     def load(self, props):
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             a = _forensic_prop_dict.get(k)
             if a is None or not hasattr(self, a):
                 continue
             if isinstance(getattr(self, a), six.string_types):
                 setattr(self, a, v)
             elif isinstance(getattr(self, a), bool):
                 setattr(self, a, int(v) != 0)
@@ -455,15 +454,15 @@
 
         Returns a list of
         :class:`ExpertResult <omniscript.expertresult.ExpertResult>` objects.
         Match the result to the query by the table name.
         """
         querys = query_list if isinstance(query_list, list) else [query_list]
         request = ET.Element('request')
-        msg = ET.SubElement(request, 'msg', {'capture-id':str(self.id)})
+        msg = ET.SubElement(request, 'msg', {'capture-id': str(self.id)})
         for q in querys:
             q._store(msg)
         xml = ET.tostring(msg).replace('\n', '')
         response = self._engine._issue_xml_command(OMNI_EXPERT_EXECUTE_QUERY, xml)
         querys = omniscript._parse_command_response(response, 'msg')
         # return _create_expert_result_list(querys)
         return []
@@ -516,22 +515,22 @@
     if searches is not None:
         for props in searches:
             lst.append(ForensicSearch(props, engine))
     lst.sort(key=lambda x: x.name)
     return lst
 
 
-def find_forensic_search(searches, value, attrib=find_attribs[0]):
+def find_forensic_search(searches, value, attrib=ForensicSearch.find_attributes[0]):
     """Finds a forensic search in the list"""
-    if (not searches) or (attrib not in find_attribs):
+    if (not searches) or (attrib not in ForensicSearch.find_attributes):
         return []
 
     if len(searches) == 0:
         return []
 
     if isinstance(value, ForensicSearch):
         _value = value.id
         attrib = 'id'
     else:
         _value = value
-    
+
     return next((i for i in searches if getattr(i, attrib) == _value), [])
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/forensictemplate.py` & `omniscript-liveaction-3.0.49/src/omniscript/forensictemplate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 ﻿"""ForensicTemplate class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
-from distutils.command.install_egg_info import install_egg_info
 import json
-from pydoc import cli
 import six
 
 import xml.etree.ElementTree as ET
 
 import omniscript
 from omniscript.adapter import Adapter
 
-from .invariant import (LIMIT_TYPE_NONE, LIMIT_TYPE_PACKETS, LIMIT_TYPE_BYTES, LIMIT_TYPE_BUFFER,
-    MEDIA_TYPE_802_3, MEDIA_SUB_TYPE_NATIVE, MODE_ACCEPT_ALL, BYTES_PER_KILOBYTE,
-    BYTES_PER_MEGABYTE, PROP_BAG_FALSE, PROP_BAG_TRUE)
+from .invariant import (
+    LIMIT_TYPE_NONE, LIMIT_TYPE_PACKETS, LIMIT_TYPE_BYTES, LIMIT_TYPE_BUFFER, MEDIA_TYPE_802_3,
+    MEDIA_SUB_TYPE_NATIVE, MODE_ACCEPT_ALL, BYTES_PER_KILOBYTE, BYTES_PER_MEGABYTE, PROP_BAG_FALSE,
+    PROP_BAG_TRUE)
 
 from .analysismodule import AnalysisModule
 from .capturetemplate import VoIPSettings
 from .fileinformation import FileInformation
 from .filter import Filter
 from .omniid import OmniId
 from .packetfileinformation import PacketFileInformation
@@ -43,57 +42,57 @@
 
 _json_accept = 'accept'
 _json_enabled = 'enabled'
 _json_items = 'items'
 _json_type = 'type'
 
 stats_labels = {
-    '_option_break_out':'BreakOutStats',
-    'option_expert':'Expert',
-    'option_graphs':'Graphs',
-    'option_indexing':'Index',
-    'option_log':'Log',
-    'option_packets':'Packets',
-    'option_plugins':'Plugins',
-    'option_statistics':'Statistics',
-    'option_voice':'Voice',
-    '_option_web':'Web'
+    '_option_break_out': 'BreakOutStats',
+    'option_expert': 'Expert',
+    'option_graphs': 'Graphs',
+    'option_indexing': 'Index',
+    'option_log': 'Log',
+    'option_packets': 'Packets',
+    'option_plugins': 'Plugins',
+    'option_statistics': 'Statistics',
+    'option_voice': 'Voice',
+    '_option_web': 'Web'
 }
 
 break_out_stats = {
-    'ApplicationStats':'option_application',
-    'BreakOutStats':'_option_break_out',
-    'CountryStats':'option_country',
-    'ErrorStats':'option_error',
-    'HistoryStats':'option_history',
-    'NetworkStats':'option_network',
-    'NodeStats':'option_node',
-    'ConversationStats':'option_node_protocol_detail',
-    'ProtocolStats':'option_protocol',
-    'SizeStats':'option_size',
-    'SummaryStats':'option_summary',
-    'TopTalkerStats':'option_top_talkers',
-    'WirelessChannelStats':'option_wireless_channel',
-    'WirelessNodeStats':'option_wireless_node'
+    'ApplicationStats': 'option_application',
+    'BreakOutStats': '_option_break_out',
+    'CountryStats': 'option_country',
+    'ErrorStats': 'option_error',
+    'HistoryStats': 'option_history',
+    'NetworkStats': 'option_network',
+    'NodeStats': 'option_node',
+    'ConversationStats': 'option_node_protocol_detail',
+    'ProtocolStats': 'option_protocol',
+    'SizeStats': 'option_size',
+    'SummaryStats': 'option_summary',
+    'TopTalkerStats': 'option_top_talkers',
+    'WirelessChannelStats': 'option_wireless_channel',
+    'WirelessNodeStats': 'option_wireless_node'
 }
 
 break_out_stats_labels = {
-    'option_application':'ApplicationStats',
-    'option_country':'CountryStats',
-    'option_error':'ErrorStats',
-    'option_history':'HistoryStats',
-    'option_network':'NetworkStats',
-    'option_node':'NodeStats',
-    'option_node_protocol_detail':'ConversationStats',
-    'option_protocol':'ProtocolStats',
-    'option_size':'SizeStats',
-    'option_summary':'SummaryStats',
-    'option_top_talkers':'TopTalkerStats',
-    'option_wireless_channel':'WirelessChannelStats',
-    'option_wireless_node':'WirelessNodeStats'
+    'option_application': 'ApplicationStats',
+    'option_country': 'CountryStats',
+    'option_error': 'ErrorStats',
+    'option_history': 'HistoryStats',
+    'option_network': 'NetworkStats',
+    'option_node': 'NodeStats',
+    'option_node_protocol_detail': 'ConversationStats',
+    'option_protocol': 'ProtocolStats',
+    'option_size': 'SizeStats',
+    'option_summary': 'SummaryStats',
+    'option_top_talkers': 'TopTalkerStats',
+    'option_wireless_channel': 'WirelessChannelStats',
+    'option_wireless_node': 'WirelessNodeStats'
 }
 
 limit_types = {
     'none': LIMIT_TYPE_NONE,
     'packets': LIMIT_TYPE_PACKETS,
     'bytes': LIMIT_TYPE_BYTES,
     'buffer': LIMIT_TYPE_BUFFER
@@ -107,38 +106,39 @@
 def _get_clsid(clsid_name):
     class_name_ids = omniscript.get_class_name_ids()
     id = class_name_ids[clsid_name]
     return id.format() if id else ''
 
 
 def _set_clsid(obj, clsid_name):
-    if not _tag_clsid in obj.attrib:
+    if _tag_clsid not in obj.attrib:
         class_name_ids = omniscript.get_class_name_ids()
         obj.attrib[_tag_clsid] = str(class_name_ids[clsid_name])
 
 
 def _set_property_value(parent, value_type, value):
     if not isinstance(value, six.string_types):
         value = str(value)
     ET.SubElement(parent, _tag_prop,
-                  {_tag_type:str(value_type)}).text = value
+                  {_tag_type: str(value_type)}).text = value
 
 
 def _to_prop_boolean(value):
     if isinstance(value, six.string_types):
         if int(value):
             return PROP_BAG_TRUE
         return PROP_BAG_FALSE
     if value:
         return PROP_BAG_TRUE
     return PROP_BAG_FALSE
 
 
 class ExpertAuthentication(object):
-    """ExpertAuthentication"""
+    """ExpertAuthentication class.
+    """
 
     types = []
     """Type of Authentication:
     0 = None
     1 = EAP
     2 = LEAP
     3 = PEAP
@@ -170,20 +170,29 @@
             return
 
     def is_enabled(self):
         return bool(self.types)
 
 
 class ExpertChannel(object):
-    """ExpertChannel"""
-    
+    """ExpertChannel class.
+    """
+
     class ChannleFamily(object):
+        """ChannleFamily class.
+        """
+
         band = 0
+        """The channel band."""
+
         channel = 0
+        """The channel."""
+
         frequency = 0
+        """The channel frequency."""
 
         def __init__(self, band, channel, frequency):
             self.band = band
             self.channel = channel
             self.frequency = frequency
 
         def _get_props(self):
@@ -191,14 +200,16 @@
                 _json_enabled: True,
                 'band': self.band,
                 'channel': self.channel,
                 'frequency': self.frequency
             }
 
     band = ''
+    """The channel band."""
+
     families = []
     """List of ChannelFamily objects."""
 
     _json_label = 'channel'
     _json_band = 'channelBand'
     _json_family = 'channelFamily'
 
@@ -227,15 +238,16 @@
         props[ExpertChannel._json_label] = self._get_props()
 
     def is_enabled(self):
         return (self.band and self.families)
 
 
 class ExpertEncryption(object):
-    """ExpertEncryption"""
+    """ExpertEncryption
+    """
 
     protocols = []
     """list of Protocol Types:
     0 = None
     1 = WEP
     2 = CKIP
     3 = TKIP
@@ -245,15 +257,15 @@
     _json_label = 'essId'
 
     def __init__(self):
         self.items = ExpertEncryption.protocols
 
     def _get_props(self):
         props = {}
-        props[_json_accept] = len(self.protocols ) > 0
+        props[_json_accept] = len(self.protocols) > 0
         # if len(self.protocols) > 0:
         props[_json_items] = [{_json_enabled: True, _json_type: v} for v in self.protocols]
         # else:
         #     props[_json_items] = [{_json_enabled: False, _json_type: 0}]
         return props
 
     def _load(self, props):
@@ -261,36 +273,37 @@
             return
         for prop in props:
             pass
 
     def _store(self, props):
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             pass
 
     def is_enabled(self):
         return bool(self.protocols)
 
 
 class ExpertEss(object):
-    """Expert Ess Identifiers (names)"""
+    """Expert Ess Identifiers (names) class.
+    """
 
     names = []
     """List of Protocol names."""
 
     _json_label = 'essId'
     _json_value = 'value'
 
     def __init__(self):
         self.names = []
 
     def _get_props(self):
         props = {}
-        props[_json_accept] = len(self.names ) > 0
+        props[_json_accept] = len(self.names) > 0
         props[_json_items] = [{_json_enabled: True, ExpertEss._json_value: n} for n in self.names]
         return props
 
     def _load(self, props):
         if not isinstance(props, dict):
             return
         for prop in props:
@@ -302,20 +315,29 @@
         props[ExpertEss._json_label] = self._get_props()
 
     def is_enabled(self):
         return bool(self.names)
 
 
 class ExpertVendor(object):
-    """Expert Vendor Id"""
+    """Expert Vendor Id
+    """
 
     class Vendor(object):
+        """Vendor class.
+        """
+
         access_point = False
+        """Is this an this an access point."""
+
         client = False
+        """Does the vendor have a client."""
+
         value = ''
+        """The value of the Vendor."""
 
         _json_access_point = 'accessPoint'
         _json_client = 'client'
         _json_value = 'value'
 
         def __init__(self, access_point, client, value):
             self.access_point = access_point
@@ -325,15 +347,14 @@
         def _get_props(self):
             return {
                 ExpertVendor._json_accessPoint: self.access_point,
                 ExpertVendor._json_client: self.client,
                 ExpertVendor._json_value: self.value
             }
 
-
     vendors = []
     """List of Vendor objects."""
 
     _json_label = 'vendorId'
 
     def __init__(self):
         self.vendors = []
@@ -359,22 +380,24 @@
         return bool(self.vendors)
 
 
 class ExpertProblem(object):
     """Expert Problem"""
 
     group_id = 0
+    """The group identifier of the problem."""
 
     id = 0
     """ The Problem Identifier. Call
     <omniscript.omniscript.get_expert_problem_ids()>`
     to get the dictionary of Problem Label to id.
     """
 
     minimum_sample = 0
+    """The minimum number of samples needed to perform this Expert."""
 
     sensetivity = 0
     """One of the following levels:
     0 = None
     1 = Low
     2 = Medium
     3 = High
@@ -384,15 +407,15 @@
     """"The Problem's Severity, one of the following levels:
     0 = None
     1 = Informational
     2 = Minor
     3 = Major
     4 = Severe
     """
-    
+
     value = 0
     """The Problem's Value."""
 
     _json_label = 'problems'
 
     def __init__(self, props=None):
         self.group_id = ExpertProblem.group_id
@@ -413,15 +436,15 @@
         props['severity'] = self.severity
         props['value'] = self.value
         return props
 
     def _load(self, props):
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             if k == 'enabled':
                 self.enabled = v
             elif k == 'settingGroupId':
                 self.group_id = int(v)
             elif k == 'id':
                 self.id = int(v)
             elif k == 'minimumSample':
@@ -436,23 +459,37 @@
     def _store(self, props):
         if not isinstance(props, dict):
             return
         props[ExpertProblem._json_label] = self._get_props()
 
 
 class ExpertSettings(object):
-    """The Expert Settings (Preferences)"""
+    """The Expert Settings (Preferences).
+    """
 
     max_streams = 50000
+    """The maximum number of streams this Expert can track."""
+
     authentication = ExpertAuthentication()
+    """The authentication of this Expert."""
+
     channel = ExpertChannel()
+    """The channel for this Expert."""
+
     encryption = ExpertEncryption()
+    """The ecryption for this Expert."""
+
     ess = ExpertEss()
+    """The ESS of this Expert."""
+
     vendor = ExpertVendor()
+    """The Vendor of this object."""
+
     problems = []
+    """The list of Problems of this Expert."""
 
     # JSON Tags
     _json_label = 'expertPrefs'
     _json_max_streams = 'maxStreamCount'
     _json_policy = 'policy'
     _json_authentication = 'authentication'
     _json_channel = 'channel'
@@ -484,15 +521,15 @@
         problems = {}
         props[ExpertSettings._json_problems] = problems
         return props
 
     def _load(self, props):
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             pass
 
     def _store(self, props):
         if not isinstance(props, dict):
             return
         default = ExpertSettings()
         _current = self._get_props()
@@ -508,39 +545,40 @@
     def is_enabled(self):
         return (self.authentication.is_enabled() and self.channel.is_enabled()
                 and self.encryption.is_enabled() and self.ess.is_enabled()
                 and self.vendor.is_enabled() and bool(self.problems))
 
 
 class TimeRange(object):
-    """A range of time."""
+    """A range of time.
+    """
 
     start = None
     """The begining of the Time Range"""
 
     end = None
     """The ending of the Time Range"""
 
-    #Tags
+    # Tags
     _json_start = 'startTime'
     _json_end = 'endTime'
 
     def __init__(self, start=None, end=None, props=None):
         self.start = PeekTime(start) if start else TimeRange.start
         self.end = PeekTime(end) if end else TimeRange.end
         self._load(props)
 
     def _load(self, props):
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             if k == TimeRange._json_start:
-                start = PeekTime(v)
+                self.start = PeekTime(v)
             elif k == TimeRange._json_end:
-                end = PeekTime(v)
+                self.end = PeekTime(v)
 
     def _store(self):
         if not self.start and not self.end:
             return None
         props = {
             TimeRange._json_start: self.start.iso_time(),
             TimeRange._json_end: self.end.iso_time()
@@ -549,15 +587,15 @@
 
 
 class ForensicTemplate(object):
     """Forensic Template class.
     Use a Forensic Template object to create a
     :class:`ForensicSearch <omniscript.forensicsearch.ForensicSearch>`
     object with the function
-    :func:`create_forensic_search() 
+    :func:`create_forensic_search()
     <omniscript.omniengine.OmniEngine.create_forensic_search>`.
     """
 
     adapter_name = ''
     """The name of the search's adapter."""
 
     capture_name = ''
@@ -569,15 +607,15 @@
     capture_session_id = 0
     """The index of the Capture Session."""
 
     conversation_limits = None
     """The Conversation (Node/Protocol Detail) Limits a
     :class:`StatsLimit <omniscript.statslimit.StatsLimit>`
     object. Set the option_node_protocol_detail attribute to True to
-    enable Node/Protocol Details Stats. Either Node Stats or Protocol 
+    enable Node/Protocol Details Stats. Either Node Stats or Protocol
     Stats must also be enabled or Node/Protocol Detail Stats will be
     disabled.
     """
 
     end_time = None
     """The optional ending timestamp, as
     :class:`PeekTime <omniscript.peektime.PeekTime>`
@@ -593,23 +631,23 @@
     files = []
     """The options list of packet files to search.
     If this list is empty and capture_name is empty, then all packet files
     are search. Do not specifiy capture_name if files is not empty.
     """
 
     filter = None
-    """The 
+    """The
     :class:`Filter <omniscript.filter.Filter>`
     object of the search.
-    Use 
+    Use
     :func:`find_filter()
     <omniscript.omniengine.OmniEngine.create_forensic_search>`
     to get one of the engine's filters.
     """
-    
+
     filter_mode = MODE_ACCEPT_ALL
     """The filter mode:
            0 for MODE_ACCEPT_ALL,
            1 for MODE_ACCEPT_ANY_MATCHING,
            2 for MODE_REJECT_ALL,
            3 for MODE_REJECT_MATCHING,
            4 for MODE_ACCEPT_ALL_MATCHING,
@@ -618,16 +656,16 @@
 
     graph_interval = 0
     """The time interval for graphing when option[graphs] is enabled."""
 
     limit = LIMIT_TYPE_NONE
     """Limit the search by:
            0 for 'None' (default),
-           1 for 'Packets', 
-           2 for 'Bytes', 
+           1 for 'Packets',
+           2 for 'Bytes',
            3 for 'Buffer'.
     """
 
     limit_size = 0
     """The number of Packets, Bytes or Buffer size in bytes to limit the
     search to."""
 
@@ -644,21 +682,21 @@
     """The Node Limits a
     :class:`StatsLimit <omniscript.statslimit.StatsLimit>`
     object. Set the option_node attribute to True to enable Node Stats.
     """
 
     plugins = None
     """The list of Plugin (Analysis Module) Ids.
-    A Plugin Id may be a string, 
+    A Plugin Id may be a string,
     :class:`OmniId <omniscript.omniid.OmniId>`
     or an
     :class:`AnalysisModule <omniscript.analysismodule.AnalysisModule>`
     object.
-    Call the 
-    :func:`get_analysis_module_list() 
+    Call the
+    :func:`get_analysis_module_list()
     <omniscript.omniengine.OmniEngine.get_analysis_module_list>`
     method to get the engine's list of plugins.
     """
 
     plugins_config = None
     """The list of Plugins (Analysis Modules) configuration."""
 
@@ -919,15 +957,15 @@
 
     def __str__(self):
         return f'ForensicTemplate: {self.name}'
 
     def _load(self, props):
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             if k == '':
                 pass
 
     def _load_xml(self, props):
         if props is None:
             return
         for prop in props:
@@ -990,15 +1028,15 @@
                 self._option_web = False
             elif name == ForensicTemplate._tag_break_out:
                 self._option_break_out = _from_prop_boolean(prop.text)
         # Set the break out statistics.
         if self._option_break_out:
             for prop in props:
                 name = prop.tag
-                if break_out_stats.has_key(name):
+                if name in break_out_stats:
                     setattr(self, break_out_stats[name], _from_prop_boolean(prop.text))
             self.node_limits.enabled = self.option_node
             self.protocol_limits.enabled = self.option_protocol
             self.node_protocol_detail_limits.enabled = self.option_node_protocol_detail
         self._option_break_out = True
 
     def _load_plugins(self, pluginlist):
@@ -1012,28 +1050,28 @@
 
     def add_file(self, name):
         """Add a file to the search."""
         if isinstance(name, FileInformation):
             self.files.append(name.name)
         elif isinstance(name, PacketFileInformation):
             self.files.append(name.path)
-            if self.media_type == None:
+            if self.media_type is None:
                 self.media_type = name.media_type
                 self.media_sub_type = name.media_sub_type
         # elif isinstance(name, Forensic File <<< added space to hide from text search.):
         #     self.files.append(name.path)
         #     if self.media_type == None:
         #         self.media_type = name.media_type
         #         self.media_sub_type = name.media_sub_type
         else:
             self.files.append(name)
 
     def add_plugin(self, plugin):
         """Add a plugin id to the search.
-        A plugin id may be a string, 
+        A plugin id may be a string,
         :class:`OmniId <omniscript.omniid.OmniId>`
         or an
         :class:`AnalysisModule <omniscript.analysismodule.AnalysisModule>`
         object.
         """
         if isinstance(plugin, six.string_types):
             if OmniId.is_id(plugin):
@@ -1098,15 +1136,15 @@
         self.option_graphs = enable
         self.option_indexing = enable
         self.option_log = enable
         self.option_packets = enable
 
     def set_limit(self, limit, limit_size):
         """Set a limit on the search.
-        
+
         Args:
             limit (str): either 'none', 'packets', 'bytes' or 'buffer'.
             limit_size (int): packets are in 1k units, bytes and buffer
             in 1MB units.
         """
         self.limit = limit_types[limit]
         if self.limit == LIMIT_TYPE_BYTES or self.limit == LIMIT_TYPE_BUFFER:
@@ -1167,36 +1205,38 @@
             props[ForensicTemplate._json_limit_number] = self.limit_size
             props[ForensicTemplate._json_limit_type] = self.limit
         if self.option_log:
             props[ForensicTemplate._json_log] = self.option_log
 
         # the two required attributes:
         props[ForensicTemplate._json_media_type] = (self.media_type
-            if self.media_type is not None else ForensicTemplate.media_type)
+                                                    if self.media_type is not None
+                                                    else ForensicTemplate.media_type)
         props[ForensicTemplate._json_media_sub_type] = (self.media_sub_type
-            if self.media_sub_type is not None else ForensicTemplate.media_sub_type)
+                                                        if self.media_sub_type is not None
+                                                        else ForensicTemplate.media_sub_type)
 
         if self.name:
             props[ForensicTemplate._json_name] = self.name
         if self.option_network:
             props[ForensicTemplate._json_network] = self.option_network
         if isinstance(self.node_limits, StatsLimit) and self.node_limits.enabled:
             props[ForensicTemplate._json_node] = True
             self.node_limits._store(props)
         if self.option_packets:
             props[ForensicTemplate._json_packets] = self.option_packets
         if self.option_passive_name_resolution:
-            props[ForensicTemplate._json_passive_name_resolution] = \
-                self.option_passive_name_resolution
+            props[ForensicTemplate._json_passive_name_resolution] = (
+                self.option_passive_name_resolution)
 
         if self.plugins:
             pl = {
-            ForensicTemplate._json_classid: _get_clsid(ForensicTemplate._tag_plugins_clsid),
-            ForensicTemplate._json_plugins: False,
-            ForensicTemplate._json_plugins_list: []
+                ForensicTemplate._json_classid: _get_clsid(ForensicTemplate._tag_plugins_clsid),
+                ForensicTemplate._json_plugins: False,
+                ForensicTemplate._json_plugins_list: []
             }
             if self.plugins:
                 pl[ForensicTemplate._json_plugins] = True
                 for plugin in self.plugins:
                     if isinstance(plugin, AnalysisModule):
                         id = plugin.id
                     elif isinstance(plugin, OmniId):
@@ -1246,40 +1286,42 @@
         compass_id = omniscript.get_class_name_ids()[_tag_compass]
         if self.option_compass:
             self.option_plugins = True
             if compass_id not in self.plugins:
                 self.plugins.append(compass_id)
 
         # Sync the stats limits with the options.
-        self.option_node_protocol_detail = self.option_node_protocol_detail and \
-                                          (self.option_node or self.option_protocol)
+        self.option_node_protocol_detail = (self.option_node_protocol_detail
+                                            and (self.option_node or self.option_protocol))
         self.node_limits.enabled = self.option_node
         self.node_protocol_detail_limits.enabled = self.option_node_protocol_detail
         self.protocol_limits.enabled = self.option_protocol
 
         search = ET.Element(ForensicTemplate._tag_root_name)
         if self.files and len(self.files) > 0:
             for f in self.files:
                 ET.SubElement(search, ForensicTemplate._tag_single_file).text = f
         ET.SubElement(search, ForensicTemplate._tag_name).text = self.name
-        ET.SubElement(search, ForensicTemplate._tag_session_id).text = str(self.session_id if self.session_id else -1)
+        ET.SubElement(search, ForensicTemplate._tag_session_id).text = (str(self.session_id
+                                                                            if self.session_id
+                                                                            else -1))
         ET.SubElement(search, ForensicTemplate._tag_media_type).text = str(self.media_type)
         ET.SubElement(search, ForensicTemplate._tag_media_sub_type).text = str(self.media_sub_type)
         if self.adapter_name:
             ET.SubElement(search, ForensicTemplate._tag_adapter_name).text = self.adapter_name
         else:
             ET.SubElement(search, ForensicTemplate._tag_adapter_name)
         if self.start_time and self.end_time:
             ET.SubElement(search, ForensicTemplate._tag_start_time).text = str(self.start_time)
             ET.SubElement(search, ForensicTemplate._tag_end_time).text = str(self.end_time)
         ET.SubElement(search, ForensicTemplate._tag_filter_mode).text = str(self.filter_mode)
         if self.filter is not None:
             _filter = ET.SubElement(search, ForensicTemplate._tag_filter)
             self.filter._store(_filter)
-        
+
         # options
         for a, p in stats_labels.iteritems():
             ET.SubElement(search, p).text = str(int(getattr(self, a)))
 
         # break_out indicates new options format.
         if self._option_break_out:
             for a, p in break_out_stats_labels.iteritems():
@@ -1295,15 +1337,15 @@
         ET.SubElement(search, ForensicTemplate._tag_graph_interval).text = str(self.graph_interval)
 
         if self.option_voice and self.voip:
             self.voip._store_raw(search)
 
         plugins_id = omniscript.get_class_name_ids()[ForensicTemplate._tag_plugins_clsid]
         plugins = ET.SubElement(search, ForensicTemplate._tag_plugins_list,
-                               {'clsid': str(plugins_id)})
+                                {'clsid': str(plugins_id)})
         props = ET.SubElement(plugins, ForensicTemplate._tag_properties)
         if self.option_plugins and (self.option_all_plugins or self.plugins):
             module_list = engine.get_analysis_module_list() if engine else []
             _set_clsid(plugins, ForensicTemplate._tag_property_list)
             if self.option_all_plugins:
                 for module in module_list:
                     if module.id == compass_id:
@@ -1314,16 +1356,16 @@
             else:
                 for plugin in self.plugins:
                     id = None
                     if isinstance(plugin, six.string_types):
                         if OmniId.is_id(plugin):
                             id = OmniId(plugin)
                         else:
-                            module = next((i for i in module_list 
-                                                if getattr(i, 'name') == plugin), None)
+                            module = next((i for i in module_list
+                                           if getattr(i, 'name') == plugin), None)
                             if module:
                                 id = module.id
                     elif isinstance(plugin, OmniId):
                         id = plugin
                     elif isinstance(plugin, AnalysisModule):
                         id = plugin.id
                     if id:
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/graphtemplate.py` & `omniscript-liveaction-3.0.49/src/omniscript/graphtemplate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 ﻿"""GraphTemplate class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
-
-import xml.etree.ElementTree as ET
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 from .omniid import OmniId
 from .peektime import PeekTime
 
-
 find_attribs = ['name', 'id']
 
 
 class GraphItem(object):
     """The GraphItem class.
     A GraphTemplate contains a list of GraphItems.
     """
@@ -44,15 +41,15 @@
         self.name = GraphItem.name
         self.description = GraphItem.description
         self._load(criteria)
 
     def _load(self, props):
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             if k == 'id':
                 self.id = OmniId(v)
             elif k == 'name':
                 self.name = v
             elif k == 'description':
                 self.description = v
             elif k == 'unitType':
@@ -63,16 +60,16 @@
                 self.type = int(v)
             elif k == 'statisticFlags':
                 self.flags = int(v)
 
 
 class GraphTemplate(object):
     """The GraphTemplate class has the attributes of an Graph Template.
-    The 
-    :func:`get_graph_template_list() 
+    The
+    :func:`get_graph_template_list()
     <omniscript.omniengine.OmniEngine.get_graph_template_list>`
     function returns a list of GraphTemplate objects.
     """
 
     id = OmniId()
     """The graph template's identifier."""
 
@@ -93,14 +90,16 @@
 
     sample_count = 0
     """The sample count"""
 
     graph_item_list = []
     """The list of graph items"""
 
+    find_attributes = ('name', 'id')
+
     def __init__(self, criteria):
         self.id = OmniId(True) if criteria is None else GraphTemplate.id
         self.name = GraphTemplate.name
         self.description = GraphTemplate.description
         self.graph_id = OmniId(True) if criteria is None else GraphTemplate.graph_id
         self.start = GraphTemplate.start
         self.sample_interval = GraphTemplate.sample_interval
@@ -110,23 +109,23 @@
 
     def __str__(self):
         return f'GraphTemplate: {self.name}'
 
     def _load(self, props):
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             if k == 'templateId':
                 self.id = OmniId(v)
             elif k == 'title':
                 self.name = v
             elif k == 'description':
                 self.description = v
             elif k == 'id':
-                self.graph_id =  OmniId(v)
+                self.graph_id = OmniId(v)
             elif k == 'startTime':
                 self.start = PeekTime(v)
             elif k == 'sampleInterval':
                 self.sample_interval = int(v)
             elif k == 'sampleCount':
                 self.sample_count = int(v)
             elif k == 'graphItems':
@@ -143,17 +142,17 @@
     graphs = props.get('graphs')
     for template in graphs:
         lst.append(GraphTemplate(criteria=template))
     lst.sort(key=lambda x: x.name)
     return lst
 
 
-def find_graph_template(graphs, value, attrib=find_attribs[0]):
+def find_graph_template(graphs, value, attrib=GraphTemplate.find_attributes[0]):
     """Finds a graph_template in the list"""
-    if (not graphs) or (attrib not in find_attribs):
+    if (not graphs) or (attrib not in GraphTemplate.find_attributes):
         return []
 
     if len(graphs) == 0:
         return []
 
     if isinstance(value, GraphTemplate):
         _value = value.id
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/mediainformation.py` & `omniscript-liveaction-3.0.49/src/omniscript/mediainformation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """MediaInformation class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
-
-from .invariant import MEDIA_DOMAIN_NONE, MEDIA_TYPE_802_3, \
-    MEDIA_SUB_TYPE_NATIVE, MEDIA_SUB_TYPE_NATIVE
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 from .omniid import OmniId
 
+from .invariant import MEDIA_DOMAIN_NONE, MEDIA_TYPE_802_3, MEDIA_SUB_TYPE_NATIVE
 
 _mediainfo_prop_dict = {
-    'clsid' : 'class_id',
-    'linkSpeed' : 'link_speed',
-    'mediaDomain' : 'domain',
-    'mediaSubType' : 'media_sub_type',
-    'mediaType' : 'media_type'
+    'clsid': 'class_id',
+    'linkSpeed': 'link_speed',
+    'mediaDomain': 'domain',
+    'mediaSubType': 'media_sub_type',
+    'mediaType': 'media_type'
 }
 
 
 class MediaInformation(object):
     """The Media Information class.
     """
 
@@ -48,15 +46,15 @@
         self.load(props)
 
     def __str__(self):
         return f'MediaInformation: {self.media_type}'
 
     def load(self, props):
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 a = _mediainfo_prop_dict.get(k)
                 if a is not None:
                     if hasattr(self, a):
                         if isinstance(getattr(self, a), int):
                             setattr(self, a, int(v) if v else 0)
                         elif getattr(self, a) is None:
                             if (a == 'class_id'):
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/omniaddress.py` & `omniscript-liveaction-3.0.49/src/omniscript/omniaddress.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 ﻿"""OmniAddress classes.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 import re
 import six
 
 import xml.etree.ElementTree as ET
 
-from .invariant import (ADDRESS_TYPE_UNDEFINED, ADDRESS_TYPE_ETHERNET, ADDRESS_TYPE_IP,
-    ADDRESS_TYPE_IPV6, ADDRESS_TYPE_WIRELESS, ADDRESS_TYPE_OTHER)
+from .invariant import AddressType
 
 
 def _clean_split(value):
     clean = value.replace('\t', ' ')
     clean = clean.replace('\r', ' ')
     clean = clean.replace('\n', ' ')
     clean = clean.replace(',', ' ')
@@ -73,15 +72,15 @@
         if best_doublecolon_start == 0:
             hextets = [''] + hextets
     return ":".join(hextets)
 
 
 def format_ethernet(mac):
     """Format an Ethernet Address.
-    
+
     Args:
         mac (str, int): address to format as '0123456789AB' or
         as an integer value.
 
     Returns:
         String as '01:23:45:67:89:AB'
     """
@@ -89,15 +88,15 @@
         data = f'{mac:012X}' if isinstance(mac, int) else mac
         return ':'.join([data[i:i+2] for i in range(0, 12, 2)])
     return ''
 
 
 def format_ipv4(ip, mask=0xF0000000):
     """Format an IPv4 Address.
-    
+
     Args:
         ip (str, int): address to format as '12345678' or
         as an integer value.
 
     Returns:
         String as '18.52.86.120' or '12.34.56.0/24'
     """
@@ -115,23 +114,23 @@
             elif mask == 0x00000000:
                 text += '/0'  # 0 * 8 bits
     return text
 
 
 def format_ipv6(ip, compress=True):
     """Format an IPv6 Address.
-    
+
     Args:
         ip (str, list): address to format as string
             '0123456789ABCDEFFEDCBA9876543210'
             or list (0123, 4567, 89AB, CDEF, FEDC, BA98, 7654, 3210)
             or as an integer value.
-        
+
         compress (bool): remove the fist ':0000' strings.
-    
+
     Returns:
         String as '0123:4567:89AB:CDEF:FEDC:BA98:7654:3210'
     """
     if ip:
         if isinstance(ip, int):
             data = f'{ip:032X}'
             hextets = list(([data[i:i+4] for i in range(0, 32, 4)]))
@@ -143,17 +142,18 @@
             else:
                 hextets = ip
         if compress:
             return _compress_hextets(hextets)
         return ':'.join(hextets)
     return ''
 
+
 def parse_ethernet(address):
     """Parse an Ethernet Address.
-    
+
     Args:
         address (str, int): address to parse as '12:34:56:78:9A:BC' or
         as an integer value. The string may contain
         trailing wildcards '*'.
 
     Returns:
         (Address as String '123456789ABC', Mask as Integer 0xFC000000)
@@ -181,33 +181,33 @@
             addr = address
             mask = None
     return (addr, mask)
 
 
 def parse_ethernet_list(addresses, mask):
     """Parse a list of Ethernet Addresses.
-    
+
     Args:
         addresses (str): list of addresses seperated by '\\r\\n' or
         '\\n'.
 
     Returns:
         List of EthernetAddress objects.
     """
     _addresses = addresses
     if '\\r' in addresses:
-        _address = addresses.replace('\\r', '')
+        _addresses = addresses.replace('\\r', '')
     _addresses = _addresses.strip('\\n')
     lst = [EthernetAddress(a, mask=mask) for a in _addresses.split('\\n') if a]
     return lst
 
 
 def parse_ipv4(address):
     """Parse an IPv4 Address.
-    
+
     Args:
         address (str, int): address to parse as '18.52.86.120' or
         as an integer value. Optional wild cards: '10.*.*.*' or
         '10.0.0.0/8'
 
     Returns:
         (Addres as String '12345678', Mask as Integer 0xFF000000)
@@ -238,15 +238,15 @@
     elif isinstance(address, int):
         addr = f'{address:08X}'
     return (addr, mask)
 
 
 def parse_ipv4_list(addresses, mask):
     """Parse a list of IPv4 Addresses.
-    
+
     Args:
         addresses (str): list of addresses seperated by '\\r\\n' or
         '\\n'.
 
     Returns:
         List of IPv4Address objects.
     """
@@ -256,18 +256,18 @@
     _addresses = _addresses.strip('\\n')
     lst = [IPv4Address(a, mask=mask) for a in _addresses.split('\\n') if a]
     return lst
 
 
 def parse_ipv6(address):
     """Parse an IPv6 Address.
-    
+
     Args:
         address (str, int): address to parse as
-        '0123:4567:89AB:CDEF:FEDC:BA98:7654:3210' or 
+        '0123:4567:89AB:CDEF:FEDC:BA98:7654:3210' or
         as an integer value.
 
     Returns:
         String as '0123456789ABCDEFFEDCBA9876543210'
     """
     if isinstance(address, int):
         data = f'{address:32X}'
@@ -284,15 +284,15 @@
             else:
                 data += h.zfill(4)
     return data
 
 
 def parse_ipv6_list(addresses, mask):
     """Parse a list of IPv6 Addresses.
-    
+
     Args:
         address (str): list of addresses seperated by '\\r\\n' or
         '\\n'.
 
     Returns:
         List of IPv6Addres objects.
     """
@@ -322,112 +322,118 @@
         self.series = series
 
     def format(self, compressed=True):
         return str(self)
 
 
 class UndefinedAddress(BaseAddress):
+    """The UndefinedAddress is for unknow address formats.
+    """
+
     def __init__(self):
         BaseAddress.__init__(self, False, None)
 
     @property
     def address_type(self):
-        return ADDRESS_TYPE_UNDEFINED
+        return AddressType.NONE
 
     @property
     def _data(self):
         return None
 
 
 class EthernetAddress(BaseAddress):
-    """An Ethernet address."""
+    """An Ethernet address (aka. MAC address.).
+    """
 
     address = None
     """An ethernet address string.
     Format is '1234567890AB'
     """
 
     def __init__(self, address=None, series=False, mask=None, data=None):
         BaseAddress.__init__(self, series, mask)
         if address:
             self.address, self.mask = parse_ethernet(address)
         elif data is not None:
             self.address = data
-##        self.addresses = []
-##        self.addresses = _clean_split(data)
-##        for address in addresses:
-##            if address.find(':') > 0:
-##                self.addresses.append(address)
-##            else:
-##                addr = format_ethernet(address)
-##                if mask is not None:
-##                    cidr = int(mask)
-##                    if cidr != 0:
-##                        addr + r'/' + str(_high_bits_set(cidr))
-##                self.addresses.append(addr)
+#        self.addresses = []
+#        self.addresses = _clean_split(data)
+#        for address in addresses:
+#            if address.find(':') > 0:
+#                self.addresses.append(address)
+#            else:
+#                addr = format_ethernet(address)
+#                if mask is not None:
+#                    cidr = int(mask)
+#                    if cidr != 0:
+#                        addr + r'/' + str(_high_bits_set(cidr))
+#                self.addresses.append(addr)
 
     def __repr__(self) -> str:
         return f'EthernetAddress: {format_ethernet(self.address)}'
 
     def __str__(self) -> str:
         return format_ethernet(self.address)
 
     @property
     def _data(self):
         return self.address
 
     @property
     def address_type(self):
-        return ADDRESS_TYPE_ETHERNET
+        return AddressType.ETHERNET
 
 
 class IPv4Address(BaseAddress):
-    """An IP version 4 address."""
+    """An IP version 4 address.
+    """
 
     address = None
     """The IPv4 address strings.
     Format: 01020304, 12345600/24, 2468AC80/25
     """
 
     def __init__(self, address=None, series=False, mask=None, data=None):
         BaseAddress.__init__(self, series, mask)
         if address:
             (self.address, self.mask) = parse_ipv4(address)
         elif data is not None:
             self.address = data
-##        self.addresses = []
-##        self.addresses = _clean_split(data)
-##        for address in addresses:
-##            if address.find('.') > 0:
-##                self.addresses.append(address)
-##            else:
-##                addr = format_ipv4(address)
-##                if mask is not None:
-##                    cidr = int(mask)
-##                    if cidr != 0:
-##                        addr + r'/' + str(cidr)
-##                self.addresses.append(addr)
+#        self.addresses = []
+#        self.addresses = _clean_split(data)
+#        for address in addresses:
+#            if address.find('.') > 0:
+#                self.addresses.append(address)
+#            else:
+#                addr = format_ipv4(address)
+#                if mask is not None:
+#                    cidr = int(mask)
+#                    if cidr != 0:
+#                        addr + r'/' + str(cidr)
+#                self.addresses.append(addr)
 
     def __repr__(self) -> str:
         return f'IPv4Address: {format_ipv4(self.address, self.mask)}'
 
     def __str__(self) -> str:
         return format_ipv4(self.address, self.mask)
 
     @property
     def _data(self):
         return self.address
 
     @property
     def address_type(self):
-        return ADDRESS_TYPE_IP
+        return AddressType.IPV4
 
 
 class IPv6Address(BaseAddress):
-    """An IP version 6 address."""
+    """An IP version 6 address.
+    """
 
     address = None
     """An IPv6 address string.
     Format: '123456789ABCDEF0FEDCBA9876543210'
     """
 
     compressed = True
@@ -440,47 +446,48 @@
     def __init__(self, address=None, series=False, mask=None, data=None):
         BaseAddress.__init__(self, series, mask)
         self.compressed = IPv6Address.compressed
         if address:
             self.address = parse_ipv6(address)
         elif data is not None:
             self.address = data
-##        self.addresses = []
-##        addresses = _clean_split(data)
-##        for address in addresses:
-##            if address.find(':') > 0:
-##                self.addresses.append(address)
-##            else:
-##                addr = format_ipv6(address)
-##                if mask is not None:
-##                    cidr = int(mask)
-##                    if cidr != 0:
-##                        addr + r'/' + str(cidr)
-##                self.addresses.append(addr)
+#        self.addresses = []
+#        addresses = _clean_split(data)
+#        for address in addresses:
+#            if address.find(':') > 0:
+#                self.addresses.append(address)
+#            else:
+#                addr = format_ipv6(address)
+#                if mask is not None:
+#                    cidr = int(mask)
+#                    if cidr != 0:
+#                        addr + r'/' + str(cidr)
+#                self.addresses.append(addr)
 
     def __repr__(self):
         return f'IPv6: {format_ipv6(self.address, self.compressed)}'
 
     def __str__(self):
         return format_ipv6(self.address, self.compressed)
 
     @property
     def _data(self):
         return self.address
 
     @property
     def address_type(self):
-        return ADDRESS_TYPE_IPV6
+        return AddressType.IPV6
 
     def format(self, compressed=True):
         return format_ipv6(self.address, compressed)
 
 
 class OtherAddress(BaseAddress):
-    """All Other address types."""
+    """All Other address types.
+    """
 
     address = None
     """The address string.
     Format is '1234', ASCII-Hex string.
     """
 
     def __init__(self, data, mask):
@@ -495,19 +502,20 @@
 
     @property
     def _data(self):
         return self.address
 
     @property
     def address_type(self):
-        return ADDRESS_TYPE_OTHER
+        return AddressType.OTHER
 
 
 class OmniAddress(object):
-    """The OmniAddress class holds various types of network addresses."""
+    """The OmniAddress class holds various types of network addresses.
+    """
 
     name = None
 
     address_list = None
     """A list of one of the BaseAddress class of address."""
 
     def __init__(self, name, address, address_type=None, mask=None):
@@ -542,72 +550,85 @@
         """The type of the address. (Read Only)"""
         return self.address.address_type
 
     def _load(self, address, address_type=None, mask=None):
         if isinstance(address, BaseAddress):
             self.address_list = [address]
         if isinstance(address, six.string_types):
-            series = False
-            if address_type == ADDRESS_TYPE_ETHERNET:
+            # TODO: investigate if series is needed.
+            # series = False
+            if address_type == AddressType.ETHERNET:
                 self.address_list = parse_ethernet_list(address, mask)
-            elif address_type == ADDRESS_TYPE_IP:
+            elif address_type == AddressType.IPV4:
                 self.address_list = parse_ipv4_list(address, mask)
-            elif address_type == ADDRESS_TYPE_IPV6:
+            elif address_type == AddressType.IPV6:
                 self.address_list = parse_ipv6_list(address, mask)
-            elif address_type == ADDRESS_TYPE_WIRELESS:
+            elif address_type == AddressType.WIRELESS:
                 self.address_list = parse_ethernet_list(address, mask)
             else:
                 self.address_list = [OtherAddress(address, mask)]
 
     def _load_xml(self, node):
         self.name = node.tag
         series = (self.name[0].lower() == 's')
         address_type = int(node.get('type', '0'))
         mask = node.get('mask')
         if mask:
             mask = int(mask)
         data = node.get('data')
-        if address_type == ADDRESS_TYPE_ETHERNET:
+        if address_type == AddressType.ETHERNET:
             self.address_list = EthernetAddress(None, series, mask, data)
-        elif address_type == ADDRESS_TYPE_IP:
+        elif address_type == AddressType.IPV4:
             self.address_list = IPv4Address(None, series, mask, data)
-        elif address_type == ADDRESS_TYPE_IPV6:
+        elif address_type == AddressType.IPV6:
             self.address_list = IPv6Address(None, series, mask, data)
-        elif address_type == ADDRESS_TYPE_WIRELESS:
+        elif address_type == AddressType.WIRELESS:
             self.address_list = EthernetAddress(None, series, mask, data)
         else:
             self.address_list = OtherAddress(data, mask)
 
     def _store_xml(self, node):
         elem = ET.SubElement(node, self.name,
-                             {'class':'2',
-                              'type':str(self.address.address_type),
-                              'data':self.address._data})
+                             {'class': '2',
+                              'type': str(self.address.address_type),
+                              'data': self.address._data})
         if self.mask is not None:
             elem.set('mask', str(self.mask))
 
     # def parse(self, address):
     #     if address.find('.'):
     #         offset = address.find('/')
     #         series = offset != -1
     #         if series:
     #             mask = int(address[offset+1:])
     #             data = address[:offset]
     #         else:
     #             mask = 0
     #             data = address
     #         self.address = IPv4Address(series, mask, data)
-            
+
+
+def is_valid_hostname(hostname: str) -> bool:
+    # from: stackoverflow.com/questions/2532053/validate-a-hostname-string
+    # replaced double-quotes with single-quotes. Flake8 compliance.
+    # replaced '\d' with '[0-9].
+    if len(hostname) > 255:
+        return False
+    if hostname[-1] == '.':
+        hostname = hostname[:-1]  # strip exactly one dot from the right, if present
+    allowed = re.compile('(?!-)[A-Z0-9-]{1,63}(?<!-)$', re.IGNORECASE)
+    return all(allowed.match(x) for x in hostname.split('.'))
+
 
 def parse_ip_address(address):
     """Parse IP Address.
-    
+
     Args:
-        address (str, int): address to parse as an integer or a string: 
-        '18.52.86.120' or '1234::5678:90ab' or '15 1234::5678:90ab' 
+        address (str, int): address to parse as an integer or a string:
+        '18.52.86.120' or '1234::5678:90ab' or '15 1234::5678:90ab'
         (IPv6 address return by an Expert Query).
 
     Returns:
         An OmniAddress object:
         :class:`IPv4Address <omniscript.omniaddress.IPv4Address>` or
         :class:`IPv6Address <omniscript.omniaddress.IPv6Address>` or
         None.
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/omnidatatable.py` & `omniscript-liveaction-3.0.49/src/omniscript/omnidatatable.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 ﻿"""OmniDataTable class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 from .omnierror import OmniError
 from .readstream import ReadStream
 
+
 class OmniDataTable(object):
     """Parses a serialized IDataTable object into itself.
     This class is used by other OmniScript classes to parse binary data
     returned by an OmniEngine.
     """
 
     labels = []
@@ -30,21 +31,21 @@
         self.rows = []
 
     def load(self, data):
         """Load the Data Table from a string buffer containing a serialized
         IDataTable object.
         """
         stream = ReadStream(data)
-        #print len(data)
+        # print len(data)
         if len(data) < 8:
             return
         # TODO: use a readstream.
         major_ver = stream.read_uint()
         stream.read_uint()      # minor_ver
-        #Expecting Version 3.0
+        # Expecting Version 3.0
         if major_ver != 3:
             raise OmniError('Unsupported Data Table version.')
         column_count = stream.read_uint()
         row_count = stream.read_uint()
         for _ in range(column_count):
             _type = stream.read_ushort()
             self.types.append(_type)
@@ -65,14 +66,14 @@
                 elif _type == 22:
                     row.append(stream.read_uint())
                 elif _type == 23:
                     row.append(stream.read_uint())
                 elif _type == 0:
                     row.append(None)
                 else:
-                    #print 'Row:', r, 'Column', c, 'Unknown Type:', type
-                    #raise TypeError('Invalid type in data.')
+                    # print 'Row:', r, 'Column', c, 'Unknown Type:', type
+                    # raise TypeError('Invalid type in data.')
                     pass
             self.rows.append(row)
 
     def __str__(self):
         return 'OmniDataTable'
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/omniengine.py` & `omniscript-liveaction-3.0.49/src/omniscript/omniengine.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,96 @@
 ﻿"""OmniEngine class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 import os
-import fileinput
 import json
-import logging
-import re
 import requests
 import six
 import time
-import xml.etree.ElementTree as ET
 
-from contextlib import closing
-from pathlib import PurePath
+from pathlib import PurePath, PurePosixPath
+from typing import List, Optional, Union
 
 import omniscript
 
-from .invariant import (BYTES_PER_MEGABYTE, BYTES_PER_GIGABYTE, DEFAULT_PORT,
-    ID_FLAG_BRACES, OMNI_FLAG_NO_HTTPS_WARNINGS, OMNI_GET_LOG_MSGS)
-
+from .alarm import Alarm
+from .adapter import Adapter
+from .analysismodule import AnalysisModule
+from .auditlog import AuditLog
+from .authenticationtoken import AuthenticationToken
+from .capabilities import Capabilities
 from .capture import Capture
 from .capturesession import CaptureSession
 from .capturetemplate import CaptureTemplate
+from .decryptionkey import DecryptionKey
+from .decryptionkeytemplate import DecryptionKeyTemplate
 from .directory import Directory
 from .enginestatus import EngineStatus
+from .enginesettings import EngineSettings, SetSettingsResponse
+from .expertpreferences import ExpertPreferences
 from .eventlog import EventLog, EventLogEntry
 from .fileinformation import FileInformation
 from .filter import Filter
-from .filternode import FilterNode
-from .forensicsearch import ForensicSearch, find_forensic_search
+from .forensicsearch import ForensicSearch
 from .forensictemplate import ForensicTemplate
-from .graphtemplate import GraphTemplate
+from .helpers import OmniScriptEncoder
 from .invariant import (DatabaseOperation, Diagnostics, EngineOperation as EO,
-    EngineDataFormat as DF)
-from .omniaddress import OmniAddress, IPv4Address, IPv6Address
+                        EngineDataFormat as DF, TraceLogLevel)
+from .license import License, LicenseSettings
+from .liveflow import (LiveFlow, LiveFlowConfiguration, LiveFlowConfigurationResponse,
+                       LiveFlowContext, LiveFlowStatus)
+from .nametable import NameTable
+from .notifications import Notifications, NotificationActions, SendEmailResponse
 from .omnierror import OmniError
 from .omniid import OmniId
-from .omniport import OmniPort
 from .peektime import PeekTime
 from .performancelogger import PerformanceLogger
+from .protocol import Protocol
+from .protocoltranslation import ProtocolTranslation as PT
+from .remoteengine import RemoteEngine
+from .selection import Selection
+from .user import User
 
-from .adapter import _create_adapter_list, find_adapter, adapter_find_attributes
+from .adapter import _create_adapter_list, find_adapter
 from .adapterinformation import _create_adapter_information_list
 from .alarm import _create_alarm_list
 from .analysismodule import _create_analysis_module_list
 from .application import _create_application_list
 from .authenticationtoken import _create_authentication_token_list
 from .capture import _create_capture_list, find_capture
 from .capturesession import _create_capture_session_list
-from .capturetemplate import _create_capture_template_list, find_capture_template
+from .capturetemplate import _create_capture_template_list
 from .country import _create_country_list
+from .decryptionkey import _create_decryption_key_list, find_decryption_key
 # from .directory import _create_file_system
 # from .fileinformation import _create_file_information_list
 from .filter import _create_filter_list, find_filter
-from .forensicsearch import _create_forensic_search_list
-from .graphtemplate import _create_graph_template_list, find_graph_template
+from .forensicsearch import _create_forensic_search_list, find_forensic_search
+from .graphtemplate import _create_graph_template_list
+from .helpers import is_almost_success, is_success
+from .invariant import DEFAULT_CONNECTION_TIMEOUT, DEFAULT_PORT, DEFAULT_REQUEST_TIMEOUT
 from .packetfileinformation import PacketFileInformation, _create_packet_file_information_list
-
+from .protocol import _create_protocol_list
+from .protocoltranslation import _create_protocol_translations_list
 
 ENGINECONFIG = '/etc/omni/engineconfig.xml'
 OMNI_CONF = '/etc/omni/omni.conf'
 CTD_RATIO = 75
 
 find_attributes = ('name', 'id')
 
 _tag_results = 'results'
 
 jtrue = 'true'
 jfalse = 'false'
 
+
 def jbool(b):
     """Returns 'true' if 'b' is True else 'false'.
     """
     return jtrue if b else jfalse
 
 
 def _capture_id_list(captures):
@@ -104,44 +119,110 @@
     lst = []
     for s in session_list:
         if isinstance(s, (int, six.string_types)):
             lst.append(int(s))
         elif isinstance(s, CaptureSession):
             lst.append(s.session_id)
         else:
-            raise TypeError('session must be or contain an integer session id.')
+            raise TypeError(
+                'session must be or contain an integer session id.')
+    return lst
+
+
+def _capture_decryption_key_list(keys):
+    """Returns a list of session ids.
+    """
+    key_list = keys if isinstance(keys, list) else [keys]
+    lst = []
+    for s in key_list:
+        if isinstance(s, (int, six.string_types)):
+            lst.append(OmniId(s))
+        elif isinstance(s, DecryptionKey):
+            lst.append(s.id)
+        elif isinstance(s, DecryptionKeyTemplate):
+            lst.append(s.id)
+        else:
+            raise TypeError(
+                'decryption key must be or contain an integer decryption key id.')
     return lst
 
 
 def _capture_template_list(template):
     """Returns a list of template ids.
     """
     template_list = template if isinstance(template, list) else [template]
     lst = []
     for t in template_list:
         if isinstance(t, (int, six.string_types)):
             lst.append(OmniId(t))
         elif isinstance(t, CaptureTemplate):
             lst.append(t.id)
         else:
-            raise TypeError('template must be or contain an integer template id.')
+            raise TypeError(
+                'template must be or contain an integer template id.')
     return lst
 
 
-def _success(props):
-    return isinstance(props, dict) and (_tag_results in props) and \
-        isinstance(props[_tag_results], list) and \
-        (len(props[_tag_results]) > 0) and (props[_tag_results][0] == 0)
+class EngineTimeouts(object):
+    """The Timeouts for an OmniEngine."""
 
+    connection = DEFAULT_CONNECTION_TIMEOUT
+    """The HTTP Connection timeout value in seconds.
+    The numeric value may be an integer or float."""
+
+    request = DEFAULT_REQUEST_TIMEOUT
+    """The HTTP Request timeout value in seconds.
+    The numeric value may be an integer or float."""
+
+    def __init__(self, value: Optional[Union['EngineTimeouts', str, list]] = None,
+                 request: Optional[Union[int, float, str]] = None):
+        self.connection = EngineTimeouts.connection
+        self.request = EngineTimeouts.request
+        self._load(value, request)
+
+    def __str__(self):
+        return f'Connection: {self.connection}, Request: {self.request}'
+
+    def _load(self, args: Union['EngineTimeouts', str, list],
+              request: Optional[Union[int, float, str]]):
+        if args is None:
+            return
+        if isinstance(args, EngineTimeouts):
+            self.set_connection(args.connection)
+            self.set_request(args.request)
+        elif isinstance(args, six.string_types):
+            if args.lower() == 'off' or args.lower() == 'none':
+                self.connection = None
+                self.request = None
+            else:
+                c, r = args.split()
+                self.set_connection(c)
+                self.set_request(r)
+        elif isinstance(args, list):
+            if len(args) >= 2:
+                self.set_connection(args[0])
+                self.set_request(args[1])
+        elif isinstance(args, (int, float, str)) and isinstance(request, (int, float, str)):
+            self.set_connection(args)
+            self.set_request(request)
 
-def _almost_success(props):
-    # Start Capture sometimes returns: {'returns': []}
-    if isinstance(props, dict) and (_tag_results in props):
-        return isinstance(props[_tag_results], list)
-    return False
+    def as_tuple(self):
+        if self.connection is None and self.request is None:
+            return None
+        return (self.connection, self.request)
+
+    def set_connection(self, value: Union[int, float, str]):
+        connection = float(value.strip(', /(/)')) if isinstance(value, six.string_types) else value
+        if connection is not None and connection >= 0.0:
+            self.connection = float(connection)
+
+    def set_request(self, value: Union[int, float, str]):
+        request = float(value.strip(', /(/)')) if isinstance(value, six.string_types) else value
+        if request is not None and request >= 0.0:
+            self.request = float(request)
 
 
 class OmniEngine(object):
     """The OmniEngine class provides access to an OmniEngie.
     The function
     :func:`create_engine() <omniscript.omniscript.OmniScript.create_engine>`
     returns an OmniEngine object.
@@ -155,60 +236,51 @@
 
     host = ''
     """The address of the host system."""
 
     port = DEFAULT_PORT
     """The port, https (443)."""
 
-    timeout = 600000
+    timeout = EngineTimeouts()
     """The default timeout, in milliseconds, for issuing commands.
     The default is 10 minutes.
     """
 
     _omni = None
     """The parent OmniScript object of self."""
 
     _base_url = ''
     """The base URL for the REST API."""
 
+    _base_dms_url = ''
+    """The base URL for the REST API."""
+
     _session = None
     """The HTTP Session for the REST API."""
 
     _connected = False
     """Is the client connected and logged in?"""
 
-    _filter_list = None
-    """Cached Filter List: (
-    :class:`Filter <omniscript.filter.Filter>`,
-    :class:`PeekTime <omniscript.peektime.PeekTime>`).
-    """
-
-    _filter_timeout = 120 * 1000000000
-    """The timeout, in nanoseconds, for refreshing the Filter List.
-    Default 2 minutes.
-    """
-
     _last_status = None
     """The last EngineStatus object. Cached for performance."""
 
     _file_system = None
     """The file system of the host system. A tree of Directory object"""
 
     _perf_logger = None
     """The engine's Performance Log file."""
 
-    def __init__(self, omni, host, port=DEFAULT_PORT, secure=True):
+    def __init__(self, omni, host: str = 'localhost', port: int = DEFAULT_PORT,
+                 secure: bool = True, timeouts: Optional[Union[EngineTimeouts, str, list]] = None):
         self._omni = omni
         self.logger = omni.logger
         self.host = host if host else 'localhost'
         self.port = port if port else OmniEngine.port
-        self.timeout = OmniEngine.timeout
+        self.timeouts = EngineTimeouts(timeouts)
         self._connected = False
-        self._filter_list = None
-        self._filter_timeout = OmniEngine._filter_timeout
         self._last_status = None
         self._file_system = Directory(self, 'root')
         self._perf_logger = OmniEngine._perf_logger
 
         # if isinstance(self.host, (OmniAddress, IPv4Address, IPv6Address)):
         #     _host = self.host.format()
         # else:
@@ -216,53 +288,67 @@
 
         # if isinstance(self.port, OmniPort):
         #     _port = self.port.port
         # else:
         #     _port = int(port)
 
         # _base_url must end with a '/'.
+        # _base_dms_url must end with a '/'.
         protocol = 'https' if secure else 'http'
         self._base_url = f'{protocol}://{self.host}:{int(self.port)}/api/v1/'
+        self._base_dms_url = f'{protocol}://{self.host}:{int(self.port)}/dms/v1/'
         self._session = requests.Session()
         self._session.keep_alive = True
 
     def __repr__(self) -> str:
-        return f'OmniEngine: {self._last_status.name}' if self._last_status else 'OmniEngine'
+        return f'OmniEngine: {self.name}'
 
     def __str__(self) -> str:
-        return f'OmniEngine: {self._last_status.name}' if self._last_status else 'OmniEngine'
+        return f'OmniEngine: {self.name}'
+
+    @property
+    def name(self):
+        return self._last_status.name if self._last_status else 'OmniEngine'
 
     def _operate_url(self, operation, url, params=None, data=None):
         if operation == EO.GET:
-            return self._session.get(url, verify=False, params=params, data=data)
+            return self._session.get(url, verify=False, params=params, data=data,
+                                     timeout=self.timeouts.as_tuple())
         elif operation == EO.POST:
-            return self._session.post(url, verify=False, params=params, data=data)
+            return self._session.post(url, verify=False, params=params, data=data,
+                                      timeout=self.timeouts.as_tuple())
         elif operation == EO.PUT:
-            return self._session.put(url, verify=False, params=params, data=data)
+            return self._session.put(url, verify=False, params=params, data=data,
+                                     timeout=self.timeouts.as_tuple())
         elif operation == EO.DELETE:
-            return self._session.delete(url, verify=False, params=params, data=data)
+            return self._session.delete(url, verify=False, params=params, data=data,
+                                        timeout=self.timeouts.as_tuple())
         return None
 
     def _pr_operate_url(self, pr, operation, url, params=None, data=None):
         resp = None
         if operation == EO.GET:
             pr.start = PeekTime()
-            resp = self._session.get(url, verify=False, params=params, data=data)
+            resp = self._session.get(
+                url, verify=False, params=params, data=data, timeout=self.timeouts.as_tuple())
             pr.end = PeekTime()
         elif operation == EO.POST:
             pr.start = PeekTime()
-            resp = self._session.post(url, verify=False, params=params, data=data)
+            resp = self._session.post(
+                url, verify=False, params=params, data=data, timeout=self.timeouts.as_tuple())
             pr.end = PeekTime()
         elif operation == EO.PUT:
             pr.start = PeekTime()
-            resp = self._session.put(url, verify=False, params=params, data=data)
+            resp = self._session.put(
+                url, verify=False, params=params, data=data, timeout=self.timeouts.as_tuple())
             pr.end = PeekTime()
         elif operation == EO.DELETE:
             pr.start = PeekTime()
-            resp = self._session.delete(url, verify=False, params=params, data=data)
+            resp = self._session.delete(
+                url, verify=False, params=params, data=data, timeout=self.timeouts.as_tuple())
             pr.end = PeekTime()
         return resp
 
     def _retry_operate_url(self, operation, url, params=None, data=None):
         retries = 3
         resp = self._operate_url(operation, url, params, data)
         while (resp.status_code == 503) and (retries > 0):
@@ -277,89 +363,130 @@
         while (resp.status_code == 503) and (retries > 0):
             time.sleep(1)
             retries -= 1
             resp = self._pr_operate_url(pr, operation, url)
         return resp
 
     def _issue_command(self, command, pr=None, operation=EO.GET,
-            format=DF.JSON, params=None, data=None):
+                       format=DF.JSON, params=None, data=None, dms=False):
         """Issue the command and return the response data.
-        The OmniEngine object must have a connection to an OmniEngine. 
+        The OmniEngine object must have a connection to an OmniEngine.
 
         Args:
             command (str): the command to issue.
 
         Returns:
             Success: response data or None on failure.
         """
         _text = None
         if self.is_connected:
             if format == DF.JSON:
-                self._session.headers.update({'accept':'application/json'})
+                self._session.headers.update({'accept': 'application/json'})
             elif format == DF.PLAIN:
-                self._session.headers.update({'accept':'text/plain'})
+                self._session.headers.update({'accept': 'text/plain'})
             elif format == DF.HTML:
-                self._session.headers.update({'accept':'text/html'})
+                self._session.headers.update({'accept': 'text/html'})
             elif format == DF.TAG_STREAM:
                 self._session.headers.update(
-                    {'accept':'application/octet-stream'})
+                    {'accept': 'application/octet-stream'})
             else:
                 raise OmniError('Unrecognized format parameter.')
-            url = self._base_url + command
+            # TODO: refactor out the dms test.
+            url = self._base_url + command if not dms else self._base_dms_url + command
             if pr:
-                resp = self._pr_retry_operate_url(pr, operation, url, params=params, data=data)
+                resp = self._pr_retry_operate_url(
+                    pr, operation, url, params=params, data=data)
             else:
-                resp = self._retry_operate_url(operation, url, params=params, data=data)
+                resp = self._retry_operate_url(
+                    operation, url, params=params, data=data)
 
             if format != DF.JSON:
-                self._session.headers.update({'accept':'application/json'})
+                self._session.headers.update({'accept': 'application/json'})
 
             if resp is None:
-                raise OmniError(f'REST API Command failed: Invalid operation.')                
-            if resp.status_code == 200:
+                raise OmniError('REST API Command failed: Invalid operation.')
+            if resp.status_code == 200 or resp.status_code == 201:
                 if format == DF.JSON:
                     _text = json.loads(resp.text)
                 elif format == DF.TAG_STREAM:
                     _text = resp.text.encode()
                 else:
                     _text = resp.text
             elif resp.status_code == 204:
-                _text = { 'results': [0] }
+                _text = {'results': [0]}
             elif resp.status_code == 503:
                 # 503 - Service temporarily unavailable
-                raise OmniError('REST API Command failed: ' \
-                    f'{resp.status_code}: {resp.reason}.')
+                raise OmniError('REST API Command failed: '
+                                f'{resp.status_code}: {resp.reason}.')
             else:
-                raise OmniError(f'REST API Command failed: {resp.status_code}', code=resp.status_code)
+                raise OmniError(
+                    f'REST API Command failed: {resp.status_code}', code=resp.status_code)
         return _text
 
+    def add_alarm(self, alarm: Alarm):
+        """ Add a new alarm to the OmniEngine
+        """
+        if not isinstance(alarm, Alarm):
+            raise ValueError('An Alarm object is required.')
+        pr = self.perf('add_alarm')
+        data = json.dumps(alarm._store())
+        return self._issue_command(f'{Alarm._endpoint}{alarm.id.format()}/', pr, EO.PUT, data=data)
+
     def add_capture_template(self, template):
         """Add a Capture Template to the OmniEngine.
 
         Return:
             bool: True on success, False on failure.
         """
         if isinstance(template, CaptureTemplate):
             t = template.store(encapsulate=True)
         else:
             raise ValueError('A CaptureTemplate is required.')
         pr = self.perf('add_capture_template')
         resp = self._issue_command('capture-templates/', pr, EO.POST, data=t)
-        return _success(resp)
+        return is_success(resp)
+
+    def add_decryption_key_templates(self, key_template):
+        """Add one or more Decryption Key Templates to the OmniEngine.
+
+        Return:
+            bool: True on success, False on failure.
+        """
+        key_template_props = []
+        key_templates = [key_template] if isinstance(
+            key_template, DecryptionKeyTemplate) else key_template
+
+        if not isinstance(key_templates, list):
+            raise TypeError(
+                "The decryption key templates parameter must be a DecryptionKeyTemplate or a list.")
+        for _key_template in key_templates:
+            if isinstance(_key_template, DecryptionKeyTemplate):
+                props = _key_template._store()
+                key_template_props.append(props)
+
+        req_props = {
+            'keys': key_template_props
+        }
+        pr = self.perf('add_decryption_key_templates')
+
+        data = json.dumps(req_props)
+        self._issue_command('decryption-keys/', pr, EO.POST, data=data)
+        return None
 
     def add_events(self, events):
         """Add one or more entries to the OmniEngine's Event Log.
 
         Args:
-            event (EventLogEntry or a list of EventLogEntry): 
+            event (EventLogEntry or a list of EventLogEntry):
         """
         evt_props = []
         _events = [events] if isinstance(events, EventLogEntry) else events
         if not isinstance(_events, list):
-            raise TypeError("The events parameter must be an EventLogEntry or a list.")
+            raise TypeError(
+                "The events parameter must be an EventLogEntry or a list.")
         for evt in _events:
             if isinstance(evt, EventLogEntry):
                 props = {
                     'longMessage': '',
                     'severity': evt.severity,
                     'shortMessage': evt.message,
                     'sourceId': str(OmniId.null_id),
@@ -392,107 +519,182 @@
         else:
             raise TypeError('omnifilter must be or contain a Filter.')
 
         pr = self.perf('add_filter')
         props = item._store()
         cmd = f'filters/{item.id.format()}'
         resp = self._issue_command(cmd, pr, EO.PUT, data=props)
-        if not _success(resp):
+        if not is_success(resp):
             raise OmniError('Failed to add filter.')
         return self.get_filter(item.id)
 
+    def add_remote_engine(self, ids: List[RemoteEngine]):
+        """Add one or more RemoteEngines to the OmniEngine."""
+        return RemoteEngine.add(self, ids)
+
+    def convert_filter_string(self, filter: str, validate: bool = False) -> Optional[Filter]:
+        """ Convert a filter string to a filter object and return the object and error status """
+        ret = None
+        pr = self.perf('convert_filter_string')
+        params = {'validateOnly': jbool(validate)}
+        resp = self._issue_command(
+            'filter-convert/', pr, EO.POST, params=params, data=filter)
+
+        if isinstance(resp, dict):
+            if 'filter' in resp:
+                ret = Filter(criteria=resp['filter'])
+
+        return ret
+
     def create_capture(self, template):
         """Create a new Capture from a
         :class:`CaptureTemplate <omniscript.capturetemplate.CaptureTemplate>`
         object.
-        
+
         Args:
             template(str or
             :class:`CaptureTemplate <omniscript.capturetemplate.CaptureTemplate>`
             ): the capture template.
 
         Returns:
-            A :class:`Capture <omniscript.capture.Capture>` 
+            A :class:`Capture <omniscript.capture.Capture>`
             object of the new capture or None.
         """
         if isinstance(template, six.string_types):
             ct = template
         elif isinstance(template, CaptureTemplate):
             ct = template.store(self, True)
         pr = self.perf('create_capture')
-        cmd = f'captures/'
+        cmd = 'captures/'
         resp = self._issue_command(cmd, pr, EO.POST, data=ct)
         if not resp:
             raise OmniError('Failed to create capture.')
         if isinstance(resp, dict):
             if 'id' in resp:
                 id = resp['id']
                 cl = self.get_capture_list()
                 return find_capture(cl, id, 'id')
         return None
 
+    def create_directory(self, directory: str) -> None:
+        """Creates a new directory on the engine."""
+        Directory.create(self, directory)
+
+    def create_file(self, file: str) -> Optional[dict]:
+        """Create a file on the engine, if the file exists its content
+        will be discarded.
+        """
+        params = {
+            'path': file
+        }
+        pr = self.perf('create_file')
+        self._issue_command('create-file/', pr, EO.POST, params=params)
+
     def create_forensic_search(self, template):
         """Create a new Forensic Search from a
-        :class:`ForensicTemplate 
+        :class:`ForensicTemplate
         <omniscript.forensictemplate.ForensicTemplate>`
         object.
 
         Args:
             template(str or
-            :class:`ForensicTemplate 
+            :class:`ForensicTemplate
             <omniscript.forensictemplate.ForensicTemplate>`
             ): the settings of the search.
 
         Returns:
-            A :class:`ForensicSearch 
+            A :class:`ForensicSearch
             <omniscript.forensicsearch.ForensicSearch>`
             object or None."""
         if isinstance(template, six.string_types):
             fst = template
         elif isinstance(template, ForensicTemplate):
             fst = template.store(self, True)
         pr = self.perf('create_forensic_search')
-        cmd = f'forensic-searches/'
+        cmd = 'forensic-searches/'
         resp = self._issue_command(cmd, pr, EO.POST, data=fst)
         if not resp:
             raise OmniError('Failed to create Forensic Search.')
         if isinstance(resp, dict):
             if 'id' in resp:
                 id = resp['id']
                 return self.get_forensic_search(id)
         return None
 
+    def create_token(self, token: AuthenticationToken) -> Optional[dict]:
+        """ Create a new authentication token with the given template """
+        resp = None
+        if isinstance(token, AuthenticationToken):
+            pr = self.perf('create_token')
+            data = json.dumps(token._create_template())
+            resp = self._issue_command(
+                AuthenticationToken.endpoint, pr, EO.POST, data=data)
+
+            if not resp:
+                raise OmniError('Failed to create authentication token')
+
+        return resp if isinstance(resp, dict) else None
+
+    def delete_adapter(self, adapter: Union[Adapter, OmniId, str]):
+        """ Delete the specified adapter from the engine. """
+        id = adapter.adapter_id if isinstance(adapter, Adapter) else adapter
+        pr = self.perf('delete_adapter')
+        command = f'{Adapter._endpoint}/{str(id)}/'
+        props = self._issue_command(command, pr, EO.DELETE)
+        if not is_success(props):
+            raise OmniError('Delete Adapter failed')
+
+    def delete_alarm(self, alarm_id: Union[Alarm, OmniId, str]):
+        """ Delete the specified alarm in the list """
+        _id = alarm_id.id if isinstance(alarm_id, Alarm) else OmniId(alarm_id)
+        pr = self.perf('delete_alarm')
+        props = self._issue_command(f'{Alarm._endpoint}{_id.format()}', pr, EO.DELETE)
+        if not is_success(props):
+            raise OmniError('Delete Alarm failed')
+
+    def delete_all_audit_log(self):
+        """Delete all messages in the OmniEngine's Audit Log.
+        """
+        pr = self.perf('delete_all_audit_log')
+        props = self._issue_command('audit-log/', pr, EO.DELETE)
+        if not is_success(props):
+            raise OmniError('Delete all Audit Log Messages failed.')
+
     def delete_all_capture_sessions(self):
         """ Delete all the Capture Sessions from the engine.
 
         Note that 'Capture Sessions' are different from Captures.
         See the Details tab at the bottom of an OmniEngine's
         Forensics tab.
         """
         pr = self.perf('delete_all_capture_sessions')
         props = self._issue_command('capture-sessions/', pr, EO.DELETE)
-        if not _success(props):
-            raise OmniError('Command failed: 0x80004005')
+        if not is_success(props):
+            raise OmniError('Faild to delete all Capture Sessions.')
 
     def delete_all_filters(self):
         """ Delete all the Filters from the engine.
         """
         pr = self.perf('delete_all_filters')
         props = self._issue_command('filters/', pr, EO.DELETE)
-        if not _success(props):
-            raise OmniError('Command failed: 0x80004005')
+        if not is_success(props):
+            raise OmniError('Failed to delete all Filters.')
 
     def delete_all_forensic_searches(self):
         """ Delete all the Forensic Searches from the engine.
         """
         pr = self.perf('delete_all_forensic_searches')
         props = self._issue_command('forensic-searches/', pr, EO.DELETE)
         # if there are no Forensic Searches, then {return:[]} is returned.
-        if not _almost_success(props):
-            raise OmniError('Command failed: 0x80004005')
+        if not is_almost_success(props):
+            raise OmniError('Failed to delete all Forensic Searches')
+
+    def delete_all_remote_engines(self):
+        """ Delete all the RemoteEngines from the engine."""
+        RemoteEngine.delete_all(self)
 
     def delete_capture(self, capture, retry=3):
         """Delete a Capture from the OmniEngine.
 
         Args:
             capture (str,
             :class:`OmniId <omniscript.omniid.OmniId>` or
@@ -501,16 +703,16 @@
             Or a list of captures.
         """
         ids = _capture_id_list(capture)
         for id in ids:
             pr = self.perf('delete_capture')
             cmd = f'captures/{id.format()}'
             props = self._issue_command(cmd, pr, EO.DELETE)
-            if not _success(props):
-                raise OmniError('Command failed: 0x80004005')
+            if not is_success(props):
+                raise OmniError('Failed to delete Capture')
 
     def delete_capture_session(self, session):
         """Deletes Capture Sessions from the OmniEngine.
 
         Args:
             session (int, str,
             :class:`CaptureSession <omniscript.capturesession.CaptureSession>`
@@ -518,16 +720,16 @@
             Or a list of sessions.
         """
         ids = _capture_session_list(session)
         for id in ids:
             pr = self.perf('delete_capture_session')
             cmd = f'capture-sessions/{id}'
             props = self._issue_command(cmd, pr, EO.DELETE)
-            if not _success(props):
-                raise OmniError('Command failed: 0x80004005')
+            if not is_success(props):
+                raise OmniError('Failed to delete Capture Session')
 
     def delete_capture_template(self, template):
         """Deletes Capture Templates from the OmniEngine.
 
         Args:
             template (int, str,
             :class:`CaptureTemplate <omniscript.capturetemplate.CaptureTemplate>`
@@ -535,22 +737,43 @@
             Or a list of templates.
         """
         ids = _capture_template_list(template)
         for id in ids:
             pr = self.perf('delete_capture_template')
             cmd = f'capture-templates/{id.format()}'
             props = self._issue_command(cmd, pr, EO.DELETE)
-            if not _success(props):
-                raise OmniError('Command failed: 0x80004005')
+            if not is_success(props):
+                raise OmniError('Failed to delete Capture Template.')
+
+    def delete_decryption_keys(self, decryptkey: list):
+        """Deletes Decryption Keys from the OmniEngine.
+        """
+        _ids = _capture_decryption_key_list(decryptkey)
+        req_props = []
+        for _id in _ids:
+            req_props.append(('ids', _id))
+        if not req_props:
+            raise TypeError('No decryption key specified.')
+
+        pr = self.perf('delete_decryption_keys')
+        cmd = 'decryption-keys/'
+        resp = self._issue_command(cmd, pr, EO.DELETE, params=req_props)
+
+        if not is_almost_success(resp):
+            raise OmniError('Failed to delete Decryption Keys')
+
+    def delete_directory(self, directory: str) -> None:
+        """Delete/remove a directory from the engine."""
+        Directory.delete(self, directory)
 
     def delete_event_log(self, capture=None, compact=False):
         """Delete the OmniEngine's Event Log.
 
         Args:
-            capture (OmniId, str, Capture, CaptureSession): 
+            capture (OmniId, str, Capture, CaptureSession):
             Delete the entries for just this 'capture'.
             compact (bool): compact the Event Log after deleting
             entries.
         """
         if isinstance(capture, OmniId):
             _context_id = capture
         elif isinstance(capture, six.string_types):
@@ -562,22 +785,22 @@
         else:
             _context_id = OmniId()
         req_props = {
             'contextId': _context_id.format(),
             'compact': jbool(compact)
         }
         pr = self.perf('delete_event_log')
-        cmd = f'events/'
+        cmd = 'events/'
         resp = self._issue_command(cmd, pr, EO.DELETE, params=req_props)
         if not isinstance(resp, dict):
             raise OmniError('Failed to Delete Event Log.')
 
     def delete_file(self, target):
         """Delete a list of files from the OmniEngine.
-        
+
         Args:
             target (str): one or more files to delete. If not fully qualified
                           then target will be relative to the engine's
                           data directory.
 
         Failure:
             Raises an OmniError with results as the list of failures.
@@ -587,46 +810,46 @@
         for _t in _target:
             if isinstance(_t, PacketFileInformation):
                 _name = _t.path
             elif isinstance(_t, FileInformation):
                 _name = _t.name
             else:
                 _name = _t
-            req_props.append( ('files', _name) )
+            req_props.append(('files', _name))
         if not req_props:
             raise TypeError('No files specified.')
         pr = self.perf('delete_files')
-        cmd = f'files/'
+        cmd = 'files/'
         resp = self._issue_command(cmd, pr, EO.DELETE, params=req_props)
         if isinstance(resp, dict):
             results = resp.get('results')
             failures = []
             if isinstance(results, list):
                 for r in results:
                     if isinstance(r, dict):
                         code = r.get('result')
                         if code != 0:
                             failures.append(r)
                 if failures:
-                    raise OmniError('Failed to delete 1 or more files.', result=failures)
+                    raise OmniError(
+                        'Failed to delete 1 or more files.', result=failures)
 
-    def delete_filter(self, omnifilter):
+    def delete_filter(self, omnifilter: Union[Filter, List[Filter]]):
         """Delete a filter from the OmniEngine's filter set.
 
         Args:
             omnifilter (str,
             :class:`OmniId <omniscript.omniid.OmniId>` or
             :class:`Filter <omniscript.filter.Filter>`
             ): the id of the filter or a Filter object.
         """
         if not omnifilter:
             return
         idlist = []
-        filterlist = omnifilter \
-            if isinstance(omnifilter, list) else [omnifilter]
+        filterlist = omnifilter if isinstance(omnifilter, list) else [omnifilter]
         for f in filterlist:
             if isinstance(f, Filter):
                 idlist.append(f.id)
             elif isinstance(f, OmniId):
                 idlist.append(f)
             elif isinstance(f, six.string_types):
                 idlist.append(OmniId(f))
@@ -635,60 +858,85 @@
         if idlist:
             fl = self.get_filter_list()
             for id in idlist:
                 if find_filter(fl, id, 'id'):
                     pr = self.perf('delete_filter')
                     cmd = f'filters/{id.format()}'
                     props = self._issue_command(cmd, pr, EO.DELETE)
-                    if not _success(props):
-                        raise OmniError('Command failed: 0x80004005')
+                    if not is_success(props):
+                        raise OmniError('Failed to delete Filter')
+
+    def delete_filter_list(self):
+        """ Delete the entire filter list """
+        if len(self.get_filter_list()) > 0:
+            pr = self.perf('delete_filter_list')
+            self._issue_command(Filter.endpoint, pr, EO.DELETE)
 
     def delete_forensic_search(self, search):
-        """Delete a 
+        """Delete a
         :class:`ForensicSearch <omniscript.forensicsearch.ForensicSearch>`
         for the specified id.
-        
+
         Returns:
             A
             :class:`ForensicSearch <omniscript.forensicsearch.ForensicSearch>`
             object.
         """
         if isinstance(search, ForensicSearch):
             id = search.id
         else:
             id = OmniId(search)
         pr = self.perf('delete_forensic_search')
-        props = self._issue_command(f'forensic-searches/{id.format()}', pr, EO.DELETE)
-        if not _success(props):
-            raise OmniError('Command failed: 0x80004005')
+        props = self._issue_command(
+            f'forensic-searches/{id.format()}', pr, EO.DELETE)
+        if not is_success(props):
+            raise OmniError('Failed to delete Forensic Search')
+
+    def delete_notification(self, notificationId) -> Optional[dict]:
+        """ Delete the notification from the engine """
+        return Notifications(self).delete_notification(notificationId)
+
+    def delete_remote_engine(self, remote_engine: Union[RemoteEngine, OmniId, str]):
+        return RemoteEngine.delete(self, remote_engine)
+
+    def delete_token(self, tokens: Union[List[AuthenticationToken], AuthenticationToken]):
+        """ Delete the specified tokens from the input list """
+        list_ = tokens if isinstance(tokens, list) else [tokens]
+        if list_:
+            pr = self.perf('delete_token')
+            props = [('ids', token.authentication_token_id) for token in list_]
+            resp = self._issue_command(
+                AuthenticationToken.endpoint, pr, EO.DELETE, params=props)
+            if not is_almost_success(resp):
+                raise OmniError('Delete Token failed')
 
     def disconnect(self):
         """Disconnect from the OmniEngine
         """
         return self.logout()
 
     def file_database_operation(self, operation=DatabaseOperation.SYNC):
         """Perform one of the file database maintenance operations.
 
         Input:
             operation : Must be one of the DATABASE_ constants.
         """
         if operation == DatabaseOperation.SYNC:
             pr = self.perf('synchronize_file_databases')
-            props = self._issue_command('database-sync/', pr, EO.POST)
+            self._issue_command('database-sync/', pr, EO.POST)
         elif operation == DatabaseOperation.INDEX:
             pr = self.perf('file_databases_index')
-            props = self._issue_command('database-index/', pr, EO.POST)
+            self._issue_command('database-index/', pr, EO.POST)
         elif operation == DatabaseOperation.MAINTENANCE:
             pr = self.perf('file_databases_maintenance')
-            props = self._issue_command('database-maintenance/', pr, EO.POST, DF.PLAIN)
+            self._issue_command('database-maintenance/', pr, EO.POST, DF.PLAIN)
         else:
-            raise OmniEngine('Illeagal operation, must be one of the DATABASE_ constants.')
+            raise OmniError('Illeagal operation, must be one of the DATABASE_ constants.')
 
-    def find_adapter(self, value, attrib=adapter_find_attributes[0]):
+    def find_adapter(self, value, attrib=Adapter.find_attributes[0]):
         """Find an :class:`Adapter <omniscript.adapter.Adapter>`
         in the OmniEngine's list of adapters.
 
         Args:
             value (str or :class:`Adapter <omniscript.adapter.Adapter>`
             ): the search key.
             attrib ('name' or 'id'): what attribute to search on.
@@ -720,14 +968,34 @@
         Note:
             If value is an :class:`Capture <omniscript.capture.Capture>`,
             then the search is performed on the Capture's id.
         """
         captures = self.get_capture_list()
         return find_capture(captures, value, attrib)
 
+    def find_decryption_key(self, value, attrib=DecryptionKey.find_attributes[0]):
+        """Find an :class:`DecryptionKey <omniscript.decryptionkey.DecryptionKey>`
+        in the OmniEngine's list of decryption keys.
+
+        Args:
+            value (str or :class:`DecryptionKey <omniscript.decryptionkey.DecryptionKey>`
+            ): the search key.
+            attrib ('name' or 'id'): what attribute to search on.
+
+        Returns:
+            An :class:`DecryptionKey <omniscript.decryptionkey.DecryptionKey>`
+            object of the DecryptionKey.
+
+        Note:
+            If value is an :class:`DecryptionKey<omniscript.decryptionkey.DecryptionKey>`,
+            then the search is performed on the DecryptionKey's id.
+        """
+        keys = self.get_decryption_key_list()
+        return find_decryption_key(keys, value, attrib)
+
     def find_filter(self, value, attrib=find_attributes[0]):
         """Find a :class:`Filter <omniscript.filter.Filter>`
         in the OmniEngine's filter set.
 
         Args:
             value (str or :class:`Filter <omniscript.filter.Filter>`
             ): the search key.
@@ -758,84 +1026,109 @@
         """
         searches = self.get_forensic_search_list()
         return find_forensic_search(searches, value, attrib)
 
     def get_adapter_list(self):
         """Get the OmniEngine's list of
         :class:`Adapter <omniscript.adapter.Adapter>`.
-        
+
         Returns:
             A list of
             :class:`Adapter <omniscript.adapter.Adapter>`
             objects.
         """
         pr = self.perf('get_adapter_list')
         props = self._issue_command('adapters/', pr)
         return _create_adapter_list(self, props) if props else None
- 
+
     def get_adapter_information_list(self):
         """Get the OmniEngine's list of
         :class:`AdapterInformation <omniscript.adapterinformation.AdapterInformation>`.
-        
+
         Returns:
             A list of
             :class:`AdapterInformation <omniscript.adapterinformation.AdapterInformation>`
             objects.
         """
         pr = self.perf('get_adapter_information_list')
         props = self._issue_command('adapters/info/', pr)
         return _create_adapter_information_list(self, props) if props else None
- 
-    def get_alarm_list(self):
+
+    def get_alarm(self, alarm_id: Union[Alarm, OmniId, str]) -> Optional[Alarm]:
+        """Get a specific OmniEngine Alarm.
+        """
+        _id = alarm_id.id if isinstance(alarm_id, Alarm) else OmniId(alarm_id)
+        pr = self.perf('get_alarm')
+        props = self._issue_command(f'{Alarm._endpoint}{_id.format()}/', pr)
+        alarm_list = _create_alarm_list(props)
+        return alarm_list[0] if alarm_list and len(alarm_list) else None
+
+    def get_alarm_list(self) -> Optional[List[Alarm]]:
         """Get the OmniEngine's list of alarms.
-        
+
         Returns:
             A list of :class:`Alarm <omniscript.alarm.Alarm>` objects.
         """
         pr = self.perf('get_alarm_list')
-        props = self._issue_command('alarms/', pr)
-        return _create_alarm_list(props) if props else None
+        props = self._issue_command(Alarm._endpoint, pr)
+        return _create_alarm_list(props) if isinstance(props, dict) else []
 
     def get_analysis_module_list(self):
         """Get the OmniEngine's list of Analysis Modules.
 
         Returns:
             A list of
             :class:`AnalysisModule <omniscript.analysismodule.AnalysisModule>`
             objects.
         """
         pr = self.perf('get_analysis_module_list')
         props = self._issue_command('capabilities/', pr)
         return _create_analysis_module_list(self, props.get('pluginsInfo')) if (
             props and 'pluginsInfo' in props) else None
 
+    def get_audit_log(self):
+        """Return the OmniEngine's Audit Log.
+        """
+        pr = self.perf('get_audit_log')
+        props = self._issue_command('audit-log/', pr)
+        return AuditLog(self, props)
+
     def get_application_list(self):
         """The the list of Applications.
         """
         pr = self.perf('get_application_list')
         props = self._issue_command('applications/', pr)
         return _create_application_list(props)
 
+    def get_capabilities(self) -> Capabilities:
+        """Gets the engine capabilties"""
+        command = 'capabilities/'
+        pr = self.perf('get_capabilities')
+        props = self._issue_command(command, pr)
+        if not isinstance(props, dict):
+            raise OmniError('Failed to get engine capabilities.')
+        return Capabilities(props)
+
     def get_capture_list(self):
         """Get the OmniEngine's list of
         :class:`Capture <omniscript.capture.Capture>`.
-        
+
         Returns:
             A list of
             :class:`Capture <omniscript.capture.Capture>`
             objects.
         """
         pr = self.perf('get_capture_list')
         props = self._issue_command('captures/', pr)
         return _create_capture_list(self, props) if props else None
 
     def get_capture_session_list(self):
         """Get the OmniEngine's list of
         :class:`CaptureSession <omniscript.capturesession.CaptureSession>`.
-        
+
         Returns:
             A list of
             :class:`CaptureSession <omniscript.capturesession.CaptureSession>`
             objects.
         """
         pr = self.perf('get_capture_session_list')
         props = self._issue_command('capture-sessions/', pr)
@@ -854,53 +1147,65 @@
             id = OmniId(obj)
         pr = self.perf('get_capture_template')
         cmd = f'capture-templates/{id.format()}/'
         props = self._issue_command(cmd, pr)
         return CaptureTemplate(props=props, engine=self) if props else None
 
     def get_capture_template_list(self):
-        """Get the OmniEngine's list of stored 
+        """Get the OmniEngine's list of stored
         :class:`CaptureTemplates <omniscript.capturetemplate.CaptureTemplate>`.
-        
+
         Returns:
             A list of
             :class:`Capture <omniscript.capturetemplate.CaptureTemplate>`
             objects.
         """
         pr = self.perf('get_capture_template_list')
         props = self._issue_command('capture-templates/', pr)
         return _create_capture_template_list(self, props) if props else None
 
+    def get_connected_user_list(self):
+        """Return the list of connected users."""
+        return User.get_connected_user_list(self)
+
     def get_country_list(self):
         """Return the list of Country Names and Codes.
         """
         pr = self.perf('get_country_list')
         props = self._issue_command('countries/', pr)
         return _create_country_list(props)
 
-    def get_diagnostics(self, command=Diagnostics.DEFAULT, verbose=False):
+    def get_decryption_key_list(self) -> list:
+        """Return the list of DecryptionKeys
+
+        """
+        pr = self.perf('get_decryption_key_list')
+        props = self._issue_command('decryption-keys/', pr)
+        return _create_decryption_key_list(props)
+
+    def get_diagnostics(self, command: Diagnostics = Diagnostics.DEFAULT,
+                        verbose: bool = False) -> Optional[str]:
         """Get diagnostice information from the Engine.
         """
         cmd_labels = 'default', 'drives', 'processes', 'raid', 'system-log'
         if command not in Diagnostics:
-            raise TypeError('command must be one of the Diagnostics constants.')
+            raise TypeError(
+                'command must be one of the Diagnostics constants.')
         req_props = {
             'verbose': jbool(verbose)
         }
         pr = self.perf('get_diagnostics')
         cmd = f'diagnostics/{cmd_labels[command]}/'
         txt = self._issue_command(cmd, pr, EO.POST, DF.PLAIN, params=req_props)
         return txt
 
-    def get_directory(self, path=None, files=True, hidden=False):
+    def get_directory(self, path: str = None, files: bool = True, hidden: bool = False):
         """Get a :class:`Directory <omniscript.directory.Directory>`
         object of the host system's File System.
-
         Default path is the engine's data directory.
-        
         Returns:
             A
             :class:`Directory <omniscript.directory.Directory>`
             object.
         """
         if path:
             _path = path
@@ -910,25 +1215,29 @@
             _path = '/var/lib/omni/data'
         req_props = {
             'path': _path,
             'showFiles': jbool(files),
             'showHiddenFiles': jbool(hidden)
         }
         pr = self.perf('get_directory')
-        cmd = f'directory-list/'
+        cmd = 'directory-list/'
         resp = self._issue_command(cmd, pr, params=req_props)
         return Directory(self, resp)
-    
+
+    def get_engine_settings(self) -> Optional[EngineSettings]:
+        """ Get the engine settings from the engine """
+        return EngineSettings.get(self)
+
     def get_event_log(self, first=None, count=None, capture=None, query=None, time_span=None):
         """Get the OmniEngine's Event Log.
 
         Args:
             first (int): the index of the first entry to retrieve.
             count (int): the maximum number of entries to retrieve.
-            capture (OmniId, str, Capture, CaptureSession): 
+            capture (OmniId, str, Capture, CaptureSession):
             Get entries for just this 'capture'.
             query (str): only entries whos message contains query.
 
         Returns:
             A :class:`EventLog <omniscript.eventlog.EventLog>` object.
         """
         if isinstance(capture, OmniId):
@@ -943,17 +1252,17 @@
             _context_id = None
 
         req_props = {
             'informational': jtrue,
             'major': jtrue,
             'minor': jtrue,
             'severe': jtrue,
-            'messages': jtrue,
-            'sourceId': str(OmniId.null_id),
-            'sourceKey': 0,
+            'messages': jtrue
+            # 'sourceId': str(OmniId.null_id),
+            # 'sourceKey': 0,
         }
 
         if first is not None:
             req_props['offset'] = int(first)
         if count is not None:
             req_props['limit'] = int(count)
         if _context_id:
@@ -961,22 +1270,28 @@
         if query:
             req_props['search'] = query
         if isinstance(time_span, (tuple, list, dict)) and len(time_span) == 2:
             req_props['startTime'] = time_span[0].iso_time()
             req_props['stopTime'] = time_span[1].iso_time()
 
         pr = self.perf('get_event_log')
-        data = json.dumps(req_props)
-        cmd = f'events/'
+        cmd = 'events/'
         resp = self._issue_command(cmd, pr, params=req_props)
         return EventLog(self, resp, _context_id, query)
 
-    def get_file(self, source):
+    def get_expert_preferences(self) -> List[ExpertPreferences]:
+        """ Get the expert preferences from the engine """
+        pr = self.perf('get_expert_prefs')
+        command = 'expert-prefs/'
+        resp = self._issue_command(command, pr)
+        return ExpertPreferences(resp)
+
+    def get_file(self, source: str, delete: bool = False):
         """Get a file from the OmniEngine.
-        
+
         Args:
             source (str): name of the file to get. If not fully qualified
                           then source will be relative to the engine's
                           data directory.
 
         Returns:
             The contents of the file as an array of bytes.
@@ -986,25 +1301,25 @@
         elif isinstance(source, FileInformation):
             _source = source.name
         else:
             _source = source
 
         req_props = {
             'file': _source,
-            'delete': jfalse
+            'delete': jtrue if delete else jfalse
         }
         pr = self.perf('get_file')
-        cmd = f'files/'
+        cmd = 'files/'
         resp = self._issue_command(cmd, pr, params=req_props, format=DF.PLAIN)
         return resp
-    
+
     # def get_file_system(self, path='/', files=True, hidden=False):
     #     """Get host system's File System as a tree of Directory
     #     objects.
-        
+
     #     Returns:
     #         A list of
     #         :class:`Directory <omniscript.directory.Directory>`
     #         objects.
     #     """
     #     p = self._last_status.data_directory
     #     req_props = {
@@ -1015,18 +1330,18 @@
     #     pr = self.perf('get_file_system')
     #     cmd = f'directory-list/'
     #     resp = self._issue_command(cmd, pr, params=req_props)
     #     if resp.status_code != 200:
     #         return None
     #     props = json.loads(resp.text)
     #     return _create_file_system(self, props)
-    
-    def get_filter(self, omnifilter):
+
+    def get_filter(self, omnifilter: Union[Filter, OmniId, str]) -> Optional[Filter]:
         """Get :class:`Filter <omniscript.filter.Filter>` from the engine.
-        
+
         Args:
             omnifilter (str, id, Filter): id of the Filter
         Returns:
             A  :class:`Filter <omniscript.filter.Filter>` object.
         """
         if isinstance(omnifilter, Filter):
             id = omnifilter.id
@@ -1036,47 +1351,40 @@
             id = OmniId(omnifilter)
         elif omnifilter is not None:
             raise TypeError('omnifilter must be an OmniId.')
         else:
             return None
 
         pr = self.perf('get_filter')
-        cmd = f'filters/{id.format()}'
+        cmd = f'{Filter.endpoint}{id.format()}'
         props = self._issue_command(cmd, pr)
         filter_list = _create_filter_list(props)
         return filter_list[0] if filter_list else None
 
     def get_filter_list(self, refresh=True):
         """Get the OmniEngine's :class:`Filter <omniscript.filter.Filter>`
         set.
-        
+
         Args:
             refresh(bool): If True will force a refresh, else refresh
                            if the timeout has expired.
         Returns:
             A list of
             :class:`Filter <omniscript.filter.Filter>`
             objects.
         """
-        do_refresh = refresh
-        if not refresh and self._filter_list:
-            delta_time = PeekTime() - self._filter_list[1]
-            do_refresh = delta_time.value > self._filter_timeout
-        if not self._filter_list or do_refresh:
-            pr = self.perf('get_filter_list')
-            props = self._issue_command('filters/', pr)
-            filter_list = _create_filter_list(props)
-            self._filter_list = (filter_list, PeekTime())
-        return self._filter_list[0]
+        pr = self.perf('get_filter_list')
+        props = self._issue_command(Filter.endpoint, pr)
+        return _create_filter_list(props)
 
     def get_forensic_search(self, search):
-        """Get a 
+        """Get a
         :class:`ForensicSearch <omniscript.forensicsearch.ForensicSearch>`
         for the specified id.
-        
+
         Returns:
             A
             :class:`ForensicSearch <omniscript.forensicsearch.ForensicSearch>`
             object.
         """
         if isinstance(search, ForensicSearch):
             id = search.id
@@ -1088,48 +1396,159 @@
 
     def get_forensic_file_list(self):
         return None
 
     def get_forensic_search_list(self):
         """Get the OmniEngine's list of
         :class:`ForensicSearch <omniscript.forensicsearch.ForensicSearch>`.
-        
+
         Returns:
             A list of
             :class:`ForensicSearch <omniscript.forensicsearch.ForensicSearch>`
             objects.
         """
         pr = self.perf('get_forensic_search_list')
         props = self._issue_command('forensic-searches/', pr)
         return _create_forensic_search_list(self, props) if props else None
 
     def get_graph_template_list(self):
         """Get the OmniEngine's list of
         :class:`GraphTemplate <omniscript.graphtemplate.GraphTemplate>`.
-        
+
         Returns:
             A list of :class:`GraphTemplate <omniscript.graphtemplate.GraphTemplate>`
             objects.
         """
         pr = self.perf('get_graph_template_list')
         props = self._issue_command('graphs/', pr)
         return _create_graph_template_list(props) if props else None
 
+    def get_license(self) -> Optional[License]:
+        """ Get the license information from the engine """
+        pr = self.perf('get_license')
+        props = self._issue_command(License.endpoint, pr)
+        return License(props) if isinstance(props, dict) else None
+
+    def get_license_locking_code(self, criteria: Union[List[int], int]) -> Optional[str]:
+        """ Get the license locking code from the engine """
+        pr = self.perf('get_license_locking_code')
+        flags = sum(criteria, 0) if isinstance(criteria, list) else criteria
+        props = self._issue_command(
+            f'{License.endpoint}locking-code/{flags}', pr)
+
+        return props['lockingCode'] if isinstance(props, dict) else None
+
+    def get_license_settings(self) -> Optional[LicenseSettings]:
+        """ Get the license settings from the engine """
+        pr = self.perf('get_license_settings')
+        props = self._issue_command(LicenseSettings.endpoint, pr)
+        return LicenseSettings(props) if isinstance(props, dict) else None
+
+    def get_liveflow_configuration(self) -> Optional[LiveFlowConfiguration]:
+        """ Get the liveflow configuration from the engine """
+        return LiveFlow(self).get_liveflow_configuration()
+
+    def get_liveflow_context(self) -> Optional[LiveFlowContext]:
+        """ Get the liveflow context from the engine """
+        return LiveFlow(self).get_liveflow_context()
+
+    def get_liveflow_status(self) -> Optional[LiveFlowStatus]:
+        """ Get the liveflow status from the engine """
+        return LiveFlow(self).get_liveflow_status()
+
+    def get_name_table(self):
+        """Get the list of Name Objects."""
+        pr = self.perf('get_names')
+        props = self._issue_command('names/', pr)
+        return NameTable(self, props)
+
+    def get_notification(self, notificationId) -> Optional[NotificationActions]:
+        """ Get the notification from the engine """
+        return Notifications(self).get_notification(notificationId)
+
+    def get_notifications(self) -> Optional[NotificationActions]:
+        """ Get the notifications from the engine """
+        return Notifications(self).get_notifications()
+
     def get_packet_file_list(self):
         """Get a list of packet files and their attributes.
-        
+
         Returns:
             A list of
             :class:`PacketFileInformation <omniscript.packetfileinformation.PacketFileInformation>`
             objects.
         """
         pr = self.perf('get_packet_file_list')
         props = self._issue_command('files-list/', pr)
         return _create_packet_file_information_list(props) if props else None
 
+    def get_protocol_list(self) -> List[Protocol]:
+        """Get the list of protocols.
+        """
+        pr = self.perf('get_protocol_list')
+        props = self._issue_command('protocols/', pr)
+        return _create_protocol_list(props)
+
+    def get_protocol_translation_list(self) -> List[PT]:
+        """ Get the list of protocol translations """
+        pr = self.perf('get_protocol_translations_list')
+        props = self._issue_command(PT.endpoint, pr)
+        return _create_protocol_translations_list(props)
+
+    def get_remote_engine(self, id):
+        return RemoteEngine.get(self, id)
+
+    def get_remote_engine_list(self) -> Optional[RemoteEngine]:
+        """ Get the engine's list of remote engines """
+        return RemoteEngine.get_all(self)
+
+    def get_select_related_progress(self, endpoint: str, id: int, timeout: float) -> int:
+        """ Get the progress percentage for the select related """
+        progress = 0
+        pr = self.perf('get_select_related_progress')
+        command = f'{endpoint}/{Selection.Command.Progress}/{id}/'
+
+        # Add some delay if needed to help the select related complete
+        time.sleep(timeout)
+
+        props = self._issue_command(command, pr)
+
+        if isinstance(props, dict):
+            if Selection.Command.Progress in props:
+                val = props[Selection.Command.Progress]
+                if isinstance(val, int):
+                    progress = val
+
+        return progress
+
+    def get_selection_packets(self, id: int, endpoint: str, pr_log: str, timeout: float) -> dict:
+        """ Shared helper to retrieve the packets based on id and endpoint """
+        packets = {}
+        if self.get_select_related_progress(endpoint, id, timeout) == 100:
+            command = f'{endpoint}/{Selection.Command.Results}/{id}/'
+            pr = self.perf(pr_log)
+            props = self._issue_command(command, pr)
+            packets = props if isinstance(props, dict) else {}
+        else:
+            OmniError(
+                'Failed to complete select related in a timely manner. Increase timeout')
+
+        return packets
+
+    def get_select_related_packets(self, id: int, timeout: float = 0.2) -> dict:
+        """ Get the select related packets """
+        return self.get_selection_packets(id, endpoint='select-related',
+                                          pr_log='get_select_related_packets', timeout=timeout)
+
+    def get_select_related_filter_config_packets(self, id: int, timeout: float = 0.2) -> dict:
+        """ Get the select related packets """
+        return self.get_selection_packets(id, endpoint='select-related-filter-config',
+                                          pr_log='get_select_related_filter_config_packets',
+                                          timeout=timeout)
+
     def get_session_token(self):
         """Return the current Session Token.
         """
         if 'authorization' in self._session.headers:
             token = self._session.headers['authorization']
             if len(token) > 11:
                 return token[11:]
@@ -1139,86 +1558,145 @@
         """Return the current OmniEngine Status.
         """
         pr = self.perf('get_status')
         data = self._issue_command('status/', pr)
         self._last_status = EngineStatus(self, data)
         return self._last_status
 
-    def get_token_list(self):
+    def get_settings(self) -> Optional[EngineSettings]:
+        """Gets the engine settings"""
+        if self.engine is not None:
+            command = 'settings/'
+            pr = self.engine.perf('get_settings')
+            resp = self.engine._issue_command(command, pr, EO.GET)
+            if not isinstance(resp, dict):
+                raise OmniError('Failed to get engine settings.')
+            return EngineSettings(resp)
+        return None
+
+    # def get_support_information(self) -> Optional[str]:
+    #     """Return Support Information for the OmniEngine.
+
+    #     Returns:
+    #         The Support Information text as a string.
+    #     """
+    #     return Engine(self).get_support()
+
+    def get_timeouts(self) -> EngineTimeouts:
+        """Return a list with the engine's HTTPS Connection and Request
+        timeouts in seconds."""
+        return self.timeouts
+
+    def get_token(self, id: str) -> Optional[AuthenticationToken]:
+        """ Return the token based on the ID """
+        pr = self.perf('get_token')
+        props = self._issue_command(f'token/{id}', pr)
+        return AuthenticationToken(props) if isinstance(props, dict) else None
+
+    def get_token_list(self) -> List[AuthenticationToken]:
         pr = self.perf('get_token_list')
-        props = self._issue_command('token/', pr)
-        return _create_authentication_token_list(props)
+        props = self._issue_command(AuthenticationToken.endpoint, pr)
+        return _create_authentication_token_list(props) if isinstance(props, dict) else []
+
+    def get_trace_log_level(self):
+        """Return the Trace Log logging level.
+
+        Returns:
+            Logging levels as TraceLogLevel.
+        """
+        level = TraceLogLevel.OFF
+        pr = self.perf('get_audit_logging_level')
+        props = self._issue_command('log-level/', pr)
+        if isinstance(props, dict):
+            level = props.get('logLevel')
+            if level is None:
+                raise (OmniError('Failed to get the Trace Log logging level.'))
+        return TraceLogLevel(level)
+
+    def get_user_list(self):
+        return User.get_user_list(self)
 
     def get_version(self):
         """Get the OmniEngine's version string.
-        
+
         Returns:
             The OmniEngine's version as a string.
         """
         pr = self.perf('get_version')
         props = self._issue_command('version/', pr)
         return props['engineVersion'] if isinstance(props, dict) and (
             'engineVersion' in props) else None
 
     def is_connected(self):
         """Get the connection status of the OmniEngine object.
-        
+
         Returns:
             True if OmniEngine object is connected to an OmniEngine,
             otherwise False.
         """
         return self._connected
 
-    def login(self, user, password, session_token=None):
-        """Login and connect to the OmniEngine.
+    def login(self, user, password, otp=None, session_token=None, timeouts=None):
+        """Login and connect to the OmniEngine: Account user name, Account
+        password, optional One Time Password (otp), optional Session token
+        and optional Connection timeout.
         """
+        _timeouts = (EngineTimeouts(timeouts) if timeouts is not None else self.timeouts)
         try:
             if session_token:
                 # TODO: rewrite with f-string.
                 token = ('authToken: '
-                    + session_token.decode('utf-8')).encode('utf-8')
-                self._session.headers.update({'authorization':token})
+                         + session_token.decode('utf-8')).encode('utf-8')
+                self._session.headers.update({'authorization': token})
                 status_url = f'{self._base_url}status/'
-                resp = self._session.get(status_url, verify=False)
+                resp = self._session.get(status_url, verify=False, timeouts=_timeouts.as_tuple())
                 if resp.status_code == 200:
                     self._connected = True
                     self.get_status()
                     return True
             url = f'{self._base_url}login/'
             cred_dict = {
                 'username': user,
                 'password': password,
                 'client': 'OmniScript',
                 'attempt': 0
             }
+            if otp is not None:
+                cred_dict['otp'] = otp
             credentials = json.dumps(cred_dict)
-            self._session.headers.update({'accept':'application/json'})
-            self._session.headers.update({'Content-Type':'application/json'})
-            resp = self._session.post(url, verify=False, data=credentials)
+            self._session.headers.update({'accept': 'application/json'})
+            self._session.headers.update({'Content-Type': 'application/json'})
+            resp = self._session.post(url, verify=False, data=credentials,
+                                      timeout=_timeouts.as_tuple())
             if (resp is None) or (resp.status_code != 200):
                 self.logger.debug('Could not login. Retrying')
                 retry = True
                 while retry and (cred_dict['attempts'] < 6) and (resp.status_code != 200):
                     cred_dict['attempts'] += 1
                     self.logger.debug(f'Attempt No: {cred_dict["attempts"]}')
                     credentials = json.dumps(cred_dict)
                     time.sleep(5)
-                    resp = self._session.post(url, verify=False, data=credentials)
+                    resp = self._session.post(url, verify=False, data=credentials,
+                                              timeout=_timeouts.as_tuple())
                     if resp.status_code == 200:
-                        self.logger.debug(f'Retry Succeeded after {cred_dict["attempts"]} attempts.')
+                        self.logger.debug(
+                            f'Retry Succeeded after {cred_dict["attempts"]} attempts.')
                         retry = False
                 if cred_dict['attempts'] > 5:
                     if resp.status_code == 502:
-                        self.logger.debug(f'Could not connect to engine. Please Check if engine is running and then retry. Response code : {resp.status_code}')
+                        self.logger.debug(
+                            'Could not connect to engine. Please Check if engine is running and '
+                            f'then retry. Response code : {resp.status_code}')
                     else:
-                        self.logger.debug(f'Could not connect to engine. Response code : {resp.status_code}')
+                        self.logger.debug(
+                            f'Could not connect to engine. Response code : {resp.status_code}')
                     return False
             resp_data = json.loads(resp.text)
             token = ('authToken: ' + resp_data['authToken']).encode('utf-8')
-            self._session.headers.update({'authorization':token})
+            self._session.headers.update({'authorization': token})
             self._connected = True
             self.get_status()
         except Exception as e:
             self.logger.debug(f'Exception while logging in. {e}')
         return self._connected
 
     def logout(self):
@@ -1229,41 +1707,90 @@
         if 'authorization' not in self._session.headers:
             return errors
         url = f'{self._base_url}logout/'
         token = self._session.headers['authorization'].decode('utf-8')
         # TODO: rewrite with f-string.
         data = "{\"authToken\":\"" + token + "\"}"
         try:
-            resp = self._session.post(url, verify=False, data=data)
-        except Exception as e:
+            self._session.post(url, verify=False, data=data, timeout=self.timeouts.as_tuple())
+        except Exception:
             errors.extend(['Exception while logging out'])
             self.logger.debug('Exception while logging out')
         return errors
 
+    def modify_alarm(self, alarm: Alarm) -> None:
+        """ Modify an alarm to the OmniEngine
+        """
+        pr = self.perf('modify_alarm')
+        data = json.dumps(alarm._store())
+        return self._issue_command(f'{Alarm._endpoint}{alarm.id.format()}/', pr, EO.PUT, data=data)
+
+    def modify_token(self, token: AuthenticationToken):
+        """ Modify an authentication token at the input ID """
+        pr = self.perf('modify_token')
+
+        data = json.dumps(token._modify_template())
+        self._issue_command(f'{AuthenticationToken.endpoint}{token.authentication_token_id}/',
+                            pr, EO.PUT, data=data)
+
     def perf(self, msg):
         """Log a performance message.
         """
         return self._perf_logger.perf(msg) if self._perf_logger else None
 
-    def restart(self):
-        """Request the OmniEngine to Restart itself.
-        The user will be logged off and the connection will be lost.
+    def rename_decryption_key(self, decryptkeys, name: str):
+        """ Sets the name of the DecryptionKey specified by the id.
+        Function does nothing if no key exists.
         """
-        url = f'{self._base_url}restart/'
-        try:
-            resp = self._session.post(url, verify=False)
-        except Exception as e:
-            self.logger.debug('Exception while restarting the engine.')
+        if isinstance(decryptkeys, DecryptionKey) or isinstance(decryptkeys, DecryptionKeyTemplate):
+            id = decryptkeys.id
+        else:
+            id = OmniId(decryptkeys)
+
+        pr = self.perf('rename_decryption_key')
+        data = json.dumps({"name": name})
+        return self._issue_command(f'decryption-keys/name/{id.format()}/', pr, EO.PUT, data=data)
+
+    def redirect_standard_out(self, std_out=None, std_err=None):
+        """Redirect the Standard Output and Standard Error
+        to the specified file paths.
+        """
+        pr = self.perf('redirect_standard_out')
+        req_props = {}
+        if std_out:
+            req_props['stdoutlog'] = std_out
+        if std_err:
+            req_props['stderrlog'] = std_err
+        data = json.dumps(req_props)
+        self._issue_command('log-redirect/', pr, EO.POST, data=data)
+
+    def rename_adapter(self, new_name):
+        raise OmniError('Not implemented')
 
-    def send_file(self, path):
+    # def restart(self):
+    #     """Request the OmniEngine to Restart itself.
+    #     The user will be logged off and the connection will be lost.
+    #     """
+    #     try:
+    #         return Engine(self).engine_restart()
+    #     except Exception:
+    #         self.logger.debug('Exception while restarting the engine.')
+
+    def send_email(self, email) -> Optional[SendEmailResponse]:
+        """ Send an email from the engine """
+        return Notifications(self).send_email(email)
+
+    def send_file(self, path, destination=''):
         """Send a file to the OmniEngine.
-        
+
         Args:
             path (str): name of the name of the file to send. If not fully qualified
                           then a relative path will be used.
+            destination (str): destination path. If None then engine's data
+                          directory.
 
         Returns:
             The number of bytes transfered.
         """
         if isinstance(path, PacketFileInformation):
             _path = path.path
         elif isinstance(path, FileInformation):
@@ -1274,29 +1801,157 @@
             raise OmniError(f'File not found: {_path}')
         with open(_path, 'rb') as data_file:
             data = data_file.read()
 
         p = PurePath(_path)
         kind = ''   # magic.from_file(_path, mime=True)
         req_props = {
-            'file': p.name,
+            'file': str(PurePosixPath(destination, p.name)),
             'type': kind
         }
         pr = self.perf('send_file')
-        cmd = f'files/'
+        cmd = 'files/'
         resp = self._issue_command(cmd, pr, EO.POST, params=req_props, data=data)
         count = 0
         if isinstance(resp, dict):
             count = int(resp.get('size'))
         return count
 
-    def set_filter_list_timeout(self, timeout):
-        """Set the Filter List refresh timeout in seconds.
+    def send_notifications(self, notifications) -> Optional[dict]:
+        """ Send a notification from the engine """
+        return Notifications(self).send_notifications(notifications)
+
+    def send_plugin_message(self, plugin, message=None):
+        if isinstance(plugin, AnalysisModule):
+            id = plugin.id
+        else:
+            id = OmniId(plugin)
+        pr = self.perf('plugin_message')
+        cmd = f'plugins/{str(id)}/message/'
+        data = json.dumps({
+            "data": "",
+            "message": message if message is not None else ""
+        })
+        self._issue_command(cmd, pr, EO.POST, data=data)
+
+    def set_alarm_list(self, alarms: List[Alarm]):
+        """ Update the engine's list of alarms with the input list
+        """
+        pr = self.perf('set_alarm_list')
+        props_list = [alarm._store() for alarm in alarms]
+        data = json.dumps({
+            "alarms": props_list,
+            "modificationTime": PeekTime().iso_time()
+        })
+        self._issue_command(Alarm._endpoint, pr, EO.POST, data=data)
+
+    # def set_engine_settings(self, settings: EngineSettings) -> Optional[SetSettingsResponse]:
+    #     """ Set the engine settings from the engine """
+    #     return Engine(self).set_settings(settings)
+
+    # def set_expert_prefs(self, preferences: ExpertPreferences) -> Optional[dict]:
+    #     """ Set the expert preferences from the engine """
+    #     return Engine(self).set_expert_prefs(preferences)
+
+    def set_filter_list(self, list_: List[Filter]):
+        """ Update the engine's list of filters with the input list """
+
+        if isinstance(list_, list):
+            props_list = []
+            pr = self.perf('set_filter_list')
+
+            for filter in list_:
+                props_list.append(filter.props)
+
+            data = json.dumps({
+                "filters": props_list,
+                "modificationTime": PeekTime().iso_time()
+            })
+            self._issue_command(Filter.endpoint, pr, EO.POST, data=data)
+
+    def set_license(self, license: str, source: int = 1):
+        """ Set the license of the engine. Will cause a restart """
+        pr = self.perf('set_license')
+        data = json.dumps({
+            'data': license,
+            'source': source
+        })
+        self._issue_command(License.endpoint, pr, EO.POST, data=data)
+
+    def set_license_settings(self, settings: dict):
+        """ Set the license settings of the engine """
+        pr = self.perf('set_license_settings')
+        data = json.dumps(settings)
+        self._issue_command(LicenseSettings.endpoint, pr, EO.POST, data=data)
+
+    def set_liveflow_configuration(self, liveflowConfig: LiveFlowConfiguration) -> (
+            Optional[LiveFlowConfigurationResponse]):
+        """ Set the liveflow configuration on the engine """
+        return LiveFlow(self).set_liveflow_configuration(liveflowConfig)
+
+    def set_notification(self, notificationId, notifications) -> Optional[dict]:
+        """ Set the notification from the engine """
+        return Notifications(self).set_notification(notificationId, notifications)
+
+    def set_notifications(self, notifications) -> Optional[dict]:
+        """ Set the notifications from the engine """
+        return Notifications(self).set_notifications(notifications)
+
+    def set_protocol_translations_list(self, list_: List[PT]):
+        """ Update the engine's list of translations with the input list """
+        props_list = []
+
+        if isinstance(list_, list):
+            pr = self.perf('set_protocol_translations_list')
+
+            for translation in list_:
+                props_list.append(translation.props)
+
+        data = json.dumps({
+            "protocolTranslations": props_list
+        })
+        self._issue_command(PT.endpoint, pr, EO.POST, data=data)
+
+    def set_settings(self, settings: EngineSettings) -> Optional[SetSettingsResponse]:
+        """Sets the engine settings"""
+        if self.engine is not None:
+            command = 'settings/'
+            pr = self.engine.perf('set_settings')
+            resp = self.engine._issue_command(command, pr, EO.POST,
+                                              data=json.dumps(settings, cls=OmniScriptEncoder))
+            if not isinstance(resp, dict):
+                raise OmniError('Failed to set engine settings.')
+            return SetSettingsResponse(resp)
+        return None
+
+    def set_timeouts(self, connection_timeout: Union[int, float],
+                     request_timeout: Optional[Union[int, float]]) -> EngineTimeouts:
+        """Set the timeout values for HTTP Connection and Timeout in seconds.
+        If the connection_timeout is less then zero or None, then the
+        connection_timeout value is not changed.
+        If the request_timeout is less then zero or None, then the
+        request_timeout is set to the connection_timeout.
+        """
+        if connection_timeout is not None and connection_timeout >= 0:
+            self.timeouts.set_connection(connection_timeout)
+        if request_timeout is not None and request_timeout >= 0:
+            self.timeouts.set_request(request_timeout)
+        else:
+            self.timeouts.set_request(self.timeouts.connection)
+        return self.timeouts
+
+    def set_trace_log_level(self, level):
+        """Set the Trace Log logging level.
         """
-        self._filter_timeout = int(timeout) * 1000000000    # to nanoseconds.
+        pr = self.perf('set_trace_log_level')
+        req_props = {
+            'logLevel': int(level)
+        }
+        data = json.dumps(req_props)
+        self._issue_command('log-level/', pr, EO.POST, data=data)
 
     def start_capture(self, capture, retry=3):
         """Signal a Capture, or list of Captures, to begin
         capturing packets.
 
         Args:
             capture (str,
@@ -1306,29 +1961,68 @@
             Or a list of captures.
         """
         ids = _capture_id_list(capture)
         for id in ids:
             pr = self.perf('start_capture')
             command = f'running-captures/{id.format()}/'
             props = self._issue_command(command, pr, EO.POST)
-            if not _almost_success(props):
+            if not is_almost_success(props):
                 raise OmniError('Command failed: 0x80004005')
 
     def start_performance_logging(self, filename, mode='a'):
         """Start loggin the time it takes for the OmniEngine to perform
         each command.
 
         Args:
             filename: the name of the file to write the log entries.
             mode: open the file in append 'a', or create/overwrite 'c'.
         """
         if self._perf_logger:
             self.stop_performance_logging()
         self._perf_logger = PerformanceLogger(filename, mode)
 
+    def start_selection(self, id: Union[str, OmniId], pr_log: str, endpoint: str,
+                        data: Optional[str] = None, params=None) -> Optional[Selection]:
+        """ Shared helper for starting select related operations """
+        pr = self.perf(pr_log)
+        select_id = id.get_id() if isinstance(id, OmniId) else id
+        command = f'{endpoint}/start/{select_id}/'
+        resp = self._issue_command(
+            command, pr, EO.POST, data=data, params=params)
+
+        return Selection(resp) if isinstance(resp, dict) else None
+
+    def start_select_related(
+            self, id: Union[str, OmniId], packets: List[int], prefer_logical_addr: bool,
+            select_related_by: int) -> Optional[Selection]:
+        """ Starts a select related operation for the specified capture or search on the engine """
+        data = json.dumps({
+            'packets': packets,
+            'preferLogicalAddress': prefer_logical_addr,
+            'selectRelatedBy': select_related_by
+        })
+
+        return self.start_selection(id, pr_log='start_select_related',
+                                    endpoint='select-related', data=data)
+
+    def start_select_related_filter_config(self, id: Union[str, OmniId], filters: List[Filter],
+                                           mode: int, first_packet_number: int,
+                                           last_packet_number: int) -> Optional[Selection]:
+        """ Starts a select related operation using a pre-defined filter configuration """
+        data = json.dumps({
+            'filters': [filter.UUID for filter in filters],
+            'mode': mode
+        })
+        params = [('firstPacketNumber', first_packet_number),
+                  ('lastPacketNumber', last_packet_number)]
+
+        return self.start_selection(id, pr_log='start_select_related_filter_config',
+                                    endpoint='select-related-filter-config', data=data,
+                                    params=params)
+
     def stop_capture(self, capture, retry=3):
         """Signal a Capture, or list of Captures, to
         stop capturing packets.
 
         Args:
             capture (str,
             :class:`OmniId <omniscript.omniid.OmniId>` or
@@ -1337,15 +2031,15 @@
             Or a list of captures.
         """
         ids = _capture_id_list(capture)
         for id in ids:
             pr = self.perf('stop_capture')
             command = f'running-captures/{id.format()}/'
             props = self._issue_command(command, pr, EO.DELETE)
-            if not _almost_success(props):
+            if not is_almost_success(props):
                 raise OmniError('Command failed: 0x80004005')
 
     def stop_performance_logging(self):
         """Stop Performance Logging.
         """
         if self._perf_logger:
             self._perf_logger = None
@@ -1359,8 +2053,11 @@
         if isinstance(template, CaptureTemplate):
             t = template.store()
         else:
             raise ValueError('A CaptureTemplate is required.')
         pr = self.perf('update_capture_template')
         cmd = f'capture-templates/{template.id.format()}/'
         resp = self._issue_command(cmd, pr, EO.PUT, data=t)
-        return _success(resp)
+        return is_success(resp)
+
+    def update_remote_engine(self, remote):
+        return remote.update(self, remote)
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/omnierror.py` & `omniscript-liveaction-3.0.49/src/omniscript/omnierror.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ﻿"""OmniError class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 
 class OmniError(Exception):
     """The exception class raised by OmniScript methods.
     """
 
     code = 0
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/omniid.py` & `omniscript-liveaction-3.0.49/src/omniscript/omniid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 ﻿"""OmniId class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 import six
 import uuid
 
-from .invariant import (ID_FLAG_NONE, ID_FLAG_NO_BRACES, ID_FLAG_BRACES,
-    ID_FLAG_LOWERCASE, ID_FLAG_UPPERCASE)
+from .invariant import ID_FLAG_NONE, ID_FLAG_BRACES, ID_FLAG_LOWERCASE
 
 
 class OmniId(object):
     """A uuid.UUID with a default string format:
     {ABCDEF01-2345-6789-ABCD-0123456789AB}
     """
 
@@ -57,15 +56,15 @@
     def __hash__(self):
         return self.id.__hash__()
 
     def __repr__(self):
         return f'{self.__class__.__name__}("{self.id}")'
 
     def __str__(self):
-        return f'{{{str(self.id).upper()}}}' if self.id else ''
+        return f'{(str(self.id)).upper()}' if self.id else ''
 
     def bytes_le(self):
         """Return the id as a 16-byte string in little-endian format"""
         return self.id.bytes_le
 
     def format(self, flags=ID_FLAG_NONE):
         """Return the id as a string with formatting based on flags.
@@ -89,20 +88,26 @@
 
     @staticmethod
     def is_id(value):
         if isinstance(value, OmniId):
             return True
         if isinstance(value, six.string_types):
             if len(value) == 38:
-                if value[0] != '{': return False
-                if value[9] != '-': return False
-                if value[14] != '-': return False
-                if value[19] != '-': return False
-                if value[24] != '-': return False
-                if value[37] != '}': return False
+                if value[0] != '{':
+                    return False
+                if value[9] != '-':
+                    return False
+                if value[14] != '-':
+                    return False
+                if value[19] != '-':
+                    return False
+                if value[24] != '-':
+                    return False
+                if value[37] != '}':
+                    return False
                 return True
         return False
 
     def parse(self, value):
         """Parse the value into the id."""
         self.id = uuid.UUID(value)
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/omniport.py` & `omniscript-liveaction-3.0.49/src/omniscript/omniport.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 ﻿"""OmniPort classes.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 import six
 import xml.etree.ElementTree as ET
 
-import omniscript
-
 from .invariant import PORT_TYPE_IP
 
 
 class PortRange(object):
     """A range of ports."""
 
     min = 0
@@ -35,33 +33,33 @@
             self.min, self.max = value, None
         elif isinstance(value, six.string_types):
             items = value.split('-')
             if len(items) == 1:
                 self.min, self.max = int(items[0]), None
             elif len(items) == 2:
                 self.min, self.max = int(items[0]), int(items[1])
-                      
+
 
 class OmniPort(object):
     """The OmniPort class."""
 
     _mask = 0xC0000000
     """The mask value for _storing the port."""
 
     port_type = PORT_TYPE_IP
     """The type of port. One of the PORT TYPE constants.
     Default is PORT_TYPE_IP.
     """
 
     port = None
     """The port and/or port-range list."""
-    
+
     def __init__(self, port=None):
         self._mask = OmniPort._mask
-        self.port_type = omniscript.PORT_TYPE_IP
+        self.port_type = PORT_TYPE_IP
         self.port = []
         if isinstance(port, int):
             self.port.append(port)
         elif isinstance(port, six.string_types):
             items = port.split()
             for item in items:
                 self.port.append(PortRange(item))
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/omniscript.py` & `omniscript-liveaction-3.0.49/src/omniscript/omniscript.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 """OmniScript class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 # pylint: disable-msg=w0614
 
-VERSION = "3.0"
-MIN_PYTHON = "3.8"
-
 import os
 import logging
-import urllib3
 import xml.etree.ElementTree as ET
 
-from .invariant import (DEFAULT_PORT, OMNI_FLAG_NO_HTTPS_WARNINGS, WIRELESS_BAND_ALL,
-    WIRELESS_BAND_GENERIC, WIRELESS_BAND_B, WIRELESS_BAND_A, WIRELESS_BAND_G, WIRELESS_BAND_N,
-    WIRELESS_BAND_TURBOA, WIRELESS_BAND_TURBOG, WIRELESS_BAND_SUPERG, WIRELESS_BAND_LICENSEDA1MHZ,
+from typing import Optional, Union
+from urllib3 import disable_warnings
+from .invariant import (
+    DEFAULT_PORT, OMNI_FLAG_NO_HTTPS_WARNINGS, WIRELESS_BAND_ALL, WIRELESS_BAND_GENERIC,
+    WIRELESS_BAND_B, WIRELESS_BAND_A, WIRELESS_BAND_G, WIRELESS_BAND_N, WIRELESS_BAND_TURBOA,
+    WIRELESS_BAND_TURBOG, WIRELESS_BAND_SUPERG, WIRELESS_BAND_LICENSEDA1MHZ,
     WIRELESS_BAND_LICENSEDA5MHZ, WIRELESS_BAND_LICENSEDA10MHZ, WIRELESS_BAND_LICENSEDA15MHZ,
     WIRELESS_BAND_LICENSEDA20MHZ, WIRELESS_BAND_PRIMARYAC0, WIRELESS_BAND_PRIMARYAC1,
     WIRELESS_BAND_PRIMARYAC2, WIRELESS_BAND_PRIMARYAC3, WIRELESS_BAND_UNKNOWN5,
-    WIRELESS_BAND_UNKNOWN6, WIRELESS_BAND_UNKNOWN7, WIRELESS_BAND_UNKNOWN8,
-    WIRELESS_BAND_UNKNOWN9, WIRELESS_BAND_N20MHZ, WIRELESS_BAND_N40MHZ, WIRELESS_BAND_N40MHZLOW,
-    WIRELESS_BAND_N40MHZHIGH)
+    WIRELESS_BAND_UNKNOWN6, WIRELESS_BAND_UNKNOWN7, WIRELESS_BAND_UNKNOWN8, WIRELESS_BAND_UNKNOWN9,
+    WIRELESS_BAND_N20MHZ, WIRELESS_BAND_N40MHZ, WIRELESS_BAND_N40MHZLOW, WIRELESS_BAND_N40MHZHIGH)
 
-from .omniengine import OmniEngine
+from .omniengine import OmniEngine, EngineTimeouts
 from .omniid import OmniId
-from .omniengine import find_capture, find_capture_template
 from .peektime import PeekTime
 
+__version__ = "3.0.0"
+__build__ = "1"
 
 # Dictionary of OmniId (GUID) to class name.
 _id_class_names = None
 
 # Dictionary of class name to OmniId (GUID).
 _class_name_ids = None
 
+# Dictionary of OmniId (GUID) to capability name.
+_id_capability_name = None
+
 # Dictionary of country names to codes.
 _co_name_codes = None
 
 # Dictionary of Expert Problem label to id.
 _expert_problem_id = None
 
 # Dictionary of OmniId (GUID) to expert description.
@@ -97,35 +102,44 @@
         for sub_spec in spec.iter('PSpec'):
             id = sub_spec.find('PSpecID')
             if id is not None:
                 name = sub_spec.attrib['Name']
                 index = int(id.text)
                 id_protocol_names[index] = name
                 sname = sub_spec.find('SName')
-                id_protocol_short_names[index] = sname.text \
-                    if sname is not None else name
+                id_protocol_short_names[index] = sname.text if sname is not None else name
     else:
         id = spec.find('PSpecID')
         if id is not None:
             name = spec.attrib['Name']
             index = int(id.text)
             id_protocol_names[index] = name
             sname = spec.find('SName')
-            id_protocol_short_names[index] = sname.text \
-                if sname is not None else name
+            id_protocol_short_names[index] = sname.text if sname is not None else name
+
+
+def _load_capability_ids():
+    id_capability_names = {}
+    _dirname = os.path.dirname(__file__)
+    with open(os.path.join(_dirname, 'data', '_capability_ids.txt'), 'r') as clsdct:
+        for line in clsdct:
+            if len(line) > 0:
+                k, v = line.split(' ', 1)
+                id_capability_names[OmniId(k)] = v.strip()
+    return id_capability_names
 
 
 def _load_class_ids():
     id_class_names = {}
     _dirname = os.path.dirname(__file__)
     with open(os.path.join(_dirname, 'data', '_class_ids.txt'), 'r') as clsdct:
         for line in clsdct:
-          if len(line) > 0:
-              k, v = line.split(' ', 1)
-              id_class_names[OmniId(k)] = v.strip()
+            if len(line) > 0:
+                k, v = line.split(' ', 1)
+                id_class_names[OmniId(k)] = v.strip()
     return id_class_names
 
 
 def _load_expert_names():
     id_expert_names = {}
     _dirname = os.path.dirname(__file__)
     experts = ET.parse(os.path.join(_dirname, 'data', 'expertdescriptions.xml'))
@@ -145,18 +159,18 @@
 
 def _load_expert_problems():
     expert_problem_id = {}
     expert_problem_id[''] = 0
     _dirname = os.path.dirname(__file__)
     with open(os.path.join(_dirname, 'data', '_expert_problem_ids.txt'), 'r') as exproblems:
         for raw_line in exproblems:
-          line = raw_line.strip()
-          if len(line) > 0:
-              v, k = line.split(' ', 1) # note: value, key (18 'DNS Error')
-              expert_problem_id[k.strip('\'')] = int(v)
+            line = raw_line.strip()
+            if len(line) > 0:
+                v, k = line.split(' ', 1)  # note: value, key (18 'DNS Error')
+                expert_problem_id[k.strip('\'')] = int(v)
     return expert_problem_id
 
 
 def _load_pspecs():
     id_protocol_names = {}
     id_protocol_short_names = {}
     _dirname = os.path.dirname(__file__)
@@ -182,41 +196,52 @@
     """Returns a dictionary with the key being the string name of a class
     and the value the :class:`OmniId <omniscript.omniid.OmniId>` GUID of the class.
     """
     global _class_name_ids
     if _class_name_ids is None:
         id_names = get_id_class_names()
         if id_names is not None:
-            _class_name_ids = dict((v,k) for k,v in id_names.items())
+            _class_name_ids = dict((v, k) for k, v in id_names.items())
     return _class_name_ids
 
 
 def get_expert_problem_id():
-    """Returns a dictionary with the key being a string of the 
+    """Returns a dictionary with the key being a string of the
     Expert Problem label and the value is the integer problem id.
     """
     global _expert_problem_id
     if _expert_problem_id is None:
         _expert_problem_id = _load_expert_problems()
     return _expert_problem_id
 
 
+def get_id_capability_names():
+    """Returns a dictionary with the key being the
+    :class:`OmniId <omniscript.omniid.OmniId>` GUID of an engine
+    capability and the value the string name of the capability.
+    """
+    global _id_capability_name
+    if _id_capability_name is None:
+        _id_capability_name = _load_capability_ids()
+    return _id_capability_name
+
+
 def get_id_class_names():
-    """Returns a dictionary with the key being the 
+    """Returns a dictionary with the key being the
     :class:`OmniId <omniscript.omniid.OmniId>` GUID of a class
     and the value the string name of the class.
     """
     global _id_class_names
     if _id_class_names is None:
         _id_class_names = _load_class_ids()
     return _id_class_names
 
 
 def get_id_expert_names():
-    """Returns a dictionary with the key being the 
+    """Returns a dictionary with the key being the
     :class:`OmniId <omniscript.omniid.OmniId>` GUID of a class
     and the value the string name of the expert.
     """
     global _id_expert_names
     if _id_expert_names is None:
         _id_expert_names = _load_expert_names()
     return _id_expert_names
@@ -268,15 +293,15 @@
     """Returns a dictionary with the key being the string short name of
     a protocol and the value the :class:`OmniId <omniscript.omniid.OmniId>`
     GUID of the protocol.
     """
     global _protocol_short_name_ids
     if _protocol_short_name_ids is None:
         id_names = get_id_protocol_short_names()
-        _protocol_short_name_ids = dict((v,k) for k,v in id_names.items())
+        _protocol_short_name_ids = dict((v, k) for k, v in id_names.items())
     return _protocol_short_name_ids
 
 
 def get_wireless_band_id_names():
     """Returns a dictionary with the names of the wireless bands."""
     # global _wireless_band_id_names
     return _wireless_band_id_names
@@ -309,15 +334,15 @@
 
 
 class OmniScript(object):
     """The OmniScript class is used to connect to an OmniEngine."""
 
     def __init__(self, level=logging.INFO, flags=OMNI_FLAG_NO_HTTPS_WARNINGS):
         if flags & OMNI_FLAG_NO_HTTPS_WARNINGS:
-            urllib3.disable_warnings()
+            disable_warnings()
 
         # Logging
         self.logger = logging.getLogger('OmniScript')
         self.logger.setLevel(level)
         self._console_handler = logging.StreamHandler()
         self._console_handler.setLevel(level)
         self._console_formatter = LogFormatter()
@@ -332,53 +357,57 @@
 
     def __str__(self):
         return 'OmniScript'
 
     def __setitem__(self, key, item):
         self.__dict__[key] = item
 
-    def connect(self, host = 'localhost', port = 80, auth = 'Default',
-                domain = '', user = '', password = '', timeout = 30000):
-        """Estabilish a connection to an OmniEngine.
-
-        Args:
-            host (str): the IP Address or name of the system hosting
-            the OmniEngine.
-            port (int): the IP Port of the OmniEngine.
-            auth (str): the authorization type: Default or Third Party.
-            domain (str): the domain of the user's account.
-            user (str): the name of the user's account.
-            password (str): the password of the user's account.
-            timeout (int): the timeout in milliseconds. Default is
-            30 seconds.
-
-        Returns:
-            An
-            :class:`OmniEngine <omniscript.omniengine.OmniEngine>`
-            object.
-        """
-        try:
-            engine = self.create_engine(host, port)
-            if engine:
-                engine.login(user, password)
-        except RuntimeError:
-            self.logger.error('Engine is off-line or inaccessible.')
-            return None
-        return engine
-
-    def create_engine(self, host='localhost', port=DEFAULT_PORT, secure=True):
+    # def connect(self, host = 'localhost', port = 80, auth = 'Default',
+    #             domain = '', user = '', password = '', timeout = 30000):
+    #     """Estabilish a connection to an OmniEngine.
+
+    #     Args:
+    #         host (str): the IP Address or name of the system hosting
+    #         the OmniEngine.
+    #         port (int): the IP Port of the OmniEngine.
+    #         auth (str): the authorization type: Default or Third Party.
+    #         domain (str): the domain of the user's account.
+    #         user (str): the name of the user's account.
+    #         password (str): the password of the user's account.
+    #         timeout (int): the timeout in milliseconds. Default is
+    #         30 seconds.
+
+    #     Returns:
+    #         An
+    #         :class:`OmniEngine <omniscript.omniengine.OmniEngine>`
+    #         object.
+    #     """
+    #     try:
+    #         engine = self.create_engine(host, port)
+    #         if engine:
+    #             engine.login(user, password)
+    #     except RuntimeError:
+    #         self.logger.error('Engine is off-line or inaccessible.')
+    #         return None
+    #     return engine
+
+    def create_engine(self, host: str = 'localhost', port: int = DEFAULT_PORT,
+                      secure: bool = True,
+                      timeouts: Optional[Union[EngineTimeouts, str, list]] = None):
         """Create an OmniEngine object.
 
         Args:
             host (str): the IP Address or name of the system hosting
             the OmniEngine.
             port (int): the IP Port of the OmniEngine.
             secure (boolean): use https when true, otherwise use http.
+            timeouts (EngineTimeouts, string, list): the HTTP Connection and
+            requests timeouts in seconds.
         """
-        return OmniEngine(self, host, port, secure)
+        return OmniEngine(self, host, port, secure, timeouts)
 
     def critical(self, msg, *args, **kwargs):
         """Log a critical message."""
         self.logger.critical(msg, *args, **kwargs)
 
     def error(self, msg, *args, **kwargs):
         """Log an error message."""
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/packet.py` & `omniscript-liveaction-3.0.49/src/omniscript/packet.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ﻿"""Packet class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 import six
 
 import omniscript
 
 from .omniaddress import EthernetAddress, IPv4Address
-from .omnierror import OmniError
+from .country import Country
 from .omniport import OmniPort
 from .peektime import PeekTime
 # from .readstream import ReadStream
 
 # from .omniscript import get_id_protocol_names
 
 
@@ -77,29 +77,29 @@
     'wanDirection': 'wan_direction',
     'wirelessChannel': 'wireless_channel'
 }
 
 
 class Packet(object):
     """The Packet class has packet information.
-    The 
-    :func:`get_packets() 
+    The
+    :func:`get_packets()
     <omniscript.capture.Capture.get_packets>`
     function returns a list of Packet objects.
 
     Packet number vs index: the packet number, which starts at 0, is a
     counter of the packets as they are captured. When a packet is
     captured the packet counter becomes the packet number of the packet
     and then the packet counter is incremented.
     The packet index is the index into the list of packets called the
     packet buffer.
     The first index in the packet buffer is 0. The first packet in the
     packet buffer, index 0, always contains the packet with the lowest
     packet number.
-    
+
     A capture buffer can only hold a finite number of packets. Once
     the buffer  has filled and a new packet is captured then the
     first packet in the packet buffer (index 0) is deleted makeing what
     was the second packet (index 1) into the first packet (index 0).
     And the newly captured packet becomes the last packet in the buffer.
 
     The first_packet attribute of a
@@ -116,195 +116,249 @@
     address_3 = None
     """The third address.."""
 
     address_4 = None
     """The fourth address.."""
 
     application = ''
+    """The application."""
 
     application_id = ''
+    """The application identifier."""
 
     application_color = ''
+    """The application color."""
 
     band = ''
-    """   """
+    """The band."""
 
     bssid = ''
-    """   """
+    """The BSSID."""
 
     data = None
     """The packet data."""
 
     data_rate = 0
-    """   """
+    """The data rate."""
 
     date = None
-    """   """
+    """The packet data."""
 
     delta_time = None
-    """   """
+    """How long it's been since the previous packet."""
 
     destination = ''
-    """Physical desination MAC Address."""
+    """Physical desination Ehternet Address."""
 
     destination_city = ''
-    """   """
+    """The destination city of based on Destination Address."""
 
-    destination_country = ''
-    """   """
+    destination_country = None
+    """The destination country of based on Destination Address."""
 
     destination_latitude = ''
-    """   """
+    """The destination latitude based on Destination Address."""
 
     destination_logical = ''
-    """   """
+    """The logical destination address."""
 
     destination_longitude = ''
-    """   """
+    """The destination longitude based on Destination Address."""
 
     destination_physical = None
-    """   """
+    """The physical destination address."""
 
     destination_port = None
-    """   """
+    """The destination port."""
 
     expert = ''
-    """   """
+    """The ExpertEvent triggered by this packet."""
 
     filter = ''
-    """   """
+    """The Filter used to accept this packet."""
 
     flags = None
-    """   """
+    """The flags."""
 
     flags80211 = ''
-    """   """
+    """The Wireless flags."""
 
     flow_id = 0
-    """   """
+    """The identifier of the flow this packet is in."""
 
     frequency = ''
-    """   """
+    """The frequency the packet was captured at."""
 
     full_duplex_channel = ''
-    """   """
+    """The full duplex channel the packet was captured on."""
 
     index = 0
     """The packet's index from the starting of the capture buffer."""
 
     ip_identifier = ''
-    """   """
+    """The IP Identifier of the packet."""
 
     ip_length = 0
-    """   """
+    """The length of the IP poertion of the packet."""
 
     ip_ttl = ''
-    """   """
+    """The Time To Live (TTL) of the packet."""
 
     mcs = ''
-    """   """
+    """The MCS of the packet."""
 
     mpls = ''
-    """   """
+    """The MPLS Label of the packet."""
 
     noise_dbm = ''
-    """   """
+    """The noise level in decibals the packet was captured."""
 
     noise_strength = ''
-    """   """
+    """The strength of the noise the packet was captured at."""
 
     number = 0
     """The packet's number starting from when the capture starts."""
 
     packet_length = 0
-    """   """
+    """The length in bytes of the packet."""
 
     protocol = ''
     """The packet's protocol."""
 
     receiver = ''
-    """   """
+    """The address of the packet's receiver."""
 
     relative_time = None
-    """   """
+    """The amount of time since the Capture was started."""
 
     signal_dbm = ''
-    """   """
+    """The quality of the wireless signal in decibels."""
 
     signal_strength = ''
-    """   """
+    """The strength of the wireless signal when the packet was captured."""
 
     size_bar = ''
-    """   """
+    """The size bar of the packet."""
 
     source = ''
     """Physical source MAC Address."""
 
     source_city = ''
-    """   """
+    """The source city of based on Source Address."""
 
-    source_country = ''
-    """   """
+    source_country = None
+    """The source country of based on Source Address."""
 
     source_latitude = ''
-    """   """
+    """The source latitude of based on Source Address."""
 
     source_logical = ''
-    """   """
+    """The logical value of the Source Address."""
 
     source_longitude = ''
-    """   """
+    """The source longitude of the Source Address."""
 
     source_physical = ''
-    """   """
+    """The source physical of based on Source Address."""
 
     source_port = ''
-    """   """
+    """The source port of based on Source Address."""
 
     spatial_streams = ''
-    """   """
+    """The spatial streams of the packet."""
 
     status = 0
     """The packet's status."""
 
     summary = ''
-    """   """
+    """The Summary Information of the packet."""
 
     summary_source = ''
-    """   """
+    """The source of the summary attribute."""
 
     timestamp = None
     """The packet's timestamp as
     :class:`PeekTime <omniscript.peektime.PeekTime>`.
     """
 
     transmitter = ''
-    """   """
+    """The address of the wireless transmitter."""
 
     vlan = ''
-    """   """
+    """The VLAN the packet is on."""
 
     wan_direction = ''
-    """   """
+    """The direction of the packet: to server, or from server."""
 
     wireless_channel = ''
-    """   """
+    """The wireless channel the packet was captured on."""
 
     def __init__(self, number=None, props=None, data=None):
         self.number = number if number and (number > 0) else Packet.number
+        self.address_1 = Packet.address_1
+        self.address_2 = Packet.address_2
+        self.address_3 = Packet.address_3
+        self.address_4 = Packet.address_4
         self.application = Packet.application
+        self.application_id = Packet.application_id
+        self.application_color = Packet.application_color
+        self.band = Packet.band
+        self.bssid = Packet.bssid
         self.data = Packet.data
-        self.packet_length = Packet.packet_length
+        self.data_rate = Packet.data_rate
+        self.date = Packet.date
+        self.delta_time = Packet.delta_time
+        self.destination = Packet.destination
+        self.destination_city = Packet.destination_city
+        self.destination_country = Packet.destination_country
+        self.destination_latitude = Packet.destination_latitude
+        self.destination_logical = Packet.destination_logical
+        self.destination_longitude = Packet.destination_longitude
+        self.destination_physical = Packet.destination_physical
+        self.destination_port = Packet.destination_port
+        self.expert = Packet.expert
+        self.filter = Packet.filter
         self.flags = Packet.flags
+        self.flags80211 = Packet.flags80211
         self.flow_id = Packet.flow_id
+        self.frequency = Packet.frequency
+        self.full_duplex_channel = Packet.full_duplex_channel
+        self.index = Packet.index
+        self.ip_identifier = Packet.ip_identifier
+        self.ip_length = Packet.ip_length
+        self.ip_ttl = Packet.ip_ttl
+        self.mcs = Packet.mcs
+        self.mpls = Packet.mpls
+        self.noise_dbm = Packet.noise_dbm
+        self.noise_strength = Packet.noise_strength
+        self.number = Packet.number
         self.packet_length = Packet.packet_length
         self.protocol = Packet.protocol
+        self.receiver = Packet.receiver
+        self.relative_time = Packet.relative_time
+        self.signal_dbm = Packet.signal_dbm
+        self.signal_strength = Packet.signal_strength
+        self.size_bar = Packet.size_bar
+        self.source = Packet.source
+        self.source_city = Packet.source_city
+        self.source_country = Packet.source_country
+        self.source_latitude = Packet.source_latitude
+        self.source_logical = Packet.source_logical
+        self.source_longitude = Packet.source_longitude
+        self.source_physical = Packet.source_physical
+        self.source_port = Packet.source_port
+        self.spatial_streams = Packet.spatial_streams
         self.status = Packet.status
-        self.timestamp = None
-        self.data = Packet.data
+        self.summary = Packet.summary
+        self.summary_source = Packet.summary_source
+        self.timestamp = Packet.timestamp
+        self.transmitter = Packet.transmitter
+        self.vlan = Packet.vlan
+        self.wan_direction = Packet.wan_direction
+        self.wireless_channel = Packet.wireless_channel
         self._load(props)
         self._load_data(data)
 
     def __repr__(self) -> str:
         return f'Packet: {self.index}'
 
     def __str__(self) -> str:
@@ -324,30 +378,32 @@
     def get_prop_dict(cls):
         return _packet_prop_dict
 
     def _load(self, props):
         """Set attributes from a dictionary."""
         if isinstance(props, dict):
             missed = 0
-            for k,v in props.items():
+            for k, v in props.items():
                 a = _packet_prop_dict.get(k)
                 if a is None or not hasattr(self, a):
                     continue
                 if isinstance(getattr(self, a), six.string_types):
                     setattr(self, a, v if v else '')
                 elif isinstance(getattr(self, a), int):
                     setattr(self, a, int(v) if v else 0)
                 elif getattr(self, a) is None:
                     if a in ('address_1', 'address_2', 'address_3', 'address_4', 'destination',
-                                'destination_logical', 'destination_physical', 'source',
-                                'source_logical', 'source_physical'):
+                             'destination_logical', 'destination_physical', 'source',
+                             'source_logical', 'source_physical'):
                         try:
                             setattr(self, a, EthernetAddress(v) if v else None)
-                        except:
+                        except Exception:
                             setattr(self, a, v)
+                    elif a in ('destination_country', 'source_country'):
+                        setattr(self, a, Country(v))
                     elif a in ('destination_logical', 'source_logical'):
                         setattr(self, a, IPv4Address(v) if v else None)
                     elif a in ('destination_port', 'source_port'):
                         setattr(self, a, OmniPort(v) if v else None)
                     elif a in ('date', 'delta_time', 'relative_time', 'timestamp'):
                         setattr(self, a, PeekTime(v) if v else None)
                     elif a == 'flags':
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/packetfileinformation.py` & `omniscript-liveaction-3.0.49/src/omniscript/packetfileinformation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 ﻿"""PacketFileInformation class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
-import six
-
-from .invariant import FILE_FLAGS_DIRECTORY
 from .omniid import OmniId
 from .peektime import PeekTime
 
 
 class PacketFileInformation(object):
     """Information about a Packet File.
     """
@@ -142,15 +139,15 @@
         self.status = PacketFileInformation.status
         self.time_zone_bias = PacketFileInformation.time_zone_bias
         self._load(props)
 
     def _load(self, props):
         """Load the File Informaiont from a dictionary."""
         if isinstance(props, dict):
-            for k,v in props.items():
+            for k, v in props.items():
                 a = PacketFileInformation._pfi_prop_dict.get(k)
                 if a is not None and hasattr(self, a):
                     if a == PacketFileInformation._tag_adapter_address:
                         self.adapter_address = v
                     elif a == PacketFileInformation._tag_adapter_name:
                         self.adapter_name = v
                     elif a == PacketFileInformation._tag_capture_id:
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/peektime.py` & `omniscript-liveaction-3.0.49/src/omniscript/peektime.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 ﻿"""PeekTime class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 import six
 import time
 
 from datetime import datetime, timezone
-from .invariant import (MINUTES_PER_HOUR, NANOSECONDS_PER_SECOND, SECONDS_PER_DAY,
-    SECONDS_PER_HOUR, SECONDS_PER_MINUTE, TIME_FLAGS_NONE, TIME_FLAGS_NANOSECONDS)
+from .invariant import (
+    NANOSECONDS_PER_SECOND, SECONDS_PER_HOUR, SECONDS_PER_MINUTE, SECONDS_PER_DAY,
+    TIME_FLAGS_NANOSECONDS)
 
 
 # Convert from Ansi time (seconds) to Peek Time (nanoseconds).
 ANSI_TIME_MULTIPLIER = 1000000000
 # The adjustment in seconds (Ansi Time), seconds between 1/1/1601 and 1/1/1970.
 ANSI_TIME_ADJUSTMENT = 11644473600
 
@@ -23,15 +24,15 @@
 UNIX_EPOCH_DELTA = 719468   # Wolfram Alpha: days between 03/01/0000 to 1/1/1601
 PEEK_EPOCH_DELTA = 584694   # Wolfram Alpha: days between 03/01/0000 to 1/1/1970
 
 
 class PeekTime(object):
     """Peek Time is the number of nanoseconds since
     midnight January 1, 1601.
-    
+
     PeekTime(), with no arguments is set to the current date and time.
     PeekTime(int), uses the integer as the value in nanoseconds.
     PeekTime(string), either ISO 8601, or the number of nanoseconds.
     PeekTime(PeekTime), copies the value of the other PeekTime.
     """
 
     value = 0
@@ -85,77 +86,77 @@
 
     @classmethod
     def parse_8601(cls, value):
         """A Class method that parses an ISO-8601 timestamep and returns the
         number of nanoseconds in UTC since 1/1/1601.
         """
         if not isinstance(value, six.string_types):
-            raise(Exception('The value to parse must be a string.'))
+            raise (Exception('The value to parse must be a string.'))
         if not value:
             return 0
         if 'T' not in value:
-            raise(Exception('The value must contain a "T".'))
+            raise (Exception('The value must contain a "T".'))
 
         ns = 0
         date_secs = time_secs = 0
         _date, _remaining = value.split('T')
         if '-' in _date:
             _date_split = _date.split('-')
             if len(_date_split) != 3:
-                raise(Exception('Insufficent separators in date portion.'))
+                raise (Exception('Insufficent separators in date portion.'))
 
             year, month, day = _date_split
             _days = PeekTime.days_from_date(int(year), int(month), int(day))
             date_secs = _days * (24 * 60 * 60)
 
-        if '.' not in _remaining:
-            raise(Exception('The time portion must contains a ".".'))
-        
-        _remaining_split = _remaining.split('.')
-        if len(_remaining_split) != 2:
-            raise(Exception('The seconds portion must contain two parts.'))
+        time_zone_minutes = 0
+        if 'Z' in _remaining:
+            zone_split = _remaining.split('Z')
+        elif '-' in _remaining:
+            zone_split = _remaining.split('-')
+            time_zone_minutes = 1
+        elif '+' in _remaining:
+            zone_split = _remaining.split('+')
+            time_zone_minutes = -1
+        else:
+            zone_split = [_remaining, '']
+
+        if len(zone_split) != 2:
+            raise (Exception('If a timezone offset is specified it must contain 2 parts.'))
+
+        _full_time, time_zone = zone_split
+
+        _full_time_split = _full_time.split('.')
+        if not _full_time_split:
+            raise (Exception('The time portion is missing.'))
+
+        _time = _full_time_split[0]
+        nano = _full_time_split[1] if len(_full_time_split) > 1 else '000000000'
 
-        _time, fragment = _remaining_split    
         if ':' not in _time:
-            raise(Exception('The time portion must contain colons.'))
+            raise (Exception('The time portion must contain colons.'))
 
         _time_split = _time.split(':')
         if len(_time_split) != 3:
-            raise(Exception('The time portions must contains 3 parts separated by colons.'))
+            raise (Exception('The time portions must contains 3 parts separated by colons.'))
 
         hour, minute, second = _time_split
         time_secs = (int(hour) * 3600) + (int(minute) * 60) + int(second)
 
-        time_zone_minutes = 0
-        if 'Z' in fragment:
-            fragment_split = fragment.split('Z')
-        elif '-' in fragment:
-            fragment_split = fragment.split('-')
-            time_zone_minutes = 1
-        elif '+' in fragment:
-            fragment_split = fragment.split('+')
-            time_zone_minutes = -1
-        else:
-            fragment_split = [fragment, '']
-
-        if len(fragment_split) != 2:
-            raise(Exception('If a timezone offset is specified it must contain 2 parts.'))
-
-        nano, time_zone = fragment_split
         nano_secs = int(nano[:9]) * pow(10, (9 - len(nano[:9])))
 
         tzs = 0
         if len(time_zone) > 0:
             tz_clean = time_zone.replace(':', '')
             if len(tz_clean) < 2:
-                raise(Exception('Timezone offset must be at least 2 charaters.'))
+                raise (Exception('Timezone offset must be at least 2 charaters.'))
             tzm = (int(tz_clean[:2]) * 60)
             if len(tz_clean) > 2:
                 if len(tz_clean) != 4:
-                    raise(Exception('Timezone offset must be: hhmm, hh:mm or hh.'))
+                    raise (Exception('Timezone offset must be: hhmm, hh:mm or hh.'))
                 tzm += int(tz_clean[2:])
             tzs = tzm * 60
             tzs *= time_zone_minutes
 
         ns = (((date_secs + time_secs + tzs) * 1000000000)) + nano_secs
         return ns
 
@@ -258,16 +259,17 @@
         # The year will be one off for dates in January and February, so adjust if the Jan or Feb.
         # month is 1 to 12, month_index is 0 to 11.
 
         peek_days = (self.value // ANSI_TIME_MULTIPLIER) // SECONDS_PER_DAY
         days = peek_days + PEEK_EPOCH_DELTA        # days from 1/3/0000 to 1/1/1601
 
         quad = (days if (days >= 0) else (days - 146096)) // 146097
-        quad_day = int( days - (quad * 146097) )
-        quad_year = (quad_day - (quad_day // 1460) + (quad_day // 36524) - (quad_day // 146096)) // 365
+        quad_day = int(days - (quad * 146097))
+        quad_year = ((quad_day - (quad_day // 1460)
+                      + (quad_day // 36524) - (quad_day // 146096)) // 365)
         year_index = quad_year + (quad * 400)
         year_day = quad_day - ((365 * quad_year) + (quad_year // 4) - (quad_year // 100))
         month_index = ((5 * year_day) + 2) // 153
         day = year_day - (((153 * month_index) + 2) // 5) + 1
         month = (month_index + 3) if (month_index < 10) else (month_index - 9)
         year = year_index + (month < 3)
         return year, month, day
@@ -275,15 +277,15 @@
     def get_time(self):
         """Convert the PeekTime to hours, minutes, seconds, nanoseconds.
 
         Returns a tuple of: hours, minutes, seconds and nanoseconds.
         """
         v1 = self.value // NANOSECONDS_PER_SECOND
         nanoseconds = self.value % NANOSECONDS_PER_SECOND
-        days = v1 // SECONDS_PER_DAY
+        # days = v1 // SECONDS_PER_DAY
         v2 = v1 % SECONDS_PER_DAY
         hours = v2 // SECONDS_PER_HOUR
         v3 = v2 % SECONDS_PER_HOUR
         minutes = v3 // SECONDS_PER_MINUTE
         seconds = v3 % SECONDS_PER_MINUTE
         return hours, minutes, seconds, nanoseconds
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/performancelogger.py` & `omniscript-liveaction-3.0.49/src/omniscript/performancelogger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """PerformanceLogger class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
-
-import logging
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 from .peektime import PeekTime
 
 
 class PerformanceRecord(object):
     def __init__(self, command):
         self.command = command
         self.start = self.end = PeekTime()
 
     def __str__(self):
         return (f'{self.start.iso_time()}, {self.end.iso_time()}, '
-            f'{self.end - self.start}, {self.command}')
+                f'{self.end - self.start}, {self.command}')
 
     def log_format(self):
         return (f'{self.start.iso_time()}, {self.end.iso_time()}, '
-            f'{self.end - self.start}, {self.command}\n')
+                f'{self.end - self.start}, {self.command}\n')
 
 
 class PerformanceLogger(object):
     file = None
     cache = []
 
     def __init__(self, filename, mode='w'):
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/readstream.py` & `omniscript-liveaction-3.0.49/src/omniscript/readstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ﻿"""ReadStream class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 # " ".join(['%02X' % ord(b) for b in data])
 
 import os
 import struct
 
 import omniscript
@@ -101,15 +101,15 @@
     def read_double(self):
         """Read a long, 8-byte, floating-point value and advance the
         current position.
         """
         value = struct.unpack_from('=d', self.data, self.offset)[0]
         self.seek(8, os.SEEK_CUR)
         return value
-        
+
     def read_guid(self):
         """Read a 16-byte GUID and advance the current position."""
         value = struct.unpack_from('=16s', self.data, self.offset)[0]
         id = OmniId(bytes_le=value)
         self.seek(16, os.SEEK_CUR)
         return id
 
@@ -132,15 +132,15 @@
     def read_unicode(self, count=0):
         """Read an integer length and string value and advance the
         current position.
         """
         if count == 0:
             length = self.read_uint()
             if length == 0:
-               return ''
+                return ''
             if (length % 2) != 0:
                 raise ValueError
             if length > 512:
                 raise OmniError(f'Unicode String is too long: {length}')
         else:
             length = count
         data = struct.unpack_from(
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript/statslimit.py` & `omniscript-liveaction-3.0.49/src/omniscript/statslimit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,70 +1,66 @@
 ﻿"""StatsLimit class.
 """
-#Copyright (c) LiveAction, Inc. 2022. All rights reserved.
-#Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
-#Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
+# Copyright (c) LiveAction, Inc. 2022. All rights reserved.
+# Copyright (c) Savvius, Inc. 2013-2019. All rights reserved.
+# Copyright (c) WildPackets, Inc. 2013-2014. All rights reserved.
 
 
-import xml.etree.ElementTree as ET
-
-# from .omniscript import get_class_name_ids
 from .omnierror import OmniError
-
-from .invariant import (LIMIT_TYPE_NONE, LIMIT_TYPE_PACKETS,
-    LIMIT_TYPE_BYTES, LIMIT_TYPE_BUFFER, SEVERITY_INFORMATIONAL)
-
+from .invariant import (
+    LIMIT_TYPE_NONE, LIMIT_TYPE_PACKETS, LIMIT_TYPE_BYTES, LIMIT_TYPE_BUFFER, Severity)
 
 ATTRIB_TRUE = '1'
 ATTRIB_FALSE = '0'
 
 STATS_LIMIT_MAGIC = 0x6D696C73
 STATS_LIMIT_VERSION_1 = 0x0001
 STATS_LIMIT_VERSION_2 = 0x0002
 
 limit_types = {
-    'none' : LIMIT_TYPE_NONE,
-    'packets' : LIMIT_TYPE_PACKETS,
-    'bytes' : LIMIT_TYPE_BYTES,
-    'buffer' : LIMIT_TYPE_BUFFER
+    'none': LIMIT_TYPE_NONE,
+    'packets': LIMIT_TYPE_PACKETS,
+    'bytes': LIMIT_TYPE_BYTES,
+    'buffer': LIMIT_TYPE_BUFFER
 }
 
 
 def _is_attrib_enabled(prop, attrib):
     """Return if an attribute of a node is aa non-zero value."""
     return int(prop.attrib.get(attrib, '0')) != 0
 
 
 def _get_class_id(name):
     from .omniscript import get_class_name_ids
-    
+
     class_name_ids = get_class_name_ids()
     id = class_name_ids[name]
     return id.format() if id else ''
 
 
 def _to_attrib_boolean(value):
     return ATTRIB_TRUE if value else ATTRIB_FALSE
 
 
 class StatsLimit(object):
-    """The Stats Limit settings of an object."""
+    """The Stats Limit settings of an object.
+    """
 
     enabled = False
     """Is this Stats Limit enabled."""
 
     limit = 100000
     """The maximum number of statitic entries to maintain.
     Default is 100,000.
     """
 
     reset_count = 0
     """The number of times this statistic has been reset."""
 
-    severity = SEVERITY_INFORMATIONAL
+    severity = Severity.INFORMATIONAL
     """The severity level of the Notification to post."""
 
     timeout_count = 0
     """The number of times this statistic has timed-out."""
 
     option_reset = False
     """Is the Reset the statistics when the limit has been reached
@@ -75,22 +71,22 @@
     """Is the Post a Notification when the limit has been reached
     option enabled.
     """
 
     _name = '_'
     """The XML Tag of this Stats Limit."""
 
-    #Tags
+    # Tags
     _json_classid = 'clsid'
     _json_enabled = 'enabled'
     _json_limit = 'limit'
     _json_notify = 'notify'
     _json_reset = 'reset'
     _json_severity = 'severity'
- 
+
     _tag_class_name = 'PeekStatsLimitSettings'
     _tag_root_name = 'PeekStatsLimitSettings'
     _tag_enabled = 'Enabled'
     _tag_limit = 'Limit'
     _tag_notify = 'Notify'
     _tag_reset = 'Reset'
     _tag_severity = 'Severity'
@@ -109,15 +105,15 @@
 
     def __str__(self):
         return f'StatsLimit: {self._name}'
 
     def _load(self, props):
         if not isinstance(props, dict):
             return
-        for k,v in props.items():
+        for k, v in props.items():
             if k == StatsLimit._json_enabled:
                 self.enabled = v
             elif k == StatsLimit._json_limit:
                 self.limit = int(v)
             elif k == StatsLimit._json_notify:
                 self.option_notify = v
             elif k == StatsLimit._json_reset:
@@ -144,20 +140,17 @@
 
     def parse(self, obj):
         """Parse the limit settings from an ETree.SubElement."""
         limit = obj.find(StatsLimit._tag_root_name)
         if limit is not None:
             self.enabled = _is_attrib_enabled(limit, StatsLimit._tag_enabled)
             self.limit = int(limit.attrib.get(StatsLimit._tag_limit, '0'))
-            self.severity = \
-                int(limit.attrib.get(StatsLimit._tag_severity, '0'))
-            self.option_reset = \
-                _is_attrib_enabled(limit, StatsLimit._tag_reset)
-            self.option_notify = \
-                _is_attrib_enabled(limit, StatsLimit._tag_notify)
+            self.severity = int(limit.attrib.get(StatsLimit._tag_severity, '0'))
+            self.option_reset = _is_attrib_enabled(limit, StatsLimit._tag_reset)
+            self.option_notify = _is_attrib_enabled(limit, StatsLimit._tag_notify)
 
     def _store(self, props):
         _props = {}
         _props[StatsLimit._json_classid] = _get_class_id(StatsLimit._tag_class_name)
         _props[StatsLimit._json_enabled] = self.enabled
         _props[StatsLimit._json_limit] = self.limit
         _props[StatsLimit._json_notify] = self.option_notify
@@ -166,15 +159,15 @@
         props[self._name] = _props
 
     # def to_xml(self, format=0):
     #     """Render as XML.
 
     #     format 0 (default) is as an object (obj), otherwise with the same
     #     tag as it's type (_name).
-        
+
     #     Returns:
     #         :class:`ETree.SubElement`
     #     """
     #     class_name_ids = omniscript.get_class_name_ids()
     #     if format == 1:
     #         elem = ET.Element(self._name,
     #                           {'clsid':str(class_name_ids[StatsLimit._tag_class_name])})
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript_liveaction.egg-info/PKG-INFO` & `omniscript-liveaction-3.0.49/src/omniscript_liveaction.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: omniscript-liveaction
-Version: 3.0.44
+Version: 3.0.49
 Summary: Automate LiveAction LiveCapture and LiveWire.
 Home-page: https://MyPeek.LiveAction.com
 Author: gvisser
 Author-email: gvisser@liveaction.com
 Project-URL: Bug Tracker, https://MyPeek.LiveAction.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Example Package
+# OmniScript 3.0
 
 Automate LiveAction LiveCapture and LiveWire.
```

### Comparing `omniscript-liveaction-3.0.44/src/omniscript_liveaction.egg-info/SOURCES.txt` & `omniscript-liveaction-3.0.49/src/omniscript_liveaction.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,81 @@
 LICENSE
 MANIFEST.in
 README.md
 build.txt
+next_version.txt
 pyproject.toml
 setup.cfg
 src/omniscript/__init__.py
 src/omniscript/adapter.py
 src/omniscript/adapterinformation.py
 src/omniscript/alarm.py
 src/omniscript/analysismodule.py
 src/omniscript/application.py
+src/omniscript/auditlog.py
 src/omniscript/authenticationtoken.py
+src/omniscript/capabilities.py
 src/omniscript/capture.py
 src/omniscript/capturesession.py
 src/omniscript/capturetemplate.py
 src/omniscript/country.py
+src/omniscript/decryptionkey.py
+src/omniscript/decryptionkeytemplate.py
 src/omniscript/directory.py
+src/omniscript/dms.py
+src/omniscript/enginesettings.py
 src/omniscript/enginestatus.py
 src/omniscript/eventlog.py
+src/omniscript/expertpreferences.py
 src/omniscript/fileinformation.py
 src/omniscript/filter.py
 src/omniscript/filternode.py
 src/omniscript/forensicsearch.py
 src/omniscript/forensictemplate.py
 src/omniscript/graphtemplate.py
+src/omniscript/helpers.py
 src/omniscript/invariant.py
+src/omniscript/license.py
+src/omniscript/liveflow.py
 src/omniscript/mediainformation.py
+src/omniscript/nametable.py
+src/omniscript/notifications.py
 src/omniscript/omniaddress.py
 src/omniscript/omnidatatable.py
 src/omniscript/omniengine.py
 src/omniscript/omnierror.py
 src/omniscript/omniid.py
 src/omniscript/omniport.py
 src/omniscript/omniscript.py
 src/omniscript/packet.py
 src/omniscript/packetfileinformation.py
 src/omniscript/peektime.py
 src/omniscript/performancelogger.py
+src/omniscript/protocol.py
+src/omniscript/protocoltranslation.py
 src/omniscript/readstream.py
+src/omniscript/remoteengine.py
+src/omniscript/selection.py
 src/omniscript/statslimit.py
+src/omniscript/user.py
 src/omniscript/voipsettings.py
+src/omniscript/data/_capability_ids.txt
 src/omniscript/data/_capture_template.xml
 src/omniscript/data/_capture_template_linux.xml
 src/omniscript/data/_capture_template_windows.xml
 src/omniscript/data/_class_ids.txt
 src/omniscript/data/_co_codes.txt
 src/omniscript/data/_expert_problem_ids.txt
 src/omniscript/data/_stat_ids.txt
 src/omniscript/data/expertdescriptions.xml
 src/omniscript/data/pspecs.xml
 src/omniscript_liveaction.egg-info/PKG-INFO
 src/omniscript_liveaction.egg-info/SOURCES.txt
 src/omniscript_liveaction.egg-info/dependency_links.txt
 src/omniscript_liveaction.egg-info/requires.txt
-src/omniscript_liveaction.egg-info/top_level.txt
+src/omniscript_liveaction.egg-info/top_level.txt
+src/tests/__init__.py
+src/tests/conftest.py
+src/tests/decrypt_file.py
+src/tests/encrypt_file.py
+src/tests/encryption_util.py
+src/tests/gen_key.py
```

