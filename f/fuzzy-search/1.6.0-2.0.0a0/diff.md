# Comparing `tmp/fuzzy_search-1.6.0.tar.gz` & `tmp/fuzzy_search-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzy_search-1.6.0.tar", last modified: Fri Apr  7 07:57:59 2023, max compression
+gzip compressed data, was "fuzzy_search-2.0.0a0.tar", last modified: Thu May 11 15:37:27 2023, max compression
```

## Comparing `fuzzy_search-1.6.0.tar` & `fuzzy_search-2.0.0a0.tar`

### file list

```diff
@@ -1,35 +1,56 @@
-drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-04-07 07:57:59.850145 fuzzy_search-1.6.0/
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     1085 2020-12-08 10:17:28.000000 fuzzy_search-1.6.0/LICENSE
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     7663 2023-04-07 07:57:59.850022 fuzzy_search-1.6.0/PKG-INFO
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     6745 2022-05-04 14:52:31.000000 fuzzy_search-1.6.0/README.md
-drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-04-07 07:57:59.848344 fuzzy_search-1.6.0/fuzzy_search/
--rw-r--r--   0 marijnkoolen   (501) staff       (20)      397 2023-04-07 07:57:17.000000 fuzzy_search-1.6.0/fuzzy_search/__init__.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)      209 2020-12-28 12:32:03.000000 fuzzy_search-1.6.0/fuzzy_search/fuzzy_config.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     6839 2022-05-09 13:28:05.000000 fuzzy_search-1.6.0/fuzzy_search/fuzzy_context_searcher.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)    40080 2022-05-09 13:33:49.000000 fuzzy_search-1.6.0/fuzzy_search/fuzzy_match.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     7716 2020-12-07 10:17:03.000000 fuzzy_search-1.6.0/fuzzy_search/fuzzy_patterns.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     9262 2021-08-31 13:07:11.000000 fuzzy_search-1.6.0/fuzzy_search/fuzzy_phrase.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)    31370 2021-07-01 08:55:57.000000 fuzzy_search-1.6.0/fuzzy_search/fuzzy_phrase_model.py
--rw-rw-rw-   0 marijnkoolen   (501) staff       (20)    50726 2023-04-06 14:05:11.000000 fuzzy_search-1.6.0/fuzzy_search/fuzzy_phrase_searcher.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     8716 2019-10-29 21:19:08.000000 fuzzy_search-1.6.0/fuzzy_search/fuzzy_searcher.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     8088 2023-02-02 18:33:08.000000 fuzzy_search-1.6.0/fuzzy_search/fuzzy_string.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)    18030 2021-09-10 09:16:12.000000 fuzzy_search-1.6.0/fuzzy_search/fuzzy_template.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)    32877 2021-08-31 13:48:09.000000 fuzzy_search-1.6.0/fuzzy_search/fuzzy_template_searcher.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     9595 2023-02-02 18:56:54.000000 fuzzy_search-1.6.0/fuzzy_search/similarity.py
-drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-04-07 07:57:59.848803 fuzzy_search-1.6.0/fuzzy_search.egg-info/
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     7663 2023-04-07 07:57:59.000000 fuzzy_search-1.6.0/fuzzy_search.egg-info/PKG-INFO
--rw-r--r--   0 marijnkoolen   (501) staff       (20)      844 2023-04-07 07:57:59.000000 fuzzy_search-1.6.0/fuzzy_search.egg-info/SOURCES.txt
--rw-r--r--   0 marijnkoolen   (501) staff       (20)        1 2023-04-07 07:57:59.000000 fuzzy_search-1.6.0/fuzzy_search.egg-info/dependency_links.txt
--rw-r--r--   0 marijnkoolen   (501) staff       (20)       18 2023-04-07 07:57:59.000000 fuzzy_search-1.6.0/fuzzy_search.egg-info/top_level.txt
--rw-r--r--   0 marijnkoolen   (501) staff       (20)       38 2023-04-07 07:57:59.850185 fuzzy_search-1.6.0/setup.cfg
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     3983 2023-02-02 18:40:00.000000 fuzzy_search-1.6.0/setup.py
-drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-04-07 07:57:59.849837 fuzzy_search-1.6.0/test/
--rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2020-10-14 12:59:55.000000 fuzzy_search-1.6.0/test/__init__.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     1946 2020-12-11 10:14:23.000000 fuzzy_search-1.6.0/test/test_fuzzy_context_searcher.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     9330 2020-12-31 09:40:05.000000 fuzzy_search-1.6.0/test/test_fuzzy_match.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     2847 2020-12-22 08:42:06.000000 fuzzy_search-1.6.0/test/test_fuzzy_phrase.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     3726 2021-06-23 14:43:21.000000 fuzzy_search-1.6.0/test/test_fuzzy_phrase_model.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)    17941 2023-04-07 07:55:40.000000 fuzzy_search-1.6.0/test/test_fuzzy_phrase_searcher.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     3315 2020-10-19 18:08:15.000000 fuzzy_search-1.6.0/test/test_fuzzy_string.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     6190 2020-12-14 11:34:04.000000 fuzzy_search-1.6.0/test/test_fuzzy_template.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     5756 2020-12-22 08:19:21.000000 fuzzy_search-1.6.0/test/test_fuzzy_template_searcher.py
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.237927 fuzzy_search-2.0.0a0/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     1085 2020-12-08 10:17:28.000000 fuzzy_search-2.0.0a0/LICENSE
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     7666 2023-05-11 15:37:27.237813 fuzzy_search-2.0.0a0/PKG-INFO
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     6746 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/README.md
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.233013 fuzzy_search-2.0.0a0/fuzzy_search/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)      513 2023-05-11 15:37:16.000000 fuzzy_search-2.0.0a0/fuzzy_search/__init__.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     8716 2019-10-29 21:19:08.000000 fuzzy_search-2.0.0a0/fuzzy_search/fuzzy_searcher.py
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.233911 fuzzy_search-2.0.0a0/fuzzy_search/match/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2023-04-18 08:43:19.000000 fuzzy_search-2.0.0a0/fuzzy_search/match/__init__.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    12788 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/fuzzy_search/match/candidate_match.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    10376 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/fuzzy_search/match/exact_match.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    31262 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/fuzzy_search/match/phrase_match.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    12964 2023-04-20 11:54:21.000000 fuzzy_search-2.0.0a0/fuzzy_search/match/skip_match.py
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.234196 fuzzy_search-2.0.0a0/fuzzy_search/pattern/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2023-04-18 08:17:29.000000 fuzzy_search-2.0.0a0/fuzzy_search/pattern/__init__.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     7716 2020-12-07 10:17:03.000000 fuzzy_search-2.0.0a0/fuzzy_search/pattern/fuzzy_patterns.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    18032 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/fuzzy_search/pattern/fuzzy_template.py
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.234482 fuzzy_search-2.0.0a0/fuzzy_search/phrase/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2023-04-18 08:12:13.000000 fuzzy_search-2.0.0a0/fuzzy_search/phrase/__init__.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     9868 2023-04-24 06:58:56.000000 fuzzy_search-2.0.0a0/fuzzy_search/phrase/phrase.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    33515 2023-04-21 11:38:57.000000 fuzzy_search-2.0.0a0/fuzzy_search/phrase/phrase_model.py
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.235429 fuzzy_search-2.0.0a0/fuzzy_search/search/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2023-04-18 08:16:54.000000 fuzzy_search-2.0.0a0/fuzzy_search/search/__init__.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     1179 2023-04-20 07:57:23.000000 fuzzy_search-2.0.0a0/fuzzy_search/search/config.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     6847 2023-04-19 10:36:26.000000 fuzzy_search-2.0.0a0/fuzzy_search/search/context_searcher.py
+-rw-rw-rw-   0 marijnkoolen   (501) staff       (20)    14654 2023-04-20 08:18:19.000000 fuzzy_search-2.0.0a0/fuzzy_search/search/phrase_searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    17372 2023-04-20 08:51:05.000000 fuzzy_search-2.0.0a0/fuzzy_search/search/searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    32894 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/fuzzy_search/search/template_searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    25410 2023-04-24 10:58:42.000000 fuzzy_search-2.0.0a0/fuzzy_search/search/token_searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     9609 2023-04-18 13:00:52.000000 fuzzy_search-2.0.0a0/fuzzy_search/similarity.py
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.235792 fuzzy_search-2.0.0a0/fuzzy_search/tokenization/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2023-04-18 08:18:47.000000 fuzzy_search-2.0.0a0/fuzzy_search/tokenization/__init__.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     8088 2023-02-02 18:33:08.000000 fuzzy_search-2.0.0a0/fuzzy_search/tokenization/string.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     5488 2023-04-18 12:51:10.000000 fuzzy_search-2.0.0a0/fuzzy_search/tokenization/token.py
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.233411 fuzzy_search-2.0.0a0/fuzzy_search.egg-info/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     7666 2023-05-11 15:37:26.000000 fuzzy_search-2.0.0a0/fuzzy_search.egg-info/PKG-INFO
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     1420 2023-05-11 15:37:27.000000 fuzzy_search-2.0.0a0/fuzzy_search.egg-info/SOURCES.txt
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)        1 2023-05-11 15:37:27.000000 fuzzy_search-2.0.0a0/fuzzy_search.egg-info/dependency_links.txt
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)       18 2023-05-11 15:37:27.000000 fuzzy_search-2.0.0a0/fuzzy_search.egg-info/top_level.txt
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)       38 2023-05-11 15:37:27.237962 fuzzy_search-2.0.0a0/setup.cfg
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     3983 2023-02-02 18:40:00.000000 fuzzy_search-2.0.0a0/setup.py
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.237653 fuzzy_search-2.0.0a0/test/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2020-10-14 12:59:55.000000 fuzzy_search-2.0.0a0/test/__init__.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)      945 2023-04-20 07:55:27.000000 fuzzy_search-2.0.0a0/test/test_match_candidate.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     9352 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/test/test_match_phrase.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)      496 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/test/test_match_skip.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     6200 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/test/test_pattern_template.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     4153 2023-04-21 16:20:10.000000 fuzzy_search-2.0.0a0/test/test_phrase_phrase.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     4322 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/test/test_phrase_phrase_model.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     1934 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/test/test_search_context_searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    16858 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/test/test_search_phrase_searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     1680 2023-04-20 08:20:37.000000 fuzzy_search-2.0.0a0/test/test_search_searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     5728 2023-04-20 07:55:27.000000 fuzzy_search-2.0.0a0/test/test_search_template_searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     9306 2023-04-24 07:16:40.000000 fuzzy_search-2.0.0a0/test/test_search_token_searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     3255 2023-04-18 13:00:52.000000 fuzzy_search-2.0.0a0/test/test_tokenization_string.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     3313 2023-04-18 12:39:41.000000 fuzzy_search-2.0.0a0/test/test_tokenization_token.py
```

### Comparing `fuzzy_search-1.6.0/LICENSE` & `fuzzy_search-2.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `fuzzy_search-1.6.0/PKG-INFO` & `fuzzy_search-2.0.0a0/fuzzy_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fuzzy_search
-Version: 1.6.0
+Name: fuzzy-search
+Version: 2.0.0a0
 Summary: Tool for fuzzy searching in texts with historical language use and OCR/HTR errors
 Home-page: https://github.com/marijnkoolen/fuzzy-search
 Author: Marijn Koolen
 Author-email: marijn.koolen@gmail.com
 License: MIT
 Keywords: information extraction,historical research,digital resources
 Platform: UNKNOWN
@@ -31,16 +31,16 @@
 ```commandline
 pip install -u fuzzy-search
 ```
 
 ## Usage
 
 ```python
