# Comparing `tmp/agstream-2.0.8.tar.gz` & `tmp/agstream-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\agstream-2.0.8.tar", last modified: Fri Apr  8 08:48:37 2022, max compression
+gzip compressed data, was "dist\agstream-2.0.9.tar", last modified: Thu Sep 15 13:15:02 2022, max compression
```

## Comparing `agstream-2.0.8.tar` & `agstream-2.0.9.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxrwxrwx   0        0        0        0 2022-04-08 08:48:37.000000 agstream-2.0.8/
--rw-rw-rw-   0        0        0     1894 2022-04-06 07:48:23.000000 agstream-2.0.8/.gitignore
--rw-rw-rw-   0        0        0      379 2018-02-15 15:59:55.000000 agstream-2.0.8/.project
--rw-rw-rw-   0        0        0      435 2019-09-17 08:44:05.000000 agstream-2.0.8/.pydevproject
--rw-rw-rw-   0        0        0      134 2018-02-15 15:59:55.000000 agstream-2.0.8/.pypirc
-drwxrwxrwx   0        0        0        0 2022-04-08 08:48:37.000000 agstream-2.0.8/.settings/
--rw-rw-rw-   0        0        0      337 2019-08-26 14:00:45.000000 agstream-2.0.8/.settings/org.eclipse.core.resources.prefs
-drwxrwxrwx   0        0        0        0 2022-04-08 08:48:37.000000 agstream-2.0.8/.vscode/
--rw-rw-rw-   0        0        0      164 2022-04-06 07:48:23.000000 agstream-2.0.8/.vscode/launch.json
--rw-rw-rw-   0        0        0      346 2022-01-07 15:22:46.000000 agstream-2.0.8/.vscode/settings.json
--rw-rw-rw-   0        0        0     7816 2018-02-15 15:59:55.000000 agstream-2.0.8/LICENSE
--rw-rw-rw-   0        0        0       14 2018-02-15 15:59:55.000000 agstream-2.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     7163 2022-04-08 08:48:37.000000 agstream-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5438 2022-04-08 08:48:00.000000 agstream-2.0.8/README.md
--rw-rw-rw-   0        0        0        0 2022-01-07 13:52:19.000000 agstream-2.0.8/agsp_stream.log
-drwxrwxrwx   0        0        0        0 2022-04-08 08:48:37.000000 agstream-2.0.8/agstream/
--rw-rw-rw-   0        0        0      346 2022-04-08 08:46:31.000000 agstream-2.0.8/agstream/__init__.py
--rw-rw-rw-   0        0        0    20108 2022-04-08 08:43:26.000000 agstream-2.0.8/agstream/connector.py
--rw-rw-rw-   0        0        0     3191 2022-04-07 14:43:59.000000 agstream-2.0.8/agstream/decorators.py
--rw-rw-rw-   0        0        0     6249 2022-04-07 14:44:42.000000 agstream-2.0.8/agstream/devices.py
--rw-rw-rw-   0        0        0    20571 2022-04-08 07:30:44.000000 agstream-2.0.8/agstream/session.py
--rw-rw-rw-   0        0        0     7273 2022-04-07 14:44:42.000000 agstream-2.0.8/agstream/session_extended.py
-drwxrwxrwx   0        0        0        0 2022-04-08 08:48:37.000000 agstream-2.0.8/agstream/tests/
--rw-rw-rw-   0        0        0        0 2022-01-07 15:24:25.000000 agstream-2.0.8/agstream/tests/__init__.py
--rw-rw-rw-   0        0        0     3836 2022-04-07 14:44:42.000000 agstream-2.0.8/agstream/tests/agstream_extended_session_test.py
--rw-rw-rw-   0        0        0     2122 2022-04-07 14:44:42.000000 agstream-2.0.8/agstream/tests/agstream_test.py
--rw-rw-rw-   0        0        0     4415 2022-04-07 14:44:42.000000 agstream-2.0.8/agstream/virtual_datasources.py
-drwxrwxrwx   0        0        0        0 2022-04-08 08:48:37.000000 agstream-2.0.8/agstream.egg-info/
--rw-rw-rw-   0        0        0     7163 2022-04-08 08:48:37.000000 agstream-2.0.8/agstream.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1176 2022-04-08 08:48:37.000000 agstream-2.0.8/agstream.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-08 08:48:37.000000 agstream-2.0.8/agstream.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2022-04-08 08:48:37.000000 agstream-2.0.8/agstream.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-04-08 08:48:37.000000 agstream-2.0.8/agstream.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-04-08 08:48:37.000000 agstream-2.0.8/bin/
--rw-rw-rw-   0        0        0      381 2022-01-12 15:45:07.000000 agstream-2.0.8/bin/run_jenkins.sh
--rw-rw-rw-   0        0        0      483 2022-01-12 15:44:58.000000 agstream-2.0.8/bin/run_jenkins_p39_hortus.sh
-drwxrwxrwx   0        0        0        0 2022-04-08 08:48:37.000000 agstream-2.0.8/demo/
-drwxrwxrwx   0        0        0        0 2022-04-08 08:48:37.000000 agstream-2.0.8/demo/extended/
--rw-rw-rw-   0        0        0     1213 2022-04-07 14:44:42.000000 agstream-2.0.8/demo/extended/extended_helloworldDemo_by_each_sensors.py
--rw-rw-rw-   0        0        0      828 2022-04-07 14:44:42.000000 agstream-2.0.8/demo/extended/extended_test.py
--rw-rw-rw-   0        0        0     2351 2022-04-07 14:44:42.000000 agstream-2.0.8/demo/helloworldDemo.py
--rw-rw-rw-   0        0        0     1316 2022-04-07 14:44:42.000000 agstream-2.0.8/demo/helloworldDemoUtc.py
--rw-rw-rw-   0        0        0     1116 2022-04-07 14:44:42.000000 agstream-2.0.8/demo/helloworldDemo_by_each_sensors.py
-drwxrwxrwx   0        0        0        0 2022-04-08 08:48:37.000000 agstream-2.0.8/demo/supagro/
--rw-rw-rw-   0        0        0      686 2022-04-07 14:44:42.000000 agstream-2.0.8/demo/supagro/test.py
--rw-rw-rw-   0        0        0      325 2021-06-11 09:45:30.000000 agstream-2.0.8/deploying.txt
-drwxrwxrwx   0        0        0        0 2022-04-08 08:48:37.000000 agstream-2.0.8/docs/
--rw-rw-rw-   0        0        0      628 2018-02-15 15:59:55.000000 agstream-2.0.8/docs/Makefile
--rw-rw-rw-   0        0        0      156 2018-02-15 15:59:55.000000 agstream-2.0.8/docs/generateDoc.txt
--rwxrwxrwx   0        0        0      816 2018-02-15 15:59:55.000000 agstream-2.0.8/docs/make.bat
-drwxrwxrwx   0        0        0        0 2022-04-08 08:48:37.000000 agstream-2.0.8/docs/source/
--rw-rw-rw-   0        0        0      154 2018-02-15 15:59:55.000000 agstream-2.0.8/docs/source/agstream.connector.rst
--rw-rw-rw-   0        0        0      148 2018-02-15 15:59:55.000000 agstream-2.0.8/docs/source/agstream.devices.rst
--rw-rw-rw-   0        0        0     1202 2022-01-10 16:25:16.000000 agstream-2.0.8/docs/source/agstream.rst
--rw-rw-rw-   0        0        0      148 2018-02-15 15:59:55.000000 agstream-2.0.8/docs/source/agstream.session.rst
--rw-rw-rw-   0        0        0      624 2022-01-10 16:25:17.000000 agstream-2.0.8/docs/source/agstream.tests.rst
--rw-rw-rw-   0        0        0     4910 2022-04-07 14:44:42.000000 agstream-2.0.8/docs/source/conf.py
--rw-rw-rw-   0        0        0      482 2018-02-15 15:59:55.000000 agstream-2.0.8/docs/source/index.rst
--rw-rw-rw-   0        0        0     1839 2022-04-07 14:44:42.000000 agstream-2.0.8/docs/source/introduction.rst
--rw-rw-rw-   0        0        0       61 2018-11-13 08:41:54.000000 agstream-2.0.8/docs/source/modules.rst
--rw-rw-rw-   0        0        0       42 2022-04-08 08:48:37.000000 agstream-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3595 2022-04-07 14:43:59.000000 agstream-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-09-15 13:15:02.000000 agstream-2.0.9/
+-rw-rw-rw-   0        0        0     1894 2022-04-06 07:48:23.000000 agstream-2.0.9/.gitignore
+-rw-rw-rw-   0        0        0      379 2018-02-15 15:59:55.000000 agstream-2.0.9/.project
+-rw-rw-rw-   0        0        0      435 2019-09-17 08:44:05.000000 agstream-2.0.9/.pydevproject
+-rw-rw-rw-   0        0        0      134 2018-02-15 15:59:55.000000 agstream-2.0.9/.pypirc
+drwxrwxrwx   0        0        0        0 2022-09-15 13:15:02.000000 agstream-2.0.9/.settings/
+-rw-rw-rw-   0        0        0      337 2019-08-26 14:00:45.000000 agstream-2.0.9/.settings/org.eclipse.core.resources.prefs
+drwxrwxrwx   0        0        0        0 2022-09-15 13:15:02.000000 agstream-2.0.9/.vscode/
+-rw-rw-rw-   0        0        0      164 2022-04-06 07:48:23.000000 agstream-2.0.9/.vscode/launch.json
+-rw-rw-rw-   0        0        0      346 2022-01-07 15:22:46.000000 agstream-2.0.9/.vscode/settings.json
+-rw-rw-rw-   0        0        0     7816 2018-02-15 15:59:55.000000 agstream-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0       14 2018-02-15 15:59:55.000000 agstream-2.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     7204 2022-09-15 13:15:02.000000 agstream-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5471 2022-09-15 13:09:45.000000 agstream-2.0.9/README.md
+-rw-rw-rw-   0        0        0        0 2022-01-07 13:52:19.000000 agstream-2.0.9/agsp_stream.log
+drwxrwxrwx   0        0        0        0 2022-09-15 13:15:02.000000 agstream-2.0.9/agstream/
+-rw-rw-rw-   0        0        0      346 2022-09-15 13:11:09.000000 agstream-2.0.9/agstream/__init__.py
+-rw-rw-rw-   0        0        0    20148 2022-09-15 13:05:11.000000 agstream-2.0.9/agstream/connector.py
+-rw-rw-rw-   0        0        0     3191 2022-04-07 14:43:59.000000 agstream-2.0.9/agstream/decorators.py
+-rw-rw-rw-   0        0        0     6249 2022-04-07 14:44:42.000000 agstream-2.0.9/agstream/devices.py
+-rw-rw-rw-   0        0        0    20572 2022-04-13 13:52:09.000000 agstream-2.0.9/agstream/session.py
+-rw-rw-rw-   0        0        0     7273 2022-04-07 14:44:42.000000 agstream-2.0.9/agstream/session_extended.py
+drwxrwxrwx   0        0        0        0 2022-09-15 13:15:02.000000 agstream-2.0.9/agstream/tests/
+-rw-rw-rw-   0        0        0        0 2022-01-07 15:24:25.000000 agstream-2.0.9/agstream/tests/__init__.py
+-rw-rw-rw-   0        0        0     3836 2022-04-07 14:44:42.000000 agstream-2.0.9/agstream/tests/agstream_extended_session_test.py
+-rw-rw-rw-   0        0        0     2122 2022-04-07 14:44:42.000000 agstream-2.0.9/agstream/tests/agstream_qualcorse.py
+-rw-rw-rw-   0        0        0     2122 2022-04-07 14:44:42.000000 agstream-2.0.9/agstream/tests/agstream_test.py
+-rw-rw-rw-   0        0        0     4415 2022-04-07 14:44:42.000000 agstream-2.0.9/agstream/virtual_datasources.py
+drwxrwxrwx   0        0        0        0 2022-09-15 13:15:02.000000 agstream-2.0.9/agstream.egg-info/
+-rw-rw-rw-   0        0        0     7204 2022-09-15 13:15:01.000000 agstream-2.0.9/agstream.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1213 2022-09-15 13:15:01.000000 agstream-2.0.9/agstream.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-15 13:15:01.000000 agstream-2.0.9/agstream.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2022-09-15 13:15:01.000000 agstream-2.0.9/agstream.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-09-15 13:15:01.000000 agstream-2.0.9/agstream.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-09-15 13:15:02.000000 agstream-2.0.9/bin/
+-rw-rw-rw-   0        0        0      381 2022-01-12 15:45:07.000000 agstream-2.0.9/bin/run_jenkins.sh
+-rw-rw-rw-   0        0        0      483 2022-01-12 15:44:58.000000 agstream-2.0.9/bin/run_jenkins_p39_hortus.sh
+drwxrwxrwx   0        0        0        0 2022-09-15 13:15:02.000000 agstream-2.0.9/demo/
+drwxrwxrwx   0        0        0        0 2022-09-15 13:15:02.000000 agstream-2.0.9/demo/extended/
+-rw-rw-rw-   0        0        0     1213 2022-04-07 14:44:42.000000 agstream-2.0.9/demo/extended/extended_helloworldDemo_by_each_sensors.py
+-rw-rw-rw-   0        0        0      828 2022-04-07 14:44:42.000000 agstream-2.0.9/demo/extended/extended_test.py
+-rw-rw-rw-   0        0        0     2351 2022-04-07 14:44:42.000000 agstream-2.0.9/demo/helloworldDemo.py
+-rw-rw-rw-   0        0        0     1316 2022-04-07 14:44:42.000000 agstream-2.0.9/demo/helloworldDemoUtc.py
+-rw-rw-rw-   0        0        0     1116 2022-04-07 14:44:42.000000 agstream-2.0.9/demo/helloworldDemo_by_each_sensors.py
+drwxrwxrwx   0        0        0        0 2022-09-15 13:15:02.000000 agstream-2.0.9/demo/supagro/
+-rw-rw-rw-   0        0        0      686 2022-04-07 14:44:42.000000 agstream-2.0.9/demo/supagro/test.py
+-rw-rw-rw-   0        0        0      325 2021-06-11 09:45:30.000000 agstream-2.0.9/deploying.txt
+drwxrwxrwx   0        0        0        0 2022-09-15 13:15:02.000000 agstream-2.0.9/docs/
+-rw-rw-rw-   0        0        0      628 2018-02-15 15:59:55.000000 agstream-2.0.9/docs/Makefile
+-rw-rw-rw-   0        0        0      156 2018-02-15 15:59:55.000000 agstream-2.0.9/docs/generateDoc.txt
+-rwxrwxrwx   0        0        0      816 2018-02-15 15:59:55.000000 agstream-2.0.9/docs/make.bat
+drwxrwxrwx   0        0        0        0 2022-09-15 13:15:02.000000 agstream-2.0.9/docs/source/
+-rw-rw-rw-   0        0        0      154 2018-02-15 15:59:55.000000 agstream-2.0.9/docs/source/agstream.connector.rst
+-rw-rw-rw-   0        0        0      148 2018-02-15 15:59:55.000000 agstream-2.0.9/docs/source/agstream.devices.rst
+-rw-rw-rw-   0        0        0     1202 2022-01-10 16:25:16.000000 agstream-2.0.9/docs/source/agstream.rst
+-rw-rw-rw-   0        0        0      148 2018-02-15 15:59:55.000000 agstream-2.0.9/docs/source/agstream.session.rst
+-rw-rw-rw-   0        0        0      624 2022-01-10 16:25:17.000000 agstream-2.0.9/docs/source/agstream.tests.rst
+-rw-rw-rw-   0        0        0     4910 2022-04-07 14:44:42.000000 agstream-2.0.9/docs/source/conf.py
+-rw-rw-rw-   0        0        0      482 2018-02-15 15:59:55.000000 agstream-2.0.9/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1839 2022-04-07 14:44:42.000000 agstream-2.0.9/docs/source/introduction.rst
+-rw-rw-rw-   0        0        0       61 2018-11-13 08:41:54.000000 agstream-2.0.9/docs/source/modules.rst
+-rw-rw-rw-   0        0        0       42 2022-09-15 13:15:02.000000 agstream-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3595 2022-04-07 14:43:59.000000 agstream-2.0.9/setup.py
```

### Comparing `agstream-2.0.8/.gitignore` & `agstream-2.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/LICENSE` & `agstream-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/PKG-INFO` & `agstream-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agstream
-Version: 2.0.8
+Version: 2.0.9
 Summary: Agriscope python library to access data
 Home-page: https://github.com/agriscope/agstream/
 Author: Agriscope
 Author-email: team@agriscope.fr
 License: UNKNOWN
 Description: AgspStream
         ==============
