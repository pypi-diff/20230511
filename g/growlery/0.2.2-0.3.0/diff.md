# Comparing `tmp/growlery-0.2.2.tar.gz` & `tmp/growlery-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "growlery-0.2.2.tar", max compression
+gzip compressed data, was "growlery-0.3.0.tar", max compression
```

## Comparing `growlery-0.2.2.tar` & `growlery-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3398 2023-03-09 13:35:10.900723 growlery-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-03-09 13:35:10.904723 growlery-0.2.2/LICENSE
--rw-r--r--   0        0        0     6518 2023-03-09 13:35:10.904723 growlery-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-03-09 13:35:10.904723 growlery-0.2.2/growlery/__init__.py
--rw-r--r--   0        0        0      268 2023-03-09 13:35:10.904723 growlery-0.2.2/growlery/__main__.py
--rw-r--r--   0        0        0      106 2023-03-09 13:35:10.904723 growlery-0.2.2/growlery/cogs/__init__.py
--rw-r--r--   0        0        0     9234 2023-03-09 13:35:10.904723 growlery-0.2.2/growlery/cogs/hiscores.py
--rw-r--r--   0        0        0     3357 2023-03-09 13:35:10.904723 growlery-0.2.2/growlery/config.py
--rw-r--r--   0        0        0     1226 2023-03-09 13:35:10.904723 growlery-0.2.2/growlery/http_request.py
--rw-r--r--   0        0        0     1357 2023-03-09 13:35:10.904723 growlery-0.2.2/growlery/main.py
--rw-r--r--   0        0        0     6738 2023-03-09 13:35:10.904723 growlery-0.2.2/growlery/table.py
--rw-r--r--   0        0        0     3533 2023-03-09 13:35:10.904723 growlery-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     8537 1970-01-01 00:00:00.000000 growlery-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     4332 2023-05-11 17:59:18.913957 growlery-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-05-11 17:59:18.913957 growlery-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6728 2023-05-11 17:59:18.913957 growlery-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 17:59:18.913957 growlery-0.3.0/growlery/__init__.py
+-rw-r--r--   0        0        0      267 2023-05-11 17:59:18.913957 growlery-0.3.0/growlery/__main__.py
+-rw-r--r--   0        0        0      106 2023-05-11 17:59:18.913957 growlery-0.3.0/growlery/cogs/__init__.py
+-rw-r--r--   0        0        0    10432 2023-05-11 17:59:18.913957 growlery-0.3.0/growlery/cogs/hiscores.py
+-rw-r--r--   0        0        0     3403 2023-05-11 17:59:18.913957 growlery-0.3.0/growlery/config.py
+-rw-r--r--   0        0        0     1228 2023-05-11 17:59:18.913957 growlery-0.3.0/growlery/http_request.py
+-rw-r--r--   0        0        0     1301 2023-05-11 17:59:18.913957 growlery-0.3.0/growlery/main.py
+-rw-r--r--   0        0        0     9137 2023-05-11 17:59:18.913957 growlery-0.3.0/growlery/table.py
+-rw-r--r--   0        0        0     4762 2023-05-11 17:59:18.917957 growlery-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8792 1970-01-01 00:00:00.000000 growlery-0.3.0/PKG-INFO
```

### Comparing `growlery-0.2.2/CHANGELOG.md` & `growlery-0.3.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -46,33 +46,64 @@
 - Updated localisation files
 
 -->
 
 <!--
 _______________________________________________________________________________
 
-## [0.2.2] - 2023-03-09
+## [0.3.0] - 2023-05-11
 
-Added better instructions to `README.md`, and enhanced tests.
+`README.md` is now more up-to-date, the new Wilderness bosses are now in the
+list of bosses, and the project's linters were replaced with Ruff. The codebase
+has also been cleaned up somewhat as a result in order to pass the new linter
+guidelines.
 
 ### Added
 
-- Tests for HTTP requests
+- Added support for listing the new Wilderness bosses, fixing incorrect scores
+  for existing bosses.
 
 ### Changed
 
 - Updated `README.md` with clearer instructions for using the bot
 - Updated dependencies
-- Improved test coverage
 - Updated localisation files
 
+### Fixed
+
+- Boss hiscores are no longer broken
+
 -->
 
 _______________________________________________________________________________
 