-from fuzzy_search.fuzzy_phrase_searcher import FuzzyPhraseSearcher
-from fuzzy_search.fuzzy_phrase_model import PhraseModel
+from fuzzy_search.search.phrase_searcher import FuzzyPhraseSearcher
+from fuzzy_search.phrase.phrase_model import PhraseModel
 
 # highger matching thresholds for higher quality OCR/HTR (higher precision, recall should be good anyway)
 # lower matching thresholds for lower quality OCR/HTR (higher recall, as that's the main problem)
 config = {
     "char_match_threshold": 0.8,
     "ngram_threshold": 0.6,
     "levenshtein_threshold": 0.8,
@@ -54,15 +54,15 @@
 
 # create a list of domain keywords and phrases
 domain_phrases = [
     # terms for the chair and attendants of a meeting
     "PRAESIDE",
     "PRAESENTIBUS",
     # some weekdays in Latin
-    "Veneris", 
+    "Veneris",
     "Mercuri",
     # some date phrase where any date in January 1725 should match
     "den .. Januarii 1725"
 ]
 
 # create a PhraseModel object from the domain phrases
 phrase_model = PhraseModel(phrases=domain_phrases)
```

### Comparing `fuzzy_search-1.6.0/README.md` & `fuzzy_search-2.0.0a0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 ```commandline
 pip install -u fuzzy-search
 ```
 
 ## Usage
 
 ```python
-from fuzzy_search.fuzzy_phrase_searcher import FuzzyPhraseSearcher
-from fuzzy_search.fuzzy_phrase_model import PhraseModel
+from fuzzy_search.search.phrase_searcher import FuzzyPhraseSearcher
+from fuzzy_search.phrase.phrase_model import PhraseModel
 
 # highger matching thresholds for higher quality OCR/HTR (higher precision, recall should be good anyway)
 # lower matching thresholds for lower quality OCR/HTR (higher recall, as that's the main problem)
 config = {
     "char_match_threshold": 0.8,
     "ngram_threshold": 0.6,
     "levenshtein_threshold": 0.8,
@@ -31,15 +31,15 @@
 
 # create a list of domain keywords and phrases
 domain_phrases = [
     # terms for the chair and attendants of a meeting
     "PRAESIDE",
     "PRAESENTIBUS",
     # some weekdays in Latin
-    "Veneris", 
+    "Veneris",
     "Mercuri",
     # some date phrase where any date in January 1725 should match
     "den .. Januarii 1725"
 ]
 
 # create a PhraseModel object from the domain phrases
 phrase_model = PhraseModel(phrases=domain_phrases)
```

### Comparing `fuzzy_search-1.6.0/fuzzy_search/fuzzy_context_searcher.py` & `fuzzy_search-2.0.0a0/fuzzy_search/search/context_searcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Union
 
-from fuzzy_search.fuzzy_match import PhraseMatch, PhraseMatchInContext
-from fuzzy_search.fuzzy_phrase_searcher import FuzzyPhraseSearcher
+from fuzzy_search.match.phrase_match import PhraseMatch, PhraseMatchInContext
+from fuzzy_search.search.phrase_searcher import FuzzyPhraseSearcher
 
 
 class FuzzyContextSearcher(FuzzyPhraseSearcher):
     """
 
     Attributes
     ----------
```

### Comparing `fuzzy_search-1.6.0/fuzzy_search/fuzzy_match.py` & `fuzzy_search-2.0.0a0/fuzzy_search/match/phrase_match.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,51 @@
 from __future__ import annotations
-from typing import Dict, List, Union
-from datetime import datetime
-from collections import Counter
 import uuid
 import string
+from collections import defaultdict
+from datetime import datetime
+from typing import Dict, List, Union
+
+import fuzzy_search.tokenization.string as fuzzy_string
+from fuzzy_search.match.candidate_match import Candidate
+from fuzzy_search.phrase.phrase import Phrase
+from fuzzy_search.phrase.phrase_model import PhraseModel
 
-import fuzzy_search.fuzzy_string as fuzzy_string
-from fuzzy_search.fuzzy_string import SkipGram
-from fuzzy_search.fuzzy_phrase import Phrase
+
+def filter_matches_by_overlap(filtered_matches: List[PhraseMatch]) -> List[PhraseMatch]:
+    sorted_matches = sorted(filtered_matches, key=lambda x: (x.offset, len(x.string)))
+    filtered_matches = []
+    overlapping = defaultdict(list)
+    for match in sorted_matches:
+        overlapping[(match.offset, len(match.string))].append(match)
+    for offset_length in overlapping:
+        if len(overlapping[offset_length]) == 1:
+            filtered_matches.extend(overlapping[offset_length])
+        else:
+            best = max(overlapping[offset_length], key=lambda item: item.levenshtein_similarity)
+            filtered_matches.append(best)
+    return filtered_matches
+
+
+def candidates_to_matches(candidates: List[Candidate], text: dict, phrase_model: PhraseModel,
+                          ignorecase: bool = False) -> List[PhraseMatch]:
+    matches: List[PhraseMatch] = []
+    for candidate in candidates:
+        if candidate.phrase.phrase_string in phrase_model.is_variant_of:
+            match_phrase_string = phrase_model.is_variant_of[candidate.phrase.phrase_string]
+            match_phrase = phrase_model.phrase_index[match_phrase_string]
+        else:
+            match_phrase = candidate.phrase
+        # print('candidates_to_matches - ignorecase:', ignorecase)
+        match = PhraseMatch(match_phrase, candidate.phrase,
+                            candidate.match_string, candidate.match_start_offset, text_id=text["id"],
+                            ignorecase=ignorecase)
+        match.add_scores(skipgram_overlap=candidate.get_skip_count_overlap())
+        matches.append(match)
+    return matches
 
 
 def validate_match_props(match_phrase: Phrase, match_variant: Phrase,
                          match_string: str, match_offset: int) -> None:
     """Validate match properties.
 
     :param match_phrase: the phrase that has been matched
@@ -86,100 +120,125 @@
             return None
     else:
         # match starts with a non-word-prefix, so move offset to after the prefix
         return match_offset + len(non_word_prefix)
 
 
 def adjust_match_end_offset(phrase_string: str, candidate_string: str,
-                            text: Dict[str, any], end_offset: int, punctuation: str) -> Union[int, None]:
+                            text: Dict[str, any], end_offset: int, punctuation: str,
+                            debug: int = 0) -> Union[int, None]:
     """Adjust the end offset if it is not at a word boundary.
 
     :param phrase_string: the phrase string
     :type phrase_string: str
     :param candidate_string: the candidate match string
     :type candidate_string: str
     :param text: the text object that contains the candidate match string
     :type text: Dict[str, any]
     :param end_offset: the text offset of the candidate match string
     :type end_offset: int
     :param punctuation: the set of characters to treat as punctuation
     :type punctuation: str
+    :param debug: level to show debug information
+    :type debug: int
     :return: the adjusted offset or None if the required adjustment is too big
     :rtype: Union[int, None]
     """
     # ugly hack: if phrase string ends with punctuation, use only whitespace as word end boundary
+    if debug > 0:
+        print('\tadjust_match_end_offset - start')
     whitespace_only = True if phrase_string[-1] in punctuation else False
+    if debug > 0:
+        print('\tadjust_match_end_offset - whitespace_only:', whitespace_only)
     phrase_end = map_string(phrase_string[-3:], punctuation)
+    if debug > 0:
+        print('\tadjust_match_end_offset - prhase_end:', phrase_end)
     match_end = map_string(candidate_string[-3:], punctuation, whitespace_only=whitespace_only)
