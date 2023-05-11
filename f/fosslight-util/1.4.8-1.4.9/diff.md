# Comparing `tmp/fosslight_util-1.4.8.tar.gz` & `tmp/fosslight_util-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fosslight_util-1.4.8.tar", last modified: Fri Aug 12 00:46:50 2022, max compression
+gzip compressed data, was "dist/fosslight_util-1.4.9.tar", last modified: Thu Sep  1 08:51:46 2022, max compression
```

## Comparing `fosslight_util-1.4.8.tar` & `fosslight_util-1.4.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-12 00:46:50.000000 fosslight_util-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       98 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     6640 2022-08-12 00:46:50.000000 fosslight_util-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4875 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      117 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-08-12 00:46:50.000000 fosslight_util-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1681 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-12 00:46:50.000000 fosslight_util-1.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-12 00:46:50.000000 fosslight_util-1.4.8/src/fosslight_util/
--rwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5642 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/_get_downloadable_url.py
--rw-r--r--   0 runner    (1001) docker     (116)     2582 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/compare_yaml.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      525 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/constant.py
--rw-r--r--   0 runner    (1001) docker     (116)     2298 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/convert_excel_to_yaml.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     8141 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/download.py
--rw-r--r--   0 runner    (1001) docker     (116)     1323 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/help.py
--rw-r--r--   0 runner    (1001) docker     (116)     4255 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/oss_item.py
--rw-r--r--   0 runner    (1001) docker     (116)     3354 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/output_format.py
--rw-r--r--   0 runner    (1001) docker     (116)     3557 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/parsing_yaml.py
--rw-r--r--   0 runner    (1001) docker     (116)     4872 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/read_excel.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-12 00:46:50.000000 fosslight_util-1.4.8/src/fosslight_util/resources/
--rw-r--r--   0 runner    (1001) docker     (116)  4648187 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/resources/frequentLicenselist.json
--rw-r--r--   0 runner    (1001) docker     (116)   218743 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/resources/licenses.json
--rwxr-xr-x   0 runner    (1001) docker     (116)     2820 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/set_log.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2965 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/spdx_licenses.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      433 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/timer_thread.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     8502 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/write_excel.py
--rw-r--r--   0 runner    (1001) docker     (116)    11831 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/write_opossum.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      574 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/write_txt.py
--rw-r--r--   0 runner    (1001) docker     (116)     3294 2022-08-12 00:46:42.000000 fosslight_util-1.4.8/src/fosslight_util/write_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-12 00:46:50.000000 fosslight_util-1.4.8/src/fosslight_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6640 2022-08-12 00:46:50.000000 fosslight_util-1.4.8/src/fosslight_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1020 2022-08-12 00:46:50.000000 fosslight_util-1.4.8/src/fosslight_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-12 00:46:50.000000 fosslight_util-1.4.8/src/fosslight_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       69 2022-08-12 00:46:50.000000 fosslight_util-1.4.8/src/fosslight_util.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      188 2022-08-12 00:46:50.000000 fosslight_util-1.4.8/src/fosslight_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       15 2022-08-12 00:46:50.000000 fosslight_util-1.4.8/src/fosslight_util.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-01 08:51:46.000000 fosslight_util-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       98 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     6640 2022-09-01 08:51:46.000000 fosslight_util-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4875 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      117 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2022-09-01 08:51:46.000000 fosslight_util-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1681 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-01 08:51:46.000000 fosslight_util-1.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-01 08:51:46.000000 fosslight_util-1.4.9/src/fosslight_util/
+-rwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     5642 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/_get_downloadable_url.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2582 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/compare_yaml.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)      525 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/constant.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2298 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/convert_excel_to_yaml.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     8891 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/download.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1497 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/help.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5109 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/oss_item.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3354 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/output_format.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3689 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/parsing_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4872 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/read_excel.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-01 08:51:46.000000 fosslight_util-1.4.9/src/fosslight_util/resources/
+-rw-r--r--   0 runner    (1001) docker     (116)  4648187 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/resources/frequentLicenselist.json
+-rw-r--r--   0 runner    (1001) docker     (116)   218743 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/resources/licenses.json
+-rwxr-xr-x   0 runner    (1001) docker     (116)     2820 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/set_log.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     2965 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/spdx_licenses.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)      433 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/timer_thread.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     8502 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/write_excel.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11831 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/write_opossum.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)      574 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/write_txt.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3294 2022-09-01 08:51:37.000000 fosslight_util-1.4.9/src/fosslight_util/write_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-01 08:51:46.000000 fosslight_util-1.4.9/src/fosslight_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     6640 2022-09-01 08:51:46.000000 fosslight_util-1.4.9/src/fosslight_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1020 2022-09-01 08:51:46.000000 fosslight_util-1.4.9/src/fosslight_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-09-01 08:51:46.000000 fosslight_util-1.4.9/src/fosslight_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       69 2022-09-01 08:51:46.000000 fosslight_util-1.4.9/src/fosslight_util.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      188 2022-09-01 08:51:46.000000 fosslight_util-1.4.9/src/fosslight_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       15 2022-09-01 08:51:46.000000 fosslight_util-1.4.9/src/fosslight_util.egg-info/top_level.txt
```

### Comparing `fosslight_util-1.4.8/LICENSE` & `fosslight_util-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fosslight_util-1.4.8/PKG-INFO` & `fosslight_util-1.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight_util
-Version: 1.4.8
+Version: 1.4.9
 Summary: FOSSLight Util
 Home-page: https://github.com/fosslight/fosslight_util
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_util
 Description: <!--
         Copyright (c) 2021 LG Electronics
