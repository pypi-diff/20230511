# Comparing `tmp/starrail-toolkit-0.5.4.tar.gz` & `tmp/starrail-toolkit-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrail-toolkit-0.5.4.tar", last modified: Tue May  9 19:05:30 2023, max compression
+gzip compressed data, was "starrail-toolkit-0.5.6.tar", last modified: Thu May 11 18:40:15 2023, max compression
```

## Comparing `starrail-toolkit-0.5.4.tar` & `starrail-toolkit-0.5.6.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.757251 starrail-toolkit-0.5.4/
--rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/LICENSE
--rw-r--r--   0 littlenyima   (501) staff       (20)     5041 2023-05-09 19:05:30.757120 starrail-toolkit-0.5.4/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     4534 2023-05-09 19:05:12.000000 starrail-toolkit-0.5.4/README.md
--rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-09 19:05:30.757286 starrail-toolkit-0.5.4/setup.cfg
--rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.751750 starrail-toolkit-0.5.4/starrail/
--rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1763 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/config.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.752210 starrail-toolkit-0.5.4/starrail/entry/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/entry/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3000 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/entry/cli.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      988 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/entry/gui.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/entry/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.753214 starrail-toolkit-0.5.4/starrail/gacha/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3636 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/autodet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/database.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1103 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/fetch.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/fileio.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5078 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/parse.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3572 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/service.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/type.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/url.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.753465 starrail-toolkit-0.5.4/starrail/gui/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5958 2023-05-09 18:54:42.000000 starrail-toolkit-0.5.4/starrail/gui/application.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.753939 starrail-toolkit-0.5.4/starrail/gui/common/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/common/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      260 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/common/icon.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      611 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/common/stylesheet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1413 2023-05-09 18:54:42.000000 starrail-toolkit-0.5.4/starrail/gui/common/utils.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.754623 starrail-toolkit-0.5.4/starrail/gui/interfaces/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/interfaces/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1842 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/interfaces/base.py
--rw-r--r--   0 littlenyima   (501) staff       (20)    12878 2023-05-09 18:43:38.000000 starrail-toolkit-0.5.4/starrail/gui/interfaces/gacha_sync.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2520 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/interfaces/home.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3700 2023-05-09 19:03:50.000000 starrail-toolkit-0.5.4/starrail/gui/interfaces/setting.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      372 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/interfaces/users.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.755097 starrail-toolkit-0.5.4/starrail/gui/widgets/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/widgets/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5401 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/widgets/dialog.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/widgets/link_card.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/widgets/title_bar.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.755462 starrail-toolkit-0.5.4/starrail/utils/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/utils/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      937 2023-05-09 18:39:18.000000 starrail-toolkit-0.5.4/starrail/utils/auto_update.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.756207 starrail-toolkit-0.5.4/starrail/utils/babelfish/
--rw-r--r--   0 littlenyima   (501) staff       (20)     2823 2023-05-09 19:03:15.000000 starrail-toolkit-0.5.4/starrail/utils/babelfish/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      144 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/utils/babelfish/constants.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6502 2023-05-09 19:03:15.000000 starrail-toolkit-0.5.4/starrail/utils/babelfish/dictionary.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      373 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/utils/babelfish/locale.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/utils/babelfish/multilingual.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/utils/babelfish/translate.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/utils/loggings.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      106 2023-05-09 19:05:00.000000 starrail-toolkit-0.5.4/starrail/version.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.756935 starrail-toolkit-0.5.4/starrail_toolkit.egg-info/
--rw-r--r--   0 littlenyima   (501) staff       (20)     5041 2023-05-09 19:05:30.000000 starrail-toolkit-0.5.4/starrail_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     1473 2023-05-09 19:05:30.000000 starrail-toolkit-0.5.4/starrail_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-09 19:05:30.000000 starrail-toolkit-0.5.4/starrail_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-09 19:05:30.000000 starrail-toolkit-0.5.4/starrail_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       87 2023-05-09 19:05:30.000000 starrail-toolkit-0.5.4/starrail_toolkit.egg-info/requires.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-09 19:05:30.000000 starrail-toolkit-0.5.4/starrail_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.563663 starrail-toolkit-0.5.6/
+-rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/LICENSE
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5400 2023-05-11 18:40:15.563530 starrail-toolkit-0.5.6/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4893 2023-05-11 18:36:26.000000 starrail-toolkit-0.5.6/README.md
+-rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-11 18:40:15.563702 starrail-toolkit-0.5.6/setup.cfg
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.557408 starrail-toolkit-0.5.6/starrail/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1838 2023-05-11 13:36:54.000000 starrail-toolkit-0.5.6/starrail/config.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.557901 starrail-toolkit-0.5.6/starrail/entry/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/entry/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3000 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/entry/cli.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      988 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/entry/gui.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/entry/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.559207 starrail-toolkit-0.5.6/starrail/gacha/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gacha/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3636 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gacha/autodet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gacha/database.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1103 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gacha/fetch.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gacha/fileio.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5078 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gacha/parse.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3665 2023-05-11 14:02:35.000000 starrail-toolkit-0.5.6/starrail/gacha/service.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gacha/type.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gacha/url.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.559445 starrail-toolkit-0.5.6/starrail/gui/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5958 2023-05-09 19:22:18.000000 starrail-toolkit-0.5.6/starrail/gui/application.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.560070 starrail-toolkit-0.5.6/starrail/gui/common/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/common/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      978 2023-05-11 13:36:55.000000 starrail-toolkit-0.5.6/starrail/gui/common/config.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      260 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/common/icon.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      611 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/common/stylesheet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1136 2023-05-11 13:36:49.000000 starrail-toolkit-0.5.6/starrail/gui/common/utils.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.560906 starrail-toolkit-0.5.6/starrail/gui/interfaces/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/interfaces/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1842 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/interfaces/base.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    12864 2023-05-11 14:01:58.000000 starrail-toolkit-0.5.6/starrail/gui/interfaces/gacha_sync.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2536 2023-05-11 18:38:07.000000 starrail-toolkit-0.5.6/starrail/gui/interfaces/home.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4285 2023-05-11 18:38:38.000000 starrail-toolkit-0.5.6/starrail/gui/interfaces/setting.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      372 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/interfaces/users.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.561359 starrail-toolkit-0.5.6/starrail/gui/widgets/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/widgets/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5401 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/widgets/dialog.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/widgets/link_card.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/widgets/title_bar.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.561847 starrail-toolkit-0.5.6/starrail/utils/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/utils/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1855 2023-05-11 18:32:57.000000 starrail-toolkit-0.5.6/starrail/utils/accounts.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      937 2023-05-09 19:22:18.000000 starrail-toolkit-0.5.6/starrail/utils/auto_update.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.562617 starrail-toolkit-0.5.6/starrail/utils/babelfish/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3088 2023-05-11 14:19:58.000000 starrail-toolkit-0.5.6/starrail/utils/babelfish/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      230 2023-05-11 18:37:45.000000 starrail-toolkit-0.5.6/starrail/utils/babelfish/constants.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6791 2023-05-11 18:38:18.000000 starrail-toolkit-0.5.6/starrail/utils/babelfish/dictionary.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      373 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/utils/babelfish/locale.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/utils/babelfish/multilingual.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/utils/babelfish/translate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/utils/loggings.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      106 2023-05-11 14:03:34.000000 starrail-toolkit-0.5.6/starrail/version.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.563366 starrail-toolkit-0.5.6/starrail_toolkit.egg-info/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5400 2023-05-11 18:40:15.000000 starrail-toolkit-0.5.6/starrail_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1530 2023-05-11 18:40:15.000000 starrail-toolkit-0.5.6/starrail_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-11 18:40:15.000000 starrail-toolkit-0.5.6/starrail_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-11 18:40:15.000000 starrail-toolkit-0.5.6/starrail_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       87 2023-05-11 18:40:15.000000 starrail-toolkit-0.5.6/starrail_toolkit.egg-info/requires.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-11 18:40:15.000000 starrail-toolkit-0.5.6/starrail_toolkit.egg-info/top_level.txt
```

### Comparing `starrail-toolkit-0.5.4/LICENSE` & `starrail-toolkit-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/PKG-INFO` & `starrail-toolkit-0.5.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.5.4
+Version: 0.5.6
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -20,41 +20,43 @@
 </div>
 
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 |
 | :--------: | :----------: | :-------: |