-    text_suffix = map_string(text["text"][end_offset:end_offset+3], punctuation, whitespace_only=whitespace_only)
-    # print(f"match_end: {candidate_string[-3:]: <4}\ttext_suffix: {text['text'][end_offset:end_offset+3]: >4}")
-    # print(f"mapped suffixes - match_end: #{match_end}#\ttext_suffix: #{text_suffix}#")
+    if debug > 0:
+        print('\tadjust_match_end_offset - match_end:', match_end)
+    text_suffix = map_string(text["text"][end_offset:end_offset+3], punctuation,
+                             whitespace_only=whitespace_only, debug=debug)
+    if debug > 0:
+        print('\tadjust_match_end_offset - text_suffix:', text_suffix)
+        print(f"\tadjust_match_end_offset - match_end: {candidate_string[-3:]: <4}\ttext_suffix: {text['text'][end_offset:end_offset+3]: >4}")
+        print(f"\tadjust_match_end_offset - mapped suffixes - match_end: #{match_end}#\ttext_suffix: #{text_suffix}#")
     return calculate_end_shift(phrase_end, match_end, text_suffix, end_offset)
 
 
 def adjust_match_offsets(phrase_string: str, candidate_string: str,
                          text: Dict[str, any], candidate_start_offset: int,
                          candidate_end_offset: int,
-                         punctuation: str = string.punctuation) -> Union[Dict[str, Union[str, int]], None]:
+                         punctuation: str = string.punctuation,
+                         debug: int = 0) -> Union[Dict[str, Union[str, int]], None]:
     """Adjust the end offset if it is not at a word boundary.
 
     :param phrase_string: the phrase string
     :type phrase_string: str
     :param candidate_string: the candidate match string
     :type candidate_string: str
     :param text: the text object that contains the candidate match string
     :type text: Dict[str, any]
     :param candidate_start_offset: the text offset of the start of the candidate match string
     :type candidate_start_offset: int
     :param candidate_end_offset: the text offset of the end of the candidate match string
     :type candidate_end_offset: int
     :param punctuation: the set of characters to treat as punctuation (defaults to string.punctuation)
     :type punctuation: str
+    :param debug: level to show debug information
+    :type debug: int
     :return: the adjusted offset or None if the required adjustment is too big
     :rtype: Union[int, None]
     """
-    # print("phrase string:", phrase_string)
-    # print("adjusting candidate string:", candidate_string)
+    if debug > 0:
+        print("\tadjust_match_offset - phrase string:", phrase_string)
+        print("\tadjust_match_offset - adjusting candidate string:", candidate_string)
     if punctuation is None:
         punctuation = string.punctuation
-    # print("candidate_start_offset:", candidate_start_offset)
+    if debug > 0:
+        print("\tadjust_match_offset - candidate_start_offset:", candidate_start_offset)
     match_start_offset = adjust_match_start_offset(text, candidate_string, candidate_start_offset)
-    # print("match_start_offset:", match_start_offset)
+    if debug > 0:
+        print("\tadjust_match_offset - match_start_offset:", match_start_offset)
     if match_start_offset is None:
         return None
     match_end_offset = adjust_match_end_offset(phrase_string, candidate_string,
-                                               text, candidate_end_offset, punctuation)
+                                               text, candidate_end_offset, punctuation, debug=debug)
+    if debug > 0:
+        print("\tadjust_match_offset - match_end_offset:", match_end_offset)
     if match_end_offset is None:
         return None
     elif match_end_offset <= match_start_offset:
         return None
     return {
         "match_string": text["text"][match_start_offset:match_end_offset],
         "match_start_offset": match_start_offset,
         "match_end_offset": match_end_offset
     }
 
 
-def map_string(affix_string: str, punctuation: str, whitespace_only: bool = False) -> str:
+def map_string(affix_string: str, punctuation: str,
+               whitespace_only: bool = False, debug: int = 0) -> str:
     """Turn affix string into type char representation. Types are 'w' for non-whitespace char,
     and 's' for whitespace char.
 
     :param affix_string: a string
     :type: str
     :param punctuation: the set of characters to treat as punctuation
     :type punctuation: str
     :param whitespace_only: whether to treat only whitespace as word boundary or also include (some) punctuation
     :type whitespace_only: bool
+    :param debug: level to show debug information
+    :type debug: int
     :return: the type char representation
     :rtype: str
     """
     if whitespace_only:
-        return "".join(["s" if char == " " else "w" for char in affix_string])
+        return ''.join(['s' if char in ' \t\n\r' else 'w' for char in affix_string])
     else:
-        return "".join(["s" if char == " " or char in punctuation else "w" for char in affix_string])
+        return ''.join(['s' if char in ' \t\n\r' or char in punctuation else 'w' for char in affix_string])
 
 
 def calculate_end_shift(phrase_end: str, match_end: str, text_suffix: str, end_offset: int):
     if phrase_end == match_end:
         if text_suffix == "" or text_suffix.startswith("s"):
             return end_offset
     if phrase_end.endswith("s") and match_end.endswith("s"):
@@ -322,250 +381,14 @@
         else:
             return None
     else:
         details = f"phrase_end {phrase_end}, match_end {match_end}, text_suffix {text_suffix}"
         raise ValueError(f"combination not captured: {details}")
 
 
