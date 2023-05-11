# Comparing `tmp/play-poker-0.1.0.tar.gz` & `tmp/play-poker-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "play-poker-0.1.0.tar", last modified: Thu May 11 03:22:48 2023, max compression
+gzip compressed data, was "play-poker-0.1.2.tar", last modified: Thu May 11 05:09:51 2023, max compression
```

## Comparing `play-poker-0.1.0.tar` & `play-poker-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1772 2023-05-11 03:22:40.751881 play-poker-0.1.0/README.md
--rw-r--r--   0        0        0       83 2023-05-11 03:22:40.751881 play-poker-0.1.0/poker/__init__.py
--rw-r--r--   0        0        0      245 2023-05-11 03:22:40.751881 play-poker-0.1.0/poker/__main__.py
--rw-r--r--   0        0        0        0 2023-05-11 03:22:40.755881 play-poker-0.1.0/poker/utils/__init__.py
--rw-r--r--   0        0        0      727 2023-05-11 03:22:40.755881 play-poker-0.1.0/poker/utils/action.py
--rw-r--r--   0        0        0      378 2023-05-11 03:22:40.755881 play-poker-0.1.0/poker/utils/card.py
--rw-r--r--   0        0        0     1975 2023-05-11 03:22:40.755881 play-poker-0.1.0/poker/utils/chip.py
--rw-r--r--   0        0        0     1044 2023-05-11 03:22:40.755881 play-poker-0.1.0/poker/utils/constants.py
--rw-r--r--   0        0        0      557 2023-05-11 03:22:40.755881 play-poker-0.1.0/poker/utils/deck.py
--rw-r--r--   0        0        0     1251 2023-05-11 03:22:40.755881 play-poker-0.1.0/poker/utils/exception.py
--rw-r--r--   0        0        0    24061 2023-05-11 03:22:40.755881 play-poker-0.1.0/poker/utils/game.py
--rw-r--r--   0        0        0     7615 2023-05-11 03:22:40.755881 play-poker-0.1.0/poker/utils/message.py
--rw-r--r--   0        0        0     3092 2023-05-11 03:22:40.755881 play-poker-0.1.0/poker/utils/player.py
--rw-r--r--   0        0        0      507 2023-05-11 03:22:40.755881 play-poker-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 play-poker-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1772 2023-05-11 05:09:44.623231 play-poker-0.1.2/README.md
+-rw-r--r--   0        0        0       83 2023-05-11 05:09:44.623231 play-poker-0.1.2/poker/__init__.py
+-rw-r--r--   0        0        0      245 2023-05-11 05:09:44.623231 play-poker-0.1.2/poker/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:09:44.623231 play-poker-0.1.2/poker/utils/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-11 05:09:44.623231 play-poker-0.1.2/poker/utils/action.py
+-rw-r--r--   0        0        0      378 2023-05-11 05:09:44.623231 play-poker-0.1.2/poker/utils/card.py
+-rw-r--r--   0        0        0     1975 2023-05-11 05:09:44.623231 play-poker-0.1.2/poker/utils/chip.py
+-rw-r--r--   0        0        0     1044 2023-05-11 05:09:44.623231 play-poker-0.1.2/poker/utils/constants.py
+-rw-r--r--   0        0        0      557 2023-05-11 05:09:44.623231 play-poker-0.1.2/poker/utils/deck.py
+-rw-r--r--   0        0        0     1251 2023-05-11 05:09:44.623231 play-poker-0.1.2/poker/utils/exception.py
+-rw-r--r--   0        0        0    24061 2023-05-11 05:09:44.623231 play-poker-0.1.2/poker/utils/game.py
+-rw-r--r--   0        0        0     7615 2023-05-11 05:09:44.623231 play-poker-0.1.2/poker/utils/message.py
+-rw-r--r--   0        0        0     3092 2023-05-11 05:09:44.623231 play-poker-0.1.2/poker/utils/player.py
+-rw-r--r--   0        0        0      564 2023-05-11 05:09:44.623231 play-poker-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2249 1970-01-01 00:00:00.000000 play-poker-0.1.2/PKG-INFO
```

### Comparing `play-poker-0.1.0/README.md` & `play-poker-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `play-poker-0.1.0/poker/utils/action.py` & `play-poker-0.1.2/poker/utils/action.py`

 * *Files identical despite different names*

### Comparing `play-poker-0.1.0/poker/utils/chip.py` & `play-poker-0.1.2/poker/utils/chip.py`

 * *Files identical despite different names*

### Comparing `play-poker-0.1.0/poker/utils/constants.py` & `play-poker-0.1.2/poker/utils/constants.py`

 * *Files identical despite different names*

### Comparing `play-poker-0.1.0/poker/utils/deck.py` & `play-poker-0.1.2/poker/utils/deck.py`

 * *Files identical despite different names*

### Comparing `play-poker-0.1.0/poker/utils/exception.py` & `play-poker-0.1.2/poker/utils/exception.py`

 * *Files identical despite different names*

### Comparing `play-poker-0.1.0/poker/utils/game.py` & `play-poker-0.1.2/poker/utils/game.py`

 * *Files identical despite different names*

### Comparing `play-poker-0.1.0/poker/utils/message.py` & `play-poker-0.1.2/poker/utils/message.py`

 * *Files identical despite different names*

### Comparing `play-poker-0.1.0/poker/utils/player.py` & `play-poker-0.1.2/poker/utils/player.py`

 * *Files identical despite different names*

### Comparing `play-poker-0.1.0/PKG-INFO` & `play-poker-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: play-poker
-Version: 0.1.0
+Version: 0.1.2
 Summary: Command Line Single-player game of Texas Hold'Em poker
 Keywords: poker,games,cards,texas holdem
 Author: Ben Griffith
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
+Requires-Dist: emoji
+Requires-Dist: Faker
+Requires-Dist: rich
 Requires-Dist: pytest ; extra == "test"
 Project-URL: Source, https://github.com/bengriffith/poker
 Provides-Extra: test
 
 ## General Info
 Command Line Single-player game of Texas Hold'Em poker.
```

