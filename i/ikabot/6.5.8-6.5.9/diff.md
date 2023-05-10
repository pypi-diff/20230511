# Comparing `tmp/ikabot-6.5.8.tar.gz` & `tmp/ikabot-6.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ikabot-6.5.8.tar", last modified: Mon Mar 15 20:48:02 2021, max compression
+gzip compressed data, was "ikabot-6.5.9.tar", last modified: Sun Mar 21 22:58:27 2021, max compression
```

## Comparing `ikabot-6.5.8.tar` & `ikabot-6.5.9.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-15 20:48:02.718439 ikabot-6.5.8/
--rw-r--r--   0 user      (1000) user      (1000)       38 2020-08-03 17:33:36.000000 ikabot-6.5.8/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)      335 2021-03-15 20:48:02.718439 ikabot-6.5.8/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     9307 2021-03-14 17:11:15.000000 ikabot-6.5.8/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-15 20:48:02.711773 ikabot-6.5.8/ikabot/
--rw-r--r--   0 user      (1000) user      (1000)        0 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)       44 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/__main__.py
--rwxr-xr-x   0 user      (1000) user      (1000)     6517 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/command_line.py
--rw-r--r--   0 user      (1000) user      (1000)     1924 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/config.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-15 20:48:02.715106 ikabot-6.5.8/ikabot/function/
--rw-r--r--   0 user      (1000) user      (1000)        0 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/function/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     9115 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/activateMiracle.py
--rw-r--r--   0 user      (1000) user      (1000)     4752 2021-03-14 17:09:40.000000 ikabot-6.5.8/ikabot/function/alertAttacks.py
--rw-r--r--   0 user      (1000) user      (1000)     3425 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/alertLowWine.py
--rw-r--r--   0 user      (1000) user      (1000)    18453 2021-03-14 16:56:30.000000 ikabot-6.5.8/ikabot/function/attackBarbarians.py
--rw-r--r--   0 user      (1000) user      (1000)    11184 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/autoPirate.py
--rw-r--r--   0 user      (1000) user      (1000)     9100 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/buyResources.py
--rw-r--r--   0 user      (1000) user      (1000)      700 2021-01-21 22:17:02.000000 ikabot-6.5.8/ikabot/function/checkForUpdate.py
--rw-r--r--   0 user      (1000) user      (1000)     3682 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/constructBuilding.py
--rw-r--r--   0 user      (1000) user      (1000)    17370 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/constructionList.py
--rw-r--r--   0 user      (1000) user      (1000)    51937 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/decaptchaConf.py
--rw-r--r--   0 user      (1000) user      (1000)    10516 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/distributeResources.py
--rw-r--r--   0 user      (1000) user      (1000)     5216 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/donate.py
--rw-r--r--   0 user      (1000) user      (1000)     4029 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/donationBot.py
--rw-r--r--   0 user      (1000) user      (1000)     5536 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/getStatus.py
--rw-r--r--   0 user      (1000) user      (1000)     3100 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/importExportCookie.py
--rw-r--r--   0 user      (1000) user      (1000)     2604 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/investigate.py
--rw-r--r--   0 user      (1000) user      (1000)     1708 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/killTasks.py
--rw-r--r--   0 user      (1000) user      (1000)     2083 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/loginDaily.py
--rw-r--r--   0 user      (1000) user      (1000)     3486 2021-03-15 15:07:13.000000 ikabot-6.5.8/ikabot/function/proxyConf.py
--rw-r--r--   0 user      (1000) user      (1000)     4691 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/searchForIslandSpaces.py
--rw-r--r--   0 user      (1000) user      (1000)    12388 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/sellResources.py
--rw-r--r--   0 user      (1000) user      (1000)     3867 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/sendResources.py
--rw-r--r--   0 user      (1000) user      (1000)     3706 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/shipMovements.py
--rw-r--r--   0 user      (1000) user      (1000)     9921 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/trainArmy.py
--rw-r--r--   0 user      (1000) user      (1000)      885 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/update.py
--rw-r--r--   0 user      (1000) user      (1000)     1455 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/function/vacationMode.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-15 20:48:02.715106 ikabot-6.5.8/ikabot/helpers/
--rw-r--r--   0 user      (1000) user      (1000)        0 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/helpers/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     4049 2021-03-15 20:46:15.000000 ikabot-6.5.8/ikabot/helpers/aesCipher.py
--rw-r--r--   0 user      (1000) user      (1000)     7093 2021-03-15 15:48:16.000000 ikabot-6.5.8/ikabot/helpers/botComm.py
--rw-r--r--   0 user      (1000) user      (1000)     4671 2020-10-24 17:04:59.000000 ikabot-6.5.8/ikabot/helpers/getJson.py
--rw-r--r--   0 user      (1000) user      (1000)     1500 2021-03-15 16:07:10.000000 ikabot-6.5.8/ikabot/helpers/gui.py
--rw-r--r--   0 user      (1000) user      (1000)     2244 2021-01-18 15:17:24.000000 ikabot-6.5.8/ikabot/helpers/market.py
--rw-r--r--   0 user      (1000) user      (1000)      782 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/helpers/naval.py
--rw-r--r--   0 user      (1000) user      (1000)     8135 2021-03-10 03:25:16.000000 ikabot-6.5.8/ikabot/helpers/pedirInfo.py
--rw-r--r--   0 user      (1000) user      (1000)     5848 2021-02-18 17:17:17.000000 ikabot-6.5.8/ikabot/helpers/planRoutes.py
--rw-r--r--   0 user      (1000) user      (1000)     2076 2021-01-21 22:16:36.000000 ikabot-6.5.8/ikabot/helpers/process.py
--rw-r--r--   0 user      (1000) user      (1000)     1822 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/helpers/resources.py
--rw-r--r--   0 user      (1000) user      (1000)     1210 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/helpers/signals.py
--rw-r--r--   0 user      (1000) user      (1000)     2063 2021-01-18 15:17:24.000000 ikabot-6.5.8/ikabot/helpers/varios.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-15 20:48:02.711773 ikabot-6.5.8/ikabot/locale/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-15 20:48:02.711773 ikabot-6.5.8/ikabot/locale/es/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-15 20:48:02.718439 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/
--rw-r--r--   0 user      (1000) user      (1000)     2828 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/activateMiracle.po
--rw-r--r--   0 user      (1000) user      (1000)      719 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/aesCipher.po
--rw-r--r--   0 user      (1000) user      (1000)     1995 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/alertAttacks.po
--rw-r--r--   0 user      (1000) user      (1000)     1481 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/alertLowWine.po
--rw-r--r--   0 user      (1000) user      (1000)     2219 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/botComm.po
--rw-r--r--   0 user      (1000) user      (1000)     2417 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/buyResources.po
--rw-r--r--   0 user      (1000) user      (1000)      575 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po
--rw-r--r--   0 user      (1000) user      (1000)     2432 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/command_line.po
--rw-r--r--   0 user      (1000) user      (1000)      755 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/config.po
--rw-r--r--   0 user      (1000) user      (1000)     1001 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/constructBuilding.po
--rw-r--r--   0 user      (1000) user      (1000)     4367 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/constructionList.po
--rw-r--r--   0 user      (1000) user      (1000)     1547 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/distributeResources.po
--rw-r--r--   0 user      (1000) user      (1000)     1416 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/donate.po
--rw-r--r--   0 user      (1000) user      (1000)     1628 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/donationBot.po
--rw-r--r--   0 user      (1000) user      (1000)     1673 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/getStatus.po
--rw-r--r--   0 user      (1000) user      (1000)      376 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/gui.mo
--rw-r--r--   0 user      (1000) user      (1000)      553 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/gui.po
--rw-r--r--   0 user      (1000) user      (1000)      841 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/loginDaily.po
--rw-r--r--   0 user      (1000) user      (1000)      837 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo
--rw-r--r--   0 user      (1000) user      (1000)     1255 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/pedirInfo.po
--rw-r--r--   0 user      (1000) user      (1000)     1235 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po
--rw-r--r--   0 user      (1000) user      (1000)     2792 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/sellResources.po
--rw-r--r--   0 user      (1000) user      (1000)     3510 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/sendResources.po
--rw-r--r--   0 user      (1000) user      (1000)     1253 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/session.mo
--rw-r--r--   0 user      (1000) user      (1000)     1828 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/session.po
--rw-r--r--   0 user      (1000) user      (1000)     1350 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/shipMovements.po
--rw-r--r--   0 user      (1000) user      (1000)      497 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/signals.mo
--rw-r--r--   0 user      (1000) user      (1000)      715 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/signals.po
--rw-r--r--   0 user      (1000) user      (1000)     2464 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/trainArmy.pot
--rw-r--r--   0 user      (1000) user      (1000)     3175 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/trainFleets.po
--rw-r--r--   0 user      (1000) user      (1000)     3169 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/trainTroops.po
--rw-r--r--   0 user      (1000) user      (1000)      579 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/update.po
--rw-r--r--   0 user      (1000) user      (1000)      717 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/vacationMode.po
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-15 20:48:02.718439 ikabot-6.5.8/ikabot/web/
--rw-r--r--   0 user      (1000) user      (1000)        0 2020-08-03 17:33:36.000000 ikabot-6.5.8/ikabot/web/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    25892 2021-03-15 20:46:52.000000 ikabot-6.5.8/ikabot/web/session.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-15 20:48:02.711773 ikabot-6.5.8/ikabot.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      335 2021-03-15 20:48:02.000000 ikabot-6.5.8/ikabot.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2987 2021-03-15 20:48:02.000000 ikabot-6.5.8/ikabot.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2021-03-15 20:48:02.000000 ikabot-6.5.8/ikabot.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       53 2021-03-15 20:48:02.000000 ikabot-6.5.8/ikabot.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       45 2021-03-15 20:48:02.000000 ikabot-6.5.8/ikabot.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2021-03-15 20:48:02.000000 ikabot-6.5.8/ikabot.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2021-03-15 20:48:02.718439 ikabot-6.5.8/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      586 2021-03-15 20:47:22.000000 ikabot-6.5.8/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-21 22:58:27.469874 ikabot-6.5.9/
+-rw-r--r--   0 user      (1000) user      (1000)       56 2021-03-15 21:19:27.000000 ikabot-6.5.9/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)      335 2021-03-21 22:58:27.469874 ikabot-6.5.9/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     9307 2021-03-14 17:11:15.000000 ikabot-6.5.9/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-21 22:58:27.463208 ikabot-6.5.9/ikabot/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)       44 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/__main__.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     6397 2021-03-21 22:54:31.000000 ikabot-6.5.9/ikabot/command_line.py
+-rw-r--r--   0 user      (1000) user      (1000)     1777 2021-03-21 22:56:32.000000 ikabot-6.5.9/ikabot/config.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-21 22:58:27.466541 ikabot-6.5.9/ikabot/function/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/function/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     9115 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/activateMiracle.py
+-rw-r--r--   0 user      (1000) user      (1000)     4752 2021-03-14 17:09:40.000000 ikabot-6.5.9/ikabot/function/alertAttacks.py
+-rw-r--r--   0 user      (1000) user      (1000)     3425 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/alertLowWine.py
+-rw-r--r--   0 user      (1000) user      (1000)    18453 2021-03-14 16:56:30.000000 ikabot-6.5.9/ikabot/function/attackBarbarians.py
+-rw-r--r--   0 user      (1000) user      (1000)    11184 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/autoPirate.py
+-rw-r--r--   0 user      (1000) user      (1000)     9100 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/buyResources.py
+-rw-r--r--   0 user      (1000) user      (1000)      700 2021-01-21 22:17:02.000000 ikabot-6.5.9/ikabot/function/checkForUpdate.py
+-rw-r--r--   0 user      (1000) user      (1000)     3682 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/constructBuilding.py
+-rw-r--r--   0 user      (1000) user      (1000)    17370 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/constructionList.py
+-rw-r--r--   0 user      (1000) user      (1000)    51937 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/decaptchaConf.py
+-rw-r--r--   0 user      (1000) user      (1000)    10516 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/distributeResources.py
+-rw-r--r--   0 user      (1000) user      (1000)     5216 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/donate.py
+-rw-r--r--   0 user      (1000) user      (1000)     4029 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/donationBot.py
+-rw-r--r--   0 user      (1000) user      (1000)     5536 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/getStatus.py
+-rw-r--r--   0 user      (1000) user      (1000)     3100 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/importExportCookie.py
+-rw-r--r--   0 user      (1000) user      (1000)     2604 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/investigate.py
+-rw-r--r--   0 user      (1000) user      (1000)     1708 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/killTasks.py
+-rw-r--r--   0 user      (1000) user      (1000)     2083 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/loginDaily.py
+-rw-r--r--   0 user      (1000) user      (1000)     3515 2021-03-21 22:52:13.000000 ikabot-6.5.9/ikabot/function/proxyConf.py
+-rw-r--r--   0 user      (1000) user      (1000)     4691 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/searchForIslandSpaces.py
+-rw-r--r--   0 user      (1000) user      (1000)    12388 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/sellResources.py
+-rw-r--r--   0 user      (1000) user      (1000)     3867 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/sendResources.py
+-rw-r--r--   0 user      (1000) user      (1000)     3706 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/shipMovements.py
+-rw-r--r--   0 user      (1000) user      (1000)     9921 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/trainArmy.py
+-rw-r--r--   0 user      (1000) user      (1000)      885 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/update.py
+-rw-r--r--   0 user      (1000) user      (1000)     1455 2021-03-10 03:25:16.000000 ikabot-6.5.9/ikabot/function/vacationMode.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-21 22:58:27.466541 ikabot-6.5.9/ikabot/helpers/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/helpers/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     4049 2021-03-15 20:46:15.000000 ikabot-6.5.9/ikabot/helpers/aesCipher.py
+-rw-r--r--   0 user      (1000) user      (1000)     7093 2021-03-15 15:48:16.000000 ikabot-6.5.9/ikabot/helpers/botComm.py
+-rw-r--r--   0 user      (1000) user      (1000)     4671 2021-03-16 21:25:35.000000 ikabot-6.5.9/ikabot/helpers/getJson.py
+-rw-r--r--   0 user      (1000) user      (1000)     1500 2021-03-15 16:07:10.000000 ikabot-6.5.9/ikabot/helpers/gui.py
+-rw-r--r--   0 user      (1000) user      (1000)     2250 2021-03-16 21:25:56.000000 ikabot-6.5.9/ikabot/helpers/market.py
+-rw-r--r--   0 user      (1000) user      (1000)      784 2021-03-16 21:26:03.000000 ikabot-6.5.9/ikabot/helpers/naval.py
+-rw-r--r--   0 user      (1000) user      (1000)     8091 2021-03-16 21:28:11.000000 ikabot-6.5.9/ikabot/helpers/pedirInfo.py
+-rw-r--r--   0 user      (1000) user      (1000)     5849 2021-03-16 21:28:38.000000 ikabot-6.5.9/ikabot/helpers/planRoutes.py
+-rw-r--r--   0 user      (1000) user      (1000)     2083 2021-03-16 21:29:02.000000 ikabot-6.5.9/ikabot/helpers/process.py
+-rw-r--r--   0 user      (1000) user      (1000)     1820 2021-03-16 21:29:20.000000 ikabot-6.5.9/ikabot/helpers/resources.py
+-rw-r--r--   0 user      (1000) user      (1000)     1149 2021-03-16 21:29:57.000000 ikabot-6.5.9/ikabot/helpers/signals.py
+-rw-r--r--   0 user      (1000) user      (1000)     2066 2021-03-16 21:30:12.000000 ikabot-6.5.9/ikabot/helpers/varios.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-21 22:58:27.463208 ikabot-6.5.9/ikabot/locale/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-21 22:58:27.463208 ikabot-6.5.9/ikabot/locale/es/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-21 22:58:27.469874 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/
+-rw-r--r--   0 user      (1000) user      (1000)     2828 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/activateMiracle.po
+-rw-r--r--   0 user      (1000) user      (1000)      719 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/aesCipher.po
+-rw-r--r--   0 user      (1000) user      (1000)     1995 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/alertAttacks.po
+-rw-r--r--   0 user      (1000) user      (1000)     1481 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/alertLowWine.po
+-rw-r--r--   0 user      (1000) user      (1000)     2219 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/botComm.po
+-rw-r--r--   0 user      (1000) user      (1000)     2417 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/buyResources.po
+-rw-r--r--   0 user      (1000) user      (1000)      575 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po
+-rw-r--r--   0 user      (1000) user      (1000)     2432 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/command_line.po
+-rw-r--r--   0 user      (1000) user      (1000)      755 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/config.po
+-rw-r--r--   0 user      (1000) user      (1000)     1001 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/constructBuilding.po
+-rw-r--r--   0 user      (1000) user      (1000)     4367 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/constructionList.po
+-rw-r--r--   0 user      (1000) user      (1000)     1547 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/distributeResources.po
+-rw-r--r--   0 user      (1000) user      (1000)     1416 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/donate.po
+-rw-r--r--   0 user      (1000) user      (1000)     1628 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/donationBot.po
+-rw-r--r--   0 user      (1000) user      (1000)     1673 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/getStatus.po
+-rw-r--r--   0 user      (1000) user      (1000)      376 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/gui.mo
+-rw-r--r--   0 user      (1000) user      (1000)      553 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/gui.po
+-rw-r--r--   0 user      (1000) user      (1000)      841 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/loginDaily.po
+-rw-r--r--   0 user      (1000) user      (1000)      837 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo
+-rw-r--r--   0 user      (1000) user      (1000)     1255 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/pedirInfo.po
+-rw-r--r--   0 user      (1000) user      (1000)     1235 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po
+-rw-r--r--   0 user      (1000) user      (1000)     2792 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/sellResources.po
+-rw-r--r--   0 user      (1000) user      (1000)     3510 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/sendResources.po
+-rw-r--r--   0 user      (1000) user      (1000)     1253 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/session.mo
+-rw-r--r--   0 user      (1000) user      (1000)     1828 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/session.po
+-rw-r--r--   0 user      (1000) user      (1000)     1350 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/shipMovements.po
+-rw-r--r--   0 user      (1000) user      (1000)      497 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/signals.mo
+-rw-r--r--   0 user      (1000) user      (1000)      715 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/signals.po
+-rw-r--r--   0 user      (1000) user      (1000)     2464 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/trainArmy.pot
+-rw-r--r--   0 user      (1000) user      (1000)     3175 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/trainFleets.po
+-rw-r--r--   0 user      (1000) user      (1000)     3169 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/trainTroops.po
+-rw-r--r--   0 user      (1000) user      (1000)      579 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/update.po
+-rw-r--r--   0 user      (1000) user      (1000)      717 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/vacationMode.po
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-21 22:58:27.469874 ikabot-6.5.9/ikabot/web/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2020-08-03 17:33:36.000000 ikabot-6.5.9/ikabot/web/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    26266 2021-03-21 22:52:41.000000 ikabot-6.5.9/ikabot/web/session.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-21 22:58:27.466541 ikabot-6.5.9/ikabot.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      335 2021-03-21 22:58:27.000000 ikabot-6.5.9/ikabot.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2987 2021-03-21 22:58:27.000000 ikabot-6.5.9/ikabot.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2021-03-21 22:58:27.000000 ikabot-6.5.9/ikabot.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       53 2021-03-21 22:58:27.000000 ikabot-6.5.9/ikabot.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)       45 2021-03-21 22:58:27.000000 ikabot-6.5.9/ikabot.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        7 2021-03-21 22:58:27.000000 ikabot-6.5.9/ikabot.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2021-03-21 22:58:27.469874 ikabot-6.5.9/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      568 2021-03-21 22:36:20.000000 ikabot-6.5.9/setup.py
```

### Comparing `ikabot-6.5.8/README.md` & `ikabot-6.5.9/README.md`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/command_line.py` & `ikabot-6.5.9/ikabot/command_line.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,22 +36,18 @@
 from ikabot.function.autoPirate import autoPirate
 from ikabot.function.investigate import investigate
 from ikabot.function.attackBarbarians import attackBarbarians
 from ikabot.function.proxyConf import proxyConf, show_proxy
 from ikabot.function.killTasks import killTasks 
 from ikabot.function.decaptchaConf import decaptchaConf
 
-t = gettext.translation('command_line',
-                        localedir,
-                        languages=languages,
-                        fallback=True)
+t = gettext.translation('command_line', localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
-
 def menu(session, checkUpdate=True):
 	"""
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 	checkUpdate : bool
 	"""
@@ -60,34 +56,34 @@
 
 	show_proxy(session)
 
 	banner()
 
 	process_list = updateProcessList(session)
 	if len(process_list) > 0:
-		print('|{:^6}|{:^35}|{:^15}|'.format('pid','task','date'))
+		print('|{:^6}|{:^35}|{:^15}|'.format('pid', 'task', 'date'))
 		print('_'*60)
 		for process in process_list:
 			if 'date' in process:
-				print('|{:^6}|{:^35}|{:^15}|'.format(process['pid'],process['action'],datetime.datetime.fromtimestamp(process['date']).strftime('%b %d %H:%M:%S')))
+				print('|{:^6}|{:^35}|{:^15}|'.format(process['pid'], process['action'], datetime.datetime.fromtimestamp(process['date']).strftime('%b %d %H:%M:%S')))
 			else:
-				print('|{:^6}|{:^35}|'.format(process['pid'],process['action']))
+				print('|{:^6}|{:^35}|'.format(process['pid'], process['action']))
 
 		print('')
 
 	menu_actions = {
-		1 :			constructionList,
-		2 :			sendResources,
-		3 :			distributeResources,
-		4 :			getStatus,
-		5 :			donate,
-		6 :			searchForIslandSpaces,
-		7 :			loginDaily,
-		8 :			alertAttacks,
-		9 :			donationBot,
+		1:			constructionList,
+		2:			sendResources,
+		3:			distributeResources,
+		4:			getStatus,
+		5:			donate,
+		6:			searchForIslandSpaces,
+		7:			loginDaily,
+		8:			alertAttacks,
+		9:			donationBot,
 		10:			alertLowWine,
 		11:			buyResources,
 		12:			sellResources,
 		13:			vacationMode,
 		14:			activateMiracle,
 		15:			trainArmy,
 		16:			shipMovements,
@@ -129,54 +125,55 @@
 	print(_('(23) Options / Settings'))
 	total_options = len(menu_actions) + 1
 	selected = read(min=0, max=total_options, digit=True)
 
 	if selected == 23:
 		banner()
 		print(_('(0) Back'))
-		print(_('(24) Configure Proxy'))
+		print(_('(1) Configure Proxy'))
 		if telegramDataIsValid(session):
-			print(_('(25) Change the Telegram data'))
+			print(_('(2) Change the Telegram data'))
 		else:
-			print(_('(25) Enter the Telegram data'))
-		print(_('(26) Kill tasks'))
-		print(_('(27) Configure captcha resolver'))
-
-		selected = read(min=0, max=total_options, digit=True)
-		if selected in [0,23]:
-			menu(session, checkUpdate = False)
-		
-		
+			print(_('(2) Enter the Telegram data'))
+		print(_('(3) Kill tasks'))
+		print(_('(4) Configure captcha resolver'))
+
+		selected = read(min=0, max=4, digit=True)
+		if selected > 0:
+			selected += 23
+
 	if selected != 0:
 		try:
-			event = multiprocessing.Event() #creates a new event
+			event = multiprocessing.Event()  # creates a new event
 			process = multiprocessing.Process(target=menu_actions[selected], args=(session, event, sys.stdin.fileno(), config.predetermined_input), name=menu_actions[selected].__name__)
 			process.start()
-			process_list.append({'pid': process.pid, 'action': menu_actions[selected].__name__, 'date' : time.time() })
+			process_list.append({'pid': process.pid, 'action': menu_actions[selected].__name__, 'date': time.time()})
 			updateProcessList(session, programprocesslist=process_list)
-			event.wait() #waits for the process to fire the event that's been given to it. When it does  this process gets back control of the command line and asks user for more input
+			event.wait()  # waits for the process to fire the event that's been given to it. When it does  this process gets back control of the command line and asks user for more input
 		except KeyboardInterrupt:
 			pass
 		menu(session, checkUpdate=False)
 	else:
 		if isWindows:
 			# in unix, you can exit ikabot and close the terminal and the processes will continue to execute
 			# in windows, you can exit ikabot but if you close the terminal, the processes will die
 			print(_('Closing this console will kill the processes.'))
 			enter()
 		clear()
-		os._exit(0) #kills the process which executes this statement, but it does not kill it's child processes
+		os._exit(0)  # kills the process which executes this statement, but it does not kill it's child processes
+
 
 def init():
 	home = 'USERPROFILE' if isWindows else 'HOME'
 	os.chdir(os.getenv(home))
 	if not os.path.isfile(ikaFile):
 		open(ikaFile, 'w')
 		os.chmod(ikaFile, 0o600)
 
+
 def start():
 	init()
 	for arg in sys.argv:
 		try:
 			config.predetermined_input.append(int(arg))
 		except ValueError:
 			config.predetermined_input.append(arg)
@@ -185,24 +182,23 @@
 	session = Session()
 	try:
 		menu(session)
 	finally:
 		clear()
 		session.logout()
 
+
 def main():
 	manager = multiprocessing.Manager()
 	predetermined_input = manager.list()
 	config.predetermined_input = predetermined_input
 	try:
 		start()
 	except KeyboardInterrupt:
 		clear()
 
 
-
 if __name__ == '__main__':
-
-	if sys.platform.startswith('win'):
 	# On Windows calling this function is necessary.
+	if sys.platform.startswith('win'):
 		multiprocessing.freeze_support()
 	main()
```

