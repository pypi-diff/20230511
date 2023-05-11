# Comparing `tmp/tweety-ns-0.7.0.tar.gz` & `tmp/tweety-ns-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweety-ns-0.7.0.tar", last modified: Sat May  6 14:00:51 2023, max compression
+gzip compressed data, was "tweety-ns-0.7.1.tar", last modified: Thu May 11 11:43:23 2023, max compression
```

## Comparing `tweety-ns-0.7.0.tar` & `tweety-ns-0.7.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 14:00:51.703019 tweety-ns-0.7.0/
--rw-rw-rw-   0        0        0     1019 2023-05-06 14:00:51.704019 tweety-ns-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0      302 2022-10-22 17:49:03.000000 tweety-ns-0.7.0/README.md
--rw-rw-rw-   0        0        0      108 2021-11-15 09:32:36.000000 tweety-ns-0.7.0/pyproject.toml
--rw-rw-rw-   0        0        0      701 2023-05-06 14:00:51.704019 tweety-ns-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0      784 2023-05-06 14:00:17.000000 tweety-ns-0.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:00:51.630502 tweety-ns-0.7.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 14:00:51.691085 tweety-ns-0.7.0/src/tweety/
--rw-rw-rw-   0        0        0       52 2023-05-06 10:37:02.000000 tweety-ns-0.7.0/src/tweety/__init__.py
--rw-rw-rw-   0        0        0     6856 2023-05-06 13:56:24.000000 tweety-ns-0.7.0/src/tweety/bot.py
--rw-rw-rw-   0        0        0    15562 2023-04-24 21:35:55.000000 tweety-ns-0.7.0/src/tweety/builder.py
--rw-rw-rw-   0        0        0    18251 2023-04-24 18:05:20.000000 tweety-ns-0.7.0/src/tweety/exceptions_.py
--rw-rw-rw-   0        0        0      282 2022-03-04 06:53:48.000000 tweety-ns-0.7.0/src/tweety/filters.py
--rw-rw-rw-   0        0        0     5347 2023-05-06 13:19:25.000000 tweety-ns-0.7.0/src/tweety/http.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:00:51.695706 tweety-ns-0.7.0/src/tweety/types/
--rw-rw-rw-   0        0        0       58 2023-03-12 12:43:32.000000 tweety-ns-0.7.0/src/tweety/types/__init__.py
--rw-rw-rw-   0        0        0     2145 2023-04-24 19:05:27.000000 tweety-ns-0.7.0/src/tweety/types/n_types.py
--rw-rw-rw-   0        0        0     4929 2023-04-24 20:14:22.000000 tweety-ns-0.7.0/src/tweety/types/search.py
--rw-rw-rw-   0        0        0    27837 2023-05-06 13:08:01.000000 tweety-ns-0.7.0/src/tweety/types/twDataTypes.py
--rw-rw-rw-   0        0        0     3584 2023-05-06 13:10:36.000000 tweety-ns-0.7.0/src/tweety/types/usertweet.py
--rw-rw-rw-   0        0        0       96 2023-03-13 06:35:02.000000 tweety-ns-0.7.0/src/tweety/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:00:51.703019 tweety-ns-0.7.0/src/tweety_ns.egg-info/
--rw-rw-rw-   0        0        0     1019 2023-05-06 14:00:51.000000 tweety-ns-0.7.0/src/tweety_ns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      523 2023-05-06 14:00:51.000000 tweety-ns-0.7.0/src/tweety_ns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 14:00:51.000000 tweety-ns-0.7.0/src/tweety_ns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-06 14:00:51.000000 tweety-ns-0.7.0/src/tweety_ns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-06 14:00:51.000000 tweety-ns-0.7.0/src/tweety_ns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 11:43:23.921986 tweety-ns-0.7.1/
+-rw-rw-rw-   0        0        0     1019 2023-05-11 11:43:23.921986 tweety-ns-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2022-10-22 17:49:03.000000 tweety-ns-0.7.1/README.md
+-rw-rw-rw-   0        0        0      108 2021-11-15 09:32:36.000000 tweety-ns-0.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0      701 2023-05-11 11:43:23.922982 tweety-ns-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      784 2023-05-11 11:42:58.000000 tweety-ns-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:43:23.895746 tweety-ns-0.7.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 11:43:23.908818 tweety-ns-0.7.1/src/tweety/
+-rw-rw-rw-   0        0        0       54 2023-05-11 11:42:45.000000 tweety-ns-0.7.1/src/tweety/__init__.py
+-rw-rw-rw-   0        0        0     9142 2023-05-11 10:52:50.000000 tweety-ns-0.7.1/src/tweety/bot.py
+-rw-rw-rw-   0        0        0    12483 2023-05-10 20:10:35.000000 tweety-ns-0.7.1/src/tweety/builder.py
+-rw-rw-rw-   0        0        0    18251 2023-04-24 18:05:20.000000 tweety-ns-0.7.1/src/tweety/exceptions_.py
+-rw-rw-rw-   0        0        0      282 2022-03-04 06:53:48.000000 tweety-ns-0.7.1/src/tweety/filters.py
+-rw-rw-rw-   0        0        0     5521 2023-05-11 04:58:39.000000 tweety-ns-0.7.1/src/tweety/http.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:43:23.915121 tweety-ns-0.7.1/src/tweety/types/
+-rw-rw-rw-   0        0        0       58 2023-03-12 12:43:32.000000 tweety-ns-0.7.1/src/tweety/types/__init__.py
+-rw-rw-rw-   0        0        0     2110 2023-05-10 06:18:15.000000 tweety-ns-0.7.1/src/tweety/types/n_types.py
+-rw-rw-rw-   0        0        0     4932 2023-05-11 07:38:05.000000 tweety-ns-0.7.1/src/tweety/types/search.py
+-rw-rw-rw-   0        0        0    27617 2023-05-10 19:53:22.000000 tweety-ns-0.7.1/src/tweety/types/twDataTypes.py
+-rw-rw-rw-   0        0        0     3690 2023-05-11 07:18:05.000000 tweety-ns-0.7.1/src/tweety/types/usertweet.py
+-rw-rw-rw-   0        0        0       96 2023-03-13 06:35:02.000000 tweety-ns-0.7.1/src/tweety/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:43:23.921002 tweety-ns-0.7.1/src/tweety_ns.egg-info/
+-rw-rw-rw-   0        0        0     1019 2023-05-11 11:43:23.000000 tweety-ns-0.7.1/src/tweety_ns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      523 2023-05-11 11:43:23.000000 tweety-ns-0.7.1/src/tweety_ns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 11:43:23.000000 tweety-ns-0.7.1/src/tweety_ns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-11 11:43:23.000000 tweety-ns-0.7.1/src/tweety_ns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-11 11:43:23.000000 tweety-ns-0.7.1/src/tweety_ns.egg-info/top_level.txt
```

### Comparing `tweety-ns-0.7.0/PKG-INFO` & `tweety-ns-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 0.7.0
+Version: 0.7.1
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

