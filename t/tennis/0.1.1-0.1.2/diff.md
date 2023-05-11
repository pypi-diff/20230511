# Comparing `tmp/tennis-0.1.1.tar.gz` & `tmp/tennis-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tennis-0.1.1.tar", last modified: Wed May 10 21:43:05 2023, max compression
+gzip compressed data, was "tennis-0.1.2.tar", last modified: Thu May 11 02:25:55 2023, max compression
```

## Comparing `tennis-0.1.1.tar` & `tennis-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 21:43:05.326835 tennis-0.1.1/
--rw-rw-rw-   0        0        0     1083 2023-05-09 03:08:15.000000 tennis-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     5443 2023-05-10 21:43:05.325837 tennis-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5002 2023-05-10 21:40:09.000000 tennis-0.1.1/README.md
--rw-rw-rw-   0        0        0      516 2023-05-10 21:42:49.000000 tennis-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 21:43:05.326835 tennis-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      284 2023-05-10 21:42:53.000000 tennis-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 21:43:05.315358 tennis-0.1.1/tennis/
--rw-rw-rw-   0        0        0        0 2023-05-06 20:11:19.000000 tennis-0.1.1/tennis/__init__.py
--rw-rw-rw-   0        0        0    30932 2023-05-09 03:05:50.000000 tennis-0.1.1/tennis/match.py
--rw-rw-rw-   0        0        0    17036 2023-05-10 21:30:40.000000 tennis-0.1.1/tennis/tiebreak.py
-drwxrwxrwx   0        0        0        0 2023-05-10 21:43:05.324839 tennis-0.1.1/tennis.egg-info/
--rw-rw-rw-   0        0        0     5443 2023-05-10 21:43:05.000000 tennis-0.1.1/tennis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-05-10 21:43:05.000000 tennis-0.1.1/tennis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 21:43:05.000000 tennis-0.1.1/tennis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-10 21:43:05.000000 tennis-0.1.1/tennis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 02:25:55.873822 tennis-0.1.2/
+-rw-rw-rw-   0        0        0     1083 2023-05-09 03:08:15.000000 tennis-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0    17775 2023-05-11 02:25:55.873822 tennis-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    17334 2023-05-11 02:23:09.000000 tennis-0.1.2/README.md
+-rw-rw-rw-   0        0        0      516 2023-05-11 02:23:31.000000 tennis-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 02:25:55.873822 tennis-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      284 2023-05-11 02:23:35.000000 tennis-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:25:55.856867 tennis-0.1.2/tennis/
+-rw-rw-rw-   0        0        0        0 2023-05-06 20:11:19.000000 tennis-0.1.2/tennis/__init__.py
+-rw-rw-rw-   0        0        0    30931 2023-05-11 01:21:55.000000 tennis-0.1.2/tennis/match.py
+-rw-rw-rw-   0        0        0    17036 2023-05-10 21:30:40.000000 tennis-0.1.2/tennis/tiebreak.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:25:55.871826 tennis-0.1.2/tennis.egg-info/
+-rw-rw-rw-   0        0        0    17775 2023-05-11 02:25:55.000000 tennis-0.1.2/tennis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-05-11 02:25:55.000000 tennis-0.1.2/tennis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 02:25:55.000000 tennis-0.1.2/tennis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-11 02:25:55.000000 tennis-0.1.2/tennis.egg-info/top_level.txt
```

### Comparing `tennis-0.1.1/LICENSE` & `tennis-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tennis-0.1.1/pyproject.toml` & `tennis-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tennis"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="bear102" },
 ]
 description = "A library for tracking tennis matches and scoring"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tennis-0.1.1/tennis/match.py` & `tennis-0.1.2/tennis/match.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,15 +521,15 @@
         self.check_match_win(player)
 
 
 #---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------#
 
     # Returns a dictionary with match results and info including statistics and score history.
 
-    def match_results(self):
+    def get_all_info(self):
         """
         returns a dictionary with all the info about the match
 
         """
         return {"winner":self.winner, "game_history":self.gameHistory, "set_history": self.setHistory, "set_tiebreak_history":self.setTieBreakScoresHistory, "match_tiebreak_history":self.matchTieBreakScore,"match_format":self.matchFormat,"match_stats":self.matchStats}
 
 #---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------#
```

### Comparing `tennis-0.1.1/tennis/tiebreak.py` & `tennis-0.1.2/tennis/tiebreak.py`

 * *Files identical despite different names*