-###################
-# Candidate class #
-###################
-
-class Candidate:
-
-    def __init__(self, phrase: Phrase, max_length_variance: int = 1, ignorecase: bool = False):
-        """Create a Candidate instance for a given Phrase object.
-
-        :param phrase: a phrase object
-        :type phrase: Phrase
-        :param ignorecase: whether to ignore case when matching skip grams
-        :type ignorecase: bool
-        """
-        self.skipgram_set = set()
-        self.skipgram_list: List[SkipGram] = []
-        self.skipgram_count = Counter()
-        self.phrase = phrase
-        self.ignorecase = ignorecase
-        if ignorecase:
-            self.skipgrams = phrase.skipgrams_lower
-            self.skipgram_index = phrase.skipgram_index_lower
-            self.skipgram_freq = phrase.skipgram_freq_lower
-            self.early_skipgram_index = phrase.early_skipgram_index_lower
-            self.late_skipgram_index = phrase.late_skipgram_index_lower
-        else:
-            self.skipgrams = phrase.skipgrams
-            self.skipgram_index = phrase.skipgram_index
-            self.skipgram_freq = phrase.skipgram_freq
-            self.early_skipgram_index = phrase.early_skipgram_index
-            self.late_skipgram_index = phrase.late_skipgram_index
-        self.max_length_variance = max_length_variance
-        self.max_length = len(self.phrase.phrase_string) + self.max_length_variance
-        self.match_start_offset: int = -1
-        self.match_end_offset: int = -1
-        self.match_string: Union[None, str] = None
-        self.skipgram_overlap: float = 0.0
-
-    def __repr__(self):
-        return f'Candidate(' + \
-               f'phrase: "{self.phrase.phrase_string}", match_string: "{self.match_string}", ' + \
-               f'match_start_offset: {self.match_start_offset}, match_end_offset: {self.match_end_offset})'
-
-    def add_skip_match(self, skipgram: SkipGram) -> None:
-        """Add a skipgram match between a text and a phrase ot the candidate.
-
-        :param skipgram: a matching skipgram
-        :type skipgram: SkipGram
-        """
-        if len(self.skipgram_list) == 0 and skipgram.string not in self.early_skipgram_index:
-            # print("skipping skipgram as first for candidate:", skipgram.string)
-            return None
-        self.skipgram_set.add(skipgram.string)
-        self.skipgram_list.append(skipgram)
-        if self.match_start_offset is None or self.match_start_offset < 0:
-            self.match_start_offset = self.get_match_start_offset()
-        if skipgram.offset + skipgram.length > self.match_end_offset:
-            self.match_end_offset = skipgram.offset + skipgram.length
-        self.skipgram_count.update([skipgram.string])
-        # print("\tadd - skipgram:", skipgram.string, skipgram.offset)
-        # print("\tadd - match length:", self.skip_match_length())
-        # print("\tadd - list:", [skip.string for skip in self.skipgram_list])
-        # check if the candidate string is too long to match the phrase
-        # if too long, remove the first skipgrams until the string is short enough
-        while self.skip_match_length() > self.max_length and len(self.skipgram_list) > 0:
-            self.remove_first_skip()
-            self.match_start_offset = self.get_match_start_offset()
-            # print("\tremove - too long - length:", self.skip_match_length())
-            # print("\tremove - too long - list:", [skip.string for skip in self.skipgram_list])
-            # print("\tremove - too long - start:", self.match_start_offset, "\tend:", self.match_end_offset)
-        while len(self.skipgram_list) > 0 and self.skipgram_list[0].string not in self.early_skipgram_index:
-            self.remove_first_skip()
-            self.match_start_offset = self.get_match_start_offset()
-            # print("\tremove - no start - length:", self.skip_match_length())
-            # print("\tremove - no start - list:", [skip.string for skip in self.skipgram_list])
-            # print("\tremove - no start - start:", self.match_start_offset, "\tend:", self.match_end_offset)
-
-    def shift_start_skip(self) -> bool:
-        """Check if there is a later skip that is a better start."""
-        if self.skip_match_length() <= len(self.phrase.phrase_string):
-            return False
-        start_skip = self.skipgram_list[0]
-        start_phrase_offset = self.skipgram_index[start_skip.string][0].offset
-        best_start_phrase_offset = start_phrase_offset
-        best_start_index = 0
-        best_start_skip = start_skip
-        for si, skip in enumerate(self.skipgram_list):
-            skip_phrase_offset = self.skipgram_index[skip.string][0].offset
-            if skip.offset - start_skip.offset > self.skip_match_length() - len(self.phrase.phrase_string):
-                # stop looking for better start when remaining skips result in too short match length
-                break
-            if skip.offset > best_start_skip.offset and skip_phrase_offset <= best_start_phrase_offset:
-                best_start_index = si
-                best_start_skip = skip
-                best_start_phrase_offset = skip_phrase_offset
-            if skip.string not in self.early_skipgram_index:
-                break
-        for _ in range(0, best_start_index):
-            self.remove_first_skip()
-        self.match_start_offset = self.get_match_start_offset()
-        return best_start_index > 0
-
-    def remove_first_skip(self) -> None:
-        """Remove the first matching skipgram from the list and update the count and set."""
-        first_skip = self.skipgram_list.pop(0)
-        # print('removing first skip')
-        # reduce count of first skipgram by 1
-        self.skipgram_count[first_skip.string] -= 1
-        # if count has dropped to zero, remove skipgram from the set
-        if self.skipgram_count[first_skip.string] == 0:
-            self.skipgram_set.remove(first_skip.string)
-
-    def skip_match_length(self) -> int:
-        """Return the length of the matching string.
-
-        :return: difference between start and end offset
-        :rtype: int
-        """
-        if self.match_start_offset is None:
-            return 0
-        return self.match_end_offset - self.match_start_offset
-
-    def is_match(self, skipgram_threshold: float):
-        """Check if the candidate is a likely match for its corresponding phrase.
-
-        :param skipgram_threshold: the threshold to for how many skipgrams have to match between candidate and phrase
-        :type skipgram_threshold: float
-        :return: a boolean whether this candidate is a likely match for the phrase
-        :rtype: bool
-        """
-        if len(self.skipgram_list) == 0:
-            # there are no matching skipgrams, so no matching string
-            # print('NO MATCH: there are no matching skipgrams, so no matching string')
-            return False
-        if self.skipgram_list[0].string not in self.early_skipgram_index:
-            # the first skipgram of candidate is not in the early skipgrams of phrase
-            # print('NO MATCH: the first skipgram of candidate is not in the early skipgrams of phrase')
-            return False
-        # length of current skip matches should be no longer than phrase plus max length variance
-        # but also no shorter than phrase minus max length variance minus late skips offset from end
-        # of phrase.
-        if self.skip_match_length() > len(self.phrase.phrase_string) + self.max_length_variance:
-            # print('NO MATCH: skip match length is longer than max length variance of phrase')
-            return False
-        elif self.skip_match_length() < self.phrase.late_threshold - self.max_length_variance:
-            # print('phrase length:', len(self.phrase.phrase_string))
-            # print('skip match length:', self.skip_match_length())
-            # print('max length variance:', self.max_length_variance)
-            # print('late threshold:', self.phrase.late_threshold)
-            # print('NO MATCH: skip match length is not with max length variance of phrase')
-            return False
-        # print('skip_set_overlap:', self.get_skip_set_overlap())
-        # print('late threshold:', self.phrase.late_threshold)
-        if self.skipgram_list[-1].string not in self.late_skipgram_index:
-            # print("NO MATCH: last skip not in late index")
-            # the last skipgram of candidate is not in the late skipgrams of phrase
-            return False
-        if self.get_skip_set_overlap() < skipgram_threshold:
-            # print("below skipgram threshold:", self.get_skip_set_overlap(), skipgram_threshold)
-            return False
-        else:
-            # print('MATCH!')
-            return True
-
-    def get_skip_set_overlap(self) -> float:
-        """Calculate and set skipgram overlap between text and phrase skipgram matches.
-
-        :return: the skipgram overlap
-        :rtype: float
-        """
-        self.skipgram_overlap = len(self.skipgram_set) / len(self.phrase.skipgram_set)
-        return self.skipgram_overlap
-
-    def get_skip_count_overlap(self) -> float:
-        """Calculate deviation of candidate skipgrams from phrase skipgrams.
-
-        :return: the skipgram overlap (-inf, 1.0]
-        :rtype: float
-        """
-        diff = 0
-        total = 0
-        for skipgram_string, count in self.skipgram_count.items():
-            diff += abs(count - self.skipgram_freq[skipgram_string])
-            total += count
-        return (total - diff) / self.phrase.num_skipgrams
-
-    def get_match_start_offset(self) -> Union[None, int]:
-        """Calculate the start offset of the match.
-
-        :return: the start offset of the match
-        :rtype: int
-        """
-        if len(self.skipgram_list) == 0:
-            return None
-        first_skip = self.skipgram_list[0]
-        first_skip_in_phrase = self.skipgram_index[first_skip.string][0]
-        match_start_offset = self.skipgram_list[0].offset - first_skip_in_phrase.offset
-        # print("in match:", first_skip.string, first_skip.offset)
-        # print("in phrase:", first_skip_in_phrase.string, first_skip_in_phrase.offset)
-        # print("match_start_offset:", match_start_offset)
-        return 0 if match_start_offset < 0 else match_start_offset
-
-    def get_match_string(self, text: Dict[str, any]) -> Union[str, None]:
-        """Find the matching string of a candidate fuzzy match between a text and a phrase.
-
-        :param text: the text object from which the candidate was derived
-        :type text: Dict[str, any]
-        :return: the matching string
-        :rtype: str
-        """
-        # print('get_match_string - text:', text)
-        if self.match_start_offset == self.match_end_offset:
-            raise ValueError('start and end offset cannot be the same')
-        if self.match_start_offset > self.match_end_offset:
-            raise ValueError('start offset cannot be bigger than end offset')
-        return text["text"][self.match_start_offset:self.match_end_offset]
-    # TODO: check if first to last offset is too long
-    # if not, the match string is probably fine
-    # if it is, find the best substring
-
-    def same_candidate(self, other: Candidate):
-        """Check if this candidate has the same start and end offsets as another candidate.
-
-        :param other: another candidate for the same phrase and text.
-        :type other: Candidate
-        :return: this candidate match has the same offsets as the other candidate
-        :rtype: bool
-        """
-        if self.match_start_offset != other.match_start_offset:
-            return False
-        if self.match_end_offset != other.match_end_offset:
-            return False
-        else:
-            return True
-
-
 ###############
 # Match class #
 ###############
 
 class PhraseMatch:
     """
```

### Comparing `fuzzy_search-1.6.0/fuzzy_search/fuzzy_patterns.py` & `fuzzy_search-2.0.0a0/fuzzy_search/pattern/fuzzy_patterns.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-1.6.0/fuzzy_search/fuzzy_phrase.py` & `fuzzy_search-2.0.0a0/fuzzy_search/phrase/phrase.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from typing import Dict, List, Set, Union
-from collections import defaultdict, Counter
 import re
+from collections import defaultdict, Counter
+from typing import Dict, List, Set, Union
 
-from fuzzy_search.fuzzy_string import SkipGram, text2skipgrams
+from fuzzy_search.tokenization.string import SkipGram, text2skipgrams
+from fuzzy_search.tokenization.token import Token
+from fuzzy_search.tokenization.token import Tokenizer
 
 
 def is_valid_label(label: Union[str, List[str]]) -> bool:
     """Test whether label has a valid value.
 
     :param label: a phrase label (either a string or a list of strings)
     :type label: Union[str, List[str]]
@@ -21,15 +23,15 @@
     return isinstance(label, str)
 
 
 class Phrase(object):
 
     def __init__(self, phrase: Union[str, Dict[str, str]], ngram_size: int = 2, skip_size: int = 2,
                  early_threshold: int = 3, late_threshold: int = 3, within_range_threshold: int = 3,
-                 ignorecase: bool = False):
+                 ignorecase: bool = False, tokens: List[Token] = None, tokenizer: Tokenizer = None):
         if isinstance(phrase, str):
             phrase = {"phrase": phrase}
         self.name = phrase["phrase"]
         self.phrase_string = self.name if not ignorecase else self.name.lower()
         self.exact_string = re.escape(self.phrase_string)
         self.extact_word_boundary_string = re.compile(rf"\b{self.exact_string}\b")
         self.label = None
@@ -64,27 +66,36 @@
         # print(self.late_skipgram_index_lower.keys())
         self.skipgram_freq_lower = Counter([skipgram.string for skipgram in self.skipgrams_lower])
         self.num_skipgrams = len(self.skipgrams)
         self.skipgram_distance = {}
         self.metadata: dict = phrase
         self.words: List[str] = [word for word in re.split(r"\W+", self.phrase_string) if word != ""]
         self.word_set: Set[str] = set(self.words)
+        self.tokens: List[Token] = tokens
+        self.token_index = defaultdict(list)
         self.first_word = None if len(self.words) == 0 else self.words[0]
         self.last_word = None if len(self.words) == 0 else self.words[-1]
         self.num_words = len(self.words)
         if "label" in phrase:
             self.set_label(phrase["label"])
         if len(phrase.keys()) > 1:
             self.add_metadata(phrase)
         self._index_skipgrams()
         self._set_within_range()
+        if tokens is None and tokenizer is not None:
+            self.tokens = tokenizer.tokenize(self.phrase_string)
+            self.words = [token.string for token in self.tokens]
+            for ti, token in enumerate(self.tokens):
+                self.token_index[token.n].append(ti)
 
     def __repr__(self):
         return f"Phrase({self.phrase_string}, {self.label})"
 
+    def __len__(self):
+        return len(self.phrase_string)
     # internal methods
 
     def _index_skipgrams(self) -> None:
         """Turn the phrase into a list of skipgrams and index them with their offset(s) as values."""
         for skipgram in self.skipgrams:
             self.skipgram_index[skipgram.string] += [skipgram]
         for skipgram in self.skipgrams_lower:
```

### Comparing `fuzzy_search-1.6.0/fuzzy_search/fuzzy_phrase_model.py` & `fuzzy_search-2.0.0a0/fuzzy_search/phrase/phrase_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-from typing import Dict, Generator, List, Set, Union
-from collections import defaultdict
-import json
 import copy
+import json
 import re
+from collections import defaultdict
+from typing import Dict, Generator, List, Set, Union
 
-from fuzzy_search.fuzzy_phrase import Phrase
+from fuzzy_search.phrase.phrase import Phrase
+from fuzzy_search.tokenization.token import Token
+from fuzzy_search.tokenization.token import Tokenizer
 
 
-def as_phrase_object(phrase: Union[str, dict, Phrase], ngram_size: int = 2, skip_size: int = 2) -> Phrase:
+def as_phrase_object(phrase: Union[str, dict, Phrase],
+                     ngram_size: int = 2,
+                     skip_size: int = 2,
+                     tokenizer: Tokenizer = None) -> Phrase:
     if isinstance(phrase, Phrase):
         return phrase
     if isinstance(phrase, dict):
         if not is_phrase_dict(phrase):
             print(phrase)
             raise KeyError("invalid phrase dictionary")
