# Comparing `tmp/columbia-discord-bot-0.1.1.tar.gz` & `tmp/columbia-discord-bot-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "columbia-discord-bot-0.1.1.tar", last modified: Sat Apr  8 00:31:53 2023, max compression
+gzip compressed data, was "columbia-discord-bot-0.2.1.tar", last modified: Thu May 11 02:52:05 2023, max compression
```

## Comparing `columbia-discord-bot-0.1.1.tar` & `columbia-discord-bot-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,2139 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 00:31:53.964516 columbia-discord-bot-0.1.1/
--rw-rw-rw-   0        0        0      311 2023-04-07 23:40:19.000000 columbia-discord-bot-0.1.1/.bumpversion.cfg
--rw-rw-rw-   0        0        0     2123 2023-04-07 23:46:27.000000 columbia-discord-bot-0.1.1/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11558 2023-04-07 23:40:18.000000 columbia-discord-bot-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      445 2023-04-07 23:40:19.000000 columbia-discord-bot-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2251 2023-04-07 23:40:19.000000 columbia-discord-bot-0.1.1/Makefile
--rw-rw-rw-   0        0        0      351 2023-04-08 00:31:53.964017 columbia-discord-bot-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-04-07 23:40:19.000000 columbia-discord-bot-0.1.1/Pipfile
--rw-rw-rw-   0        0        0     1621 2023-04-07 23:40:19.000000 columbia-discord-bot-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 00:31:53.952018 columbia-discord-bot-0.1.1/columbia_discord_bot.egg-info/
--rw-rw-rw-   0        0        0      351 2023-04-08 00:31:53.000000 columbia-discord-bot-0.1.1/columbia_discord_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      663 2023-04-08 00:31:53.000000 columbia-discord-bot-0.1.1/columbia_discord_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 00:31:53.000000 columbia-discord-bot-0.1.1/columbia_discord_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-08 00:31:53.000000 columbia-discord-bot-0.1.1/columbia_discord_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 00:31:53.000000 columbia-discord-bot-0.1.1/columbia_discord_bot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-08 00:31:53.954020 columbia-discord-bot-0.1.1/project/
--rw-rw-rw-   0        0        0     1334 2023-04-07 23:40:19.000000 columbia-discord-bot-0.1.1/project/columbia_discord_bot.py
-drwxrwxrwx   0        0        0        0 2023-04-08 00:31:53.961017 columbia-discord-bot-0.1.1/project/integration test/
--rw-rw-rw-   0        0        0     1063 2023-04-07 23:40:19.000000 columbia-discord-bot-0.1.1/project/integration test/LICENSE
--rw-rw-rw-   0        0        0      165 2023-04-07 23:40:19.000000 columbia-discord-bot-0.1.1/project/integration test/Pipfile
--rw-rw-rw-   0        0        0      994 2023-04-07 23:40:19.000000 columbia-discord-bot-0.1.1/project/integration test/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 00:31:53.962017 columbia-discord-bot-0.1.1/project/integration test/dismock/
--rw-rw-rw-   0        0        0    15175 2023-04-08 00:20:32.000000 columbia-discord-bot-0.1.1/project/integration test/dismock/__init__.py
--rw-rw-rw-   0        0        0      464 2023-04-07 23:40:19.000000 columbia-discord-bot-0.1.1/project/integration test/example_bot.py
--rw-rw-rw-   0        0        0      580 2023-04-07 23:40:19.000000 columbia-discord-bot-0.1.1/project/integration test/example_tests.py
--rw-rw-rw-   0        0        0      350 2023-04-07 23:40:19.000000 columbia-discord-bot-0.1.1/project/integration test/setup.py
--rw-rw-rw-   0        0        0     1296 2023-04-07 23:40:19.000000 columbia-discord-bot-0.1.1/project/student.py
-drwxrwxrwx   0        0        0        0 2023-04-08 00:31:53.963016 columbia-discord-bot-0.1.1/project/tests/
--rw-rw-rw-   0        0        0     1578 2023-04-07 23:40:19.000000 columbia-discord-bot-0.1.1/project/tests/unit_tests.py
--rw-rw-rw-   0        0        0     2229 2023-04-07 23:54:00.000000 columbia-discord-bot-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-08 00:31:53.964516 columbia-discord-bot-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      367 2023-04-08 00:27:10.000000 columbia-discord-bot-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.810438 columbia-discord-bot-0.2.1/
+-rw-rw-rw-   0        0        0      311 2023-05-11 02:49:28.000000 columbia-discord-bot-0.2.1/.bumpversion.cfg
+-rw-rw-rw-   0        0        0       65 2023-05-11 00:23:51.000000 columbia-discord-bot-0.2.1/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1300 2023-05-11 02:49:28.000000 columbia-discord-bot-0.2.1/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11357 2023-05-05 01:09:45.000000 columbia-discord-bot-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      606 2023-05-11 00:23:51.000000 columbia-discord-bot-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2251 2023-05-05 01:09:45.000000 columbia-discord-bot-0.2.1/Makefile
+-rw-rw-rw-   0        0        0    15887 2023-05-11 02:52:05.809436 columbia-discord-bot-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      139 2023-05-05 01:09:45.000000 columbia-discord-bot-0.2.1/Pipfile
+-rw-rw-rw-   0        0        0     1687 2023-05-11 02:35:16.000000 columbia-discord-bot-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:03.963759 columbia-discord-bot-0.2.1/columbia_discord_bot.egg-info/
+-rw-rw-rw-   0        0        0    15887 2023-05-11 02:52:00.000000 columbia-discord-bot-0.2.1/columbia_discord_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0   103369 2023-05-11 02:52:03.000000 columbia-discord-bot-0.2.1/columbia_discord_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 02:52:00.000000 columbia-discord-bot-0.2.1/columbia_discord_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      156 2023-05-11 02:52:00.000000 columbia-discord-bot-0.2.1/columbia_discord_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-11 02:52:00.000000 columbia-discord-bot-0.2.1/columbia_discord_bot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:03.966763 columbia-discord-bot-0.2.1/docs/
+-rw-rw-rw-   0        0        0      634 2023-05-11 00:23:51.000000 columbia-discord-bot-0.2.1/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:03.876680 columbia-discord-bot-0.2.1/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:03.876680 columbia-discord-bot-0.2.1/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:03.969765 columbia-discord-bot-0.2.1/docs/_build/html/_static/
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:03.970766 columbia-discord-bot-0.2.1/docs/_build/html/_static/Jinja2-3.1.2.dist-info/
+-rw-rw-rw-   0        0        0     1475 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/Jinja2-3.1.2.dist-info/LICENSE.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:03.971768 columbia-discord-bot-0.2.1/docs/_build/html/_static/MarkupSafe-2.1.2.dist-info/
+-rw-rw-rw-   0        0        0     1503 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/MarkupSafe-2.1.2.dist-info/LICENSE.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:03.973769 columbia-discord-bot-0.2.1/docs/_build/html/_static/_distutils_hack/
+-rw-rw-rw-   0        0        0     6128 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_distutils_hack/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_distutils_hack/override.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.020812 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/
+-rw-rw-rw-   0        0        0      356 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/__init__.py
+-rw-rw-rw-   0        0        0     3794 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/_argcomplete.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.023815 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/_code/
+-rw-rw-rw-   0        0        0      483 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/_code/__init__.py
+-rw-rw-rw-   0        0        0    45167 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/_code/code.py
+-rw-rw-rw-   0        0        0     7436 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/_code/source.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.027819 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/_io/
+-rw-rw-rw-   0        0        0      154 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/_io/__init__.py
+-rw-rw-rw-   0        0        0     5394 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/_io/saferepr.py
+-rw-rw-rw-   0        0        0     8152 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/_io/terminalwriter.py
+-rw-rw-rw-   0        0        0     1253 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/_io/wcwidth.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.030821 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/_py/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/_py/__init__.py
+-rw-rw-rw-   0        0        0     3014 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/_py/error.py
+-rw-rw-rw-   0        0        0    49148 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/_py/path.py
+-rw-rw-rw-   0        0        0      160 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.034824 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/assertion/
+-rw-rw-rw-   0        0        0     6458 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/assertion/__init__.py
+-rw-rw-rw-   0        0        0    45544 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/assertion/rewrite.py
+-rw-rw-rw-   0        0        0     4382 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/assertion/truncate.py
+-rw-rw-rw-   0        0        0    18009 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/assertion/util.py
+-rw-rw-rw-   0        0        0    20915 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/cacheprovider.py
+-rw-rw-rw-   0        0        0    34738 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/capture.py
+-rw-rw-rw-   0        0        0    13200 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/compat.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.039830 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/config/
+-rw-rw-rw-   0        0        0    61575 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/config/__init__.py
+-rw-rw-rw-   0        0        0    21225 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/config/argparsing.py
+-rw-rw-rw-   0        0        0     2393 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/config/compat.py
+-rw-rw-rw-   0        0        0      260 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/config/exceptions.py
+-rw-rw-rw-   0        0        0     7884 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/config/findpaths.py
+-rw-rw-rw-   0        0        0    13498 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/debugging.py
+-rw-rw-rw-   0        0        0     5487 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/deprecated.py
+-rw-rw-rw-   0        0        0    25961 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/doctest.py
+-rw-rw-rw-   0        0        0     3186 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/faulthandler.py
+-rw-rw-rw-   0        0        0    65966 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/fixtures.py
+-rw-rw-rw-   0        0        0     1339 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/freeze_support.py
+-rw-rw-rw-   0        0        0     8520 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/helpconfig.py
+-rw-rw-rw-   0        0        0    32465 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/hookspec.py
+-rw-rw-rw-   0        0        0    25716 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/junitxml.py
+-rw-rw-rw-   0        0        0    16929 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/legacypath.py
+-rw-rw-rw-   0        0        0    30626 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/logging.py
+-rw-rw-rw-   0        0        0    32448 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.042832 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/mark/
+-rw-rw-rw-   0        0        0     8468 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/mark/__init__.py
+-rw-rw-rw-   0        0        0     6385 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/mark/expression.py
+-rw-rw-rw-   0        0        0    21179 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/mark/structures.py
+-rw-rw-rw-   0        0        0    14341 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/monkeypatch.py
+-rw-rw-rw-   0        0        0    26522 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/nodes.py
+-rw-rw-rw-   0        0        0     1688 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/nose.py
+-rw-rw-rw-   0        0        0    10256 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/outcomes.py
+-rw-rw-rw-   0        0        0     3949 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/pastebin.py
+-rw-rw-rw-   0        0        0    25439 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/pathlib.py
+-rw-rw-rw-   0        0        0    61900 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/pytester.py
+-rw-rw-rw-   0        0        0     2327 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/pytester_assertions.py
+-rw-rw-rw-   0        0        0    71523 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/python.py
+-rw-rw-rw-   0        0        0    38571 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/python_api.py
+-rw-rw-rw-   0        0        0      709 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/python_path.py
+-rw-rw-rw-   0        0        0    10930 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/recwarn.py
+-rw-rw-rw-   0        0        0    20698 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/reports.py
+-rw-rw-rw-   0        0        0    18447 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/runner.py
+-rw-rw-rw-   0        0        0     2882 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/scope.py
+-rw-rw-rw-   0        0        0     3261 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/setuponly.py
+-rw-rw-rw-   0        0        0     1214 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/setupplan.py
+-rw-rw-rw-   0        0        0    10200 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/skipping.py
+-rw-rw-rw-   0        0        0     3055 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/stash.py
+-rw-rw-rw-   0        0        0     4714 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/stepwise.py
+-rw-rw-rw-   0        0        0    52060 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/terminal.py
+-rw-rw-rw-   0        0        0     2915 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/threadexception.py
+-rw-rw-rw-   0        0        0      375 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/timing.py
+-rw-rw-rw-   0        0        0    11709 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/tmpdir.py
+-rw-rw-rw-   0        0        0    14756 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/unittest.py
+-rw-rw-rw-   0        0        0     3191 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/unraisableexception.py
+-rw-rw-rw-   0        0        0     4474 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/warning_types.py
+-rw-rw-rw-   0        0        0     5070 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/_pytest/warnings.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.084870 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/
+-rw-rw-rw-   0        0        0     7086 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/__init__.py
+-rw-rw-rw-   0        0        0     5712 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/abc.py
+-rw-rw-rw-   0        0        0     2831 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/base_protocol.py
+-rw-rw-rw-   0        0        0    46342 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/client.py
+-rw-rw-rw-   0        0        0     9612 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/client_exceptions.py
+-rw-rw-rw-   0        0        0     8421 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/client_proto.py
+-rw-rw-rw-   0        0        0    38107 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/client_reqrep.py
+-rw-rw-rw-   0        0        0    10816 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/client_ws.py
+-rw-rw-rw-   0        0        0    52630 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/connector.py
+-rw-rw-rw-   0        0        0    14070 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/cookiejar.py
+-rw-rw-rw-   0        0        0     6278 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/formdata.py
+-rw-rw-rw-   0        0        0     4838 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/hdrs.py
+-rw-rw-rw-   0        0        0    27276 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/helpers.py
+-rw-rw-rw-   0        0        0     1870 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/http.py
+-rw-rw-rw-   0        0        0     2691 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/http_exceptions.py
+-rw-rw-rw-   0        0        0    34061 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/http_parser.py
+-rw-rw-rw-   0        0        0    26000 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/http_websocket.py
+-rw-rw-rw-   0        0        0     6131 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/http_writer.py
+-rw-rw-rw-   0        0        0     1177 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/locks.py
+-rw-rw-rw-   0        0        0      333 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/log.py
+-rw-rw-rw-   0        0        0    33274 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/multipart.py
+-rw-rw-rw-   0        0        0    14099 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/payload.py
+-rw-rw-rw-   0        0        0     2187 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/payload_streamer.py
+-rw-rw-rw-   0        0        0    12163 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/pytest_plugin.py
+-rw-rw-rw-   0        0        0     5252 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/resolver.py
+-rw-rw-rw-   0        0        0    21418 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/streams.py
+-rw-rw-rw-   0        0        0      998 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/tcp_helpers.py
+-rw-rw-rw-   0        0        0    22140 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/test_utils.py
+-rw-rw-rw-   0        0        0    15649 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/tracing.py
+-rw-rw-rw-   0        0        0     1830 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/typedefs.py
+-rw-rw-rw-   0        0        0    18669 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/web.py
+-rw-rw-rw-   0        0        0    17727 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/web_app.py
+-rw-rw-rw-   0        0        0    10539 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/web_exceptions.py
+-rw-rw-rw-   0        0        0    11072 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/web_fileresponse.py
+-rw-rw-rw-   0        0        0     7765 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/web_log.py
+-rw-rw-rw-   0        0        0     4256 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/web_middlewares.py
+-rw-rw-rw-   0        0        0    23078 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/web_protocol.py
+-rw-rw-rw-   0        0        0    29069 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/web_request.py
+-rw-rw-rw-   0        0        0    28296 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/web_response.py
+-rw-rw-rw-   0        0        0     6368 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/web_routedef.py
+-rw-rw-rw-   0        0        0    11538 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/web_runner.py
+-rw-rw-rw-   0        0        0     2112 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/web_server.py
+-rw-rw-rw-   0        0        0    40703 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/web_urldispatcher.py
+-rw-rw-rw-   0        0        0    17631 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/web_ws.py
+-rw-rw-rw-   0        0        0     9032 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiohttp/worker.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.085870 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiosignal/
+-rw-rw-rw-   0        0        0      867 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/aiosignal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.087872 columbia-discord-bot-0.2.1/docs/_build/html/_static/alabaster/
+-rw-rw-rw-   0        0        0      681 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/alabaster/__init__.py
+-rw-rw-rw-   0        0        0       81 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/alabaster/_version.py
+-rw-rw-rw-   0        0        0     3963 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/alabaster/support.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.097881 columbia-discord-bot-0.2.1/docs/_build/html/_static/arrow/
+-rw-rw-rw-   0        0        0      872 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/arrow/__init__.py
+-rw-rw-rw-   0        0        0       22 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/arrow/_version.py
+-rw-rw-rw-   0        0        0     2755 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/arrow/api.py
+-rw-rw-rw-   0        0        0    63570 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/arrow/arrow.py
+-rw-rw-rw-   0        0        0     3238 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/arrow/constants.py
+-rw-rw-rw-   0        0        0    11435 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/arrow/factory.py
+-rw-rw-rw-   0        0        0     5271 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/arrow/formatter.py
+-rw-rw-rw-   0        0        0   156276 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/arrow/locales.py
+-rw-rw-rw-   0        0        0    25720 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/arrow/parser.py
+-rw-rw-rw-   0        0        0     3679 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/arrow/util.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.098882 columbia-discord-bot-0.2.1/docs/_build/html/_static/async_timeout/
+-rw-rw-rw-   0        0        0     7487 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/async_timeout/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.109892 columbia-discord-bot-0.2.1/docs/_build/html/_static/attr/
+-rw-rw-rw-   0        0        0     3241 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attr/__init__.py
+-rw-rw-rw-   0        0        0     4098 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attr/_cmp.py
+-rw-rw-rw-   0        0        0     5803 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attr/_compat.py
+-rw-rw-rw-   0        0        0      826 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attr/_config.py
+-rw-rw-rw-   0        0        0    16730 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attr/_funcs.py
+-rw-rw-rw-   0        0        0    96979 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attr/_make.py
+-rw-rw-rw-   0        0        0     6271 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attr/_next_gen.py
+-rw-rw-rw-   0        0        0     2121 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attr/_version_info.py
+-rw-rw-rw-   0        0        0     3602 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attr/converters.py
+-rw-rw-rw-   0        0        0     1890 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attr/exceptions.py
+-rw-rw-rw-   0        0        0     1470 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attr/filters.py
+-rw-rw-rw-   0        0        0     1400 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attr/setters.py
+-rw-rw-rw-   0        0        0    20702 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attr/validators.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.115899 columbia-discord-bot-0.2.1/docs/_build/html/_static/attrs/
+-rw-rw-rw-   0        0        0     1039 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attrs/__init__.py
+-rw-rw-rw-   0        0        0       70 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attrs/converters.py
+-rw-rw-rw-   0        0        0       70 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attrs/exceptions.py
+-rw-rw-rw-   0        0        0       67 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attrs/filters.py
+-rw-rw-rw-   0        0        0       67 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attrs/setters.py
+-rw-rw-rw-   0        0        0       70 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/attrs/validators.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.125907 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/
+-rw-rw-rw-   0        0        0      863 2023-04-26 20:43:02.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/__init__.py
+-rw-rw-rw-   0        0        0    42619 2023-04-26 20:43:02.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/core.py
+-rw-rw-rw-   0        0        0    72571 2023-04-26 20:43:02.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/dates.py
+-rw-rw-rw-   0        0        0     2844 2023-04-26 20:43:02.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/languages.py
+-rw-rw-rw-   0        0        0     3014 2023-04-26 20:43:02.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/lists.py
+-rw-rw-rw-   0        0        0     8239 2023-04-26 20:43:02.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/localedata.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.129911 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/localtime/
+-rw-rw-rw-   0        0        0     1043 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/localtime/__init__.py
+-rw-rw-rw-   0        0        0     1207 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/localtime/_fallback.py
+-rw-rw-rw-   0        0        0     1059 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/localtime/_helpers.py
+-rw-rw-rw-   0        0        0     3455 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/localtime/_unix.py
+-rw-rw-rw-   0        0        0     3211 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/localtime/_win32.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.137918 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/messages/
+-rw-rw-rw-   0        0        0      349 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/messages/__init__.py
+-rw-rw-rw-   0        0        0    36104 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/messages/catalog.py
+-rw-rw-rw-   0        0        0     6436 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/messages/checkers.py
+-rw-rw-rw-   0        0        0    32360 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/messages/extract.py
+-rw-rw-rw-   0        0        0    41999 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/messages/frontend.py
+-rw-rw-rw-   0        0        0     7140 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/messages/jslexer.py
+-rw-rw-rw-   0        0        0     7345 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/messages/mofile.py
+-rw-rw-rw-   0        0        0     7311 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/messages/plurals.py
+-rw-rw-rw-   0        0        0    22323 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/messages/pofile.py
+-rw-rw-rw-   0        0        0    49510 2023-04-26 20:43:02.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/numbers.py
+-rw-rw-rw-   0        0        0    23216 2023-04-26 20:43:02.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/plural.py
+-rw-rw-rw-   0        0        0    26239 2023-04-26 20:43:02.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/support.py
+-rw-rw-rw-   0        0        0    11880 2023-04-26 20:43:02.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/units.py
+-rw-rw-rw-   0        0        0     7956 2023-04-26 20:43:02.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/babel/util.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.140920 columbia-discord-bot-0.2.1/docs/_build/html/_static/certifi/
+-rw-rw-rw-   0        0        0       94 2023-04-26 20:43:02.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/certifi/__init__.py
+-rw-rw-rw-   0        0        0      243 2023-04-26 20:43:02.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/certifi/__main__.py
+-rw-rw-rw-   0        0        0     4219 2023-04-26 20:43:02.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/certifi/core.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.148927 columbia-discord-bot-0.2.1/docs/_build/html/_static/charset_normalizer/
+-rw-rw-rw-   0        0        0     1594 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/charset_normalizer/__init__.py
+-rw-rw-rw-   0        0        0    19178 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/charset_normalizer/api.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.149928 columbia-discord-bot-0.2.1/docs/_build/html/_static/charset_normalizer/assets/
+-rw-rw-rw-   0        0        0    21509 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/charset_normalizer/assets/__init__.py
+-rw-rw-rw-   0        0        0    12944 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/charset_normalizer/cd.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.151931 columbia-discord-bot-0.2.1/docs/_build/html/_static/charset_normalizer/cli/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/charset_normalizer/cli/__init__.py
+-rw-rw-rw-   0        0        0    10040 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/charset_normalizer/cli/normalizer.py
+-rw-rw-rw-   0        0        0    19596 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/charset_normalizer/constant.py
+-rw-rw-rw-   0        0        0     2125 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/charset_normalizer/legacy.py
+-rw-rw-rw-   0        0        0    18829 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/charset_normalizer/md.py
+-rw-rw-rw-   0        0        0    11829 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/charset_normalizer/models.py
+-rw-rw-rw-   0        0        0    11958 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/charset_normalizer/utils.py
+-rw-rw-rw-   0        0        0       85 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/charset_normalizer/version.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.156936 columbia-discord-bot-0.2.1/docs/_build/html/_static/colorama/
+-rw-rw-rw-   0        0        0      266 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/colorama/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/colorama/ansi.py
+-rw-rw-rw-   0        0        0    11128 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     3325 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/colorama/initialise.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.162940 columbia-discord-bot-0.2.1/docs/_build/html/_static/colorama/tests/
+-rw-rw-rw-   0        0        0       75 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/colorama/tests/__init__.py
+-rw-rw-rw-   0        0        0     2839 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/colorama/tests/ansi_test.py
+-rw-rw-rw-   0        0        0    10678 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/colorama/tests/ansitowin32_test.py
+-rw-rw-rw-   0        0        0     6741 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/colorama/tests/initialise_test.py
+-rw-rw-rw-   0        0        0     1866 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/colorama/tests/isatty_test.py
+-rw-rw-rw-   0        0        0     1079 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/colorama/tests/utils.py
+-rw-rw-rw-   0        0        0     3709 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/colorama/tests/winterm_test.py
+-rw-rw-rw-   0        0        0     6181 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/colorama/win32.py
+-rw-rw-rw-   0        0        0     7134 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/colorama/winterm.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.171949 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/
+-rw-rw-rw-   0        0        0      302 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/__init__.py
+-rw-rw-rw-   0        0        0    30411 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/blocks.py
+-rw-rw-rw-   0        0        0     1430 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/cmark.py
+-rw-rw-rw-   0        0        0     3309 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/common.py
+-rw-rw-rw-   0        0        0     3644 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/dump.py
+-rw-rw-rw-   0        0        0    61553 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/entitytrans.py
+-rw-rw-rw-   0        0        0    30985 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/inlines.py
+-rw-rw-rw-   0        0        0     1268 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/main.py
+-rw-rw-rw-   0        0        0     4614 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/node.py
+-rw-rw-rw-   0        0        0     6388 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/normalize_reference.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.175952 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/render/
+-rw-rw-rw-   0        0        0        0 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/render/__init__.py
+-rw-rw-rw-   0        0        0     6585 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/render/html.py
+-rw-rw-rw-   0        0        0     1121 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/render/renderer.py
+-rw-rw-rw-   0        0        0     3879 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/render/rst.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.178956 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/tests/__init__.py
+-rw-rw-rw-   0        0        0     3540 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/tests/rst_tests.py
+-rw-rw-rw-   0        0        0     7622 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/tests/run_spec_tests.py
+-rw-rw-rw-   0        0        0     4495 2023-05-05 00:52:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/commonmark/tests/unit_tests.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.185961 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/
+-rw-rw-rw-   0        0        0      222 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/__init__.py
+-rw-rw-rw-   0        0        0      932 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/_common.py
+-rw-rw-rw-   0        0        0      142 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/_version.py
+-rw-rw-rw-   0        0        0     2678 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/easter.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.188964 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/parser/
+-rw-rw-rw-   0        0        0     1766 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/parser/__init__.py
+-rw-rw-rw-   0        0        0    58796 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/parser/_parser.py
+-rw-rw-rw-   0        0        0    13247 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/parser/isoparser.py
+-rw-rw-rw-   0        0        0    24904 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/relativedelta.py
+-rw-rw-rw-   0        0        0    66556 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/rrule.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.193969 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/tz/
+-rw-rw-rw-   0        0        0      444 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/tz/__init__.py
+-rw-rw-rw-   0        0        0    12977 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/tz/_common.py
+-rw-rw-rw-   0        0        0     2569 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/tz/_factories.py
+-rw-rw-rw-   0        0        0    62857 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/tz/tz.py
+-rw-rw-rw-   0        0        0    12935 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/tz/win.py
+-rw-rw-rw-   0        0        0       59 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/tzwin.py
+-rw-rw-rw-   0        0        0     1965 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.194970 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/zoneinfo/
+-rw-rw-rw-   0        0        0     5889 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/zoneinfo/__init__.py
+-rw-rw-rw-   0        0        0     2392 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/dateutil/zoneinfo/rebuild.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.244015 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/
+-rw-rw-rw-   0        0        0     1886 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/__init__.py
+-rw-rw-rw-   0        0        0    11051 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/__main__.py
+-rw-rw-rw-   0        0        0     1410 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/_types.py
+-rw-rw-rw-   0        0        0    65763 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/abc.py
+-rw-rw-rw-   0        0        0    26864 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/activity.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.253022 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/app_commands/
+-rw-rw-rw-   0        0        0      424 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/app_commands/__init__.py
+-rw-rw-rw-   0        0        0    18077 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/app_commands/checks.py
+-rw-rw-rw-   0        0        0    95614 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/app_commands/commands.py
+-rw-rw-rw-   0        0        0    19006 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/app_commands/errors.py
+-rw-rw-rw-   0        0        0    38500 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/app_commands/models.py
+-rw-rw-rw-   0        0        0    13123 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/app_commands/namespace.py
+-rw-rw-rw-   0        0        0    32499 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/app_commands/transformers.py
+-rw-rw-rw-   0        0        0    10686 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/app_commands/translator.py
+-rw-rw-rw-   0        0        0    47965 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/app_commands/tree.py
+-rw-rw-rw-   0        0        0    10921 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/appinfo.py
+-rw-rw-rw-   0        0        0    15837 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/asset.py
+-rw-rw-rw-   0        0        0    34509 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/audit_logs.py
+-rw-rw-rw-   0        0        0    23488 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/automod.py
+-rw-rw-rw-   0        0        0     3751 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/backoff.py
+-rw-rw-rw-   0        0        0   114410 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/channel.py
+-rw-rw-rw-   0        0        0    84965 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/client.py
+-rw-rw-rw-   0        0        0    14168 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/colour.py
+-rw-rw-rw-   0        0        0    16836 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/components.py
+-rw-rw-rw-   0        0        0     3032 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/context_managers.py
+-rw-rw-rw-   0        0        0    22722 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/embeds.py
+-rw-rw-rw-   0        0        0     8574 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/emoji.py
+-rw-rw-rw-   0        0        0    22131 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/enums.py
+-rw-rw-rw-   0        0        0     8952 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:03.888692 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.266034 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/commands/
+-rw-rw-rw-   0        0        0      437 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/commands/__init__.py
+-rw-rw-rw-   0        0        0     2638 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/commands/_types.py
+-rw-rw-rw-   0        0        0    51719 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/commands/bot.py
+-rw-rw-rw-   0        0        0    30163 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/commands/cog.py
+-rw-rw-rw-   0        0        0    34547 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/commands/context.py
+-rw-rw-rw-   0        0        0    45392 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/commands/converter.py
+-rw-rw-rw-   0        0        0     9716 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/commands/cooldowns.py
+-rw-rw-rw-   0        0        0    89352 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/commands/core.py
+-rw-rw-rw-   0        0        0    36151 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/commands/errors.py
+-rw-rw-rw-   0        0        0    22966 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/commands/flags.py
+-rw-rw-rw-   0        0        0    57705 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/commands/help.py
+-rw-rw-rw-   0        0        0    36595 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/commands/hybrid.py
+-rw-rw-rw-   0        0        0     8361 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/commands/parameters.py
+-rw-rw-rw-   0        0        0     6247 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/commands/view.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.267036 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/tasks/
+-rw-rw-rw-   0        0        0    29180 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ext/tasks/__init__.py
+-rw-rw-rw-   0        0        0     5378 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/file.py
+-rw-rw-rw-   0        0        0    52208 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/flags.py
+-rw-rw-rw-   0        0        0    34937 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/gateway.py
+-rw-rw-rw-   0        0        0   140799 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/guild.py
+-rw-rw-rw-   0        0        0    89365 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/http.py
+-rw-rw-rw-   0        0        0    13334 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/integrations.py
+-rw-rw-rw-   0        0        0    44412 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/interactions.py
+-rw-rw-rw-   0        0        0    20595 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/invite.py
+-rw-rw-rw-   0        0        0    40760 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/member.py
+-rw-rw-rw-   0        0        0     5592 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/mentions.py
+-rw-rw-rw-   0        0        0    82150 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/message.py
+-rw-rw-rw-   0        0        0     1485 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/mixins.py
+-rw-rw-rw-   0        0        0     3702 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/object.py
+-rw-rw-rw-   0        0        0     3646 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/oggparse.py
+-rw-rw-rw-   0        0        0    15065 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/opus.py
+-rw-rw-rw-   0        0        0     7950 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/partial_emoji.py
+-rw-rw-rw-   0        0        0    28320 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/permissions.py
+-rw-rw-rw-   0        0        0    26456 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/player.py
+-rw-rw-rw-   0        0        0    16826 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/raw_models.py
+-rw-rw-rw-   0        0        0     8229 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/reaction.py
+-rw-rw-rw-   0        0        0    17906 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/role.py
+-rw-rw-rw-   0        0        0    23655 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/scheduled_event.py
+-rw-rw-rw-   0        0        0    20129 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/shard.py
+-rw-rw-rw-   0        0        0     6498 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/stage_instance.py
+-rw-rw-rw-   0        0        0    73314 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/state.py
+-rw-rw-rw-   0        0        0    16029 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/sticker.py
+-rw-rw-rw-   0        0        0     4607 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/team.py
+-rw-rw-rw-   0        0        0     9574 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/template.py
+-rw-rw-rw-   0        0        0    32449 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/threads.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.292058 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/
+-rw-rw-rw-   0        0        0      149 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/__init__.py
+-rw-rw-rw-   0        0        0     2707 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/activity.py
+-rw-rw-rw-   0        0        0     2386 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/appinfo.py
+-rw-rw-rw-   0        0        0     8192 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/audit_log.py
+-rw-rw-rw-   0        0        0     4009 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/automod.py
+-rw-rw-rw-   0        0        0     4557 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/channel.py
+-rw-rw-rw-   0        0        0     6266 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/command.py
+-rw-rw-rw-   0        0        0     3057 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/components.py
+-rw-rw-rw-   0        0        0     2329 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/embed.py
+-rw-rw-rw-   0        0        0     1528 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/emoji.py
+-rw-rw-rw-   0        0        0     8453 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/gateway.py
+-rw-rw-rw-   0        0        0     5197 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/guild.py
+-rw-rw-rw-   0        0        0     2288 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/integration.py
+-rw-rw-rw-   0        0        0     6923 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/interactions.py
+-rw-rw-rw-   0        0        0     2704 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/invite.py
+-rw-rw-rw-   0        0        0     1898 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/member.py
+-rw-rw-rw-   0        0        0     4182 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/message.py
+-rw-rw-rw-   0        0        0     1746 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/role.py
+-rw-rw-rw-   0        0        0     3294 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/scheduled_event.py
+-rw-rw-rw-   0        0        0     1182 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/snowflake.py
+-rw-rw-rw-   0        0        0     2244 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/sticker.py
+-rw-rw-rw-   0        0        0     1499 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/team.py
+-rw-rw-rw-   0        0        0     1609 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/template.py
+-rw-rw-rw-   0        0        0     2454 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/threads.py
+-rw-rw-rw-   0        0        0     1540 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/user.py
+-rw-rw-rw-   0        0        0     2268 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/voice.py
+-rw-rw-rw-   0        0        0     1978 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/webhook.py
+-rw-rw-rw-   0        0        0     1460 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/welcome_screen.py
+-rw-rw-rw-   0        0        0     1883 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/types/widget.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.299064 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ui/
+-rw-rw-rw-   0        0        0      285 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ui/__init__.py
+-rw-rw-rw-   0        0        0    10620 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ui/button.py
+-rw-rw-rw-   0        0        0     5899 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ui/dynamic.py
+-rw-rw-rw-   0        0        0     4372 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ui/item.py
+-rw-rw-rw-   0        0        0     7012 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ui/modal.py
+-rw-rw-rw-   0        0        0    34049 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ui/select.py
+-rw-rw-rw-   0        0        0     8058 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ui/text_input.py
+-rw-rw-rw-   0        0        0    22878 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/ui/view.py
+-rw-rw-rw-   0        0        0    15390 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/user.py
+-rw-rw-rw-   0        0        0    41360 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/utils.py
+-rw-rw-rw-   0        0        0    24974 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/voice_client.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.302067 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/webhook/
+-rw-rw-rw-   0        0        0      182 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/webhook/__init__.py
+-rw-rw-rw-   0        0        0    69566 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/webhook/async_.py
+-rw-rw-rw-   0        0        0    42519 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/webhook/sync.py
+-rw-rw-rw-   0        0        0     7539 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/welcome_screen.py
+-rw-rw-rw-   0        0        0    10162 2023-04-26 20:39:43.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/widget.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.309074 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/
+-rw-rw-rw-   0        0        0     9389 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/__init__.py
+-rw-rw-rw-   0        0        0    29575 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/core.py
+-rw-rw-rw-   0        0        0     3959 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/examples.py
+-rw-rw-rw-   0        0        0    37324 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/frontend.py
+-rw-rw-rw-   0        0        0    17033 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/io.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.334096 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/
+-rw-rw-rw-   0        0        0     2902 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/__init__.py
+-rw-rw-rw-   0        0        0     1824 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/af.py
+-rw-rw-rw-   0        0        0     2029 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/ar.py
+-rw-rw-rw-   0        0        0     1940 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/ca.py
+-rw-rw-rw-   0        0        0     1928 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/cs.py
+-rw-rw-rw-   0        0        0     1907 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/da.py
+-rw-rw-rw-   0        0        0     1722 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/de.py
+-rw-rw-rw-   0        0        0     1848 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/en.py
+-rw-rw-rw-   0        0        0     1948 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/eo.py
+-rw-rw-rw-   0        0        0     1962 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/es.py
+-rw-rw-rw-   0        0        0     2044 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/fa.py
+-rw-rw-rw-   0        0        0     2026 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/fi.py
+-rw-rw-rw-   0        0        0     1893 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/fr.py
+-rw-rw-rw-   0        0        0     2040 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/gl.py
+-rw-rw-rw-   0        0        0     2683 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/he.py
+-rw-rw-rw-   0        0        0     1808 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/it.py
+-rw-rw-rw-   0        0        0     1942 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/ja.py
+-rw-rw-rw-   0        0        0     1882 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/ko.py
+-rw-rw-rw-   0        0        0     1940 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/lt.py
+-rw-rw-rw-   0        0        0     1867 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/lv.py
+-rw-rw-rw-   0        0        0     1865 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/nl.py
+-rw-rw-rw-   0        0        0     1900 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/pl.py
+-rw-rw-rw-   0        0        0     1982 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/pt_br.py
+-rw-rw-rw-   0        0        0     2155 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/ru.py
+-rw-rw-rw-   0        0        0     1860 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/sk.py
+-rw-rw-rw-   0        0        0     2103 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/sv.py
+-rw-rw-rw-   0        0        0     2026 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/zh_cn.py
+-rw-rw-rw-   0        0        0     2771 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/languages/zh_tw.py
+-rw-rw-rw-   0        0        0    82261 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/nodes.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.337098 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/
+-rw-rw-rw-   0        0        0     3173 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/__init__.py
+-rw-rw-rw-   0        0        0      445 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/null.py
+-rw-rw-rw-   0        0        0     6810 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/recommonmark_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.341103 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/
+-rw-rw-rw-   0        0        0    15866 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.349110 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/directives/
+-rw-rw-rw-   0        0        0    14680 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/directives/__init__.py
+-rw-rw-rw-   0        0        0     2413 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/directives/admonitions.py
+-rw-rw-rw-   0        0        0     9823 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/directives/body.py
+-rw-rw-rw-   0        0        0      691 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/directives/html.py
+-rw-rw-rw-   0        0        0     6982 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/directives/images.py
+-rw-rw-rw-   0        0        0    28454 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/directives/misc.py
+-rw-rw-rw-   0        0        0     4251 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/directives/parts.py
+-rw-rw-rw-   0        0        0      831 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/directives/references.py
+-rw-rw-rw-   0        0        0    22852 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/directives/tables.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.375133 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/
+-rw-rw-rw-   0        0        0     1222 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/__init__.py
+-rw-rw-rw-   0        0        0     3677 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/af.py
+-rw-rw-rw-   0        0        0     3355 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/ar.py
+-rw-rw-rw-   0        0        0     4467 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/ca.py
+-rw-rw-rw-   0        0        0     4857 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/cs.py
+-rw-rw-rw-   0        0        0     3765 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/da.py
+-rw-rw-rw-   0        0        0     3464 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/de.py
+-rw-rw-rw-   0        0        0     3317 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/en.py
+-rw-rw-rw-   0        0        0     3898 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/eo.py
+-rw-rw-rw-   0        0        0     4261 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/es.py
+-rw-rw-rw-   0        0        0     3430 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/fa.py
+-rw-rw-rw-   0        0        0     3661 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/fi.py
+-rw-rw-rw-   0        0        0     3709 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/fr.py
+-rw-rw-rw-   0        0        0     3711 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/gl.py
+-rw-rw-rw-   0        0        0     3640 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/he.py
+-rw-rw-rw-   0        0        0     3270 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/it.py
+-rw-rw-rw-   0        0        0     3863 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/ja.py
+-rw-rw-rw-   0        0        0     3463 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/ko.py
+-rw-rw-rw-   0        0        0     3584 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/lt.py
+-rw-rw-rw-   0        0        0     3381 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/lv.py
+-rw-rw-rw-   0        0        0     3708 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/nl.py
+-rw-rw-rw-   0        0        0     3427 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/pl.py
+-rw-rw-rw-   0        0        0     3992 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/pt_br.py
+-rw-rw-rw-   0        0        0     3306 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/ru.py
+-rw-rw-rw-   0        0        0     3979 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/sk.py
+-rw-rw-rw-   0        0        0     3331 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/sv.py
+-rw-rw-rw-   0        0        0     4007 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/zh_cn.py
+-rw-rw-rw-   0        0        0     5172 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/languages/zh_tw.py
+-rw-rw-rw-   0        0        0    15120 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/roles.py
+-rw-rw-rw-   0        0        0   132786 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/states.py
+-rw-rw-rw-   0        0        0    21001 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/parsers/rst/tableparser.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.379137 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/readers/
+-rw-rw-rw-   0        0        0     3458 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/readers/__init__.py
+-rw-rw-rw-   0        0        0     1607 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/readers/doctree.py
+-rw-rw-rw-   0        0        0     1555 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/readers/pep.py
+-rw-rw-rw-   0        0        0     2346 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/readers/standalone.py
+-rw-rw-rw-   0        0        0    57428 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/statemachine.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.388145 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/transforms/
+-rw-rw-rw-   0        0        0     6504 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/transforms/__init__.py
+-rw-rw-rw-   0        0        0     2297 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/transforms/components.py
+-rw-rw-rw-   0        0        0    20134 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/transforms/frontmatter.py
+-rw-rw-rw-   0        0        0     4881 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/transforms/misc.py
+-rw-rw-rw-   0        0        0     6992 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/transforms/parts.py
+-rw-rw-rw-   0        0        0    11154 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/transforms/peps.py
+-rw-rw-rw-   0        0        0    36694 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/transforms/references.py
+-rw-rw-rw-   0        0        0    11813 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/transforms/universal.py
+-rw-rw-rw-   0        0        0     2607 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/transforms/writer_aux.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.395152 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/utils/
+-rw-rw-rw-   0        0        0    29015 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/utils/__init__.py
+-rw-rw-rw-   0        0        0     4974 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/utils/code_analyzer.py
+-rw-rw-rw-   0        0        0     8631 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/utils/error_reporting.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.401157 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/utils/math/
+-rw-rw-rw-   0        0        0     1826 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/utils/math/__init__.py
+-rw-rw-rw-   0        0        0    51525 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/utils/math/latex2mathml.py
+-rw-rw-rw-   0        0        0   101084 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/utils/math/math2html.py
+-rw-rw-rw-   0        0        0     5708 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/utils/math/tex2mathml_extern.py
+-rw-rw-rw-   0        0        0    37450 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/utils/math/tex2unichar.py
+-rw-rw-rw-   0        0        0    19192 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/utils/math/unichar2tex.py
+-rw-rw-rw-   0        0        0     6429 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/utils/punctuation_chars.py
+-rw-rw-rw-   0        0        0     2688 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/utils/roman.py
+-rw-rw-rw-   0        0        0    39844 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/utils/smartquotes.py
+-rw-rw-rw-   0        0        0     6272 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/utils/urischemes.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.408163 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/
+-rw-rw-rw-   0        0        0     5002 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/__init__.py
+-rw-rw-rw-   0        0        0    70241 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/_html_base.py
+-rw-rw-rw-   0        0        0     7133 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/docutils_xml.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.409164 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/html4css1/
+-rw-rw-rw-   0        0        0    37712 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/html4css1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.411166 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/html5_polyglot/
+-rw-rw-rw-   0        0        0    18251 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/html5_polyglot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.412167 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/latex2e/
+-rw-rw-rw-   0        0        0   136349 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/latex2e/__init__.py
+-rw-rw-rw-   0        0        0    36643 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/manpage.py
+-rw-rw-rw-   0        0        0      450 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/null.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.414169 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/odf_odt/
+-rw-rw-rw-   0        0        0   133500 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/odf_odt/__init__.py
+-rw-rw-rw-   0        0        0     4671 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/odf_odt/pygmentsformatter.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.415169 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/pep_html/
+-rw-rw-rw-   0        0        0     3554 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/pep_html/__init__.py
+-rw-rw-rw-   0        0        0     1026 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/pseudoxml.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.416170 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/s5_html/
+-rw-rw-rw-   0        0        0    14659 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/s5_html/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.418172 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/xetex/
+-rw-rw-rw-   0        0        0     5874 2023-05-05 00:38:12.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/docutils/writers/xetex/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.419173 columbia-discord-bot-0.2.1/docs/_build/html/_static/frozenlist/
+-rw-rw-rw-   0        0        0     2419 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/frozenlist/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.427181 columbia-discord-bot-0.2.1/docs/_build/html/_static/idna/
+-rw-rw-rw-   0        0        0      849 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/idna/__init__.py
+-rw-rw-rw-   0        0        0     3374 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/idna/codec.py
+-rw-rw-rw-   0        0        0      321 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/idna/compat.py
+-rw-rw-rw-   0        0        0    12950 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/idna/core.py
+-rw-rw-rw-   0        0        0    44375 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/idna/idnadata.py
+-rw-rw-rw-   0        0        0     1881 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/idna/intranges.py
+-rw-rw-rw-   0        0        0       21 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/idna/package_data.py
+-rw-rw-rw-   0        0        0   206539 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/idna/uts46data.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.428182 columbia-discord-bot-0.2.1/docs/_build/html/_static/idna-3.4.dist-info/
+-rw-rw-rw-   0        0        0     1523 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/idna-3.4.dist-info/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.430183 columbia-discord-bot-0.2.1/docs/_build/html/_static/imagesize/
+-rw-rw-rw-   0        0        0      102 2023-04-26 20:43:01.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/imagesize/__init__.py
+-rw-rw-rw-   0        0        0    13992 2023-04-26 20:43:01.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/imagesize/imagesize.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.431184 columbia-discord-bot-0.2.1/docs/_build/html/_static/imagesize-1.4.1.dist-info/
+-rw-rw-rw-   0        0        0     1120 2023-04-26 20:43:01.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/imagesize-1.4.1.dist-info/LICENSE.rst
+-rw-rw-rw-   0        0        0    14062 2023-04-26 20:43:01.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/imagesize.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.435189 columbia-discord-bot-0.2.1/docs/_build/html/_static/iniconfig/
+-rw-rw-rw-   0        0        0     5473 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/iniconfig/__init__.py
+-rw-rw-rw-   0        0        0     2436 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/iniconfig/_parse.py
+-rw-rw-rw-   0        0        0      160 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/iniconfig/_version.py
+-rw-rw-rw-   0        0        0      501 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/iniconfig/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.460210 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/
+-rw-rw-rw-   0        0        0     1927 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/__init__.py
+-rw-rw-rw-   0        0        0     1958 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/_identifier.py
+-rw-rw-rw-   0        0        0     2472 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/async_utils.py
+-rw-rw-rw-   0        0        0    14061 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/bccache.py
+-rw-rw-rw-   0        0        0    72172 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/compiler.py
+-rw-rw-rw-   0        0        0     1433 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/constants.py
+-rw-rw-rw-   0        0        0     6299 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/debug.py
+-rw-rw-rw-   0        0        0     1267 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/defaults.py
+-rw-rw-rw-   0        0        0    61349 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/environment.py
+-rw-rw-rw-   0        0        0     5071 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/exceptions.py
+-rw-rw-rw-   0        0        0    31502 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/ext.py
+-rw-rw-rw-   0        0        0    53509 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/filters.py
+-rw-rw-rw-   0        0        0    10704 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/idtracking.py
+-rw-rw-rw-   0        0        0    29726 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/lexer.py
+-rw-rw-rw-   0        0        0    23207 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/loaders.py
+-rw-rw-rw-   0        0        0     4396 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/meta.py
+-rw-rw-rw-   0        0        0     4226 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/nativetypes.py
+-rw-rw-rw-   0        0        0    34550 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/nodes.py
+-rw-rw-rw-   0        0        0     1650 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/optimizer.py
+-rw-rw-rw-   0        0        0    39595 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/parser.py
+-rw-rw-rw-   0        0        0    33476 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/runtime.py
+-rw-rw-rw-   0        0        0    14584 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/sandbox.py
+-rw-rw-rw-   0        0        0     5905 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/tests.py
+-rw-rw-rw-   0        0        0    23965 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/utils.py
+-rw-rw-rw-   0        0        0     3568 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2/visitor.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.462212 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2_time/
+-rw-rw-rw-   0        0        0      184 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2_time/__init__.py
+-rw-rw-rw-   0        0        0     2080 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2_time/jinja2_time.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.463213 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2_time-0.2.0.dist-info/
+-rw-rw-rw-   0        0        0     4109 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/jinja2_time-0.2.0.dist-info/DESCRIPTION.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.467217 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/
+-rw-rw-rw-   0        0        0       28 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/__main__.py
+-rw-rw-rw-   0        0        0      116 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.468217 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/make_get/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/make_get/__init__.py
+-rw-rw-rw-   0        0        0     3636 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/make_get/make_get.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.470219 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/make_project/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/make_project/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.476225 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/make_project/data_medium/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/make_project/data_medium/__init__.py
+-rw-rw-rw-   0        0        0     1654 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/make_project/data_medium/base.py
+-rw-rw-rw-   0        0        0      443 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/make_project/data_medium/dry_run.py
+-rw-rw-rw-   0        0        0     2761 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/make_project/data_medium/local.py
+-rw-rw-rw-   0        0        0     3719 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/make_project/data_medium/zipsource.py
+-rw-rw-rw-   0        0        0     5570 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/make_project/make_project.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.480229 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/make_project/parsers/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/make_project/parsers/__init__.py
+-rw-rw-rw-   0        0        0     1146 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/make_project/parsers/cookiecutter_parser.py
+-rw-rw-rw-   0        0        0     2424 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/make_project/parsers/ini_parser.py
+-rw-rw-rw-   0        0        0     2552 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/make_project/parsers/json_parser.py
+-rw-rw-rw-   0        0        0      257 2023-04-26 20:40:24.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/make/template.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.481229 columbia-discord-bot-0.2.1/docs/_build/html/_static/markupsafe/
+-rw-rw-rw-   0        0        0     9601 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/markupsafe/__init__.py
+-rw-rw-rw-   0        0        0     1776 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/markupsafe/_native.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.486234 columbia-discord-bot-0.2.1/docs/_build/html/_static/multidict/
+-rw-rw-rw-   0        0        0      976 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/multidict/__init__.py
+-rw-rw-rw-   0        0        0     1238 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/multidict/_abc.py
+-rw-rw-rw-   0        0        0      330 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/multidict/_compat.py
+-rw-rw-rw-   0        0        0     3935 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/multidict/_multidict_base.py
+-rw-rw-rw-   0        0        0    15575 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/multidict/_multidict_py.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.500247 columbia-discord-bot-0.2.1/docs/_build/html/_static/packaging/
+-rw-rw-rw-   0        0        0      501 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/packaging/__init__.py
+-rw-rw-rw-   0        0        0     3266 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/packaging/_elffile.py
+-rw-rw-rw-   0        0        0     8926 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     2524 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0    10194 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/packaging/_parser.py
+-rw-rw-rw-   0        0        0     1431 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/packaging/_structures.py
+-rw-rw-rw-   0        0        0     5292 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/packaging/_tokenizer.py
+-rw-rw-rw-   0        0        0     8208 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/packaging/markers.py
+-rw-rw-rw-   0        0        0    16397 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/packaging/metadata.py
+-rw-rw-rw-   0        0        0     3287 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/packaging/requirements.py
+-rw-rw-rw-   0        0        0    39206 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    18106 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/packaging/tags.py
+-rw-rw-rw-   0        0        0     4355 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/packaging/utils.py
+-rw-rw-rw-   0        0        0    16326 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.503250 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/
+-rw-rw-rw-   0        0        0      357 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/__main__.py
+-rw-rw-rw-   0        0        0     1444 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/__pip-runner__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.511257 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/
+-rw-rw-rw-   0        0        0      573 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/__init__.py
+-rw-rw-rw-   0        0        0    10243 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/build_env.py
+-rw-rw-rw-   0        0        0     9661 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/cache.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.523269 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/cli/
+-rw-rw-rw-   0        0        0      132 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/cli/__init__.py
+-rw-rw-rw-   0        0        0     6676 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/cli/autocompletion.py
+-rw-rw-rw-   0        0        0     8176 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/cli/base_command.py
+-rw-rw-rw-   0        0        0    30030 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/cli/cmdoptions.py
+-rw-rw-rw-   0        0        0      774 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/cli/command_context.py
+-rw-rw-rw-   0        0        0     2816 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/cli/main.py
+-rw-rw-rw-   0        0        0     4338 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/cli/main_parser.py
+-rw-rw-rw-   0        0        0    10817 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/cli/parser.py
+-rw-rw-rw-   0        0        0     1968 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/cli/progress_bars.py
+-rw-rw-rw-   0        0        0    18328 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/cli/req_command.py
+-rw-rw-rw-   0        0        0     5118 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/cli/spinners.py
+-rw-rw-rw-   0        0        0      116 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/cli/status_codes.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.540283 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/
+-rw-rw-rw-   0        0        0     3882 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/__init__.py
+-rw-rw-rw-   0        0        0     7581 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/cache.py
+-rw-rw-rw-   0        0        0     1684 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/check.py
+-rw-rw-rw-   0        0        0     4129 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/completion.py
+-rw-rw-rw-   0        0        0     9815 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/configuration.py
+-rw-rw-rw-   0        0        0     6591 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/debug.py
+-rw-rw-rw-   0        0        0     5182 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/download.py
+-rw-rw-rw-   0        0        0     2951 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/freeze.py
+-rw-rw-rw-   0        0        0     1703 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/hash.py
+-rw-rw-rw-   0        0        0     1132 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/help.py
+-rw-rw-rw-   0        0        0     4793 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/index.py
+-rw-rw-rw-   0        0        0     3188 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/inspect.py
+-rw-rw-rw-   0        0        0    28722 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/install.py
+-rw-rw-rw-   0        0        0    12343 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/list.py
+-rw-rw-rw-   0        0        0     5697 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/search.py
+-rw-rw-rw-   0        0        0     6419 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/show.py
+-rw-rw-rw-   0        0        0     3886 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/uninstall.py
+-rw-rw-rw-   0        0        0     6324 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/commands/wheel.py
+-rw-rw-rw-   0        0        0    13529 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/configuration.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.545288 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/distributions/
+-rw-rw-rw-   0        0        0      858 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/distributions/__init__.py
+-rw-rw-rw-   0        0        0     1221 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/distributions/base.py
+-rw-rw-rw-   0        0        0      729 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/distributions/installed.py
+-rw-rw-rw-   0        0        0     6494 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/distributions/sdist.py
+-rw-rw-rw-   0        0        0     1164 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/distributions/wheel.py
+-rw-rw-rw-   0        0        0    23741 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.549292 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/index/
+-rw-rw-rw-   0        0        0       30 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/index/__init__.py
+-rw-rw-rw-   0        0        0    16504 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/index/collector.py
+-rw-rw-rw-   0        0        0    37873 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/index/package_finder.py
+-rw-rw-rw-   0        0        0     6556 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/index/sources.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.553295 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/locations/
+-rw-rw-rw-   0        0        0    15365 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/locations/__init__.py
+-rw-rw-rw-   0        0        0     6100 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/locations/_distutils.py
+-rw-rw-rw-   0        0        0     7680 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/locations/_sysconfig.py
+-rw-rw-rw-   0        0        0     2556 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/locations/base.py
+-rw-rw-rw-   0        0        0      340 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.557299 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/metadata/
+-rw-rw-rw-   0        0        0     4280 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/metadata/__init__.py
+-rw-rw-rw-   0        0        0     2595 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/metadata/_json.py
+-rw-rw-rw-   0        0        0    25277 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/metadata/base.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.561303 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/metadata/importlib/
+-rw-rw-rw-   0        0        0      107 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/metadata/importlib/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/metadata/importlib/_compat.py
+-rw-rw-rw-   0        0        0     8181 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/metadata/importlib/_dists.py
+-rw-rw-rw-   0        0        0     7457 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/metadata/importlib/_envs.py
+-rw-rw-rw-   0        0        0     9773 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/metadata/pkg_resources.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.573313 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/models/
+-rw-rw-rw-   0        0        0       63 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/models/__init__.py
+-rw-rw-rw-   0        0        0      990 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/models/candidate.py
+-rw-rw-rw-   0        0        0     6931 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/models/direct_url.py
+-rw-rw-rw-   0        0        0     2520 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/models/format_control.py
+-rw-rw-rw-   0        0        0     1030 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/models/index.py
+-rw-rw-rw-   0        0        0     2619 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/models/installation_report.py
+-rw-rw-rw-   0        0        0    18817 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/models/link.py
+-rw-rw-rw-   0        0        0      738 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/models/scheme.py
+-rw-rw-rw-   0        0        0     4643 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/models/search_scope.py
+-rw-rw-rw-   0        0        0     1907 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/models/selection_prefs.py
+-rw-rw-rw-   0        0        0     3858 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/models/target_python.py
+-rw-rw-rw-   0        0        0     3600 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/models/wheel.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.581322 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/network/
+-rw-rw-rw-   0        0        0       50 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/network/__init__.py
+-rw-rw-rw-   0        0        0    20435 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/network/auth.py
+-rw-rw-rw-   0        0        0     2145 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/network/cache.py
+-rw-rw-rw-   0        0        0     6096 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/network/download.py
+-rw-rw-rw-   0        0        0     7638 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/network/lazy_wheel.py
+-rw-rw-rw-   0        0        0    18442 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/network/session.py
+-rw-rw-rw-   0        0        0     4073 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/network/utils.py
+-rw-rw-rw-   0        0        0     1791 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/network/xmlrpc.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.585324 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.593332 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/build/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/build/__init__.py
+-rw-rw-rw-   0        0        0     4133 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/build/build_tracker.py
+-rw-rw-rw-   0        0        0     1422 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/build/metadata.py
+-rw-rw-rw-   0        0        0     1474 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/build/metadata_editable.py
+-rw-rw-rw-   0        0        0     2198 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/build/metadata_legacy.py
+-rw-rw-rw-   0        0        0     1075 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/build/wheel.py
+-rw-rw-rw-   0        0        0     1417 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/build/wheel_editable.py
+-rw-rw-rw-   0        0        0     3064 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/build/wheel_legacy.py
+-rw-rw-rw-   0        0        0     5122 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/check.py
+-rw-rw-rw-   0        0        0     9816 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/freeze.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.596336 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/install/
+-rw-rw-rw-   0        0        0       51 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/install/__init__.py
+-rw-rw-rw-   0        0        0     1282 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/install/editable_legacy.py
+-rw-rw-rw-   0        0        0    27475 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/install/wheel.py
+-rw-rw-rw-   0        0        0    27696 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/operations/prepare.py
+-rw-rw-rw-   0        0        0     7161 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/pyproject.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.602340 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/req/
+-rw-rw-rw-   0        0        0     2738 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/req/__init__.py
+-rw-rw-rw-   0        0        0    16610 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/req/constructors.py
+-rw-rw-rw-   0        0        0    17872 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/req/req_file.py
+-rw-rw-rw-   0        0        0    32782 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/req/req_install.py
+-rw-rw-rw-   0        0        0     2858 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/req/req_set.py
+-rw-rw-rw-   0        0        0    24678 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/req/req_uninstall.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.604342 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/resolution/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/resolution/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/resolution/base.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.605343 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/resolution/legacy/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/resolution/legacy/__init__.py
+-rw-rw-rw-   0        0        0    24128 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/resolution/legacy/resolver.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.615352 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/resolution/resolvelib/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/resolution/resolvelib/__init__.py
+-rw-rw-rw-   0        0        0     5220 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/resolution/resolvelib/base.py
+-rw-rw-rw-   0        0        0    18864 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/resolution/resolvelib/candidates.py
+-rw-rw-rw-   0        0        0    27845 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/resolution/resolvelib/factory.py
+-rw-rw-rw-   0        0        0     5705 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-rw-rw-   0        0        0     9824 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/resolution/resolvelib/provider.py
+-rw-rw-rw-   0        0        0     3094 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/resolution/resolvelib/reporter.py
+-rw-rw-rw-   0        0        0     5454 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/resolution/resolvelib/requirements.py
+-rw-rw-rw-   0        0        0    11538 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/resolution/resolvelib/resolver.py
+-rw-rw-rw-   0        0        0     8167 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/self_outdated_check.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.642377 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/__init__.py
+-rw-rw-rw-   0        0        0     3351 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/_jaraco_text.py
+-rw-rw-rw-   0        0        0     1015 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/_log.py
+-rw-rw-rw-   0        0        0     1665 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/appdirs.py
+-rw-rw-rw-   0        0        0     1884 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/compat.py
+-rw-rw-rw-   0        0        0     5377 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/compatibility_tags.py
+-rw-rw-rw-   0        0        0      242 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/datetime.py
+-rw-rw-rw-   0        0        0     3627 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/deprecation.py
+-rw-rw-rw-   0        0        0     3206 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/direct_url_helpers.py
+-rw-rw-rw-   0        0        0     2118 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/egg_link.py
+-rw-rw-rw-   0        0        0     1169 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/encoding.py
+-rw-rw-rw-   0        0        0     3064 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/entrypoints.py
+-rw-rw-rw-   0        0        0     5122 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/filesystem.py
+-rw-rw-rw-   0        0        0      716 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/filetypes.py
+-rw-rw-rw-   0        0        0     3110 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/glibc.py
+-rw-rw-rw-   0        0        0     5118 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/hashes.py
+-rw-rw-rw-   0        0        0      795 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/inject_securetransport.py
+-rw-rw-rw-   0        0        0    11632 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/logging.py
+-rw-rw-rw-   0        0        0    22216 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/misc.py
+-rw-rw-rw-   0        0        0     1193 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/models.py
+-rw-rw-rw-   0        0        0     2108 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/packaging.py
+-rw-rw-rw-   0        0        0     4435 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/setuptools_build.py
+-rw-rw-rw-   0        0        0     9200 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/subprocess.py
+-rw-rw-rw-   0        0        0     7702 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/temp_dir.py
+-rw-rw-rw-   0        0        0     8821 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/unpacking.py
+-rw-rw-rw-   0        0        0     1759 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/urls.py
+-rw-rw-rw-   0        0        0     3456 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/virtualenv.py
+-rw-rw-rw-   0        0        0     4549 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/utils/wheel.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.648382 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/vcs/
+-rw-rw-rw-   0        0        0      596 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/vcs/__init__.py
+-rw-rw-rw-   0        0        0     3519 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/vcs/bazaar.py
+-rw-rw-rw-   0        0        0    18116 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/vcs/git.py
+-rw-rw-rw-   0        0        0     5238 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/vcs/mercurial.py
+-rw-rw-rw-   0        0        0    11729 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/vcs/subversion.py
+-rw-rw-rw-   0        0        0    22811 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/vcs/versioncontrol.py
+-rw-rw-rw-   0        0        0    11842 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_internal/wheel_builder.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.651385 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/
+-rw-rw-rw-   0        0        0     4966 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.660392 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/cachecontrol/
+-rw-rw-rw-   0        0        0      465 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/cachecontrol/__init__.py
+-rw-rw-rw-   0        0        0     1379 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/cachecontrol/_cmd.py
+-rw-rw-rw-   0        0        0     5033 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/cachecontrol/adapter.py
+-rw-rw-rw-   0        0        0     1535 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/cachecontrol/cache.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.663396 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/cachecontrol/caches/
+-rw-rw-rw-   0        0        0      242 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-rw-rw-   0        0        0     5271 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-rw-rw-   0        0        0     1033 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-rw-rw-   0        0        0      778 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/cachecontrol/compat.py
+-rw-rw-rw-   0        0        0    16416 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/cachecontrol/controller.py
+-rw-rw-rw-   0        0        0     3946 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/cachecontrol/filewrapper.py
+-rw-rw-rw-   0        0        0     4154 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/cachecontrol/heuristics.py
+-rw-rw-rw-   0        0        0     7105 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/cachecontrol/serialize.py
+-rw-rw-rw-   0        0        0      774 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/cachecontrol/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.666397 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/certifi/
+-rw-rw-rw-   0        0        0       94 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/certifi/__init__.py
+-rw-rw-rw-   0        0        0      255 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/certifi/__main__.py
+-rw-rw-rw-   0        0        0     4279 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/certifi/core.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.709437 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/
+-rw-rw-rw-   0        0        0     4797 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/__init__.py
+-rw-rw-rw-   0        0        0    31274 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/big5freq.py
+-rw-rw-rw-   0        0        0     1763 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/big5prober.py
+-rw-rw-rw-   0        0        0    10032 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/chardistribution.py
+-rw-rw-rw-   0        0        0     3915 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/charsetgroupprober.py
+-rw-rw-rw-   0        0        0     5420 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/charsetprober.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.710439 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/cli/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/cli/__init__.py
+-rw-rw-rw-   0        0        0     3242 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/cli/chardetect.py
+-rw-rw-rw-   0        0        0     3732 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/codingstatemachine.py
+-rw-rw-rw-   0        0        0      542 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-rw-rw-   0        0        0     1860 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/cp949prober.py
+-rw-rw-rw-   0        0        0     1683 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/enums.py
+-rw-rw-rw-   0        0        0     4006 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/escprober.py
+-rw-rw-rw-   0        0        0    12176 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/escsm.py
+-rw-rw-rw-   0        0        0     3934 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/eucjpprober.py
+-rw-rw-rw-   0        0        0    13566 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/euckrfreq.py
+-rw-rw-rw-   0        0        0     1753 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/euckrprober.py
+-rw-rw-rw-   0        0        0    36913 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/euctwfreq.py
+-rw-rw-rw-   0        0        0     1753 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/euctwprober.py
+-rw-rw-rw-   0        0        0    20735 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/gb2312freq.py
+-rw-rw-rw-   0        0        0     1759 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/gb2312prober.py
+-rw-rw-rw-   0        0        0    14537 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/hebrewprober.py
+-rw-rw-rw-   0        0        0    25796 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/jisfreq.py
+-rw-rw-rw-   0        0        0    42498 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/johabfreq.py
+-rw-rw-rw-   0        0        0     1752 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/johabprober.py
+-rw-rw-rw-   0        0        0    27055 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/jpcntx.py
+-rw-rw-rw-   0        0        0   104562 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-rw-rw-   0        0        0    98484 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/langgreekmodel.py
+-rw-rw-rw-   0        0        0    98196 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/langhebrewmodel.py
+-rw-rw-rw-   0        0        0   101363 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/langhungarianmodel.py
+-rw-rw-rw-   0        0        0   128035 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/langrussianmodel.py
+-rw-rw-rw-   0        0        0   102774 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/langthaimodel.py
+-rw-rw-rw-   0        0        0    95372 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/langturkishmodel.py
+-rw-rw-rw-   0        0        0     5380 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/latin1prober.py
+-rw-rw-rw-   0        0        0     6077 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/macromanprober.py
+-rw-rw-rw-   0        0        0     3715 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/mbcharsetprober.py
+-rw-rw-rw-   0        0        0     2131 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-rw-rw-   0        0        0    30391 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/mbcssm.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.712440 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/metadata/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/metadata/__init__.py
+-rw-rw-rw-   0        0        0    13560 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/metadata/languages.py
+-rw-rw-rw-   0        0        0      402 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/resultdict.py
+-rw-rw-rw-   0        0        0     6400 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/sbcharsetprober.py
+-rw-rw-rw-   0        0        0     4137 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-rw-rw-   0        0        0     4007 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/sjisprober.py
+-rw-rw-rw-   0        0        0    14848 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/universaldetector.py
+-rw-rw-rw-   0        0        0     8505 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/utf1632prober.py
+-rw-rw-rw-   0        0        0     2812 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/utf8prober.py
+-rw-rw-rw-   0        0        0      244 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/chardet/version.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.718446 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/colorama/
+-rw-rw-rw-   0        0        0      266 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/colorama/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/colorama/ansi.py
+-rw-rw-rw-   0        0        0    11128 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     3325 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/colorama/initialise.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.724451 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/colorama/tests/
+-rw-rw-rw-   0        0        0       75 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/colorama/tests/__init__.py
+-rw-rw-rw-   0        0        0     2839 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/colorama/tests/ansi_test.py
+-rw-rw-rw-   0        0        0    10678 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-rw-rw-   0        0        0     6741 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/colorama/tests/initialise_test.py
+-rw-rw-rw-   0        0        0     1866 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/colorama/tests/isatty_test.py
+-rw-rw-rw-   0        0        0     1079 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/colorama/tests/utils.py
+-rw-rw-rw-   0        0        0     3709 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/colorama/tests/winterm_test.py
+-rw-rw-rw-   0        0        0     6181 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/colorama/win32.py
+-rw-rw-rw-   0        0        0     7134 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/colorama/winterm.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.737464 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distlib/
+-rw-rw-rw-   0        0        0      581 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distlib/__init__.py
+-rw-rw-rw-   0        0        0    41259 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distlib/compat.py
+-rw-rw-rw-   0        0        0    51697 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distlib/database.py
+-rw-rw-rw-   0        0        0    20834 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distlib/index.py
+-rw-rw-rw-   0        0        0    51991 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distlib/locators.py
+-rw-rw-rw-   0        0        0    14811 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distlib/manifest.py
+-rw-rw-rw-   0        0        0     5058 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distlib/markers.py
+-rw-rw-rw-   0        0        0    39801 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distlib/metadata.py
+-rw-rw-rw-   0        0        0    10820 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distlib/resources.py
+-rw-rw-rw-   0        0        0    18102 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distlib/scripts.py
+-rw-rw-rw-   0        0        0    66262 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distlib/util.py
+-rw-rw-rw-   0        0        0    23513 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distlib/version.py
+-rw-rw-rw-   0        0        0    43898 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distlib/wheel.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.740466 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distro/
+-rw-rw-rw-   0        0        0      981 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distro/__init__.py
+-rw-rw-rw-   0        0        0       64 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distro/__main__.py
+-rw-rw-rw-   0        0        0    49330 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/distro/distro.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.748473 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/idna/
+-rw-rw-rw-   0        0        0      849 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/idna/__init__.py
+-rw-rw-rw-   0        0        0     3374 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/idna/codec.py
+-rw-rw-rw-   0        0        0      321 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/idna/compat.py
+-rw-rw-rw-   0        0        0    12950 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/idna/core.py
+-rw-rw-rw-   0        0        0    44375 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/idna/idnadata.py
+-rw-rw-rw-   0        0        0     1881 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/idna/intranges.py
+-rw-rw-rw-   0        0        0       21 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/idna/package_data.py
+-rw-rw-rw-   0        0        0   206539 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/idna/uts46data.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.752477 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/msgpack/
+-rw-rw-rw-   0        0        0     1132 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/msgpack/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/msgpack/exceptions.py
+-rw-rw-rw-   0        0        0     6079 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/msgpack/ext.py
+-rw-rw-rw-   0        0        0    34544 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/msgpack/fallback.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.762486 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8487 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4676 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.763487 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pkg_resources/
+-rw-rw-rw-   0        0        0   109388 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pkg_resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.771494 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/platformdirs/
+-rw-rw-rw-   0        0        0    18003 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/platformdirs/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/platformdirs/__main__.py
+-rw-rw-rw-   0        0        0     4303 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/platformdirs/android.py
+-rw-rw-rw-   0        0        0     5706 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/platformdirs/api.py
+-rw-rw-rw-   0        0        0     2800 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/platformdirs/macos.py
+-rw-rw-rw-   0        0        0     7448 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/platformdirs/unix.py
+-rw-rw-rw-   0        0        0      160 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/platformdirs/version.py
+-rw-rw-rw-   0        0        0     7098 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/platformdirs/windows.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.786507 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/
+-rw-rw-rw-   0        0        0     2999 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/__init__.py
+-rw-rw-rw-   0        0        0      353 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/__main__.py
+-rw-rw-rw-   0        0        0    23685 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/cmdline.py
+-rw-rw-rw-   0        0        0     1697 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/console.py
+-rw-rw-rw-   0        0        0     1938 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/filter.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.787508 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/filters/
+-rw-rw-rw-   0        0        0    40386 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/filters/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/formatter.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.800521 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/formatters/
+-rw-rw-rw-   0        0        0     4800 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/formatters/__init__.py
+-rw-rw-rw-   0        0        0     4104 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/formatters/_mapping.py
+-rw-rw-rw-   0        0        0     3314 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/formatters/bbcode.py
+-rw-rw-rw-   0        0        0     5086 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/formatters/groff.py
+-rw-rw-rw-   0        0        0    35601 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/formatters/html.py
+-rw-rw-rw-   0        0        0    21938 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/formatters/img.py
+-rw-rw-rw-   0        0        0     4981 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/formatters/irc.py
+-rw-rw-rw-   0        0        0    19351 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/formatters/latex.py
+-rw-rw-rw-   0        0        0     5073 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/formatters/other.py
+-rw-rw-rw-   0        0        0     2212 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-rw-rw-   0        0        0     5014 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/formatters/rtf.py
+-rw-rw-rw-   0        0        0     7335 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/formatters/svg.py
+-rw-rw-rw-   0        0        0     4674 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/formatters/terminal.py
+-rw-rw-rw-   0        0        0    11753 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/formatters/terminal256.py
+-rw-rw-rw-   0        0        0    32064 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/lexer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.803522 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/lexers/
+-rw-rw-rw-   0        0        0    11164 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/lexers/__init__.py
+-rw-rw-rw-   0        0        0    71556 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/lexers/_mapping.py
+-rw-rw-rw-   0        0        0    53572 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/lexers/python.py
+-rw-rw-rw-   0        0        0      986 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/modeline.py
+-rw-rw-rw-   0        0        0     2591 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/plugin.py
+-rw-rw-rw-   0        0        0     3072 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/regexopt.py
+-rw-rw-rw-   0        0        0     3092 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/scanner.py
+-rw-rw-rw-   0        0        0     6882 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/sphinxext.py
+-rw-rw-rw-   0        0        0     6257 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/style.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.804524 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/styles/
+-rw-rw-rw-   0        0        0     3419 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/styles/__init__.py
+-rw-rw-rw-   0        0        0     6184 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/token.py
+-rw-rw-rw-   0        0        0    63187 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/unistring.py
+-rw-rw-rw-   0        0        0     9110 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pygments/util.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.814533 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9171 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6426 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   213344 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.814533 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    23685 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9023 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    39129 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25341 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13402 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10787 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyparsing/util.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.817535 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyproject_hooks/
+-rw-rw-rw-   0        0        0      491 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyproject_hooks/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyproject_hooks/_compat.py
+-rw-rw-rw-   0        0        0    11920 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyproject_hooks/_impl.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.819538 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyproject_hooks/_in_process/
+-rw-rw-rw-   0        0        0      546 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-rw-rw-   0        0        0    10927 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.837553 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/
+-rw-rw-rw-   0        0        0     5178 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/__version__.py
+-rw-rw-rw-   0        0        0     1397 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/_internal_utils.py
+-rw-rw-rw-   0        0        0    21443 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/adapters.py
+-rw-rw-rw-   0        0        0     6377 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/api.py
+-rw-rw-rw-   0        0        0    10187 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/auth.py
+-rw-rw-rw-   0        0        0      575 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/certs.py
+-rw-rw-rw-   0        0        0     1286 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/compat.py
+-rw-rw-rw-   0        0        0    18560 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/cookies.py
+-rw-rw-rw-   0        0        0     3823 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/exceptions.py
+-rw-rw-rw-   0        0        0     3879 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/help.py
+-rw-rw-rw-   0        0        0      733 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/hooks.py
+-rw-rw-rw-   0        0        0    35288 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/models.py
+-rw-rw-rw-   0        0        0      695 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/packages.py
+-rw-rw-rw-   0        0        0    30180 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/sessions.py
+-rw-rw-rw-   0        0        0     4235 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/status_codes.py
+-rw-rw-rw-   0        0        0     2912 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/structures.py
+-rw-rw-rw-   0        0        0    33240 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/requests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.843559 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/resolvelib/
+-rw-rw-rw-   0        0        0      537 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/resolvelib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.845561 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/resolvelib/compat/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/resolvelib/compat/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-rw-rw-   0        0        0     5871 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/resolvelib/providers.py
+-rw-rw-rw-   0        0        0     1601 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/resolvelib/reporters.py
+-rw-rw-rw-   0        0        0    20511 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/resolvelib/resolvers.py
+-rw-rw-rw-   0        0        0     4963 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/resolvelib/structs.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.920628 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/
+-rw-rw-rw-   0        0        0     6090 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/__init__.py
+-rw-rw-rw-   0        0        0     8478 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/__main__.py
+-rw-rw-rw-   0        0        0    10096 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_cell_widths.py
+-rw-rw-rw-   0        0        0   140235 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_emoji_codes.py
+-rw-rw-rw-   0        0        0     1064 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_emoji_replace.py
+-rw-rw-rw-   0        0        0     2100 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_export_format.py
+-rw-rw-rw-   0        0        0      265 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_extension.py
+-rw-rw-rw-   0        0        0      799 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_fileno.py
+-rw-rw-rw-   0        0        0     9695 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_inspect.py
+-rw-rw-rw-   0        0        0     3225 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_log_render.py
+-rw-rw-rw-   0        0        0     1236 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_loop.py
+-rw-rw-rw-   0        0        0     1387 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_null_file.py
+-rw-rw-rw-   0        0        0     7063 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_palettes.py
+-rw-rw-rw-   0        0        0      423 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_pick.py
+-rw-rw-rw-   0        0        0     5472 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_ratio.py
+-rw-rw-rw-   0        0        0    19919 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_spinners.py
+-rw-rw-rw-   0        0        0      351 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_stack.py
+-rw-rw-rw-   0        0        0      417 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_timer.py
+-rw-rw-rw-   0        0        0    22820 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_win32_console.py
+-rw-rw-rw-   0        0        0     1926 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_windows.py
+-rw-rw-rw-   0        0        0     2783 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_windows_renderer.py
+-rw-rw-rw-   0        0        0     1840 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/_wrap.py
+-rw-rw-rw-   0        0        0      890 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/abc.py
+-rw-rw-rw-   0        0        0    10368 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/align.py
+-rw-rw-rw-   0        0        0     6906 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/ansi.py
+-rw-rw-rw-   0        0        0     3264 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/bar.py
+-rw-rw-rw-   0        0        0     9842 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/box.py
+-rw-rw-rw-   0        0        0     4509 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/cells.py
+-rw-rw-rw-   0        0        0    18224 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/color.py
+-rw-rw-rw-   0        0        0     1054 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/color_triplet.py
+-rw-rw-rw-   0        0        0     7131 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/columns.py
+-rw-rw-rw-   0        0        0    99195 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/console.py
+-rw-rw-rw-   0        0        0     1288 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/constrain.py
+-rw-rw-rw-   0        0        0     5497 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/containers.py
+-rw-rw-rw-   0        0        0     6630 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/control.py
+-rw-rw-rw-   0        0        0     8082 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/default_styles.py
+-rw-rw-rw-   0        0        0      972 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/diagnose.py
+-rw-rw-rw-   0        0        0     2501 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/emoji.py
+-rw-rw-rw-   0        0        0      642 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/errors.py
+-rw-rw-rw-   0        0        0     1683 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/file_proxy.py
+-rw-rw-rw-   0        0        0     2508 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/filesize.py
+-rw-rw-rw-   0        0        0     9584 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/highlighter.py
+-rw-rw-rw-   0        0        0     5032 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/json.py
+-rw-rw-rw-   0        0        0     3252 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/jupyter.py
+-rw-rw-rw-   0        0        0    14007 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/layout.py
+-rw-rw-rw-   0        0        0    14273 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/live.py
+-rw-rw-rw-   0        0        0     3667 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/live_render.py
+-rw-rw-rw-   0        0        0    11903 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/logging.py
+-rw-rw-rw-   0        0        0     8198 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/markup.py
+-rw-rw-rw-   0        0        0     5305 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/measure.py
+-rw-rw-rw-   0        0        0     4970 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/padding.py
+-rw-rw-rw-   0        0        0      828 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/pager.py
+-rw-rw-rw-   0        0        0     3396 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/palette.py
+-rw-rw-rw-   0        0        0    10574 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/panel.py
+-rw-rw-rw-   0        0        0    35852 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/pretty.py
+-rw-rw-rw-   0        0        0    59706 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/progress.py
+-rw-rw-rw-   0        0        0     8165 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/progress_bar.py
+-rw-rw-rw-   0        0        0    11303 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/prompt.py
+-rw-rw-rw-   0        0        0     1391 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/protocol.py
+-rw-rw-rw-   0        0        0      166 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/region.py
+-rw-rw-rw-   0        0        0     4431 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/repr.py
+-rw-rw-rw-   0        0        0     4602 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/rule.py
+-rw-rw-rw-   0        0        0     2843 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/scope.py
+-rw-rw-rw-   0        0        0     1591 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/screen.py
+-rw-rw-rw-   0        0        0    24247 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/segment.py
+-rw-rw-rw-   0        0        0     4339 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/spinner.py
+-rw-rw-rw-   0        0        0     4425 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/status.py
+-rw-rw-rw-   0        0        0    27073 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/style.py
+-rw-rw-rw-   0        0        0     1258 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/styled.py
+-rw-rw-rw-   0        0        0    35153 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/syntax.py
+-rw-rw-rw-   0        0        0    39684 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/table.py
+-rw-rw-rw-   0        0        0     3370 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/terminal_theme.py
+-rw-rw-rw-   0        0        0    45525 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/text.py
+-rw-rw-rw-   0        0        0     3777 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/theme.py
+-rw-rw-rw-   0        0        0      102 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/themes.py
+-rw-rw-rw-   0        0        0    29604 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/traceback.py
+-rw-rw-rw-   0        0        0     9169 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/rich/tree.py
+-rw-rw-rw-   0        0        0    34549 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/six.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.931640 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/tenacity/
+-rw-rw-rw-   0        0        0    20493 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/tenacity/__init__.py
+-rw-rw-rw-   0        0        0     3551 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/tenacity/_asyncio.py
+-rw-rw-rw-   0        0        0     2179 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/tenacity/_utils.py
+-rw-rw-rw-   0        0        0     1682 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/tenacity/after.py
+-rw-rw-rw-   0        0        0     1562 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/tenacity/before.py
+-rw-rw-rw-   0        0        0     2372 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/tenacity/before_sleep.py
+-rw-rw-rw-   0        0        0     1383 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/tenacity/nap.py
+-rw-rw-rw-   0        0        0     8746 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/tenacity/retry.py
+-rw-rw-rw-   0        0        0     3086 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/tenacity/stop.py
+-rw-rw-rw-   0        0        0     2142 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/tenacity/tornadoweb.py
+-rw-rw-rw-   0        0        0     8024 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/tenacity/wait.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.935643 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/tomli/
+-rw-rw-rw-   0        0        0      396 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/tomli/__init__.py
+-rw-rw-rw-   0        0        0    22633 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2943 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/tomli/_re.py
+-rw-rw-rw-   0        0        0      254 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/tomli/_types.py
+-rw-rw-rw-   0        0        0    84101 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/typing_extensions.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.945652 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/
+-rw-rw-rw-   0        0        0     3333 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/__init__.py
+-rw-rw-rw-   0        0        0    10811 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/_collections.py
+-rw-rw-rw-   0        0        0       64 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/_version.py
+-rw-rw-rw-   0        0        0    20300 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/connection.py
+-rw-rw-rw-   0        0        0    39128 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/connectionpool.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.952658 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/contrib/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/contrib/__init__.py
+-rw-rw-rw-   0        0        0      957 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.954661 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-rw-   0        0        0    17632 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-rw-   0        0        0    13922 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-rw-   0        0        0    11036 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/contrib/appengine.py
+-rw-rw-rw-   0        0        0     4528 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-rw-rw-   0        0        0    17081 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-rw-rw-   0        0        0    34448 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-rw-rw-   0        0        0     7097 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/contrib/socks.py
+-rw-rw-rw-   0        0        0     8217 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/exceptions.py
+-rw-rw-rw-   0        0        0     8579 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/fields.py
+-rw-rw-rw-   0        0        0     2440 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/filepost.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.956662 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/packages/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/packages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.958663 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/packages/backports/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-rw-rw-   0        0        0     1417 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-rw-rw-   0        0        0    34665 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/packages/six.py
+-rw-rw-rw-   0        0        0    19786 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/poolmanager.py
+-rw-rw-rw-   0        0        0     5985 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/request.py
+-rw-rw-rw-   0        0        0    30641 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/response.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.970675 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/util/
+-rw-rw-rw-   0        0        0     1155 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/util/__init__.py
+-rw-rw-rw-   0        0        0     4901 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/util/connection.py
+-rw-rw-rw-   0        0        0     1605 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/util/proxy.py
+-rw-rw-rw-   0        0        0      498 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/util/queue.py
+-rw-rw-rw-   0        0        0     3997 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/util/request.py
+-rw-rw-rw-   0        0        0     3510 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/util/response.py
+-rw-rw-rw-   0        0        0    22003 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/util/retry.py
+-rw-rw-rw-   0        0        0    17177 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/util/ssl_.py
+-rw-rw-rw-   0        0        0     5758 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-rw-rw-   0        0        0     6895 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/util/ssltransport.py
+-rw-rw-rw-   0        0        0    10168 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/util/timeout.py
+-rw-rw-rw-   0        0        0    14296 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/util/url.py
+-rw-rw-rw-   0        0        0     5403 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/urllib3/util/wait.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.975679 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/webencodings/
+-rw-rw-rw-   0        0        0    10579 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/webencodings/__init__.py
+-rw-rw-rw-   0        0        0     8979 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/webencodings/labels.py
+-rw-rw-rw-   0        0        0     1305 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/webencodings/mklabels.py
+-rw-rw-rw-   0        0        0     6563 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/webencodings/tests.py
+-rw-rw-rw-   0        0        0     4307 2023-04-26 20:33:30.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/webencodings/x_user_defined.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.977681 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/
+-rw-rw-rw-   0        0        0   108568 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.980685 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/__init__.py
+-rw-rw-rw-   0        0        0    24701 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/appdirs.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.988692 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/importlib_resources/
+-rw-rw-rw-   0        0        0      506 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-rw-rw-   0        0        0     4504 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-rw-rw-   0        0        0     2741 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-rw-rw-   0        0        0     2706 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-rw-rw-   0        0        0      884 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-rw-rw-   0        0        0     3494 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-rw-rw-   0        0        0     3886 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-rw-rw-   0        0        0     3566 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-rw-rw-   0        0        0     2836 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/importlib_resources/simple.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.991694 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/jaraco/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/jaraco/__init__.py
+-rw-rw-rw-   0        0        0     5420 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/jaraco/context.py
+-rw-rw-rw-   0        0        0    13515 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/jaraco/functools.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.992695 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/jaraco/text/
+-rw-rw-rw-   0        0        0    15526 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/jaraco/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:04.995698 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/more_itertools/
+-rw-rw-rw-   0        0        0       83 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   132569 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/more_itertools/more.py
+-rw-rw-rw-   0        0        0    18410 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/more_itertools/recipes.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.006707 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8496 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4706 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.016716 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9159 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6426 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   213310 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.017717 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    23668 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9023 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    39129 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25341 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13402 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10787 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/pyparsing/util.py
+-rw-rw-rw-   0        0        0     8425 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/_vendor/zipp.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.018718 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/extern/
+-rw-rw-rw-   0        0        0     2426 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pkg_resources/extern/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.024723 columbia-discord-bot-0.2.1/docs/_build/html/_static/pluggy/
+-rw-rw-rw-   0        0        0      489 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pluggy/__init__.py
+-rw-rw-rw-   0        0        0     2097 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pluggy/_callers.py
+-rw-rw-rw-   0        0        0    11496 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pluggy/_hooks.py
+-rw-rw-rw-   0        0        0    14752 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pluggy/_manager.py
+-rw-rw-rw-   0        0        0     1535 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pluggy/_result.py
+-rw-rw-rw-   0        0        0     1541 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pluggy/_tracing.py
+-rw-rw-rw-   0        0        0      142 2023-04-26 20:40:19.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pluggy/_version.py
+-rw-rw-rw-   0        0        0      263 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/py.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.040738 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/
+-rw-rw-rw-   0        0        0     2959 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/__init__.py
+-rw-rw-rw-   0        0        0      348 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/__main__.py
+-rw-rw-rw-   0        0        0    23530 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/cmdline.py
+-rw-rw-rw-   0        0        0     1697 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/console.py
+-rw-rw-rw-   0        0        0     1938 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/filter.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.041739 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/filters/
+-rw-rw-rw-   0        0        0    40338 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/filters/__init__.py
+-rw-rw-rw-   0        0        0     4154 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/formatter.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.055752 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/formatters/
+-rw-rw-rw-   0        0        0     5388 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/formatters/__init__.py
+-rw-rw-rw-   0        0        0     4176 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/formatters/_mapping.py
+-rw-rw-rw-   0        0        0     3290 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/formatters/bbcode.py
+-rw-rw-rw-   0        0        0     5070 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/formatters/groff.py
+-rw-rw-rw-   0        0        0    35574 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/formatters/html.py
+-rw-rw-rw-   0        0        0    21914 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/formatters/img.py
+-rw-rw-rw-   0        0        0     4945 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/formatters/irc.py
+-rw-rw-rw-   0        0        0    19303 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/formatters/latex.py
+-rw-rw-rw-   0        0        0     5025 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/formatters/other.py
+-rw-rw-rw-   0        0        0     2200 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/formatters/pangomarkup.py
+-rw-rw-rw-   0        0        0     4990 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/formatters/rtf.py
+-rw-rw-rw-   0        0        0     7299 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/formatters/svg.py
+-rw-rw-rw-   0        0        0     4626 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/formatters/terminal.py
+-rw-rw-rw-   0        0        0    11717 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/formatters/terminal256.py
+-rw-rw-rw-   0        0        0    34541 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.291967 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/
+-rw-rw-rw-   0        0        0    12082 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/__init__.py
+-rw-rw-rw-   0        0        0     1543 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_ada_builtins.py
+-rw-rw-rw-   0        0        0    27287 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_asy_builtins.py
+-rw-rw-rw-   0        0        0    13994 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_cl_builtins.py
+-rw-rw-rw-   0        0        0   105182 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_cocoa_builtins.py
+-rw-rw-rw-   0        0        0    18414 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_csound_builtins.py
+-rw-rw-rw-   0        0        0    12446 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_css_builtins.py
+-rw-rw-rw-   0        0        0    11883 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_julia_builtins.py
+-rw-rw-rw-   0        0        0   134510 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_lasso_builtins.py
+-rw-rw-rw-   0        0        0   108094 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_lilypond_builtins.py
+-rw-rw-rw-   0        0        0     8116 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_lua_builtins.py
+-rw-rw-rw-   0        0        0    65633 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_mapping.py
+-rw-rw-rw-   0        0        0    24713 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_mql_builtins.py
+-rw-rw-rw-   0        0        0    25842 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_mysql_builtins.py
+-rw-rw-rw-   0        0        0    49398 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_openedge_builtins.py
+-rw-rw-rw-   0        0        0   107930 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_php_builtins.py
+-rw-rw-rw-   0        0        0    13355 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_postgres_builtins.py
+-rw-rw-rw-   0        0        0    12595 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_qlik_builtins.py
+-rw-rw-rw-   0        0        0    32564 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_scheme_builtins.py
+-rw-rw-rw-   0        0        0    52413 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_scilab_builtins.py
+-rw-rw-rw-   0        0        0    26781 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_sourcemod_builtins.py
+-rw-rw-rw-   0        0        0    13445 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_stan_builtins.py
+-rw-rw-rw-   0        0        0    27227 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_stata_builtins.py
+-rw-rw-rw-   0        0        0    15460 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_tsql_builtins.py
+-rw-rw-rw-   0        0        0     1658 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_usd_builtins.py
+-rw-rw-rw-   0        0        0     4225 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_vbscript_builtins.py
+-rw-rw-rw-   0        0        0    57066 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/_vim_builtins.py
+-rw-rw-rw-   0        0        0    11676 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/actionscript.py
+-rw-rw-rw-   0        0        0     5320 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/ada.py
+-rw-rw-rw-   0        0        0      876 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/agile.py
+-rw-rw-rw-   0        0        0     9873 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/algebra.py
+-rw-rw-rw-   0        0        0     2606 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/ambient.py
+-rw-rw-rw-   0        0        0     1670 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/amdgpu.py
+-rw-rw-rw-   0        0        0     4177 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/ampl.py
+-rw-rw-rw-   0        0        0    30766 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/apdlexer.py
+-rw-rw-rw-   0        0        0     3405 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/apl.py
+-rw-rw-rw-   0        0        0    11469 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/archetype.py
+-rw-rw-rw-   0        0        0     3565 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/arrow.py
+-rw-rw-rw-   0        0        0    11417 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/arturo.py
+-rw-rw-rw-   0        0        0     1621 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/asc.py
+-rw-rw-rw-   0        0        0    41243 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/asm.py
+-rw-rw-rw-   0        0        0    19815 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/automation.py
+-rw-rw-rw-   0        0        0     3021 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/bare.py
+-rw-rw-rw-   0        0        0    27923 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/basic.py
+-rw-rw-rw-   0        0        0     1652 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/bdd.py
+-rw-rw-rw-   0        0        0     3211 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/berry.py
+-rw-rw-rw-   0        0        0     4723 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/bibtex.py
+-rw-rw-rw-   0        0        0     3915 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/boa.py
+-rw-rw-rw-   0        0        0    28112 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/business.py
+-rw-rw-rw-   0        0        0    17791 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/c_cpp.py
+-rw-rw-rw-   0        0        0    29206 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/c_like.py
+-rw-rw-rw-   0        0        0     2175 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/capnproto.py
+-rw-rw-rw-   0        0        0     3231 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/carbon.py
+-rw-rw-rw-   0        0        0     5182 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/cddl.py
+-rw-rw-rw-   0        0        0     5157 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/chapel.py
+-rw-rw-rw-   0        0        0     6395 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/clean.py
+-rw-rw-rw-   0        0        0     3156 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/comal.py
+-rw-rw-rw-   0        0        0     1407 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/compiled.py
+-rw-rw-rw-   0        0        0    42338 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/configs.py
+-rw-rw-rw-   0        0        0     4148 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/console.py
+-rw-rw-rw-   0        0        0     1390 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/cplint.py
+-rw-rw-rw-   0        0        0    15756 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/crystal.py
+-rw-rw-rw-   0        0        0    16994 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/csound.py
+-rw-rw-rw-   0        0        0    25322 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/css.py
+-rw-rw-rw-   0        0        0     9875 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/d.py
+-rw-rw-rw-   0        0        0     4607 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/dalvik.py
+-rw-rw-rw-   0        0        0    26940 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/data.py
+-rw-rw-rw-   0        0        0     8099 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/dax.py
+-rw-rw-rw-   0        0        0     4020 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/devicetree.py
+-rw-rw-rw-   0        0        0     5278 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/diff.py
+-rw-rw-rw-   0        0        0    37623 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/dotnet.py
+-rw-rw-rw-   0        0        0    36774 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/dsls.py
+-rw-rw-rw-   0        0        0    10380 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/dylan.py
+-rw-rw-rw-   0        0        0     6372 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/ecl.py
+-rw-rw-rw-   0        0        0     2690 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/eiffel.py
+-rw-rw-rw-   0        0        0     3152 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/elm.py
+-rw-rw-rw-   0        0        0     6370 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/elpi.py
+-rw-rw-rw-   0        0        0     4742 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/email.py
+-rw-rw-rw-   0        0        0    19170 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/erlang.py
+-rw-rw-rw-   0        0        0    10396 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/esoteric.py
+-rw-rw-rw-   0        0        0     3273 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/ezhil.py
+-rw-rw-rw-   0        0        0    19531 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/factor.py
+-rw-rw-rw-   0        0        0    10197 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/fantom.py
+-rw-rw-rw-   0        0        0     9646 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/felix.py
+-rw-rw-rw-   0        0        0     1621 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/fift.py
+-rw-rw-rw-   0        0        0     2668 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/floscript.py
+-rw-rw-rw-   0        0        0     7194 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/forth.py
+-rw-rw-rw-   0        0        0    10336 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/fortran.py
+-rw-rw-rw-   0        0        0    26212 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/foxpro.py
+-rw-rw-rw-   0        0        0    26914 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/freefem.py
+-rw-rw-rw-   0        0        0     3622 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/func.py
+-rw-rw-rw-   0        0        0      674 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/functional.py
+-rw-rw-rw-   0        0        0     3732 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/futhark.py
+-rw-rw-rw-   0        0        0      826 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/gcodelexer.py
+-rw-rw-rw-   0        0        0     7543 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/gdscript.py
+-rw-rw-rw-   0        0        0     3761 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/go.py
+-rw-rw-rw-   0        0        0     7980 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/grammar_notation.py
+-rw-rw-rw-   0        0        0     3861 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/graph.py
+-rw-rw-rw-   0        0        0    39026 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/graphics.py
+-rw-rw-rw-   0        0        0     1935 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/graphviz.py
+-rw-rw-rw-   0        0        0     3991 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/gsql.py
+-rw-rw-rw-   0        0        0    32898 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/haskell.py
+-rw-rw-rw-   0        0        0    30976 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/haxe.py
+-rw-rw-rw-   0        0        0    22520 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/hdl.py
+-rw-rw-rw-   0        0        0     3603 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/hexdump.py
+-rw-rw-rw-   0        0        0    19879 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/html.py
+-rw-rw-rw-   0        0        0    15450 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/idl.py
+-rw-rw-rw-   0        0        0    30631 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/igor.py
+-rw-rw-rw-   0        0        0     3136 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/inferno.py
+-rw-rw-rw-   0        0        0    13178 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/installers.py
+-rw-rw-rw-   0        0        0    57119 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/int_fiction.py
+-rw-rw-rw-   0        0        0     1906 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/iolang.py
+-rw-rw-rw-   0        0        0     4854 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/j.py
+-rw-rw-rw-   0        0        0    62859 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/javascript.py
+-rw-rw-rw-   0        0        0     2059 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/jmespath.py
+-rw-rw-rw-   0        0        0     3701 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/jslt.py
+-rw-rw-rw-   0        0        0     5635 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/jsonnet.py
+-rw-rw-rw-   0        0        0    11646 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/julia.py
+-rw-rw-rw-   0        0        0    72929 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/jvm.py
+-rw-rw-rw-   0        0        0    11406 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/kuin.py
+-rw-rw-rw-   0        0        0     9753 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/lilypond.py
+-rw-rw-rw-   0        0        0   144039 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/lisp.py
+-rw-rw-rw-   0        0        0    31914 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/macaulay2.py
+-rw-rw-rw-   0        0        0     7618 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/make.py
+-rw-rw-rw-   0        0        0    58129 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/markup.py
+-rw-rw-rw-   0        0        0      676 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/math.py
+-rw-rw-rw-   0        0        0   132852 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/matlab.py
+-rw-rw-rw-   0        0        0     2716 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/maxima.py
+-rw-rw-rw-   0        0        0     4337 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/meson.py
+-rw-rw-rw-   0        0        0     7538 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/mime.py
+-rw-rw-rw-   0        0        0    13846 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/minecraft.py
+-rw-rw-rw-   0        0        0     4604 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/mips.py
+-rw-rw-rw-   0        0        0    35324 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/ml.py
+-rw-rw-rw-   0        0        0    13524 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/modeling.py
+-rw-rw-rw-   0        0        0    53073 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/modula2.py
+-rw-rw-rw-   0        0        0     6290 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/monte.py
+-rw-rw-rw-   0        0        0     9187 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/mosel.py
+-rw-rw-rw-   0        0        0    63962 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/ncl.py
+-rw-rw-rw-   0        0        0     6416 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/nimrod.py
+-rw-rw-rw-   0        0        0     2726 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/nit.py
+-rw-rw-rw-   0        0        0     4015 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/nix.py
+-rw-rw-rw-   0        0        0     4169 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/oberon.py
+-rw-rw-rw-   0        0        0    22961 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/objective.py
+-rw-rw-rw-   0        0        0     2982 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/ooc.py
+-rw-rw-rw-   0        0        0     1744 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/other.py
+-rw-rw-rw-   0        0        0     2720 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/parasail.py
+-rw-rw-rw-   0        0        0    25904 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/parsers.py
+-rw-rw-rw-   0        0        0    30880 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/pascal.py
+-rw-rw-rw-   0        0        0     8146 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/pawn.py
+-rw-rw-rw-   0        0        0    39170 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/perl.py
+-rw-rw-rw-   0        0        0    23252 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/phix.py
+-rw-rw-rw-   0        0        0    13040 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/php.py
+-rw-rw-rw-   0        0        0     1975 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/pointless.py
+-rw-rw-rw-   0        0        0     3244 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/pony.py
+-rw-rw-rw-   0        0        0    12677 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/praat.py
+-rw-rw-rw-   0        0        0     1156 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/procfile.py
+-rw-rw-rw-   0        0        0    12351 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/prolog.py
+-rw-rw-rw-   0        0        0     4715 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/promql.py
+-rw-rw-rw-   0        0        0    53376 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/python.py
+-rw-rw-rw-   0        0        0     6932 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/q.py
+-rw-rw-rw-   0        0        0     3665 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/qlik.py
+-rw-rw-rw-   0        0        0     6072 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/qvt.py
+-rw-rw-rw-   0        0        0     6185 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/r.py
+-rw-rw-rw-   0        0        0    15790 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/rdf.py
+-rw-rw-rw-   0        0        0    18248 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/rebol.py
+-rw-rw-rw-   0        0        0     2902 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/resource.py
+-rw-rw-rw-   0        0        0     5056 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/ride.py
+-rw-rw-rw-   0        0        0     1128 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/rita.py
+-rw-rw-rw-   0        0        0     1973 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/rnc.py
+-rw-rw-rw-   0        0        0     1962 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/roboconf.py
+-rw-rw-rw-   0        0        0    18449 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/robotframework.py
+-rw-rw-rw-   0        0        0    22775 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/ruby.py
+-rw-rw-rw-   0        0        0     8216 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/rust.py
+-rw-rw-rw-   0        0        0     9400 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/sas.py
+-rw-rw-rw-   0        0        0     4645 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/savi.py
+-rw-rw-rw-   0        0        0     2239 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/scdoc.py
+-rw-rw-rw-   0        0        0    70014 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/scripting.py
+-rw-rw-rw-   0        0        0     1986 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/sgf.py
+-rw-rw-rw-   0        0        0    36466 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/shell.py
+-rw-rw-rw-   0        0        0     2441 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/sieve.py
+-rw-rw-rw-   0        0        0     8482 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/slash.py
+-rw-rw-rw-   0        0        0     7206 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/smalltalk.py
+-rw-rw-rw-   0        0        0     2660 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/smithy.py
+-rw-rw-rw-   0        0        0     2773 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/smv.py
+-rw-rw-rw-   0        0        0     2732 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/snobol.py
+-rw-rw-rw-   0        0        0     3127 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/solidity.py
+-rw-rw-rw-   0        0        0     3330 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/sophia.py
+-rw-rw-rw-   0        0        0     3414 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/special.py
+-rw-rw-rw-   0        0        0     2733 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/spice.py
+-rw-rw-rw-   0        0        0    42086 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/sql.py
+-rw-rw-rw-   0        0        0     1693 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/srcinfo.py
+-rw-rw-rw-   0        0        0     6416 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/stata.py
+-rw-rw-rw-   0        0        0     3698 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/supercollider.py
+-rw-rw-rw-   0        0        0     2639 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/tal.py
+-rw-rw-rw-   0        0        0     5513 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/tcl.py
+-rw-rw-rw-   0        0        0     3523 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/teal.py
+-rw-rw-rw-   0        0        0    72610 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/templates.py
+-rw-rw-rw-   0        0        0     9719 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/teraterm.py
+-rw-rw-rw-   0        0        0    10767 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/testing.py
+-rw-rw-rw-   0        0        0     1029 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/text.py
+-rw-rw-rw-   0        0        0     7609 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/textedit.py
+-rw-rw-rw-   0        0        0    15192 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/textfmts.py
+-rw-rw-rw-   0        0        0    20157 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/theorem.py
+-rw-rw-rw-   0        0        0     4228 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/thingsdb.py
+-rw-rw-rw-   0        0        0     1377 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/tlb.py
+-rw-rw-rw-   0        0        0    10457 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/tnt.py
+-rw-rw-rw-   0        0        0     1474 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/trafficscript.py
+-rw-rw-rw-   0        0        0     8207 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/typoscript.py
+-rw-rw-rw-   0        0        0     8956 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/ul4.py
+-rw-rw-rw-   0        0        0    18512 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/unicon.py
+-rw-rw-rw-   0        0        0     6037 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/urbi.py
+-rw-rw-rw-   0        0        0     3513 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/usd.py
+-rw-rw-rw-   0        0        0     7273 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/varnish.py
+-rw-rw-rw-   0        0        0     3885 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/verification.py
+-rw-rw-rw-   0        0        0      894 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/web.py
+-rw-rw-rw-   0        0        0     5699 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/webassembly.py
+-rw-rw-rw-   0        0        0    10517 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/webidl.py
+-rw-rw-rw-   0        0        0    40549 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/webmisc.py
+-rw-rw-rw-   0        0        0    11920 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/wgsl.py
+-rw-rw-rw-   0        0        0     4018 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/whiley.py
+-rw-rw-rw-   0        0        0     4021 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/wowtoc.py
+-rw-rw-rw-   0        0        0     3239 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/wren.py
+-rw-rw-rw-   0        0        0     1920 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/x10.py
+-rw-rw-rw-   0        0        0      902 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/xorg.py
+-rw-rw-rw-   0        0        0     4500 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/yang.py
+-rw-rw-rw-   0        0        0     3953 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/lexers/zig.py
+-rw-rw-rw-   0        0        0      986 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/modeline.py
+-rw-rw-rw-   0        0        0     2579 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/plugin.py
+-rw-rw-rw-   0        0        0     3072 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/regexopt.py
+-rw-rw-rw-   0        0        0     3092 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/scanner.py
+-rw-rw-rw-   0        0        0     6816 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/sphinxext.py
+-rw-rw-rw-   0        0        0     6245 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/style.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.338008 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/
+-rw-rw-rw-   0        0        0     3676 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/__init__.py
+-rw-rw-rw-   0        0        0      705 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/abap.py
+-rw-rw-rw-   0        0        0     2216 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/algol.py
+-rw-rw-rw-   0        0        0     2231 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/algol_nu.py
+-rw-rw-rw-   0        0        0     4443 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/arduino.py
+-rw-rw-rw-   0        0        0     2096 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/autumn.py
+-rw-rw-rw-   0        0        0     1514 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/borland.py
+-rw-rw-rw-   0        0        0     1308 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/bw.py
+-rw-rw-rw-   0        0        0     2730 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/colorful.py
+-rw-rw-rw-   0        0        0     2488 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/default.py
+-rw-rw-rw-   0        0        0     3314 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/dracula.py
+-rw-rw-rw-   0        0        0     2439 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/emacs.py
+-rw-rw-rw-   0        0        0     2502 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/friendly.py
+-rw-rw-rw-   0        0        0     2707 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/friendly_grayscale.py
+-rw-rw-rw-   0        0        0     1274 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/fruity.py
+-rw-rw-rw-   0        0        0     3481 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/gh_dark.py
+-rw-rw-rw-   0        0        0     3230 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/gruvbox.py
+-rw-rw-rw-   0        0        0      692 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/igor.py
+-rw-rw-rw-   0        0        0     2302 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/inkpot.py
+-rw-rw-rw-   0        0        0     2016 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/lilypond.py
+-rw-rw-rw-   0        0        0     3117 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/lovelace.py
+-rw-rw-rw-   0        0        0     2350 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/manni.py
+-rw-rw-rw-   0        0        0     4083 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/material.py
+-rw-rw-rw-   0        0        0     5063 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/monokai.py
+-rw-rw-rw-   0        0        0     2703 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/murphy.py
+-rw-rw-rw-   0        0        0     1948 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/native.py
+-rw-rw-rw-   0        0        0     5244 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/nord.py
+-rw-rw-rw-   0        0        0     1664 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/onedark.py
+-rw-rw-rw-   0        0        0     5526 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/paraiso_dark.py
+-rw-rw-rw-   0        0        0     5530 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/paraiso_light.py
+-rw-rw-rw-   0        0        0     2425 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/pastie.py
+-rw-rw-rw-   0        0        0     2128 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/perldoc.py
+-rw-rw-rw-   0        0        0     2432 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/rainbow_dash.py
+-rw-rw-rw-   0        0        0      874 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/rrt.py
+-rw-rw-rw-   0        0        0     1393 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/sas.py
+-rw-rw-rw-   0        0        0     4078 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/solarized.py
+-rw-rw-rw-   0        0        0      770 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/staroffice.py
+-rw-rw-rw-   0        0        0     1198 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/stata_dark.py
+-rw-rw-rw-   0        0        0     1227 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/stata_light.py
+-rw-rw-rw-   0        0        0     7039 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/tango.py
+-rw-rw-rw-   0        0        0     1885 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/trac.py
+-rw-rw-rw-   0        0        0     1922 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/vim.py
+-rw-rw-rw-   0        0        0     1026 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/vs.py
+-rw-rw-rw-   0        0        0     1453 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/xcode.py
+-rw-rw-rw-   0        0        0     2148 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/styles/zenburn.py
+-rw-rw-rw-   0        0        0     6184 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/token.py
+-rw-rw-rw-   0        0        0    63223 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/unistring.py
+-rw-rw-rw-   0        0        0    10230 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pygments/util.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.340011 columbia-discord-bot-0.2.1/docs/_build/html/_static/pytest/
+-rw-rw-rw-   0        0        0     5163 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pytest/__init__.py
+-rw-rw-rw-   0        0        0      116 2023-04-26 20:40:20.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/pytest/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.345015 columbia-discord-bot-0.2.1/docs/_build/html/_static/recommonmark/
+-rw-rw-rw-   0        0        0      468 2023-05-05 00:52:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/recommonmark/__init__.py
+-rw-rw-rw-   0        0        0    10145 2023-05-05 00:52:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/recommonmark/parser.py
+-rw-rw-rw-   0        0        0     1856 2023-05-05 00:52:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/recommonmark/scripts.py
+-rw-rw-rw-   0        0        0     4624 2023-05-05 00:52:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/recommonmark/states.py
+-rw-rw-rw-   0        0        0    11945 2023-05-05 00:52:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/recommonmark/transform.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.362031 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/
+-rw-rw-rw-   0        0        0     4972 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/__version__.py
+-rw-rw-rw-   0        0        0     1495 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/_internal_utils.py
+-rw-rw-rw-   0        0        0    19578 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/adapters.py
+-rw-rw-rw-   0        0        0     6449 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/api.py
+-rw-rw-rw-   0        0        0    10187 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/auth.py
+-rw-rw-rw-   0        0        0      429 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/certs.py
+-rw-rw-rw-   0        0        0     1451 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/compat.py
+-rw-rw-rw-   0        0        0    18560 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/cookies.py
+-rw-rw-rw-   0        0        0     3811 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/exceptions.py
+-rw-rw-rw-   0        0        0     3875 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/help.py
+-rw-rw-rw-   0        0        0      733 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/hooks.py
+-rw-rw-rw-   0        0        0    35223 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/models.py
+-rw-rw-rw-   0        0        0      957 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/packages.py
+-rw-rw-rw-   0        0        0    30180 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/sessions.py
+-rw-rw-rw-   0        0        0     4235 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/status_codes.py
+-rw-rw-rw-   0        0        0     2912 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/structures.py
+-rw-rw-rw-   0        0        0    33448 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/requests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.392058 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/
+-rw-rw-rw-   0        0        0     8429 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/__init__.py
+-rw-rw-rw-   0        0        0      218 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_deprecation_warning.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.425087 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/
+-rw-rw-rw-   0        0        0      537 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/__init__.py
+-rw-rw-rw-   0        0        0     1330 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/_collections.py
+-rw-rw-rw-   0        0        0      411 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/_functools.py
+-rw-rw-rw-   0        0        0      239 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/_macos_compat.py
+-rw-rw-rw-   0        0        0    19672 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/_msvccompiler.py
+-rw-rw-rw-   0        0        0     8603 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/archive_util.py
+-rw-rw-rw-   0        0        0    14789 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/bcppcompiler.py
+-rw-rw-rw-   0        0        0    47369 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/ccompiler.py
+-rw-rw-rw-   0        0        0    17973 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/cmd.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.448108 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/
+-rw-rw-rw-   0        0        0      430 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/__init__.py
+-rw-rw-rw-   0        0        0     1614 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/_framework_compat.py
+-rw-rw-rw-   0        0        0     5441 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/bdist.py
+-rw-rw-rw-   0        0        0     4701 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/bdist_dumb.py
+-rw-rw-rw-   0        0        0    22051 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0     5617 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/build.py
+-rw-rw-rw-   0        0        0     7728 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/build_clib.py
+-rw-rw-rw-   0        0        0    31558 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/build_ext.py
+-rw-rw-rw-   0        0        0    16568 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/build_py.py
+-rw-rw-rw-   0        0        0     5624 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/build_scripts.py
+-rw-rw-rw-   0        0        0     4888 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/check.py
+-rw-rw-rw-   0        0        0     2603 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/clean.py
+-rw-rw-rw-   0        0        0    13137 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/config.py
+-rw-rw-rw-   0        0        0    30221 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/install.py
+-rw-rw-rw-   0        0        0     2779 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/install_data.py
+-rw-rw-rw-   0        0        0     2785 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     1189 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/install_headers.py
+-rw-rw-rw-   0        0        0     8434 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/install_lib.py
+-rw-rw-rw-   0        0        0     1936 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/install_scripts.py
+-rw-rw-rw-   0        0        0      672 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/py37compat.py
+-rw-rw-rw-   0        0        0    11765 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/register.py
+-rw-rw-rw-   0        0        0    19241 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/sdist.py
+-rw-rw-rw-   0        0        0     7477 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/command/upload.py
+-rw-rw-rw-   0        0        0     4920 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/config.py
+-rw-rw-rw-   0        0        0     9451 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/core.py
+-rw-rw-rw-   0        0        0    12537 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/cygwinccompiler.py
+-rw-rw-rw-   0        0        0      139 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/debug.py
+-rw-rw-rw-   0        0        0     3423 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/dep_util.py
+-rw-rw-rw-   0        0        0     8082 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/dir_util.py
+-rw-rw-rw-   0        0        0    50186 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/dist.py
+-rw-rw-rw-   0        0        0     3589 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/errors.py
+-rw-rw-rw-   0        0        0    10270 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/extension.py
+-rw-rw-rw-   0        0        0    17910 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/fancy_getopt.py
+-rw-rw-rw-   0        0        0     8226 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/file_util.py
+-rw-rw-rw-   0        0        0    13713 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/filelist.py
+-rw-rw-rw-   0        0        0     1972 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/log.py
+-rw-rw-rw-   0        0        0    30235 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/msvc9compiler.py
+-rw-rw-rw-   0        0        0    23602 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/msvccompiler.py
+-rw-rw-rw-   0        0        0      217 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/py38compat.py
+-rw-rw-rw-   0        0        0      639 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/py39compat.py
+-rw-rw-rw-   0        0        0     3517 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/spawn.py
+-rw-rw-rw-   0        0        0    18858 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/sysconfig.py
+-rw-rw-rw-   0        0        0    12096 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/text_file.py
+-rw-rw-rw-   0        0        0    15641 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/unixccompiler.py
+-rw-rw-rw-   0        0        0    18128 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/util.py
+-rw-rw-rw-   0        0        0    12952 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/version.py
+-rw-rw-rw-   0        0        0     5248 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_distutils/versionpredicate.py
+-rw-rw-rw-   0        0        0     1972 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_entry_points.py
+-rw-rw-rw-   0        0        0     2392 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_imp.py
+-rw-rw-rw-   0        0        0     1311 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_importlib.py
+-rw-rw-rw-   0        0        0      675 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_itertools.py
+-rw-rw-rw-   0        0        0      749 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_path.py
+-rw-rw-rw-   0        0        0      501 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_reqs.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.452113 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.459118 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_metadata/
+-rw-rw-rw-   0        0        0    30130 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-rw-rw-   0        0        0     1862 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-rw-rw-   0        0        0      743 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-rw-rw-   0        0        0     1828 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-rw-rw-   0        0        0     2895 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-rw-rw-   0        0        0     2068 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-rw-rw-   0        0        0     1154 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-rw-rw-   0        0        0     2166 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_metadata/_text.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.467126 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_resources/
+-rw-rw-rw-   0        0        0      506 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_resources/__init__.py
+-rw-rw-rw-   0        0        0     4504 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-rw-rw-   0        0        0     2741 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_resources/_common.py
+-rw-rw-rw-   0        0        0     2706 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_resources/_compat.py
+-rw-rw-rw-   0        0        0      884 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-rw-rw-   0        0        0     3494 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-rw-rw-   0        0        0     3886 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_resources/abc.py
+-rw-rw-rw-   0        0        0     3566 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_resources/readers.py
+-rw-rw-rw-   0        0        0     2836 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/importlib_resources/simple.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.470129 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/jaraco/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/jaraco/__init__.py
+-rw-rw-rw-   0        0        0     5420 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/jaraco/context.py
+-rw-rw-rw-   0        0        0    13512 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/jaraco/functools.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.471129 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/jaraco/text/
+-rw-rw-rw-   0        0        0    15517 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/jaraco/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.474133 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/more_itertools/
+-rw-rw-rw-   0        0        0       82 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   117959 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/more_itertools/more.py
+-rw-rw-rw-   0        0        0    16256 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/more_itertools/recipes.py
+-rw-rw-rw-   0        0        0    15130 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/ordered_set.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.484141 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8493 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4700 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.494150 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9159 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6426 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   213310 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.495150 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    23668 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9023 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    39129 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25341 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13402 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10787 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/pyparsing/util.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.499155 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/tomli/
+-rw-rw-rw-   0        0        0      396 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/tomli/__init__.py
+-rw-rw-rw-   0        0        0    22633 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2943 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/tomli/_re.py
+-rw-rw-rw-   0        0        0      254 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/tomli/_types.py
+-rw-rw-rw-   0        0        0    87149 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/typing_extensions.py
+-rw-rw-rw-   0        0        0     8425 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/_vendor/zipp.py
+-rw-rw-rw-   0        0        0     7346 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/archive_util.py
+-rw-rw-rw-   0        0        0    19539 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/build_meta.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.523177 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/
+-rw-rw-rw-   0        0        0      396 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/__init__.py
+-rw-rw-rw-   0        0        0     2381 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/alias.py
+-rw-rw-rw-   0        0        0    16623 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/bdist_egg.py
+-rw-rw-rw-   0        0        0     1182 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0     6595 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/build.py
+-rw-rw-rw-   0        0        0     4415 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/build_clib.py
+-rw-rw-rw-   0        0        0    15821 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/build_ext.py
+-rw-rw-rw-   0        0        0    14115 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/build_py.py
+-rw-rw-rw-   0        0        0     7012 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/develop.py
+-rw-rw-rw-   0        0        0     4800 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/dist_info.py
+-rw-rw-rw-   0        0        0    85662 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/easy_install.py
+-rw-rw-rw-   0        0        0    31188 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/editable_wheel.py
+-rw-rw-rw-   0        0        0    26795 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/egg_info.py
+-rw-rw-rw-   0        0        0     5163 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/install.py
+-rw-rw-rw-   0        0        0     2226 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     3875 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/install_lib.py
+-rw-rw-rw-   0        0        0     2612 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/install_scripts.py
+-rw-rw-rw-   0        0        0     4946 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/py36compat.py
+-rw-rw-rw-   0        0        0      468 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/register.py
+-rw-rw-rw-   0        0        0     2128 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/rotate.py
+-rw-rw-rw-   0        0        0      658 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/saveopts.py
+-rw-rw-rw-   0        0        0     7071 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/sdist.py
+-rw-rw-rw-   0        0        0     5086 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/setopt.py
+-rw-rw-rw-   0        0        0     8102 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/test.py
+-rw-rw-rw-   0        0        0      462 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/upload.py
+-rw-rw-rw-   0        0        0     7494 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/command/upload_docs.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.527181 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/config/
+-rw-rw-rw-   0        0        0     1121 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/config/__init__.py
+-rw-rw-rw-   0        0        0    13398 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/config/_apply_pyprojecttoml.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.533185 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/config/_validate_pyproject/
+-rw-rw-rw-   0        0        0     1038 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/config/_validate_pyproject/__init__.py
+-rw-rw-rw-   0        0        0    11266 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-rw-rw-   0        0        0     1153 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-rw-rw-   0        0        0     1612 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-rw-rw-   0        0        0   269900 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-rw-rw-   0        0        0     8736 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/config/_validate_pyproject/formats.py
+-rw-rw-rw-   0        0        0    16319 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/config/expand.py
+-rw-rw-rw-   0        0        0    19304 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/config/pyprojecttoml.py
+-rw-rw-rw-   0        0        0    25198 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/config/setupcfg.py
+-rw-rw-rw-   0        0        0      949 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/dep_util.py
+-rw-rw-rw-   0        0        0     5499 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/depends.py
+-rw-rw-rw-   0        0        0    20799 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/discovery.py
+-rw-rw-rw-   0        0        0    45578 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/dist.py
+-rw-rw-rw-   0        0        0     2464 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/errors.py
+-rw-rw-rw-   0        0        0     5591 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/extension.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.534186 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/extern/
+-rw-rw-rw-   0        0        0     2512 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/extern/__init__.py
+-rw-rw-rw-   0        0        0     4873 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/glob.py
+-rw-rw-rw-   0        0        0     3824 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/installer.py
+-rw-rw-rw-   0        0        0      812 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/launch.py
+-rw-rw-rw-   0        0        0     1210 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/logging.py
+-rw-rw-rw-   0        0        0     4857 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/monkey.py
+-rw-rw-rw-   0        0        0    47724 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/msvc.py
+-rw-rw-rw-   0        0        0     3093 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/namespaces.py
+-rw-rw-rw-   0        0        0    40020 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/package_index.py
+-rw-rw-rw-   0        0        0      245 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/py34compat.py
+-rw-rw-rw-   0        0        0    14348 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/sandbox.py
+-rw-rw-rw-   0        0        0      941 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/unicode_utils.py
+-rw-rw-rw-   0        0        0      144 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/version.py
+-rw-rw-rw-   0        0        0     8376 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/wheel.py
+-rw-rw-rw-   0        0        0      718 2023-04-26 20:28:25.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/setuptools/windows_support.py
+-rw-rw-rw-   0        0        0    34549 2023-04-26 20:40:23.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/six.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.566216 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/
+-rw-rw-rw-   0        0        0     2677 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/__init__.py
+-rw-rw-rw-   0        0        0      404 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/among.py
+-rw-rw-rw-   0        0        0    40812 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/arabic_stemmer.py
+-rw-rw-rw-   0        0        0    12393 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/armenian_stemmer.py
+-rw-rw-rw-   0        0        0     9418 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/basestemmer.py
+-rw-rw-rw-   0        0        0    20778 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/basque_stemmer.py
+-rw-rw-rw-   0        0        0    24572 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/catalan_stemmer.py
+-rw-rw-rw-   0        0        0     6329 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/danish_stemmer.py
+-rw-rw-rw-   0        0        0    14388 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/dutch_stemmer.py
+-rw-rw-rw-   0        0        0    22303 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/english_stemmer.py
+-rw-rw-rw-   0        0        0    16228 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/finnish_stemmer.py
+-rw-rw-rw-   0        0        0    32591 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/french_stemmer.py
+-rw-rw-rw-   0        0        0    12988 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/german_stemmer.py
+-rw-rw-rw-   0        0        0    85974 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/greek_stemmer.py
+-rw-rw-rw-   0        0        0     7514 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/hindi_stemmer.py
+-rw-rw-rw-   0        0        0    14729 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/hungarian_stemmer.py
+-rw-rw-rw-   0        0        0     9182 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/indonesian_stemmer.py
+-rw-rw-rw-   0        0        0     7915 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/irish_stemmer.py
+-rw-rw-rw-   0        0        0    22739 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/italian_stemmer.py
+-rw-rw-rw-   0        0        0    14715 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/lithuanian_stemmer.py
+-rw-rw-rw-   0        0        0     9847 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/nepali_stemmer.py
+-rw-rw-rw-   0        0        0     5442 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/norwegian_stemmer.py
+-rw-rw-rw-   0        0        0    14967 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/porter_stemmer.py
+-rw-rw-rw-   0        0        0    20772 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/portuguese_stemmer.py
+-rw-rw-rw-   0        0        0    20414 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/romanian_stemmer.py
+-rw-rw-rw-   0        0        0    15270 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/russian_stemmer.py
+-rw-rw-rw-   0        0        0   123318 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/serbian_stemmer.py
+-rw-rw-rw-   0        0        0    21981 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/spanish_stemmer.py
+-rw-rw-rw-   0        0        0     5354 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/swedish_stemmer.py
+-rw-rw-rw-   0        0        0    63370 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/tamil_stemmer.py
+-rw-rw-rw-   0        0        0    61219 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/turkish_stemmer.py
+-rw-rw-rw-   0        0        0    33769 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/snowballstemmer/yiddish_stemmer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.585234 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/
+-rw-rw-rw-   0        0        0     1829 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/__main__.py
+-rw-rw-rw-   0        0        0    17579 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/addnodes.py
+-rw-rw-rw-   0        0        0    55756 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/application.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.598245 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/
+-rw-rw-rw-   0        0        0    27703 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/__init__.py
+-rw-rw-rw-   0        0        0    28999 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/_epub_base.py
+-rw-rw-rw-   0        0        0     6474 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/changes.py
+-rw-rw-rw-   0        0        0     1504 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/dirhtml.py
+-rw-rw-rw-   0        0        0      982 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/dummy.py
+-rw-rw-rw-   0        0        0    11284 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/epub3.py
+-rw-rw-rw-   0        0        0    11407 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/gettext.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.600246 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/html/
+-rw-rw-rw-   0        0        0    59207 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/html/__init__.py
+-rw-rw-rw-   0        0        0     2525 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/html/transforms.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.606251 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/latex/
+-rw-rw-rw-   0        0        0    24143 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/latex/__init__.py
+-rw-rw-rw-   0        0        0     7365 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/latex/constants.py
+-rw-rw-rw-   0        0        0      866 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/latex/nodes.py
+-rw-rw-rw-   0        0        0     4445 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/latex/theming.py
+-rw-rw-rw-   0        0        0    20998 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/latex/transforms.py
+-rw-rw-rw-   0        0        0     1703 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/latex/util.py
+-rw-rw-rw-   0        0        0    23404 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/linkcheck.py
+-rw-rw-rw-   0        0        0     4511 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/manpage.py
+-rw-rw-rw-   0        0        0     7425 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/singlehtml.py
+-rw-rw-rw-   0        0        0     9634 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/texinfo.py
+-rw-rw-rw-   0        0        0     2870 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/text.py
+-rw-rw-rw-   0        0        0     3726 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/builders/xml.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.610256 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/cmd/
+-rw-rw-rw-   0        0        0       44 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/cmd/__init__.py
+-rw-rw-rw-   0        0        0    13411 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/cmd/build.py
+-rw-rw-rw-   0        0        0     6552 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/cmd/make_mode.py
+-rw-rw-rw-   0        0        0    23835 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/cmd/quickstart.py
+-rw-rw-rw-   0        0        0    21519 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/config.py
+-rw-rw-rw-   0        0        0     1800 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/deprecation.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.614259 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/directives/
+-rw-rw-rw-   0        0        0    13518 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/directives/__init__.py
+-rw-rw-rw-   0        0        0    18354 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/directives/code.py
+-rw-rw-rw-   0        0        0    14672 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/directives/other.py
+-rw-rw-rw-   0        0        0     6781 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/directives/patches.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.625269 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/domains/
+-rw-rw-rw-   0        0        0    15320 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/domains/__init__.py
+-rw-rw-rw-   0        0        0   151003 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/domains/c.py
+-rw-rw-rw-   0        0        0     5524 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/domains/changeset.py
+-rw-rw-rw-   0        0        0     5676 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/domains/citation.py
+-rw-rw-rw-   0        0        0   329631 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/domains/cpp.py
+-rw-rw-rw-   0        0        0     4086 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/domains/index.py
+-rw-rw-rw-   0        0        0    18844 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/domains/javascript.py
+-rw-rw-rw-   0        0        0     5459 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/domains/math.py
+-rw-rw-rw-   0        0        0    60090 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/domains/python.py
+-rw-rw-rw-   0        0        0    10876 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/domains/rst.py
+-rw-rw-rw-   0        0        0    47197 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/domains/std.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.626271 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/environment/
+-rw-rw-rw-   0        0        0    29692 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/environment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.630274 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/environment/adapters/
+-rw-rw-rw-   0        0        0       34 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/environment/adapters/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/environment/adapters/asset.py
+-rw-rw-rw-   0        0        0     7509 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/environment/adapters/indexentries.py
+-rw-rw-rw-   0        0        0    16449 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/environment/adapters/toctree.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.636280 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/environment/collectors/
+-rw-rw-rw-   0        0        0     2784 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/environment/collectors/__init__.py
+-rw-rw-rw-   0        0        0     6161 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/environment/collectors/asset.py
+-rw-rw-rw-   0        0        0     1887 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/environment/collectors/dependencies.py
+-rw-rw-rw-   0        0        0     2609 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/environment/collectors/metadata.py
+-rw-rw-rw-   0        0        0     2144 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/environment/collectors/title.py
+-rw-rw-rw-   0        0        0    15869 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/environment/collectors/toctree.py
+-rw-rw-rw-   0        0        0     3388 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/errors.py
+-rw-rw-rw-   0        0        0     4230 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/events.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.653295 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/
+-rw-rw-rw-   0        0        0       57 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/__init__.py
+-rw-rw-rw-   0        0        0    19197 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/apidoc.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.660301 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/autodoc/
+-rw-rw-rw-   0        0        0   114236 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/autodoc/__init__.py
+-rw-rw-rw-   0        0        0     5925 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/autodoc/directive.py
+-rw-rw-rw-   0        0        0    11371 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/autodoc/importer.py
+-rw-rw-rw-   0        0        0     5900 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/autodoc/mock.py
+-rw-rw-rw-   0        0        0     4588 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/autodoc/preserve_defaults.py
+-rw-rw-rw-   0        0        0     5292 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/autodoc/type_comment.py
+-rw-rw-rw-   0        0        0     7789 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/autodoc/typehints.py
+-rw-rw-rw-   0        0        0     2292 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/autosectionlabel.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.662302 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/autosummary/
+-rw-rw-rw-   0        0        0    31630 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/autosummary/__init__.py
+-rw-rw-rw-   0        0        0    26212 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/autosummary/generate.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:03.931731 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/autosummary/templates/
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.665306 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/autosummary/templates/autosummary/
+-rw-rw-rw-   0        0        0      106 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/autosummary/templates/autosummary/base.rst
+-rw-rw-rw-   0        0        0      553 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/autosummary/templates/autosummary/class.rst
+-rw-rw-rw-   0        0        0     1071 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/autosummary/templates/autosummary/module.rst
+-rw-rw-rw-   0        0        0    14065 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/coverage.py
+-rw-rw-rw-   0        0        0    22423 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/doctest.py
+-rw-rw-rw-   0        0        0     2887 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/duration.py
+-rw-rw-rw-   0        0        0     4523 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/extlinks.py
+-rw-rw-rw-   0        0        0     1962 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/githubpages.py
+-rw-rw-rw-   0        0        0    15864 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/graphviz.py
+-rw-rw-rw-   0        0        0     2517 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/ifconfig.py
+-rw-rw-rw-   0        0        0     3582 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/imgconverter.py
+-rw-rw-rw-   0        0        0    15117 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/imgmath.py
+-rw-rw-rw-   0        0        0    17031 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/inheritance_diagram.py
+-rw-rw-rw-   0        0        0    28441 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/intersphinx.py
+-rw-rw-rw-   0        0        0     2203 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/linkcode.py
+-rw-rw-rw-   0        0        0     5182 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/mathjax.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.668309 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/napoleon/
+-rw-rw-rw-   0        0        0    17936 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/napoleon/__init__.py
+-rw-rw-rw-   0        0        0    48417 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/napoleon/docstring.py
+-rw-rw-rw-   0        0        0     7602 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/napoleon/iterators.py
+-rw-rw-rw-   0        0        0     8017 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/todo.py
+-rw-rw-rw-   0        0        0    12900 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/ext/viewcode.py
+-rw-rw-rw-   0        0        0     2995 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/extension.py
+-rw-rw-rw-   0        0        0     6986 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/highlighting.py
+-rw-rw-rw-   0        0        0     7844 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/io.py
+-rw-rw-rw-   0        0        0     7107 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/jinja2glue.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.669310 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/locale/
+-rw-rw-rw-   0        0        0     7316 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/locale/__init__.py
+-rw-rw-rw-   0        0        0     3098 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/parsers.py
+-rw-rw-rw-   0        0        0     3432 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/project.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.672313 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/pycode/
+-rw-rw-rw-   0        0        0     5581 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/pycode/__init__.py
+-rw-rw-rw-   0        0        0     7303 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/pycode/ast.py
+-rw-rw-rw-   0        0        0    21072 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/pycode/parser.py
+-rw-rw-rw-   0        0        0     2861 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/pygments_styles.py
+-rw-rw-rw-   0        0        0    22631 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/registry.py
+-rw-rw-rw-   0        0        0    15975 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/roles.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.689328 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/
+-rw-rw-rw-   0        0        0    23568 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/__init__.py
+-rw-rw-rw-   0        0        0     3561 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/da.py
+-rw-rw-rw-   0        0        0     4637 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/de.py
+-rw-rw-rw-   0        0        0     4899 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/en.py
+-rw-rw-rw-   0        0        0     5723 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/es.py
+-rw-rw-rw-   0        0        0     3207 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/fi.py
+-rw-rw-rw-   0        0        0     3438 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/fr.py
+-rw-rw-rw-   0        0        0     1949 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/hu.py
+-rw-rw-rw-   0        0        0     5089 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/it.py
+-rw-rw-rw-   0        0        0    31156 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/ja.py
+-rw-rw-rw-   0        0        0     4571 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/nl.py
+-rw-rw-rw-   0        0        0     4893 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/no.py
+-rw-rw-rw-   0        0        0     4648 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/pt.py
+-rw-rw-rw-   0        0        0      557 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/ro.py
+-rw-rw-rw-   0        0        0     7905 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/ru.py
+-rw-rw-rw-   0        0        0     3436 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/sv.py
+-rw-rw-rw-   0        0        0      551 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/tr.py
+-rw-rw-rw-   0        0        0     6146 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/search/zh.py
+-rw-rw-rw-   0        0        0     7123 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/setup_command.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:03.934733 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/templates/
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.691330 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/templates/apidoc/
+-rw-rw-rw-   0        0        0       18 2023-05-05 01:23:26.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/templates/apidoc/module.rst
+-rw-rw-rw-   0        0        0        0 2023-05-05 01:23:26.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/templates/apidoc/package.rst
+-rw-rw-rw-   0        0        0        0 2023-05-05 01:23:26.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/templates/apidoc/toc.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.695334 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/templates/quickstart/
+-rw-rw-rw-   0        0        0     4099 2023-05-05 01:23:26.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/templates/quickstart/Makefile
+-rw-rw-rw-   0        0        0        0 2023-05-05 01:23:26.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/templates/quickstart/conf.py
+-rwxrwxrwx   0        0        0     3373 2023-05-05 01:23:26.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/templates/quickstart/make.bat
+-rw-rw-rw-   0        0        0      451 2023-05-05 01:23:26.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/templates/quickstart/root_doc.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.695334 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/templates/texinfo/
+-rw-rw-rw-   0        0        0     1423 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/templates/texinfo/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.701338 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/testing/
+-rw-rw-rw-   0        0        0      171 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/testing/__init__.py
+-rw-rw-rw-   0        0        0     2710 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/testing/comparer.py
+-rw-rw-rw-   0        0        0     7508 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/testing/fixtures.py
+-rw-rw-rw-   0        0        0     6317 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/testing/path.py
+-rw-rw-rw-   0        0        0     1029 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/testing/restructuredtext.py
+-rw-rw-rw-   0        0        0     7297 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/testing/util.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.703340 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/texinputs/
+-rw-rw-rw-   0        0        0     1612 2023-05-05 01:23:26.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/texinputs/Makefile
+-rwxrwxrwx   0        0        0      503 2023-05-05 01:23:26.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/texinputs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.704341 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/texinputs_win/
+-rw-rw-rw-   0        0        0     2368 2023-05-05 01:23:26.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/texinputs_win/Makefile
+-rw-rw-rw-   0        0        0     7937 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/theming.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.708345 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/transforms/
+-rw-rw-rw-   0        0        0    14420 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/transforms/__init__.py
+-rw-rw-rw-   0        0        0     2768 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/transforms/compact_bullet_list.py
+-rw-rw-rw-   0        0        0    23400 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/transforms/i18n.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.710346 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/transforms/post_transforms/
+-rw-rw-rw-   0        0        0    12011 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/transforms/post_transforms/__init__.py
+-rw-rw-rw-   0        0        0     4486 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/transforms/post_transforms/code.py
+-rw-rw-rw-   0        0        0    10043 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/transforms/post_transforms/images.py
+-rw-rw-rw-   0        0        0     1361 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/transforms/references.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.737372 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/
+-rw-rw-rw-   0        0        0    14314 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/__init__.py
+-rw-rw-rw-   0        0        0      240 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/build_phase.py
+-rw-rw-rw-   0        0        0    15290 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/cfamily.py
+-rw-rw-rw-   0        0        0     3218 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/console.py
+-rw-rw-rw-   0        0        0     2281 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/display.py
+-rw-rw-rw-   0        0        0    16330 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/docfields.py
+-rw-rw-rw-   0        0        0     2930 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/docstrings.py
+-rw-rw-rw-   0        0        0    22957 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/docutils.py
+-rw-rw-rw-   0        0        0     1960 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/exceptions.py
+-rw-rw-rw-   0        0        0     3722 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/fileutil.py
+-rw-rw-rw-   0        0        0      513 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/http_date.py
+-rw-rw-rw-   0        0        0    10043 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/i18n.py
+-rw-rw-rw-   0        0        0     3451 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/images.py
+-rw-rw-rw-   0        0        0    28244 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/inspect.py
+-rw-rw-rw-   0        0        0     6311 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/inventory.py
+-rw-rw-rw-   0        0        0     5855 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/jsdump.py
+-rw-rw-rw-   0        0        0    18103 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/logging.py
+-rw-rw-rw-   0        0        0     5274 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/matching.py
+-rw-rw-rw-   0        0        0     1816 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/math.py
+-rw-rw-rw-   0        0        0    22872 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/nodes.py
+-rw-rw-rw-   0        0        0     6973 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/osutil.py
+-rw-rw-rw-   0        0        0     5023 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/parallel.py
+-rw-rw-rw-   0        0        0     1445 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/png.py
+-rw-rw-rw-   0        0        0     2870 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/requests.py
+-rw-rw-rw-   0        0        0     3330 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/rst.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.738372 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/stemmer/
+-rw-rw-rw-   0        0        0     2230 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/stemmer/__init__.py
+-rw-rw-rw-   0        0        0     2651 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/tags.py
+-rw-rw-rw-   0        0        0     4691 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/template.py
+-rw-rw-rw-   0        0        0     5442 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/texescape.py
+-rw-rw-rw-   0        0        0    14984 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/util/typing.py
+-rw-rw-rw-   0        0        0     5801 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/versioning.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.747381 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/writers/
+-rw-rw-rw-   0        0        0       31 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/writers/__init__.py
+-rw-rw-rw-   0        0        0    33271 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/writers/_html4.py
+-rw-rw-rw-   0        0        0     1669 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/writers/html.py
+-rw-rw-rw-   0        0        0    31991 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/writers/html5.py
+-rw-rw-rw-   0        0        0    85057 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/writers/latex.py
+-rw-rw-rw-   0        0        0    15475 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/writers/manpage.py
+-rw-rw-rw-   0        0        0    52823 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/writers/texinfo.py
+-rw-rw-rw-   0        0        0    37916 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/writers/text.py
+-rw-rw-rw-   0        0        0     1457 2023-04-26 20:43:03.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx/writers/xml.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.748381 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx_rtd_theme/
+-rw-rw-rw-   0        0        0     3193 2023-05-05 00:38:13.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinx_rtd_theme/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:03.939738 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.749382 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/applehelp/
+-rw-rw-rw-   0        0        0    10985 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/applehelp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.751384 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/devhelp/
+-rw-rw-rw-   0        0        0     5146 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/devhelp/__init__.py
+-rw-rw-rw-   0        0        0      271 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/devhelp/version.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.751384 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/htmlhelp/
+-rw-rw-rw-   0        0        0    12044 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/htmlhelp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.752384 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/jquery/
+-rw-rw-rw-   0        0        0     1787 2023-05-05 00:38:13.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/jquery/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.754387 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/jsmath/
+-rw-rw-rw-   0        0        0     3409 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/jsmath/__init__.py
+-rw-rw-rw-   0        0        0      293 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/jsmath/version.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.756389 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/qthelp/
+-rw-rw-rw-   0        0        0    10712 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/qthelp/__init__.py
+-rw-rw-rw-   0        0        0      269 2023-04-26 20:42:59.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/qthelp/version.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.759390 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/serializinghtml/
+-rw-rw-rw-   0        0        0     6064 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/serializinghtml/__init__.py
+-rw-rw-rw-   0        0        0     1095 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/serializinghtml/jsonimpl.py
+-rw-rw-rw-   0        0        0      287 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/sphinxcontrib/serializinghtml/version.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.769401 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/
+-rw-rw-rw-   0        0        0     3333 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/__init__.py
+-rw-rw-rw-   0        0        0    10811 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/_collections.py
+-rw-rw-rw-   0        0        0       64 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/_version.py
+-rw-rw-rw-   0        0        0    20300 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/connection.py
+-rw-rw-rw-   0        0        0    39128 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/connectionpool.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.775406 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/contrib/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/contrib/__init__.py
+-rw-rw-rw-   0        0        0      957 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/contrib/_appengine_environ.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.778408 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/contrib/_securetransport/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-rw-   0        0        0    17632 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-rw-   0        0        0    13922 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-rw-   0        0        0    11012 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/contrib/appengine.py
+-rw-rw-rw-   0        0        0     4528 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/contrib/ntlmpool.py
+-rw-rw-rw-   0        0        0    17055 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/contrib/pyopenssl.py
+-rw-rw-rw-   0        0        0    34416 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/contrib/securetransport.py
+-rw-rw-rw-   0        0        0     7097 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/contrib/socks.py
+-rw-rw-rw-   0        0        0     8217 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/exceptions.py
+-rw-rw-rw-   0        0        0     8579 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/fields.py
+-rw-rw-rw-   0        0        0     2440 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/filepost.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.780410 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/packages/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/packages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.782412 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/packages/backports/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/packages/backports/__init__.py
+-rw-rw-rw-   0        0        0     1417 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/packages/backports/makefile.py
+-rw-rw-rw-   0        0        0    34665 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/packages/six.py
+-rw-rw-rw-   0        0        0    19786 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/poolmanager.py
+-rw-rw-rw-   0        0        0     5985 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/request.py
+-rw-rw-rw-   0        0        0    30761 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/response.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.795423 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/util/
+-rw-rw-rw-   0        0        0     1155 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/util/__init__.py
+-rw-rw-rw-   0        0        0     4901 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/util/connection.py
+-rw-rw-rw-   0        0        0     1605 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/util/proxy.py
+-rw-rw-rw-   0        0        0      498 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/util/queue.py
+-rw-rw-rw-   0        0        0     4225 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/util/request.py
+-rw-rw-rw-   0        0        0     3510 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/util/response.py
+-rw-rw-rw-   0        0        0    22003 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/util/retry.py
+-rw-rw-rw-   0        0        0    17165 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/util/ssl_.py
+-rw-rw-rw-   0        0        0     5758 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/util/ssl_match_hostname.py
+-rw-rw-rw-   0        0        0     6895 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/util/ssltransport.py
+-rw-rw-rw-   0        0        0    10168 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/util/timeout.py
+-rw-rw-rw-   0        0        0    14279 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/util/url.py
+-rw-rw-rw-   0        0        0     5403 2023-04-26 20:42:58.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/urllib3/util/wait.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.799427 columbia-discord-bot-0.2.1/docs/_build/html/_static/yarl/
+-rw-rw-rw-   0        0        0      159 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/yarl/__init__.py
+-rw-rw-rw-   0        0        0      555 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/yarl/_quoting.py
+-rw-rw-rw-   0        0        0     6567 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/yarl/_quoting_py.py
+-rw-rw-rw-   0        0        0    39132 2023-04-26 20:39:42.000000 columbia-discord-bot-0.2.1/docs/_build/html/_static/yarl/_url.py
+-rw-rw-rw-   0        0        0     1542 2023-05-11 00:23:51.000000 columbia-discord-bot-0.2.1/docs/conf.py
+-rw-rw-rw-   0        0        0      117 2023-05-11 00:23:51.000000 columbia-discord-bot-0.2.1/docs/index.md
+-rwxrwxrwx   0        0        0      765 2023-05-11 00:23:51.000000 columbia-discord-bot-0.2.1/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.803431 columbia-discord-bot-0.2.1/docs/source/
+-rw-rw-rw-   0        0        0      152 2023-05-11 00:23:51.000000 columbia-discord-bot-0.2.1/docs/source/columbia_discord_bot.rst
+-rw-rw-rw-   0        0        0       82 2023-05-11 00:23:51.000000 columbia-discord-bot-0.2.1/docs/source/modules.rst
+-rw-rw-rw-   0        0        0      109 2023-05-11 00:23:51.000000 columbia-discord-bot-0.2.1/docs/source/student.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.806434 columbia-discord-bot-0.2.1/project/
+-rw-rw-rw-   0        0        0     2414 2023-05-11 02:24:21.000000 columbia-discord-bot-0.2.1/project/columbia_discord_bot.py
+-rw-rw-rw-   0        0        0       85 2023-05-10 18:34:00.000000 columbia-discord-bot-0.2.1/project/config.json
+-rw-rw-rw-   0        0        0     2487 2023-05-11 02:22:05.000000 columbia-discord-bot-0.2.1/project/student.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:05.808436 columbia-discord-bot-0.2.1/project/tests/
+-rw-rw-rw-   0        0        0     1249 2023-05-11 02:30:35.000000 columbia-discord-bot-0.2.1/project/tests/integration_test.py
+-rw-rw-rw-   0        0        0     2390 2023-05-11 02:30:49.000000 columbia-discord-bot-0.2.1/project/tests/unit_tests.py
+-rw-rw-rw-   0        0        0     2229 2023-05-11 02:49:28.000000 columbia-discord-bot-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 02:52:05.810438 columbia-discord-bot-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      367 2023-05-05 01:09:45.000000 columbia-discord-bot-0.2.1/setup.py
```

### Comparing `columbia-discord-bot-0.1.1/LICENSE` & `columbia-discord-bot-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `columbia-discord-bot-0.1.1/Makefile` & `columbia-discord-bot-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `columbia-discord-bot-0.1.1/README.md` & `columbia-discord-bot-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Columbia Discord Bot
 
 [![Build Status](https://github.com/mw3071/columbia-discord-bot/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/mw3071/columbia-discord-bot/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/mw3071/columbia-discord-bot/branch/main/graph/badge.svg)](https://codecov.io/gh/mw3071/columbia-discord-bot)
 [![PyPI](https://img.shields.io/pypi/v/columbia-discord-bot)](https://pypi.org/project/columbia-discord-bot/)
 ![GitHub](https://img.shields.io/github/license/mw3071/columbia-discord-bot)
 ![GitHub issues](https://img.shields.io/github/issues/mw3071/columbia-discord-bot)
+![Docs](https://img.shields.io/readthedocs/columbia-discord-bot)
 
 ## Overview
 A Discord bot that allows users to keep track of and find other students with the same classes and professors.
 
 ## How to add to your Discord server
 Invite this bot using this [link](https://discord.com/api/oauth2/authorize?client_id=1079902946768199700&permissions=8&scope=bot) 
 
@@ -24,8 +25,8 @@
 ```!removeprof <professor>``` - removes a professor from your profile
 
 ```!getclasses <class>``` - gives you the list of classes you have
 
 ```!getprofs <professor>``` - gives you the list of professors you have
 
 ## Downloading and installing this repo
-You can check out CONTRIBUTING.md to find out how to fork, clone, and make edits to this bot. You will need your own bot token from Discord along with some other dependencies.
+You can check out CONTRIBUTING.md to find out how to fork, clone, and make edits to this bot. You will need your own bot token from Discord along with some other dependencies.
```

### Comparing `columbia-discord-bot-0.1.1/project/columbia_discord_bot.py` & `columbia-discord-bot-0.2.1/project/columbia_discord_bot.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,94 @@
 import discord
 import json
 from student import Student
 from discord.ext import commands
+import os
 
 
-with open('./config.json', 'r') as cfg:
+directory_path = os.path.dirname(os.path.abspath(__file__))
+new_path = os.path.join(directory_path, "config.json")
+
+with open(new_path, 'r') as cfg:
     data = json.load(cfg)
     token = data["token"]
 
 print(token)
 CHANNEL_ID = '1079912337571598438'
 intents = discord.Intents.all()
 bot = commands.Bot(command_prefix='!', intents=intents)
 users = {}
 s = None
 
 
 @bot.event
 async def on_ready():
+    '''tells user that the bot is now running'''
     print("Bot is now running")
 
 
 @bot.command()
 async def ping(ctx):
+    '''tests if the bot responds with pong when the user messages ping'''
     await ctx.send('pong!')
 
 
 @bot.command(help="creates a new student, must give it a uni")
 async def createuser(ctx):
+    '''takes the discord context and extracts the uni from the
+    message and then creates the student object'''
     username = str(ctx.author)
     uni = ctx.message.content.split(' ')[1]
     print(uni)
     print(username)
     s = Student(username, uni)
     users[username] = s
     print(s)
     print(users)
     await ctx.send('created!')
 
 
 @bot.command()
 async def addclass(ctx):
+    '''takes the discord context and extracts class from the message,
+    and then adds a class to the student'''
     username = str(ctx.author)
     users[username].add_class(ctx.message.content.split(' ')[1])
     print(users[username])
 
     await ctx.send('Added class!')
 
 
 @bot.command()
 async def addprof(ctx):
+    '''takes the discord context and extracts professor from the message,
+    and then adds a professor to the student'''
+    username = str(ctx.author)
+    users[username].add_prof(ctx.message.content.split(' ')[1])
+    print(users[username])
+
     await ctx.send('Added prof!')
 
 
-# @bot.command()
-# async def getusernames(ctx):
-#     await ctx.send(df['username'])
-
-# @bot.command()
-# async def getclasses(ctx):
-#     await ctx.send(df['class_name'][0])
-
-# @bot.command()
-# async def getunis(ctx):
-#     await ctx.send(df['uni'])
+@bot.command()
+async def lookupclass(ctx):
+    '''takes the discord context and extracts a class from the message,
+    and then returns unis with that class'''
+    username = str(ctx.author)
+    c = users[username].look_up_class(ctx.message.content.split(' ')[1], users)
+    print(c)
+
+    await ctx.send(c)
+
+
+@bot.command()
+async def lookupprof(ctx):
+    '''takes the discord context and extracts a class from the message,
+    and then returns unis with that class'''
+    username = str(ctx.author)
+    p = users[username].look_up_prof(ctx.message.content.split(' ')[1], users)
+    print(p)
+
+    await ctx.send(p)
+
 
 bot.run(token)
```

### Comparing `columbia-discord-bot-0.1.1/project/integration test/LICENSE` & `columbia-discord-bot-0.2.1/docs/_build/html/_static/discord/_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,34 @@
-MIT License
+"""
+The MIT License (MIT)
 
-Copyright (c) 2018 Declan
+Copyright (c) 2015-present Rapptz
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+from typing import TypeVar, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing_extensions import TypeVar
+    from .client import Client
+
+    ClientT = TypeVar('ClientT', bound=Client, covariant=True, default=Client)
+else:
+    ClientT = TypeVar('ClientT', bound='Client', covariant=True)
```

### Comparing `columbia-discord-bot-0.1.1/project/integration test/dismock/__init__.py` & `columbia-discord-bot-0.2.1/docs/_build/html/_static/pip/_vendor/pyparsing/testing.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,442 +1,331 @@
-''' Dismock is a small library designed to help with the
-    creation of bots to test other bots. This is currently
-    part of the MathBot project but if it gains enough
-    traction I might fork it into its own repository
-    Interfacing with the bot through discord:
+# testing.py
 
-    ::stats
-        Gives details about which tests have been
-        run and what the results were
+from contextlib import contextmanager
+import typing
 
-    ::run test_name
-        Run a particular test
-
-    ::run all
-        Run all tests
-
-    ::run unrun
-        Run all tests that have not yet been run
-
-    ::run failed
-        Run all tests that failed on the most recent run
-
-'''
-
-
-import asyncio
-import re
-import enum
-
-import discord
-
-
-TIMEOUT = 20
-
-
-HELP_TEXT = '''\
-**::help** - Sshow this help
-**::run** all - Run all tests
-**::run** unrun - Run all tests that have not been run
-**::run** *name* - Run a specific test
-**::list** - List all the tests and their status
-'''
-
-
-SPECIAL_TEST_NAMES = {'all', 'unrun', 'failed'}
-
-
-class TestRequirementFailure(Exception):
-    '''Base calss for the errors that are
-    raised when an expectation is not met'''
-
-
-class NoResponseError(TestRequirementFailure):
-    '''Raised when the target bot fails to respond to a message'''
-
-
-class NoReactionError(TestRequirementFailure):
-    '''Raised when the target bot failed to react to a message'''
-
-
-class UnexpectedResponseError(TestRequirementFailure):
-    '''Raised when the target bot failed to stay silent'''
-
-
-class ErrordResponseError(TestRequirementFailure):
-    '''Raised when the target bot produced an error message'''
-
-
-class UnexpectedSuccessError(TestRequirementFailure):
-    '''Raised when the target bot failed to produce an error message'''
-
-
-class HumanResponseTimeout(TestRequirementFailure):
-    '''Raised when a human fails to assert the result of a test'''
-
-
-class HumanResponseFailure(TestRequirementFailure):
-    '''Raised when a human fails a test'''
-
-
-class ResponseDidNotMatchError(TestRequirementFailure):
-    '''Raised when the target bot responds with a
-    message that doesn't meet criteria'''
-
-
-class ReactionDidNotMatchError(TestRequirementFailure):
-    '''Raised when the target bot reacts with the wrong emoji'''
-
-
-class TestResult(enum.Enum):
-    '''Enum representing the result of running a test case'''
-
-    UNRUN = 0
-    SUCCESS = 1
-    FAILED = 2
-
-
-class Test:
-
-    '''Holds data about a specific test'''
-
-    def __init__(self, name: str, func, needs_human: bool = False) -> None:
-        if name in SPECIAL_TEST_NAMES:
-            raise ValueError('{} is not a valid test name'.format(name))
-        self.name = name  # The name of the test
-        self.func = func  # The function to run when running the test
-        self.last_run = 0  # When the test was last run
-        self.result = TestResult.UNRUN
-        # The result of the test (True or False) or None if it was not run
-        self.needs_human = needs_human
-        # Whether the test requires human interation
-
-
-class Interface:
-
-    '''The interface that the test functions should use to
-    interface with discord.
-    Test functions should not access the discord.py client directly.
-    '''
-
-    def __init__(self, client: discord.Client, channel: discord.TextChannel, target: discord.User) -> None:
-        self.client = client  # The discord.py client object
-        self.channel = channel  # The channel the test is running in
-        self.target = target  # The bot which we are testing
-
-    async def send_message(self, content):
-        '''Send a message to the testing channel.'''
-        return await self.channel.send(content)
-
-    async def edit_message(self, message, new_content):
-        '''Modified a message. Doesn't actually care what this message is.'''
-        return await self.client.edit_message(message, new_content)
-
-    async def wait_for_reaction(self, message):
-        def check(reaction, user):
-            return (
-                reaction.message.id == message.id and user == self.target and reaction.message.channel == self.channel
+from .core import (
+    ParserElement,
+    ParseException,
+    Keyword,
+    __diag__,
+    __compat__,
+)
+
+
+class pyparsing_test:
+    """
+    namespace class for classes useful in writing unit tests
+    """
+
+    class reset_pyparsing_context:
+        """
+        Context manager to be used when writing unit tests that modify pyparsing config values:
+        - packrat parsing
+        - bounded recursion parsing
+        - default whitespace characters.
+        - default keyword characters
+        - literal string auto-conversion class
+        - __diag__ settings
+
+        Example::
+
+            with reset_pyparsing_context():
+                # test that literals used to construct a grammar are automatically suppressed
+                ParserElement.inlineLiteralsUsing(Suppress)
+
+                term = Word(alphas) | Word(nums)
+                group = Group('(' + term[...] + ')')
+
+                # assert that the '()' characters are not included in the parsed tokens
+                self.assertParseAndCheckList(group, "(abc 123 def)", ['abc', '123', 'def'])
+
+            # after exiting context manager, literals are converted to Literal expressions again
+        """
+
+        def __init__(self):
+            self._save_context = {}
+
+        def save(self):
+            self._save_context["default_whitespace"] = ParserElement.DEFAULT_WHITE_CHARS
+            self._save_context["default_keyword_chars"] = Keyword.DEFAULT_KEYWORD_CHARS
+
+            self._save_context[
+                "literal_string_class"
+            ] = ParserElement._literalStringClass
+
+            self._save_context["verbose_stacktrace"] = ParserElement.verbose_stacktrace
+
+            self._save_context["packrat_enabled"] = ParserElement._packratEnabled
+            if ParserElement._packratEnabled:
+                self._save_context[
+                    "packrat_cache_size"
+                ] = ParserElement.packrat_cache.size
+            else:
+                self._save_context["packrat_cache_size"] = None
+            self._save_context["packrat_parse"] = ParserElement._parse
+            self._save_context[
+                "recursion_enabled"
+            ] = ParserElement._left_recursion_enabled
+
+            self._save_context["__diag__"] = {
+                name: getattr(__diag__, name) for name in __diag__._all_names
+            }
+
+            self._save_context["__compat__"] = {
+                "collect_all_And_tokens": __compat__.collect_all_And_tokens
+            }
+
+            return self
+
+        def restore(self):
+            # reset pyparsing global state
+            if (
+                ParserElement.DEFAULT_WHITE_CHARS
+                != self._save_context["default_whitespace"]
+            ):
+                ParserElement.set_default_whitespace_chars(
+                    self._save_context["default_whitespace"]
+                )
+
+            ParserElement.verbose_stacktrace = self._save_context["verbose_stacktrace"]
+
+            Keyword.DEFAULT_KEYWORD_CHARS = self._save_context["default_keyword_chars"]
+            ParserElement.inlineLiteralsUsing(
+                self._save_context["literal_string_class"]
             )
 
-        result = await self.client.wait_for_reaction(timeout=TIMEOUT, check=check)
-        if result is None:
-            raise NoReactionError
-        return result
-
-    async def wait_for_message(self):
-        ''' Waits for the bot the send a message.
-                        If the bot takes longer than {} seconds,
-                        the test fails.
-                '''.format(
-            TIMEOUT
-        )
+            for name, value in self._save_context["__diag__"].items():
+                (__diag__.enable if value else __diag__.disable)(name)
 
-        result = await self.client.wait_for(
-            'message',
-            timeout=TIMEOUT,
-            # channel=self.channel,
-            # author=self.target
-        )
-        if result is None:
-            raise NoResponseError
-        print("CHANNEL LAST MESSAGE", self.channel.last_message)
-        return self.channel.last_message
-        return result
-
-    async def wait_for_reply(self, content):
-        '''Sends a message and returns the
-        next message that the targeted bot sends.'''
-        await self.send_message(content)
-        return await self.wait_for_message()
-
-    async def assert_message_equals(self, matches):
-        '''Waits for the next message.
-        If the message does not match a string exactly, fail the test.
-        '''
-        response = await self.wait_for_message()
-        if response.content != matches:
-            raise ResponseDidNotMatchError
-        return response
-
-    async def assert_message_contains(self, substring):
-        '''Waits for the next message.
-        If the message does not contain
-        the given substring, fail the test.
-        '''
-        response = await self.wait_for_message()
-        if substring not in response.content:
-            raise ResponseDidNotMatchError
-        return response
-
-    async def assert_message_matches(self, regex):
-        '''Waits for the next message.
-        If the message does not match a regex, fail the test.
-        '''
-        response = await self.wait_for_message()
-        if not re.match(regex, response.content):
-            raise ResponseDidNotMatchError
-        return response
-
-    async def assert_reply_equals(self, contents, matches):
-        '''Send a message and wait for a response.
-        If the response does not match a s
-        tring exactly, fail the test.
-        '''
-        # print('Sending...')
-        await self.send_message(contents)
-        # print('About to wait...')
-        response = await self.wait_for_message()
-        print("response: ", response)
-        print("matches: ", matches)
-        if response.content != matches:
-            raise ResponseDidNotMatchError
-        return response
-
-    async def assert_reply_contains(self, contents, substring):
-        '''Send a message and wait for a response.
-        If the response does not contain
-        the given substring, fail the test.
-        '''
-        await self.send_message(contents)
-        response = await self.wait_for_message()
-        if substring not in response.content:
-            raise ResponseDidNotMatchError
-        return response
-
-    async def assert_reply_matches(self, contents, regex):
-        '''Send a message and wait for a response.
-        If the response does not match a regex, fail the test.
-        '''
-        await self.send_message(contents)
-        response = await self.wait_for_message()
-        if not re.match(regex, response.content):
-            raise ResponseDidNotMatchError
-        return response
-
-    async def assert_reaction_equals(self, contents, emoji):
-        reaction = await self.wait_for_reaction(await self.send_message(contents))
-        if str(reaction.emoji) != emoji:
-            raise ReactionDidNotMatchError
-        return reaction
-
-    async def ensure_silence(self):
-        '''Ensures that the bot does not post any messages
-        for some number of seconds.'''
-        result = await self.client.wait_for_message(timeout=TIMEOUT, channel=self.channel, author=self.target)
-        if result is not None:
-            raise UnexpectedResponseError
-
-    async def ask_human(self, query):
-        '''Asks a human for an opinion on a question.
-        Currently, only yes-no questions
-        are supported. If the human answers 'no', the test will be failed.
-        '''
-        message = await self.channel.send(query)
-        await self.client.add_reaction(message, u'\u2714')
-        await self.client.add_reaction(message, u'\u274C')
-        await asyncio.sleep(0.5)
-        reaction = await self.client.wait_for_reaction(timeout=TIMEOUT, message=message)
-        if reaction is None:
-            raise HumanResponseTimeout
-        reaction, _ = reaction
-        if reaction.emoji == u'\u274C':
-            raise HumanResponseFailure
-
-
-class ExpectCalls:  # pylint: disable=too-few-public-methods
-
-    '''Wrap a function in an object which counts the number
-    of times it was called. If the number of calls is not
-    equal to the expected number when this object is
-    garbage collected, something has gone wrong, and in
-    that case an error is thrown.
-    '''
-
-    def __init__(self, function, expected_calls=1):
-        self.function = function
-        self.expected_calls = expected_calls
-        self.call_count = 0
-
-    def __call__(self, *args, **kwargs):
-        self.call_count += 1
-        return self.function(*args, **kwargs)
-
-    def __del__(self):
-        if self.call_count != self.expected_calls:
-            message = """{} was called {} times.
-            It was expcted to have been called {} times"""
-            raise RuntimeError(message.format(self.function, self.call_count, self.expected_calls))
-
-
-class TestCollector:
-
-    '''Used to group tests and pass them around all at once.'''
-
-    def __init__(self):
-        self._tests = []
-
-    def add(self, function, name: str = '', needs_human: bool = False):
-        '''Adds a test function to the group.'''
-        name = name or function.__name__
-        test = Test(name, function, needs_human=needs_human)
-        if name in self._tests:
-            raise KeyError('A test case called {} already exists.'.format(name))
-        self._tests.append(test)
-
-    def find_by_name(self, name: str):
-        '''Return the test with the given name.
-        Return None if it does not exist.
-        '''
-        for i in self._tests:
-            if i.name == name:
-                return i
-        return None
-
-    def __call__(self, *args, **kwargs):
-        '''Add a test decorator-style.'''
-
-        def _decorator(function):
-            self.add(function, *args, **kwargs)
-
-        return ExpectCalls(_decorator, 1)
-
-    def __iter__(self):
-        return (i for i in self._tests)
-
-
-class DiscordBot(discord.Client):
-
-    '''Discord bot used to run tests.
-    This class by itself does not
-    provide any useful methods for human interaction.
-    '''
-
-    def __init__(self, target_name: str) -> None:
-        super().__init__(intents=discord.Intents.all())
-        self._target_name = target_name.lower()
-        # self._setup_done = False
-
-    def _find_target(self, server: discord.Guild) -> discord.Member:
-        for i in server.members:
-            if self._target_name in i.name.lower():
-                return i
-        raise KeyError('Could not find memory with name {}'.format(self._target_name))
-
-    async def run_test(self, test: Test, channel: discord.TextChannel, stop_error: bool = False) -> TestResult:
-        '''Run a single test in a given channel.
-        Updates the test with the result, and also returns it.
-        '''
-        interface = Interface(self, channel, self._find_target(channel.guild))
-        try:
-            await test.func(interface)
-        except TestRequirementFailure:
-            test.result = TestResult.FAILED
-            if not stop_error:
-                raise
-        else:
-            test.result = TestResult.SUCCESS
-        return test.result
+            ParserElement._packratEnabled = False
+            if self._save_context["packrat_enabled"]:
+                ParserElement.enable_packrat(self._save_context["packrat_cache_size"])
+            else:
+                ParserElement._parse = self._save_context["packrat_parse"]
+            ParserElement._left_recursion_enabled = self._save_context[
+                "recursion_enabled"
+            ]
+
+            __compat__.collect_all_And_tokens = self._save_context["__compat__"]
+
+            return self
+
+        def copy(self):
+            ret = type(self)()
+            ret._save_context.update(self._save_context)
+            return ret
+
+        def __enter__(self):
+            return self.save()
+
+        def __exit__(self, *args):
+            self.restore()
+
+    class TestParseResultsAsserts:
+        """
+        A mixin class to add parse results assertion methods to normal unittest.TestCase classes.
+        """
+
+        def assertParseResultsEquals(
+            self, result, expected_list=None, expected_dict=None, msg=None
+        ):
+            """
+            Unit test assertion to compare a :class:`ParseResults` object with an optional ``expected_list``,
+            and compare any defined results names with an optional ``expected_dict``.
+            """
+            if expected_list is not None:
+                self.assertEqual(expected_list, result.as_list(), msg=msg)
+            if expected_dict is not None:
+                self.assertEqual(expected_dict, result.as_dict(), msg=msg)
+
+        def assertParseAndCheckList(
+            self, expr, test_string, expected_list, msg=None, verbose=True
+        ):
+            """
+            Convenience wrapper assert to test a parser element and input string, and assert that
+            the resulting ``ParseResults.asList()`` is equal to the ``expected_list``.
+            """
+            result = expr.parse_string(test_string, parse_all=True)
+            if verbose:
+                print(result.dump())
+            else:
+                print(result.as_list())
+            self.assertParseResultsEquals(result, expected_list=expected_list, msg=msg)
 
+        def assertParseAndCheckDict(
+            self, expr, test_string, expected_dict, msg=None, verbose=True
+        ):
+            """
+            Convenience wrapper assert to test a parser element and input string, and assert that
+            the resulting ``ParseResults.asDict()`` is equal to the ``expected_dict``.
+            """
+            result = expr.parse_string(test_string, parseAll=True)
+            if verbose:
+                print(result.dump())
+            else:
+                print(result.as_list())
+            self.assertParseResultsEquals(result, expected_dict=expected_dict, msg=msg)
 
-class DiscordUI(DiscordBot):
+        def assertRunTestResults(
+            self, run_tests_report, expected_parse_results=None, msg=None
+        ):
+            """
+            Unit test assertion to evaluate output of ``ParserElement.runTests()``. If a list of
+            list-dict tuples is given as the ``expected_parse_results`` argument, then these are zipped
+            with the report tuples returned by ``runTests`` and evaluated using ``assertParseResultsEquals``.
+            Finally, asserts that the overall ``runTests()`` success value is ``True``.
+
+            :param run_tests_report: tuple(bool, [tuple(str, ParseResults or Exception)]) returned from runTests
+            :param expected_parse_results (optional): [tuple(str, list, dict, Exception)]
+            """
+            run_test_success, run_test_results = run_tests_report
+
+            if expected_parse_results is not None:
+                merged = [
+                    (*rpt, expected)
+                    for rpt, expected in zip(run_test_results, expected_parse_results)
+                ]
+                for test_string, result, expected in merged:
+                    # expected should be a tuple containing a list and/or a dict or an exception,
+                    # and optional failure message string
+                    # an empty tuple will skip any result validation
+                    fail_msg = next(
+                        (exp for exp in expected if isinstance(exp, str)), None
+                    )
+                    expected_exception = next(
+                        (
+                            exp
+                            for exp in expected
+                            if isinstance(exp, type) and issubclass(exp, Exception)
+                        ),
+                        None,
+                    )
+                    if expected_exception is not None:
+                        with self.assertRaises(
+                            expected_exception=expected_exception, msg=fail_msg or msg
+                        ):
+                            if isinstance(result, Exception):
+                                raise result
+                    else:
+                        expected_list = next(
+                            (exp for exp in expected if isinstance(exp, list)), None
+                        )
+                        expected_dict = next(
+                            (exp for exp in expected if isinstance(exp, dict)), None
+                        )
+                        if (expected_list, expected_dict) != (None, None):
+                            self.assertParseResultsEquals(
+                                result,
+                                expected_list=expected_list,
+                                expected_dict=expected_dict,
+                                msg=fail_msg or msg,
+                            )
+                        else:
+                            # warning here maybe?
+                            print("no validation for {!r}".format(test_string))
+
+            # do this last, in case some specific test results can be reported instead
+            self.assertTrue(
+                run_test_success, msg=msg if msg is not None else "failed runTests"
+            )
 
-    '''A variant of the discord bot which supports additional commands
-    to allow a human to also interact with it.
-    '''
-
-    def __init__(self, target_name: str, tests: TestCollector) -> None:
-        super().__init__(target_name)
-        self._tests = tests
-
-    async def _run_by_predicate(self, channel, prediate):
-        for test in self._tests:
-            if prediate(test):
-                await channel.send('**Running test {}**'.format(test.name))
-                await self.run_test(test, channel, stop_error=True)
-
-    async def _display_stats(self, channel: discord.TextChannel) -> None:
-        '''Display the status of the various tests.'''
-        # NOTE: An emoji is the width of two spaces
-        response = '```\n'
-        longest_name = max(map(lambda t: len(t.name), self._tests))
-        for test in self._tests:
-            response += test.name.rjust(longest_name) + ' '
-            if test.needs_human:
-                response += '✋ '
+        @contextmanager
+        def assertRaisesParseException(self, exc_type=ParseException, msg=None):
+            with self.assertRaises(exc_type, msg=msg):
+                yield
+
+    @staticmethod
+    def with_line_numbers(
+        s: str,
+        start_line: typing.Optional[int] = None,
+        end_line: typing.Optional[int] = None,
+        expand_tabs: bool = True,
+        eol_mark: str = "|",
+        mark_spaces: typing.Optional[str] = None,
+        mark_control: typing.Optional[str] = None,
+    ) -> str:
+        """
+        Helpful method for debugging a parser - prints a string with line and column numbers.
+        (Line and column numbers are 1-based.)
+
+        :param s: tuple(bool, str - string to be printed with line and column numbers
+        :param start_line: int - (optional) starting line number in s to print (default=1)
+        :param end_line: int - (optional) ending line number in s to print (default=len(s))
+        :param expand_tabs: bool - (optional) expand tabs to spaces, to match the pyparsing default
+        :param eol_mark: str - (optional) string to mark the end of lines, helps visualize trailing spaces (default="|")
+        :param mark_spaces: str - (optional) special character to display in place of spaces
+        :param mark_control: str - (optional) convert non-printing control characters to a placeholding
+                                 character; valid values:
+                                 - "unicode" - replaces control chars with Unicode symbols, such as "␍" and "␊"
+                                 - any single character string - replace control characters with given string
+                                 - None (default) - string is displayed as-is
+
+        :return: str - input string with leading line numbers and column number headers
+        """
+        if expand_tabs:
+            s = s.expandtabs()
+        if mark_control is not None:
+            if mark_control == "unicode":
+                tbl = str.maketrans(
+                    {c: u for c, u in zip(range(0, 33), range(0x2400, 0x2433))}
+                    | {127: 0x2421}
+                )
+                eol_mark = ""
             else:
-                response += '   '
-            if test.result is TestResult.UNRUN:
-                response += '⚫ Not run\n'
-            elif test.result is TestResult.SUCCESS:
-                response += '✔️ Passed\n'
-            elif test.result is TestResult.FAILED:
-                response += '❌ Failed\n'
-        response += '```\n'
-        await channel.send(response)
-
-    async def on_ready(self) -> None:
-        '''Report when the bot is ready for use'''
-        print('Started dismock bot.')
-        print('Available tests are:')
-        for i in self._tests:
-            print('   {}'.format(i.name))
-
-    async def on_message(self, message: discord.Message) -> None:
-        '''Handle an incomming message'''
-        # if not message.channel.is_private:
-        if message.content.startswith('::run '):
-            name = message.content[6:]
-            print('Running test:', name)
-            if name == 'all':
-                await self._run_by_predicate(message.channel, lambda t: True)
-            elif name == 'unrun':
-
-                def pred(t):
-                    return t.result is TestResult.UNRUN
-
-                await self._run_by_predicate(message.channel, pred)
-            elif name == 'failed':
-
-                def pred(t):
-                    return t.result is TestResult.FAILED
-
-                await self._run_by_predicate(message.channel, pred)
-            elif '*' in name:
-                regex = re.compile(name.replace('*', '.*'))
-                await self.run_many(message, lambda t: regex.fullmatch(t.name))
-            elif self._tests.find_by_name(name) is None:
-                text = ':x: There is no test called `{}`'
-                await self.send_message(message.channel, text.format(name))
+                tbl = str.maketrans(
+                    {c: mark_control for c in list(range(0, 32)) + [127]}
+                )
+            s = s.translate(tbl)
+        if mark_spaces is not None and mark_spaces != " ":
+            if mark_spaces == "unicode":
+                tbl = str.maketrans({9: 0x2409, 32: 0x2423})
+                s = s.translate(tbl)
             else:
-                await message.channel.send('Running test `{}`'.format(name))
-                await self.run_test(self._tests.find_by_name(name), message.channel)
-                await self._display_stats(message.channel)
-        # Status display command
-        elif message.content in ['::stats', '::list']:
-            await self._display_stats(message.channel)
-        elif message.content == '::help':
-            await self.send_message(message.channel, HELP_TEXT)
-
+                s = s.replace(" ", mark_spaces)
+        if start_line is None:
+            start_line = 1
+        if end_line is None:
+            end_line = len(s)
+        end_line = min(end_line, len(s))
+        start_line = min(max(1, start_line), end_line)
 
-def run_interactive_bot(target_name, token, test_collector):
-    bot = DiscordUI(target_name, test_collector)
-    bot.run(token)
+        if mark_control != "unicode":
+            s_lines = s.splitlines()[start_line - 1 : end_line]
+        else:
+            s_lines = [line + "␊" for line in s.split("␊")[start_line - 1 : end_line]]
+        if not s_lines:
+            return ""
+
+        lineno_width = len(str(end_line))
+        max_line_len = max(len(line) for line in s_lines)
+        lead = " " * (lineno_width + 1)
+        if max_line_len >= 99:
+            header0 = (
+                lead
+                + "".join(
+                    "{}{}".format(" " * 99, (i + 1) % 100)
+                    for i in range(max(max_line_len // 100, 1))
+                )
+                + "\n"
+            )
+        else:
+            header0 = ""
+        header1 = (
+            header0
+            + lead
+            + "".join(
+                "         {}".format((i + 1) % 10)
+                for i in range(-(-max_line_len // 10))
+            )
+            + "\n"
+        )
+        header2 = lead + "1234567890" * (-(-max_line_len // 10)) + "\n"
+        return (
+            header1
+            + header2
+            + "\n".join(
+                "{:{}d}:{}{}".format(i, lineno_width, line, eol_mark)
+                for i, line in enumerate(s_lines, start=start_line)
+            )
+            + "\n"
+        )
```

### Comparing `columbia-discord-bot-0.1.1/pyproject.toml` & `columbia-discord-bot-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "columbia-discord-bot"
 authors = [{name = "Matthew Wang", email = "mw3071@columbia.edu"}]
 description="A discord bot for Columbia University"
 readme = "README.md"
-version = "0.1.0"
+version = "0.2.1"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

