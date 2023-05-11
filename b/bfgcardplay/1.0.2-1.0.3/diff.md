# Comparing `tmp/bfgcardplay-1.0.2.tar.gz` & `tmp/bfgcardplay-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfgcardplay-1.0.2.tar", last modified: Wed Mar  8 17:57:28 2023, max compression
+gzip compressed data, was "bfgcardplay-1.0.3.tar", last modified: Thu May 11 08:45:27 2023, max compression
```

## Comparing `bfgcardplay-1.0.2.tar` & `bfgcardplay-1.0.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-08 17:57:28.698224 bfgcardplay-1.0.2/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3686 2023-03-08 17:57:28.694891 bfgcardplay-1.0.2/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)        2 2021-07-03 11:00:43.000000 bfgcardplay-1.0.2/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-08 17:57:28.638224 bfgcardplay-1.0.2/bfgcardplay/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      227 2021-10-01 11:09:27.000000 bfgcardplay-1.0.2/bfgcardplay/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-03-08 17:55:15.000000 bfgcardplay-1.0.2/bfgcardplay/_version.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      912 2021-11-08 15:49:35.000000 bfgcardplay-1.0.2/bfgcardplay/logger.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-08 17:57:28.691557 bfgcardplay-1.0.2/bfgcardplay/source/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2021-12-22 17:41:36.000000 bfgcardplay-1.0.2/bfgcardplay/source/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3402 2021-12-22 17:41:36.000000 bfgcardplay-1.0.2/bfgcardplay/source/card_player_components.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2347 2023-01-20 16:29:14.000000 bfgcardplay-1.0.2/bfgcardplay/source/cards.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    19631 2023-01-05 11:19:24.000000 bfgcardplay-1.0.2/bfgcardplay/source/dashboard.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4715 2023-02-02 07:57:08.000000 bfgcardplay-1.0.2/bfgcardplay/source/data_classes.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    12323 2023-02-10 13:38:26.000000 bfgcardplay-1.0.2/bfgcardplay/source/declarer_play.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4085 2023-03-08 17:55:15.000000 bfgcardplay-1.0.2/bfgcardplay/source/defender_play.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     9806 2023-02-10 13:38:26.000000 bfgcardplay-1.0.2/bfgcardplay/source/first_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    16175 2023-02-03 17:43:49.000000 bfgcardplay-1.0.2/bfgcardplay/source/first_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    16647 2023-02-02 07:57:08.000000 bfgcardplay-1.0.2/bfgcardplay/source/first_seat_declarer_nt.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    22029 2023-02-02 07:57:08.000000 bfgcardplay-1.0.2/bfgcardplay/source/first_seat_declarer_suit.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    16559 2023-02-02 07:57:08.000000 bfgcardplay-1.0.2/bfgcardplay/source/first_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2791 2023-02-02 07:57:08.000000 bfgcardplay-1.0.2/bfgcardplay/source/fourth_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     5957 2023-02-02 07:57:08.000000 bfgcardplay-1.0.2/bfgcardplay/source/fourth_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4559 2023-02-02 07:57:08.000000 bfgcardplay-1.0.2/bfgcardplay/source/fourth_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      134 2021-12-22 17:41:36.000000 bfgcardplay-1.0.2/bfgcardplay/source/global_variables.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3966 2022-01-04 17:55:18.000000 bfgcardplay-1.0.2/bfgcardplay/source/manager.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      667 2022-06-27 17:02:41.000000 bfgcardplay-1.0.2/bfgcardplay/source/opening_lead.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6981 2023-01-20 16:49:44.000000 bfgcardplay-1.0.2/bfgcardplay/source/opening_lead_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    43121 2023-03-08 17:55:15.000000 bfgcardplay-1.0.2/bfgcardplay/source/opening_lead_suit.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    24155 2023-02-03 17:28:17.000000 bfgcardplay-1.0.2/bfgcardplay/source/player.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3052 2023-02-02 07:57:08.000000 bfgcardplay-1.0.2/bfgcardplay/source/second_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     9977 2023-02-02 07:57:08.000000 bfgcardplay-1.0.2/bfgcardplay/source/second_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     7234 2023-02-02 07:57:08.000000 bfgcardplay-1.0.2/bfgcardplay/source/second_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3672 2023-02-02 07:57:08.000000 bfgcardplay-1.0.2/bfgcardplay/source/suggested_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2428 2023-02-02 07:57:08.000000 bfgcardplay-1.0.2/bfgcardplay/source/third_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    17717 2023-02-02 07:57:08.000000 bfgcardplay-1.0.2/bfgcardplay/source/third_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    13898 2023-02-02 07:57:08.000000 bfgcardplay-1.0.2/bfgcardplay/source/third_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1483 2023-01-20 11:07:39.000000 bfgcardplay-1.0.2/bfgcardplay/source/utilities.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-08 17:57:28.694891 bfgcardplay-1.0.2/bfgcardplay/test/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2021-10-25 15:12:22.000000 bfgcardplay-1.0.2/bfgcardplay/test/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    11741 2023-01-20 16:48:53.000000 bfgcardplay-1.0.2/bfgcardplay/test/test_opening_lead_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    14967 2023-01-20 17:51:03.000000 bfgcardplay-1.0.2/bfgcardplay/test/test_opening_lead_suit.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-08 17:57:28.644891 bfgcardplay-1.0.2/bfgcardplay.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3686 2023-03-08 17:57:28.000000 bfgcardplay-1.0.2/bfgcardplay.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1434 2023-03-08 17:57:28.000000 bfgcardplay-1.0.2/bfgcardplay.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-03-08 17:57:28.000000 bfgcardplay-1.0.2/bfgcardplay.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       12 2023-03-08 17:57:28.000000 bfgcardplay-1.0.2/bfgcardplay.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-03-08 17:57:28.698224 bfgcardplay-1.0.2/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1284 2021-07-03 11:10:30.000000 bfgcardplay-1.0.2/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:45:27.798407 bfgcardplay-1.0.3/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3757 2023-05-11 08:45:27.798407 bfgcardplay-1.0.3/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        2 2021-07-03 11:00:43.000000 bfgcardplay-1.0.3/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:45:27.768407 bfgcardplay-1.0.3/bfgcardplay/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      227 2021-10-01 11:09:27.000000 bfgcardplay-1.0.3/bfgcardplay/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-11 08:43:28.000000 bfgcardplay-1.0.3/bfgcardplay/_version.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      912 2021-11-08 15:49:35.000000 bfgcardplay-1.0.3/bfgcardplay/logger.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:45:27.791740 bfgcardplay-1.0.3/bfgcardplay/source/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2021-12-22 17:41:36.000000 bfgcardplay-1.0.3/bfgcardplay/source/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3402 2021-12-22 17:41:36.000000 bfgcardplay-1.0.3/bfgcardplay/source/card_player_components.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2347 2023-01-20 16:29:14.000000 bfgcardplay-1.0.3/bfgcardplay/source/cards.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    19631 2023-01-05 11:19:24.000000 bfgcardplay-1.0.3/bfgcardplay/source/dashboard.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4714 2023-05-11 08:43:28.000000 bfgcardplay-1.0.3/bfgcardplay/source/data_classes.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    12323 2023-02-10 13:38:26.000000 bfgcardplay-1.0.3/bfgcardplay/source/declarer_play.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4085 2023-03-08 17:55:15.000000 bfgcardplay-1.0.3/bfgcardplay/source/defender_play.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     9806 2023-02-10 13:38:26.000000 bfgcardplay-1.0.3/bfgcardplay/source/first_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    16175 2023-02-03 17:43:49.000000 bfgcardplay-1.0.3/bfgcardplay/source/first_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    17044 2023-05-11 08:43:28.000000 bfgcardplay-1.0.3/bfgcardplay/source/first_seat_declarer_nt.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    22029 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/first_seat_declarer_suit.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    16559 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/first_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2791 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/fourth_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     5957 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/fourth_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4836 2023-05-11 08:43:28.000000 bfgcardplay-1.0.3/bfgcardplay/source/fourth_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      134 2021-12-22 17:41:36.000000 bfgcardplay-1.0.3/bfgcardplay/source/global_variables.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3966 2022-01-04 17:55:18.000000 bfgcardplay-1.0.3/bfgcardplay/source/manager.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      667 2022-06-27 17:02:41.000000 bfgcardplay-1.0.3/bfgcardplay/source/opening_lead.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     6981 2023-01-20 16:49:44.000000 bfgcardplay-1.0.3/bfgcardplay/source/opening_lead_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    43121 2023-03-08 17:55:15.000000 bfgcardplay-1.0.3/bfgcardplay/source/opening_lead_suit.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    24518 2023-05-11 08:43:28.000000 bfgcardplay-1.0.3/bfgcardplay/source/player.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3052 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/second_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     9977 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/second_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     7234 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/second_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3672 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/suggested_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2428 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/third_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    17717 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/third_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    13898 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/third_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1483 2023-01-20 11:07:39.000000 bfgcardplay-1.0.3/bfgcardplay/source/utilities.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:45:27.798407 bfgcardplay-1.0.3/bfgcardplay/test/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2021-10-25 15:12:22.000000 bfgcardplay-1.0.3/bfgcardplay/test/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    11741 2023-01-20 16:48:53.000000 bfgcardplay-1.0.3/bfgcardplay/test/test_opening_lead_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    14967 2023-01-20 17:51:03.000000 bfgcardplay-1.0.3/bfgcardplay/test/test_opening_lead_suit.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:45:27.768407 bfgcardplay-1.0.3/bfgcardplay.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3757 2023-05-11 08:45:27.000000 bfgcardplay-1.0.3/bfgcardplay.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1434 2023-05-11 08:45:27.000000 bfgcardplay-1.0.3/bfgcardplay.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-11 08:45:27.000000 bfgcardplay-1.0.3/bfgcardplay.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       12 2023-05-11 08:45:27.000000 bfgcardplay-1.0.3/bfgcardplay.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-11 08:45:27.798407 bfgcardplay-1.0.3/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1284 2021-07-03 11:10:30.000000 bfgcardplay-1.0.3/setup.py
```

### Comparing `bfgcardplay-1.0.2/PKG-INFO` & `bfgcardplay-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: bfgcardplay
-Version: 1.0.2
+Version: 1.0.3
 Summary: A collection of modules that facilitate cardplay in the BfG environment.
 Home-page: https://psionman@bitbucket.org/psionman/bfgcardplay.git
 Download-URL: https://pypi.org/project/bfgcardplay/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, duplicate bridge, contract bridge, hand, board, suit, auction, contract, card
 Description-Content-Type: text/markdown
 
  
 
 
 # Version History
 