```

### Comparing `fosslight_util-1.4.8/README.md` & `fosslight_util-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `fosslight_util-1.4.8/setup.py` & `fosslight_util-1.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open('requirements.txt', 'r', 'utf-8') as f:
     required = f.read().splitlines()
 
 if __name__ == "__main__":
     setup(
         name='fosslight_util',
-        version='1.4.8',
+        version='1.4.9',
         package_dir={"": "src"},
         packages=find_packages(where='src'),
         description='FOSSLight Util',
         long_description=readme,
         long_description_content_type='text/markdown',
         license='Apache-2.0',
         author='LG Electronics',
```

### Comparing `fosslight_util-1.4.8/src/fosslight_util/_get_downloadable_url.py` & `fosslight_util-1.4.9/src/fosslight_util/_get_downloadable_url.py`

 * *Files identical despite different names*

### Comparing `fosslight_util-1.4.8/src/fosslight_util/compare_yaml.py` & `fosslight_util-1.4.9/src/fosslight_util/compare_yaml.py`

 * *Files identical despite different names*

### Comparing `fosslight_util-1.4.8/src/fosslight_util/constant.py` & `fosslight_util-1.4.9/src/fosslight_util/constant.py`

 * *Files identical despite different names*

### Comparing `fosslight_util-1.4.8/src/fosslight_util/convert_excel_to_yaml.py` & `fosslight_util-1.4.9/src/fosslight_util/convert_excel_to_yaml.py`

 * *Files identical despite different names*

### Comparing `fosslight_util-1.4.8/src/fosslight_util/download.py` & `fosslight_util-1.4.9/src/fosslight_util/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,34 +14,49 @@
 import bz2
 from datetime import datetime
 from pathlib import Path
 from ._get_downloadable_url import get_downloadable_url
 import fosslight_util.constant as constant
 from fosslight_util.set_log import init_log
 import signal
+import time
+import threading
+import platform
 
 logger = logging.getLogger(constant.LOGGER_NAME)
 compression_extension = {".tar.bz2", ".tar.gz", ".tar.xz", ".tgz", ".tar", ".zip", ".jar", ".bz2"}
 SIGNAL_TIMEOUT = 600
 
 
+class Alarm(threading.Thread):
+    def __init__(self, timeout):
+        threading.Thread.__init__(self)
+        self.timeout = timeout
+        self.setDaemon(True)
+
+    def run(self):
+        time.sleep(self.timeout)
+        logger.error("download timeout! (%d sec)", SIGNAL_TIMEOUT)
+        os._exit(1)
+
+
 class TimeOutException(Exception):
     pass
 
 
 def alarm_handler(signum, frame):
-    logger.warning("git clone timeout! (%d sec)", SIGNAL_TIMEOUT)
+    logger.warning("download timeout! (%d sec)", SIGNAL_TIMEOUT)
     raise TimeOutException()
 
 
 def print_help_msg():
     print("* Required : -s link_to_download")
     print("* Optional : -t target_directory")
     print("* Optional : -d log_file_directory")
-    sys.exit()
+    sys.exit(0)
 
 
 def main():
 
     src_link = ""
     target_dir = os.getcwd()
     log_dir = os.getcwd()
@@ -117,22 +132,29 @@
             x for x in ref_list if x.endswith(checkout_to))
     except Exception as error:
         logger.warning("git find ref - failed:"+str(error))
     return ref_to_checkout
 
 
 def download_git_clone(git_url, target_dir, checkout_to=""):