-        return Phrase(phrase, ngram_size=ngram_size, skip_size=skip_size)
+        return Phrase(phrase, ngram_size=ngram_size, skip_size=skip_size, tokenizer=tokenizer)
     if isinstance(phrase, str):
-        return Phrase(phrase, ngram_size=ngram_size, skip_size=skip_size)
+        return Phrase(phrase, ngram_size=ngram_size, skip_size=skip_size, tokenizer=tokenizer)
     else:
         raise TypeError('phrase must be of type string')
 
 
 def is_phrase_dict(phrase_dict: Dict[str, Union[str, List[str]]]) -> bool:
     if not isinstance(phrase_dict, dict):
         return False
@@ -51,15 +56,16 @@
 
     def __init__(self, phrases: Union[None, List[Union[str, Dict[str, Union[str, list]], Phrase]]] = None,
                  variants: Union[None, List[Union[Dict[str, List[str]], Phrase]]] = None,
                  phrase_labels: Union[None, List[Dict[str, str]]] = None,
                  distractors: Union[None, List[Union[Dict[str, List[str]], Phrase]]] = None,
                  model: Union[None, List[Dict[str, Union[str, list]]]] = None,
                  custom: Union[None, List[Dict[str, Union[str, int, float, list]]]] = None,
-                 config: dict = None):
+                 config: dict = None,
+                 tokenizer: Tokenizer = None):
         if config is None:
             config = {}
         self.ngram_size = config["ngram_size"] if "ngram_size" in config else 2
         self.skip_size = config["skip_size"] if "skip_size" in config else 2
         self.phrase_index: Dict[str, Phrase] = {}
         # only register variants of known phrases
         self.variant_index: Dict[str, Phrase] = {}
@@ -70,17 +76,20 @@
         self.is_distractor_of: Dict[str, Set[str]] = defaultdict(set)
         self.phrase_length_index: Dict[int, set] = defaultdict(set)
         self.variant_length_index: Dict[int, set] = defaultdict(set)
         self.has_labels: Dict[str, Set[str]] = defaultdict(set)
         self.is_label_of: Dict[str, Set[str]] = defaultdict(set)
         self.custom = {}
         self.word_in_phrase: Dict[str, Set[str]] = defaultdict(set)
+        self.token_in_phrase: Dict[str, Set[str]] = defaultdict(set)
         self.first_word_in_phrase: Dict[str, Dict[str, int]] = defaultdict(dict)
+        self.first_token_in_phrase: Dict[str, Dict[str, int]] = defaultdict(dict)
         self.phrase_type: Dict[str, Set[str]] = defaultdict(set)
         self.phrase_string_map: Dict[str, Phrase] = {}
+        self.tokenizer = tokenizer
         if phrases:
             self.add_phrases(phrases)
         if variants:
             self.add_variants(variants)
         if distractors:
             self.add_distractors(distractors)
         if phrase_labels:
@@ -136,15 +145,16 @@
         :param phrase: a phrase to be added
         :type phrase: Phrase
         """
         self.phrase_string_map[phrase.phrase_string] = phrase
         self.phrase_type[phrase.phrase_string].add("phrase")
         self.phrase_index[phrase.phrase_string] = phrase
         self.phrase_length_index[len(phrase.phrase_string)].add(phrase.phrase_string)
-        self.index_phrase_words(phrase)
+        self._index_phrase_words(phrase)
+        self._index_phrase_tokens(phrase)
 
     def add_variant(self, variant_phrase: Phrase, main_phrase: Phrase):
         """Add a phrase to the model as variant of a given main phrase.
 
         :param variant_phrase: a variant phrase to be added as variant of main_phrase
         :type variant_phrase: Phrase
         :param main_phrase: a main phrase that the variant phrase is a variant of
@@ -153,15 +163,16 @@
         if variant_phrase.phrase_string not in self.phrase_string_map:
             self.phrase_string_map[variant_phrase.phrase_string] = variant_phrase
         self.variant_index[variant_phrase.phrase_string] = variant_phrase
         self.is_variant_of[variant_phrase.phrase_string] = main_phrase.phrase_string
         self.has_variants[main_phrase.phrase_string].add(variant_phrase.phrase_string)
         self.phrase_type[variant_phrase.phrase_string].add("variant")
         self.variant_length_index[len(variant_phrase.phrase_string)].add(variant_phrase.phrase_string)
-        self.index_phrase_words(variant_phrase)
+        self._index_phrase_words(variant_phrase)
+        self._index_phrase_tokens(variant_phrase)
 
     def add_distractor(self, distractor_phrase: Phrase, main_phrase: Phrase):
         """Add a phrase to the model as distractor of a given main phrase.
 
         :param distractor_phrase: a distractor phrase to be added as distractor of main_phrase
         :type distractor_phrase: Phrase
         :param main_phrase: a main phrase that the distractor phrase is a distractor of
@@ -169,15 +180,16 @@
         """
         if distractor_phrase.phrase_string not in self.phrase_string_map:
             self.phrase_string_map[distractor_phrase.phrase_string] = distractor_phrase
         self.distractor_index[distractor_phrase.phrase_string] = distractor_phrase
         self.is_distractor_of[distractor_phrase.phrase_string].add(main_phrase.phrase_string)
         self.has_distractors[main_phrase.phrase_string].add(distractor_phrase.phrase_string)
         self.phrase_type[distractor_phrase.phrase_string].add("distractor")
-        self.index_phrase_words(distractor_phrase)
+        self._index_phrase_words(distractor_phrase)
+        self._index_phrase_tokens(distractor_phrase)
 
     def remove_phrase(self, phrase: Phrase):
         """Remove a main phrase from the model, including its connections to any variant and distractor phrases.
 
         :param phrase: a phrase that is registered as a main phrase
         :type phrase: Phrase
         """
@@ -189,15 +201,16 @@
         # remove the phrase string from the main phrase index
         del self.phrase_index[phrase.phrase_string]
         # remove the phrase from the phrase length index
         self.phrase_length_index[len(phrase.phrase_string)].remove(phrase.phrase_string)
         if len(self.phrase_type[phrase.phrase_string]) == 0:
             # if the phrase string is not registered as another type (variant or distractor)
             # remove the phrase words from the word_to_phrase index
-            self.remove_phrase_words(phrase)
+            self._remove_phrase_words(phrase)
+            self._remove_phrase_tokens(phrase)
         # if the phrase has variants, remove those as well
         if phrase.phrase_string in self.has_variants:
             for variant_string in self.has_variants:
                 variant_phrase = self.variant_index[variant_string]
                 self.remove_variant(variant_phrase)
         # if the phrase has distractors, remove its connections with them as well
         if phrase.phrase_string in self.has_distractors:
@@ -220,15 +233,16 @@
         # first check if variant phrase is registered as a variant
         if variant_phrase.phrase_string not in self.is_variant_of:
             raise ValueError(f"{variant_phrase.phrase_string} is not registered as a variant")
         # remove variant from the type index
         self.phrase_type[variant_phrase.phrase_string].remove("variant")
         # if that is the only type of the phrase, remove it from the word_to_phrase index
         if len(self.phrase_type[variant_phrase.phrase_string]) == 0:
-            self.remove_phrase_words(variant_phrase)
+            self._remove_phrase_words(variant_phrase)
+            self._remove_phrase_tokens(variant_phrase)
         # remove the variant from the variant index
         del self.variant_index[variant_phrase.phrase_string]
         # remove the variant from the phrase length index
         self.variant_length_index[len(variant_phrase.phrase_string)].remove(variant_phrase.phrase_string)
         # remove its connection with its main phrase
         main_phrase_string = self.is_variant_of[variant_phrase.phrase_string]
         del self.is_variant_of[variant_phrase.phrase_string]
@@ -244,15 +258,16 @@
         :param distractor_phrase: a phrase that is registered as a distractor of one or more main phrases
         :type distractor_phrase: Phrase
         """
         if distractor_phrase.phrase_string not in self.is_distractor_of:
             raise ValueError(f"{distractor_phrase.phrase_string} is not registered as a distractor")
         self.phrase_type[distractor_phrase.phrase_string].remove("distractor")
         if len(self.phrase_type[distractor_phrase.phrase_string]) == 0:
-            self.remove_phrase_words(distractor_phrase)
+            self._remove_phrase_words(distractor_phrase)
+            self._remove_phrase_tokens(distractor_phrase)
         del self.distractor_index[distractor_phrase.phrase_string]
         for main_phrase_string in self.is_distractor_of[distractor_phrase.phrase_string]:
             self.has_distractors[main_phrase_string].remove(distractor_phrase.phrase_string)
             if len(self.has_distractors[main_phrase_string]) == 0:
                 del self.has_distractors[main_phrase_string]
         del self.is_distractor_of[distractor_phrase.phrase_string]
 
@@ -262,33 +277,38 @@
         - a list of dictionaries with property 'phrase' and the phrase as a string value
         - a list of Phrase objects
 
         :param phrases: a list of phrases
         :type phrases: List[Union[str, Dict[str, Union[str, List[str]]]]]
         """
         for phrase in phrases:
-            phrase = as_phrase_object(phrase, ngram_size=self.ngram_size, skip_size=self.skip_size)
+            phrase = as_phrase_object(phrase, ngram_size=self.ngram_size,
+                                      skip_size=self.skip_size, tokenizer=self.tokenizer)
             self.add_phrase(phrase)
         # if phrases is a dictionary with possible variants, distractors, labels and custom metadata
         # per phrase, add those variants and distractors
         phrase_dicts = [phrase for phrase in phrases if isinstance(phrase, dict)]
