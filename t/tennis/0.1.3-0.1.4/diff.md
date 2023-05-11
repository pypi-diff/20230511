# Comparing `tmp/tennis-0.1.3.tar.gz` & `tmp/tennis-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tennis-0.1.3.tar", last modified: Thu May 11 03:31:56 2023, max compression
+gzip compressed data, was "tennis-0.1.4.tar", last modified: Thu May 11 03:33:51 2023, max compression
```

## Comparing `tennis-0.1.3.tar` & `tennis-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 03:31:56.976299 tennis-0.1.3/
--rw-rw-rw-   0        0        0     1083 2023-05-09 03:08:15.000000 tennis-0.1.3/LICENSE
--rw-rw-rw-   0        0        0    17810 2023-05-11 03:31:56.976299 tennis-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    17323 2023-05-11 03:16:20.000000 tennis-0.1.3/README.md
--rw-rw-rw-   0        0        0      516 2023-05-11 03:31:38.000000 tennis-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 03:31:56.976299 tennis-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      330 2023-05-11 03:31:35.000000 tennis-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 03:31:56.962336 tennis-0.1.3/tennis/
--rw-rw-rw-   0        0        0        0 2023-05-06 20:11:19.000000 tennis-0.1.3/tennis/__init__.py
--rw-rw-rw-   0        0        0    30931 2023-05-11 01:21:55.000000 tennis-0.1.3/tennis/match.py
--rw-rw-rw-   0        0        0    17036 2023-05-10 21:30:40.000000 tennis-0.1.3/tennis/tiebreak.py
-drwxrwxrwx   0        0        0        0 2023-05-11 03:31:56.974304 tennis-0.1.3/tennis.egg-info/
--rw-rw-rw-   0        0        0    17810 2023-05-11 03:31:56.000000 tennis-0.1.3/tennis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-05-11 03:31:56.000000 tennis-0.1.3/tennis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 03:31:56.000000 tennis-0.1.3/tennis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-11 03:31:56.000000 tennis-0.1.3/tennis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 03:33:51.147351 tennis-0.1.4/
+-rw-rw-rw-   0        0        0     1083 2023-05-09 03:08:15.000000 tennis-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0    16039 2023-05-11 03:33:51.147351 tennis-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    15552 2023-05-11 03:33:28.000000 tennis-0.1.4/README.md
+-rw-rw-rw-   0        0        0      516 2023-05-11 03:33:39.000000 tennis-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 03:33:51.148349 tennis-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      330 2023-05-11 03:33:34.000000 tennis-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 03:33:51.132390 tennis-0.1.4/tennis/
+-rw-rw-rw-   0        0        0        0 2023-05-06 20:11:19.000000 tennis-0.1.4/tennis/__init__.py
+-rw-rw-rw-   0        0        0    30931 2023-05-11 01:21:55.000000 tennis-0.1.4/tennis/match.py
+-rw-rw-rw-   0        0        0    17036 2023-05-10 21:30:40.000000 tennis-0.1.4/tennis/tiebreak.py
+drwxrwxrwx   0        0        0        0 2023-05-11 03:33:51.145357 tennis-0.1.4/tennis.egg-info/
+-rw-rw-rw-   0        0        0    16039 2023-05-11 03:33:51.000000 tennis-0.1.4/tennis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-05-11 03:33:51.000000 tennis-0.1.4/tennis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 03:33:51.000000 tennis-0.1.4/tennis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-11 03:33:51.000000 tennis-0.1.4/tennis.egg-info/top_level.txt
```

### Comparing `tennis-0.1.3/LICENSE` & `tennis-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tennis-0.1.3/PKG-INFO` & `tennis-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tennis
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library for tracking tennis matches and scoring
 Home-page: https://github.com/bear102/tennis
 Author: bear102
 License: MIT
 Project-URL: Homepage, https://github.com/bear102/tennis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,41 +19,15 @@
 ![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 The Tennis library is a Python package that provides functionalities for simulating tennis matches and tiebreakers. It offers easy-to-use methods to simulate and track scores, tiebreakers, and various statistics. The tennis library is perfect for tracking real time data input.
 
 <br>
 
-## **Table Of Contents**
-- [Tennis Library](#tennis-library)
-  - [**Table Of Contents**](#table-of-contents)
-  - [Features](#features)
-    - [1. Match Simulation](#1-match-simulation)
-    - [2. Tiebreaker](#2-tiebreaker)
-    - [Tracking Stats](#tracking-stats)
-  - [Usage](#usage)
-    - [Quick Start](#quick-start)
-    - [Match Methods](#match-methods)
-      - [***TennisMatch (self, player1:str, player2:str, matchFormat:dict=None)***](#tennismatch-self-player1str-player2str-matchformatdictnone)
-      - [***backup\_match ()***](#backup_match-)
-      - [***load\_backup (self, backup\_data)***](#load_backup-self-backup_data)
-      - [***win\_point (self, player:str, how\_won=\[\])***](#win_point-self-playerstr-how_won)
-      - [***serve\_fault (self, player:str)***](#serve_fault-self-playerstr)
-      - [***win\_game (self, player:str)***](#win_game-self-playerstr)
-      - [***win\_set (self, player:str)***](#win_set-self-playerstr)
-      - [***get\_all\_info (self)***](#get_all_info-self)
-      - [***get\_scoreboard (self, player:str)***](#get_scoreboard-self-playerstr)
-      - [***match\_stats (self, player:str)***](#match_stats-self-playerstr)
-    - [Tiebreak Methods](#tiebreak-methods)
-      - [***tiebreak (self, player1:str, player2:str, matchFormat:dict=None)***](#tiebreak-self-player1str-player2str-matchformatdictnone)
-      - [***backup\_tiebreak ()***](#backup_tiebreak-)
-      - [***load\_backup (self, backup\_data)***](#load_backup-self-backup_data-1)
-      - [***win\_point (self, player:str, how\_won=\[\])***](#win_point-self-playerstr-how_won-1)
-      - [***tiebreak\_stats (self, player:str)***](#tiebreak_stats-self-playerstr)
-      - [***get\_scoreboard (self, player:str)***](#get_scoreboard-self-playerstr-1)
+
 
 
 
 
 ## [Features](#features)
 
 The Tennis library offers the following main features:
```

### Comparing `tennis-0.1.3/README.md` & `tennis-0.1.4/tennis.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,33 @@
+Metadata-Version: 2.1
+Name: tennis
+Version: 0.1.4
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
 
 <br>
 
-## **Table Of Contents**
-- [Tennis Library](#tennis-library)
-  - [**Table Of Contents**](#table-of-contents)
-  - [Features](#features)
-    - [1. Match Simulation](#1-match-simulation)
-    - [2. Tiebreaker](#2-tiebreaker)
-    - [Tracking Stats](#tracking-stats)
-  - [Usage](#usage)
-    - [Quick Start](#quick-start)
-    - [Match Methods](#match-methods)
-      - [***TennisMatch (self, player1:str, player2:str, matchFormat:dict=None)***](#tennismatch-self-player1str-player2str-matchformatdictnone)
-      - [***backup\_match ()***](#backup_match-)
-      - [***load\_backup (self, backup\_data)***](#load_backup-self-backup_data)
-      - [***win\_point (self, player:str, how\_won=\[\])***](#win_point-self-playerstr-how_won)
-      - [***serve\_fault (self, player:str)***](#serve_fault-self-playerstr)
-      - [***win\_game (self, player:str)***](#win_game-self-playerstr)
-      - [***win\_set (self, player:str)***](#win_set-self-playerstr)
-      - [***get\_all\_info (self)***](#get_all_info-self)
-      - [***get\_scoreboard (self, player:str)***](#get_scoreboard-self-playerstr)
-      - [***match\_stats (self, player:str)***](#match_stats-self-playerstr)
-    - [Tiebreak Methods](#tiebreak-methods)
-      - [***tiebreak (self, player1:str, player2:str, matchFormat:dict=None)***](#tiebreak-self-player1str-player2str-matchformatdictnone)
-      - [***backup\_tiebreak ()***](#backup_tiebreak-)
-      - [***load\_backup (self, backup\_data)***](#load_backup-self-backup_data-1)
-      - [***win\_point (self, player:str, how\_won=\[\])***](#win_point-self-playerstr-how_won-1)
-      - [***tiebreak\_stats (self, player:str)***](#tiebreak_stats-self-playerstr)
-      - [***get\_scoreboard (self, player:str)***](#get_scoreboard-self-playerstr-1)
+
 
 
 
 
 ## [Features](#features)
 
 The Tennis library offers the following main features:
```

### Comparing `tennis-0.1.3/pyproject.toml` & `tennis-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tennis"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="bear102" },
 ]
 description = "A library for tracking tennis matches and scoring"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tennis-0.1.3/tennis/match.py` & `tennis-0.1.4/tennis/match.py`

 * *Files identical despite different names*

### Comparing `tennis-0.1.3/tennis/tiebreak.py` & `tennis-0.1.4/tennis/tiebreak.py`

 * *Files identical despite different names*

### Comparing `tennis-0.1.3/tennis.egg-info/PKG-INFO` & `tennis-0.1.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,18 @@
-Metadata-Version: 2.1
-Name: tennis
-Version: 0.1.3
-Summary: A library for tracking tennis matches and scoring
-Home-page: https://github.com/bear102/tennis
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
 
 <br>
 
-## **Table Of Contents**
-- [Tennis Library](#tennis-library)
-  - [**Table Of Contents**](#table-of-contents)
-  - [Features](#features)
-    - [1. Match Simulation](#1-match-simulation)
-    - [2. Tiebreaker](#2-tiebreaker)
-    - [Tracking Stats](#tracking-stats)
-  - [Usage](#usage)
-    - [Quick Start](#quick-start)
-    - [Match Methods](#match-methods)
-      - [***TennisMatch (self, player1:str, player2:str, matchFormat:dict=None)***](#tennismatch-self-player1str-player2str-matchformatdictnone)
-      - [***backup\_match ()***](#backup_match-)
-      - [***load\_backup (self, backup\_data)***](#load_backup-self-backup_data)
-      - [***win\_point (self, player:str, how\_won=\[\])***](#win_point-self-playerstr-how_won)
-      - [***serve\_fault (self, player:str)***](#serve_fault-self-playerstr)
-      - [***win\_game (self, player:str)***](#win_game-self-playerstr)
-      - [***win\_set (self, player:str)***](#win_set-self-playerstr)
-      - [***get\_all\_info (self)***](#get_all_info-self)
-      - [***get\_scoreboard (self, player:str)***](#get_scoreboard-self-playerstr)
-      - [***match\_stats (self, player:str)***](#match_stats-self-playerstr)
-    - [Tiebreak Methods](#tiebreak-methods)
-      - [***tiebreak (self, player1:str, player2:str, matchFormat:dict=None)***](#tiebreak-self-player1str-player2str-matchformatdictnone)
-      - [***backup\_tiebreak ()***](#backup_tiebreak-)
-      - [***load\_backup (self, backup\_data)***](#load_backup-self-backup_data-1)
-      - [***win\_point (self, player:str, how\_won=\[\])***](#win_point-self-playerstr-how_won-1)
-      - [***tiebreak\_stats (self, player:str)***](#tiebreak_stats-self-playerstr)
-      - [***get\_scoreboard (self, player:str)***](#get_scoreboard-self-playerstr-1)
+
 
 
 
 
 ## [Features](#features)
 
 The Tennis library offers the following main features:
```

