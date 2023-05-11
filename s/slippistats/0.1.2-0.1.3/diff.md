# Comparing `tmp/slippistats-0.1.2.tar.gz` & `tmp/slippistats-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slippistats-0.1.2.tar", last modified: Thu May  4 00:44:18 2023, max compression
+gzip compressed data, was "slippistats-0.1.3.tar", last modified: Thu May 11 07:52:19 2023, max compression
```

## Comparing `slippistats-0.1.2.tar` & `slippistats-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 00:44:18.398912 slippistats-0.1.2/
--rw-rw-rw-   0        0        0     1084 2023-04-28 03:43:11.000000 slippistats-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     5002 2023-05-04 00:44:18.397412 slippistats-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3271 2023-05-02 01:59:46.000000 slippistats-0.1.2/README.md
--rw-rw-rw-   0        0        0      605 2023-05-04 00:43:55.000000 slippistats-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 00:44:18.398912 slippistats-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      728 2023-04-25 21:47:20.000000 slippistats-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 00:44:18.329900 slippistats-0.1.2/slippistats/
--rw-rw-rw-   0        0        0      315 2023-04-28 04:43:30.000000 slippistats-0.1.2/slippistats/__init__.py
--rw-rw-rw-   0        0        0     2912 2023-04-25 21:47:20.000000 slippistats-0.1.2/slippistats/controller.py
-drwxrwxrwx   0        0        0        0 2023-05-04 00:44:18.371408 slippistats-0.1.2/slippistats/enums/
--rw-rw-rw-   0        0        0      361 2023-04-28 04:10:10.000000 slippistats-0.1.2/slippistats/enums/__init__.py
--rw-rw-rw-   0        0        0     2739 2023-04-25 21:47:21.000000 slippistats-0.1.2/slippistats/enums/attack.py
--rw-rw-rw-   0        0        0     5670 2023-04-25 21:47:21.000000 slippistats-0.1.2/slippistats/enums/character.py
--rw-rw-rw-   0        0        0     6161 2023-04-25 21:47:21.000000 slippistats-0.1.2/slippistats/enums/item.py
--rw-rw-rw-   0        0        0     3309 2023-04-26 00:48:25.000000 slippistats-0.1.2/slippistats/enums/stage.py
--rw-rw-rw-   0        0        0    51534 2023-05-04 00:42:26.000000 slippistats-0.1.2/slippistats/enums/state.py
--rw-rw-rw-   0        0        0    61331 2023-05-04 00:42:26.000000 slippistats-0.1.2/slippistats/event.py
--rw-rw-rw-   0        0        0     2719 2023-04-25 21:47:21.000000 slippistats-0.1.2/slippistats/game.py
--rw-rw-rw-   0        0        0      394 2023-04-25 21:47:21.000000 slippistats-0.1.2/slippistats/log.py
--rw-rw-rw-   0        0        0     5691 2023-04-25 21:47:21.000000 slippistats-0.1.2/slippistats/metadata.py
--rw-rw-rw-   0        0        0    12567 2023-05-04 00:41:23.000000 slippistats-0.1.2/slippistats/parse.py
-drwxrwxrwx   0        0        0        0 2023-05-04 00:44:18.386410 slippistats-0.1.2/slippistats/stats/
--rw-rw-rw-   0        0        0      153 2023-04-25 21:47:21.000000 slippistats-0.1.2/slippistats/stats/__init__.py
--rw-rw-rw-   0        0        0    13781 2023-05-04 00:41:23.000000 slippistats-0.1.2/slippistats/stats/combo_computer.py
--rw-rw-rw-   0        0        0    18117 2023-05-04 00:42:26.000000 slippistats-0.1.2/slippistats/stats/common.py
--rw-rw-rw-   0        0        0    11145 2023-04-25 21:47:23.000000 slippistats-0.1.2/slippistats/stats/computer.py
--rw-rw-rw-   0        0        0    33926 2023-04-26 01:15:54.000000 slippistats-0.1.2/slippistats/stats/stat_types.py
--rw-rw-rw-   0        0        0    38543 2023-05-04 00:42:26.000000 slippistats-0.1.2/slippistats/stats/stats_computer.py
--rw-rw-rw-   0        0        0     3417 2023-04-25 21:47:21.000000 slippistats-0.1.2/slippistats/util.py
-drwxrwxrwx   0        0        0        0 2023-05-04 00:44:18.356905 slippistats-0.1.2/slippistats.egg-info/
--rw-rw-rw-   0        0        0     5002 2023-05-04 00:44:18.000000 slippistats-0.1.2/slippistats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      793 2023-05-04 00:44:18.000000 slippistats-0.1.2/slippistats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 00:44:18.000000 slippistats-0.1.2/slippistats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-04 00:44:18.000000 slippistats-0.1.2/slippistats.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-04 00:44:18.000000 slippistats-0.1.2/slippistats.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 00:44:18.392911 slippistats-0.1.2/test/
--rw-rw-rw-   0        0        0        0 2022-12-29 08:44:12.000000 slippistats-0.1.2/test/__init__.py
--rw-rw-rw-   0        0        0    16926 2023-05-04 00:42:26.000000 slippistats-0.1.2/test/replays_test.py
+drwxrwxrwx   0        0        0        0 2023-05-11 07:52:19.064430 slippistats-0.1.3/
+-rw-rw-rw-   0        0        0     1084 2023-04-28 03:43:11.000000 slippistats-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     4929 2023-05-11 07:52:19.063432 slippistats-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3271 2023-05-02 01:59:46.000000 slippistats-0.1.3/README.md
+-rw-rw-rw-   0        0        0      660 2023-05-11 07:51:57.000000 slippistats-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 07:52:19.064430 slippistats-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 07:52:18.995418 slippistats-0.1.3/slippistats/
+-rw-rw-rw-   0        0        0      315 2023-04-28 04:43:30.000000 slippistats-0.1.3/slippistats/__init__.py
+-rw-rw-rw-   0        0        0     2912 2023-04-25 21:47:20.000000 slippistats-0.1.3/slippistats/controller.py
+drwxrwxrwx   0        0        0        0 2023-05-11 07:52:19.041427 slippistats-0.1.3/slippistats/enums/
+-rw-rw-rw-   0        0        0      361 2023-04-28 04:10:10.000000 slippistats-0.1.3/slippistats/enums/__init__.py
+-rw-rw-rw-   0        0        0     2739 2023-04-25 21:47:21.000000 slippistats-0.1.3/slippistats/enums/attack.py
+-rw-rw-rw-   0        0        0     5670 2023-04-25 21:47:21.000000 slippistats-0.1.3/slippistats/enums/character.py
+-rw-rw-rw-   0        0        0     6161 2023-04-25 21:47:21.000000 slippistats-0.1.3/slippistats/enums/item.py
+-rw-rw-rw-   0        0        0     3375 2023-05-11 05:52:29.000000 slippistats-0.1.3/slippistats/enums/stage.py
+-rw-rw-rw-   0        0        0    51205 2023-05-11 05:52:29.000000 slippistats-0.1.3/slippistats/enums/state.py
+-rw-rw-rw-   0        0        0    61331 2023-05-04 00:42:26.000000 slippistats-0.1.3/slippistats/event.py
+-rw-rw-rw-   0        0        0     2719 2023-04-25 21:47:21.000000 slippistats-0.1.3/slippistats/game.py
+-rw-rw-rw-   0        0        0      394 2023-04-25 21:47:21.000000 slippistats-0.1.3/slippistats/log.py
+-rw-rw-rw-   0        0        0     5691 2023-04-25 21:47:21.000000 slippistats-0.1.3/slippistats/metadata.py
+-rw-rw-rw-   0        0        0    12567 2023-05-04 00:41:23.000000 slippistats-0.1.3/slippistats/parse.py
+drwxrwxrwx   0        0        0        0 2023-05-11 07:52:19.055929 slippistats-0.1.3/slippistats/stats/
+-rw-rw-rw-   0        0        0      153 2023-04-25 21:47:21.000000 slippistats-0.1.3/slippistats/stats/__init__.py
+-rw-rw-rw-   0        0        0    13781 2023-05-04 00:41:23.000000 slippistats-0.1.3/slippistats/stats/combo_computer.py
+-rw-rw-rw-   0        0        0    18117 2023-05-04 00:42:26.000000 slippistats-0.1.3/slippistats/stats/common.py
+-rw-rw-rw-   0        0        0    12261 2023-05-11 05:52:29.000000 slippistats-0.1.3/slippistats/stats/computer.py
+-rw-rw-rw-   0        0        0    34250 2023-05-11 06:31:53.000000 slippistats-0.1.3/slippistats/stats/stat_types.py
+-rw-rw-rw-   0        0        0    38420 2023-05-11 05:52:29.000000 slippistats-0.1.3/slippistats/stats/stats_computer.py
+-rw-rw-rw-   0        0        0     3417 2023-04-25 21:47:21.000000 slippistats-0.1.3/slippistats/util.py
+drwxrwxrwx   0        0        0        0 2023-05-11 07:52:19.027924 slippistats-0.1.3/slippistats.egg-info/
+-rw-rw-rw-   0        0        0     4929 2023-05-11 07:52:18.000000 slippistats-0.1.3/slippistats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2023-05-11 07:52:18.000000 slippistats-0.1.3/slippistats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 07:52:18.000000 slippistats-0.1.3/slippistats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-11 07:52:18.000000 slippistats-0.1.3/slippistats.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-11 07:52:18.000000 slippistats-0.1.3/slippistats.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 07:52:19.059930 slippistats-0.1.3/test/
+-rw-rw-rw-   0        0        0        0 2022-12-29 08:44:12.000000 slippistats-0.1.3/test/__init__.py
+-rw-rw-rw-   0        0        0    16926 2023-05-04 00:42:26.000000 slippistats-0.1.3/test/replays_test.py
```

### Comparing `slippistats-0.1.2/LICENSE.txt` & `slippistats-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.2/PKG-INFO` & `slippistats-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: slippistats
-Version: 0.1.2
+Version: 0.1.3
 Summary: Stats library for SSBM replay files
