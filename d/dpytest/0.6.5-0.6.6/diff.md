# Comparing `tmp/dpytest-0.6.5.tar.gz` & `tmp/dpytest-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpytest-0.6.5.tar", last modified: Sat Apr 29 10:40:53 2023, max compression
+gzip compressed data, was "dpytest-0.6.6.tar", last modified: Thu May 11 08:49:49 2023, max compression
```

## Comparing `dpytest-0.6.5.tar` & `dpytest-0.6.6.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:53.195425 dpytest-0.6.5/
--rw-rw-rw-   0        0        0     1906 2023-04-29 10:38:51.000000 dpytest-0.6.5/HISTORY.md
--rw-rw-rw-   0        0        0     1102 2022-11-29 17:57:13.000000 dpytest-0.6.5/LICENSE
--rw-rw-rw-   0        0        0      228 2022-11-30 13:48:52.000000 dpytest-0.6.5/MANIFEST.in
--rw-rw-rw-   0        0        0     5380 2023-04-29 10:40:53.197427 dpytest-0.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     1142 2023-04-20 13:50:15.000000 dpytest-0.6.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:52.825855 dpytest-0.6.5/discord/
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:52.826869 dpytest-0.6.5/discord/ext/
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:52.885619 dpytest-0.6.5/discord/ext/test/
--rw-rw-rw-   0        0        0      586 2023-04-29 10:39:11.000000 dpytest-0.6.5/discord/ext/test/__init__.py
--rw-rw-rw-   0        0        0      541 2023-01-13 14:54:07.000000 dpytest-0.6.5/discord/ext/test/_types.py
--rw-rw-rw-   0        0        0    41717 2023-04-29 10:26:18.000000 dpytest-0.6.5/discord/ext/test/backend.py
--rw-rw-rw-   0        0        0     1992 2022-11-29 17:57:13.000000 dpytest-0.6.5/discord/ext/test/callbacks.py
--rw-rw-rw-   0        0        0    20502 2023-04-29 10:26:18.000000 dpytest-0.6.5/discord/ext/test/factories.py
--rw-rw-rw-   0        0        0    14511 2023-04-29 10:26:18.000000 dpytest-0.6.5/discord/ext/test/runner.py
--rw-rw-rw-   0        0        0     3873 2023-04-29 10:26:18.000000 dpytest-0.6.5/discord/ext/test/state.py
--rw-rw-rw-   0        0        0     1870 2023-02-24 14:30:23.000000 dpytest-0.6.5/discord/ext/test/utils.py
--rw-rw-rw-   0        0        0    10242 2022-11-29 17:57:13.000000 dpytest-0.6.5/discord/ext/test/verify.py
--rw-rw-rw-   0        0        0     1355 2023-04-29 10:26:18.000000 dpytest-0.6.5/discord/ext/test/voice.py
--rw-rw-rw-   0        0        0     1605 2022-11-30 13:48:52.000000 dpytest-0.6.5/discord/ext/test/websocket.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:52.897711 dpytest-0.6.5/docs/
--rw-rw-rw-   0        0        0     2957 2023-04-29 10:39:11.000000 dpytest-0.6.5/docs/conf.py
--rw-rw-rw-   0        0        0      796 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:52.978948 dpytest-0.6.5/docs/modules/
--rw-rw-rw-   0        0        0       64 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/backend.rst
--rw-rw-rw-   0        0        0       70 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/callbacks.rst
--rw-rw-rw-   0        0        0       70 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/factories.rst
--rw-rw-rw-   0        0        0      171 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/index.rst
--rw-rw-rw-   0        0        0       61 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/runner.rst
--rw-rw-rw-   0        0        0       58 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/state.rst
--rw-rw-rw-   0        0        0       58 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/utils.rst
--rw-rw-rw-   0        0        0       61 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/verify.rst
--rw-rw-rw-   0        0        0       70 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/websocket.rst
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:53.016080 dpytest-0.6.5/docs/tutorials/
--rw-rw-rw-   0        0        0     1707 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/tutorials/getting_started.rst
--rw-rw-rw-   0        0        0      310 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/tutorials/index.rst
--rw-rw-rw-   0        0        0     5008 2022-11-30 13:48:52.000000 dpytest-0.6.5/docs/tutorials/using_pytest.rst
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:53.080889 dpytest-0.6.5/dpytest.egg-info/
--rw-rw-rw-   0        0        0     5380 2023-04-29 10:40:52.000000 dpytest-0.6.5/dpytest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1493 2023-04-29 10:40:52.000000 dpytest-0.6.5/dpytest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 10:40:52.000000 dpytest-0.6.5/dpytest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2023-04-29 10:40:52.000000 dpytest-0.6.5/dpytest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-29 10:40:52.000000 dpytest-0.6.5/dpytest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1534 2023-04-20 13:50:51.000000 dpytest-0.6.5/pyproject.toml
--rw-rw-rw-   0        0        0      514 2023-04-29 10:40:53.202427 dpytest-0.6.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:53.161428 dpytest-0.6.5/tests/
--rw-rw-rw-   0        0        0        0 2022-11-29 17:57:13.000000 dpytest-0.6.5/tests/__init__.py
--rw-rw-rw-   0        0        0     1377 2023-02-28 14:20:17.000000 dpytest-0.6.5/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:53.164428 dpytest-0.6.5/tests/data/
--rw-rw-rw-   0        0        0     3561 2022-11-29 17:57:13.000000 dpytest-0.6.5/tests/data/loremimpsum.txt
--rw-rw-rw-   0        0        0    48027 2022-11-29 17:57:13.000000 dpytest-0.6.5/tests/data/unit-tests.jpg
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:53.169467 dpytest-0.6.5/tests/internal/
--rw-rw-rw-   0        0        0        0 2022-11-29 17:57:13.000000 dpytest-0.6.5/tests/internal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:53.194429 dpytest-0.6.5/tests/internal/cogs/
--rw-rw-rw-   0        0        0        0 2022-11-29 17:57:13.000000 dpytest-0.6.5/tests/internal/cogs/__init__.py
--rw-rw-rw-   0        0        0      330 2022-11-30 13:48:52.000000 dpytest-0.6.5/tests/internal/cogs/echo.py
--rw-rw-rw-   0        0        0      352 2022-11-30 13:48:52.000000 dpytest-0.6.5/tests/internal/cogs/greeting.py
--rw-rw-rw-   0        0        0      809 2022-11-30 10:51:57.000000 dpytest-0.6.5/tests/test_activity.py
--rw-rw-rw-   0        0        0      948 2023-04-29 10:26:18.000000 dpytest-0.6.5/tests/test_create_channel.py
--rw-rw-rw-   0        0        0      508 2022-11-30 11:00:30.000000 dpytest-0.6.5/tests/test_dmchannel.py
--rw-rw-rw-   0        0        0      552 2023-04-03 09:36:38.000000 dpytest-0.6.5/tests/test_edit.py
--rw-rw-rw-   0        0        0      442 2022-12-11 11:08:54.000000 dpytest-0.6.5/tests/test_fetch_message.py
--rw-rw-rw-   0        0        0     1800 2022-11-30 13:48:52.000000 dpytest-0.6.5/tests/test_get.py
--rw-rw-rw-   0        0        0      783 2022-11-30 10:51:13.000000 dpytest-0.6.5/tests/test_member.py
--rw-rw-rw-   0        0        0     1386 2022-11-30 11:00:21.000000 dpytest-0.6.5/tests/test_mentions.py
--rw-rw-rw-   0        0        0     1192 2023-01-13 15:03:51.000000 dpytest-0.6.5/tests/test_message.py
--rw-rw-rw-   0        0        0     2333 2022-12-05 09:09:54.000000 dpytest-0.6.5/tests/test_permissions.py
--rw-rw-rw-   0        0        0     1789 2022-11-30 10:51:19.000000 dpytest-0.6.5/tests/test_reactions.py
--rw-rw-rw-   0        0        0     1926 2023-01-13 14:55:26.000000 dpytest-0.6.5/tests/test_role.py
--rw-rw-rw-   0        0        0      509 2022-12-11 11:06:57.000000 dpytest-0.6.5/tests/test_send.py
--rw-rw-rw-   0        0        0     3102 2023-02-24 14:30:23.000000 dpytest-0.6.5/tests/test_utils.py
--rw-rw-rw-   0        0        0     1684 2022-11-30 13:48:52.000000 dpytest-0.6.5/tests/test_verify_embed.py
--rw-rw-rw-   0        0        0     1146 2022-11-30 10:51:30.000000 dpytest-0.6.5/tests/test_verify_file.py
--rw-rw-rw-   0        0        0     1675 2023-02-24 14:38:30.000000 dpytest-0.6.5/tests/test_verify_message.py
--rw-rw-rw-   0        0        0      754 2023-04-29 10:26:18.000000 dpytest-0.6.5/tests/test_voice.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:49:49.272755 dpytest-0.6.6/
+-rw-rw-rw-   0        0        0     1969 2023-05-11 08:45:53.000000 dpytest-0.6.6/HISTORY.md
+-rw-rw-rw-   0        0        0     1102 2023-05-05 10:24:22.000000 dpytest-0.6.6/LICENSE
+-rw-rw-rw-   0        0        0      228 2023-05-05 10:24:22.000000 dpytest-0.6.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     5443 2023-05-11 08:49:49.276753 dpytest-0.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2023-05-05 10:24:22.000000 dpytest-0.6.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 08:49:48.334757 dpytest-0.6.6/discord/
+drwxrwxrwx   0        0        0        0 2023-05-11 08:49:48.337762 dpytest-0.6.6/discord/ext/
+drwxrwxrwx   0        0        0        0 2023-05-11 08:49:48.494756 dpytest-0.6.6/discord/ext/test/
+-rw-rw-rw-   0        0        0      586 2023-05-11 08:46:22.000000 dpytest-0.6.6/discord/ext/test/__init__.py
+-rw-rw-rw-   0        0        0      541 2023-05-05 10:24:22.000000 dpytest-0.6.6/discord/ext/test/_types.py
+-rw-rw-rw-   0        0        0    41717 2023-05-11 08:44:19.000000 dpytest-0.6.6/discord/ext/test/backend.py
+-rw-rw-rw-   0        0        0     1992 2023-05-05 10:24:22.000000 dpytest-0.6.6/discord/ext/test/callbacks.py
+-rw-rw-rw-   0        0        0    20502 2023-05-11 08:44:19.000000 dpytest-0.6.6/discord/ext/test/factories.py
+-rw-rw-rw-   0        0        0    14745 2023-05-11 08:44:19.000000 dpytest-0.6.6/discord/ext/test/runner.py
+-rw-rw-rw-   0        0        0     3873 2023-05-05 10:24:22.000000 dpytest-0.6.6/discord/ext/test/state.py
+-rw-rw-rw-   0        0        0     1870 2023-05-05 11:49:16.000000 dpytest-0.6.6/discord/ext/test/utils.py
+-rw-rw-rw-   0        0        0    10242 2023-05-05 10:24:22.000000 dpytest-0.6.6/discord/ext/test/verify.py
+-rw-rw-rw-   0        0        0     1355 2023-05-05 10:24:22.000000 dpytest-0.6.6/discord/ext/test/voice.py
+-rw-rw-rw-   0        0        0     1605 2023-05-05 10:24:22.000000 dpytest-0.6.6/discord/ext/test/websocket.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:49:48.524752 dpytest-0.6.6/docs/
+-rw-rw-rw-   0        0        0     2957 2023-05-11 08:46:22.000000 dpytest-0.6.6/docs/conf.py
+-rw-rw-rw-   0        0        0      796 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 08:49:48.796753 dpytest-0.6.6/docs/modules/
+-rw-rw-rw-   0        0        0       64 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/backend.rst
+-rw-rw-rw-   0        0        0       70 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/callbacks.rst
+-rw-rw-rw-   0        0        0       70 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/factories.rst
+-rw-rw-rw-   0        0        0      171 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/index.rst
+-rw-rw-rw-   0        0        0       61 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/runner.rst
+-rw-rw-rw-   0        0        0       58 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/state.rst
+-rw-rw-rw-   0        0        0       58 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/utils.rst
+-rw-rw-rw-   0        0        0       61 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/verify.rst
+-rw-rw-rw-   0        0        0       70 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/websocket.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 08:49:48.955751 dpytest-0.6.6/docs/tutorials/
+-rw-rw-rw-   0        0        0     1707 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/tutorials/getting_started.rst
+-rw-rw-rw-   0        0        0      310 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/tutorials/index.rst
+-rw-rw-rw-   0        0        0     5008 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/tutorials/using_pytest.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 08:49:49.055757 dpytest-0.6.6/dpytest.egg-info/
+-rw-rw-rw-   0        0        0     5443 2023-05-11 08:49:48.000000 dpytest-0.6.6/dpytest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1493 2023-05-11 08:49:48.000000 dpytest-0.6.6/dpytest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 08:49:48.000000 dpytest-0.6.6/dpytest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2023-05-11 08:49:48.000000 dpytest-0.6.6/dpytest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-11 08:49:48.000000 dpytest-0.6.6/dpytest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1534 2023-05-05 10:24:22.000000 dpytest-0.6.6/pyproject.toml
+-rw-rw-rw-   0        0        0      514 2023-05-11 08:49:49.293752 dpytest-0.6.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 08:49:49.242753 dpytest-0.6.6/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     1377 2023-05-05 12:04:47.000000 dpytest-0.6.6/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:49:49.259750 dpytest-0.6.6/tests/data/
+-rw-rw-rw-   0        0        0     3561 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/data/loremimpsum.txt
+-rw-rw-rw-   0        0        0    48027 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/data/unit-tests.jpg
+drwxrwxrwx   0        0        0        0 2023-05-11 08:49:49.262751 dpytest-0.6.6/tests/internal/
+-rw-rw-rw-   0        0        0        0 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/internal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:49:49.269753 dpytest-0.6.6/tests/internal/cogs/
+-rw-rw-rw-   0        0        0        0 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/internal/cogs/__init__.py
+-rw-rw-rw-   0        0        0      330 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/internal/cogs/echo.py
+-rw-rw-rw-   0        0        0      352 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/internal/cogs/greeting.py
+-rw-rw-rw-   0        0        0      809 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_activity.py
+-rw-rw-rw-   0        0        0      948 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_create_channel.py
+-rw-rw-rw-   0        0        0      508 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_dmchannel.py
+-rw-rw-rw-   0        0        0      552 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_edit.py
+-rw-rw-rw-   0        0        0      442 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_fetch_message.py
+-rw-rw-rw-   0        0        0     1800 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_get.py
+-rw-rw-rw-   0        0        0      783 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_member.py
+-rw-rw-rw-   0        0        0     1386 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_mentions.py
+-rw-rw-rw-   0        0        0     1192 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_message.py
+-rw-rw-rw-   0        0        0     2333 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_permissions.py
+-rw-rw-rw-   0        0        0     1789 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_reactions.py
+-rw-rw-rw-   0        0        0     1926 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_role.py
+-rw-rw-rw-   0        0        0      509 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_send.py
+-rw-rw-rw-   0        0        0     3102 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_utils.py
+-rw-rw-rw-   0        0        0     1684 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_verify_embed.py
+-rw-rw-rw-   0        0        0     1146 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_verify_file.py
+-rw-rw-rw-   0        0        0     1675 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_verify_message.py
+-rw-rw-rw-   0        0        0      754 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_voice.py
```

### Comparing `dpytest-0.6.5/HISTORY.md` & `dpytest-0.6.6/HISTORY.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # History
 