+## [0.3.0] - 2023-05-11
+
+`README.md` is now more up-to-date, the new Wilderness bosses are now in the
+list of bosses, and the project's linters were replaced with Ruff. The codebase
+has also been cleaned up somewhat as a result in order to pass the new linter
+guidelines.
+
+### Added
+
+- Added support for listing the new Wilderness bosses, fixing incorrect scores
+  for existing bosses.
+
+### Changed
+
+- Updated `README.md` with clearer instructions for using the bot
+- Updated dependencies
+- Updated localisation files
+
+### Fixed
+
+- Boss hiscores are no longer broken
+
+_______________________________________________________________________________
+
 ## [0.2.2] - 2023-03-09
 
 Added better instructions to `README.md`, and enhanced tests.
 
 ### Added
 
 - Tests for HTTP requests
```

### Comparing `growlery-0.2.2/LICENSE` & `growlery-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `growlery-0.2.2/README.md` & `growlery-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,66 @@
 # Growlery - The Clan Quest OSRS Discord Bot
 
-![Stuff](./docs/assets/cq_logo_wide.png)
+![CQ Logo](./docs/assets/cq_logo_wide.png)
 
-Ever since the untimely demise of RuneInfo, there's been a lack of OSRS support in the Discord bot department. While RuneScape 3 has Elenora, it doesn't support OSRS.
-
-The Council of Elders looked about them and saw regression, not progress. The decision was made by the wisest: a new bot would be hardened and removed from the cycle. Its power would herald a new era.
+Ever since the untimely demise of RuneInfo, there's been a lack of OSRS support
+in the Discord bot department. While RuneScape 3 has Elenora, it doesn't
+support OSRS.
+
+The Council of Elders looked about them and saw regression, not progress. The
+decision was made by the wisest: a new bot would be hardened and removed from
+the cycle. Its power would herald a new era.
 
 | Type         | Badges |
 |--------------|---|
 | PyPI         | ![Python versions](https://img.shields.io/pypi/pyversions/growlery?logo=python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/growlery) ![Wheel](https://img.shields.io/pypi/wheel/growlery?logo=pypi) ![Downloads](https://img.shields.io/pypi/dm/growlery?logo=pypi) [![Version](https://img.shields.io/pypi/v/growlery)](https://pypi.org/project/growlery/) |
 | Tests        | [![codecov](https://codecov.io/gh/Diapolo10/clan-quest-osrs-discord-bot/branch/main/graph/badge.svg?token=N3JOBzERqP)](https://codecov.io/gh/Diapolo10/clan-quest-osrs-discord-bot) ![Unit tests](https://github.com/diapolo10/clan-quest-osrs-discord-bot/workflows/Unit%20tests/badge.svg) ![Pylint](https://github.com/diapolo10/clan-quest-osrs-discord-bot/workflows/Pylint/badge.svg) ![Flake8](https://github.com/diapolo10/clan-quest-osrs-discord-bot/workflows/Flake8/badge.svg) ![Deploy to PyPI](https://github.com/diapolo10/clan-quest-osrs-discord-bot/workflows/Deploy%20to%20PyPI/badge.svg) |
 | Activity     | ![GitHub contributors](https://img.shields.io/github/contributors/diapolo10/clan-quest-osrs-discord-bot) ![Last commit](https://img.shields.io/github/last-commit/diapolo10/clan-quest-osrs-discord-bot?logo=github) ![GitHub all releases](https://img.shields.io/github/downloads/diapolo10/clan-quest-osrs-discord-bot/total?logo=github) ![GitHub issues](https://img.shields.io/github/issues/diapolo10/clan-quest-osrs-discord-bot) ![GitHub closed issues](https://img.shields.io/github/issues-closed/diapolo10/clan-quest-osrs-discord-bot) ![GitHub pull requests](https://img.shields.io/github/issues-pr/diapolo10/clan-quest-osrs-discord-bot) ![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/diapolo10/clan-quest-osrs-discord-bot) |
 | QA           | [![CodeFactor](https://www.codefactor.io/repository/github/diapolo10/clan-quest-osrs-discord-bot/badge?logo=codefactor)](https://www.codefactor.io/repository/github/diapolo10/clan-quest-osrs-discord-bot) [![Rating](https://img.shields.io/librariesio/sourcerank/pypi/growlery)](https://libraries.io/github/Diapolo10/clan-quest-osrs-discord-bot/sourcerank) |
 | Other        | [![License](https://img.shields.io/github/license/diapolo10/clan-quest-osrs-discord-bot)](https://opensource.org/licenses/MIT) ![Repository size](https://img.shields.io/github/repo-size/diapolo10/clan-quest-osrs-discord-bot?logo=github) ![Code size](https://img.shields.io/github/languages/code-size/diapolo10/clan-quest-osrs-discord-bot?logo=github) ![Lines of code](https://img.shields.io/tokei/lines/github/diapolo10/clan-quest-osrs-discord-bot?logo=github) |
 
 ## Installation
 
-The project is currently as source code, via PyPI
+The project is currently available both as a source release, and as a wheel,
+via PyPI
 
 ```sh
 pip install growlery
 ```
 
 and as GitHub releases.
 
-Installation requires Python 3.10 or newer. Platform-independent.
+Installation requires Python 3.10 or newer. The project is platform-independent
+and should work fine on all major operating systems. Each release has been
+automatically tested to run on Windows, Ubuntu, and Mac OS.
 
-To run the bot, either manually execute `growlery/main.py` or, for future releases, you can attempt to run it via
+To run the bot, either manually execute `growlery/main.py` or, alternatively,
+you may run it as an executable package
 
 ```sh
 python -m growlery
 ```
 
-in case the functionality has been implemented.
+as long as the needed environmental variables have been set.
 
 ## Usage
 
-The bot expects a Discord authentication token to be given via an environmental variable called `DISCORD_TOKEN`. It can alternatively be provided by writing it to a file called `.env` and placing that inside the `growlery` folder. An example file could look like this:
+The bot expects a Discord authentication token to be given via an environmental
+variable called `DISCORD_TOKEN`. It can alternatively be provided by writing it
+to a file called `.env` and placing that inside the `growlery` folder. An
+example file could look like this:
 
 ```txt
 DISCORD_TOKEN=MzA5NzY3Njg0NzcwMTg1NzIy.V89mA1.9R8aoZ4vwhCUbIEd20BtzkVquLG
 ```
 
 Note that the example token is just a dummy.
 
-If you need to generate a token, go to the [Discord developers page][Discord Developers] and create a new bot. [This tutorial][Discord bot tutorial] may prove useful.
+If you need to generate a token, go to the [Discord developers page][Discord Developers]
+and create a new bot. [This tutorial][Discord bot tutorial] may prove useful.
 
 The only required permissions are:
 
 - Read Messages/View Channels
 - Send Messages
 - Use Slash Commands
 
@@ -87,17 +99,19 @@
 - [x] Fetching boss hiscores
 - [ ] Player comparisons
 - [ ] Storing usernames for Discord IDs
 - [ ] Support for the new Slash Commands
 
 ## Caught a Bug?
 
-1. [Fork][Forking a repository] this repository to your own GitHub account and then [clone][Cloning a repository] it to your local device
+1. [Fork][Forking a repository] this repository to your own GitHub account and
+   then [clone][Cloning a repository] it to your local device
 2. Install `poetry` (if it isn't already installed)
-3. Run `poetry install` in the project directory. This fetches development dependencies like `pytest` and sets up everything for you to start debugging
+3. Run `poetry install` in the project directory. This fetches development
+   dependencies like `pytest` and sets up everything for you to start debugging
 
 As always, you can run the tests using: `poetry run pytest`
 
 [Discord Developers]: https://discord.com/developers
 [Discord bot tutorial]: https://www.freecodecamp.org/news/create-a-discord-bot-with-python/
 [Forking a repository]: https://help.github.com/articles/fork-a-repo/
 [Cloning a repository]: https://help.github.com/articles/cloning-a-repository/
```