-Home-page: https://github.com/Walnut356/py-slippi-stats
-Author: Walnut
 Author-email: Walnut356 <walnut356@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 melkor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `slippistats-0.1.2/README.md` & `slippistats-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.2/pyproject.toml` & `slippistats-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 00000050: 6122 0d0a 0d0a 5b70 726f 6a65 6374 5d0d  a"....[project].
 00000060: 0a6e 616d 6520 3d20 2273 6c69 7070 6973  .name = "slippis
 00000070: 7461 7473 220d 0a61 7574 686f 7273 203d  tats"..authors =
 00000080: 205b 0d0a 2020 2020 7b6e 616d 6520 3d20   [..    {name = 
 00000090: 2257 616c 6e75 7433 3536 222c 2065 6d61  "Walnut356", ema
 000000a0: 696c 203d 2022 7761 6c6e 7574 3335 3640  il = "walnut356@
 000000b0: 676d 6169 6c2e 636f 6d22 7d0d 0a5d 0d0a  gmail.com"}..]..
-000000c0: 7665 7273 696f 6e20 3d20 2230 2e31 2e32  version = "0.1.2
+000000c0: 7665 7273 696f 6e20 3d20 2230 2e31 2e33  version = "0.1.3
 000000d0: 220d 0a64 6570 656e 6465 6e63 6965 7320  "..dependencies 
 000000e0: 3d20 5b0d 0a20 2020 2022 7079 2d75 626a  = [..    "py-ubj
 000000f0: 736f 6e7e 3d30 2e31 3622 2c0d 0a20 2020  son~=0.16",..   
 00000100: 2022 747a 6c6f 6361 6c7e 3d34 2e33 222c   "tzlocal~=4.3",
 00000110: 0d0a 2020 2020 2270 6f6c 6172 737e 3d30  ..    "polars~=0
 00000120: 2e31 372e 3922 2c0d 0a5d 0d0a 636c 6173  .17.9",..]..clas
 00000130: 7369 6669 6572 7320 3d20 5b0d 0a20 2020  sifiers = [..   
@@ -31,8 +31,12 @@
 000001e0: 7b66 696c 6520 3d20 224c 4943 454e 5345  {file = "LICENSE
 000001f0: 2e74 7874 227d 0d0a 6465 7363 7269 7074  .txt"}..descript
 00000200: 696f 6e20 3d20 2253 7461 7473 206c 6962  ion = "Stats lib
 00000210: 7261 7279 2066 6f72 2053 5342 4d20 7265  rary for SSBM re
 00000220: 706c 6179 2066 696c 6573 220d 0a72 6561  play files"..rea
 00000230: 646d 6520 3d20 2252 4541 444d 452e 6d64  dme = "README.md
 00000240: 220d 0a72 6571 7569 7265 732d 7079 7468  "..requires-pyth
-00000250: 6f6e 203d 2022 3e3d 332e 3130 22         on = ">=3.10"
+00000250: 6f6e 203d 2022 3e3d 332e 3130 220d 0a0d  on = ">=3.10"...
+00000260: 0a5b 746f 6f6c 2e73 6574 7570 746f 6f6c  .[tool.setuptool
+00000270: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000280: 0d0a 6e61 6d65 7370 6163 6573 203d 2066  ..namespaces = f
+00000290: 616c 7365                                alse
```