@@ -19,14 +19,15 @@
         data analysis comming from agricultural field.
         
         
           
           
         What's New
         ===========
+        - (2022/09) v2.0.9  : Use Https
         - (2022/01) v2.0.8  : Bug correction in logger
         - (2022/01) v2.0.7  : Add a retry API when something wrong seems to be there
         - (2022/01) v2.0.6  : Improve capabilities to select virtual datasources to update
         - (2022/01) v2.0.0  : Add capabilities to get virtual datasources
         - (2021/06) v1.0.4  : Again optimize exception reporting when server is not joinable
         - (2021/06) v1.0.3  : Optimize exception reporting when server is not joinable
         - (2021/03) v1.0.2  : Optimize sensor data retrieving
```

### Comparing `agstream-2.0.8/README.md` & `agstream-2.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 data analysis comming from agricultural field.
 
 
   
   
 What's New
 ===========
+- (2022/09) v2.0.9  : Use Https
 - (2022/01) v2.0.8  : Bug correction in logger
 - (2022/01) v2.0.7  : Add a retry API when something wrong seems to be there
 - (2022/01) v2.0.6  : Improve capabilities to select virtual datasources to update
 - (2022/01) v2.0.0  : Add capabilities to get virtual datasources
 - (2021/06) v1.0.4  : Again optimize exception reporting when server is not joinable
 - (2021/06) v1.0.3  : Optimize exception reporting when server is not joinable
 - (2021/03) v1.0.2  : Optimize sensor data retrieving
