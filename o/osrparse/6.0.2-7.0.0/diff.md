# Comparing `tmp/osrparse-6.0.2.tar.gz` & `tmp/osrparse-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osrparse-6.0.2.tar", last modified: Sun Dec 11 18:14:07 2022, max compression
+gzip compressed data, was "osrparse-7.0.0.tar", last modified: Wed May 10 23:14:58 2023, max compression
```

## Comparing `osrparse-6.0.2.tar` & `osrparse-7.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2022-12-11 18:14:07.181805 osrparse-6.0.2/
--rw-r--r--   0 tybug      (501) staff       (20)     1073 2021-01-27 02:38:38.000000 osrparse-6.0.2/LICENSE
--rw-r--r--   0 tybug      (501) staff       (20)     2617 2022-12-11 18:14:07.181674 osrparse-6.0.2/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)     1917 2022-11-22 01:50:19.000000 osrparse-6.0.2/README.md
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2022-12-11 18:14:07.180331 osrparse-6.0.2/osrparse/
--rw-r--r--   0 tybug      (501) staff       (20)      427 2022-12-11 18:13:52.000000 osrparse-6.0.2/osrparse/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)    16447 2022-12-11 18:13:21.000000 osrparse-6.0.2/osrparse/replay.py
--rw-r--r--   0 tybug      (501) staff       (20)     4358 2022-11-22 01:50:19.000000 osrparse-6.0.2/osrparse/utils.py
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2022-12-11 18:14:07.180791 osrparse-6.0.2/osrparse.egg-info/
--rw-r--r--   0 tybug      (501) staff       (20)     2617 2022-12-11 18:14:06.000000 osrparse-6.0.2/osrparse.egg-info/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)      273 2022-12-11 18:14:07.000000 osrparse-6.0.2/osrparse.egg-info/SOURCES.txt
--rw-r--r--   0 tybug      (501) staff       (20)        1 2022-12-11 18:14:06.000000 osrparse-6.0.2/osrparse.egg-info/dependency_links.txt
--rw-r--r--   0 tybug      (501) staff       (20)       15 2022-12-11 18:14:07.000000 osrparse-6.0.2/osrparse.egg-info/top_level.txt
--rw-r--r--   0 tybug      (501) staff       (20)       38 2022-12-11 18:14:07.181848 osrparse-6.0.2/setup.cfg
--rw-r--r--   0 tybug      (501) staff       (20)     1046 2022-11-07 23:16:52.000000 osrparse-6.0.2/setup.py
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2022-12-11 18:14:07.181338 osrparse-6.0.2/tests/
--rw-r--r--   0 tybug      (501) staff       (20)        0 2021-01-27 02:38:38.000000 osrparse-6.0.2/tests/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)     1156 2022-11-22 01:50:19.000000 osrparse-6.0.2/tests/test_dumping.py
--rw-r--r--   0 tybug      (501) staff       (20)     4715 2022-12-11 18:13:21.000000 osrparse-6.0.2/tests/test_replay.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-05-10 23:14:58.272369 osrparse-7.0.0/
+-rw-r--r--   0 tybug      (501) staff       (20)     1073 2021-01-27 02:38:38.000000 osrparse-7.0.0/LICENSE
+-rw-r--r--   0 tybug      (501) staff       (20)     2401 2023-05-10 23:14:58.272208 osrparse-7.0.0/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)     1786 2023-04-30 19:06:37.000000 osrparse-7.0.0/README.md
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-05-10 23:14:58.270249 osrparse-7.0.0/osrparse/
+-rw-r--r--   0 tybug      (501) staff       (20)      480 2023-05-10 23:10:04.000000 osrparse-7.0.0/osrparse/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)    16920 2023-05-10 23:13:25.000000 osrparse-7.0.0/osrparse/replay.py
+-rw-r--r--   0 tybug      (501) staff       (20)     4358 2022-11-22 01:50:19.000000 osrparse-7.0.0/osrparse/utils.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-05-10 23:14:58.271093 osrparse-7.0.0/osrparse.egg-info/
+-rw-r--r--   0 tybug      (501) staff       (20)     2401 2023-05-10 23:14:58.000000 osrparse-7.0.0/osrparse.egg-info/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)      279 2023-05-10 23:14:58.000000 osrparse-7.0.0/osrparse.egg-info/SOURCES.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        1 2023-05-10 23:14:58.000000 osrparse-7.0.0/osrparse.egg-info/dependency_links.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        9 2023-05-10 23:14:58.000000 osrparse-7.0.0/osrparse.egg-info/top_level.txt
+-rw-r--r--   0 tybug      (501) staff       (20)      639 2023-05-10 23:14:18.000000 osrparse-7.0.0/pyproject.toml
+-rw-r--r--   0 tybug      (501) staff       (20)       38 2023-05-10 23:14:58.272421 osrparse-7.0.0/setup.cfg
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-05-10 23:14:58.271896 osrparse-7.0.0/tests/
+-rw-r--r--   0 tybug      (501) staff       (20)        0 2021-01-27 02:38:38.000000 osrparse-7.0.0/tests/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)     1156 2023-05-04 04:35:28.000000 osrparse-7.0.0/tests/test_dumping.py
+-rw-r--r--   0 tybug      (501) staff       (20)     4715 2023-05-10 23:13:25.000000 osrparse-7.0.0/tests/test_replay.py
```

### Comparing `osrparse-6.0.2/LICENSE` & `osrparse-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osrparse-6.0.2/PKG-INFO` & `osrparse-7.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 2.1
 Name: osrparse