### Comparing `slippistats-0.1.2/slippistats/controller.py` & `slippistats-0.1.3/slippistats/controller.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.2/slippistats/enums/attack.py` & `slippistats-0.1.3/slippistats/enums/attack.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.2/slippistats/enums/character.py` & `slippistats-0.1.3/slippistats/enums/character.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.2/slippistats/enums/item.py` & `slippistats-0.1.3/slippistats/enums/item.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.2/slippistats/enums/stage.py` & `slippistats-0.1.3/slippistats/enums/stage.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     RANDALL = 0
     LEFT_PLATFORM = 1
     LEFT_SLANT = 2
     MAIN_STAGE = 3
     TOP_PLATFORM = 4
     RIGHT_PLATFORM = 5
     RIGHT_SLANT = 6
+    #TODO do the weird lips on the walls have ground IDs?
 
 
 class Battlefield(GroundID):
     LEFT_EDGE = 0
     MAIN_STAGE = 1
     LEFT_PLATFORM = 2
     TOP_PLATFORM = 3
@@ -92,15 +93,15 @@
 class FinalDestination(GroundID):
     LEFT_EDGE = 0
     MAIN_STAGE = 1
     RIGHT_EDGE = 2
 
 
 @lru_cache(maxsize=16)
-def get_ground(stage: Stage, ground_id: int) -> IntEnum | None:
+def get_ground(stage: Stage, ground_id: int) -> GroundID | int | None:
     if stage is None or ground_id is None:
         return ground_id
 
     match stage:
         case Stage.YOSHIS_STORY:
             if ground_id in {2, 6}:
                 ground = Yoshis.MAIN_STAGE
