# Comparing `tmp/7Wonder-RL-Lib-0.1.0.tar.gz` & `tmp/7Wonder-RL-Lib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "7Wonder-RL-Lib-0.1.0.tar", last modified: Thu May 11 00:11:28 2023, max compression
+gzip compressed data, was "7Wonder-RL-Lib-0.1.1.tar", last modified: Thu May 11 10:50:23 2023, max compression
```

## Comparing `7Wonder-RL-Lib-0.1.0.tar` & `7Wonder-RL-Lib-0.1.1.tar`

### file list

```diff
@@ -1,67 +1,175 @@
-drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 00:11:28.271238 7Wonder-RL-Lib-0.1.0/
--rw-r--r--   0 mirrorcraze   (501) staff       (20)      400 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/.bumpversion.cfg
-drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 00:11:28.259256 7Wonder-RL-Lib-0.1.0/.github/
-drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 00:11:28.259962 7Wonder-RL-Lib-0.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 mirrorcraze   (501) staff       (20)      834 2023-03-23 22:40:49.000000 7Wonder-RL-Lib-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 mirrorcraze   (501) staff       (20)      595 2023-03-23 22:40:49.000000 7Wonder-RL-Lib-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 mirrorcraze   (501) staff       (20)      117 2023-05-10 18:57:26.000000 7Wonder-RL-Lib-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 00:11:28.260268 7Wonder-RL-Lib-0.1.0/.github/workflows/
--rw-r--r--   0 mirrorcraze   (501) staff       (20)      891 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 mirrorcraze   (501) staff       (20)     2145 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/.gitignore
--rw-r--r--   0 mirrorcraze   (501) staff       (20)    21142 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/.pylintrc
-drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 00:11:28.261221 7Wonder-RL-Lib-0.1.0/7Wonder_RL_Lib.egg-info/
--rw-r--r--   0 mirrorcraze   (501) staff       (20)     4817 2023-05-11 00:11:28.000000 7Wonder-RL-Lib-0.1.0/7Wonder_RL_Lib.egg-info/PKG-INFO
--rw-r--r--   0 mirrorcraze   (501) staff       (20)     2105 2023-05-11 00:11:28.000000 7Wonder-RL-Lib-0.1.0/7Wonder_RL_Lib.egg-info/SOURCES.txt
--rw-r--r--   0 mirrorcraze   (501) staff       (20)        1 2023-05-11 00:11:28.000000 7Wonder-RL-Lib-0.1.0/7Wonder_RL_Lib.egg-info/dependency_links.txt
--rw-r--r--   0 mirrorcraze   (501) staff       (20)       99 2023-05-11 00:11:28.000000 7Wonder-RL-Lib-0.1.0/7Wonder_RL_Lib.egg-info/requires.txt
--rw-r--r--   0 mirrorcraze   (501) staff       (20)       16 2023-05-11 00:11:28.000000 7Wonder-RL-Lib-0.1.0/7Wonder_RL_Lib.egg-info/top_level.txt
--rw-r--r--   0 mirrorcraze   (501) staff       (20)      667 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 mirrorcraze   (501) staff       (20)     1072 2023-03-23 22:40:49.000000 7Wonder-RL-Lib-0.1.0/LICENSE
--rw-r--r--   0 mirrorcraze   (501) staff       (20)      342 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/MANIFEST.in
--rw-r--r--   0 mirrorcraze   (501) staff       (20)     2561 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/Makefile
--rw-r--r--   0 mirrorcraze   (501) staff       (20)     4817 2023-05-11 00:11:28.271016 7Wonder-RL-Lib-0.1.0/PKG-INFO
--rw-r--r--   0 mirrorcraze   (501) staff       (20)     2876 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/README.md
-drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 00:11:28.261676 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/
-drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 00:11:28.261958 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/
--rw-r--r--   0 mirrorcraze   (501) staff       (20)      141 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/__init__.py
-drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 00:11:28.264453 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/
-drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 00:11:28.264667 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/GameLog/
--rw-r--r--   0 mirrorcraze   (501) staff       (20)      674 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/GameLog/gameLog0.txt
-drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 00:11:28.266306 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/Graph/
--rw-r--r--   0 mirrorcraze   (501) staff       (20)    56761 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/Graph/100.png
--rw-r--r--   0 mirrorcraze   (501) staff       (20)    84453 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/Graph/200.png
--rw-r--r--   0 mirrorcraze   (501) staff       (20)    93053 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/Graph/300.png
--rw-r--r--   0 mirrorcraze   (501) staff       (20)    94884 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/Graph/400.png
--rw-r--r--   0 mirrorcraze   (501) staff       (20)    20893 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/SevenWonderEnv.py
-drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 00:11:28.266646 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/Test/
--rw-r--r--   0 mirrorcraze   (501) staff       (20)     4514 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/Test/allTests.py
--rw-r--r--   0 mirrorcraze   (501) staff       (20)       59 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/__init__.py
--rw-r--r--   0 mirrorcraze   (501) staff       (20)     2247 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/gameLog.txt
--rw-r--r--   0 mirrorcraze   (501) staff       (20)     8867 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/main.py
-drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 00:11:28.269000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/
-drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 00:11:28.270438 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Card/
--rw-r--r--   0 mirrorcraze   (501) staff       (20)    79069 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Card/card_list.json
--rw-r--r--   0 mirrorcraze   (501) staff       (20)      489 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Card/effect_list.json
--rw-r--r--   0 mirrorcraze   (501) staff       (20)      255 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Card/resources_list.json
--rw-r--r--   0 mirrorcraze   (501) staff       (20)    15475 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Card/wonders_list.json
--rw-r--r--   0 mirrorcraze   (501) staff       (20)     6976 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Personality.py
--rw-r--r--   0 mirrorcraze   (501) staff       (20)    21987 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/PlayerClass.py
--rw-r--r--   0 mirrorcraze   (501) staff       (20)      655 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/WonderClass.py
--rw-r--r--   0 mirrorcraze   (501) staff       (20)      330 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/cardClass.py
--rw-r--r--   0 mirrorcraze   (501) staff       (20)        0 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/loggers.txt
--rw-r--r--   0 mirrorcraze   (501) staff       (20)     4925 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/main.py
--rw-r--r--   0 mirrorcraze   (501) staff       (20)     1831 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/mainHelper.py
--rw-r--r--   0 mirrorcraze   (501) staff       (20)      179 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/resourceClass.py
--rw-r--r--   0 mirrorcraze   (501) staff       (20)      309 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/stageClass.py
--rw-r--r--   0 mirrorcraze   (501) staff       (20)        0 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/tester.py
--rw-r--r--   0 mirrorcraze   (501) staff       (20)     1992 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/model.py
-drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 00:11:28.263120 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv.egg-info/
--rw-r--r--   0 mirrorcraze   (501) staff       (20)      737 2023-05-10 00:49:12.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv.egg-info/SOURCES.txt
--rw-r--r--   0 mirrorcraze   (501) staff       (20)        1 2023-05-10 00:49:12.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv.egg-info/dependency_links.txt
--rw-r--r--   0 mirrorcraze   (501) staff       (20)       24 2023-05-10 00:49:12.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv.egg-info/requires.txt
--rw-r--r--   0 mirrorcraze   (501) staff       (20)       12 2023-05-10 00:49:12.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv.egg-info/top_level.txt
--rw-r--r--   0 mirrorcraze   (501) staff       (20)       22 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/_version.py
--rw-r--r--   0 mirrorcraze   (501) staff       (20)      122 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/SevenWondersEnv/setup.py
--rw-r--r--   0 mirrorcraze   (501) staff       (20)     1739 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/pyproject.toml
--rw-r--r--   0 mirrorcraze   (501) staff       (20)       38 2023-05-11 00:11:28.271318 7Wonder-RL-Lib-0.1.0/setup.cfg
--rw-r--r--   0 mirrorcraze   (501) staff       (20)       37 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.0/setup.py
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.273398 7Wonder-RL-Lib-0.1.1/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      300 2023-05-11 10:46:00.000000 7Wonder-RL-Lib-0.1.1/.bumpversion.cfg
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.214200 7Wonder-RL-Lib-0.1.1/.github/
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.214971 7Wonder-RL-Lib-0.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      834 2023-03-23 22:40:49.000000 7Wonder-RL-Lib-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      595 2023-03-23 22:40:49.000000 7Wonder-RL-Lib-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      117 2023-05-10 18:57:26.000000 7Wonder-RL-Lib-0.1.1/.github/dependabot.yml
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.215269 7Wonder-RL-Lib-0.1.1/.github/workflows/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      891 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.1/.github/workflows/build.yml
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     2145 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.1/.gitignore
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    21142 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.1/.pylintrc
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.216245 7Wonder-RL-Lib-0.1.1/7Wonder_RL_Lib.egg-info/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     5068 2023-05-11 10:50:23.000000 7Wonder-RL-Lib-0.1.1/7Wonder_RL_Lib.egg-info/PKG-INFO
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     5587 2023-05-11 10:50:23.000000 7Wonder-RL-Lib-0.1.1/7Wonder_RL_Lib.egg-info/SOURCES.txt
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)        1 2023-05-11 10:50:23.000000 7Wonder-RL-Lib-0.1.1/7Wonder_RL_Lib.egg-info/dependency_links.txt
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)       99 2023-05-11 10:50:23.000000 7Wonder-RL-Lib-0.1.1/7Wonder_RL_Lib.egg-info/requires.txt
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)       16 2023-05-11 10:50:23.000000 7Wonder-RL-Lib-0.1.1/7Wonder_RL_Lib.egg-info/top_level.txt
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      643 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     1072 2023-03-23 22:40:49.000000 7Wonder-RL-Lib-0.1.1/LICENSE
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      368 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/MANIFEST.in
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     2561 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.1/Makefile
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     5068 2023-05-11 10:50:23.273185 7Wonder-RL-Lib-0.1.1/PKG-INFO
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     3128 2023-05-11 10:32:33.000000 7Wonder-RL-Lib-0.1.1/README.md
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.216717 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.217015 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      141 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/__init__.py
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.218947 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.219272 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/GameLog/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      674 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/GameLog/gameLog0.txt
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.220994 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/Graph/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    56761 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/Graph/100.png
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    84453 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/Graph/200.png
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    93053 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/Graph/300.png
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    94884 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/Graph/400.png
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    21900 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/SevenWonderEnv.py
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.221359 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/Test/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     4514 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/Test/allTests.py
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)       59 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/__init__.py
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.223861 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.225079 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Card/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    79069 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Card/card_list.json
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      489 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Card/effect_list.json
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      255 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Card/resources_list.json
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    15475 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Card/wonders_list.json
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     6976 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Personality.py
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    21987 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/PlayerClass.py
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      655 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/WonderClass.py
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      330 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/cardClass.py
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     4925 2023-05-11 02:03:10.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/main.py
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     1831 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/mainHelper.py
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      179 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/resourceClass.py
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      309 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/stageClass.py
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)        0 2023-05-10 01:55:59.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/tester.py
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.218267 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv.egg-info/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      737 2023-05-11 02:09:37.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv.egg-info/SOURCES.txt
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)        1 2023-05-11 02:09:37.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv.egg-info/dependency_links.txt
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)       17 2023-05-11 09:28:42.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv.egg-info/requires.txt
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)       12 2023-05-11 02:09:37.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv.egg-info/top_level.txt
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)       22 2023-05-11 10:46:00.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/_version.py
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      122 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.1/SevenWondersEnv/setup.py
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.227625 7Wonder-RL-Lib-0.1.1/docs/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/.nojekyll
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      634 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/Makefile
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.227847 7Wonder-RL-Lib-0.1.1/docs/_build/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     6148 2023-05-11 07:45:08.000000 7Wonder-RL-Lib-0.1.1/docs/_build/.DS_Store
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.229040 7Wonder-RL-Lib-0.1.1/docs/_build/doctrees/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    80690 2023-05-11 03:59:02.000000 7Wonder-RL-Lib-0.1.1/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   117513 2023-05-11 03:59:02.000000 7Wonder-RL-Lib-0.1.1/docs/_build/doctrees/index.doctree
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.231318 7Wonder-RL-Lib-0.1.1/docs/_build/html/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      230 2023-05-11 03:59:02.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/.buildinfo
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.232093 7Wonder-RL-Lib-0.1.1/docs/_build/html/_sources/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      397 2023-05-11 02:30:45.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_sources/index.md.txt
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      409 2023-05-11 03:35:14.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_sources/index.rst.txt
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.236002 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    11230 2023-05-11 01:54:02.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    14813 2023-05-11 03:59:02.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.236555 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     3229 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.249101 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    87624 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    67312 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    86288 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    66444 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   165742 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   444379 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   165548 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    98024 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    77160 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   323344 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   193308 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   309728 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   184912 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   328412 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   195704 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   309192 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   182708 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   135235 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)       42 2023-05-11 01:49:34.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/custom.css
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     4472 2023-05-11 01:49:34.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      420 2023-05-11 03:59:02.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      286 2023-05-11 01:49:34.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/file.png
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.250882 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/js/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      934 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     4370 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     2734 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     5023 2023-05-11 02:36:27.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     4758 2023-05-11 03:59:02.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)       90 2023-05-11 01:49:34.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)       90 2023-05-11 01:49:34.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     4819 2023-05-11 03:59:02.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    18215 2023-05-11 01:49:34.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     4712 2023-05-11 01:49:34.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     5743 2023-05-11 03:59:02.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/genindex.html
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    22958 2023-05-11 03:59:02.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/index.html
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      371 2023-05-11 03:59:02.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/objects.inv
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     3916 2023-05-11 03:59:02.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/py-modindex.html
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     3550 2023-05-11 03:59:02.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/search.html
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     6141 2023-05-11 03:59:02.000000 7Wonder-RL-Lib-0.1.1/docs/_build/html/searchindex.js
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.251417 7Wonder-RL-Lib-0.1.1/docs/_sources/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      397 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_sources/index.md.txt
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      409 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_sources/index.rst.txt
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.254722 7Wonder-RL-Lib-0.1.1/docs/_static/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    11230 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/alabaster.css
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    14813 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/basic.css
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.255284 7Wonder-RL-Lib-0.1.1/docs/_static/css/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     3229 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/badge_only.css
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.270033 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    87624 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    67312 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    86288 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    66444 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   165742 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   444379 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   165548 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    98024 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    77160 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   323344 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   193308 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   309728 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   184912 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   328412 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   195704 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   309192 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   182708 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   135235 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/css/theme.css
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)       42 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/custom.css
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     4472 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/doctools.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      420 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/documentation_options.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      286 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/file.png
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.272140 7Wonder-RL-Lib-0.1.1/docs/_static/js/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      934 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/js/badge_only.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     4370 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     2734 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/js/html5shiv.min.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     5023 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/js/theme.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     4758 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/language_data.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)       90 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/minus.png
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)       90 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/plus.png
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     4819 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/pygments.css
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    18215 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/searchtools.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     4712 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/_static/sphinx_highlight.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     1487 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/conf.py
+drwxr-xr-x   0 mirrorcraze   (501) staff       (20)        0 2023-05-11 10:50:23.272696 7Wonder-RL-Lib-0.1.1/docs/doctrees/
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    80690 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/doctrees/environment.pickle
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)   117513 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/doctrees/index.doctree
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     5743 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/genindex.html
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)    22958 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/index.html
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      409 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/index.rst
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      800 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/make.bat
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)      371 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/objects.inv
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     3916 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/py-modindex.html
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     3550 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/search.html
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     6141 2023-05-11 10:26:44.000000 7Wonder-RL-Lib-0.1.1/docs/searchindex.js
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)     1737 2023-05-11 10:46:00.000000 7Wonder-RL-Lib-0.1.1/pyproject.toml
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)       38 2023-05-11 10:50:23.273458 7Wonder-RL-Lib-0.1.1/setup.cfg
+-rw-r--r--   0 mirrorcraze   (501) staff       (20)       37 2023-05-10 23:56:47.000000 7Wonder-RL-Lib-0.1.1/setup.py
```

### Comparing `7Wonder-RL-Lib-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `7Wonder-RL-Lib-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `7Wonder-RL-Lib-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/.github/workflows/build.yml` & `7Wonder-RL-Lib-0.1.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/.gitignore` & `7Wonder-RL-Lib-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/.pylintrc` & `7Wonder-RL-Lib-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/7Wonder_RL_Lib.egg-info/PKG-INFO` & `7Wonder-RL-Lib-0.1.1/7Wonder_RL_Lib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 7Wonder-RL-Lib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Gymnasium Environment for the game Seven Wonders
 Author-email: Phudis Dawieang <pd2654@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Phudis Dawieang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,25 +43,36 @@
 <img alt="GitHub" src="https://img.shields.io/github/license/mirrorcraze/7Wonder-RL-Lib">
 
 <img alt="GitHub issues" src="https://img.shields.io/github/issues/mirrorcraze/7Wonder-RL-Lib">
 
 [![codecov](https://codecov.io/gh/MirrorCraze/7Wonder-RL-Lib/branch/main/graph/badge.svg?token=7JDHEZ4E76)](https://codecov.io/gh/MirrorCraze/7Wonder-RL-Lib)
 [![CodeQL](https://github.com/MirrorCraze/7Wonder-RL-Lib/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/MirrorCraze/7Wonder-RL-Lib/actions/workflows/github-code-scanning/codeql)
 [![Build + CodeCov + Pylint/Black](https://github.com/MirrorCraze/7Wonder-RL-Lib/actions/workflows/build.yml/badge.svg)](https://github.com/MirrorCraze/7Wonder-RL-Lib/actions/workflows/build.yml)
+[![PyPI](https://img.shields.io/pypi/v/7Wonder-RL-Lib)](https://pypi.org/project/7Wonder-RL-Lib/0.1.0/)
+[![GitHub Pages](https://img.shields.io/badge/Github%20Pages-Link-lightgrey)](https://mirrorcraze.github.io/7Wonder-RL-Lib/)
 
 ## Overview
 There are multiple environments for the AI game testing. However, environments implemented now are mostly covered only the traditional board games (Go, Chess, etc.) or 52-card based card games (Poker, Rummy, etc.) where games do not really have interactions with other players.
 
 Most of the Euro-games board games are good game environments to test the algorithm on as there are many aspects to explore, such as tradings, dealing with imperfect informations, stochastic elements, etc.
 
 7 Wonders board games introduced multiple elements mentioned above which are good for testing out new algorithm. This library will cover basic game systems and allow users to customize the environments with custom state space and rewarding systems.
 
 ## Installation
-To install the gym environment, run ```pip install -e SevenWondersEnv```
+To install the gym environment, run 
+```
+make develop
+make build 
+make install
+```
+
+## Usage
 Example codes of how to declare the gym environment is displayed below
+
+
 ```
 import SevenWonEnv
 from SevenWonEnv.envs.mainGameEnv import Personality 
 
 env = gym.make("SevenWonderEnv", player=4) #Declare Environment with 4 Players
 ```
 To use the Personality that is given (RandomAI, RuleBasedAI, DQNAI, Human), use ```setPersonality(personalityList)```
```

### Comparing `7Wonder-RL-Lib-0.1.0/LICENSE` & `7Wonder-RL-Lib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/Makefile` & `7Wonder-RL-Lib-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/PKG-INFO` & `7Wonder-RL-Lib-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 7Wonder-RL-Lib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Gymnasium Environment for the game Seven Wonders
 Author-email: Phudis Dawieang <pd2654@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Phudis Dawieang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,25 +43,36 @@
 <img alt="GitHub" src="https://img.shields.io/github/license/mirrorcraze/7Wonder-RL-Lib">
 
 <img alt="GitHub issues" src="https://img.shields.io/github/issues/mirrorcraze/7Wonder-RL-Lib">
 
 [![codecov](https://codecov.io/gh/MirrorCraze/7Wonder-RL-Lib/branch/main/graph/badge.svg?token=7JDHEZ4E76)](https://codecov.io/gh/MirrorCraze/7Wonder-RL-Lib)
 [![CodeQL](https://github.com/MirrorCraze/7Wonder-RL-Lib/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/MirrorCraze/7Wonder-RL-Lib/actions/workflows/github-code-scanning/codeql)
 [![Build + CodeCov + Pylint/Black](https://github.com/MirrorCraze/7Wonder-RL-Lib/actions/workflows/build.yml/badge.svg)](https://github.com/MirrorCraze/7Wonder-RL-Lib/actions/workflows/build.yml)
+[![PyPI](https://img.shields.io/pypi/v/7Wonder-RL-Lib)](https://pypi.org/project/7Wonder-RL-Lib/0.1.0/)
+[![GitHub Pages](https://img.shields.io/badge/Github%20Pages-Link-lightgrey)](https://mirrorcraze.github.io/7Wonder-RL-Lib/)
 
 ## Overview
 There are multiple environments for the AI game testing. However, environments implemented now are mostly covered only the traditional board games (Go, Chess, etc.) or 52-card based card games (Poker, Rummy, etc.) where games do not really have interactions with other players.
 
 Most of the Euro-games board games are good game environments to test the algorithm on as there are many aspects to explore, such as tradings, dealing with imperfect informations, stochastic elements, etc.
 
 7 Wonders board games introduced multiple elements mentioned above which are good for testing out new algorithm. This library will cover basic game systems and allow users to customize the environments with custom state space and rewarding systems.
 
 ## Installation
-To install the gym environment, run ```pip install -e SevenWondersEnv```
+To install the gym environment, run 
+```
+make develop
+make build 
+make install
+```
+
+## Usage
 Example codes of how to declare the gym environment is displayed below
+
+
 ```
 import SevenWonEnv
 from SevenWonEnv.envs.mainGameEnv import Personality 
 
 env = gym.make("SevenWonderEnv", player=4) #Declare Environment with 4 Players
 ```
 To use the Personality that is given (RandomAI, RuleBasedAI, DQNAI, Human), use ```setPersonality(personalityList)```
```

### Comparing `7Wonder-RL-Lib-0.1.0/README.md` & `7Wonder-RL-Lib-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,36 @@
 <img alt="GitHub" src="https://img.shields.io/github/license/mirrorcraze/7Wonder-RL-Lib">
 
 <img alt="GitHub issues" src="https://img.shields.io/github/issues/mirrorcraze/7Wonder-RL-Lib">
 
 [![codecov](https://codecov.io/gh/MirrorCraze/7Wonder-RL-Lib/branch/main/graph/badge.svg?token=7JDHEZ4E76)](https://codecov.io/gh/MirrorCraze/7Wonder-RL-Lib)
 [![CodeQL](https://github.com/MirrorCraze/7Wonder-RL-Lib/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/MirrorCraze/7Wonder-RL-Lib/actions/workflows/github-code-scanning/codeql)
 [![Build + CodeCov + Pylint/Black](https://github.com/MirrorCraze/7Wonder-RL-Lib/actions/workflows/build.yml/badge.svg)](https://github.com/MirrorCraze/7Wonder-RL-Lib/actions/workflows/build.yml)
+[![PyPI](https://img.shields.io/pypi/v/7Wonder-RL-Lib)](https://pypi.org/project/7Wonder-RL-Lib/0.1.0/)
+[![GitHub Pages](https://img.shields.io/badge/Github%20Pages-Link-lightgrey)](https://mirrorcraze.github.io/7Wonder-RL-Lib/)
 
 ## Overview
 There are multiple environments for the AI game testing. However, environments implemented now are mostly covered only the traditional board games (Go, Chess, etc.) or 52-card based card games (Poker, Rummy, etc.) where games do not really have interactions with other players.
 
 Most of the Euro-games board games are good game environments to test the algorithm on as there are many aspects to explore, such as tradings, dealing with imperfect informations, stochastic elements, etc.
 
 7 Wonders board games introduced multiple elements mentioned above which are good for testing out new algorithm. This library will cover basic game systems and allow users to customize the environments with custom state space and rewarding systems.
 
 ## Installation
-To install the gym environment, run ```pip install -e SevenWondersEnv```
+To install the gym environment, run 
+```
+make develop
+make build 
+make install
+```
+
+## Usage
 Example codes of how to declare the gym environment is displayed below
+
+
 ```
 import SevenWonEnv
 from SevenWonEnv.envs.mainGameEnv import Personality 
 
 env = gym.make("SevenWonderEnv", player=4) #Declare Environment with 4 Players
 ```
 To use the Personality that is given (RandomAI, RuleBasedAI, DQNAI, Human), use ```setPersonality(personalityList)```
@@ -46,8 +57,8 @@
 ```
 class RandomAI(Personality):
     def __init__(self):
         super().__init__()
 
     def make_choice(self, player, age, options):
         return random.choice(range(len(options)))
-```
+```
```

### Comparing `7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/GameLog/gameLog0.txt` & `7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/GameLog/gameLog0.txt`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/Graph/100.png` & `7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/Graph/100.png`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/Graph/200.png` & `7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/Graph/200.png`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/Graph/300.png` & `7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/Graph/300.png`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/Graph/400.png` & `7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/Graph/400.png`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/SevenWonderEnv.py` & `7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/SevenWonderEnv.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,34 +20,36 @@
 )
 from SevenWonEnv.envs.mainGameEnv.stageClass import Stage
 
 EnvAmount = 0
 
 
 class SevenWonderEnv(gym.Env):
-    def loadWonder(self):
+
+    #Private helper methods
+    def __loadWonder(self):
         fileOper = open("mainGameEnv/Card/wonders_list.json", "rt")
         wonderList = json.load(fileOper)
         wonderList = wonderList["wonders"]
         wonderName = list(wonderList.keys())
         fileOper.close()
         return wonderList, wonderName
 
-    def actionToCode(self, cardCode, actionCode):
+    def __actionToCode(self, cardCode, actionCode):
         return cardCode * 4 + actionCode
 
-    def codeToAction(self, action):
+    def __codeToAction(self, action):
         cardCode = int(action / 4)
         actionCode = action % 4
         # convert cardCode and actionCode to ones that can be used in step
         card = self.dictCard[cardCode]
         playlist = self.dictPlay[actionCode]
         return card, playlist
 
-    def initActionSpace(self):
+    def __initActionSpace(self):
         counter = 0
         fileOper = open("mainGameEnv/Card/card_list.json", "rt")
         cardList = json.load(fileOper)
         for age in cardList:
             for playerNum in cardList[age]:
                 for color in cardList[age][playerNum]:
                     for card in cardList[age][playerNum][color]:
@@ -74,45 +76,29 @@
             None,
         ]  # playStatus -1 = discard the card for 3 coins
         self.dictPlay[3] = [2, None, None, None]  # upgrade wonders
         fileOper.close()
 
     metadata = {"render.modes": ["human"]}
 
-    def getCardAge(self, age, player, cardList):
-        jsonAge = filterPlayer(cardList[age], player)
-        cardAge = []
-        for color in jsonAge:
-            for card in jsonAge[color]:
-                card = buildCard(card["name"], color, card["payResource"], card["getResource"])
-                cardAge.append(card)
-        return cardAge
-
-    def addPlayer(self, personality):
+    def __addPlayer(self, personality):
         assignNumber = self.player - self.unAssignedPersonality + 1
         self.playerList[assignNumber].assignPersonality(personality)
         self.unAssignedPersonality -= 1
         print("Player {} is ".format(assignNumber), personality)
 
-    def setPersonality(self, personalityList):
-        self.personalityList = personalityList
-        for personality in personalityList:
-            if self.unAssignedPersonality == 0:
-                sys.exit("Program Stopped : Add too many players' personality")
-            self.addPlayer(personality)
-
-    def initGameNPerson(self, player):
+    def __initGameNPerson(self, player):
         self.unAssignedPersonality = player
         fileOper = open("mainGameEnv/Card/card_list.json", "rt")
         cardList = json.load(fileOper)
         cardAge = []
         for i in range(1, 4):
             cardAge.append(self.getCardAge("age_" + str(i), player, cardList))
         fileOper.close()
-        wonderList, wonderName = self.loadWonder()
+        wonderList, wonderName = self.__loadWonder()
         random.shuffle(wonderName)
         wonderSelected = wonderName[0:player]
         playerList = {}
         for i in range(1, player + 1):
             newPlayer = Player(i, player, Human)
             side = "A" if random.randrange(2) % 2 == 0 else "B"
             wonderCurName = wonderSelected[i - 1]
@@ -123,43 +109,16 @@
             playerList[i] = newPlayer
         for i in range(1, player + 1):
             curPlayer = playerList[i]
             playerList[i].assignLeftRight(playerList[curPlayer.left], playerList[curPlayer.right])
         print("SETUP COMPLETE")
         return cardAge, playerList
 
-    def legalAction(self, playerNum):
-        player = self.playerList[playerNum]
-        actionCode = range(4)
-        posAct = []
-        for card in player.hand:
-            if self.specialAction == 1:  # play from discard
-                posAct.append(self.actionToCode(self.dictCardToCode[card.name], 0))
-                continue
-            for action in actionCode:
-                if action == 2:  # discard is always available
-                    posAct.append(self.actionToCode(self.dictCardToCode[card.name], action))
-                if action == 0:  # pay normally
-                    left, right = player.playable(card)
-                    if left != -1 and right != -1:
-                        posAct.append(self.actionToCode(self.dictCardToCode[card.name], action))
-                if action == 1:  # pay with effect freeStructure
-                    if player.freeStructure:
-                        posAct.append(self.actionToCode(self.dictCardToCode[card.name], action))
-                if action == 3:
-                    steps = player.wonders.step
-                    existedStage = player.wonders.stage + 1
-                    # print(type(steps[existedStage]))
-                    if existedStage < len(steps):
-                        left, right = player.playable(steps[existedStage])
-                        if left != -1 and right != -1:
-                            posAct.append(self.actionToCode(self.dictCardToCode[card.name], action))
-        return posAct
 
-    def stateGenerator(self, playerNum):
+    def __stateGenerator(self, playerNum):
         state = []
         for resourceAmount in self.playerList[playerNum].resource.values():
             state.append(resourceAmount)
         for colorAmount in self.playerList[playerNum].color.values():
             state.append(colorAmount)
         for eastPrice in self.playerList[playerNum].eastTradePrices.values():
             state.append(eastPrice - 1)
@@ -173,72 +132,27 @@
         for resourceAmount in self.playerList[playerNum].right.resource.values():
             state.append(resourceAmount)
         for colorAmount in self.playerList[playerNum].right.color.values():
             state.append(colorAmount)
         state.append(self.age - 1)
         return state
 
-    def __init__(self, player):
-        global EnvAmount
-        super(SevenWonderEnv, self).__init__()
-        self.player = player
-        self.dictPlay = {}
-        self.dictCard = {}
-        self.dictCardToCode = {}
-        self.personalityList = []
-        self.initActionSpace()
-        path = "GameLog/gameLog" + str(EnvAmount) + ".txt"
-        EnvAmount = EnvAmount + 1
-        # sys.stdout = open(path, 'w')
-        # action space
-        # 75 unique cards to play * (play(2, use effect FREESTRUCTURE and NOT use effect) + discard(1) + upgradeWonder(1) = 4 action per card) = 300 total actions
-        # action = 4*cardCode + actionCode
-        self.action_space = spaces.Discrete(300)
-        # observation space
-        # resourceAmountOwn(11) + colorAmountOwn(7)+ownEastTradingCost(7)+ownWestTradingCost(7)+ coin (1) resourceAmountLeft(11)+colorAmountLeft(7)
-        # +resourceAmountRight(11)+colorAmountRight(7)+AgeNumber(1)
-        # =observation_space of 70
-        obserSpaceSize = (
-            ([5] * 10 + [20] + [10] * 7 + [2] * 7 + [2] * 7 + [100])
-            + ([5] * 10 + [20] + [10] * 7)
-            + ([5] * 10 + [20] + [10] * 7)
-            + [3]
-        )
-        self.observation_space = spaces.MultiDiscrete(obserSpaceSize)
-        self.discarded = []
-        self.cardAge = None
-        self.playerList = None
-        self.age = 1
-        self.turn = 0
-        self.cardShuffled = []
-        self.specialAction = 0
-        self.tempCardList = []
-        self.unAssignedPersonality = 0
-        self.cardAge, self.playerList = self.initGameNPerson(self.player)
-        for ageNum in range(1, 4):
-            cardThisAge = self.cardAge[ageNum - 1]
-            random.shuffle(cardThisAge)
-            self.cardShuffled.append([cardThisAge[i : i + 7] for i in range(0, len(cardThisAge), 7)])
-        for i in range(len(self.cardShuffled[0])):
-            self.playerList[i + 1].assignHand(self.cardShuffled[0][i])
-        print("Setup complete")
-
     def printPersonality(self):
         for i in range(1, self.player + 1):
             print(self.playerList[i].personality)
 
-    def stepActionDict(self):
+    def __stepActionDict(self):
         actionDict = {}
         for i in range(1, self.player + 1):
             card, action = self.playerList[i].playCard(self.age)
-            actionDict[i] = self.actionToCode(card, action)
+            actionDict[i] = self.__actionToCode(card, action)
         return actionDict
 
-    def illegalAction(self, action, playerNum):
-        cardName, actionList = self.codeToAction(action)
+    def __illegalAction(self, action, playerNum):
+        cardName, actionList = self.__codeToAction(action)
         card = self.playerList[playerNum].findCardFromHand(cardName)
         info = {}
         done = False
         reward = 0
         if card is None:
             return True  # Card not on hand
         if self.specialAction != 0:  # extraTurn from card effect
@@ -252,23 +166,23 @@
                     return True  # illegal action. Can't upgrade wonders if it's already maxed
         if actionList[0] == 2 and self.playerList[playerNum].wonders.stage + 1 >= len(
             self.playerList[playerNum].wonders.step
         ):
             return True  # illegal action. Can't upgrade wonders if it's already maxed
         return False
 
-    def rewardCalculation(self, action, playerNum):
-        cardName, actionList = self.codeToAction(action)
+    def __rewardCalculation(self, action, playerNum):
+        cardName, actionList = self.__codeToAction(action)
         player = self.playerList[playerNum]
         card = player.findCardFromHand(cardName)
         info = {}
         done = False
         reward = 0
-        if self.illegalAction(action, playerNum):
-            state = self.stateGenerator(playerNum)
+        if self.__illegalAction(action, playerNum):
+            state = self.__stateGenerator(playerNum)
             vecState = np.array(state).reshape((70,))
             return vecState, -10000, done, info
         left, right = player.playable(card)
         if self.specialAction != 0:  # extraTurn from card effect
             if self.specialAction == 1:  # buildDiscarded
                 left, right = (0, 0)
                 selectedCard = [card, left, right, actionList[0]]
@@ -286,15 +200,15 @@
                         left,
                         right,
                         0,
                         card,
                     ]
                 cardGet, action = player.playChosenCard(selectedCard)
                 self.specialAction = 0
-            state = self.stateGenerator(playerNum)
+            state = self.__stateGenerator(playerNum)
             vecState = np.array(state).reshape((70,))
             if self.turn == 6 and "extraPlay" not in info.keys():
                 for j in range(len(self.playerList)):
                     self.discarded.append(self.playerList[j + 1].hand[0])
                     # print(self.playerList[j + 1].hand)
                 if player.endAgeEffect == "playSeventhCard":
                     info["extraPlay"] = "playSeventhCard"
@@ -341,28 +255,109 @@
                     right,
                     0,
                     card,
                 ]
             cardGet, action = player.playChosenCard(selectedCard)
             if action == -1:
                 self.discarded.append(card)
-        state = self.stateGenerator(playerNum)
+        state = self.__stateGenerator(playerNum)
         vecState = np.array(state).reshape((70,))
         return vecState, reward, done, info
 
+
+    #Public methods
+    def __init__(self, player):
+        """
+        Initialize the environment with given amount of player
+        Args:
+            player: amount of player
+        """
+        global EnvAmount
+        super(SevenWonderEnv, self).__init__()
+        self.player = player
+        self.dictPlay = {}
+        self.dictCard = {}
+        self.dictCardToCode = {}
+        self.personalityList = []
+        self.__initActionSpace()
+        path = "GameLog/gameLog" + str(EnvAmount) + ".txt"
+        EnvAmount = EnvAmount + 1
+        # sys.stdout = open(path, 'w')
+        # action space
+        # 75 unique cards to play * (play(2, use effect FREESTRUCTURE and NOT use effect) + discard(1) + upgradeWonder(1) = 4 action per card) = 300 total actions
+        # action = 4*cardCode + actionCode
+        self.action_space = spaces.Discrete(300)
+        # observation space
+        # resourceAmountOwn(11) + colorAmountOwn(7)+ownEastTradingCost(7)+ownWestTradingCost(7)+ coin (1) resourceAmountLeft(11)+colorAmountLeft(7)
+        # +resourceAmountRight(11)+colorAmountRight(7)+AgeNumber(1)
+        # =observation_space of 70
+        obserSpaceSize = (
+            ([5] * 10 + [20] + [10] * 7 + [2] * 7 + [2] * 7 + [100])
+            + ([5] * 10 + [20] + [10] * 7)
+            + ([5] * 10 + [20] + [10] * 7)
+            + [3]
+        )
+        self.observation_space = spaces.MultiDiscrete(obserSpaceSize)
+        self.discarded = []
+        self.cardAge = None
+        self.playerList = None
+        self.age = 1
+        self.turn = 0
+        self.cardShuffled = []
+        self.specialAction = 0
+        self.tempCardList = []
+        self.unAssignedPersonality = 0
+        self.cardAge, self.playerList = self.__initGameNPerson(self.player)
+        for ageNum in range(1, 4):
+            cardThisAge = self.cardAge[ageNum - 1]
+            random.shuffle(cardThisAge)
+            self.cardShuffled.append([cardThisAge[i : i + 7] for i in range(0, len(cardThisAge), 7)])
+        for i in range(len(self.cardShuffled[0])):
+            self.playerList[i + 1].assignHand(self.cardShuffled[0][i])
+        print("Setup complete")
+    def setPersonality(self, personalityList):
+        """
+        Set the personality for each player.
+
+        Args:
+            personalityList: List[Personality]
+        """
+        self.personalityList = personalityList
+        for personality in personalityList:
+            if self.unAssignedPersonality == 0:
+                sys.exit("Program Stopped : Add too many players' personality")
+            self.__addPlayer(personality)
+
+    def getCardAge(self, age, player, cardList):
+        jsonAge = filterPlayer(cardList[age], player)
+        cardAge = []
+        for color in jsonAge:
+            for card in jsonAge[color]:
+                card = buildCard(card["name"], color, card["payResource"], card["getResource"])
+                cardAge.append(card)
+        return cardAge
     def step(self, action):
+        """
+        Proceed one turn of the game.
+
+        Args:
+            action: 0 by default.
+
+        Returns:
+            List[tuple] containing (new_state, reward, done, info)
+        """
         if self.unAssignedPersonality != 0:
             sys.exit("Program Stopped : Some Players do not have personality.")
         rewardAll = []
         for j in range(0, len(self.playerList)):
             card, action = self.playerList[j + 1].playCard(self.age)
             print("Card, action", card, action)
 
-            actionCode = self.actionToCode(self.dictCardToCode[card.name], action)
-            vecState, reward, done, info = self.rewardCalculation(actionCode, j + 1)
+            actionCode = self.__actionToCode(self.dictCardToCode[card.name], action)
+            vecState, reward, done, info = self.__rewardCalculation(actionCode, j + 1)
             rewardAll.append((vecState, reward, done, info))
             if action == -1:  # card discarded
                 self.discarded.append(card)
                 print("PLAYER {} discard {}".format(j + 1, card.name))
             elif action == 2:
                 print("PLAYER {} upgrade wonders to stage {}".format(j + 1, self.playerList[j + 1].wonders.stage))
             else:
@@ -437,29 +432,77 @@
         #    print("Card")
         #    for card in playerCur.hand:
         #        print(card.name)
 
         # print("special " + str(self.specialAction))
 
         return rewardAll
+    def legalAction(self, playerNum):
+        """
+        Given the player number, return all legal actions as a list of action code
+
+        Args:
+            playerNum: The position of player (1-n)
+
+        Returns:
+            List[actionCode]
+
+        """
+        player = self.playerList[playerNum]
+        actionCode = range(4)
+        posAct = []
+        for card in player.hand:
+            if self.specialAction == 1:  # play from discard
+                posAct.append(self.__actionToCode(self.dictCardToCode[card.name], 0))
+                continue
+            for action in actionCode:
+                if action == 2:  # discard is always available
+                    posAct.append(self.__actionToCode(self.dictCardToCode[card.name], action))
+                if action == 0:  # pay normally
+                    left, right = player.playable(card)
+                    if left != -1 and right != -1:
+                        posAct.append(self.__actionToCode(self.dictCardToCode[card.name], action))
+                if action == 1:  # pay with effect freeStructure
+                    if player.freeStructure:
+                        posAct.append(self.__actionToCode(self.dictCardToCode[card.name], action))
+                if action == 3:
+                    steps = player.wonders.step
+                    existedStage = player.wonders.stage + 1
+                    # print(type(steps[existedStage]))
+                    if existedStage < len(steps):
+                        left, right = player.playable(steps[existedStage])
+                        if left != -1 and right != -1:
+                            posAct.append(self.__actionToCode(self.dictCardToCode[card.name], action))
+        return posAct
 
     def reset(self, seed=None, options=None):
+        """
+        Reset the environment after each episode
+
+        Args:
+            seed: Seed ID for randomization
+            options: Default to None
+
+        Returns:
+            List[State]
+
+        """
         self.age = 1
         self.turn = 0
         self.cardShuffled = []
         self.discarded = []
-        self.cardAge, self.playerList = self.initGameNPerson(self.player)
+        self.cardAge, self.playerList = self.__initGameNPerson(self.player)
         self.setPersonality(self.personalityList)
         for ageNum in range(1, 4):
             cardThisAge = self.cardAge[ageNum - 1]
             random.shuffle(cardThisAge)
             self.cardShuffled.append([cardThisAge[i : i + 7] for i in range(0, len(cardThisAge), 7)])
         for i in range(len(self.cardShuffled[0])):
             self.playerList[i + 1].assignHand(self.cardShuffled[0][i])
-        state = self.stateGenerator(1)
+        state = self.__stateGenerator(1)
         vecState = np.array(state).reshape((70,))
         # (vecState.shape)
         return vecState
 
     def render(self, mode="human"):
         pass
```

### Comparing `7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/Test/allTests.py` & `7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/Test/allTests.py`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Card/card_list.json` & `7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Card/card_list.json`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Card/wonders_list.json` & `7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Card/wonders_list.json`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Personality.py` & `7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/Personality.py`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/PlayerClass.py` & `7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/PlayerClass.py`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/WonderClass.py` & `7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/WonderClass.py`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/main.py` & `7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/main.py`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/mainHelper.py` & `7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv/envs/mainGameEnv/mainHelper.py`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/SevenWondersEnv/SevenWonEnv.egg-info/SOURCES.txt` & `7Wonder-RL-Lib-0.1.1/SevenWondersEnv/SevenWonEnv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `7Wonder-RL-Lib-0.1.0/pyproject.toml` & `7Wonder-RL-Lib-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "7Wonder-RL-Lib"
 authors = [{name = "Phudis Dawieang", email = "pd2654@columbia.edu"}]
 description="Gymnasium Environment for the game Seven Wonders"
 readme = "README.md"
-version = "0.1.0"
+version="0.1.1"
 requires-python = ">=3.9"
 
 dependencies = ["gymnasium"]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