-|   0.5.4    |    0.5.4     |   0.5.4   |
+|   0.5.4    |    0.5.6     |   0.5.6   |
 
-- [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
-- [x] 支持命令行显示抽卡报告
-- [x] 支持导出 markdown 格式抽卡报告
-- [x] 支持导出网页版抽卡报告
-- [x] 支持中英文多语言导出
-- [x] 支持 Windows 平台游戏中自动检测 API URL
-- [x] 实现用户界面并编译到 Windows 平台
-- [x] 支持自动检查更新
+目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
+
+- [ ] 支持更多的可设置选项
+- [x] 支持夜间模式
+- [ ] 支持多用户切换
+- [ ] 美化抽卡导出页面
+
+## 常见问题解答
+
+关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
 
 ## 安装方式
 
 ### 下载可执行程序
 
-目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/i3GIq0v3hbbe)，两种途径的内容相同，可以自行选择下载方式。
+目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/i8l5L0v48e5i)，两种途径的内容相同，可以自行选择下载方式。
 
 ***BREAKING：目前用户界面的第一个版本已经实现完成，界面预览：***
 
 ![gui_preview](https://s1.ax1x.com/2023/05/08/p90QWex.png)
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
-python3 -m pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
+python3 -m pip install starrail-toolkit --force-reinstall --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
 ```
 
 ### 从源码安装
 
 若需要使用尚未推送到 PyPI 版本的功能，可通过源码安装：
 
 ```shell
@@ -63,15 +65,15 @@
 python3 setup.py install
 ```
 
 ##  命令行使用指南
 
 ### 获取抽卡查询 API URL
 
-请参考[【这个教程】](docs/how-to-get-api-url.md)获取查询链接。
+请参考[这个教程](docs/how-to-get-api-url.md)获取查询链接。
 
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间（大约 24 小时）后过期，过期后需要重新获取。
 
 **注：若为 Windows 平台，可以使用本工具自动检测 API URL。** 首先登陆游戏，进入抽卡查询页面，当显示出一页抽卡查询结果后，退出游戏（由于 Windows 系统文件占用问题，若不退出，可能导致缓存无法读取），运行本工具，即可检测到抽卡查询 URL。如果需要切换账号，建议使用上述教程中的方法获取每个账号的 API URL，以便精确控制导出的账号。
 
 ### 导出抽卡记录
 
@@ -105,7 +107,11 @@
 - Markdown 结果示例：
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GYNKf.png" alt="markdown" style="width: 600px;" />
 
 ## 安全提醒
 
 本仓库代码完全开源，且用户数据全部保存在本地，**本项目不会上传任何用户数据**。本项目仅在该 GitHub 仓库及 PyPI 进行分发，请仔细甄别下载到的程序，防止遭遇恶意程序。
+
+## Credits
+
+本仓库用户界面部分基于 [**zhiyiYo/PyQt-Fluent-Widgets**](https://github.com/zhiyiYo/PyQt-Fluent-Widgets) 实现，缓存解析部分参考了 [**sunfkny/genshin-gacha-export**](https://github.com/sunfkny/genshin-gacha-export)。
```

### Comparing `starrail-toolkit-0.5.4/README.md` & `starrail-toolkit-0.5.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,41 +5,43 @@
 </div>
 
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 |
 | :--------: | :----------: | :-------: |
-|   0.5.4    |    0.5.4     |   0.5.4   |
+|   0.5.4    |    0.5.6     |   0.5.6   |
 
-- [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
-- [x] 支持命令行显示抽卡报告
-- [x] 支持导出 markdown 格式抽卡报告
-- [x] 支持导出网页版抽卡报告
-- [x] 支持中英文多语言导出
-- [x] 支持 Windows 平台游戏中自动检测 API URL
-- [x] 实现用户界面并编译到 Windows 平台
-- [x] 支持自动检查更新
+目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
+
+- [ ] 支持更多的可设置选项
+- [x] 支持夜间模式
+- [ ] 支持多用户切换
+- [ ] 美化抽卡导出页面
+
+## 常见问题解答
+
+关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
 
 ## 安装方式
 
 ### 下载可执行程序
 
-目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/i3GIq0v3hbbe)，两种途径的内容相同，可以自行选择下载方式。
+目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/i8l5L0v48e5i)，两种途径的内容相同，可以自行选择下载方式。
 
 ***BREAKING：目前用户界面的第一个版本已经实现完成，界面预览：***
 
 ![gui_preview](https://s1.ax1x.com/2023/05/08/p90QWex.png)
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
-python3 -m pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
+python3 -m pip install starrail-toolkit --force-reinstall --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
 ```
 
 ### 从源码安装
 
 若需要使用尚未推送到 PyPI 版本的功能，可通过源码安装：
 
 ```shell
@@ -48,15 +50,15 @@
 python3 setup.py install
 ```
 
 ##  命令行使用指南
 
 ### 获取抽卡查询 API URL
 
-请参考[【这个教程】](docs/how-to-get-api-url.md)获取查询链接。
+请参考[这个教程](docs/how-to-get-api-url.md)获取查询链接。
 
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间（大约 24 小时）后过期，过期后需要重新获取。
 
 **注：若为 Windows 平台，可以使用本工具自动检测 API URL。** 首先登陆游戏，进入抽卡查询页面，当显示出一页抽卡查询结果后，退出游戏（由于 Windows 系统文件占用问题，若不退出，可能导致缓存无法读取），运行本工具，即可检测到抽卡查询 URL。如果需要切换账号，建议使用上述教程中的方法获取每个账号的 API URL，以便精确控制导出的账号。
 
 ### 导出抽卡记录
 
@@ -90,7 +92,11 @@
 - Markdown 结果示例：
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GYNKf.png" alt="markdown" style="width: 600px;" />
 
 ## 安全提醒
 
 本仓库代码完全开源，且用户数据全部保存在本地，**本项目不会上传任何用户数据**。本项目仅在该 GitHub 仓库及 PyPI 进行分发，请仔细甄别下载到的程序，防止遭遇恶意程序。
+
+## Credits
+
+本仓库用户界面部分基于 [**zhiyiYo/PyQt-Fluent-Widgets**](https://github.com/zhiyiYo/PyQt-Fluent-Widgets) 实现，缓存解析部分参考了 [**sunfkny/genshin-gacha-export**](https://github.com/sunfkny/genshin-gacha-export)。
```

### Comparing `starrail-toolkit-0.5.4/setup.py` & `starrail-toolkit-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/__init__.py` & `starrail-toolkit-0.5.6/starrail/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/config.py` & `starrail-toolkit-0.5.6/starrail/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,23 +37,22 @@
                 json.dump(cfg, fcfg, indent=2)
 
 
 configuration = Configuration(
     cache_dir=os.path.join(userroot, '.starrail'),
     db_dir=os.path.join(userroot, '.starrail', 'database'),
     config_path=os.path.join(userroot, '.starrail', 'config.json'),
+    account_record_path=os.path.join(userroot, '.starrail', 'accounts.json'),
     check_update=True,
     locale='zhs',
     log_level='DEBUG',
-    theme_mode='LIGHT',
-    uid='',
 )
 configuration.set_skip_keys(
     'skip_keys', 'no_flush',
-    'cache_dir', 'config_path',
+    'cache_dir', 'config_path', 'db_dir', 'account_record_path',
 )
 
 
 def init_config():
 
     os.makedirs(configuration.cache_dir, exist_ok=True)
     os.makedirs(configuration.db_dir, exist_ok=True)
```

### Comparing `starrail-toolkit-0.5.4/starrail/entry/cli.py` & `starrail-toolkit-0.5.6/starrail/entry/cli.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/entry/gui.py` & `starrail-toolkit-0.5.6/starrail/entry/gui.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/entry/setup.py` & `starrail-toolkit-0.5.6/starrail/entry/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/gacha/autodet.py` & `starrail-toolkit-0.5.6/starrail/gacha/autodet.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/gacha/database.py` & `starrail-toolkit-0.5.6/starrail/gacha/database.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/gacha/fetch.py` & `starrail-toolkit-0.5.6/starrail/gacha/fetch.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/gacha/fileio.py` & `starrail-toolkit-0.5.6/starrail/gacha/fileio.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/gacha/parse.py` & `starrail-toolkit-0.5.6/starrail/gacha/parse.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/gacha/service.py` & `starrail-toolkit-0.5.6/starrail/gacha/service.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import starrail.gacha.fileio as fileio
 from starrail.gacha.autodet import detect_api_url
 from starrail.gacha.fetch import fetch_json
 from starrail.gacha.parse import GachaDataManager
 from starrail.gacha.type import GachaType
 from starrail.gacha.url import get_api_url, get_url_template
 from starrail.utils import loggings
+from starrail.utils.accounts import account_record
 
 logger = loggings.get_logger(__file__)
 
 
 def integers():
     r = 1
     while True:
@@ -89,14 +90,16 @@
         )
         manager.add_records(gacha_type.value, records)
         manager.gacha[gacha_type.value].sort()
         logger.info(f'Finish downloading records of {gacha_type.name}')
 
     fileio.export_as_sql(manager, manager.cache_path)
 