```

### Comparing `slippistats-0.1.2/slippistats/enums/state.py` & `slippistats-0.1.3/slippistats/enums/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import IntFlag
 from functools import lru_cache
 from .character import InGameCharacter
-from ..util import IntEnum
+from ..util import IntEnum, try_enum
 
 # Use reference: https://docs.google.com/spreadsheets/d/1JX2w-r2fuvWuNgGb6D3Cs4wHQKLFegZe2jhbBuIhCG8/edit#gid=13
 
 # To check if an action state is zero-indexed:https://github.com/altf4/libmelee/blob/master/melee/actiondata.csv
 # I might add some form of check in here, but for now i just handle it manually.
 
 
@@ -811,59 +811,28 @@
     BARREL_CANNON_WAIT = 340
 
 
 # ---------------------------------------------------------------------------- #
 #                           Character Specific State                           #
 # ---------------------------------------------------------------------------- #
 
-CHARACTER_STATE_DICT = {
-    InGameCharacter.BOWSER: lambda x: Bowser(x),
-    InGameCharacter.CAPTAIN_FALCON: lambda x: CaptainFalcon(x),
-    InGameCharacter.DONKEY_KONG: lambda x: DonkeyKong(x),
-    InGameCharacter.DR_MARIO: lambda x: DrMario(x),
-    InGameCharacter.FALCO: lambda x: Falco(x),
-    InGameCharacter.FOX: lambda x: Fox(x),
-    InGameCharacter.GAME_AND_WATCH: lambda x: GameAndWatch(x),
-    InGameCharacter.GANONDORF: lambda x: Ganondorf(x),
-    InGameCharacter.JIGGLYPUFF: lambda x: Jigglypuff(x),
-    InGameCharacter.KIRBY: lambda x: Kirby(x),
-    InGameCharacter.LINK: lambda x: Link(x),
-    InGameCharacter.LUIGI: lambda x: Luigi(x),
-    InGameCharacter.MARIO: lambda x: Mario(x),
-    InGameCharacter.MARTH: lambda x: Marth(x),
-    InGameCharacter.MEWTWO: lambda x: Mewtwo(x),
-    InGameCharacter.NANA: lambda x: Nana(x),
-    InGameCharacter.NESS: lambda x: Ness(x),
-    InGameCharacter.PEACH: lambda x: Peach(x),
-    InGameCharacter.PICHU: lambda x: Pichu(x),
-    InGameCharacter.PIKACHU: lambda x: Pikachu(x),
-    InGameCharacter.POPO: lambda x: Popo(x),
-    InGameCharacter.ROY: lambda x: Roy(x),
-    InGameCharacter.SAMUS: lambda x: Samus(x),
-    InGameCharacter.SHEIK: lambda x: Sheik(x),
-    InGameCharacter.YOSHI: lambda x: Yoshi(x),
-    InGameCharacter.YOUNG_LINK: lambda x: YoungLink(x),
-    InGameCharacter.ZELDA: lambda x: Zelda(x),
-    None: lambda x: x,
-}
-
 
 @lru_cache
 def get_character_state(state: int, character: InGameCharacter | int | None = None) -> ActionState:
     """Accepts state and optionally a character, returns a character-specific action state if possible, otherwise
     returns a general action state.
 
     Raises:
         ValueError if state is less than 0
         KeyError if supplied character does not match any valid in-game character values"""
     if state < 0:
         raise ValueError()
     if state < 341:
         return ActionState(state)