### Comparing `growlery-0.2.2/growlery/cogs/hiscores.py` & `growlery-0.3.0/growlery/cogs/hiscores.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,209 +1,226 @@
 """Implements commands for hiscores"""
 
+from __future__ import annotations
+
 import logging
 from http import HTTPStatus
+from typing import TYPE_CHECKING
 
 from discord.ext import commands
+from reactionmenu import ViewButton, ViewMenu  # type: ignore[import]
+
+if TYPE_CHECKING:
+    from discord.message import Message
 
 from growlery.config import (
+    RUNESCAPE_HISCORES_LITE_URL,
     AccountType,
     AccountTypeName,
-    RUNESCAPE_HISCORES_LITE_URL,
 )
 from growlery.http_request import fetch_page_content
-from growlery.table import SkillsTable, MinigamesTable, BossesTable
+from growlery.table import BossesTable, MinigamesTable, SkillsTable
 
 logger = logging.getLogger(__name__)
 
 
 class Hiscores(commands.Cog):  # pylint: disable=R0904
     """Hiscores commands"""
 
     @commands.command('07hs')
-    async def default_hiscores(self, ctx: commands.Context, *, username: str | None = None):
+    async def default_hiscores(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches default hiscores for the given username"""
 
         await self.reply_with_hiscores(ctx, username, AccountType.NORMAL, AccountTypeName.NORMAL)
 
     @commands.command('07hs-im')
-    async def ironman_hiscores(self, ctx: commands.Context, *, username: str | None = None):
+    async def ironman_hiscores(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches ironman hiscores for the given username"""
 
         await self.reply_with_hiscores(ctx, username, AccountType.IRONMAN, AccountTypeName.IRONMAN)
 
     @commands.command('07hs-hcim')
-    async def hardcore_ironman_hiscores(self, ctx: commands.Context, *, username: str | None = None):
+    async def hardcore_ironman_hiscores(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches hardcore ironman hiscores for the given username"""
 
         await self.reply_with_hiscores(ctx, username, AccountType.HARDCORE_IRONMAN, AccountTypeName.HARDCORE_IRONMAN)
 
     @commands.command('07hs-uim')
-    async def ultimate_ironman_hiscores(self, ctx: commands.Context, *, username: str | None = None):
+    async def ultimate_ironman_hiscores(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches ultimate ironman hiscores for the given username"""
 
         await self.reply_with_hiscores(ctx, username, AccountType.ULTIMATE_IRONMAN, AccountTypeName.ULTIMATE_IRONMAN)
 
     @commands.command('07hs-skiller')
-    async def skiller_hiscores(self, ctx: commands.Context, *, username: str | None = None):
+    async def skiller_hiscores(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches skiller hiscores for the given username"""
 
         await self.reply_with_hiscores(ctx, username, AccountType.SKILLER, AccountTypeName.SKILLER)
 
     @commands.command('07hs-def')
-    async def defence_pure_hiscores(self, ctx: commands.Context, *, username: str | None = None):
+    async def defence_pure_hiscores(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches 1 Defence hiscores for the given username"""
 
         await self.reply_with_hiscores(ctx, username, AccountType.DEFENCE_PURE, AccountTypeName.DEFENCE_PURE)
 
     @commands.command('07hs-minigames')
-    async def default_minigames(self, ctx: commands.Context, *, username: str | None = None):
+    async def default_minigames(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches default minigame hiscores for the given username"""
 
         await self.reply_with_minigames(ctx, username, AccountType.NORMAL, AccountTypeName.NORMAL)
 
     @commands.command('07hs-im-minigames')
-    async def ironman_minigames(self, ctx: commands.Context, *, username: str | None = None):
+    async def ironman_minigames(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches ironman minigame hiscores for the given username"""
 
         await self.reply_with_minigames(ctx, username, AccountType.IRONMAN, AccountTypeName.IRONMAN)
 
     @commands.command('07hs-hcim-minigames')
-    async def hardcore_ironman_minigames(self, ctx: commands.Context, *, username: str | None = None):
+    async def hardcore_ironman_minigames(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches hardcore ironman minigame hiscores for the given username"""
 
         await self.reply_with_minigames(ctx, username, AccountType.HARDCORE_IRONMAN, AccountTypeName.HARDCORE_IRONMAN)
 
     @commands.command('07hs-uim-minigames')
-    async def ultimate_ironman_minigames(self, ctx: commands.Context, *, username: str | None = None):
+    async def ultimate_ironman_minigames(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches ultimate ironman minigame hiscores for the given username"""
 
         await self.reply_with_minigames(ctx, username, AccountType.ULTIMATE_IRONMAN, AccountTypeName.ULTIMATE_IRONMAN)
 
     @commands.command('07hs-skiller-minigames')
-    async def skiller_minigames(self, ctx: commands.Context, *, username: str | None = None):
+    async def skiller_minigames(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches skiller minigame hiscores for the given username"""
 
         await self.reply_with_minigames(ctx, username, AccountType.SKILLER, AccountTypeName.SKILLER)
 
     @commands.command('07hs-def-minigames')
-    async def defence_pure_minigames(self, ctx: commands.Context, *, username: str | None = None):
+    async def defence_pure_minigames(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches 1 Defence minigame hiscores for the given username"""
 
         await self.reply_with_minigames(ctx, username, AccountType.DEFENCE_PURE, AccountTypeName.DEFENCE_PURE)
 
     @commands.command('07hs-bosses')
-    async def default_bosses(self, ctx: commands.Context, *, username: str | None = None):
+    async def default_bosses(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches default boss hiscores for the given username"""
 
         await self.reply_with_bosses(ctx, username, AccountType.NORMAL, AccountTypeName.NORMAL)
 
     @commands.command('07hs-im-bosses')
-    async def ironman_bosses(self, ctx: commands.Context, *, username: str | None = None):
+    async def ironman_bosses(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches ironman boss hiscores for the given username"""
 
         await self.reply_with_bosses(ctx, username, AccountType.IRONMAN, AccountTypeName.IRONMAN)
 
     @commands.command('07hs-hcim-bosses')
-    async def hardcore_ironman_bosses(self, ctx: commands.Context, *, username: str | None = None):
+    async def hardcore_ironman_bosses(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches hardcore ironman boss hiscores for the given username"""
 
         await self.reply_with_bosses(ctx, username, AccountType.HARDCORE_IRONMAN, AccountTypeName.HARDCORE_IRONMAN)
 
     @commands.command('07hs-uim-bosses')
-    async def ultimate_ironman_bosses(self, ctx: commands.Context, *, username: str | None = None):
+    async def ultimate_ironman_bosses(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches ultimate ironman boss hiscores for the given username"""
 
         await self.reply_with_bosses(ctx, username, AccountType.ULTIMATE_IRONMAN, AccountTypeName.ULTIMATE_IRONMAN)
 
     @commands.command('07hs-skiller-bosses')
-    async def skiller_bosses(self, ctx: commands.Context, *, username: str | None = None):
+    async def skiller_bosses(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches skiller boss hiscores for the given username"""
 
         await self.reply_with_bosses(ctx, username, AccountType.SKILLER, AccountTypeName.SKILLER)
 
     @commands.command('07hs-def-bosses')
-    async def defence_pure_bosses(self, ctx: commands.Context, *, username: str | None = None):
+    async def defence_pure_bosses(self: Hiscores, ctx: commands.Context, *, username: str | None = None) -> None:
         """Fetches 1 Defence boss hiscores for the given username"""
 
         await self.reply_with_bosses(ctx, username, AccountType.DEFENCE_PURE, AccountTypeName.DEFENCE_PURE)
 
     @classmethod
-    async def reply_with_hiscores(cls,
+    async def reply_with_hiscores(cls: type[Hiscores],
                                   ctx: commands.Context,
                                   username: str | None,
                                   account_type: AccountType,
-                                  account_type_name: AccountTypeName):
+                                  account_type_name: AccountTypeName) -> Message:
         """Replies to the chat with the given username's hiscores"""
 
         result = "Hiscores not found."
 
         if username is None:
             logger.warning(result := "Username assigning to Discord profile not implemented yet.")
             return await ctx.send(result)
 
         hiscores = await cls._fetch_hiscores(username, account_type)
         if hiscores:
-            result = SkillsTable(username, account_type, account_type_name, hiscores).render_table()
+            result = SkillsTable(username, account_type, account_type_name, hiscores).render_table()  # type: ignore[assignment]
 
-        await ctx.send(result)
+        return await ctx.send(result)
 
     @classmethod
-    async def reply_with_minigames(cls,
+    async def reply_with_minigames(cls: type[Hiscores],
                                    ctx: commands.Context,
                                    username: str | None,
                                    account_type: AccountType,
-                                   account_type_name: AccountTypeName):
+                                   account_type_name: AccountTypeName) -> Message:
         """Replies to the chat with the given username's hiscores"""
 
         result = "Hiscores not found."
 
         if username is None:
             logger.warning(result := "Username assigning to Discord profile not implemented yet.")
             return await ctx.send(result)
 
         hiscores = await cls._fetch_hiscores(username, account_type)
         if hiscores:
-            result = MinigamesTable(username, account_type, account_type_name, hiscores).render_table()
+            result = MinigamesTable(username, account_type, account_type_name, hiscores).render_table()  # type: ignore[assignment]
 
-        await ctx.send(result)
+        return await ctx.send(result)
 
     @classmethod
-    async def reply_with_bosses(cls,
+    async def reply_with_bosses(cls: type[Hiscores],
                                 ctx: commands.Context,
                                 username: str | None,
                                 account_type: AccountType,
-                                account_type_name: AccountTypeName):
+                                account_type_name: AccountTypeName) -> Message | None:
         """Replies to the chat with the given username's hiscores"""
 
         result = "Hiscores not found."
 
         if username is None:
             logger.warning(result := "Username assigning to Discord profile not implemented yet.")
             return await ctx.send(result)
 
         hiscores = await cls._fetch_hiscores(username, account_type)
         if hiscores:
-            result = BossesTable(username, account_type, account_type_name, hiscores).render_table()
+            menu = ViewMenu(ctx, menu_type=ViewMenu.TypeText)
+            result = BossesTable(username, account_type, account_type_name, hiscores).render_table()  # type: ignore[assignment]
+            if isinstance(result, str):
+                menu.add_page(content=result)
+            else:
+                for page in result:
+                    menu.add_page(content=page)
+            menu.add_button(ViewButton.go_to_first_page())
+            menu.add_button(ViewButton.back())
+            menu.add_button(ViewButton.next())
+            menu.add_button(ViewButton.go_to_last_page())
+            return await menu.start()
 
-        await ctx.send(result)
+        return await ctx.send(result)
 
     @staticmethod
     async def _fetch_hiscores(username: str, account_type: AccountType) -> list[list[str]] | None:
         """Handles fetching the hiscores for RuneScape accounts"""
 
         url: str = RUNESCAPE_HISCORES_LITE_URL.format(
             hiscores='_oldschool',
             gamemode=account_type,
-            player_name=username
+            player_name=username,
         )
         status_messages = {
             HTTPStatus.NOT_FOUND: "Could not find player hiscores",
         }
 
         csv_data = await fetch_page_content(url=url, status_message_override=status_messages)
 
-        hiscores = [
-            row.split(',') for row in csv_data.strip().splitlines()
+        return [
+            row.split(',')
+            for row in csv_data.strip().splitlines()
         ]
-
-        return hiscores
```

### Comparing `growlery-0.2.2/growlery/config.py` & `growlery-0.3.0/growlery/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import os
 from enum import Enum
 from pathlib import Path
 
 from dotenv import load_dotenv
 
-
 PROJECT_DIR = Path(__file__).parent
 ROOT_DIR = PROJECT_DIR.parent
 DOCS_DIR = ROOT_DIR / 'docs'
 CODE_EXAMPLES = DOCS_DIR / 'example_code'
 ENV_FILE = PROJECT_DIR / '.env'
 
 # Loads environmental variables from an .env-file
@@ -72,17 +71,19 @@
     'Soul Wars Zeal',
     'Rifts closed',
 )
 
 BOSS_NAMES = (
     'Abyssal Sire',
     'Alchemical Hydra',
+    'Artio',
     'Barrows Chests',
     'Bryophyta',
     'Callisto',
+    'Calvar\'ion',
     'Cerberus',
     'Chambers of Xeric',
     'Chambers of Xeric: Challenge Mode',
     'Chaos Elemental',
     'Chaos Fanatic',
     'Commander Zilyana',
     'Corporeal Beast',
@@ -105,14 +106,15 @@
     'Nightmare',
     'Phosani\'s Nightmare',
     'Obor',
     'Phantom Muspah',
     'Sarachnis',
     'Scorpia',
     'Skotizo',
+    'Spindel',
     'Tempoross',
     'The Gauntlet',
     'The Corrupted Gauntlet',
     'Theatre of Blood',
     'Theatre of Blood: Hard Mode',
     'Thermonuclear Smoke Devil',
     'Tombs of Amascut',
```

### Comparing `growlery-0.2.2/growlery/http_request.py` & `growlery-0.3.0/growlery/http_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                 if request.status == HTTPStatus.OK:
                     result = await request.text()
 
                 elif request.status in status_message:
                     logger.error(
                         status_message.get(
                             HTTPStatus(request.status),
-                            f"[{request.status}] - {request.reason or 'Unidentified problem'}"
-                        )
+                            f"[{request.status}] - {request.reason or 'Unidentified problem'}",
+                        ),
                     )
 
         except aiohttp.ClientConnectionError as err:
             logger.error("Connection error: %s", err)
 
     return result
```

### Comparing `growlery-0.2.2/PKG-INFO` & `growlery-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: growlery
-Version: 0.2.2
+Version: 0.3.0
 Summary: An OSRS Discord bot for Clan Quest.
 Home-page: https://pypi.org/project/clan-quest-osrs-discord-bot/
 License: MIT
 Keywords: python3,discord,runescape,osrs,oldschool
 Author: Lari Liuhamo
 Author-email: lari.liuhamo+pypi@gmail.com
 Maintainer: Lari Liuhamo
@@ -29,69 +29,82 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: discord.py (>=2.2.2,<3.0.0)
+Requires-Dist: discord.py (>=2.2.3,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: reactionmenu (>=3.1.3,<4.0.0)
 Project-URL: Changelog, https://github.com/Diapolo10/clan-quest-osrs-discord-bot/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/Diapolo10/clan-quest-osrs-discord-bot/tree/main/docs
 Project-URL: Repository, https://github.com/Diapolo10/clan-quest-osrs-discord-bot
 Project-URL: Tracker, https://github.com/Diapolo10/clan-quest-osrs-discord-bot/issues
 Description-Content-Type: text/markdown
 
 # Growlery - The Clan Quest OSRS Discord Bot
 
-![Stuff](./docs/assets/cq_logo_wide.png)
+![CQ Logo](./docs/assets/cq_logo_wide.png)
 
-Ever since the untimely demise of RuneInfo, there's been a lack of OSRS support in the Discord bot department. While RuneScape 3 has Elenora, it doesn't support OSRS.
-
-The Council of Elders looked about them and saw regression, not progress. The decision was made by the wisest: a new bot would be hardened and removed from the cycle. Its power would herald a new era.
+Ever since the untimely demise of RuneInfo, there's been a lack of OSRS support
+in the Discord bot department. While RuneScape 3 has Elenora, it doesn't
+support OSRS.
+
+The Council of Elders looked about them and saw regression, not progress. The
+decision was made by the wisest: a new bot would be hardened and removed from
+the cycle. Its power would herald a new era.
 
 | Type         | Badges |
 |--------------|---|
 | PyPI         | ![Python versions](https://img.shields.io/pypi/pyversions/growlery?logo=python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/growlery) ![Wheel](https://img.shields.io/pypi/wheel/growlery?logo=pypi) ![Downloads](https://img.shields.io/pypi/dm/growlery?logo=pypi) [![Version](https://img.shields.io/pypi/v/growlery)](https://pypi.org/project/growlery/) |
 | Tests        | [![codecov](https://codecov.io/gh/Diapolo10/clan-quest-osrs-discord-bot/branch/main/graph/badge.svg?token=N3JOBzERqP)](https://codecov.io/gh/Diapolo10/clan-quest-osrs-discord-bot) ![Unit tests](https://github.com/diapolo10/clan-quest-osrs-discord-bot/workflows/Unit%20tests/badge.svg) ![Pylint](https://github.com/diapolo10/clan-quest-osrs-discord-bot/workflows/Pylint/badge.svg) ![Flake8](https://github.com/diapolo10/clan-quest-osrs-discord-bot/workflows/Flake8/badge.svg) ![Deploy to PyPI](https://github.com/diapolo10/clan-quest-osrs-discord-bot/workflows/Deploy%20to%20PyPI/badge.svg) |
 | Activity     | ![GitHub contributors](https://img.shields.io/github/contributors/diapolo10/clan-quest-osrs-discord-bot) ![Last commit](https://img.shields.io/github/last-commit/diapolo10/clan-quest-osrs-discord-bot?logo=github) ![GitHub all releases](https://img.shields.io/github/downloads/diapolo10/clan-quest-osrs-discord-bot/total?logo=github) ![GitHub issues](https://img.shields.io/github/issues/diapolo10/clan-quest-osrs-discord-bot) ![GitHub closed issues](https://img.shields.io/github/issues-closed/diapolo10/clan-quest-osrs-discord-bot) ![GitHub pull requests](https://img.shields.io/github/issues-pr/diapolo10/clan-quest-osrs-discord-bot) ![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/diapolo10/clan-quest-osrs-discord-bot) |
 | QA           | [![CodeFactor](https://www.codefactor.io/repository/github/diapolo10/clan-quest-osrs-discord-bot/badge?logo=codefactor)](https://www.codefactor.io/repository/github/diapolo10/clan-quest-osrs-discord-bot) [![Rating](https://img.shields.io/librariesio/sourcerank/pypi/growlery)](https://libraries.io/github/Diapolo10/clan-quest-osrs-discord-bot/sourcerank) |
 | Other        | [![License](https://img.shields.io/github/license/diapolo10/clan-quest-osrs-discord-bot)](https://opensource.org/licenses/MIT) ![Repository size](https://img.shields.io/github/repo-size/diapolo10/clan-quest-osrs-discord-bot?logo=github) ![Code size](https://img.shields.io/github/languages/code-size/diapolo10/clan-quest-osrs-discord-bot?logo=github) ![Lines of code](https://img.shields.io/tokei/lines/github/diapolo10/clan-quest-osrs-discord-bot?logo=github) |
 
 ## Installation
 
-The project is currently as source code, via PyPI
+The project is currently available both as a source release, and as a wheel,
+via PyPI
 
 ```sh
 pip install growlery
 ```
 
 and as GitHub releases.
 
-Installation requires Python 3.10 or newer. Platform-independent.
+Installation requires Python 3.10 or newer. The project is platform-independent
+and should work fine on all major operating systems. Each release has been
+automatically tested to run on Windows, Ubuntu, and Mac OS.
 
-To run the bot, either manually execute `growlery/main.py` or, for future releases, you can attempt to run it via
+To run the bot, either manually execute `growlery/main.py` or, alternatively,
+you may run it as an executable package
 
 ```sh
 python -m growlery
 ```
 
-in case the functionality has been implemented.
+as long as the needed environmental variables have been set.
 
 ## Usage
 
-The bot expects a Discord authentication token to be given via an environmental variable called `DISCORD_TOKEN`. It can alternatively be provided by writing it to a file called `.env` and placing that inside the `growlery` folder. An example file could look like this:
+The bot expects a Discord authentication token to be given via an environmental
+variable called `DISCORD_TOKEN`. It can alternatively be provided by writing it
+to a file called `.env` and placing that inside the `growlery` folder. An
+example file could look like this:
 
 ```txt
 DISCORD_TOKEN=MzA5NzY3Njg0NzcwMTg1NzIy.V89mA1.9R8aoZ4vwhCUbIEd20BtzkVquLG
 ```
 
 Note that the example token is just a dummy.
 
-If you need to generate a token, go to the [Discord developers page][Discord Developers] and create a new bot. [This tutorial][Discord bot tutorial] may prove useful.
+If you need to generate a token, go to the [Discord developers page][Discord Developers]
+and create a new bot. [This tutorial][Discord bot tutorial] may prove useful.
 
 The only required permissions are:
 
 - Read Messages/View Channels
 - Send Messages
 - Use Slash Commands
 
@@ -130,17 +143,19 @@
 - [x] Fetching boss hiscores
 - [ ] Player comparisons
 - [ ] Storing usernames for Discord IDs
 - [ ] Support for the new Slash Commands
 
 ## Caught a Bug?
 
-1. [Fork][Forking a repository] this repository to your own GitHub account and then [clone][Cloning a repository] it to your local device
+1. [Fork][Forking a repository] this repository to your own GitHub account and
+   then [clone][Cloning a repository] it to your local device
 2. Install `poetry` (if it isn't already installed)
-3. Run `poetry install` in the project directory. This fetches development dependencies like `pytest` and sets up everything for you to start debugging
+3. Run `poetry install` in the project directory. This fetches development
+   dependencies like `pytest` and sets up everything for you to start debugging
 
 As always, you can run the tests using: `poetry run pytest`
 
 [Discord Developers]: https://discord.com/developers
 [Discord bot tutorial]: https://www.freecodecamp.org/news/create-a-discord-bot-with-python/
 [Forking a repository]: https://help.github.com/articles/fork-a-repo/
 [Cloning a repository]: https://help.github.com/articles/cloning-a-repository/
```