### Comparing `ikabot-6.5.8/ikabot/config.py` & `ikabot-6.5.9/ikabot/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,50 +8,48 @@
 if 'es_' in local:
 	languages = ['es']
 else:
 	languages = ['en']
 languages = ['none']
 
 localedir = os.path.join(os.path.abspath(os.path.dirname(__file__)), 'locale')
-t = gettext.translation('config',
-                        localedir,
-                        languages=languages,
-                        fallback=True)
+t = gettext.translation('config', localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 # only use common browsers
 if random.randint(0, 1) == 0:
 	user_agent = 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.83 Safari/537.36'
 else:
 	user_agent = 'Mozilla/5.0 (X11; Linux x86_64; rv:80.0) Gecko/20100101 Firefox/80.0'
 
 update_msg = ''
 
 isWindows = os.name == 'nt'
 
+do_ssl_verify = True
 ids_cache = None
 cities_cache = None
 menu_cities = ''
 infoUser = ''
 ikaFile = '.ikabot'
 city_url = 'view=city&cityId='
 island_url = 'view=island&islandId='
 prompt = ' >>  '
 materials_names = [_('Wood'), _('Wine'), _('Marble'), _('Cristal'), _('Sulfur')]
 materials_names_english = ['Wood', 'Wine', 'Marble', 'Cristal', 'Sulfur']
 materials_names_tec = ['wood', 'wine', 'marble', 'glass', 'sulfur']
 tradegoods_names = [_('Saw mill'), _('Vineyard'), _('Quarry'), _('Crystal Mine'), _('Sulfur Pit')]
 ConnectionError_wait = 5 * 60
 actionRequest = 'REQUESTID'
-piracyMissionToBuildingLevel = {1 : 1, 2 : 3, 3 : 5, 4 : 7, 5 : 9, 6 : 11, 7 : 13, 8 : 15, 9 : 17}
-piracyMissionWaitingTime = {1 : 150, 2 : 450, 3 : 900, 4 : 1800, 5 : 3600, 6 : 7200, 7 : 14400, 8 : 28800, 9 : 57600}
+piracyMissionToBuildingLevel = {1: 1, 2: 3, 3: 5, 4: 7, 5: 9, 6: 11, 7: 13, 8: 15, 9: 17}
+piracyMissionWaitingTime = {1: 150, 2: 450, 3: 900, 4: 1800, 5: 3600, 6: 7200, 7: 14400, 8: 28800, 9: 57600}
 predetermined_input = []
-debugON_alertAttacks          = False
-debugON_alertLowWine          = False
-debugON_donationBot           = False
+debugON_alertAttacks = False
+debugON_alertLowWine = False
+debugON_donationBot = False
 debugON_searchForIslandSpaces = False
-debugON_loginDaily            = False
-debugON_enviarVino            = False
-debugON_sendResources         = False
-debugON_constructionList      = False
-debugON_buyResources          = False
-debugON_activateMiracle       = False
+debugON_loginDaily = False
+debugON_enviarVino = False
+debugON_sendResources = False
+debugON_constructionList = False
+debugON_buyResources = False
+debugON_activateMiracle = False
```

### Comparing `ikabot-6.5.8/ikabot/function/activateMiracle.py` & `ikabot-6.5.9/ikabot/function/activateMiracle.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/alertAttacks.py` & `ikabot-6.5.9/ikabot/function/alertAttacks.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/alertLowWine.py` & `ikabot-6.5.9/ikabot/function/alertLowWine.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/attackBarbarians.py` & `ikabot-6.5.9/ikabot/function/attackBarbarians.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/autoPirate.py` & `ikabot-6.5.9/ikabot/function/autoPirate.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/buyResources.py` & `ikabot-6.5.9/ikabot/function/buyResources.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/checkForUpdate.py` & `ikabot-6.5.9/ikabot/function/checkForUpdate.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/constructBuilding.py` & `ikabot-6.5.9/ikabot/function/constructBuilding.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/constructionList.py` & `ikabot-6.5.9/ikabot/function/constructionList.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/decaptchaConf.py` & `ikabot-6.5.9/ikabot/function/decaptchaConf.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/distributeResources.py` & `ikabot-6.5.9/ikabot/function/distributeResources.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/donate.py` & `ikabot-6.5.9/ikabot/function/donate.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/donationBot.py` & `ikabot-6.5.9/ikabot/function/donationBot.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/getStatus.py` & `ikabot-6.5.9/ikabot/function/getStatus.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/importExportCookie.py` & `ikabot-6.5.9/ikabot/function/importExportCookie.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/investigate.py` & `ikabot-6.5.9/ikabot/function/investigate.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/killTasks.py` & `ikabot-6.5.9/ikabot/function/killTasks.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/loginDaily.py` & `ikabot-6.5.9/ikabot/function/loginDaily.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/proxyConf.py` & `ikabot-6.5.9/ikabot/function/proxyConf.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 	elif msg in config.update_msg:
 		# delete old proxy message
 		config.update_msg = config.update_msg.replace('\n'.join(config.update_msg.split('\n')[-2:]), '')
 
 
 def test_proxy(proxy_dict):
 	try:
-		requests.get('https://lobby.ikariam.gameforge.com/', proxies=proxy_dict)
+		requests.get('https://lobby.ikariam.gameforge.com/', proxies=proxy_dict, verify=config.do_ssl_verify)
 	except Exception:
 		return False
 	return True
 
 
 def read_proxy():
 	print(_('Enter the proxy (examples: socks5://127.0.0.1:9050, https://45.117.163.22:8080):'))
```

### Comparing `ikabot-6.5.8/ikabot/function/searchForIslandSpaces.py` & `ikabot-6.5.9/ikabot/function/searchForIslandSpaces.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/sellResources.py` & `ikabot-6.5.9/ikabot/function/sellResources.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/sendResources.py` & `ikabot-6.5.9/ikabot/function/sendResources.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/shipMovements.py` & `ikabot-6.5.9/ikabot/function/shipMovements.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/trainArmy.py` & `ikabot-6.5.9/ikabot/function/trainArmy.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/update.py` & `ikabot-6.5.9/ikabot/function/update.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/function/vacationMode.py` & `ikabot-6.5.9/ikabot/function/vacationMode.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/helpers/aesCipher.py` & `ikabot-6.5.9/ikabot/helpers/aesCipher.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/helpers/botComm.py` & `ikabot-6.5.9/ikabot/helpers/botComm.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/helpers/getJson.py` & `ikabot-6.5.9/ikabot/helpers/getJson.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import re
 import json
 from ikabot.helpers.resources import *
 
+
 def getFreeCitizens(html):
 	"""This function is used in the ``getCity`` function to determine the amount of free (idle) citizens in the given city.
 	Parameters
 	----------
 	html : str
 		a string representing html which is returned when sending a get request to view a city.
 
@@ -16,32 +17,34 @@
 	-------
 	freeCitizens : int
 		an integer representing the amount of free citizens in the given city.
 	"""
 	ciudadanosDisp = re.search(r'js_GlobalMenu_citizens">(.*?)</span>', html).group(1)
 	return int(ciudadanosDisp.replace(',', '').replace('.', ''))
 
+
 def onSale(html):
 	"""This function is used in the ``getCity`` function to determine the amount of each resource which is on sale in the branch office
 	Parameters
 	----------
 	html : str
 		a string representing html which is returned when sending a get request to view a city.
 
 	Returns
 	-------
 	onSale : list[int]
 		a list containing 5 integers each of which representing the amount of that particular resource which is on sale in the given city. For more information about the order of the resources, refer to ``config.py``
 	"""
 	rta = re.search(r'branchOfficeResources: JSON\.parse\(\'{\\"resource\\":\\"(\d+)\\",\\"1\\":\\"(\d+)\\",\\"2\\":\\"(\d+)\\",\\"3\\":\\"(\d+)\\",\\"4\\":\\"(\d+)\\"}\'\)', html)
 	if rta:
-		return [ int(rta.group(1)), int(rta.group(2)), int(rta.group(3)), int(rta.group(4)), int(rta.group(5))]
+		return [int(rta.group(1)), int(rta.group(2)), int(rta.group(3)), int(rta.group(4)), int(rta.group(5))]
 	else:
 		return [0, 0, 0, 0, 0]
 
+
 def getIsland(html):
 	"""This function uses the html passed to it as a string to extract, parse and return an Island object
 	Parameters
 	----------
 	html : str
 		the html returned when a get request to view the island is made. This request can be made with the following statement: ``s.get(urlIsla + islandId)``, where ``urlIsla`` is a string defined in ``config.py`` and ``islandId`` is the id of the island.
 
@@ -53,23 +56,23 @@
 	isla = re.search(r'\[\["updateBackgroundData",([\s\S]*?),"specialServerBadges', html).group(1) + '}'
 
 	isla = isla.replace('buildplace', 'empty')
 	isla = isla.replace('xCoord', 'x')
 	isla = isla.replace('yCoord', 'y')
 	isla = isla.replace(',"owner', ',"')
 
-
 	# {"id":idIsla,"name":nombreIsla,"x":,"y":,"good":numeroBien,"woodLv":,"goodLv":,"wonder":numeroWonder, "wonderName": "nombreDelMilagro","wonderLv":"5","cities":[{"type":"city","name":cityName,"id":cityId,"level":lvIntendencia,"Id":playerId,"Name":playerName,"AllyId":,"AllyTag":,"state":"vacation"},...}}
 	isla = json.loads(isla, strict=False)
 	isla['tipo'] = re.search(r'"tradegood":"(\d)"', html).group(1)
 	isla['x'] = int(isla['x'])
 	isla['y'] = int(isla['y'])
 
 	return isla
 
+
 def getCity(html):
 	"""This function uses the ``html`` passed to it as a string to extract, parse and return a City object
 	Parameters
 	----------
 	html : str
 		the html returned when a get request to view the city is made. This request can be made with the following statement: ``s.get(urlCiudad + id)``, where urlCiudad is a string defined in ``config.py`` and id is the id of the city.
 
@@ -108,10 +111,10 @@
 	city['recursos'] = getAvailableResources(html, num=True)
 	city['storageCapacity'] = getWarehouseCapacity(html)
 	city['ciudadanosDisp'] = getFreeCitizens(html)
 	city['consumo'] = getWineConsumption(html)
 	city['enventa'] = onSale(html)
 	city['freeSpaceForResources'] = []
 	for i in range(5):
-		city['freeSpaceForResources'].append( city['storageCapacity'] - city['recursos'][i] - city['enventa'][i] )
+		city['freeSpaceForResources'].append(city['storageCapacity'] - city['recursos'][i] - city['enventa'][i])
 
 	return city
```

### Comparing `ikabot-6.5.8/ikabot/helpers/gui.py` & `ikabot-6.5.9/ikabot/helpers/gui.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/helpers/market.py` & `ikabot-6.5.9/ikabot/helpers/market.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import re
 import json
 from ikabot.config import *
 from ikabot.helpers.getJson import getCity
 from ikabot.helpers.pedirInfo import getIdsOfCities
 
+
 def getCommercialCities(session):
 	"""
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 
 	Returns
@@ -28,37 +29,41 @@
 				html = getMarketHtml(session, city)
 				positions = re.findall(r'<option.*?>(\d+)</option>', html)
 				city['rango'] = int(positions[-1])
 				commercial_cities.append(city)
 				break
 	return commercial_cities
 
+
 def getMarketHtml(session, city):
 	"""
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 	city : dict
 	"""
 	url = 'view=branchOffice&cityId={}&position={:d}&currentCityId={}&backgroundView=city&actionRequest={}&ajax=1'.format(city['id'], city['pos'], city['id'], actionRequest)
 	data = session.post(url)
 	json_data = json.loads(data, strict=False)
 	return json_data[1][1][1]
 
+
 def storageCapacityOfMarket(html):
 	match = re.search(r'var\s*storageCapacity\s*=\s*(\d+);', html)
 	if match:
 		return int(match.group(1))
 	else:
 		return 0
 
+
 def onSellInMarket(html):
 	mad, vin, mar, cri, azu = re.findall(r'<input type="text" class="textfield"\s*size="\d+"\s*name=".*?"\s*id=".*?"\s*value="(\d+)"', html)
 	return [int(mad), int(vin), int(mar), int(cri), int(azu)]
 
+
 def getGold(session, city):
 	"""
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 	city : dict
 	Returns
@@ -67,9 +72,9 @@
 	"""
 	url = 'view=finances&backgroundView=city&currentCityId={}&templateView=finances&actionRequest={}&ajax=1'.format(city['id'], actionRequest)
 	data = session.post(url)
 	json_data = json.loads(data, strict=False)
 	gold = json_data[0][1]['headerData']['gold']
 	gold = gold.split('.')[0]
 	gold = int(gold)
-	gold_production = json_data[0][1]['headerData']['scientistsUpkeep'] + json_data[0][1]['headerData']['income'] +json_data[0][1]['headerData']['upkeep']
+	gold_production = json_data[0][1]['headerData']['scientistsUpkeep'] + json_data[0][1]['headerData']['income'] + json_data[0][1]['headerData']['upkeep']
 	return gold, int(gold_production)
```

### Comparing `ikabot-6.5.8/ikabot/helpers/naval.py` & `ikabot-6.5.9/ikabot/helpers/naval.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import re
 
+
 def getAvailableShips(session):
 	"""Function that returns the total number of free (available) ships
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 		Session object
 
@@ -14,14 +15,15 @@
 	-------
 	ships : int
 		number of currently available ships
 	"""
 	html = session.get()
 	return int(re.search(r'GlobalMenu_freeTransporters">(\d+)<', html).group(1))
 
+
 def getTotalShips(session):
 	"""Function that returns the total number of ships, regardless of if they're available or not
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 		Session object
```

### Comparing `ikabot-6.5.8/ikabot/helpers/pedirInfo.py` & `ikabot-6.5.9/ikabot/helpers/pedirInfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,21 @@
 import os
 from ikabot import config
 from decimal import *
 from ikabot.config import *
 from ikabot.helpers.getJson import *
 from ikabot.helpers.gui import *
 
-t = gettext.translation('pedirInfo',
-                        localedir,
-                        languages=languages,
-                        fallback=True)
+t = gettext.translation('pedirInfo', localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 getcontext().prec = 30
 
-def read(min=None, max=None, digit=False, msg=prompt, values=None, empty=False, additionalValues=None, default=None): # user input
+
+def read(min=None, max=None, digit=False, msg=prompt, values=None, empty=False, additionalValues=None, default=None):  # user input
 	"""Reads input from user
 	Parameters
 	----------
 	min : int
 		smallest number acceptable as input
 	max : int
 		greatest number acceptable as input
@@ -41,22 +39,22 @@
 
 	Returns
 	-------
 	result : int | str
 		int representing the user's choice
 	"""
 	try:
-		if len(config.predetermined_input) !=0:
+		if len(config.predetermined_input) != 0:
 			return config.predetermined_input.pop(0)
 	except Exception:
 		pass
 
 	def _invalid():
-		print('\033[1A\033[K', end="") # remove line
-		return read(min, max, digit, msg, values, additionalValues = additionalValues)
+		print('\033[1A\033[K', end="")  # remove line
+		return read(min, max, digit, msg, values, additionalValues=additionalValues)
 
 	try:
 		read_input = input(msg)
 	except EOFError:
 		return _invalid()
 
 	if additionalValues is not None and read_input in additionalValues:
@@ -80,14 +78,15 @@
 		return _invalid()
 	if max is not None and read_input > max:
 		return _invalid()
 	if values is not None and read_input not in values:
 		return _invalid()
 	return read_input
 
+
 def chooseCity(session, foreign=False):
 	"""Prompts the user to chose a city
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 		Session object
 	foreign : bool
@@ -102,15 +101,18 @@
 	(ids, cities) = getIdsOfCities(session)
 	if menu_cities == '':
 		longest_city_name_length = 0
 		for city_id in ids:
 			length = len(cities[city_id]['name'])
 			if length > longest_city_name_length:
 				longest_city_name_length = length
-		pad = lambda city_name: ' ' * (longest_city_name_length - len(city_name) + 2)
+
+		def pad(city_name):
+			return ' ' * (longest_city_name_length - len(city_name) + 2)
+
 		resources_abbreviations = {'1': _('(W)'), '2': _('(M)'), '3': _('(C)'), '4': _('(S)')}
 
 		i = 0
 		if foreign:
 			print(_(' 0: foreign city'))
 		else:
 			print('')
@@ -137,50 +139,53 @@
 		selected_city_index = read(min=1, max=len(ids))
 	if selected_city_index == 0:
 		return chooseForeignCity(session)
 	else:
 		html = session.get(city_url + ids[selected_city_index - 1])
 		return getCity(html)
 
+
 def chooseForeignCity(session):
 	"""Prompts the user to select an island, and a city on that island (is only used in chooseCity)
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 		Session object
 
 	Returns
 	-------
-	 city : City
+	city : City
 		a city object representing the city the user chose
 	"""
 	banner()
 	x = read(msg='coordinate x:', digit=True)
 	y = read(msg='coordinate y:', digit=True)
 	print('')
 	url = 'view=worldmap_iso&islandX={}&islandY={}&oldBackgroundView=island&islandWorldviewScale=1'.format(x, y)
 	html = session.get(url)
 	try:
 		islands_json = re.search(r'jsonData = \'(.*?)\';', html).group(1)
 		islands_json = json.loads(islands_json, strict=False)
 		island_id = islands_json['data'][str(x)][str(y)][0]
-	except:
+	except Exception:
 		print(_('Incorrect coordinates'))
 		enter()
 		banner()
 		return chooseCity(session, foreign=True)
 	html = session.get(island_url + island_id)
 	island = getIsland(html)
 	longest_city_name_length = 0
 	for city in island['cities']:
 		if city['type'] == 'city':
 			city_name_length = len(city['name'])
 			if city_name_length > longest_city_name_length:
 				longest_city_name_length = city_name_length
-	pad = lambda name: ' ' * (longest_city_name_length - len(name) + 2)
+
+	def pad(name):
+		return ' ' * (longest_city_name_length - len(name) + 2)
 	i = 0
 	city_options = []
 	for city in island['cities']:
 		if city['type'] == 'city' and city['state'] == '' and city['Name'] != session.username:
 			i += 1
 			num = ' ' + str(i) if i < 10 else str(i)
 			print('{}: {}{}({})'.format(num, city['name'], pad(city['name']), city['Name']))
@@ -192,14 +197,15 @@
 	selected_city_index = read(min=1, max=i)
 	city = city_options[selected_city_index - 1]
 	city['islandId'] = island['id']
 	city['cityName'] = city['name']
 	city['propia'] = False
 	return city
 
+
 def askForValue(text, max):
 	"""Displays text and asks the user to enter a value between 0 and max
 
 	Parameters
 	----------
 	text : str
 		text to be displayed when asking the user for input
@@ -213,14 +219,15 @@
 		if the user has inputed nothing, 0 will be returned instead
 	"""
 	var = read(msg=text, min=0, max=max, empty=True)
 	if var == '':
 		var = 0
 	return var
 
+
 def getIdsOfCities(session, all=False):
 	"""Gets the user's cities
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 		Session object
 	all : bool
@@ -241,23 +248,24 @@
 		cities_cache = json.loads(cities_cache, strict=False)
 
 		ids_cache = [city_id for city_id in cities_cache]
 		ids_cache = sorted(ids_cache)
 
 	# {'coords': '[x:y] ', 'id': idCiudad, 'tradegood': '..', 'name': 'nomberCiudad', 'relationship': 'ownCity'|'occupiedCities'|..}
 	if all is False:
-		ids_own   = [city_id for city_id in cities_cache if cities_cache[city_id]['relationship'] == 'ownCity']
+		ids_own = [city_id for city_id in cities_cache if cities_cache[city_id]['relationship'] == 'ownCity']
 		ids_other = [city_id for city_id in cities_cache if cities_cache[city_id]['relationship'] != 'ownCity']
 		own_cities = cities_cache.copy()
 		for id in ids_other:
 			del own_cities[id]
 		return ids_own, own_cities
 	else:
 		return ids_cache, cities_cache
 
+
 def getIslandsIds(session):
 	"""Gets the IDs of islands the user has cities on
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 		Session object
```

### Comparing `ikabot-6.5.8/ikabot/helpers/planRoutes.py` & `ikabot-6.5.9/ikabot/helpers/planRoutes.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import json
 from decimal import *
 from ikabot.config import *
 from ikabot.helpers.varios import wait
 from ikabot.helpers.getJson import getCity
 from ikabot.helpers.naval import *
 
+
 def sendGoods(session, originCityId, destinationCityId, islandId, ships, send):
 	"""This function will execute one route
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 		Session object
 	originCityId : int
@@ -48,14 +49,15 @@
 		resp = json.loads(resp, strict=False)
 		if resp[3][1][0]['type'] == 10:
 			break
 		elif resp[3][1][0]['type'] == 11:
 			wait(getMinimumWaitingTime(session))
 		time.sleep(5)
 
+
 def executeRoutes(session, routes):
 	"""This function will execute all the routes passed to it, regardless if there are enough ships available to do so
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 		Session object
 	routes : list
@@ -93,14 +95,15 @@
 				# wait an hour and try again
 				wait(60 * 60)
 				continue
 
 			available_ships = int(math.ceil((Decimal(resources_to_send) / Decimal(500))))
 			sendGoods(session, origin_city['id'], destination_city_id, island_id, available_ships, send)
 
+
 def getMinimumWaitingTime(session):
 	"""This function returns the time needed to wait for the closest fleet to arrive. If all ships are unavailable, this represents the minimum time needed to wait for any ships to become available. A random waiting time between 0 and 10 seconds is added to the waiting time to avoid race conditions between multiple concurrently running processes.
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 		Session object
 
@@ -113,22 +116,23 @@
 	idCiudad = re.search(r'currentCityId:\s(\d+),', html).group(1)
 	url = 'view=militaryAdvisor&oldView=city&oldBackgroundView=city&backgroundView=city&currentCityId={}&actionRequest={}&ajax=1'.format(idCiudad, actionRequest)
 	posted = session.post(url)
 	postdata = json.loads(posted, strict=False)
 	militaryMovements = postdata[1][1][2]['viewScriptParams']['militaryAndFleetMovements']
 	current_time = int(postdata[0][1]['time'])
 	delivered_times = []
-	for militaryMovement in [ mv for mv in militaryMovements if mv['isOwnArmyOrFleet'] ]:
+	for militaryMovement in [mv for mv in militaryMovements if mv['isOwnArmyOrFleet']]:
 		remaining_time = int(militaryMovement['eventTime']) - current_time
 		delivered_times.append(remaining_time)
 	if delivered_times:
-		return min(delivered_times) + random.uniform(0,10)
+		return min(delivered_times) + random.uniform(0, 10)
 	else:
 		return 0
 
+
 def waitForArrival(session):
 	"""This function will return the number of available ships, and if there aren't any, it will wait for the closest fleet to arrive and then return the number of available ships
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 		Session object
 
@@ -136,10 +140,10 @@
 	-------
 	ships : int
 		number of available ships
 	"""
 	available_ships = getAvailableShips(session)
 	while available_ships == 0:
 		minimum_waiting_time_for_ship = getMinimumWaitingTime(session)
-		wait( minimum_waiting_time_for_ship )
+		wait(minimum_waiting_time_for_ship)
 		available_ships = getAvailableShips(session)
 	return available_ships
```

### Comparing `ikabot-6.5.8/ikabot/helpers/process.py` & `ikabot-6.5.9/ikabot/helpers/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,31 +4,34 @@
 import os
 import json
 import psutil
 import subprocess
 from ikabot.config import *
 from ikabot.helpers.signals import deactivate_sigint
 
+
 def set_child_mode(session):
 	"""
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 	"""
 	session.padre = False
 	deactivate_sigint()
 
+
 def run(command):
 	ret = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE).stdout.read()
 	try:
 		return ret.decode('utf-8').strip()
-	except:
+	except Exception:
 		return ret
 
-def updateProcessList(session, programprocesslist = []):
+
+def updateProcessList(session, programprocesslist=[]):
 	"""This function will return data about all the active ikabot processes. If it is passed the ``programprocesslist`` argument, it will write new processes from that list to the .ikabot file
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 		Session object
 	programprocesslist : list[dict]
 		a list of dictionaries containing relevant data about a running ikabot process ('pid', 'proxies' and 'action')
@@ -43,18 +46,18 @@
 	try:
 		fileList = sessionData['processList']
 	except KeyError:
 		fileList = []
 
 	# check it's still running
 	runningIkabotProcessList = []
-	ika_process = psutil.Process(pid = os.getpid()).name()
+	ika_process = psutil.Process(pid=os.getpid()).name()
 	for process in fileList:
 		try:
-			proc = psutil.Process(pid = process['pid'])
+			proc = psutil.Process(pid=process['pid'])
 		except psutil.NoSuchProcess:
 			continue
 
 		# windows doesn't support the status method
 		isAlive = True if isWindows else proc.status() != 'zombie'
 
 		if proc.name() == ika_process and isAlive:
```

### Comparing `ikabot-6.5.8/ikabot/helpers/resources.py` & `ikabot-6.5.9/ikabot/helpers/resources.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import re
 import json
 from decimal import *
 from ikabot.config import *
 
 getcontext().prec = 30
 
+
 def getAvailableResources(html, num=False):
 	"""
 	Parameters
 	----------
 	html : string
 
 	Returns
@@ -20,52 +21,55 @@
 	"""
 	resources = re.search(r'\\"resource\\":(\d+),\\"2\\":(\d+),\\"1\\":(\d+),\\"4\\":(\d+),\\"3\\":(\d+)}', html)
 	if num:
 		return [int(resources.group(1)), int(resources.group(3)), int(resources.group(2)), int(resources.group(5)), int(resources.group(4))]
 	else:
 		return [resources.group(1), resources.group(3), resources.group(2), resources.group(5), resources.group(4)]
 
+
 def getWarehouseCapacity(html):
 	"""
 	Parameters
 	----------
 	html : string
 	Returns
 	-------
 	capacity : int
 	"""
 	capacity = re.search(r'maxResources:\s*JSON\.parse\(\'{\\"resource\\":(\d+),', html).group(1)
 	return int(capacity)
 
+
 def getWineConsumption(html):
 	"""
 	Parameters
 	----------
 	html : string
 	Returns
 	-------
 	capacity : int
 	"""
 	result = re.search(r'GlobalMenu_WineConsumption"\s*class="rightText">\s*(\d+)\s', html)
 	if result:
 		return int(result.group(1))
 	return 0
 
+
 def getProductionPerSecond(session, city_id):
 	"""
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 	city_id : int
 
 	Returns
 	-------
 	production: tuple[Decimal, Decimal, int]
 	"""
 	prod = session.post(payloadPost={'action': 'header', 'function': 'changeCurrentCity', 'actionRequest': actionRequest, 'cityId': city_id, 'ajax': '1'})
 	prod = json.loads(prod, strict=False)
 	prod = prod[0][1]['headerData']
-	wood_production = Decimal( prod['resourceProduction'] )
-	luxury_production = Decimal( prod['tradegoodProduction'] )
-	luxury_resource_type = int( prod['producedTradegood'] )
+	wood_production = Decimal(prod['resourceProduction'])
+	luxury_production = Decimal(prod['tradegoodProduction'])
+	luxury_resource_type = int(prod['producedTradegood'])
 
 	return wood_production, luxury_production, luxury_resource_type
```

### Comparing `ikabot-6.5.8/ikabot/helpers/signals.py` & `ikabot-6.5.9/ikabot/helpers/signals.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,40 +3,43 @@
 
 import os
 import signal
 import gettext
 from ikabot.config import *
 from ikabot.helpers.botComm import *
 
-t = gettext.translation('signals',
-                        localedir,
-                        languages=languages,
-                        fallback=True)
+t = gettext.translation('signals', localedir, languages=languages, fallback=True)
 _ = t.gettext
 
+
 def do_nothing(signal, frame):
 	pass
 
+
 def deactivate_sigint():
-	signal.signal(signal.SIGINT, do_nothing) #signal.SIGHUP replaced with signal.SIGINT for compatibility
+	signal.signal(signal.SIGINT, do_nothing)  #signal.SIGHUP replaced with signal.SIGINT for compatibility
+
 
 def create_handler(s):
 	def _handler(signum, frame):
 		raise Exception(_('Signal number {:d} received').format(signum))
 	return _handler
 
+
 def setSignalsHandlers(s):
-	signals = [signal.SIGINT, signal.SIGTERM] #signal.SIGQUIT replaced with signal.SIGINT for compatibility
+	signals = [signal.SIGINT, signal.SIGTERM]  # signal.SIGQUIT replaced with signal.SIGINT for compatibility
 	for sgn in signals:
 		signal.signal(sgn, create_handler(s))
 
-def setInfoSignal(session, info): # send process info to bot
+
+def setInfoSignal(session, info):  # send process info to bot
 	"""
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 	info : str
 	"""
 	info = _('information of the process {}:\n{}').format(os.getpid(), info)
+
 	def _sendInfo(signum, frame):
 		sendToBot(session, info)
-	signal.signal(signal.SIGABRT, _sendInfo) # kill -SIGUSR1 pid, SIGUSR1 replaced with SIGABRT for compatibility
+	signal.signal(signal.SIGABRT, _sendInfo)  # kill -SIGUSR1 pid, SIGUSR1 replaced with SIGABRT for compatibility
```

### Comparing `ikabot-6.5.8/ikabot/helpers/varios.py` & `ikabot-6.5.9/ikabot/helpers/varios.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import re
 import time
 import random
 from decimal import *
 
 getcontext().prec = 30
 
+
 def addThousandSeparator(num, character = '.'):
 	"""Formats the number into a string and adds a `character` for every thousand (eg. 3000 -> 3.000)
 	Parameters
 	----------
 	num : int
 		integer number to format
 	character : str
@@ -20,14 +21,15 @@
 	Returns
 	-------
 	number : str
 		a string representing that number with added `character` for every thousand
 	"""
 	return '{0:,}'.format(int(num)).replace(',', character)
 
+
 def daysHoursMinutes(totalSeconds):
 	"""Formats the total number of seconds into days hours minutes (eg. 321454 -> 3D 17H)
 	Parameters
 	----------
 	totalSeconds : int
 		total number of seconds
 
@@ -48,35 +50,37 @@
 		texto = str(dias) + 'D '
 	if horas > 0:
 		texto = texto + str(horas) + 'H '
 	if minutos > 0 and dias == 0:
 		texto = texto + str(minutos) + 'M '
 	return texto[:-1]
 
-def wait(seconds, maxrandom = 0):
+
+def wait(seconds, maxrandom=0):
 	"""This function will wait the provided number of seconds plus a random number of seconds between 0 and maxrandom
 	Parameters
 	-----------
 	seconds : int
 		the number of seconds to wait for
 	maxrandom : int
 		the maximum number of additional seconds to wait for
 	"""
 	if seconds <= 0:
 		return
 	randomTime = random.randint(0, maxrandom)
-	ratio = (1 + 5 ** 0.5) / 2 - 1 # 0.6180339887498949
+	ratio = (1 + 5 ** 0.5) / 2 - 1  # 0.6180339887498949
 	comienzo = time.time()
 	fin = comienzo + seconds
 	restantes = seconds
 	while restantes > 0:
 		time.sleep(restantes * ratio)
 		restantes = fin - time.time()
 	time.sleep(randomTime)
 
+
 def getCurrentCityId(session):
 	"""
 	Parameters
 	----------
 	session : ikabot.web.session.Session
 	"""
 	html = session.get()
```

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/activateMiracle.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/activateMiracle.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/aesCipher.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/aesCipher.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/alertAttacks.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/alertAttacks.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/alertLowWine.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/alertLowWine.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/botComm.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/botComm.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/buyResources.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/buyResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/command_line.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/command_line.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/config.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/config.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/constructBuilding.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/constructBuilding.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/constructionList.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/constructionList.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/distributeResources.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/distributeResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/donate.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/donate.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/donationBot.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/donationBot.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/getStatus.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/getStatus.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/gui.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/gui.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/loginDaily.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/loginDaily.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/pedirInfo.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/pedirInfo.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/sellResources.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/sellResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/sendResources.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/sendResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/session.mo` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/session.mo`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/session.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/session.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/shipMovements.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/shipMovements.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/signals.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/signals.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/trainArmy.pot` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/trainArmy.pot`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/trainFleets.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/trainFleets.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/trainTroops.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/trainTroops.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/update.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/update.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/locale/es/LC_MESSAGES/vacationMode.po` & `ikabot-6.5.9/ikabot/locale/es/LC_MESSAGES/vacationMode.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.5.8/ikabot/web/session.py` & `ikabot-6.5.9/ikabot/web/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,28 +15,31 @@
 from ikabot import config
 from ikabot.config import *
 from ikabot.helpers.botComm import *
 from ikabot.helpers.gui import banner
 from ikabot.helpers.aesCipher import *
 from ikabot.helpers.pedirInfo import read
 from ikabot.helpers.getJson import getCity
+from urllib3.exceptions import InsecureRequestWarning
 
 t = gettext.translation('session', localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
 class Session:
 	def __init__(self):
 		if isWindows:
 			self.logfile = os.getenv('temp') + '/ikabot.log'
 		else:
 			self.logfile = '/tmp/ikabot.log'
 		self.log = False
 		self.padre = True
 		self.logged = False
+		# disable ssl verification warning
+		requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
 		self.__login()
 
 	def writeLog(self, msg):
 		return self.__log(msg)
 
 	def __log(self, msg):
 		if self.log is False:
@@ -57,15 +60,15 @@
 		return self.__genRand() + self.__genRand() + '-' + self.__genRand() + '-' + self.__genRand() + '-' + self.__genRand() + '-' + self.__genRand() + self.__genRand() + self.__genRand()
 
 	def __logout(self, html):
 		if html is not None:
 			idCiudad = getCity(html)['id']
 			token = re.search(r'actionRequest"?:\s*"(.*?)"', html).group(1)
 			urlLogout = 'action=logoutAvatar&function=logout&sideBarExt=undefined&startPageShown=1&detectedDevice=1&cityId={0}&backgroundView=city&currentCityId={0}&actionRequest={1}'.format(idCiudad, token)
-			self.s.get(self.urlBase + urlLogout)
+			self.s.get(self.urlBase + urlLogout, verify=config.do_ssl_verify)
 
 	def __isInVacation(self, html):
 		return 'nologin_umod' in html
 
 	def __isExpired(self, html):
 		return 'index.php?logout' in html
 
@@ -306,15 +309,15 @@
 			old_s.headers.update(self.headers)
 			# set the cookies to test
 			cookie_dict = sessionData['cookies']
 			requests.cookies.cookiejar_from_dict(cookie_dict, cookiejar=old_s.cookies, overwrite=True)
 			self.__update_proxy(obj=old_s, sessionData=sessionData)
 			try:
 				# make a request to check the connection
-				html = old_s.get(self.urlBase).text
+				html = old_s.get(self.urlBase, verify=config.do_ssl_verify).text
 			except Exception:
 				self.__proxy_error()
 
 			cookies_are_valid = self.__isExpired(html) is False
 			if cookies_are_valid:
 				self.__log('using old cookies')
 				used_old_cookies = True
@@ -352,15 +355,15 @@
 			self.s.headers.update(self.headers)
 
 			# set the proxy
 			self.__update_proxy(sessionData=sessionData)
 
 			# use the new cookies instead, invalidate the old ones
 			try:
-				html = self.s.get(url).text
+				html = self.s.get(url, verify=config.do_ssl_verify).text
 			except Exception:
 				self.__proxy_error()
 
 		if self.__isInVacation(html):
 			msg = _('The account went into vacation mode')
 			if self.padre:
 				print(msg)
@@ -404,43 +407,46 @@
 			try:
 				self.__login(3)
 			except Exception:
 				self.__sessionExpired()
 
 	def __proxy_error(self):
 		sessionData = self.getSessionData()
-		if 'proxy' not in sessionData or sessionData['proxy']['set'] is False:
+		if 'proxy' not in sessionData['shared'] or sessionData['shared']['proxy']['set'] is False:
 			sys.exit('network error')
 		if self.padre is True:
 			print(_('There seems to be a problem connecting to ikariam.'))
 			print(_('Do you want to disable the proxy? [Y/n]'))
 			rta = read(values=['y', 'Y', 'n', 'N', ''])
 			if rta.lower() == 'n':
 				sys.exit()
 			else:
-				sessionData['proxy'] = {}
-				sessionData['proxy']['conf'] = {}
-				sessionData['proxy']['set'] = False
-				self.setSessionData(sessionData)
+				proxy_conf = {}
+				proxy_conf['proxy'] = {}
+				proxy_conf['proxy']['conf'] = {}
+				proxy_conf['proxy']['set'] = False
+				self.setSessionData(proxy_conf, shared=True)
 				print(_('Proxy disabled, try again.'))
 				enter()
 				sys.exit()
 		else:
 			msg = _('Network error. Consider disabling the proxy.')
 			sendToBot(self, msg)
 			sys.exit()
 
 	def __update_proxy(self, *, obj=None, sessionData=None):
 		# set the proxy
 		if obj is None:
 			obj = self.s
 		if sessionData is None:
 			sessionData = self.getSessionData()
-		if 'proxy' in sessionData:
-			obj.proxies.update(sessionData['proxy']['conf'])
+		if 'proxy' in sessionData['shared'] and sessionData['shared']['proxy']['set'] is True:
+			obj.proxies.update(sessionData['shared']['proxy']['conf'])
+		else:
+			obj.proxies.update({})
 
 	def __checkCookie(self):
 		self.__log('__checkCookie()')
 		sessionData = self.getSessionData()
 
 		try:
 			if self.s.cookies['PHPSESSID'] != sessionData['cookies']['PHPSESSID']:
@@ -457,14 +463,15 @@
 		-------
 		token : str
 			a string representing a valid actionRequest token
 		"""
 		html = self.get()
 		return re.search(r'actionRequest"?:\s*"(.*?)"', html).group(1)
 
+
 	def get(self, url='', params={}, ignoreExpire=False, noIndex=False, fullResponse=False):
 		"""Sends get request to ikariam
 		Parameters
 		----------
 		url : str
 			this string will be appended to the end of the urlBase of the Session object. urlBase will look like: 'https://s(number)-(country).ikariam.gameforge.com/index.php?'
 		params : dict
@@ -485,22 +492,22 @@
 		if noIndex:
 			url = self.urlBase.replace('index.php', '') + url
 		else:
 			url = self.urlBase + url
 		self.__log('get({}), params:{}'.format(url, str(params)))
 		while True:
 			try:
-				if fullResponse:
-					response = self.s.get(url, params=params)
-				else:
-					response = self.s.get(url, params=params).text  # this isn't recursion, this get is different from the one it's in
-				html = response
+				response = self.s.get(url, params=params, verify=config.do_ssl_verify)
+				html = response.text
 				if ignoreExpire is False:
 					assert self.__isExpired(html) is False
-				return html
+				if fullResponse:
+					return response
+				else:
+					return html
 			except AssertionError:
 				self.__sessionExpired()
 			except requests.exceptions.ConnectionError:
 				time.sleep(ConnectionError_wait)
 
 	def post(self, url='', payloadPost={}, params={}, ignoreExpire=False, noIndex=False):
 		"""Sends post request to ikariam
@@ -539,15 +546,15 @@
 		if noIndex:
 			url = self.urlBase.replace('index.php', '') + url
 		else:
 			url = self.urlBase + url
 		self.__log('post({}), data={}'.format(url, str(payloadPost)))
 		while True:
 			try:
-				resp = self.s.post(url, data=payloadPost, params=params).text
+				resp = self.s.post(url, data=payloadPost, params=params, verify=config.do_ssl_verify).text
 				if ignoreExpire is False:
 					assert self.__isExpired(resp) is False
 				if 'TXT_ERROR_WRONG_REQUEST_ID' in resp:
 					self.__log(_('got TXT_ERROR_WRONG_REQUEST_ID'))
 					return self.post(url=url_original, payloadPost=payloadPost_original, params=params_original, ignoreExpire=ignoreExpire, noIndex=noIndex)
 				self.__log(resp)
 				return resp
```

### Comparing `ikabot-6.5.8/ikabot.egg-info/SOURCES.txt` & `ikabot-6.5.9/ikabot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