-    return CHARACTER_STATE_DICT[character](state)
+    return try_enum(CHARACTER_STATE_DICT[character], state)
 
 
 class Bowser(IntEnum):
     FIRE_BREATH_GROUND_STARTUP = 341
     FIRE_BREATH_GROUND_LOOP = 342
     FIRE_BREATH_GROUND_END = 343
     FIRE_BREATH_AIR_STARTUP = 344
@@ -1731,7 +1700,39 @@
     FARORES_WIND_AIR = 352
     FARORES_WIND_AIR_DISAPPEAR = 353
     FARORES_WIND_AIR_REAPPEAR = 354
     TRANSFORM_GROUND = 355
     TRANSFORM_GROUND_ENDING = 356
     TRANSFORM_AIR = 357
     TRANSFORM_AIR_ENDING = 358
+
+
+CHARACTER_STATE_DICT = {
+    InGameCharacter.BOWSER: Bowser,
+    InGameCharacter.CAPTAIN_FALCON: CaptainFalcon,
+    InGameCharacter.DONKEY_KONG: DonkeyKong,
+    InGameCharacter.DR_MARIO: DrMario,
+    InGameCharacter.FALCO: Falco,
+    InGameCharacter.FOX: Fox,
+    InGameCharacter.GAME_AND_WATCH: GameAndWatch,
+    InGameCharacter.GANONDORF: Ganondorf,
+    InGameCharacter.JIGGLYPUFF: Jigglypuff,
+    InGameCharacter.KIRBY: Kirby,
+    InGameCharacter.LINK: Link,
+    InGameCharacter.LUIGI: Luigi,
+    InGameCharacter.MARIO: Mario,
+    InGameCharacter.MARTH: Marth,
+    InGameCharacter.MEWTWO: Mewtwo,
+    InGameCharacter.NANA: Nana,
+    InGameCharacter.NESS: Ness,
+    InGameCharacter.PEACH: Peach,
+    InGameCharacter.PICHU: Pichu,
+    InGameCharacter.PIKACHU: Pikachu,
+    InGameCharacter.POPO: Popo,
+    InGameCharacter.ROY: Roy,
+    InGameCharacter.SAMUS: Samus,
+    InGameCharacter.SHEIK: Sheik,
+    InGameCharacter.YOSHI: Yoshi,
+    InGameCharacter.YOUNG_LINK: YoungLink,
+    InGameCharacter.ZELDA: Zelda,
+    None: ActionState,
+}
```

### Comparing `slippistats-0.1.2/slippistats/event.py` & `slippistats-0.1.3/slippistats/event.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.2/slippistats/game.py` & `slippistats-0.1.3/slippistats/game.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.2/slippistats/metadata.py` & `slippistats-0.1.3/slippistats/metadata.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.2/slippistats/parse.py` & `slippistats-0.1.3/slippistats/parse.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.2/slippistats/stats/combo_computer.py` & `slippistats-0.1.3/slippistats/stats/combo_computer.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.2/slippistats/stats/common.py` & `slippistats-0.1.3/slippistats/stats/common.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.2/slippistats/stats/computer.py` & `slippistats-0.1.3/slippistats/stats/computer.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass
 from itertools import permutations
 from os import PathLike
 
 from ..enums.character import CSSCharacter
 from ..event import Frame, Start
 from ..game import Game