+    account_record.update_timestamp(uid)
+
     manager.log_stats()
 
     export_hooks = dict(
         csv=fileio.export_as_csv,
         html=fileio.export_as_html,
         json=fileio.export_as_json,
         md=fileio.export_as_md,
```

### Comparing `starrail-toolkit-0.5.4/starrail/gacha/url.py` & `starrail-toolkit-0.5.6/starrail/gacha/url.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/gui/application.py` & `starrail-toolkit-0.5.6/starrail/gui/application.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/gui/common/stylesheet.py` & `starrail-toolkit-0.5.6/starrail/gui/common/stylesheet.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/gui/interfaces/base.py` & `starrail-toolkit-0.5.6/starrail/gui/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/gui/interfaces/gacha_sync.py` & `starrail-toolkit-0.5.6/starrail/gui/interfaces/gacha_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 
 import qfluentwidgets as qfw
 from PySide6 import QtWidgets
 from PySide6.QtCore import Qt, QThread, Signal
 from PySide6.QtWidgets import QLabel, QTableWidgetItem, QVBoxLayout
 
 import starrail.gacha.service as service
-from starrail.config import configuration as cfg
 from starrail.gacha.type import GachaType
 from starrail.gui.common.stylesheet import StyleSheet
-from starrail.gui.common.utils import get_current_uid
 from starrail.gui.interfaces.base import BaseInterface
 from starrail.utils import babelfish, loggings
+from starrail.utils.accounts import account_record, get_latest_uid
 
 AF = Qt.AlignmentFlag
 logger = loggings.get_logger(__file__)
 
 
 class GachaSyncThread(QThread):
 
@@ -220,15 +219,15 @@
         )
 
         # Gacha Sync Temp Objects
         self.syncThread = None
         self.syncToolTip = None
         self.saveThread = None
 