+Version 1.0.3 11 May 2023
+
+1. Correct manager.suit_to_develop
+
+------
+
 Version 1.0.2 08 Mar 2023
 
 1. Fix dummy long suit on first lead
 2. Stop using T as HiLo signal
 
 ------
```

### Comparing `bfgcardplay-1.0.2/bfgcardplay/logger.py` & `bfgcardplay-1.0.3/bfgcardplay/logger.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/card_player_components.py` & `bfgcardplay-1.0.3/bfgcardplay/source/card_player_components.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/cards.py` & `bfgcardplay-1.0.3/bfgcardplay/source/cards.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/dashboard.py` & `bfgcardplay-1.0.3/bfgcardplay/source/dashboard.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/data_classes.py` & `bfgcardplay-1.0.3/bfgcardplay/source/data_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 
     @property
     def value(self) -> int:
         """Return the sum of the values of the cards."""
         return self._value
 
 
-
 class SuitCards():
     """Represent all of the cards in a suit by name."""
     def __init__(self, suit: str):
         self.suit = suit
         self.ace = Card('A', suit)
         self.king = Card('K', suit)
         self.queen = Card('Q', suit)
```

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/declarer_play.py` & `bfgcardplay-1.0.3/bfgcardplay/source/declarer_play.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/defender_play.py` & `bfgcardplay-1.0.3/bfgcardplay/source/defender_play.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/first_seat.py` & `bfgcardplay-1.0.3/bfgcardplay/source/first_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/first_seat_declarer.py` & `bfgcardplay-1.0.3/bfgcardplay/source/first_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/first_seat_declarer_nt.py` & `bfgcardplay-1.0.3/bfgcardplay/source/first_seat_declarer_nt.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,16 @@
             return log(inspect.stack(), card)
         return None
 
     def _select_suit(self) -> Suit:
         """Return the trick lead suit for the declarer in  a suit contract."""
         player = self.player
         manager = global_vars.manager
+        if manager.suit_to_develop(player.seat):
+            self._check_suit_to_develop()
 
         # Look for suit to develop
         # print(colored(f'{dashboard.tricks_needed=}', MODULE_COLOUR))
         # print(colored(f'{dashboard.sure_tricks.count=}', MODULE_COLOUR))
         # print(colored(f'{dashboard.sure_tricks.cards=}', MODULE_COLOUR))
         # print(colored(f'{player.declarers_tricks=}', MODULE_COLOUR))
         # print(colored(f'{dashboard.probable_tricks.cards=}', MODULE_COLOUR))
@@ -189,14 +191,21 @@
         suit = self._find_suit_to_develop()
         if suit:
             return suit
 
         # Find best suit
         return self._select_best_suit()
 
+    def _check_suit_to_develop(self):
+        player = self.player
+        manager = global_vars.manager
+        suit = manager.suit_to_develop(player.seat)
+        card = player.unplayed_cards[suit][0]
+        if not player.is_master_card(card):
+            manager.set_suit_to_develop(player.seat, None)
 
     def _play_winner_no_entry(self):
         player = self.player
         dashboard = player.dashboard
         tricks_needed = dashboard.tricks_needed - player.declarers_tricks
         if tricks_needed <= dashboard.sure_tricks.count:
             for suit in SUITS:
```

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/first_seat_declarer_suit.py` & `bfgcardplay-1.0.3/bfgcardplay/source/first_seat_declarer_suit.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/first_seat_defender.py` & `bfgcardplay-1.0.3/bfgcardplay/source/first_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/fourth_seat.py` & `bfgcardplay-1.0.3/bfgcardplay/source/fourth_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/fourth_seat_declarer.py` & `bfgcardplay-1.0.3/bfgcardplay/source/fourth_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/fourth_seat_defender.py` & `bfgcardplay-1.0.3/bfgcardplay/source/fourth_seat_defender.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Fourth seat card play for defender."""
 
 import random
 from typing import Union
+
 from bridgeobjects.source.constants import CARD_VALUES
 from termcolor import cprint
 
 import inspect
 from ..logger import log
 
 from bridgeobjects import SUITS, Card, Suit
@@ -72,19 +73,26 @@
             (value_0, value_1, value_2) = self._trick_card_values(trick, player.trump_suit)
             if player.trump_cards:
                 if value_0 > value_1 or value_2 > value_1:
                     for card in player.trump_cards[::-1]:
                         if card.value + 13 > value_0 and card.value + 13 > value_2:
                             return log(inspect.stack(), card)
 
+        # Do not signal with winners
+        for suit in SUITS:
+            for card in player.unplayed_cards[suit]:
+                if not player.is_master_card(card):
+                    return log(inspect.stack(), card)
+
         # Signal best suit
         best_suit = self._best_suit()
         card = signal_card(player, manager, best_suit)
         if card:
-            return log(inspect.stack(), card)
+            if not player.is_master_card(card):
+                return log(inspect.stack(), card)
 
         # Discard if more cards than the opposition
         card = surplus_card(player)
         if card:
             return log(inspect.stack(), card)
 
         # Best discard
```

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/manager.py` & `bfgcardplay-1.0.3/bfgcardplay/source/manager.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/opening_lead.py` & `bfgcardplay-1.0.3/bfgcardplay/source/opening_lead.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/opening_lead_card.py` & `bfgcardplay-1.0.3/bfgcardplay/source/opening_lead_card.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/opening_lead_suit.py` & `bfgcardplay-1.0.3/bfgcardplay/source/opening_lead_suit.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/player.py` & `bfgcardplay-1.0.3/bfgcardplay/source/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,16 @@
         partners_seat = SEATS[partners_index]
         return partners_seat
 
     def _get_seat(self) -> str:
         """Return the current user's seat."""
         trick = self.board.tricks[-1]
         leader = trick.leader