-from ..util import Base, Port
+from ..util import Base, IntEnum, Port
 from .stat_types import Data
 
 
 class IdentifierError(Exception):
     """Connect code or port identifier does not match any players in the available Game object."""
 
     pass
@@ -29,32 +29,55 @@
 
 
 @dataclass
 class Player(Base):
     """Aggregates info from event.Start.Player and metadata.Player. Also contains all frames for the player's port.
 
     Stats and Combo output is stored here.
+
+    Attributes:
+        character : CSSCharacter
+            The character this player chose on the character select screen
+        post : Port
+            The physical port of the player P1-P4
+        connect_code : str
+            The slippi connect code of the player in the form "CODE#123" (if applicable)
+        display_name : str
+            The slippi display name of the player, max of 15 characters
+        costume : IntEnum
+            Enumerated value of the player's chosen character costume
+        did_win : bool
+            True if the player won
+        frames : tuple[Frame.Port.Data]
+            Tuple containing all of this player's frame events for convenience
+        stats : Data
+            Iterable container of stats calculated through StatsComputer object
+        combos : list[ComboData]
+            Iterable container of combos calculated through ComboComputer object
+        nana_frames : tuple[Frame.Port.Data] | None
+            Tuple containing all of nana's frames for convenience if applicable. Contains none if character is not IC's
+
     """
 
     character: CSSCharacter
     port: Port
     connect_code: str | None
     display_name: str | None
-    costume: int
+    costume: IntEnum
     did_win: bool | None
     frames: tuple[Frame.Port.Data]
     stats: Data
     combos: list
-    nana_frames: tuple[Frame.Port.Data] | None = None
+    nana_frames: tuple[Frame.Port.Data | None] | None = None
 
     def __init__(
         self,
         characters: tuple[CSSCharacter],
         port: Port,
-        costume: int,
+        costume: IntEnum,
         frames: tuple[Frame.Port.Data],
         stats_header: dict,
         nana_frames: tuple[Frame.Port.Data] | None = None,
         connect_code: str | None = None,
         display_name: str | None = None,
         did_win: bool | None = None,
     ):
@@ -171,15 +194,14 @@
                     if self.replay.frames[-1].ports[port].leader.post.stocks_remaining > 0:
                         did_win = True
                     else:
                         did_win = False
             else:
                 did_win = False
 