-        self.uid = get_current_uid()
+        self.uid = get_latest_uid()
         logger.info(f'Detected current uid: {self.uid}')
         if self.uid:
             self.updateTableDisplay()
             self.saveButton.setEnabled(True)
 
         self.__initWidget()
 
@@ -317,15 +316,15 @@
     def setToolTipContentSlot(self, tooltip: qfw.StateToolTip, content: str):
         tooltip.setContent(content)
 
     def syncSuccessSlot(self, uid: int):
         logger.info('[GUI] Gacha data synchronization success')
 
         self.uid = uid
-        cfg.uid = uid
+        account_record.update_timestamp(uid)
 
         self.syncToolTip.setTitle(babelfish.ui_sync_gacha_success())
         self.syncToolTip.setContent('')
         self.syncToolTip.setState(True)
         self.syncToolTip = None
         self.syncThread = None
```

### Comparing `starrail-toolkit-0.5.4/starrail/gui/interfaces/home.py` & `starrail-toolkit-0.5.6/starrail/gui/interfaces/home.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             babelfish.constants.DOCS_URL,
         )
 
         self.linkCardView.addCard(
             FluentIcon.HELP,
             babelfish.ui_troubleshooting(),
             babelfish.ui_troubleshooting_desc(),
-            'https://www.baidu.com',
+            babelfish.constants.TROUBLESHOOTING_URL,
         )
 
         self.linkCardView.addCard(
             FluentIcon.GITHUB,
             babelfish.ui_github_repo(),
             babelfish.ui_github_repo_desc(),
             babelfish.constants.REPO_URL,
```

### Comparing `starrail-toolkit-0.5.4/starrail/gui/interfaces/setting.py` & `starrail-toolkit-0.5.6/starrail/gui/interfaces/setting.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import qfluentwidgets as qfw
 from PySide6.QtCore import Qt, Signal
 from PySide6.QtWidgets import QLabel, QWidget
 from qfluentwidgets import FluentIcon
 
 from starrail import __version__
+from starrail.gui.common.config import qcfg
 from starrail.gui.common.stylesheet import StyleSheet
 from starrail.gui.common.utils import checkUpdate
 from starrail.utils import babelfish
 
 
 class SettingInterface(qfw.ScrollArea):
 
@@ -18,31 +19,43 @@
     def __init__(self, parent=None):
         super().__init__(parent=parent)
         self.scrollWidget = QWidget()
         self.expandLayout = qfw.ExpandLayout(self.scrollWidget)
 
         self.settingLabel = QLabel(babelfish.ui_settings(), self)
 
-        # self.personalGroup = qfw.SettingCardGroup(
-        #     babelfish.ui_personalization(), self.scrollWidget,
-        # )
+        self.personalGroup = qfw.SettingCardGroup(
+            babelfish.ui_personalization(), self.scrollWidget,
+        )
+        self.themeModeCard = qfw.OptionsSettingCard(
+            qcfg.themeMode,
+            FluentIcon.BRUSH,
+            babelfish.ui_theme_mode(),
+            babelfish.ui_theme_mode_settings_desc(),
+            [
+                babelfish.ui_theme_mode_light(),
+                babelfish.ui_theme_mode_dark(),
+                babelfish.ui_theme_mode_auto(),
+            ],
+            self.personalGroup,
+        )
 
         self.aboutGroup = qfw.SettingCardGroup(
             babelfish.ui_about(), self.scrollWidget,
         )
         self.getStartCard = qfw.HyperlinkCard(
             babelfish.constants.DOCS_URL,
             babelfish.ui_open_docs(),
             FluentIcon.BOOK_SHELF,
             babelfish.ui_get_started(),
             babelfish.ui_get_started_desc(),
             self.aboutGroup,
         )
         self.troubleshootingCard = qfw.HyperlinkCard(
-            'https://www.baidu.com',
+            babelfish.constants.TROUBLESHOOTING_URL,
             babelfish.ui_open_troubleshooting(),
             FluentIcon.HELP,
             babelfish.ui_troubleshooting(),
             babelfish.ui_troubleshooting_desc(),
             self.aboutGroup,
         )
         self.openSourceCard = qfw.HyperlinkCard(
@@ -68,15 +81,15 @@
             (
                 f'{babelfish.ui_copyright(2023)} '
                 f'{babelfish.ui_current_version(__version__)}'
             ),
             self.aboutGroup,
         )
         self.aboutCard.button.clicked.connect(
-            partial(checkUpdate, parent=self),
+            partial(checkUpdate, parent=self.parent()),
         )
 
         self.__initWidget()
         self.__initLayout()
         self.__connectSignalToSlot()
 
     def __initWidget(self):
@@ -90,20 +103,22 @@
         self.scrollWidget.setObjectName('scrollWidget')
         self.settingLabel.setObjectName('settingLabel')
         StyleSheet.SETTING_INTERFACE.apply(self)
 
     def __initLayout(self):
         self.settingLabel.move(36, 30)
 
+        self.personalGroup.addSettingCard(self.themeModeCard)
+
         self.aboutGroup.addSettingCard(self.getStartCard)
         self.aboutGroup.addSettingCard(self.troubleshootingCard)
         self.aboutGroup.addSettingCard(self.openSourceCard)
         self.aboutGroup.addSettingCard(self.feedbackCard)
         self.aboutGroup.addSettingCard(self.aboutCard)
 
         self.expandLayout.setSpacing(28)
         self.expandLayout.setContentsMargins(36, 10, 36, 0)
-        # self.expandLayout.addWidget(self.personalGroup)
+        self.expandLayout.addWidget(self.personalGroup)
         self.expandLayout.addWidget(self.aboutGroup)
 
     def __connectSignalToSlot(self):
-        pass
+        qfw.qconfig.themeChanged.connect(qfw.setTheme)
```

### Comparing `starrail-toolkit-0.5.4/starrail/gui/widgets/dialog.py` & `starrail-toolkit-0.5.6/starrail/gui/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/gui/widgets/link_card.py` & `starrail-toolkit-0.5.6/starrail/gui/widgets/link_card.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/gui/widgets/title_bar.py` & `starrail-toolkit-0.5.6/starrail/gui/widgets/title_bar.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/utils/auto_update.py` & `starrail-toolkit-0.5.6/starrail/utils/auto_update.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/utils/babelfish/__init__.py` & `starrail-toolkit-0.5.6/starrail/utils/babelfish/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -48,14 +48,19 @@
 ui_send_feedback_desc = dictionary.ui_send_feedback_desc
 ui_settings = dictionary.ui_settings
 ui_sync = dictionary.ui_sync
 ui_sync_gacha_fail = dictionary.ui_sync_gacha_fail
 ui_sync_gacha_initial = dictionary.ui_sync_gacha_initial
 ui_sync_gacha_success = dictionary.ui_sync_gacha_success
 ui_synchronizing_gacha = dictionary.ui_synchronizing_gacha
+ui_theme_mode = dictionary.ui_theme_mode
+ui_theme_mode_auto = dictionary.ui_theme_mode_auto
+ui_theme_mode_dark = dictionary.ui_theme_mode_dark
+ui_theme_mode_light = dictionary.ui_theme_mode_light
+ui_theme_mode_settings_desc = dictionary.ui_theme_mode_settings_desc
 ui_title = dictionary.ui_title
 ui_traceback = dictionary.ui_traceback
 ui_troubleshooting = dictionary.ui_troubleshooting
 ui_troubleshooting_desc = dictionary.ui_troubleshooting_desc
 ui_update_available = dictionary.ui_update_available
 ui_update_desc = dictionary.ui_update_desc
 ui_users = dictionary.ui_users
```

### Comparing `starrail-toolkit-0.5.4/starrail/utils/babelfish/dictionary.py` & `starrail-toolkit-0.5.6/starrail/utils/babelfish/dictionary.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,20 +127,28 @@
     en='Synchronization Success',
     zhs='同步成功',
 )
 ui_synchronizing_gacha = _MS(
     en='Synchronizing...',
     zhs='正在同步抽卡数据',
 )