-        self.add_variants(phrase_dicts)
-        self.add_distractors(phrase_dicts)
-        self.add_custom(phrase_dicts)
-        self.add_labels(phrase_dicts)
+        phrases = [Phrase(phrase_dict, tokenizer=self.tokenizer) for phrase_dict in phrase_dicts]
+        self.add_variants(phrases)
+        self.add_distractors(phrases)
+        self.add_custom(phrases)
+        self.add_labels(phrases)
 
     def remove_phrases(self, phrases: List[Union[str, Dict[str, Union[str, List[str]]], Phrase]]):
         """Remove a list of phrases from the phrase model. If it has any registered spelling variants,
         remove those as well.
 
         :param phrases: a list of phrases/keyphrases
         :type phrases: List[Union[str, Dict[str, Union[str, List[str]]]]]
         """
+        print('REMOVING PHRASES')
         for phrase in phrases:
+            print('\tphrase:', phrase)
             phrase = as_phrase_object(phrase, ngram_size=self.ngram_size, skip_size=self.skip_size)
+            print('\tas phrase:', phrase)
             if phrase.phrase_string not in self.phrase_index:
                 raise KeyError(f"Unknown phrase: {phrase.phrase_string}")
             self.remove_phrase(phrase)
 
     def get_phrases_by_max_length(self, max_length: int,
                                   include_variants: bool = False) -> Generator[Phrase, None, None]:
         """Return all phrase in the phrase model that are no longer than a given length.
@@ -323,27 +343,27 @@
         :type phrase: Union[str, Dict[str, any], Phrase]
         :return: a boolean indicating whether phrase is registered
         :rtype: bool
         """
         phrase = as_phrase_object(phrase, ngram_size=self.ngram_size, skip_size=self.skip_size)
         return phrase.phrase_string in self.phrase_index
 