-
             temp.append(
                 Player(
                     characters=characters.pop(0),
                     port=port,
                     connect_code=self.replay.metadata.players[port].connect_code,
                     display_name=self.replay.metadata.players[port].display_name,
                     costume=self.replay.start.players[port].costume,
```

### Comparing `slippistats-0.1.2/slippistats/stats/stat_types.py` & `slippistats-0.1.3/slippistats/stats/stat_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from abc import ABC, abstractmethod
 from collections import UserList
 from dataclasses import dataclass, field
-from datetime import tzinfo
 from math import degrees, dist
 from pathlib import Path
 
 import polars as pl
 from tzlocal import get_localzone_name
 from ..enums.stage import GroundID
 
@@ -54,15 +53,16 @@
     """The frame the event began on (0-indexed)"""
     stocks_remaining: int | None
     angle: float | None
     """Wavedash angle in degrees below horizontal"""
     direction: Direction | None
     """Direction of the wavedash, can be LEFT, RIGHT, or DOWN"""
     trigger_frame: int
-    """If the event is not a waveland, the number of frames between the last jumpsquat frame and the trigger press"""  # TODO
+    """If the event is not a waveland, the number of frames between the last jumpsquat frame and the trigger press"""
+    # TODO
     airdodge_frames: int
     """The number of frames the character was in airdodge between the trigger press and landing"""
     waveland: bool
     """True if there were no jumpsquat frames within a few frames of the trigger input"""
 
     def __init__(
         self,
@@ -101,15 +101,16 @@
             elif self.angle == 90:
                 self.angle *= -1
                 self.direction = Direction.DOWN
             else:
                 self.angle = None
                 self.direction = None
                 raise ValueError(
-                    f"unexpected wavedash angle. Frame = {frame_index}, Stickpos = {stick}, angle = {degrees(get_angle(stick))}"
+                    f"""unexpected wavedash angle. Frame = {frame_index},
+                    Stickpos = {stick}, angle = {degrees(get_angle(stick))}"""
                 )
         else:
             self.angle = None
             self.direction = None
         self.trigger_frame = trigger_frame
         self.airdodge_frames = airdodge_frames
         self.waveland = True
@@ -369,15 +370,16 @@
         l_cancel : bool
             True if successful l-cancel
         move : Attack
             IntEnum representing which move was l-canceled
         position : GroundID
             IntEnum representing which platform/ground the player landed on
         trigger_input_frame : int
-            Relative timing of the L/R/Z press. Negative values occur before landing, positive values occur after landing
+            Relative timing of the L/R/Z press. Negative values occur before landing, positive values occur after
+            landing
         during_hitlag : bool
             True if the l-cancel input occurred during hitlag (thus extending the timing window)
         fastfall : bool
             True if character was fastfalling prior to landing
     """
 
     frame_index: int
@@ -404,15 +406,17 @@
 
 
 # @dataclass
 # class RecoveryData(Stat):
 #     frame_index: int
 
 
-# --------------------------------- Wrappers --------------------------------- #
+# ---------------------------------------------------------------------------- #
+#                                   Wrappers                                   #
+# ---------------------------------------------------------------------------- #
 
 # TODO ABC, protocol, mixin? for append, to_polars, etc.
 
 
 class StatList(ABC, UserList):
     data: list[Stat]
     _data_header: dict
@@ -440,14 +444,18 @@
         if len(self.data) == 0:
             return pl.DataFrame([], schema=self._schema)
         else:
             return pl.DataFrame(
                 [self._data_header | vars(stat) for stat in self.data if stat is not None], schema=self._schema
             )
 
+    # if it's stupid and it works, it's not stupid
+    def to_pandas(self):
+        self.to_polars().to_pandas()
+
     def write_excel(self, target: str | Path, utc_time: bool = False) -> None:
         """Writes excel file with target path.
 
         Excel cannot accept timezone-aware dataframes.
 
         If utc_time is False,
         the document will contain naive time local to the machine that parsed the replay.
@@ -637,19 +645,19 @@
             return pl.DataFrame([], self._schema)
         else:
             rows = []
 
             for stat in self.data:
                 try:
                     name = stat.last_hit_by.name
-                except:
+                except AttributeError:
                     name = None
                 try:
-                    ground_id = stat.ground_id.nameS
-                except:
+                    ground_id = stat.ground_id.name
+                except AttributeError:
                     ground_id = None
                 stat_dict = vars(stat).copy()
                 stat_dict["position"] = list(stat.position)
                 stat_dict["tech_type"] = stat.tech_type.name
                 stat_dict["ground_id"] = ground_id
                 stat_dict["last_hit_by"] = name
                 rows.append(self._data_header | stat_dict)
```

### Comparing `slippistats-0.1.2/slippistats/stats/stats_computer.py` & `slippistats-0.1.3/slippistats/stats/stats_computer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,44 +1,39 @@
 import concurrent.futures
 import os
 from pathlib import Path
 from typing import NamedTuple
 import warnings
-from collections import deque
+
 from itertools import permutations
 from math import degrees
 
 import polars as pl
 
-from ..enums.stage import Yoshis, get_ground
+from ..enums.stage import get_ground
 from ..enums.state import (
     ActionRange,
     ActionState,
     LCancel,
 )
 from ..event import Attack, Buttons
 from ..game import Game
 from ..util import Port, try_enum
 from .common import (
-    THROW_STATE_TO_ATTACK,
     JoystickRegion,
     TechType,
     get_angle,
     get_joystick_region,
     get_post_di_angle,
     get_post_di_velocity,
     get_tech_type,
     is_damaged,
     is_downed,
-    is_dying,
     is_fastfalling,
     is_in_hitlag,
-    is_in_hitstun,
-    is_ledge_action,
-    is_offstage,
     is_shielding,
     is_teching,
     just_entered_state,
     just_exited_state,
     just_input_l_cancel,
     just_took_damage,
 )
@@ -133,15 +128,16 @@
         Args:
             identifier : str | int | Ports | None
                 Defaults to None. str format "CODE#123". Ports/int correspond to physical ports p1-p4. If None,
                 calculates stats for all players present in the game
 
         Returns:
             Player | tuple[Player]
-                Returns the Player object matching the identifier argument. If no identifier is given, returns a tuple containing both player objects.
+                Returns the Player object matching the identifier argument. If no identifier is given,
+                returns a tuple containing both player objects.
 
                 Stats can be accessed through Player.stats
         """
         if identifier is None:
             player_perms = permutations(self.players)
         else:
             player_perms = [(self.get_player(identifier), self.get_opponent(identifier))]
@@ -432,16 +428,16 @@
             )
 
             # this whole block basically calculates DI and KB trajectories and outputs the event
             if not in_hitlag:
                 # Not every throw puts the player in hitlag, so we need a bespoke check to catch them.
                 # TODO check how KB and DI velocities look just before/during/after the grabbed -> thrown transition
                 if (
-                    (  # the downed and teching checks are necessary for things like fox's dthrow where the opponent goes
-                        # straight from capture throw -> downed/tech state
+                    (  # the downed and teching checks are necessary for things like fox's dthrow where
+                        # the opponent goes straight from capture throw -> downed/tech state
                         is_damaged(player_frame.post.state)
                         or is_downed(player_frame.post.state)
                         or is_teching(player_frame.post.state)
                     )
                     and just_took_damage(player_frame.post.percent, player_frame.pre.percent)
                     and (ActionRange.THROWN_START <= prev_player_frame.post.state <= ActionRange.THROWN_END)
                 ):
```

### Comparing `slippistats-0.1.2/slippistats/util.py` & `slippistats-0.1.3/slippistats/util.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.2/slippistats.egg-info/PKG-INFO` & `slippistats-0.1.3/slippistats.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: slippistats
-Version: 0.1.2
+Version: 0.1.3
 Summary: Stats library for SSBM replay files
-Home-page: https://github.com/Walnut356/py-slippi-stats
-Author: Walnut
 Author-email: Walnut356 <walnut356@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 melkor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `slippistats-0.1.2/slippistats.egg-info/SOURCES.txt` & `slippistats-0.1.3/slippistats.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE.txt
 README.md
 pyproject.toml
-setup.py
 slippistats/__init__.py
 slippistats/controller.py
 slippistats/event.py
 slippistats/game.py
 slippistats/log.py
 slippistats/metadata.py
 slippistats/parse.py
```

### Comparing `slippistats-0.1.2/test/replays_test.py` & `slippistats-0.1.3/test/replays_test.py`

 * *Files identical despite different names*