-Version: 6.0.2
+Version: 7.0.0
 Summary: Parser for osr files and lzma replay streams for osu!
-Home-page: https://github.com/kszlim/osu-replay-parser
-Download-URL: https://github.com/kszlim/osu-replay-parser/tarball/v6.0.2
-Author: Kevin Lim, Liam DeVoe
-Author-email: kszlim@gmail.com, orionldevoe@gmail.com
-License: MIT
-Keywords: osu!, osr, replay, replays, parsing, parser, python
+Author-email: Kevin Lim <kszlim@gmail.com>, Liam DeVoe <orionldevoe@gmail.com>
+Project-URL: Homepage, https://github.com/kszlim/osu-replay-parser
+Keywords: osu!,osr,replay,replays,parsing,parser,python
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPi version](https://badge.fury.io/py/osrparse.svg)](https://pypi.org/project/osrparse/)
-[![Build Status](https://travis-ci.org/kszlim/osu-replay-parse.svg?branch=master)](https://travis-ci.org/kszlim/osu-replay-parser)
 
 # osrparse, a python parser for osu! replays
 
 This is a parser for the ``.osr`` format for osu! replay files, as described by [the wiki](https://osu.ppy.sh/wiki/en/Client/File_formats/Osr_%28file_format%29).
 
 ## Installation
 
@@ -29,15 +25,15 @@
 
 ```sh
 pip install osrparse
 ```
 
 ## Documentation
 
-Please see the full documentation for a comprehensive guide: <https://kevin-lim.ca/osu-replay-parser/>. A quickstart follows below for the impatient, but you should read the full documentation if you are at all confused.
+Please see the full documentation for a comprehensive guide: <https://kszlim.github.io/osu-replay-parser>. A quickstart follows below for the impatient, but you should read the full documentation if you are at all confused.
 
 ### Quickstart
 
 ```python
 from osrparse import Replay, parse_replay_data
 # parse from a path
 replay = Replay.from_path("path/to/osr.osr")
@@ -50,17 +46,17 @@
 with open("path/to/osr.osr") as f:
     replay_string = f.read()
 replay = Replay.from_string(replay_string)
 
 # a replay has various attributes
 r = replay
 print(r.mode, r.game_version, r.beatmap_hash, r.username,
-    r.replay_hash, r.count_300, r.count_100, r.count_50, 
-    r.count_geki, r.count_miss, r.score, r.max_combo, r.perfect, 
-    r.mods, r.life_bar_graph, r.timestamp, r.replay_data, 
+    r.replay_hash, r.count_300, r.count_100, r.count_50,
+    r.count_geki, r.count_miss, r.score, r.max_combo, r.perfect,
+    r.mods, r.life_bar_graph, r.timestamp, r.replay_data,
     r.replay_id, r.rng_seed)
 
 # parse the replay data from api v1's /get_replay endpoint
 lzma_string = retrieve_from_api()
 replay_data = parse_replay_data(lzma_string)
 # replay_data is a list of ReplayEvents
```

### Comparing `osrparse-6.0.2/README.md` & `osrparse-7.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 [![PyPi version](https://badge.fury.io/py/osrparse.svg)](https://pypi.org/project/osrparse/)
-[![Build Status](https://travis-ci.org/kszlim/osu-replay-parse.svg?branch=master)](https://travis-ci.org/kszlim/osu-replay-parser)
 
 # osrparse, a python parser for osu! replays
 
 This is a parser for the ``.osr`` format for osu! replay files, as described by [the wiki](https://osu.ppy.sh/wiki/en/Client/File_formats/Osr_%28file_format%29).
 
 ## Installation
 
@@ -11,15 +10,15 @@
 
 ```sh
 pip install osrparse
 ```
 
 ## Documentation
 
-Please see the full documentation for a comprehensive guide: <https://kevin-lim.ca/osu-replay-parser/>. A quickstart follows below for the impatient, but you should read the full documentation if you are at all confused.
+Please see the full documentation for a comprehensive guide: <https://kszlim.github.io/osu-replay-parser>. A quickstart follows below for the impatient, but you should read the full documentation if you are at all confused.
 
 ### Quickstart
 
 ```python
 from osrparse import Replay, parse_replay_data
 # parse from a path
 replay = Replay.from_path("path/to/osr.osr")
@@ -32,17 +31,17 @@
 with open("path/to/osr.osr") as f:
     replay_string = f.read()
 replay = Replay.from_string(replay_string)
 
 # a replay has various attributes
 r = replay
 print(r.mode, r.game_version, r.beatmap_hash, r.username,
-    r.replay_hash, r.count_300, r.count_100, r.count_50, 
-    r.count_geki, r.count_miss, r.score, r.max_combo, r.perfect, 
-    r.mods, r.life_bar_graph, r.timestamp, r.replay_data, 
+    r.replay_hash, r.count_300, r.count_100, r.count_50,
+    r.count_geki, r.count_miss, r.score, r.max_combo, r.perfect,
+    r.mods, r.life_bar_graph, r.timestamp, r.replay_data,
     r.replay_id, r.rng_seed)
 
 # parse the replay data from api v1's /get_replay endpoint
 lzma_string = retrieve_from_api()
 replay_data = parse_replay_data(lzma_string)
 # replay_data is a list of ReplayEvents
```

### Comparing `osrparse-6.0.2/osrparse/replay.py` & `osrparse-7.0.0/osrparse/replay.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,24 +75,33 @@
         # remove trailing comma (if it exists) to make splitting easier.
         # stable always adds a trailing comma, but some lazer versions do not.
         replay_data_str = replay_data_str.rstrip(",")
         events = [event.split('|') for event in replay_data_str.split(',')]
 
         rng_seed = None
         play_data = []
-        for event in events:
+        for i, event in enumerate(events):
             time_delta = int(event[0])
             x = event[1]
             y = event[2]
             keys = int(event[3])
 
-            if time_delta == -12345 and event == events[-1]:
+            if time_delta == -12345 and i == len(events) - 1:
                 rng_seed = keys
                 continue
 
+            # I don't really know why these frames exist, but lazer removes them
+            # and they can cause issues for minigame replays - e.g., mania
+            # interprets x as keys.
+            # See
+            # https://github.com/ppy/osu/blob/6a04708a7e9801949c6c7ac7ddf6a4d7
+            # fa0835e5/osu.Game/Scoring/Legacy/LegacyScoreDecoder.cs#L290-L294.
+            if i < 2 and float(x) == 256 and float(y) == -500:
+                continue
+
             if mode is GameMode.STD:
                 keys = Key(keys)
                 event = ReplayEventOsu(time_delta, float(x), float(y), keys)
             if mode is GameMode.TAIKO:
                 event = ReplayEventTaiko(time_delta, int(x), KeyTaiko(keys))
             if mode is GameMode.CTB:
                 event = ReplayEventCatch(time_delta, float(x), int(keys) == 1)
```

### Comparing `osrparse-6.0.2/osrparse/utils.py` & `osrparse-7.0.0/osrparse/utils.py`

 * *Files identical despite different names*

### Comparing `osrparse-6.0.2/osrparse.egg-info/PKG-INFO` & `osrparse-7.0.0/osrparse.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 2.1
 Name: osrparse
-Version: 6.0.2
+Version: 7.0.0
 Summary: Parser for osr files and lzma replay streams for osu!
-Home-page: https://github.com/kszlim/osu-replay-parser
-Download-URL: https://github.com/kszlim/osu-replay-parser/tarball/v6.0.2
-Author: Kevin Lim, Liam DeVoe
-Author-email: kszlim@gmail.com, orionldevoe@gmail.com
-License: MIT
-Keywords: osu!, osr, replay, replays, parsing, parser, python
+Author-email: Kevin Lim <kszlim@gmail.com>, Liam DeVoe <orionldevoe@gmail.com>
+Project-URL: Homepage, https://github.com/kszlim/osu-replay-parser
+Keywords: osu!,osr,replay,replays,parsing,parser,python
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPi version](https://badge.fury.io/py/osrparse.svg)](https://pypi.org/project/osrparse/)
-[![Build Status](https://travis-ci.org/kszlim/osu-replay-parse.svg?branch=master)](https://travis-ci.org/kszlim/osu-replay-parser)
 
 # osrparse, a python parser for osu! replays
 
 This is a parser for the ``.osr`` format for osu! replay files, as described by [the wiki](https://osu.ppy.sh/wiki/en/Client/File_formats/Osr_%28file_format%29).
 
 ## Installation
 
@@ -29,15 +25,15 @@
 
 ```sh
 pip install osrparse
 ```
 
 ## Documentation
 
-Please see the full documentation for a comprehensive guide: <https://kevin-lim.ca/osu-replay-parser/>. A quickstart follows below for the impatient, but you should read the full documentation if you are at all confused.
+Please see the full documentation for a comprehensive guide: <https://kszlim.github.io/osu-replay-parser>. A quickstart follows below for the impatient, but you should read the full documentation if you are at all confused.
 
 ### Quickstart
 
 ```python
 from osrparse import Replay, parse_replay_data
 # parse from a path
 replay = Replay.from_path("path/to/osr.osr")
@@ -50,17 +46,17 @@
 with open("path/to/osr.osr") as f:
     replay_string = f.read()
 replay = Replay.from_string(replay_string)
 
 # a replay has various attributes
 r = replay
 print(r.mode, r.game_version, r.beatmap_hash, r.username,
-    r.replay_hash, r.count_300, r.count_100, r.count_50, 
-    r.count_geki, r.count_miss, r.score, r.max_combo, r.perfect, 
-    r.mods, r.life_bar_graph, r.timestamp, r.replay_data, 
+    r.replay_hash, r.count_300, r.count_100, r.count_50,
+    r.count_geki, r.count_miss, r.score, r.max_combo, r.perfect,
+    r.mods, r.life_bar_graph, r.timestamp, r.replay_data,
     r.replay_id, r.rng_seed)
 
 # parse the replay data from api v1's /get_replay endpoint
 lzma_string = retrieve_from_api()
 replay_data = parse_replay_data(lzma_string)
 # replay_data is a list of ReplayEvents
```

### Comparing `osrparse-6.0.2/tests/test_dumping.py` & `osrparse-7.0.0/tests/test_dumping.py`

 * *Files identical despite different names*

### Comparing `osrparse-6.0.2/tests/test_replay.py` & `osrparse-7.0.0/tests/test_replay.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     def test_timestamp(self):
         for replay in self._replays:
             self.assertEqual(replay.timestamp, datetime(2013, 2, 1, 16, 31, 34, tzinfo=timezone.utc), "Timestamp is wrong")
 
     def test_play_data(self):
         for replay in self._replays:
             self.assertIsInstance(replay.replay_data[0], ReplayEventOsu, "Replay data is wrong")
-            self.assertEqual(len(replay.replay_data), 17500, "Replay data is wrong")
+            self.assertEqual(len(replay.replay_data), 17498, "Replay data is wrong")
 
     def test_replay_id(self):
         for replay in self._replays:
             self.assertEqual(replay.replay_id, 1040219800)
         # old replays had game_version stored as a short, we want to make sure
         # we can parse it properly instead of erroring
         self.assertEqual(self._old_replayid_replay.replay_id, 1127598189)
@@ -79,37 +79,37 @@
     @classmethod
     def setUpClass(cls):
         cls.replay = Replay.from_path(RES / "taiko.osr")
 
     def test_play_data(self):
         replay_data = self.replay.replay_data
         self.assertIsInstance(replay_data[0], ReplayEventTaiko, "Replay data is wrong")
-        self.assertEqual(len(replay_data), 17475, "Replay data is wrong")
+        self.assertEqual(len(replay_data), 17473, "Replay data is wrong")
 
 class TestCatchReplay(TestCase):
 
     @classmethod
     def setUpClass(cls):
         cls.replay = Replay.from_path(RES / "ctb.osr")
 
     def test_play_data(self):
         replay_data = self.replay.replay_data
         self.assertIsInstance(replay_data[0], ReplayEventCatch, "Replay data is wrong")
-        self.assertEqual(len(replay_data), 10439, "Replay data is wrong")
+        self.assertEqual(len(replay_data), 10437, "Replay data is wrong")
 
 class TestManiaReplay(TestCase):
 
     @classmethod
     def setUpClass(cls):
         cls.replay = Replay.from_path(RES / "mania.osr")
 
     def test_play_data(self):
         play_data = self.replay.replay_data
         self.assertIsInstance(play_data[0], ReplayEventMania, "Replay data is wrong")
-        self.assertEqual(len(play_data), 17432, "Replay data is wrong")
+        self.assertEqual(len(play_data), 17430, "Replay data is wrong")
 
 class TestLazerReplay(TestCase):
     @classmethod
     def setUpClass(cls):
         cls.replay = Replay.from_path(RES / "lazer_standard_format.osr")
 
     def test_play_data(self):
```