+## 0.6.6
+
+Support asyncio tasks that have no \_\_name\_\_
+
 ## 0.6.5
 
 This release allows testing with Voice Channels.
 
 New :
 
 - `FakeVoiceChannel` and `FakeVoiceClient` classes implemetation
```

### Comparing `dpytest-0.6.5/LICENSE` & `dpytest-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/PKG-INFO` & `dpytest-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpytest
-Version: 0.6.5
+Version: 0.6.6
 Summary: A package that assists in writing tests for discord.py
 Author-email: Rune Tynan <runetynan@gmail.com>
 Maintainer: CraftSpider, Sergeileduc
 License: The MIT License (MIT)
         
         Copyright (c) 2018-2019 CraftSpider
         
@@ -65,14 +65,18 @@
 
 ## Documentation
 
 Documentation can be found at [dpytest.readthedocs.io](https://dpytest.readthedocs.io/en/latest/), including examples and tutorials
 
 # History
 
+## 0.6.6
+
+Support asyncio tasks that have no \_\_name\_\_
+
 ## 0.6.5
 
 This release allows testing with Voice Channels.
 
 New :
 
 - `FakeVoiceChannel` and `FakeVoiceClient` classes implemetation
```

### Comparing `dpytest-0.6.5/README.md` & `dpytest-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/discord/ext/test/__init__.py` & `dpytest-0.6.6/discord/ext/test/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 __title__ = "dpytest"
 __author__ = "Rune Tynan"
 __license__ = "MIT"
 __copyright__ = "Copyright 2018-2019 CraftSpider"
-__version__ = "0.6.5"
+__version__ = "0.6.6"
 
 from . import backend as backend
 
 from .runner import *
 
 from .utils import embed_eq as embed_eq
 from .utils import activity_eq as activity_eq
```

### Comparing `dpytest-0.6.5/discord/ext/test/_types.py` & `dpytest-0.6.6/discord/ext/test/_types.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/discord/ext/test/backend.py` & `dpytest-0.6.6/discord/ext/test/backend.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/discord/ext/test/callbacks.py` & `dpytest-0.6.6/discord/ext/test/callbacks.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/discord/ext/test/factories.py` & `dpytest-0.6.6/discord/ext/test/factories.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/discord/ext/test/runner.py` & `dpytest-0.6.6/discord/ext/test/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,40 +57,47 @@
 
     wrapper.__wrapped__ = func
     wrapper.__annotations__ = func.__annotations__
     wrapper.__doc__ = func.__doc__
     return wrapper
 
 
+def _task_coro_name(task: asyncio.Task) -> typing.Optional[str]:
+    """
+        Uses getattr() to avoid AttributeErrors when the _coro doesn't have a __name__
+    """
+    return getattr(task._coro, "__name__", None)
+
+
 async def run_all_events() -> None:
     """
         Ensure that all dpy related coroutines have completed or been cancelled. If any dpy coroutines
         are currently running, this will also wait for those.
     """
     while True:
         if sys.version_info[1] >= 7:
             pending = asyncio.all_tasks()
         else:
             pending = asyncio.Task.all_tasks()
-        if not any(map(lambda x: x._coro.__name__ == "_run_event" and not (x.done() or x.cancelled()), pending)):
+        if not any(map(lambda x: _task_coro_name(x) == "_run_event" and not (x.done() or x.cancelled()), pending)):
             break
         for task in pending:
-            if task._coro.__name__ == "_run_event" and not (task.done() or task.cancelled()):
+            if _task_coro_name(task) == "_run_event" and not (task.done() or task.cancelled()):
                 await task
 
 
 async def finish_on_command_error() -> None:
     """
         Ensure that all dpy related coroutines have completed or been cancelled. This will only
         wait for dpy related coroutines, not any other coroutines currently running.
     """
     if sys.version_info[1] >= 7:
-        pending = filter(lambda x: x._coro.__name__ == "_run_event", asyncio.all_tasks())
+        pending = filter(lambda x: _task_coro_name(x) == "_run_event", asyncio.all_tasks())
     else:
-        pending = filter(lambda x: x._coro.__name__ == "_run_event", asyncio.Task.all_tasks())
+        pending = filter(lambda x: _task_coro_name(x) == "_run_event", asyncio.Task.all_tasks())
     for task in pending:
         if not (task.done() or task.cancelled()):
             await task
 
 
 def get_message(peek: bool = False) -> discord.Message:
     """
```

### Comparing `dpytest-0.6.5/discord/ext/test/state.py` & `dpytest-0.6.6/discord/ext/test/state.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/discord/ext/test/utils.py` & `dpytest-0.6.6/discord/ext/test/utils.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/discord/ext/test/verify.py` & `dpytest-0.6.6/discord/ext/test/verify.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/discord/ext/test/voice.py` & `dpytest-0.6.6/discord/ext/test/voice.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/discord/ext/test/websocket.py` & `dpytest-0.6.6/discord/ext/test/websocket.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/docs/conf.py` & `dpytest-0.6.6/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'dpytest'
 copyright = '2020, CraftSpider'
 author = 'CraftSpider'
 
 # The full version, including alpha/beta/rc tags
-release = '0.6.5'
+release = '0.6.6'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `dpytest-0.6.5/docs/index.rst` & `dpytest-0.6.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/docs/tutorials/getting_started.rst` & `dpytest-0.6.6/docs/tutorials/getting_started.rst`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/docs/tutorials/using_pytest.rst` & `dpytest-0.6.6/docs/tutorials/using_pytest.rst`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/dpytest.egg-info/PKG-INFO` & `dpytest-0.6.6/dpytest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpytest
-Version: 0.6.5
+Version: 0.6.6
 Summary: A package that assists in writing tests for discord.py
 Author-email: Rune Tynan <runetynan@gmail.com>
 Maintainer: CraftSpider, Sergeileduc
 License: The MIT License (MIT)
         
         Copyright (c) 2018-2019 CraftSpider
         
@@ -65,14 +65,18 @@
 
 ## Documentation
 
 Documentation can be found at [dpytest.readthedocs.io](https://dpytest.readthedocs.io/en/latest/), including examples and tutorials
 
 # History
 
+## 0.6.6
+
+Support asyncio tasks that have no \_\_name\_\_
+
 ## 0.6.5
 
 This release allows testing with Voice Channels.
 
 New :
 
 - `FakeVoiceChannel` and `FakeVoiceClient` classes implemetation
```

### Comparing `dpytest-0.6.5/dpytest.egg-info/SOURCES.txt` & `dpytest-0.6.6/dpytest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/pyproject.toml` & `dpytest-0.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
     "Topic :: Software Development :: Testing",
 ]
 
 dependencies = [
-    "discord.py == 2.2.2",
+    "discord.py == 2.2.3",
     "pytest",
     "pytest-asyncio",
 ]
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-asyncio"]
 doc = ["sphinx"]
```

### Comparing `dpytest-0.6.5/setup.cfg` & `dpytest-0.6.6/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.6.5
+current_version = 0.6.6
 commit = True
 tag = True
 
 [tool:pytest]
 junit_family = xunit1
 testpaths = tests
 markers =
```

### Comparing `dpytest-0.6.5/tests/conftest.py` & `dpytest-0.6.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/tests/data/loremimpsum.txt` & `dpytest-0.6.6/tests/data/loremimpsum.txt`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/tests/data/unit-tests.jpg` & `dpytest-0.6.6/tests/data/unit-tests.jpg`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/tests/test_activity.py` & `dpytest-0.6.6/tests/test_activity.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/tests/test_create_channel.py` & `dpytest-0.6.6/tests/test_create_channel.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/tests/test_edit.py` & `dpytest-0.6.6/tests/test_edit.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/tests/test_get.py` & `dpytest-0.6.6/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/tests/test_member.py` & `dpytest-0.6.6/tests/test_member.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/tests/test_mentions.py` & `dpytest-0.6.6/tests/test_mentions.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/tests/test_message.py` & `dpytest-0.6.6/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/tests/test_permissions.py` & `dpytest-0.6.6/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/tests/test_reactions.py` & `dpytest-0.6.6/tests/test_reactions.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/tests/test_role.py` & `dpytest-0.6.6/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/tests/test_utils.py` & `dpytest-0.6.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/tests/test_verify_embed.py` & `dpytest-0.6.6/tests/test_verify_embed.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/tests/test_verify_file.py` & `dpytest-0.6.6/tests/test_verify_file.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/tests/test_verify_message.py` & `dpytest-0.6.6/tests/test_verify_message.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.5/tests/test_voice.py` & `dpytest-0.6.6/tests/test_voice.py`

 * *Files identical despite different names*