```

### Comparing `agstream-2.0.8/agstream/connector.py` & `agstream-2.0.9/agstream/connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     """
 
     debug = True
 
     def __init__(self, server="jsonapi.agriscope.fr"):
         self.sessionOpen = False
         self.agspSessionId = 0
-        self.server = "http://" + server
+        self.server = "https://" + server
         self.application = "/agriscope-web/app"
         self.lastLogin = "undefined"
         self.lastPassword = "undefined"
         self.debug = False
 
     def login(self, login_p, password_p):
         """
@@ -421,14 +421,15 @@
 
             if retry == 0:
                 print("Probleme de connexion pour aller vers " + url)
                 return
             str_response = response.read().decode("utf-8")
 
             if self.debug == True:
+                #print (str_response)
                 logger.debug(str_response)
             obj = json.loads(str_response, strict=False)
             infomessage = "N/A"
             if "infoMessage" in obj:
                 infomessage = obj["infoMessage"]
                 if "session invalide" in infomessage:
                     if len(method) > 0:
```

### Comparing `agstream-2.0.8/agstream/decorators.py` & `agstream-2.0.9/agstream/decorators.py`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/agstream/devices.py` & `agstream-2.0.9/agstream/devices.py`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/agstream/session.py` & `agstream-2.0.9/agstream/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             # reinitialise
             self.agribases = list()
             logger.info(login_p + " logging OK.")
             if updateAgribaseInfo == True:
                 self.__refreshAgribases()
         if self.debug == True:
             if status == True:
-                logger.info(login_p + " logging OK.")
+                logger.debug(login_p + " logging OK.")
 
             else:
                 logger.error("Erreur de connection pour " + login_p + ".")
         self.status = status
         self.sessionId = sessionId
         return status
```

### Comparing `agstream-2.0.8/agstream/session_extended.py` & `agstream-2.0.9/agstream/session_extended.py`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/agstream/tests/agstream_extended_session_test.py` & `agstream-2.0.9/agstream/tests/agstream_extended_session_test.py`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/agstream/tests/agstream_test.py` & `agstream-2.0.9/agstream/tests/agstream_qualcorse.py`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/agstream/virtual_datasources.py` & `agstream-2.0.9/agstream/virtual_datasources.py`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/agstream.egg-info/PKG-INFO` & `agstream-2.0.9/agstream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agstream
-Version: 2.0.8
+Version: 2.0.9
 Summary: Agriscope python library to access data
 Home-page: https://github.com/agriscope/agstream/
 Author: Agriscope
 Author-email: team@agriscope.fr
 License: UNKNOWN
 Description: AgspStream
         ==============
@@ -19,14 +19,15 @@
         data analysis comming from agricultural field.
         
         
           
           
         What's New
         ===========
+        - (2022/09) v2.0.9  : Use Https
         - (2022/01) v2.0.8  : Bug correction in logger
         - (2022/01) v2.0.7  : Add a retry API when something wrong seems to be there
         - (2022/01) v2.0.6  : Improve capabilities to select virtual datasources to update
         - (2022/01) v2.0.0  : Add capabilities to get virtual datasources
         - (2021/06) v1.0.4  : Again optimize exception reporting when server is not joinable
         - (2021/06) v1.0.3  : Optimize exception reporting when server is not joinable
         - (2021/03) v1.0.2  : Optimize sensor data retrieving