+        if trick.winner:
+            leader = trick.winner
         leader_index = SEATS.index(leader)
         seat_index = (leader_index + len(trick.cards)) % 4
         seat = SEATS[seat_index]
         return seat
 
     def cards_for_trick_suit(self, trick: Trick) -> List[Card]:
         """Return a list of cards in the trick suit."""
@@ -353,14 +355,23 @@
             for card in cards:
                 if self._is_master(card, entries):
                     entries[suit_name].append(card)
                 else:
                     break
         return entries
 
+    def is_master_card(self, card: Card) -> bool:
+        """Return True if card is a master."""
+        unplayed_cards = self.total_unplayed_cards[card.suit]
+        for unplayed_card in unplayed_cards:
+            if unplayed_card.value > card.value:
+                return False
+        return True
+
+
     def _is_master(self, card: Card, other_masters: Dict[str, List[Card]]) -> bool:
         """Return True if card is a master."""
         # unplayed_cards = [unplayed_card for unplayed_card in self.unplayed_cards[card.suit.name]]
         unplayed_cards = self.total_unplayed_cards[card.suit]
         for master_card in other_masters[card.suit.name]:
             if master_card in unplayed_cards:
                 unplayed_cards.remove(master_card)
```

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/second_seat.py` & `bfgcardplay-1.0.3/bfgcardplay/source/second_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/second_seat_declarer.py` & `bfgcardplay-1.0.3/bfgcardplay/source/second_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/second_seat_defender.py` & `bfgcardplay-1.0.3/bfgcardplay/source/second_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/suggested_card.py` & `bfgcardplay-1.0.3/bfgcardplay/source/suggested_card.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/third_seat.py` & `bfgcardplay-1.0.3/bfgcardplay/source/third_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/third_seat_declarer.py` & `bfgcardplay-1.0.3/bfgcardplay/source/third_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/third_seat_defender.py` & `bfgcardplay-1.0.3/bfgcardplay/source/third_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/source/utilities.py` & `bfgcardplay-1.0.3/bfgcardplay/source/utilities.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/test/test_opening_lead_card.py` & `bfgcardplay-1.0.3/bfgcardplay/test/test_opening_lead_card.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay/test/test_opening_lead_suit.py` & `bfgcardplay-1.0.3/bfgcardplay/test/test_opening_lead_suit.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/bfgcardplay.egg-info/PKG-INFO` & `bfgcardplay-1.0.3/bfgcardplay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: bfgcardplay
-Version: 1.0.2
+Version: 1.0.3
 Summary: A collection of modules that facilitate cardplay in the BfG environment.
 Home-page: https://psionman@bitbucket.org/psionman/bfgcardplay.git
 Download-URL: https://pypi.org/project/bfgcardplay/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, duplicate bridge, contract bridge, hand, board, suit, auction, contract, card
 Description-Content-Type: text/markdown
 
  
 
 
 # Version History
 
+Version 1.0.3 11 May 2023
+
+1. Correct manager.suit_to_develop
+
+------
+
 Version 1.0.2 08 Mar 2023
 
 1. Fix dummy long suit on first lead
 2. Stop using T as HiLo signal
 
 ------
```

### Comparing `bfgcardplay-1.0.2/bfgcardplay.egg-info/SOURCES.txt` & `bfgcardplay-1.0.3/bfgcardplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.2/setup.py` & `bfgcardplay-1.0.3/setup.py`

 * *Files identical despite different names*