### Comparing `tweety-ns-0.7.0/setup.cfg` & `tweety-ns-0.7.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 7765 6574 792d 6e73 0d0a 7665   = tweety-ns..ve
-00000020: 7273 696f 6e20 3d20 302e 372e 300d 0a61  rsion = 0.7.0..a
+00000020: 7273 696f 6e20 3d20 302e 372e 310d 0a61  rsion = 0.7.1..a
 00000030: 7574 686f 7220 3d20 5461 7979 6162 204b  uthor = Tayyab K
 00000040: 6861 726c 0d0a 6175 7468 6f72 5f65 6d61  harl..author_ema
 00000050: 696c 203d 2074 6179 7961 626d 6168 7240  il = tayyabmahr@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2041 6e20 6561 7379  iption = An easy
 00000080: 2054 7769 7474 6572 2053 6372 6170 6572   Twitter Scraper
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

### Comparing `tweety-ns-0.7.0/setup.py` & `tweety-ns-0.7.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='tweety-ns',
     packages=['tweety', 'tweety.types'],
-    version='0.7.0',
+    version='0.7.1',
     license='MIT',
     description='An easy Twitter Scraper',
     author='Tayyab Kharl',
     author_email='tayyabmahr@gmail.com',
     url='https://github.com/mahrtayyab/tweety',
     keywords=['TWITTER', 'TWITTER SCRAPE', 'SCRAPE TWEETS'],
     install_requires=[
```

### Comparing `tweety-ns-0.7.0/src/tweety/bot.py` & `tweety-ns-0.7.1/src/tweety/bot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import functools
+import re
 from typing import Union
 
 from .types.n_types import Proxy
 from .exceptions_ import *
 from .http import Request
 from .types.usertweet import UserTweets
 from .types.search import Search
@@ -66,40 +67,70 @@
         Get the user unique twitter id
 
         :return: int
         """
 
         return self.user.rest_id if self.user else None
 
+    def _get_user_id(self, username):
+        if isinstance(username, User):
+            user_id = username.rest_id
+        elif isinstance(username, int):
+            user_id = username
+        elif isinstance(username, str) and str(username).isdigit():
+            user_id = int(username)
+        else:
+            user_id = self.get_user_info(username).rest_id
+
+        return user_id
+
     def get_tweets(self, username: Union[str, int, User], pages: int = 1, replies: bool = False, wait_time: int = 2, cursor: str = None):
         """
-        Get the tweets from a user
+         Get the tweets from a user
 
         :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
         :param: pages: (`int`) number of pages to be scraped
         :param: replies: (`boolean`) get the replied tweets of the user too
         :param: wait_time: (`int`) seconds to wait between multiple requests
         :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
 
-
         :return: .types.usertweet.UserTweets
         """
         if wait_time is None:
             wait_time = 0
 
-        if isinstance(username, User):
-            user_id = username.rest_id
-        elif isinstance(username, int):
-            user_id = username
-        elif isinstance(username, str) and str(username).isdigit():
-            user_id = int(username)
-        else:
-            user_id = self.get_user_info(username).rest_id
+        user_id = self._get_user_id(username)
+
+        userTweets = UserTweets(user_id, self.request, pages, replies, wait_time, cursor)
+
+        # TODO : Find proper way to run the generator
+        results = [i for i in userTweets.generator()]
+
+        return userTweets
+
+    def iter_tweets(self,  username: Union[str, int, User], pages: int = 1, replies: bool = False, wait_time: int = 2, cursor: str = None):
+        """
+         Generator for getting the tweets from a user
+
+        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: replies: (`boolean`) get the replied tweets of the user too
+        :param: wait_time: (`int`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
 
-        return UserTweets(user_id, self.request, pages, replies, wait_time, cursor)
+        :return: (.types.usertweet.UserTweets, list[.types.twDataTypes.Tweet])
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        user_id = self._get_user_id(username)
+
+        userTweets = UserTweets(user_id, self.request, pages, replies, wait_time, cursor)
+
+        return userTweets.generator()
 
     def get_trends(self):
         """
         Get the Trends from you locale
 
         :return:list of .types.twDataTypes.Trends
         """
@@ -130,38 +161,62 @@
         :param filter_: (
            `str`| `filters.SearchFilters.Users()`| `filters.SearchFilters.Latest()` | `filters.SearchFilters.Photos()` | `filters.SearchFilters.Videos()`
         )
         :param wait_time : (`int`) seconds to wait between multiple requests
         :param cursor: (`str`) Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
 
 
-        :return: .types.search.Search
+        :return: .types.search.Search | if iter: (.types.search.Search, list[.types.twDataTypes.Tweet])
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        search = Search(keyword, self.request, pages, filter_, wait_time, cursor)
+
+        # TODO : Find proper way to run the generator
+        results = [i for i in search.generator()]
+
+        return search
+
+    @AuthRequired
+    def iter_search(self, keyword: str, pages: int = 1, filter_: str = None, wait_time: int = 2, cursor: str = None):
+        """
+        Search for a keyword or hashtag on Twitter
+
+        :param keyword: (`str`) The keyword which is supposed to be searched
+        :param pages: (`int`) The number of pages to get
+        :param filter_: (
+           `str`| `filters.SearchFilters.Users()`| `filters.SearchFilters.Latest()` | `filters.SearchFilters.Photos()` | `filters.SearchFilters.Videos()`
+        )
+        :param wait_time : (`int`) seconds to wait between multiple requests
+        :param cursor: (`str`) Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+
+        :return: (.types.search.Search, list[.types.twDataTypes.Tweet])
         """
         if wait_time is None:
             wait_time = 0
 
-        return Search(keyword, self.request, pages, filter_, wait_time, cursor)
+        search = Search(keyword, self.request, pages, filter_, wait_time, cursor)
+
+        return search.generator()
 
     def tweet_detail(self, identifier: str):
         """
         Get Detail of a single tweet
 
         :param identifier: (`str`) The unique identifier of the tweet , either the `Tweet id` or `Tweet Link`
 
         :return: .types.twDataTypes.Tweet
         """
 
-        if str(identifier).startswith("https://"):
-            if str(identifier).endswith("/"):
-                tweetId = str(identifier)[:-1].split("/")[-1]
-            else:
-                tweetId = str(identifier).split("/")[-1]
-        else:
-            tweetId = identifier
+        tweetId = re.findall("\d+", identifier)[0]
+
         r = self.request.get_tweet_detail(tweetId)
+
         try:
             for entry in r['data']['threaded_conversation_with_injections_v2']['instructions'][0]['entries']:
                 if str(entry['entryId']).split("-")[0] == "tweet":
                     raw_tweet = entry['content']['itemContent']['tweet_results']['result']
 
                     if raw_tweet['rest_id'] == str(tweetId):
                         return Tweet(r, raw_tweet, self.request, True, False, True)
```

### Comparing `tweety-ns-0.7.0/src/tweety/builder.py` & `tweety-ns-0.7.1/src/tweety/builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from urllib.parse import urlencode
 import random
 import string
 from functools import wraps
 
 REQUEST_USER_AGENT = 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36'
 REQUEST_PLATFORMS = ['Linux', 'Windows']
@@ -21,15 +22,15 @@
     URL_API_INIT = "https://twitter.com/i/api/1.1/branch/init.json"
     URL_USER_BY_SCREEN_NAME = "https://api.twitter.com/graphql/rePnxwe9LZ51nQ7Sn_xN_A/UserByScreenName"
     URL_USER_TWEETS = "https://twitter.com/i/api/graphql/OXXUyHfKYZ-xLx4NcL9-_Q/UserTweets"
     URL_USER_TWEETS_WITH_REPLIES = "https://twitter.com/i/api/graphql/nrdle2catTyGnTyj1Qa7wA/UserTweetsAndReplies"
     URL_TRENDS = "https://twitter.com/i/api/2/guide.json"
     URL_SEARCH = "https://twitter.com/i/api/2/search/adaptive.json"
     URL_TWEET_DETAILS = "https://twitter.com/i/api/graphql/1oIoGPTOJN2mSjbbXlQifA/TweetDetail"
-    URL_AUSER_SETTINGS = "https://api.twitter.com/1.1/account/settings.json" # noqa
+    URL_AUSER_SETTINGS = "https://api.twitter.com/1.1/account/settings.json"  # noqa
 
     def __init__(self, cookies=None):
         self.cookies = cookies
         self.user_id = None
         self.guest_token = None
 
     def _get_headers(self):
@@ -78,45 +79,55 @@
 
     @return_with_headers
     def init_api(self):
         return "POST", self.URL_API_INIT
 
     @return_with_headers
     def user_by_screen_name(self, username):
-        params = {
-            'variables': f'{{"screen_name":"{username}","withSafetyModeUserFields":true,"withSuperFollowsUserFields":true}}',
-            'features': '{"responsive_web_twitter_blue_verified_badge_is_enabled":true,"responsive_web_graphql_exclude_directive_enabled":false,"verified_phone_label_enabled":false,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"responsive_web_graphql_timeline_navigation_enabled":true}',
-        }
+        variables = {"screen_name": str(username), "withSafetyModeUserFields": True, "withSuperFollowsUserFields": True}
+        features = {"responsive_web_twitter_blue_verified_badge_is_enabled": True,
+                    "responsive_web_graphql_exclude_directive_enabled": False, "verified_phone_label_enabled": False,
+                    "responsive_web_graphql_skip_user_profile_image_extensions_enabled": False,
+                    "responsive_web_graphql_timeline_navigation_enabled": True}
+
+        params = {'variables': str(json.dumps(variables)), 'features': str(json.dumps(features))}
+
         return "GET", self._build(self.URL_USER_BY_SCREEN_NAME, urlencode(params))
 
     @return_with_headers
     def user_tweets(self, user_id, replies=False, cursor=None):
+        variables = {"userId": str(user_id), "count": 40, "includePromotedContent": True, "withCommunity": True,
+                     "withSuperFollowsUserFields": True, "withDownvotePerspective": False,
+                     "withReactionsMetadata": False, "withReactionsPerspective": False,
+                     "withSuperFollowsTweetFields": True, "withVoice": True, "withV2Timeline": True}
+        features = {"responsive_web_twitter_blue_verified_badge_is_enabled": True,
+                    "rweb_lists_timeline_redesign_enabled": False, "blue_business_profile_image_shape_enabled": True,
+                    "responsive_web_graphql_exclude_directive_enabled": True, "verified_phone_label_enabled": False,
+                    "creator_subscriptions_tweet_preview_api_enabled": False,
+                    "responsive_web_graphql_timeline_navigation_enabled": True,
+                    "responsive_web_graphql_skip_user_profile_image_extensions_enabled": False,
+                    "tweetypie_unmention_optimization_enabled": True, "vibe_api_enabled": True,
+                    "responsive_web_edit_tweet_api_enabled": True,
+                    "graphql_is_translatable_rweb_tweet_is_translatable_enabled": True,
+                    "view_counts_everywhere_api_enabled": True, "longform_notetweets_consumption_enabled": True,
+                    "tweet_awards_web_tipping_enabled": False, "freedom_of_speech_not_reach_fetch_enabled": True,
+                    "standardized_nudges_misinfo": True,
+                    "tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled": False,
+                    "interactive_text_enabled": True, "responsive_web_text_conversations_enabled": False,
+                    "longform_notetweets_rich_text_read_enabled": True,
+                    "longform_notetweets_inline_media_enabled": False, "responsive_web_enhance_cards_enabled": False}
+
+        if cursor:
+            variables['cursor'] = str(cursor)
+
+        params = {'variables': str(json.dumps(variables)), 'features': str(json.dumps(features))}
+
         if replies:
-            if not cursor:
-                params = {
-                    'variables': f'{{"userId":"{user_id}","count":40,"includePromotedContent":true,"withCommunity":true,"withSuperFollowsUserFields":true,"withDownvotePerspective":false,"withReactionsMetadata":false,"withReactionsPerspective":false,"withSuperFollowsTweetFields":true,"withVoice":true,"withV2Timeline":true}}',
-                    'features': '{"responsive_web_twitter_blue_verified_badge_is_enabled":true,"responsive_web_graphql_exclude_directive_enabled":false,"verified_phone_label_enabled":false,"responsive_web_graphql_timeline_navigation_enabled":true,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"tweetypie_unmention_optimization_enabled":true,"vibe_api_enabled":true,"responsive_web_edit_tweet_api_enabled":true,"graphql_is_translatable_rweb_tweet_is_translatable_enabled":true,"view_counts_everywhere_api_enabled":true,"longform_notetweets_consumption_enabled":true,"tweet_awards_web_tipping_enabled":false,"freedom_of_speech_not_reach_fetch_enabled":false,"standardized_nudges_misinfo":true,"tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled":false,"interactive_text_enabled":true,"responsive_web_text_conversations_enabled":false,"responsive_web_enhance_cards_enabled":false}',
-                }
-            else:
-                params = {
-                    'variables': f'{{"userId":"{user_id}","count":40,"cursor":"{cursor}","includePromotedContent":true,"withCommunity":true,"withSuperFollowsUserFields":true,"withDownvotePerspective":false,"withReactionsMetadata":false,"withReactionsPerspective":false,"withSuperFollowsTweetFields":true,"withVoice":true,"withV2Timeline":true}}',
-                    'features': '{"responsive_web_twitter_blue_verified_badge_is_enabled":true,"responsive_web_graphql_exclude_directive_enabled":false,"verified_phone_label_enabled":false,"responsive_web_graphql_timeline_navigation_enabled":true,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"tweetypie_unmention_optimization_enabled":true,"vibe_api_enabled":true,"responsive_web_edit_tweet_api_enabled":true,"graphql_is_translatable_rweb_tweet_is_translatable_enabled":true,"view_counts_everywhere_api_enabled":true,"longform_notetweets_consumption_enabled":true,"tweet_awards_web_tipping_enabled":false,"freedom_of_speech_not_reach_fetch_enabled":false,"standardized_nudges_misinfo":true,"tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled":false,"interactive_text_enabled":true,"responsive_web_text_conversations_enabled":false,"responsive_web_enhance_cards_enabled":false}',
-                }
-            return self._build(self.URL_USER_TWEETS_WITH_REPLIES, urlencode(params))
-
-        if not cursor:
-            params = {
-                'variables': f'{{"userId":"{user_id}","count":40,"includePromotedContent":true,"withQuickPromoteEligibilityTweetFields":true,"withSuperFollowsUserFields":true,"withDownvotePerspective":false,"withReactionsMetadata":false,"withReactionsPerspective":false,"withSuperFollowsTweetFields":true,"withVoice":true,"withV2Timeline":true}}',
-                'features': '{"responsive_web_twitter_blue_verified_badge_is_enabled":true,"responsive_web_graphql_exclude_directive_enabled":false,"verified_phone_label_enabled":false,"responsive_web_graphql_timeline_navigation_enabled":true,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"tweetypie_unmention_optimization_enabled":true,"vibe_api_enabled":true,"responsive_web_edit_tweet_api_enabled":true,"graphql_is_translatable_rweb_tweet_is_translatable_enabled":true,"view_counts_everywhere_api_enabled":true,"longform_notetweets_consumption_enabled":true,"tweet_awards_web_tipping_enabled":false,"freedom_of_speech_not_reach_fetch_enabled":false,"standardized_nudges_misinfo":true,"tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled":false,"interactive_text_enabled":true,"responsive_web_text_conversations_enabled":false,"responsive_web_enhance_cards_enabled":false}',
-            }
-        else:
-            params = {
-                'variables': f'{{"userId":"{user_id}","count":40,"cursor":"{cursor}","includePromotedContent":true,"withQuickPromoteEligibilityTweetFields":true,"withSuperFollowsUserFields":true,"withDownvotePerspective":false,"withReactionsMetadata":false,"withReactionsPerspective":false,"withSuperFollowsTweetFields":true,"withVoice":true,"withV2Timeline":true}}',
-                'features': '{"responsive_web_twitter_blue_verified_badge_is_enabled":true,"responsive_web_graphql_exclude_directive_enabled":false,"verified_phone_label_enabled":false,"responsive_web_graphql_timeline_navigation_enabled":true,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"tweetypie_unmention_optimization_enabled":true,"vibe_api_enabled":true,"responsive_web_edit_tweet_api_enabled":true,"graphql_is_translatable_rweb_tweet_is_translatable_enabled":true,"view_counts_everywhere_api_enabled":true,"longform_notetweets_consumption_enabled":true,"tweet_awards_web_tipping_enabled":false,"freedom_of_speech_not_reach_fetch_enabled":false,"standardized_nudges_misinfo":true,"tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled":false,"interactive_text_enabled":true,"responsive_web_text_conversations_enabled":false,"responsive_web_enhance_cards_enabled":false}',
-            }
+            return "GET", self._build(self.URL_USER_TWEETS_WITH_REPLIES, urlencode(params))
+
         return "GET", self._build(self.URL_USER_TWEETS, urlencode(params))
 
     @return_with_headers
     def trends(self):
         params = {
             'include_profile_interstitial_type': '1',
             'include_blocking': '1',
@@ -184,17 +195,17 @@
             'include_user_entities': 'true',
             'include_ext_media_color': 'true',
             'include_ext_media_availability': 'true',
             'include_ext_sensitive_media_warning': 'true',
             'include_ext_trusted_friends_metadata': 'true',
             'send_error_codes': 'true',
             'simple_quoted_tweet': 'true',
-            'q': keyword,
-            'query_source': 'typeahead_click',
-            'count': '40',
+            'q': str(keyword),
+            'query_source': 'typed_query',
+            'count': '20',
             'requestContext': 'launch',
             'pc': '1',
             'spelling_corrections': '1',
             'include_ext_edit_control': 'true',
             'ext': 'mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,birdwatchPivot,enrichments,superFollowMetadata,unmentionInfo,editControl,vibe',
         }
 
@@ -210,18 +221,19 @@
         if cursor:
             params['cursor'] = cursor
 
         return "GET", self._build(self.URL_SEARCH, urlencode(params))
 
     @return_with_headers
     def tweet_detail(self, tweet_id):
-        params = {
-            'variables': f'{{"focalTweetId":"{tweet_id}","with_rux_injections":false,"includePromotedContent":true,"withCommunity":true,"withQuickPromoteEligibilityTweetFields":true,"withBirdwatchNotes":true,"withDownvotePerspective":false,"withReactionsMetadata":false,"withReactionsPerspective":false,"withVoice":true,"withV2Timeline":true}}',
-            'features': '{"blue_business_profile_image_shape_enabled":false,"responsive_web_graphql_exclude_directive_enabled":true,"verified_phone_label_enabled":false,"responsive_web_graphql_timeline_navigation_enabled":true,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"tweetypie_unmention_optimization_enabled":true,"vibe_api_enabled":true,"responsive_web_edit_tweet_api_enabled":true,"graphql_is_translatable_rweb_tweet_is_translatable_enabled":true,"view_counts_everywhere_api_enabled":true,"longform_notetweets_consumption_enabled":true,"tweet_awards_web_tipping_enabled":false,"freedom_of_speech_not_reach_fetch_enabled":false,"standardized_nudges_misinfo":true,"tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled":false,"interactive_text_enabled":true,"responsive_web_text_conversations_enabled":false,"longform_notetweets_richtext_consumption_enabled":false,"responsive_web_enhance_cards_enabled":false}',
-        }
+        variables = {"focalTweetId":str(tweet_id),"with_rux_injections":False,"includePromotedContent":True,"withCommunity":True,"withQuickPromoteEligibilityTweetFields":True,"withBirdwatchNotes":True,"withDownvotePerspective":False,"withReactionsMetadata":False,"withReactionsPerspective":False,"withVoice":True,"withV2Timeline":True}
+        features = {"blue_business_profile_image_shape_enabled":False,"responsive_web_graphql_exclude_directive_enabled":True,"verified_phone_label_enabled":False,"responsive_web_graphql_timeline_navigation_enabled":True,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":False,"tweetypie_unmention_optimization_enabled":True,"vibe_api_enabled":True,"responsive_web_edit_tweet_api_enabled":True,"graphql_is_translatable_rweb_tweet_is_translatable_enabled":True,"view_counts_everywhere_api_enabled":True,"longform_notetweets_consumption_enabled":True,"tweet_awards_web_tipping_enabled":False,"freedom_of_speech_not_reach_fetch_enabled":False,"standardized_nudges_misinfo":True,"tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled":False,"interactive_text_enabled":True,"responsive_web_text_conversations_enabled":False,"longform_notetweets_richtext_consumption_enabled":False,"responsive_web_enhance_cards_enabled":False}
+
+        params = {'variables': str(json.dumps(variables)), 'features': str(json.dumps(features))}
+
         return "GET", self._build(self.URL_TWEET_DETAILS, urlencode(params))
 
     @return_with_headers
     def aUser_settings(self):
         params = {
             'include_mention_filter': 'true',
             'include_nsfw_user_flag': 'true',
```

### Comparing `tweety-ns-0.7.0/src/tweety/exceptions_.py` & `tweety-ns-0.7.1/src/tweety/exceptions_.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.7.0/src/tweety/http.py` & `tweety-ns-0.7.1/src/tweety/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import warnings
 import httpx as s
 from tqdm import tqdm
 
 from .exceptions_ import GuestTokenNotFound, UnknownError, UserNotFound, InvalidCredentials
 from .types.n_types import GenericError
 from .utils import custom_json
 from .builder import UrlBuilder
@@ -46,17 +45,20 @@
         if not cookies:
             return None
 
         true_cookies = dict()
         if isinstance(cookies, str):
             cookie_list = cookies.split(";")
             for cookie in cookie_list:
-                cookie_key = cookie.strip().split("=")[0]
-                cookie_value = cookie.strip().split("=")[1]
-                true_cookies[cookie_key] = cookie_value
+                split_cookie = cookie.strip().split("=")
+
+                if len(split_cookie) >= 2:
+                    cookie_key = split_cookie[0]
+                    cookie_value = split_cookie[1]
+                    true_cookies[cookie_key] = cookie_value
         elif isinstance(cookies, dict):
             true_cookies = cookies
         else:
             raise TypeError("cookies should be of class 'str' or 'dict' not {}".format(cookies.__class__))
 
         if not true_cookies.get("ct0"):
             raise InvalidCredentials(None, None, None, "'ct0' key in cookies isn't available")
@@ -90,14 +92,18 @@
         if not response.get("screen_name"):
             raise InvalidCredentials(None, None, None)
 
         self.username = response.get("screen_name")
 
     def get_user(self, username=None):
         if not username:
+
+            if not self.username:
+                raise ValueError("'username' is required")
+
             username = self.username
 
         response = self.__get_response__(**self.__builder.user_by_screen_name(username))
 
         if response.get("data"): # noqa
             return response
 
@@ -113,15 +119,15 @@
         return response
 
     def perform_search(self, keyword, cursor, filter_):
         if keyword.startswith("#"):
             keyword = f"%23{keyword[1:]}"
 
         request_data = self.__builder.search(keyword, cursor, filter_)
-        del request_data['headers']['content-type']
+        # del request_data['headers']['content-type']
         request_data['headers']['referer'] = f"https://twitter.com/search?q={keyword}"
 
         response = self.__get_response__(**request_data)
         return response
 
     def get_tweet_detail(self, tweetId):
         response = self.__get_response__(**self.__builder.tweet_detail(tweetId))
```

### Comparing `tweety-ns-0.7.0/src/tweety/types/n_types.py` & `tweety-ns-0.7.1/src/tweety/types/n_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Union
-import socks
 from ..exceptions_ import *
 
-PROXY_TYPES = Union[socks.SOCKS4, socks.SOCKS5, socks.HTTP]
+PROXY_TYPE_SOCKS4 = SOCKS4 = 1
+PROXY_TYPE_SOCKS5 = SOCKS5 = 2
+PROXY_TYPE_HTTP = HTTP = 3
 
 
 class Proxy:
-    def __init__(self, host: str, port: int, proxy_type: PROXY_TYPES, username: str = None, password: str = None):
+    def __init__(self, host: str, port: int, proxy_type: int, username: str = None, password: str = None):
         self.host = host
         self.password = password
         self.proxy_type = proxy_type
         self.username = username
         self.port = port
         self.proxy = self.__parse__()
 
@@ -20,20 +20,20 @@
                 self.username, self.password, self.host, self.password
             )
         else:
             return "{}:{}".format(self.host, self.password)
 
     def __parse__(self):
         proxy_url = self.__proxy_url__()
-        if self.proxy_type == socks.HTTP:
+        if self.proxy_type == HTTP:
             return dict(http=proxy_url, https=proxy_url)
-        elif self.proxy_type == socks.SOCKS4:
+        elif self.proxy_type == SOCKS4:
             socks_url = "socks4://{}".format(proxy_url)
             return dict(http=socks_url, https=socks_url)
-        elif self.proxy_type == socks.SOCKS5:
+        elif self.proxy_type == SOCKS5:
             socks_url = "socks5://{}".format(proxy_url)
             return dict(http=socks_url, https=socks_url)
 
         raise ProxyParseError()
 
 
 class GenericError:
```

### Comparing `tweety-ns-0.7.0/src/tweety/types/search.py` & `tweety-ns-0.7.1/src/tweety/types/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,35 +9,36 @@
         super().__init__()
         self.tweets = []
         self.users = []
         self.keyword = keyword
         self.cursor = cursor
         self.is_next_page = True
         self.http = http
+        self.pages = pages
+        self.wait_time = wait_time
         self.filter = filter_.lower().strip() if filter_ else None
-        self._search(pages, wait_time)
 
     def __repr__(self):
         return "Search(keyword={}, count={}, filter={})".format(
             self.keyword,
             len(self.users) if self.filter == "users" else len(self.tweets),
             self.filter
         )
 
     def get_next_page(self):
-        _tweets = []
         if self.is_next_page:
             response = self.http.perform_search(self.keyword, self.cursor, self.filter)
             thisTweets = self._parse_response(response)
 
             self['is_next_page'] = self.is_next_page
             self['cursor'] = self.cursor
 
             return thisTweets
 
+        return []
     def _parse_response(self, response):
         thisObjects = []
         if self.filter == "users":
             for raw_user in response['globalObjects']['users'].values():
                 try:
                     user = User(raw_user)
                     self.users.append(user)
@@ -81,43 +82,43 @@
                             if newCursor == self.cursor:
                                 return False
                             self.cursor = newCursor
                             return True
                 except:
                     pass
                 try:
-                    for j in response.json()['timeline']['instructions']:
+                    for j in response['timeline']['instructions']:
                         for key in j.keys():
                             if key == "replaceEntry":
                                 if j['replaceEntry']['entry']['content']['operation']['cursor']['cursorType'] == "Bottom":
                                     newCursor = j['replaceEntry']['entry']['content']['operation']['cursor']['value']
                                     if newCursor == self.cursor:
                                         return False
                                     self.cursor = newCursor
                                     return True
                 except:
                     pass
         return False
 
-    def _search(self, pages, wait_time):
-        for page in range(1, int(pages) + 1):
+    def generator(self):
+        for page in range(1, int(self.pages) + 1):
             this_tweets = self.get_next_page()
 
-            if self.is_next_page and page != pages:
-                time.sleep(wait_time)
+            yield self, this_tweets
+
+            if self.is_next_page and page != self.pages:
+                time.sleep(self.wait_time)
+
+        return self
 
     def to_xlsx(self, filename=None):
         if self.filter == "users":
             return AttributeError("to_xlsx with 'users' filter isn't supported yet")
         return Excel(self.tweets, f"search-{self.keyword}", filename)
 
-    @deprecated
-    def to_dict(self):
-        return self.tweets
-
     def __getitem__(self, index):
         if self.filter == "users":
             return self.users[index]
         else:
             return self.tweets[index]
 
     def __iter__(self):
```

### Comparing `tweety-ns-0.7.0/src/tweety/types/twDataTypes.py` & `tweety-ns-0.7.1/src/tweety/types/twDataTypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 import re
 import sys
 import warnings
 from dateutil import parser
 import openpyxl
 import dateutil
 
-try:
-    import wget
-except ModuleNotFoundError:
-    warnings.warn(' "wget" not found in system ,you will not be able to download the medias')
 WORKBOOK_HEADERS = ['Created on', 'author', 'is_retweet', 'is_reply', 'tweet_id', 'tweet_body', 'language', 'likes',
                     'retweet_count', 'source', 'medias', 'user_mentioned', 'urls', 'hashtags', 'symbols']
 
 
 def decodeBase64(encoded_string):
     return str(base64.b64decode(bytes(encoded_string, "utf-8")))[2:-1]
 
@@ -56,15 +52,15 @@
 
     def _set_headers(self):
         for index, value in enumerate(WORKBOOK_HEADERS, start=1):
             self.worksheet.cell(row=1, column=index).value = value
 
     def _write_data(self):
         for tweet in self.tweets:
-            self.worksheet[f'A{self.max_row  + 1}'] = tweet.created_on
+            self.worksheet[f'A{self.max_row  + 1}'] = tweet.date
             self.worksheet[f'B{self.max_row  + 1}'] = tweet.author.name
             self.worksheet[f'C{self.max_row  + 1}'] = tweet.is_retweet
             self.worksheet[f'D{self.max_row  + 1}'] = tweet.is_reply
             self.worksheet[f'E{self.max_row  + 1}'] = tweet.id
             self.worksheet[f'F{self.max_row  + 1}'] = tweet.text
             self.worksheet[f'G{self.max_row  + 1}'] = tweet.language
             self.worksheet[f'H{self.max_row  + 1}'] = tweet.likes
@@ -113,15 +109,15 @@
         if self.threads:  # noqa
             for thread_ in self.threads:  # noqa
                 yield thread_
 
     def _format_tweet(self):
         original_tweet = self._get_original_tweet()
         self.id = self._get_id()
-        self.created_on = dateutil.parser.parse(original_tweet["created_at"])
+        self.created_on = self.date = dateutil.parser.parse(original_tweet["created_at"])
         self.author = self._get_author()
         self.is_retweet = self._is_retweet(original_tweet)
         self.retweeted_tweet = self._get_retweeted_tweet(self.is_retweet, original_tweet)
         self.text = self.tweet_body = self._get_tweet_text(original_tweet, self.is_retweet)
         self.is_quoted = self._is_quoted(original_tweet)
         self.quoted_tweet = self._get_quoted_tweet(self.is_quoted)
         self.is_reply = self._is_reply(original_tweet)
@@ -134,14 +130,15 @@
         self.views = self._get_views()
         self.language = self._get_language(original_tweet)
         self.likes = self._get_likes(original_tweet)
         self.card = self._get_card()
         self.place = self._get_place(original_tweet)
         self.retweet_counts = self._get_retweet_counts(original_tweet)
         self.source = self._get_source(self.__raw_tweet)
+        self.voice_info = None  # TODO
         self.media = self._get_tweet_media(original_tweet)
         self.user_mentions = self._get_tweet_mentions(original_tweet)
         self.urls = self._get_tweet_urls(original_tweet)
         self.hashtags = self._get_tweet_hashtags(original_tweet)
         self.symbols = self._get_tweet_symbols(original_tweet)
         self.threads = []
         self.comments = []
@@ -392,14 +389,15 @@
         self.features = self.__dictionary.get("features")
         self.media_key = self.__dictionary.get("media_key")
         self.mediaStats = self.__dictionary.get("mediaStats")
         self.sizes = [MediaSize(k, v) for k, v in self.__dictionary.get("sizes").items() if self.__dictionary.get('sizes')]
         self.original_info = self.__dictionary.get("original_info")
         self.file_format = self._get_file_format()
         self.streams = []
+
         if self.type == "video" or self.type == "animated_gif":
             self.__parse_video_streams()
 
         for k, v in vars(self).items():
             if not k.startswith("_"):
                 self[k] = v
 
@@ -432,18 +430,14 @@
                         return self.__http.download_media(stream.url, filename, show_progress)
         elif self.type == "animated_gif":
             file_format = self.streams[0].content_type.split("/")[-1]
             if not file_format == "x-mpegURL":
                 return self.__http.download_media(self.streams[0].url, filename, show_progress)
         return None
 
-    @deprecated
-    def to_dict(self):
-        return self.__dictionary
-
 
 class Stream(dict):
     def __init__(self, videoDict, length, ratio, http):
         super().__init__()
         self.__dictionary = videoDict
         self.__http = http
         self.bitrate = self.__dictionary.get("bitrate")
@@ -498,31 +492,25 @@
         for k, v in vars(self).items():
             if not k.startswith("_"):
                 self[k] = v
 
     def __repr__(self):
         return f"ShortUser(id={self.id}, name={self.name})"
 
-    def to_dict(self):
-        return self.__dictionary
-
 
 class Trends:
     def __init__(self, trends_dict):
         self.__dictionary = trends_dict
         self.name = self.__dictionary.get("name")
         self.url = self.__dictionary.get("url")
         self.tweet_count = self.__dictionary.get("tweet_count")
 
     def __repr__(self):
         return f"Trends(name={self.name})"
 
-    def to_dict(self):
-        return self.__dictionary
-
 
 class Card(dict):
     def __init__(self, card_dict):
         super().__init__()
         self._dict = card_dict
         self._bindings = self._dict['legacy'].get("binding_values")
         self.rest_id = self._dict.get("rest_id")
@@ -639,16 +627,17 @@
 
 
 class User(dict):
     def __init__(self, user_data):
         super().__init__()
         self._json = user_data
         self.id = self.rest_id = self.get_id()
-        self.created_at = self.get_created_at()
-        self.description = self._get_key("description")
+        self.created_at = self.date = self.get_created_at()
+        self.entities = self._get_key("entities")
+        self.description = self.bio = self._get_key("description")
         self.fast_followers_count = self._get_key("fast_followers_count")
         self.favourites_count = self._get_key("favourites_count")
         self.followers_count = self._get_key("followers_count")
         self.friends_count = self._get_key("friends_count")
         self.has_custom_timelines = self._get_key("has_custom_timelines")
         self.is_translator = self._get_key("is_translator")
         self.listed_count = self._get_key("listed_count")
@@ -682,14 +671,15 @@
         if verified is False:
             verified = self._get_key("ext_is_blue_verified", False)
 
         return False if verified in (None, False) else True
 
     def get_id(self):
         raw_id = self._json.get("id")
+
         if not str(raw_id).isdigit():
             raw_id = decodeBase64(raw_id).split(":")[-1]
 
         return int(raw_id)
 
     def get_created_at(self):
         date = None
```

### Comparing `tweety-ns-0.7.0/src/tweety/types/usertweet.py` & `tweety-ns-0.7.1/src/tweety/types/usertweet.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,17 @@
         super().__init__()
         self.tweets = []
         self.get_replies = get_replies
         self.cursor = cursor
         self.is_next_page = True
         self.http = http
         self.user_id = user_id
-        self._get_tweets(pages, wait_time)
+        self.pages = pages
+        self.wait_time = wait_time
+        # self._get_tweets(pages, wait_time)
 
     @staticmethod
     def _get_entries(response):
         instructions = response['data']['user']['result']['timeline_v2']['timeline']['instructions']
         for instruction in instructions:
             if instruction.get("type") == "TimelineAddEntries":
                 return instruction['entries']
@@ -62,22 +64,24 @@
             for tweet in _tweets:
                 self.tweets.append(tweet)
 
             self['tweets'] = self.tweets
             self['is_next_page'] = self.is_next_page
             self['cursor'] = self.cursor
 
-            return self
+        return self, _tweets
 
-    def _get_tweets(self, pages, wait_time=2):
-        for page in range(1, int(pages) + 1):
-            self.get_next_page()
+    def generator(self):
+        for page in range(1, int(self.pages) + 1):
+            _, tweets = self.get_next_page()
 
-            if self.is_next_page and page != pages:
-                time.sleep(wait_time)
+            yield self, tweets
+
+            if self.is_next_page and page != self.pages:
+                time.sleep(self.wait_time)
 
     def _get_cursor(self, entries):
         for entry in entries:
             if str(entry['entryId']).split("-")[0] == "cursor":
                 if entry['content']['cursorType'] == "Bottom":
                     newCursor = entry['content']['value']
```

### Comparing `tweety-ns-0.7.0/src/tweety_ns.egg-info/PKG-INFO` & `tweety-ns-0.7.1/src/tweety_ns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 0.7.0
+Version: 0.7.1
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

### Comparing `tweety-ns-0.7.0/src/tweety_ns.egg-info/SOURCES.txt` & `tweety-ns-0.7.1/src/tweety_ns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