-    signal.signal(signal.SIGALRM, alarm_handler)
-    signal.alarm(SIGNAL_TIMEOUT)
+    if platform.system() != "Windows":
+        signal.signal(signal.SIGALRM, alarm_handler)
+        signal.alarm(SIGNAL_TIMEOUT)
+    else:
+        alarm = Alarm(SIGNAL_TIMEOUT)
+        alarm.start()
     try:
         Path(target_dir).mkdir(parents=True, exist_ok=True)
         repo = git.clone_repository(git_url, target_dir,
                                     bare=False, repository=None,
                                     remote=None, callbacks=None)
-        signal.alarm(0)
+        if platform.system() == "Windows":
+            signal.alarm(0)
+        else:
+            del alarm
     except Exception as error:
         logger.warning("git clone - failed:"+str(error))
         return False
     try:
         ref_to_checkout = checkout_to
         if checkout_to != "":
             ref_list = [x for x in repo.references]
@@ -144,17 +166,20 @@
                        " - failed:"+str(error))
     return True
 
 
 def download_wget(link, target_dir, compressed_only):
     success = False
     downloaded_file = ""
-
-    signal.signal(signal.SIGALRM, alarm_handler)
-    signal.alarm(SIGNAL_TIMEOUT)
+    if platform.system() == "Windows":
+        signal.signal(signal.SIGALRM, alarm_handler)
+        signal.alarm(SIGNAL_TIMEOUT)
+    else:
+        alarm = Alarm(SIGNAL_TIMEOUT)
+        alarm.start()
     try:
         Path(target_dir).mkdir(parents=True, exist_ok=True)
 
         ret, new_link = get_downloadable_url(link)
         if ret and new_link != "":
             link = new_link
 
@@ -167,15 +192,18 @@
             success = True
 
         if not success:
             raise Exception('Not supported compression type (link:{0})'.format(link))
 
         logger.info("wget:"+link)
         downloaded_file = wget.download(link)
-        signal.alarm(0)
+        if platform.system() == "Windows":
+            signal.alarm(0)
+        else:
+            del alarm
 
         shutil.move(downloaded_file, target_dir)
         downloaded_file = os.path.join(target_dir, downloaded_file)
         if downloaded_file != "":
             success = True
             logger.debug("wget - downloaded:"+downloaded_file)
     except Exception as error:
```

### Comparing `fosslight_util-1.4.8/src/fosslight_util/help.py` & `fosslight_util-1.4.9/src/fosslight_util/help.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2021 LG Electronics Inc.
 # SPDX-License-Identifier: Apache-2.0
 import sys
 import pkg_resources
 
 _HELP_MESSAGE_COMMON = """
-         _______  _______  _______  _______  ___      ___   _______  __   __  _______
-        |       ||       ||       ||       ||   |    |   | |       ||  | |  ||       |
-        |    ___||   _   ||  _____||  _____||   |    |   | |    ___||  |_|  ||_     _|
-        |   |___ |  | |  || |_____ | |_____ |   |    |   | |   | __ |       |  |   |
-        |    ___||  |_|  ||_____  ||_____  ||   |___ |   | |   ||  ||   _   |  |   |
-        |   |    |       | _____| | _____| ||       ||   | |   |_| ||  | |  |  |   |
-        |___|    |_______||_______||_______||_______||___| |_______||__| |__|  |___|
-        """
+         _______  _______  _______  _______  ___      ___           __
+        |       ||       ||       ||       ||   |    |___|         |  |         _
+        |    ___||   _   ||  _____||  _____||   |     ___          |  |____  __| |__
+        |   |___ |  | |  || |_____ | |_____ |   |    |   | _______ |   _   ||__   __|
+        |    ___||  |_|  ||_____  ||_____  ||   |___ |   ||   _   ||  | |  |   | |
+        |   |    |       | _____| | _____| ||       ||   ||  |_|  ||  | |  |   | |__
+        |___|    |_______||_______||_______||_______||___||____   ||__| |__|   |____|
+                                                               |  |
+                                                           ____|  |
+                                                          |_______|
+"""
 
 
 class PrintHelpMsg():
     message_suffix = ""
 
     def __init__(self, value):
         self.message_suffix = value
```

### Comparing `fosslight_util-1.4.8/src/fosslight_util/oss_item.py` & `fosslight_util-1.4.9/src/fosslight_util/oss_item.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,16 @@
         self._copyright = ""
         self.comment = ""
         self._exclude = False
         self.homepage = ""
         self.relative_path = value
         self._source_name_or_path = []
         self.download_location = ""
+        self._yocto_recipe = []
+        self._yocto_package = []
 
     def __del__(self):
         pass
 
     @property
     def copyright(self):
         return self._copyright
@@ -89,14 +91,38 @@
     def source_name_or_path(self, value):
         if not isinstance(value, list):
             value = value.split(",")
         self._source_name_or_path.extend(value)
         self._source_name_or_path = [item.strip() for item in self._source_name_or_path]
         self._source_name_or_path = list(set(self._source_name_or_path))
 
+    @property
+    def yocto_recipe(self):
+        return self._yocto_recipe
+
+    @yocto_recipe.setter
+    def yocto_recipe(self, value):
+        if not isinstance(value, list):
+            value = value.split(",")
+        self._yocto_recipe.extend(value)
+        self._yocto_recipe = [item.strip() for item in self._yocto_recipe]
+        self._yocto_recipe = list(set(self._yocto_recipe))
+
+    @property
+    def yocto_package(self):
+        return self._yocto_package
+
+    @yocto_package.setter
+    def yocto_package(self, value):
+        if not isinstance(value, list):
+            value = value.split(",")
+        self._yocto_package.extend(value)
+        self._yocto_package = [item.strip() for item in self._yocto_package]
+        self._yocto_package = list(set(self._yocto_package))
+
     def set_sheet_item(self, item):
         if len(item) < 9:
             _logger.warning(f"sheet list is too short ({len(item)}): {item}")
             return
         self.source_name_or_path = item[0]
         self.name = item[1]
         self.version = item[2]
```

### Comparing `fosslight_util-1.4.8/src/fosslight_util/output_format.py` & `fosslight_util-1.4.9/src/fosslight_util/output_format.py`

 * *Files identical despite different names*

### Comparing `fosslight_util-1.4.8/src/fosslight_util/parsing_yaml.py` & `fosslight_util-1.4.9/src/fosslight_util/parsing_yaml.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,7 +93,11 @@
         oss.copyright = value
     elif key == 'exclude':
         oss.exclude = value
     elif key == 'comment':
         oss.comment = value
     elif key == 'homepage':
         oss.homepage = value
+    elif key == 'yocto_package':
+        oss.yocto_package = value
+    elif key == 'yocto_recipe':
+        oss.yocto_recipe = value
```

### Comparing `fosslight_util-1.4.8/src/fosslight_util/read_excel.py` & `fosslight_util-1.4.9/src/fosslight_util/read_excel.py`

 * *Files identical despite different names*

### Comparing `fosslight_util-1.4.8/src/fosslight_util/resources/frequentLicenselist.json` & `fosslight_util-1.4.9/src/fosslight_util/resources/frequentLicenselist.json`

 * *Files identical despite different names*

### Comparing `fosslight_util-1.4.8/src/fosslight_util/resources/licenses.json` & `fosslight_util-1.4.9/src/fosslight_util/resources/licenses.json`

 * *Files identical despite different names*

### Comparing `fosslight_util-1.4.8/src/fosslight_util/set_log.py` & `fosslight_util-1.4.9/src/fosslight_util/set_log.py`

 * *Files identical despite different names*

### Comparing `fosslight_util-1.4.8/src/fosslight_util/spdx_licenses.py` & `fosslight_util-1.4.9/src/fosslight_util/spdx_licenses.py`

 * *Files identical despite different names*

### Comparing `fosslight_util-1.4.8/src/fosslight_util/write_excel.py` & `fosslight_util-1.4.9/src/fosslight_util/write_excel.py`

 * *Files identical despite different names*

### Comparing `fosslight_util-1.4.8/src/fosslight_util/write_opossum.py` & `fosslight_util-1.4.9/src/fosslight_util/write_opossum.py`

 * *Files identical despite different names*

### Comparing `fosslight_util-1.4.8/src/fosslight_util/write_txt.py` & `fosslight_util-1.4.9/src/fosslight_util/write_txt.py`

 * *Files identical despite different names*

### Comparing `fosslight_util-1.4.8/src/fosslight_util/write_yaml.py` & `fosslight_util-1.4.9/src/fosslight_util/write_yaml.py`

 * *Files identical despite different names*

### Comparing `fosslight_util-1.4.8/src/fosslight_util.egg-info/PKG-INFO` & `fosslight_util-1.4.9/src/fosslight_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight-util
-Version: 1.4.8
+Version: 1.4.9
 Summary: FOSSLight Util
 Home-page: https://github.com/fosslight/fosslight_util
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_util
 Description: <!--
         Copyright (c) 2021 LG Electronics
```

### Comparing `fosslight_util-1.4.8/src/fosslight_util.egg-info/SOURCES.txt` & `fosslight_util-1.4.9/src/fosslight_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