```

### Comparing `agstream-2.0.8/agstream.egg-info/SOURCES.txt` & `agstream-2.0.9/agstream.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 agstream.egg-info/PKG-INFO
 agstream.egg-info/SOURCES.txt
 agstream.egg-info/dependency_links.txt
 agstream.egg-info/requires.txt
 agstream.egg-info/top_level.txt
 agstream/tests/__init__.py
 agstream/tests/agstream_extended_session_test.py
+agstream/tests/agstream_qualcorse.py
 agstream/tests/agstream_test.py
 bin/run_jenkins.sh
 bin/run_jenkins_p39_hortus.sh
 demo/helloworldDemo.py
 demo/helloworldDemoUtc.py
 demo/helloworldDemo_by_each_sensors.py
 demo/extended/extended_helloworldDemo_by_each_sensors.py
```

### Comparing `agstream-2.0.8/demo/extended/extended_helloworldDemo_by_each_sensors.py` & `agstream-2.0.9/demo/extended/extended_helloworldDemo_by_each_sensors.py`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/demo/extended/extended_test.py` & `agstream-2.0.9/demo/extended/extended_test.py`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/demo/helloworldDemo.py` & `agstream-2.0.9/demo/helloworldDemo.py`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/demo/helloworldDemoUtc.py` & `agstream-2.0.9/demo/helloworldDemoUtc.py`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/demo/helloworldDemo_by_each_sensors.py` & `agstream-2.0.9/demo/helloworldDemo_by_each_sensors.py`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/demo/supagro/test.py` & `agstream-2.0.9/demo/supagro/test.py`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/docs/Makefile` & `agstream-2.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/docs/make.bat` & `agstream-2.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/docs/source/agstream.rst` & `agstream-2.0.9/docs/source/agstream.rst`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/docs/source/agstream.tests.rst` & `agstream-2.0.9/docs/source/agstream.tests.rst`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/docs/source/conf.py` & `agstream-2.0.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/docs/source/introduction.rst` & `agstream-2.0.9/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `agstream-2.0.8/setup.py` & `agstream-2.0.9/setup.py`

 * *Files identical despite different names*