+ui_theme_mode = _MS(en='Theme Mode', zhs='应用主题')
+ui_theme_mode_auto = _MS(en='Auto', zhs='跟随系统设置')
+ui_theme_mode_dark = _MS(en='Dark', zhs='深色')
+ui_theme_mode_light = _MS(en='Light', zhs='浅色')
+ui_theme_mode_settings_desc = _MS(
+    en='Changing the appearance of application',
+    zhs='改变应用外观',
+)
 ui_title = _MS(en='Honkai: Star Rail Toolkit', zhs='崩坏：星穹铁道工具箱')
 ui_traceback = _MS(en='Traceback', zhs='报错信息')
 ui_troubleshooting = _MS(en='TroubleShooting', zhs='常见问题')
 ui_troubleshooting_desc = _MS(
     en='Click here to view FAQ.',
-    zhs='点此查看常见问题解答。（目前还没写，所以会跳转到百度）',
+    zhs='点此查看常见问题解答。',
 )
 ui_update_available = _MS(
     en='New Version is Available',
     zhs='检查到新版本',
 )
 ui_update_desc = _MS(
     en=(
```

### Comparing `starrail-toolkit-0.5.4/starrail/utils/babelfish/multilingual.py` & `starrail-toolkit-0.5.6/starrail/utils/babelfish/multilingual.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail/utils/loggings.py` & `starrail-toolkit-0.5.6/starrail/utils/loggings.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.4/starrail_toolkit.egg-info/PKG-INFO` & `starrail-toolkit-0.5.6/starrail_toolkit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.5.4
+Version: 0.5.6
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -20,41 +20,43 @@
 </div>
 
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 |
 | :--------: | :----------: | :-------: |
-|   0.5.4    |    0.5.4     |   0.5.4   |
+|   0.5.4    |    0.5.6     |   0.5.6   |
 
-- [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
-- [x] 支持命令行显示抽卡报告
-- [x] 支持导出 markdown 格式抽卡报告
-- [x] 支持导出网页版抽卡报告
-- [x] 支持中英文多语言导出
-- [x] 支持 Windows 平台游戏中自动检测 API URL
-- [x] 实现用户界面并编译到 Windows 平台
-- [x] 支持自动检查更新
+目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
+
+- [ ] 支持更多的可设置选项
+- [x] 支持夜间模式
+- [ ] 支持多用户切换
+- [ ] 美化抽卡导出页面
+
+## 常见问题解答
+
+关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
 
 ## 安装方式
 
 ### 下载可执行程序
 
-目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/i3GIq0v3hbbe)，两种途径的内容相同，可以自行选择下载方式。
+目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/i8l5L0v48e5i)，两种途径的内容相同，可以自行选择下载方式。
 
 ***BREAKING：目前用户界面的第一个版本已经实现完成，界面预览：***
 
 ![gui_preview](https://s1.ax1x.com/2023/05/08/p90QWex.png)
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
-python3 -m pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
+python3 -m pip install starrail-toolkit --force-reinstall --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
 ```
 
 ### 从源码安装
 
 若需要使用尚未推送到 PyPI 版本的功能，可通过源码安装：
 
 ```shell
@@ -63,15 +65,15 @@
 python3 setup.py install
 ```
 
 ##  命令行使用指南
 
 ### 获取抽卡查询 API URL
 
-请参考[【这个教程】](docs/how-to-get-api-url.md)获取查询链接。
+请参考[这个教程](docs/how-to-get-api-url.md)获取查询链接。
 
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间（大约 24 小时）后过期，过期后需要重新获取。
 
 **注：若为 Windows 平台，可以使用本工具自动检测 API URL。** 首先登陆游戏，进入抽卡查询页面，当显示出一页抽卡查询结果后，退出游戏（由于 Windows 系统文件占用问题，若不退出，可能导致缓存无法读取），运行本工具，即可检测到抽卡查询 URL。如果需要切换账号，建议使用上述教程中的方法获取每个账号的 API URL，以便精确控制导出的账号。
 
 ### 导出抽卡记录
 
@@ -105,7 +107,11 @@
 - Markdown 结果示例：
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GYNKf.png" alt="markdown" style="width: 600px;" />
 
 ## 安全提醒
 
 本仓库代码完全开源，且用户数据全部保存在本地，**本项目不会上传任何用户数据**。本项目仅在该 GitHub 仓库及 PyPI 进行分发，请仔细甄别下载到的程序，防止遭遇恶意程序。
+
+## Credits
+
+本仓库用户界面部分基于 [**zhiyiYo/PyQt-Fluent-Widgets**](https://github.com/zhiyiYo/PyQt-Fluent-Widgets) 实现，缓存解析部分参考了 [**sunfkny/genshin-gacha-export**](https://github.com/sunfkny/genshin-gacha-export)。
```

### Comparing `starrail-toolkit-0.5.4/starrail_toolkit.egg-info/SOURCES.txt` & `starrail-toolkit-0.5.6/starrail_toolkit.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,28 +16,30 @@
 starrail/gacha/parse.py
 starrail/gacha/service.py
 starrail/gacha/type.py
 starrail/gacha/url.py
 starrail/gui/__init__.py
 starrail/gui/application.py
 starrail/gui/common/__init__.py
+starrail/gui/common/config.py
 starrail/gui/common/icon.py
 starrail/gui/common/stylesheet.py
 starrail/gui/common/utils.py
 starrail/gui/interfaces/__init__.py
 starrail/gui/interfaces/base.py
 starrail/gui/interfaces/gacha_sync.py
 starrail/gui/interfaces/home.py
 starrail/gui/interfaces/setting.py
 starrail/gui/interfaces/users.py
 starrail/gui/widgets/__init__.py
 starrail/gui/widgets/dialog.py
 starrail/gui/widgets/link_card.py
 starrail/gui/widgets/title_bar.py
 starrail/utils/__init__.py
+starrail/utils/accounts.py
 starrail/utils/auto_update.py
 starrail/utils/loggings.py
 starrail/utils/babelfish/__init__.py
 starrail/utils/babelfish/constants.py
 starrail/utils/babelfish/dictionary.py
 starrail/utils/babelfish/locale.py
 starrail/utils/babelfish/multilingual.py
```