-    def add_variants(self, variants: List[Dict[str, Union[str, List[str]]]],
+    def add_variants(self, variants: List[Union[Phrase, Dict[str, Union[str, List[str]]]]],
                      add_new_phrases: bool = True) -> None:
         """Add variants of a phrase. If the phrase is not registered, add it to the set.
         - input is a list of dictionaries:
         variants = [{'phrase': 'some phrase', 'variants': ['some variant', 'some other variant']}]
 
-        :param variants: a list of phrase dictionaries with 'variant' property
+        :param variants: a list of phrases or phrase dictionaries with 'variant' property
         :type variants: List[Dict[str, Union[str, List[str]]]]
         :param add_new_phrases: a Boolean to indicate if unknown phrases should be added
         :type add_new_phrases: bool
         """
-        for phrase_dict in variants:
-            main_phrase = as_phrase_object(phrase_dict, ngram_size=self.ngram_size, skip_size=self.skip_size)
+        for phrase in variants:
+            main_phrase = as_phrase_object(phrase, ngram_size=self.ngram_size, skip_size=self.skip_size)
             if main_phrase.phrase_string not in self.phrase_index:
                 if add_new_phrases:
                     self.add_phrase(main_phrase)
                 else:
                     continue
             if "variants" not in main_phrase.metadata:
                 continue
@@ -408,27 +428,27 @@
         """
         phrase_string = phrase.phrase_string if isinstance(phrase, Phrase) else phrase
         if phrase_string not in self.has_variants:
             return None
         else:
             return [self.variant_index[variant_string] for variant_string in self.has_variants[phrase_string]]
 
-    def add_distractors(self, distractors: List[Dict[str, Union[str, List[str]]]],
+    def add_distractors(self, distractors: List[Union[Phrase, Dict[str, Union[str, List[str]]]]],
                         add_new_phrases: bool = True) -> None:
         """Add distractors of a phrase. If the phrase is not registered, add it to the set.
         - input is a list of dictionaries:
         distractors = [{'phrase': 'some phrase', 'distractors': ['some distractor', 'some other distractor']}]
 
         :param distractors: a list of phrase dictionaries with 'distractor' property
         :type distractors: List[Dict[str, Union[str, List[str]]]]
         :param add_new_phrases: a Boolean to indicate if unknown phrases should be added
         :type add_new_phrases: bool
         """
-        for phrase_dict in distractors:
-            main_phrase = as_phrase_object(phrase_dict, ngram_size=self.ngram_size, skip_size=self.skip_size)
+        for phrase in distractors:
+            main_phrase = as_phrase_object(phrase, ngram_size=self.ngram_size, skip_size=self.skip_size)
             if main_phrase.phrase_string not in self.phrase_index:
                 if add_new_phrases:
                     self.add_phrase(main_phrase)
                 else:
                     continue
             if "distractors" not in main_phrase.metadata:
                 continue
@@ -459,21 +479,21 @@
                 raise IndexError(f"{main_phrase.phrase_string} is not registered in this phrase model")
             if main_phrase not in self.has_distractors:
                 return None
             for distractor_string in self.has_distractors[main_phrase.phrase_string]:
                 distractor = as_phrase_object(distractor_string, ngram_size=self.ngram_size, skip_size=self.skip_size)
                 self.remove_distractor(distractor)
 
-    def add_labels(self, phrase_labels: List[Dict[str, Union[str, list]]]):
+    def add_labels(self, phrase_labels: List[Union[Phrase, Dict[str, Union[str, List[str]]]]]):
         """Add a label to a phrase. This can be used to group phrases under the same label.
         - input is a list of phrase/label pair dictionaries:
         labels = [{'phrase': 'some phrase', 'label': 'some label'}]
         """
-        for phrase_dict in phrase_labels:
-            phrase = as_phrase_object(phrase_dict, ngram_size=self.ngram_size, skip_size=self.skip_size)
+        for phrase in phrase_labels:
+            phrase = as_phrase_object(phrase, ngram_size=self.ngram_size, skip_size=self.skip_size)
             if phrase.label is None:
                 continue
             if phrase.phrase_string not in self.phrase_index:
                 print(f'skipping label for unknown phrase {phrase}')
             for label in phrase.label_set:
                 self.has_labels[phrase.phrase_string].add(label)
                 self.is_label_of[label].add(phrase.phrase_string)
@@ -523,61 +543,50 @@
         :rtype: List[str]
         """
         phrase_string = phrase if isinstance(phrase, str) else phrase.phrase_string
         if not self.has_phrase(phrase_string):
             raise KeyError(f"Unknown phrase: {phrase}")
         return self.has_labels[phrase]
 
-    def validate_entry_phrase(self, entry: Dict[str, Union[str, int, float, list]]) -> None:
-        """Check if a given phrase (as dictionary) is registered.
-
-        :param entry: a phrase dictionary with a 'phrase' property
-        :type entry: Dict[str, Union[str, int, float, list]]
-        """
-        if 'phrase' not in entry:
-            raise KeyError("Keywords as list of dictionaries should have 'phrase' property")
-        if not isinstance(entry['phrase'], str):
-            raise ValueError("phrase property must be a string")
-        if entry['phrase'] not in self.phrase_index:
-            raise KeyError("Unknown phrase")
-
-    def add_custom(self, custom: List[Dict[str, Union[str, int, float, list]]]) -> None:
+    def add_custom(self, custom: List[Union[Phrase, Dict[str, Union[str, int, float, list]]]]) -> None:
         """Add custom key/value pairs to the entry as phrase metadata.
 
         param entry: an Array of phrase dictionaries, each with a 'phrase' property and additional key/value pairs
         type entry: Dict[str, Union[str, int, float, list]]
         """
         for entry in custom:
-            if not isinstance(entry, dict):
+            phrase = as_phrase_object(entry, ngram_size=self.ngram_size, skip_size=self.skip_size)
+            if phrase.metadata is None:
                 continue
-            self.validate_entry_phrase(entry)
-            # make sure the custom entry is a copy of the original and not a reference to the same object
-            self.custom[entry['phrase']] = copy.deepcopy(entry)
+            if phrase.phrase_string not in self.phrase_index:
+                continue
+            self.custom[phrase.phrase_string] = copy.deepcopy(phrase.metadata)
 
     def remove_custom(self, custom: List[Dict[str, any]]) -> None:
         """Remove custom properties for a list of phrases.
 
         :param custom: a list of phrase dictionaries with custom properties to remove
         :type custom: List[Dict[str, any]]
         """
         for entry in custom:
-            self.validate_entry_phrase(entry)
-            for custom_property in entry:
-                del self.custom[entry['phrase']][custom_property]
+            phrase = as_phrase_object(entry, ngram_size=self.ngram_size, skip_size=self.skip_size)
+            for custom_property in phrase.metadata:
+                del self.custom[phrase.phrase_string][custom_property]
 
     def has_custom(self, phrase_string: str, custom_property: str) -> bool:
         """Check if a phrase has a given custom property.
 
         :param phrase_string: a phrase string of a registered phrase.
         :type phrase_string: str
         :param custom_property: the name of a custom property of the registered phrase
         :type custom_property: str
         :return: a boolean to indicate whether the phrase has a custom property of the given property name
         :rtype: bool
         """
+        print('CUSTOM:', self.custom)
         return phrase_string in self.custom and custom_property in self.custom[phrase_string]
 
     def get(self, phrase_string: str, custom_property: str) -> any:
         """Get the value of a custom property for a given phrase.
 
         :param phrase_string: a phrase string of a registered phrase.
         :type phrase_string: str
@@ -588,35 +597,68 @@
         """
         if phrase_string not in self.phrase_index:
             raise KeyError("Unknown phrase_string")
         if not self.has_custom(phrase_string, custom_property):
             raise ValueError("Unknown custom property")
         return self.custom[phrase_string][custom_property]
 
-    def index_phrase_words(self, phrase: Phrase) -> None:
+    def _index_phrase_words(self, phrase: Phrase) -> None:
         """Index a phrase on its individual words, for exact match look up routines.
 
         :param phrase: a phrase object that is part of the phrase model
         :type phrase: Phrase
         """
         if phrase.phrase_string not in self.phrase_type:
             raise ValueError(f"Cannot index phrase words for non-registered phrase: {phrase.phrase_string}")
         for wi, word in enumerate(re.finditer(r"\w+", phrase.phrase_string)):
             if wi == 0:
                 self.first_word_in_phrase[word.group(0)][phrase.phrase_string] = word.start()
             self.word_in_phrase[word.group(0)].add(phrase.phrase_string)
 
-    def remove_phrase_words(self, phrase: Phrase) -> None:
+    def _remove_phrase_words(self, phrase: Phrase) -> None:
         """Remove the individual words of a phrase from the index. Only use this is you are removing
         the phrase from the phrase model.
 
         :param phrase: a phrase object that is part of the phrase model
         :type phrase: Phrase
         """
         for wi, word in enumerate(re.finditer(r"\w+", phrase.phrase_string)):
             if wi == 0:
                 del self.first_word_in_phrase[word.group(0)][phrase.phrase_string]
                 if len(self.first_word_in_phrase[word.group(0)].keys()) == 0:
                     del self.first_word_in_phrase[word.group(0)]
             self.word_in_phrase[word.group(0)].remove(phrase.phrase_string)
             if len(self.word_in_phrase[word.group(0)]) == 0:
                 del self.word_in_phrase[word.group(0)]
+
+    def _remove_phrase_tokens(self, phrase: Phrase, tokenizer: Tokenizer = None) -> None:
+        """Remove the individual words of a phrase from the index. Only use this is you are removing
+        the phrase from the phrase model.
+
+        :param phrase: a phrase object that is part of the phrase model
+        :type phrase: Phrase
+        """
+        tokenizer = self._get_tokenizer(tokenizer)
+        if tokenizer is None:
+            return None
+        tokens = tokenizer.tokenize(phrase.phrase_string)
+        for ti, token in enumerate(tokens):
+            if ti == 0:
+                del self.first_token_in_phrase[token.n][phrase.phrase_string]
+                if len(self.first_token_in_phrase[token.n].keys()) == 0:
+                    del self.first_token_in_phrase[token.n]
+            self.token_in_phrase[token.n].remove(phrase.phrase_string)
+            if len(self.token_in_phrase[token.n]) == 0:
+                del self.token_in_phrase[token.n]
+
+    def _get_tokenizer(self, tokenizer: Tokenizer = None):
+        return tokenizer if tokenizer is not None else self.tokenizer
+
+    def _index_phrase_tokens(self, phrase: Phrase, tokenizer: Tokenizer = None):
+        tokenizer = self._get_tokenizer(tokenizer)
+        if tokenizer:
+            tokens = tokenizer.tokenize(phrase.phrase_string, doc_id=phrase.phrase_string)
+            for token in tokens:
+                self.token_in_phrase[token.n].add(phrase.phrase_string)
+
+    def has_token(self, token: Union[str, Token]):
+        return token.n in self.token_in_phrase
```

### Comparing `fuzzy_search-1.6.0/fuzzy_search/fuzzy_searcher.py` & `fuzzy_search-2.0.0a0/fuzzy_search/fuzzy_searcher.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-1.6.0/fuzzy_search/fuzzy_string.py` & `fuzzy_search-2.0.0a0/fuzzy_search/tokenization/string.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-1.6.0/fuzzy_search/fuzzy_template.py` & `fuzzy_search-2.0.0a0/fuzzy_search/pattern/fuzzy_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from typing import Dict, List, Set, Union
 
-from fuzzy_search.fuzzy_phrase_model import PhraseModel
-from fuzzy_search.fuzzy_phrase import Phrase
+from fuzzy_search.phrase.phrase_model import PhraseModel
+from fuzzy_search.phrase.phrase import Phrase
 
 
 def validate_element_properties(label: str, required: bool = False, cardinality: str = "multi",
                                 next_label: Union[None, str, List[str]] = None,
                                 next_distance_max: Union[None, int] = None,
                                 variable: bool = False) -> None:
     """Validate the properties of a FuzzyTemplate element.
```

### Comparing `fuzzy_search-1.6.0/fuzzy_search/fuzzy_template_searcher.py` & `fuzzy_search-2.0.0a0/fuzzy_search/search/template_searcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, List, Union
 
 import fuzzy_search
-from fuzzy_search.fuzzy_match import PhraseMatch
-from fuzzy_search.fuzzy_phrase_model import PhraseModel
-from fuzzy_search.fuzzy_template import FuzzyTemplate, FuzzyTemplateElement, FuzzyTemplateGroupElement
-from fuzzy_search.fuzzy_context_searcher import FuzzyContextSearcher
+from fuzzy_search.match.phrase_match import PhraseMatch
+from fuzzy_search.phrase.phrase_model import PhraseModel
+from fuzzy_search.pattern.fuzzy_template import FuzzyTemplate, FuzzyTemplateElement, FuzzyTemplateGroupElement
+from fuzzy_search.search.context_searcher import FuzzyContextSearcher
 
 
 DEBUG = False
 
 
 def share_label(object1: Union[PhraseMatch, FuzzyTemplateElement],
                 object2: Union[PhraseMatch, FuzzyTemplateElement]) -> bool:
```

### Comparing `fuzzy_search-1.6.0/fuzzy_search/similarity.py` & `fuzzy_search-2.0.0a0/fuzzy_search/similarity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Generator, Iterable, List, Tuple, Union
+import math
 from collections import defaultdict
 from collections import Counter
-import math
+from typing import Generator, Iterable, List, Tuple, Union
 
 
-from fuzzy_search.fuzzy_string import score_levenshtein_distance
-from fuzzy_search.fuzzy_string import text2skipgrams
+from fuzzy_search.tokenization.string import score_levenshtein_distance
+from fuzzy_search.tokenization.string import text2skipgrams
 
 
 def vector_length(skipgram_freq):
     return math.sqrt(sum([skipgram_freq[skip] ** 2 for skip in skipgram_freq]))
 
 
 class Vocabulary:
```

### Comparing `fuzzy_search-1.6.0/fuzzy_search.egg-info/PKG-INFO` & `fuzzy_search-2.0.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fuzzy-search
-Version: 1.6.0
+Name: fuzzy_search
+Version: 2.0.0a0
 Summary: Tool for fuzzy searching in texts with historical language use and OCR/HTR errors
 Home-page: https://github.com/marijnkoolen/fuzzy-search
 Author: Marijn Koolen
 Author-email: marijn.koolen@gmail.com
 License: MIT
 Keywords: information extraction,historical research,digital resources
 Platform: UNKNOWN
@@ -31,16 +31,16 @@
 ```commandline
 pip install -u fuzzy-search
 ```
 
 ## Usage
 
 ```python
-from fuzzy_search.fuzzy_phrase_searcher import FuzzyPhraseSearcher
-from fuzzy_search.fuzzy_phrase_model import PhraseModel
+from fuzzy_search.search.phrase_searcher import FuzzyPhraseSearcher
+from fuzzy_search.phrase.phrase_model import PhraseModel
 
 # highger matching thresholds for higher quality OCR/HTR (higher precision, recall should be good anyway)
 # lower matching thresholds for lower quality OCR/HTR (higher recall, as that's the main problem)
 config = {
     "char_match_threshold": 0.8,
     "ngram_threshold": 0.6,
     "levenshtein_threshold": 0.8,
@@ -54,15 +54,15 @@
 
 # create a list of domain keywords and phrases
 domain_phrases = [
     # terms for the chair and attendants of a meeting
     "PRAESIDE",
     "PRAESENTIBUS",
     # some weekdays in Latin
-    "Veneris", 
+    "Veneris",
     "Mercuri",
     # some date phrase where any date in January 1725 should match
     "den .. Januarii 1725"
 ]
 
 # create a PhraseModel object from the domain phrases
 phrase_model = PhraseModel(phrases=domain_phrases)
```

### Comparing `fuzzy_search-1.6.0/setup.py` & `fuzzy_search-2.0.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-1.6.0/test/test_fuzzy_context_searcher.py` & `fuzzy_search-2.0.0a0/test/test_search_context_searcher.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest import TestCase
 
-from fuzzy_search.fuzzy_match import PhraseMatch, PhraseMatchInContext
-from fuzzy_search.fuzzy_context_searcher import FuzzyContextSearcher
-from fuzzy_search.fuzzy_phrase import Phrase
-from fuzzy_search.fuzzy_phrase_model import PhraseModel
+from fuzzy_search.match.phrase_match import PhraseMatch
+from fuzzy_search.search.context_searcher import FuzzyContextSearcher
+from fuzzy_search.phrase.phrase import Phrase
+from fuzzy_search.phrase.phrase_model import PhraseModel
 
 
 class TestFuzzyContextSearcher(TestCase):
 
     def setUp(self) -> None:
         self.text = "This string contains test text."
         self.phrase = Phrase("test")
```

### Comparing `fuzzy_search-1.6.0/test/test_fuzzy_match.py` & `fuzzy_search-2.0.0a0/test/test_match_phrase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest import TestCase
 import string
-from fuzzy_search.fuzzy_match import PhraseMatch, PhraseMatchInContext, adjust_match_offsets
-from fuzzy_search.fuzzy_phrase import Phrase
-from fuzzy_search.fuzzy_match import adjust_match_start_offset, adjust_match_end_offset
-from fuzzy_search.fuzzy_match import map_string
+from fuzzy_search.match.phrase_match import PhraseMatch, PhraseMatchInContext, adjust_match_offsets
+from fuzzy_search.phrase.phrase import Phrase
+from fuzzy_search.match.phrase_match import adjust_match_start_offset, adjust_match_end_offset
+from fuzzy_search.match.phrase_match import map_string
 
 
 class TestFuzzyMatch(TestCase):
 
     def test_map_string_maps_word_string(self):
         affix_string = "test"
         mapped_string = map_string(affix_string, string.punctuation)
```

### Comparing `fuzzy_search-1.6.0/test/test_fuzzy_phrase.py` & `fuzzy_search-2.0.0a0/test/test_phrase_phrase.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from unittest import TestCase
 from typing import Generator
-from fuzzy_search.fuzzy_phrase import text2skipgrams, Phrase
+from unittest import TestCase
+
+from fuzzy_search.phrase.phrase import text2skipgrams, Phrase
+from fuzzy_search.tokenization.token import Token
+from fuzzy_search.tokenization.token import Tokenizer
 
 
 class Test(TestCase):
 
     # text2skipgrams
 
     def test_text2skipgrams_rejects_negative_ngram_size(self):
@@ -70,7 +73,35 @@
     def test_fuzzy_phrase_rejects_phrase_with_invalid_label(self):
         error = None
         try:
             Phrase({"phrase": "some phrase", "label": {"complex": "label"}})
         except ValueError as err:
             error = err
         self.assertNotEqual(error, None)
+
+
+class TestPhraseTokens(TestCase):
+
+    def setUp(self) -> None:
+        self.phrase = "some phrase"
+        self.tokenizer = Tokenizer()
+        self.doc = self.tokenizer.tokenize(self.phrase)
+
+    def test_phrase_can_take_tokens(self):
+        phrase = Phrase(self.phrase, tokens=self.doc.tokens)
+        for doc_token, phrase_token in zip(self.doc.tokens, phrase.tokens):
+            with self.subTest(doc_token.char_index):
+                self.assertEqual(doc_token, phrase_token)
+
+    def test_phrase_can_take_tokenizer(self):
+        phrase = Phrase(self.phrase, tokenizer=self.tokenizer)
+        for doc_token, phrase_token in zip(self.doc.tokens, phrase.tokens):
+            with self.subTest(doc_token.char_index):
+                self.assertEqual(doc_token.char_index, phrase_token.char_index)
+
+    def test_phrase_with_tokens_has_token_index(self):
+        phrase = Phrase(self.phrase, tokenizer=self.tokenizer)
+        self.assertEqual(True, 0 in phrase.token_index['some'])
+
+    def test_phrase_with_tokens_has_token_multi_index(self):
+        phrase = Phrase('multiple occurs multiple times', tokenizer=self.tokenizer)
+        self.assertEqual(2, len(phrase.token_index['multiple']))
```

### Comparing `fuzzy_search-1.6.0/test/test_fuzzy_phrase_model.py` & `fuzzy_search-2.0.0a0/test/test_phrase_phrase_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from unittest import TestCase
-from fuzzy_search.fuzzy_phrase_model import PhraseModel
+
+from fuzzy_search.phrase.phrase_model import PhraseModel
+from fuzzy_search.tokenization.token import Tokenizer
 
 
 class Test(TestCase):
 
     def test_making_empty_phrase_model(self):
         phrase_model = PhraseModel()
         self.assertNotEqual(phrase_model, None)
@@ -77,7 +79,20 @@
         phrases = [{"phrase": "okay", "variants": ["OK"]}]
         phrase_model = PhraseModel(phrases=phrases)
         phrase_model.add_variants(phrases)
         phrase_json = phrase_model.json
         self.assertEqual(phrase_json[0]['phrase'], phrases[0]['phrase'])
         self.assertEqual(phrase_json[0]['variants'][0], phrases[0]['variants'][0])
 
+
+class TestPhraseModelTokenizer(TestCase):
+
+    def setUp(self) -> None:
+        self.tokenizer = Tokenizer()
+        self.phrase = 'this is a test'
+        self.phrases = [{"phrase": "this is a test"}]
+        self.phrase_model = PhraseModel(phrases=self.phrases, tokenizer=self.tokenizer)
+
+    def test_can_add_tokenizer_at_init(self):
+        phrase_model = PhraseModel(phrases=self.phrases, tokenizer=self.tokenizer)
+        tokens = self.tokenizer.tokenize(self.phrase)
+        self.assertEqual(True, phrase_model.has_token(tokens[0]))
```

### Comparing `fuzzy_search-1.6.0/test/test_fuzzy_phrase_searcher.py` & `fuzzy_search-2.0.0a0/test/test_search_phrase_searcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,14 @@
 from unittest import TestCase
-from fuzzy_search.fuzzy_phrase import Phrase
-from fuzzy_search.fuzzy_phrase_model import PhraseModel
-from fuzzy_search.fuzzy_string import SkipGram
-from fuzzy_search.fuzzy_phrase_searcher import FuzzyPhraseSearcher, SkipMatches, Candidate
-from fuzzy_search.fuzzy_phrase_searcher import filter_skipgram_threshold, get_skipmatch_candidates
-
-
-class TestSkipMatches(TestCase):
-
-    def test_skip_matches_registers_match(self):
-        skip_matches = SkipMatches(2, 2)
-        phrase = Phrase('test')
-        skipgram = SkipGram('ts', 0, 3)
-        skip_matches.add_skip_match(skipgram, phrase)
-        self.assertTrue(phrase in skip_matches.match_set)
-
-
-class TestCandidate(TestCase):
-
-    def test_candidate_detects_no_match_with_no_skip_match(self):
-        phrase = Phrase('test')
-        candidate = Candidate(phrase)
-        self.assertEqual(candidate.is_match(0.5), False)
-
-    def test_candidate_detects_no_match(self):
-        phrase = Phrase('test')
-        candidate = Candidate(phrase)
-        skipgram = SkipGram('ts', 0, 3)
-        candidate.add_skip_match(skipgram)
-        self.assertEqual(candidate.is_match(0.5), False)
-
-    def test_candidate_has_skipgram_overlap(self):
-        phrase = Phrase('test')
-        candidate = Candidate(phrase)
-        skipgram = SkipGram('ts', 0, 3)
-        candidate.add_skip_match(skipgram)
-        self.assertTrue(candidate.get_skip_set_overlap() > 0.0)
+
+from fuzzy_search.phrase.phrase import Phrase
+from fuzzy_search.phrase.phrase_model import PhraseModel
+from fuzzy_search.search.phrase_searcher import FuzzyPhraseSearcher
+from fuzzy_search.match.skip_match import filter_skipgram_threshold
+from fuzzy_search.match.skip_match import get_skipmatch_candidates
 
 
 class TestFuzzyPhraseSearcher(TestCase):
 
     def setUp(self) -> None:
         self.searcher = FuzzyPhraseSearcher()
 
@@ -206,15 +175,15 @@
     def setUp(self) -> None:
         self.searcher = FuzzyPhraseSearcher()
         self.phrase = {"phrase": "baking", "distractors": ["braking"]}
         self.searcher.index_phrase_model(phrase_model=PhraseModel([self.phrase]))
 
     def test_fuzzy_search_can_search_exact_match(self):
         text = "This text is about baking and not about braking."
-        matches = self.searcher.find_exact_matches(text)
+        matches = self.searcher.find_exact_matches(text, debug=True)
         self.assertEqual(len(matches), 1)
         self.assertEqual(matches[0].string, "baking")
 
     def test_fuzzy_search_can_search_exact_match_with_word_boundaries(self):
         text = "This text is about baking and not about rebaking."
         matches = self.searcher.find_exact_matches(text, use_word_boundaries=True)
         self.assertEqual(len(matches), 1)
```

### Comparing `fuzzy_search-1.6.0/test/test_fuzzy_string.py` & `fuzzy_search-2.0.0a0/test/test_tokenization_string.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from unittest import TestCase
-from fuzzy_search.fuzzy_string import make_ngrams, score_char_overlap, score_char_overlap_ratio
-from fuzzy_search.fuzzy_string import score_ngram_overlap, score_ngram_overlap_ratio
-from fuzzy_search.fuzzy_string import score_levenshtein_distance, score_levenshtein_similarity_ratio
+from fuzzy_search.tokenization.string import make_ngrams, score_char_overlap
+from fuzzy_search.tokenization.string import score_ngram_overlap
+from fuzzy_search.tokenization.string import score_levenshtein_similarity_ratio
 
 
 class Test(TestCase):
 
     ###############
     # make_ngrams #
     ###############
```

### Comparing `fuzzy_search-1.6.0/test/test_fuzzy_template.py` & `fuzzy_search-2.0.0a0/test/test_pattern_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from unittest import TestCase
 
-from fuzzy_search.fuzzy_template import FuzzyTemplate, FuzzyTemplateGroupElement, FuzzyTemplateLabelElement
-from fuzzy_search.fuzzy_phrase import Phrase
-from fuzzy_search.fuzzy_phrase_model import PhraseModel
+from fuzzy_search.pattern.fuzzy_template import FuzzyTemplate, FuzzyTemplateGroupElement, FuzzyTemplateLabelElement
+from fuzzy_search.phrase.phrase import Phrase
+from fuzzy_search.phrase.phrase_model import PhraseModel
 from data.demo_data import DemoData
 
 
 class TestFuzzyTemplateElement(TestCase):
 
     def test_template_accepts_label_only(self):
         template = FuzzyTemplateLabelElement(label="some_label")
```

### Comparing `fuzzy_search-1.6.0/test/test_fuzzy_template_searcher.py` & `fuzzy_search-2.0.0a0/test/test_search_template_searcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from unittest import TestCase
 
-from fuzzy_search.fuzzy_phrase_model import PhraseModel
-from fuzzy_search.fuzzy_phrase import Phrase
-from fuzzy_search.fuzzy_template import FuzzyTemplate
-from fuzzy_search.fuzzy_template_searcher import FuzzyTemplateSearcher, get_phrase_match_list_labels
-from fuzzy_search.fuzzy_match import PhraseMatch
+from fuzzy_search.phrase.phrase_model import PhraseModel
+from fuzzy_search.pattern.fuzzy_template import FuzzyTemplate
+from fuzzy_search.search.template_searcher import FuzzyTemplateSearcher, get_phrase_match_list_labels
+from fuzzy_search.match.phrase_match import PhraseMatch
 
 from data.demo_data import DemoData
 
 
 class TestFuzzyTemplateSearcher(TestCase):
 
     def setUp(self) -> None:
```

