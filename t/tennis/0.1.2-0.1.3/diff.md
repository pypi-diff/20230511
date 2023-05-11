# Comparing `tmp/tennis-0.1.2.tar.gz` & `tmp/tennis-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tennis-0.1.2.tar", last modified: Thu May 11 02:25:55 2023, max compression
+gzip compressed data, was "tennis-0.1.3.tar", last modified: Thu May 11 03:31:56 2023, max compression
```

## Comparing `tennis-0.1.2.tar` & `tennis-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 02:25:55.873822 tennis-0.1.2/
--rw-rw-rw-   0        0        0     1083 2023-05-09 03:08:15.000000 tennis-0.1.2/LICENSE
--rw-rw-rw-   0        0        0    17775 2023-05-11 02:25:55.873822 tennis-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    17334 2023-05-11 02:23:09.000000 tennis-0.1.2/README.md
--rw-rw-rw-   0        0        0      516 2023-05-11 02:23:31.000000 tennis-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 02:25:55.873822 tennis-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      284 2023-05-11 02:23:35.000000 tennis-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 02:25:55.856867 tennis-0.1.2/tennis/
--rw-rw-rw-   0        0        0        0 2023-05-06 20:11:19.000000 tennis-0.1.2/tennis/__init__.py
--rw-rw-rw-   0        0        0    30931 2023-05-11 01:21:55.000000 tennis-0.1.2/tennis/match.py
--rw-rw-rw-   0        0        0    17036 2023-05-10 21:30:40.000000 tennis-0.1.2/tennis/tiebreak.py
-drwxrwxrwx   0        0        0        0 2023-05-11 02:25:55.871826 tennis-0.1.2/tennis.egg-info/
--rw-rw-rw-   0        0        0    17775 2023-05-11 02:25:55.000000 tennis-0.1.2/tennis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-05-11 02:25:55.000000 tennis-0.1.2/tennis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 02:25:55.000000 tennis-0.1.2/tennis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-11 02:25:55.000000 tennis-0.1.2/tennis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 03:31:56.976299 tennis-0.1.3/
+-rw-rw-rw-   0        0        0     1083 2023-05-09 03:08:15.000000 tennis-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0    17810 2023-05-11 03:31:56.976299 tennis-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    17323 2023-05-11 03:16:20.000000 tennis-0.1.3/README.md
+-rw-rw-rw-   0        0        0      516 2023-05-11 03:31:38.000000 tennis-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 03:31:56.976299 tennis-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      330 2023-05-11 03:31:35.000000 tennis-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 03:31:56.962336 tennis-0.1.3/tennis/
+-rw-rw-rw-   0        0        0        0 2023-05-06 20:11:19.000000 tennis-0.1.3/tennis/__init__.py
+-rw-rw-rw-   0        0        0    30931 2023-05-11 01:21:55.000000 tennis-0.1.3/tennis/match.py
+-rw-rw-rw-   0        0        0    17036 2023-05-10 21:30:40.000000 tennis-0.1.3/tennis/tiebreak.py
+drwxrwxrwx   0        0        0        0 2023-05-11 03:31:56.974304 tennis-0.1.3/tennis.egg-info/
+-rw-rw-rw-   0        0        0    17810 2023-05-11 03:31:56.000000 tennis-0.1.3/tennis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-05-11 03:31:56.000000 tennis-0.1.3/tennis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 03:31:56.000000 tennis-0.1.3/tennis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-11 03:31:56.000000 tennis-0.1.3/tennis.egg-info/top_level.txt
```

### Comparing `tennis-0.1.2/LICENSE` & `tennis-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tennis-0.1.2/PKG-INFO` & `tennis-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: tennis
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for tracking tennis matches and scoring
+Home-page: https://github.com/bear102/tennis
 Author: bear102
 License: MIT
 Project-URL: Homepage, https://github.com/bear102/tennis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -28,31 +29,33 @@
   - [Features](#features)
     - [1. Match Simulation](#1-match-simulation)
     - [2. Tiebreaker](#2-tiebreaker)
     - [Tracking Stats](#tracking-stats)
   - [Usage](#usage)
     - [Quick Start](#quick-start)
     - [Match Methods](#match-methods)
-      - [TennisMatch (self, player1:str, player2:str, matchFormat:dict=None)](#tennismatch-self-player1str-player2str-matchformatdictnone)
-      - [`backup_match` ()](#backup_match-)
-      - [`load_backup` (self, backup\_data)](#load_backup-self-backup_data)
-      - [**`win_point`** (self, player:str, how\_won=\[\])](#win_point-self-playerstr-how_won)
-      - [`serve_fault` (self, player:str)](#serve_fault-self-playerstr)
-      - [`win_game` (self, player:str)](#win_game-self-playerstr)
-      - [`win_set` (self, player:str)](#win_set-self-playerstr)
-      - [`get_all_info` (self)](#get_all_info-self)
-      - [`get_scoreboard` (self, player:str)](#get_scoreboard-self-playerstr)
-      - [`match_stats` (self, player:str)](#match_stats-self-playerstr)
+      - [***TennisMatch (self, player1:str, player2:str, matchFormat:dict=None)***](#tennismatch-self-player1str-player2str-matchformatdictnone)
+      - [***backup\_match ()***](#backup_match-)
+      - [***load\_backup (self, backup\_data)***](#load_backup-self-backup_data)
+      - [***win\_point (self, player:str, how\_won=\[\])***](#win_point-self-playerstr-how_won)
+      - [***serve\_fault (self, player:str)***](#serve_fault-self-playerstr)
+      - [***win\_game (self, player:str)***](#win_game-self-playerstr)
+      - [***win\_set (self, player:str)***](#win_set-self-playerstr)
+      - [***get\_all\_info (self)***](#get_all_info-self)
+      - [***get\_scoreboard (self, player:str)***](#get_scoreboard-self-playerstr)
+      - [***match\_stats (self, player:str)***](#match_stats-self-playerstr)
     - [Tiebreak Methods](#tiebreak-methods)
-      - [Tiebreak (self, player1:str, player2:str, matchFormat:dict=None)](#tiebreak-self-player1str-player2str-matchformatdictnone)
-      - [backup\_tiebreak ()](#backup_tiebreak-)
-      - [load\_backup (self, backup\_data)](#load_backup-self-backup_data-1)
-      - [`win_point` (self, player:str, how\_won=\[\])](#win_point-self-playerstr-how_won-1)
-      - [`tiebreak_stats` (self, player:str)](#tiebreak_stats-self-playerstr)
-      - [`get_scoreboard` (self, player:str)](#get_scoreboard-self-playerstr-1)
+      - [***tiebreak (self, player1:str, player2:str, matchFormat:dict=None)***](#tiebreak-self-player1str-player2str-matchformatdictnone)
+      - [***backup\_tiebreak ()***](#backup_tiebreak-)
+      - [***load\_backup (self, backup\_data)***](#load_backup-self-backup_data-1)
+      - [***win\_point (self, player:str, how\_won=\[\])***](#win_point-self-playerstr-how_won-1)
+      - [***tiebreak\_stats (self, player:str)***](#tiebreak_stats-self-playerstr)
+      - [***get\_scoreboard (self, player:str)***](#get_scoreboard-self-playerstr-1)
+
+
 
 
 ## [Features](#features)
 
 The Tennis library offers the following main features:
 <br>
 ### [1. Match Simulation](#1-match-simulation)
@@ -250,20 +253,18 @@
 ════════════════════════════════════════
 ```
 
 <br><br><br>
 
   
 
-### <h1>[Match Methods](#match-methods)</h1>
+### <h1>Match Methods</h1>
 
-
-#### [TennisMatch](#tennismatch) (self, player1:str, player2:str, matchFormat:dict=None)
+#### ***TennisMatch (self, player1:str, player2:str, matchFormat:dict=None)***
 Creates a new instance of a tennis match.
-
 **Parameters**
 
 - player1 (str): The name of player 1.
 - player2 (str): The name of player 2.
 - matchFormat (dict): A dictionary of match settings.
   
 **Example**
@@ -275,18 +276,18 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`backup_match`](#backup_match) ()
+#### ***<h3>backup_match ()</h3>***
 Creates a backup for the current tennis match instance
 
-#### [`load_backup`](#load_backup) (self, backup_data)
+#### ***<h3>load_backup (self, backup_data)</h3>***
 Loads a backup into a new match
 
 **Parameters**
 - backup_data (dict): The backup data created by the backup_match method
 
 
 **Example**
@@ -307,15 +308,15 @@
 
 ***
 
 <br>
 
 
 
-#### **[`win_point`](#win_point)** (self, player:str, how_won=[])
+#### ***<h3>win_point (self, player:str, how_won=[])</h3>***
 method that handles a player winning or loosing a point. Do not call this method if it is a double fault. Instead, call the [`serve_fault` (self, player:str)](#serve_fault-self-playerstr) method
 
 **Parameters**
 - player (str): The name of the player who won the point.
 - how_won (Array): How the point was won (more than 1 in a method call is ok, just append them to the end of the list like ['winner','win_by_volley'])
   - `Ace`: player A wins by by acing player b (Player A's serves the ball in and player B does not even touch the ball)
   - `winner`: player A wins the point by hitting a winner. (The opponent doesnt touch the ball at all)
@@ -334,15 +335,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`serve_fault`](#serve_fault) (self, player:str)
+#### ***<h3>serve_fault (self, player:str)</h3>***
 method to call when a server misses a first or second serve
 
 **Parameters**
 - player (str): The name of the player who missed the serve
 
 **Example**
 ```python
@@ -357,15 +358,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`win_game`](#win_game) (self, player:str)
+#### ***<h3>win_game (self, player:str)</h3>***
 A method that will win the game for a player. This method is intended for development and testing. The statistics for the match will be off.
 
 **Parameters**
 - player (str): the player that will win the game
 
 **Example**
 ```python
@@ -375,15 +376,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`win_set`](#win_set) (self, player:str)
+#### ***<h3>win_set (self, player:str)</h3>***
 A method that will win the set for a player. This method is intended for development and testing. The statistics for the match will be off.
 
 **Parameters**
 - player (str): the player that will win the set
 
 **Example**
 ```python
@@ -393,15 +394,15 @@
 <br>
 
 ***
 
 <br>
 
 
-#### [`get_all_info`](#get_all_info) (self)
+#### ***<h3>get_all_info (self)</h3>***
 A method that will return all the info about the match in a dictionary format
 
 ```python
 return {"winner":self.winner, "game_history":self.gameHistory, "set_history": self.setHistory, "set_tiebreak_history":self.setTieBreakScoresHistory, "match_tiebreak_history":self.matchTieBreakScore,"match_format":self.matchFormat,"match_stats":self.matchStats}
 ```
 
 **example output**
@@ -411,15 +412,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`get_scoreboard`](#get_scoreboard) (self, player:str)
+#### ***<h3>get_scoreboard (self, player:str)</h3>***
 A method that will return a string representation of the current scoreboard.
 
 **Parameters**
 - player (str): the player whos name and score will appear on the top half of the scoreboard
 
 **Example Output**
 
@@ -436,15 +437,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`match_stats`](#match_stats) (self, player:str)
+#### ***</h3>match_stats (self, player:str)</h3>***
 A method that will return the statistics about the match in a string format
 
 **Parameters**
 - player (str): the player who will appear on the left side of the stats
 
 **Example Output**
 ```python
@@ -481,17 +482,17 @@
 
 
 
 ════════════════════════════════════════
 ```
 <br><br>
 
-### <h1>[Tiebreak Methods](#tiebreak-methods)</h1>
+### <h1>Tiebreak Methods</h1>
 
-#### [Tiebreak](#tiebreak) (self, player1:str, player2:str, matchFormat:dict=None)
+#### ***<h3>tiebreak (self, player1:str, player2:str, matchFormat:dict=None)</h3>***
 Creates a new instance of a tiebreak.
 
 **Parameters**
 - player1 (str): the name of the first player
 - player2 (str): the name of the second player
 - matchFormat (dict): A dictionary of match settings.
 
@@ -502,24 +503,24 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [backup_tiebreak](#backup_tiebreak) ()
+#### ***<h3>backup_tiebreak ()</h3>***
 A method to backup tiebreak data
 
 **Example**
 ```python
 match = tiebreak("a","b",{"first_to_num_points":7, "win_by":2, "whos_serve":"a"})
 backup_data = match.backup_tiebreak()
 ```
 
-#### [load_backup](#load_backup) (self, backup_data)
+#### ***<h3>load_backup (self, backup_data)</h3>***
 A method to load backup data from another tiebreak object
 
 **Parameters**
 - backup_data (dict): the data to load. use the backup_tiebreak method to obtain this
 
 **Example**
 ```python
@@ -539,15 +540,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`win_point`](#win_point) (self, player:str, how_won=[])
+#### ***<h3>win_point (self, player:str, how_won=[])</h3>***
 method that handles a player winning or loosing a point. Do not call this method if it is a double fault. Instead, call the [`serve_fault` (self, player:str)](#serve_fault-self-playerstr) method
 **Parameters**
 - player (str): The name of the player who won the point.
 - how_won (Array): How the point was won (more than 1 in a method call is ok, just append them to the end of the list like ['winner','win_by_volley'])
   - `Ace`: player A wins by by acing player b (Player A's serves the ball in and player B does not even touch the ball)
   - `winner`: player A wins the point by hitting a winner. (The opponent doesnt touch the ball at all)
   - `unforced_error`: player A wins the point because player B made an unforced error (An error that was not caused by player A. For example player B got an easy ball and missed it)
@@ -565,15 +566,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`tiebreak_stats`](#tiebreak_stats) (self, player:str)
+#### ***<h3>tiebreak_stats (self, player:str)</h3>***
 A method that returns a string representation of the statistics of the tiebreak
 
 **Parameters**
 - player (str): the name of the player whos stats will be displayed on the left side
 
 **Example**
 ```python
@@ -583,15 +584,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`get_scoreboard`](#get_scoreboard) (self, player:str)
+#### ***<h3>get_scoreboard (self, player:str)</h3>***
 A method that returns a string representation of the current score
 
 **Parameters**
 - player (str): the name of the player whos stats will be displayed on the top of the scoreboard
 
 **Example**
 ```python
```

### Comparing `tennis-0.1.2/README.md` & `tennis-0.1.3/tennis.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: tennis
+Version: 0.1.3
+Summary: A library for tracking tennis matches and scoring
+Home-page: https://github.com/bear102/tennis
+Author: bear102
+License: MIT
+Project-URL: Homepage, https://github.com/bear102/tennis
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Tennis Library
 
 [![GitHub](https://img.shields.io/badge/GitHub-bear102-%2312100E.svg?style=flat&logo=github)](https://github.com/bear102)
 ![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 The Tennis library is a Python package that provides functionalities for simulating tennis matches and tiebreakers. It offers easy-to-use methods to simulate and track scores, tiebreakers, and various statistics. The tennis library is perfect for tracking real time data input.
@@ -14,31 +29,33 @@
   - [Features](#features)
     - [1. Match Simulation](#1-match-simulation)
     - [2. Tiebreaker](#2-tiebreaker)
     - [Tracking Stats](#tracking-stats)
   - [Usage](#usage)
     - [Quick Start](#quick-start)
     - [Match Methods](#match-methods)
-      - [TennisMatch (self, player1:str, player2:str, matchFormat:dict=None)](#tennismatch-self-player1str-player2str-matchformatdictnone)
-      - [`backup_match` ()](#backup_match-)
-      - [`load_backup` (self, backup\_data)](#load_backup-self-backup_data)
-      - [**`win_point`** (self, player:str, how\_won=\[\])](#win_point-self-playerstr-how_won)
-      - [`serve_fault` (self, player:str)](#serve_fault-self-playerstr)
-      - [`win_game` (self, player:str)](#win_game-self-playerstr)
-      - [`win_set` (self, player:str)](#win_set-self-playerstr)
-      - [`get_all_info` (self)](#get_all_info-self)
-      - [`get_scoreboard` (self, player:str)](#get_scoreboard-self-playerstr)
-      - [`match_stats` (self, player:str)](#match_stats-self-playerstr)
+      - [***TennisMatch (self, player1:str, player2:str, matchFormat:dict=None)***](#tennismatch-self-player1str-player2str-matchformatdictnone)
+      - [***backup\_match ()***](#backup_match-)
+      - [***load\_backup (self, backup\_data)***](#load_backup-self-backup_data)
+      - [***win\_point (self, player:str, how\_won=\[\])***](#win_point-self-playerstr-how_won)
+      - [***serve\_fault (self, player:str)***](#serve_fault-self-playerstr)
+      - [***win\_game (self, player:str)***](#win_game-self-playerstr)
+      - [***win\_set (self, player:str)***](#win_set-self-playerstr)
+      - [***get\_all\_info (self)***](#get_all_info-self)
+      - [***get\_scoreboard (self, player:str)***](#get_scoreboard-self-playerstr)
+      - [***match\_stats (self, player:str)***](#match_stats-self-playerstr)
     - [Tiebreak Methods](#tiebreak-methods)
-      - [Tiebreak (self, player1:str, player2:str, matchFormat:dict=None)](#tiebreak-self-player1str-player2str-matchformatdictnone)
-      - [backup\_tiebreak ()](#backup_tiebreak-)
-      - [load\_backup (self, backup\_data)](#load_backup-self-backup_data-1)
-      - [`win_point` (self, player:str, how\_won=\[\])](#win_point-self-playerstr-how_won-1)
-      - [`tiebreak_stats` (self, player:str)](#tiebreak_stats-self-playerstr)
-      - [`get_scoreboard` (self, player:str)](#get_scoreboard-self-playerstr-1)
+      - [***tiebreak (self, player1:str, player2:str, matchFormat:dict=None)***](#tiebreak-self-player1str-player2str-matchformatdictnone)
+      - [***backup\_tiebreak ()***](#backup_tiebreak-)
+      - [***load\_backup (self, backup\_data)***](#load_backup-self-backup_data-1)
+      - [***win\_point (self, player:str, how\_won=\[\])***](#win_point-self-playerstr-how_won-1)
+      - [***tiebreak\_stats (self, player:str)***](#tiebreak_stats-self-playerstr)
+      - [***get\_scoreboard (self, player:str)***](#get_scoreboard-self-playerstr-1)
+
+
 
 
 ## [Features](#features)
 
 The Tennis library offers the following main features:
 <br>
 ### [1. Match Simulation](#1-match-simulation)
@@ -236,20 +253,18 @@
 ════════════════════════════════════════
 ```
 
 <br><br><br>
 
   
 
-### <h1>[Match Methods](#match-methods)</h1>
+### <h1>Match Methods</h1>
 
-
-#### [TennisMatch](#tennismatch) (self, player1:str, player2:str, matchFormat:dict=None)
+#### ***TennisMatch (self, player1:str, player2:str, matchFormat:dict=None)***
 Creates a new instance of a tennis match.
-
 **Parameters**
 
 - player1 (str): The name of player 1.
 - player2 (str): The name of player 2.
 - matchFormat (dict): A dictionary of match settings.
   
 **Example**
@@ -261,18 +276,18 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`backup_match`](#backup_match) ()
+#### ***<h3>backup_match ()</h3>***
 Creates a backup for the current tennis match instance
 
-#### [`load_backup`](#load_backup) (self, backup_data)
+#### ***<h3>load_backup (self, backup_data)</h3>***
 Loads a backup into a new match
 
 **Parameters**
 - backup_data (dict): The backup data created by the backup_match method
 
 
 **Example**
@@ -293,15 +308,15 @@
 
 ***
 
 <br>
 
 
 
-#### **[`win_point`](#win_point)** (self, player:str, how_won=[])
+#### ***<h3>win_point (self, player:str, how_won=[])</h3>***
 method that handles a player winning or loosing a point. Do not call this method if it is a double fault. Instead, call the [`serve_fault` (self, player:str)](#serve_fault-self-playerstr) method
 
 **Parameters**
 - player (str): The name of the player who won the point.
 - how_won (Array): How the point was won (more than 1 in a method call is ok, just append them to the end of the list like ['winner','win_by_volley'])
   - `Ace`: player A wins by by acing player b (Player A's serves the ball in and player B does not even touch the ball)
   - `winner`: player A wins the point by hitting a winner. (The opponent doesnt touch the ball at all)
@@ -320,15 +335,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`serve_fault`](#serve_fault) (self, player:str)
+#### ***<h3>serve_fault (self, player:str)</h3>***
 method to call when a server misses a first or second serve
 
 **Parameters**
 - player (str): The name of the player who missed the serve
 
 **Example**
 ```python
@@ -343,15 +358,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`win_game`](#win_game) (self, player:str)
+#### ***<h3>win_game (self, player:str)</h3>***
 A method that will win the game for a player. This method is intended for development and testing. The statistics for the match will be off.
 
 **Parameters**
 - player (str): the player that will win the game
 
 **Example**
 ```python
@@ -361,15 +376,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`win_set`](#win_set) (self, player:str)
+#### ***<h3>win_set (self, player:str)</h3>***
 A method that will win the set for a player. This method is intended for development and testing. The statistics for the match will be off.
 
 **Parameters**
 - player (str): the player that will win the set
 
 **Example**
 ```python
@@ -379,15 +394,15 @@
 <br>
 
 ***
 
 <br>
 
 
-#### [`get_all_info`](#get_all_info) (self)
+#### ***<h3>get_all_info (self)</h3>***
 A method that will return all the info about the match in a dictionary format
 
 ```python
 return {"winner":self.winner, "game_history":self.gameHistory, "set_history": self.setHistory, "set_tiebreak_history":self.setTieBreakScoresHistory, "match_tiebreak_history":self.matchTieBreakScore,"match_format":self.matchFormat,"match_stats":self.matchStats}
 ```
 
 **example output**
@@ -397,15 +412,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`get_scoreboard`](#get_scoreboard) (self, player:str)
+#### ***<h3>get_scoreboard (self, player:str)</h3>***
 A method that will return a string representation of the current scoreboard.
 
 **Parameters**
 - player (str): the player whos name and score will appear on the top half of the scoreboard
 
 **Example Output**
 
@@ -422,15 +437,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`match_stats`](#match_stats) (self, player:str)
+#### ***</h3>match_stats (self, player:str)</h3>***
 A method that will return the statistics about the match in a string format
 
 **Parameters**
 - player (str): the player who will appear on the left side of the stats
 
 **Example Output**
 ```python
@@ -467,17 +482,17 @@
 
 
 
 ════════════════════════════════════════
 ```
 <br><br>
 
-### <h1>[Tiebreak Methods](#tiebreak-methods)</h1>
+### <h1>Tiebreak Methods</h1>
 
-#### [Tiebreak](#tiebreak) (self, player1:str, player2:str, matchFormat:dict=None)
+#### ***<h3>tiebreak (self, player1:str, player2:str, matchFormat:dict=None)</h3>***
 Creates a new instance of a tiebreak.
 
 **Parameters**
 - player1 (str): the name of the first player
 - player2 (str): the name of the second player
 - matchFormat (dict): A dictionary of match settings.
 
@@ -488,24 +503,24 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [backup_tiebreak](#backup_tiebreak) ()
+#### ***<h3>backup_tiebreak ()</h3>***
 A method to backup tiebreak data
 
 **Example**
 ```python
 match = tiebreak("a","b",{"first_to_num_points":7, "win_by":2, "whos_serve":"a"})
 backup_data = match.backup_tiebreak()
 ```
 
-#### [load_backup](#load_backup) (self, backup_data)
+#### ***<h3>load_backup (self, backup_data)</h3>***
 A method to load backup data from another tiebreak object
 
 **Parameters**
 - backup_data (dict): the data to load. use the backup_tiebreak method to obtain this
 
 **Example**
 ```python
@@ -525,15 +540,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`win_point`](#win_point) (self, player:str, how_won=[])
+#### ***<h3>win_point (self, player:str, how_won=[])</h3>***
 method that handles a player winning or loosing a point. Do not call this method if it is a double fault. Instead, call the [`serve_fault` (self, player:str)](#serve_fault-self-playerstr) method
 **Parameters**
 - player (str): The name of the player who won the point.
 - how_won (Array): How the point was won (more than 1 in a method call is ok, just append them to the end of the list like ['winner','win_by_volley'])
   - `Ace`: player A wins by by acing player b (Player A's serves the ball in and player B does not even touch the ball)
   - `winner`: player A wins the point by hitting a winner. (The opponent doesnt touch the ball at all)
   - `unforced_error`: player A wins the point because player B made an unforced error (An error that was not caused by player A. For example player B got an easy ball and missed it)
@@ -551,15 +566,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`tiebreak_stats`](#tiebreak_stats) (self, player:str)
+#### ***<h3>tiebreak_stats (self, player:str)</h3>***
 A method that returns a string representation of the statistics of the tiebreak
 
 **Parameters**
 - player (str): the name of the player whos stats will be displayed on the left side
 
 **Example**
 ```python
@@ -569,15 +584,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`get_scoreboard`](#get_scoreboard) (self, player:str)
+#### ***<h3>get_scoreboard (self, player:str)</h3>***
 A method that returns a string representation of the current score
 
 **Parameters**
 - player (str): the name of the player whos stats will be displayed on the top of the scoreboard
 
 **Example**
 ```python
```

### Comparing `tennis-0.1.2/pyproject.toml` & `tennis-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tennis"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="bear102" },
 ]
 description = "A library for tracking tennis matches and scoring"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tennis-0.1.2/tennis/match.py` & `tennis-0.1.3/tennis/match.py`

 * *Files identical despite different names*

### Comparing `tennis-0.1.2/tennis/tiebreak.py` & `tennis-0.1.3/tennis/tiebreak.py`

 * *Files identical despite different names*

### Comparing `tennis-0.1.2/tennis.egg-info/PKG-INFO` & `tennis-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: tennis
-Version: 0.1.2
-Summary: A library for tracking tennis matches and scoring
-Author: bear102
-License: MIT
-Project-URL: Homepage, https://github.com/bear102/tennis
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Tennis Library
 
 [![GitHub](https://img.shields.io/badge/GitHub-bear102-%2312100E.svg?style=flat&logo=github)](https://github.com/bear102)
 ![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 The Tennis library is a Python package that provides functionalities for simulating tennis matches and tiebreakers. It offers easy-to-use methods to simulate and track scores, tiebreakers, and various statistics. The tennis library is perfect for tracking real time data input.
@@ -28,31 +14,33 @@
   - [Features](#features)
     - [1. Match Simulation](#1-match-simulation)
     - [2. Tiebreaker](#2-tiebreaker)
     - [Tracking Stats](#tracking-stats)
   - [Usage](#usage)
     - [Quick Start](#quick-start)
     - [Match Methods](#match-methods)
-      - [TennisMatch (self, player1:str, player2:str, matchFormat:dict=None)](#tennismatch-self-player1str-player2str-matchformatdictnone)
-      - [`backup_match` ()](#backup_match-)
-      - [`load_backup` (self, backup\_data)](#load_backup-self-backup_data)
-      - [**`win_point`** (self, player:str, how\_won=\[\])](#win_point-self-playerstr-how_won)
-      - [`serve_fault` (self, player:str)](#serve_fault-self-playerstr)
-      - [`win_game` (self, player:str)](#win_game-self-playerstr)
-      - [`win_set` (self, player:str)](#win_set-self-playerstr)
-      - [`get_all_info` (self)](#get_all_info-self)
-      - [`get_scoreboard` (self, player:str)](#get_scoreboard-self-playerstr)
-      - [`match_stats` (self, player:str)](#match_stats-self-playerstr)
+      - [***TennisMatch (self, player1:str, player2:str, matchFormat:dict=None)***](#tennismatch-self-player1str-player2str-matchformatdictnone)
+      - [***backup\_match ()***](#backup_match-)
+      - [***load\_backup (self, backup\_data)***](#load_backup-self-backup_data)
+      - [***win\_point (self, player:str, how\_won=\[\])***](#win_point-self-playerstr-how_won)
+      - [***serve\_fault (self, player:str)***](#serve_fault-self-playerstr)
+      - [***win\_game (self, player:str)***](#win_game-self-playerstr)
+      - [***win\_set (self, player:str)***](#win_set-self-playerstr)
+      - [***get\_all\_info (self)***](#get_all_info-self)
+      - [***get\_scoreboard (self, player:str)***](#get_scoreboard-self-playerstr)
+      - [***match\_stats (self, player:str)***](#match_stats-self-playerstr)
     - [Tiebreak Methods](#tiebreak-methods)
-      - [Tiebreak (self, player1:str, player2:str, matchFormat:dict=None)](#tiebreak-self-player1str-player2str-matchformatdictnone)
-      - [backup\_tiebreak ()](#backup_tiebreak-)
-      - [load\_backup (self, backup\_data)](#load_backup-self-backup_data-1)
-      - [`win_point` (self, player:str, how\_won=\[\])](#win_point-self-playerstr-how_won-1)
-      - [`tiebreak_stats` (self, player:str)](#tiebreak_stats-self-playerstr)
-      - [`get_scoreboard` (self, player:str)](#get_scoreboard-self-playerstr-1)
+      - [***tiebreak (self, player1:str, player2:str, matchFormat:dict=None)***](#tiebreak-self-player1str-player2str-matchformatdictnone)
+      - [***backup\_tiebreak ()***](#backup_tiebreak-)
+      - [***load\_backup (self, backup\_data)***](#load_backup-self-backup_data-1)
+      - [***win\_point (self, player:str, how\_won=\[\])***](#win_point-self-playerstr-how_won-1)
+      - [***tiebreak\_stats (self, player:str)***](#tiebreak_stats-self-playerstr)
+      - [***get\_scoreboard (self, player:str)***](#get_scoreboard-self-playerstr-1)
+
+
 
 
 ## [Features](#features)
 
 The Tennis library offers the following main features:
 <br>
 ### [1. Match Simulation](#1-match-simulation)
@@ -250,20 +238,18 @@
 ════════════════════════════════════════
 ```
 
 <br><br><br>
 
   
 
-### <h1>[Match Methods](#match-methods)</h1>
+### <h1>Match Methods</h1>
 
-
-#### [TennisMatch](#tennismatch) (self, player1:str, player2:str, matchFormat:dict=None)
+#### ***TennisMatch (self, player1:str, player2:str, matchFormat:dict=None)***
 Creates a new instance of a tennis match.
-
 **Parameters**
 
 - player1 (str): The name of player 1.
 - player2 (str): The name of player 2.
 - matchFormat (dict): A dictionary of match settings.
   
 **Example**
@@ -275,18 +261,18 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`backup_match`](#backup_match) ()
+#### ***<h3>backup_match ()</h3>***
 Creates a backup for the current tennis match instance
 
-#### [`load_backup`](#load_backup) (self, backup_data)
+#### ***<h3>load_backup (self, backup_data)</h3>***
 Loads a backup into a new match
 
 **Parameters**
 - backup_data (dict): The backup data created by the backup_match method
 
 
 **Example**
@@ -307,15 +293,15 @@
 
 ***
 
 <br>
 
 
 
-#### **[`win_point`](#win_point)** (self, player:str, how_won=[])
+#### ***<h3>win_point (self, player:str, how_won=[])</h3>***
 method that handles a player winning or loosing a point. Do not call this method if it is a double fault. Instead, call the [`serve_fault` (self, player:str)](#serve_fault-self-playerstr) method
 
 **Parameters**
 - player (str): The name of the player who won the point.
 - how_won (Array): How the point was won (more than 1 in a method call is ok, just append them to the end of the list like ['winner','win_by_volley'])
   - `Ace`: player A wins by by acing player b (Player A's serves the ball in and player B does not even touch the ball)
   - `winner`: player A wins the point by hitting a winner. (The opponent doesnt touch the ball at all)
@@ -334,15 +320,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`serve_fault`](#serve_fault) (self, player:str)
+#### ***<h3>serve_fault (self, player:str)</h3>***
 method to call when a server misses a first or second serve
 
 **Parameters**
 - player (str): The name of the player who missed the serve
 
 **Example**
 ```python
@@ -357,15 +343,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`win_game`](#win_game) (self, player:str)
+#### ***<h3>win_game (self, player:str)</h3>***
 A method that will win the game for a player. This method is intended for development and testing. The statistics for the match will be off.
 
 **Parameters**
 - player (str): the player that will win the game
 
 **Example**
 ```python
@@ -375,15 +361,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`win_set`](#win_set) (self, player:str)
+#### ***<h3>win_set (self, player:str)</h3>***
 A method that will win the set for a player. This method is intended for development and testing. The statistics for the match will be off.
 
 **Parameters**
 - player (str): the player that will win the set
 
 **Example**
 ```python
@@ -393,15 +379,15 @@
 <br>
 
 ***
 
 <br>
 
 
-#### [`get_all_info`](#get_all_info) (self)
+#### ***<h3>get_all_info (self)</h3>***
 A method that will return all the info about the match in a dictionary format
 
 ```python
 return {"winner":self.winner, "game_history":self.gameHistory, "set_history": self.setHistory, "set_tiebreak_history":self.setTieBreakScoresHistory, "match_tiebreak_history":self.matchTieBreakScore,"match_format":self.matchFormat,"match_stats":self.matchStats}
 ```
 
 **example output**
@@ -411,15 +397,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`get_scoreboard`](#get_scoreboard) (self, player:str)
+#### ***<h3>get_scoreboard (self, player:str)</h3>***
 A method that will return a string representation of the current scoreboard.
 
 **Parameters**
 - player (str): the player whos name and score will appear on the top half of the scoreboard
 
 **Example Output**
 
@@ -436,15 +422,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`match_stats`](#match_stats) (self, player:str)
+#### ***</h3>match_stats (self, player:str)</h3>***
 A method that will return the statistics about the match in a string format
 
 **Parameters**
 - player (str): the player who will appear on the left side of the stats
 
 **Example Output**
 ```python
@@ -481,17 +467,17 @@
 
 
 
 ════════════════════════════════════════
 ```
 <br><br>
 
-### <h1>[Tiebreak Methods](#tiebreak-methods)</h1>
+### <h1>Tiebreak Methods</h1>
 
-#### [Tiebreak](#tiebreak) (self, player1:str, player2:str, matchFormat:dict=None)
+#### ***<h3>tiebreak (self, player1:str, player2:str, matchFormat:dict=None)</h3>***
 Creates a new instance of a tiebreak.
 
 **Parameters**
 - player1 (str): the name of the first player
 - player2 (str): the name of the second player
 - matchFormat (dict): A dictionary of match settings.
 
@@ -502,24 +488,24 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [backup_tiebreak](#backup_tiebreak) ()
+#### ***<h3>backup_tiebreak ()</h3>***
 A method to backup tiebreak data
 
 **Example**
 ```python
 match = tiebreak("a","b",{"first_to_num_points":7, "win_by":2, "whos_serve":"a"})
 backup_data = match.backup_tiebreak()
 ```
 
-#### [load_backup](#load_backup) (self, backup_data)
+#### ***<h3>load_backup (self, backup_data)</h3>***
 A method to load backup data from another tiebreak object
 
 **Parameters**
 - backup_data (dict): the data to load. use the backup_tiebreak method to obtain this
 
 **Example**
 ```python
@@ -539,15 +525,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`win_point`](#win_point) (self, player:str, how_won=[])
+#### ***<h3>win_point (self, player:str, how_won=[])</h3>***
 method that handles a player winning or loosing a point. Do not call this method if it is a double fault. Instead, call the [`serve_fault` (self, player:str)](#serve_fault-self-playerstr) method
 **Parameters**
 - player (str): The name of the player who won the point.
 - how_won (Array): How the point was won (more than 1 in a method call is ok, just append them to the end of the list like ['winner','win_by_volley'])
   - `Ace`: player A wins by by acing player b (Player A's serves the ball in and player B does not even touch the ball)
   - `winner`: player A wins the point by hitting a winner. (The opponent doesnt touch the ball at all)
   - `unforced_error`: player A wins the point because player B made an unforced error (An error that was not caused by player A. For example player B got an easy ball and missed it)
@@ -565,15 +551,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`tiebreak_stats`](#tiebreak_stats) (self, player:str)
+#### ***<h3>tiebreak_stats (self, player:str)</h3>***
 A method that returns a string representation of the statistics of the tiebreak
 
 **Parameters**
 - player (str): the name of the player whos stats will be displayed on the left side
 
 **Example**
 ```python
@@ -583,15 +569,15 @@
 
 <br>
 
 ***
 
 <br>
 
-#### [`get_scoreboard`](#get_scoreboard) (self, player:str)
+#### ***<h3>get_scoreboard (self, player:str)</h3>***
 A method that returns a string representation of the current score
 
 **Parameters**
 - player (str): the name of the player whos stats will be displayed on the top of the scoreboard
 
 **Example**
 ```python
```

