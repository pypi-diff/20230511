# Comparing `tmp/videocdn_tv-0.1.9.tar.gz` & `tmp/videocdn_tv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "videocdn_tv-0.1.9.tar", max compression
+gzip compressed data, was "videocdn_tv-0.2.0.tar", max compression
```

## Comparing `videocdn_tv-0.1.9.tar` & `videocdn_tv-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0      598 2022-08-26 23:37:12.834020 videocdn_tv-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1691 2022-08-12 11:19:16.287103 videocdn_tv-0.1.9/README.md
--rw-r--r--   0        0        0       49 2022-08-12 10:33:20.809459 videocdn_tv-0.1.9/videocdn_tv/__init__.py
--rw-r--r--   0        0        0      229 2022-08-12 12:15:51.146981 videocdn_tv-0.1.9/videocdn_tv/exception.py
--rw-r--r--   0        0        0      648 2022-08-12 09:28:59.934718 videocdn_tv-0.1.9/videocdn_tv/link.py
--rw-r--r--   0        0        0     2609 2022-09-07 11:16:01.274681 videocdn_tv-0.1.9/videocdn_tv/main.py
--rw-r--r--   0        0        0        0 2022-08-12 09:18:44.417239 videocdn_tv-0.1.9/videocdn_tv/models/__init__.py
--rw-r--r--   0        0        0      171 2022-08-14 23:19:53.384525 videocdn_tv-0.1.9/videocdn_tv/models/api/__init__.py
--rw-r--r--   0        0        0      353 2022-09-07 11:39:40.476287 videocdn_tv-0.1.9/videocdn_tv/models/api/anime.py
--rw-r--r--   0        0        0      388 2022-09-07 11:55:25.404799 videocdn_tv-0.1.9/videocdn_tv/models/api/anime_tv_series.py
--rw-r--r--   0        0        0      425 2022-09-07 11:26:54.119946 videocdn_tv-0.1.9/videocdn_tv/models/api/base_api.py
--rw-r--r--   0        0        0      269 2022-09-07 11:39:40.442287 videocdn_tv-0.1.9/videocdn_tv/models/api/movie.py
--rw-r--r--   0        0        0      312 2022-09-07 11:39:40.526286 videocdn_tv-0.1.9/videocdn_tv/models/api/show_tv_series.py
--rw-r--r--   0        0        0      315 2022-09-07 11:45:04.295691 videocdn_tv-0.1.9/videocdn_tv/models/api/tv_series.py
--rw-r--r--   0        0        0     1579 2022-08-14 23:19:53.385525 videocdn_tv-0.1.9/videocdn_tv/models/content.py
--rw-r--r--   0        0        0      126 2022-08-14 23:19:53.385525 videocdn_tv-0.1.9/videocdn_tv/models/contents/__init__.py
--rw-r--r--   0        0        0      428 2022-09-07 11:42:32.563965 videocdn_tv-0.1.9/videocdn_tv/models/contents/episode.py
--rw-r--r--   0        0        0      495 2022-09-06 15:04:30.459765 videocdn_tv-0.1.9/videocdn_tv/models/contents/media.py
--rw-r--r--   0        0        0      131 2022-08-14 23:19:53.386525 videocdn_tv-0.1.9/videocdn_tv/models/contents/qualitie.py
--rw-r--r--   0        0        0      352 2022-08-14 23:19:53.386525 videocdn_tv-0.1.9/videocdn_tv/models/contents/translation.py
--rw-r--r--   0        0        0      627 2022-08-14 23:19:53.386525 videocdn_tv-0.1.9/videocdn_tv/models/episodes/__init__.py
--rw-r--r--   0        0        0      523 2022-08-14 23:19:53.386525 videocdn_tv-0.1.9/videocdn_tv/models/seasons/__init__.py
--rw-r--r--   0        0        0      321 2022-08-12 09:36:07.733331 videocdn_tv-0.1.9/videocdn_tv/models/translation.py
--rw-r--r--   0        0        0      106 2022-08-12 09:49:27.237953 videocdn_tv-0.1.9/videocdn_tv/params/__init__.py
--rw-r--r--   0        0        0      971 2022-08-12 12:09:01.612667 videocdn_tv-0.1.9/videocdn_tv/params/content.py
--rw-r--r--   0        0        0      953 2022-08-12 12:10:40.570236 videocdn_tv-0.1.9/videocdn_tv/params/episode.py
--rw-r--r--   0        0        0      707 2022-08-12 12:15:51.159037 videocdn_tv-0.1.9/videocdn_tv/params/season.py
--rw-r--r--   0        0        0      875 2022-08-12 12:15:51.155014 videocdn_tv-0.1.9/videocdn_tv/request.py
--rw-r--r--   0        0        0        0 2022-08-12 09:20:37.606339 videocdn_tv-0.1.9/videocdn_tv/type/__init__.py
--rw-r--r--   0        0        0       80 2022-08-12 09:24:18.425895 videocdn_tv-0.1.9/videocdn_tv/type/direction.py
--rw-r--r--   0        0        0      154 2022-08-12 09:24:18.407895 videocdn_tv-0.1.9/videocdn_tv/type/field.py
--rw-r--r--   0        0        0      110 2022-08-12 09:24:18.359895 videocdn_tv-0.1.9/videocdn_tv/type/ordering.py
--rw-r--r--   0        0        0     2573 2022-09-07 11:57:16.587209 videocdn_tv-0.1.9/setup.py
--rw-r--r--   0        0        0     2355 2022-09-07 11:57:16.588210 videocdn_tv-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1367 2023-05-10 22:36:32.679967 videocdn_tv-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1691 2022-08-12 11:19:16.287103 videocdn_tv-0.2.0/README.md
+-rw-r--r--   0        0        0      108 2023-05-10 19:06:24.105020 videocdn_tv-0.2.0/videocdn_tv/__init__.py
+-rw-r--r--   0        0        0      250 2023-05-10 22:35:59.019892 videocdn_tv-0.2.0/videocdn_tv/exception.py
+-rw-r--r--   0        0        0      648 2022-08-12 09:28:59.934718 videocdn_tv-0.2.0/videocdn_tv/link.py
+-rw-r--r--   0        0        0     3301 2023-05-10 22:37:07.804833 videocdn_tv-0.2.0/videocdn_tv/main.py
+-rw-r--r--   0        0        0        0 2022-08-12 09:18:44.417239 videocdn_tv-0.2.0/videocdn_tv/models/__init__.py
+-rw-r--r--   0        0        0      259 2023-05-10 22:37:07.806834 videocdn_tv-0.2.0/videocdn_tv/models/api/__init__.py
+-rw-r--r--   0        0        0      415 2023-05-10 22:10:37.476870 videocdn_tv-0.2.0/videocdn_tv/models/api/anime.py
+-rw-r--r--   0        0        0      465 2023-05-10 20:06:48.842008 videocdn_tv-0.2.0/videocdn_tv/models/api/anime_tv_series.py
+-rw-r--r--   0        0        0      541 2023-05-10 22:14:28.572780 videocdn_tv-0.2.0/videocdn_tv/models/api/base_api.py
+-rw-r--r--   0        0        0      336 2023-05-10 22:07:15.807383 videocdn_tv-0.2.0/videocdn_tv/models/api/movie.py
+-rw-r--r--   0        0        0      367 2023-05-10 20:06:48.822008 videocdn_tv-0.2.0/videocdn_tv/models/api/show_tv_series.py
+-rw-r--r--   0        0        0      184 2023-05-10 22:37:07.155195 videocdn_tv-0.2.0/videocdn_tv/models/api/translations.py
+-rw-r--r--   0        0        0      396 2023-05-10 22:14:35.553293 videocdn_tv-0.2.0/videocdn_tv/models/api/tv_series.py
+-rw-r--r--   0        0        0      446 2023-05-10 22:37:07.173195 videocdn_tv-0.2.0/videocdn_tv/models/base.py
+-rw-r--r--   0        0        0      158 2023-05-10 19:05:27.111647 videocdn_tv-0.2.0/videocdn_tv/models/contents/__init__.py
+-rw-r--r--   0        0        0      500 2023-05-10 22:12:55.033915 videocdn_tv-0.2.0/videocdn_tv/models/contents/episode.py
+-rw-r--r--   0        0        0      578 2023-05-10 22:12:26.391122 videocdn_tv-0.2.0/videocdn_tv/models/contents/media.py
+-rw-r--r--   0        0        0      172 2023-05-10 21:41:58.313353 videocdn_tv-0.2.0/videocdn_tv/models/contents/qualitie.py
+-rw-r--r--   0        0        0      454 2023-05-10 22:13:50.130699 videocdn_tv-0.2.0/videocdn_tv/models/contents/translation.py
+-rw-r--r--   0        0        0      697 2023-05-10 19:43:24.019711 videocdn_tv-0.2.0/videocdn_tv/models/episodes.py
+-rw-r--r--   0        0        0     1448 2023-05-10 22:37:07.829833 videocdn_tv-0.2.0/videocdn_tv/models/response.py
+-rw-r--r--   0        0        0      583 2023-05-10 20:06:48.832008 videocdn_tv-0.2.0/videocdn_tv/models/seasons.py
+-rw-r--r--   0        0        0      130 2023-05-10 19:06:24.150021 videocdn_tv-0.2.0/videocdn_tv/params/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-10 22:37:07.143196 videocdn_tv-0.2.0/videocdn_tv/params/base.py
+-rw-r--r--   0        0        0      618 2023-05-10 21:16:53.372997 videocdn_tv-0.2.0/videocdn_tv/params/content.py
+-rw-r--r--   0        0        0      636 2023-05-10 20:07:56.776517 videocdn_tv-0.2.0/videocdn_tv/params/episode.py
+-rw-r--r--   0        0        0      348 2023-05-10 20:06:49.560522 videocdn_tv-0.2.0/videocdn_tv/params/season.py
+-rw-r--r--   0        0        0      983 2023-05-10 22:35:59.002509 videocdn_tv-0.2.0/videocdn_tv/request.py
+-rw-r--r--   0        0        0        0 2022-08-12 09:20:37.606339 videocdn_tv-0.2.0/videocdn_tv/type/__init__.py
+-rw-r--r--   0        0        0       82 2023-05-10 19:00:45.033647 videocdn_tv-0.2.0/videocdn_tv/type/direction.py
+-rw-r--r--   0        0        0      156 2023-05-10 19:00:45.040646 videocdn_tv-0.2.0/videocdn_tv/type/field.py
+-rw-r--r--   0        0        0      117 2023-05-10 20:06:49.497524 videocdn_tv-0.2.0/videocdn_tv/type/ordering.py
+-rw-r--r--   0        0        0     2411 1970-01-01 00:00:00.000000 videocdn_tv-0.2.0/PKG-INFO
```

### Comparing `videocdn_tv-0.1.9/README.md` & `videocdn_tv-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `videocdn_tv-0.1.9/videocdn_tv/link.py` & `videocdn_tv-0.2.0/videocdn_tv/link.py`

 * *Files identical despite different names*

### Comparing `videocdn_tv-0.1.9/videocdn_tv/main.py` & `videocdn_tv-0.2.0/videocdn_tv/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,111 @@
-from videocdn_tv.link import *
-from videocdn_tv.models.content import (
-    MovieContent, AnimeContent, TvSeriesContent, AnimeTvSeriesContent, ShowTvSeriesContent,
-    ShowTvSeriesSeasonsContent, AnimeTvSeriesSeasonsContent, TvSeriesSeasonsContent, TvSeriesEpisodesContent,
-    AnimeTvSeriesEpisodesContent, ShowTvSeriesEpisodesContent
+from videocdn_tv.link import (
+    ANIME_TV_SERIES,
+    ANIME_TV_SERIES_EPISODES,
+    ANIME_TV_SERIES_SEASONS,
+    MOVIES,
+    SHOW_TV_SERIES,
+    SHOW_TV_SERIES_EPISODES,
+    SHOW_TV_SERIES_SEASONS,
+    TRANSLATIONS,
+    TV_SERIES,
+    TV_SERIES_EPISODES,
+    TV_SERIES_SEASONS,
 )
-from videocdn_tv.models.translation import TranslationModel
-
-from videocdn_tv.params import *
+from videocdn_tv.models.response import (
+    AnimeContent,
+    AnimeTvSeriesContent,
+    AnimeTvSeriesEpisodesContent,
+    AnimeTvSeriesSeasonsContent,
+    MovieContent,
+    ShowTvSeriesContent,
+    ShowTvSeriesEpisodesContent,
+    ShowTvSeriesSeasonsContent,
+    TranslationModel,
+    TvSeriesContent,
+    TvSeriesEpisodesContent,
+    TvSeriesSeasonsContent,
+)
+from videocdn_tv.params import ParamsContent, ParamsEpisode, ParamsSeason
 from videocdn_tv.request import get_request
 
 
 class VideoCDN:
     def __init__(self, api_token: str):
-        self.params = {'api_token': api_token}
+        self.params = {"api_token": api_token}
 
     def get_translations(self) -> TranslationModel:
         return TranslationModel(**get_request(self, TRANSLATIONS))
 
-    def get_movies(self, params: ParamsContent) -> MovieContent:
+    def get_movies(
+        self,
+        params: ParamsContent,
+    ) -> MovieContent:
         return MovieContent(**get_request(self, MOVIES, params))
 
-    def get_animes(self, params: ParamsContent) -> AnimeContent:
+    def get_animes(
+        self,
+        params: ParamsContent,
+    ) -> AnimeContent:
         return AnimeContent(**get_request(self, MOVIES, params))
 
-    def get_tv_series(self, params: ParamsContent) -> TvSeriesContent:
+    def get_tv_series(
+        self,
+        params: ParamsContent,
+    ) -> TvSeriesContent:
         return TvSeriesContent(**get_request(self, TV_SERIES, params))
 
-    def get_tv_series_seasons(self, params: ParamsSeason) -> TvSeriesSeasonsContent:
+    def get_tv_series_seasons(
+        self,
+        params: ParamsSeason,
+    ) -> TvSeriesSeasonsContent:
         return TvSeriesSeasonsContent(**get_request(self, TV_SERIES_SEASONS, params))
 
-    def get_tv_series_episodes(self, params: ParamsEpisode) -> TvSeriesEpisodesContent:
+    def get_tv_series_episodes(
+        self,
+        params: ParamsEpisode,
+    ) -> TvSeriesEpisodesContent:
         return TvSeriesEpisodesContent(**get_request(self, TV_SERIES_EPISODES, params))
 
-    def get_anime_tv_series(self, params: ParamsContent) -> AnimeTvSeriesContent:
+    def get_anime_tv_series(
+        self,
+        params: ParamsContent,
+    ) -> AnimeTvSeriesContent:
         return AnimeTvSeriesContent(**get_request(self, ANIME_TV_SERIES, params))
 
-    def get_anime_tv_series_seasons(self, params: ParamsSeason) -> AnimeTvSeriesSeasonsContent:
-        return AnimeTvSeriesSeasonsContent(**get_request(self, ANIME_TV_SERIES_SEASONS, params))
-
-    def get_anime_tv_series_episodes(self, params: ParamsEpisode) -> AnimeTvSeriesEpisodesContent:
-        return AnimeTvSeriesEpisodesContent(**get_request(self, ANIME_TV_SERIES_EPISODES, params))
-
-    def get_show_tv_series(self, params: ParamsContent) -> ShowTvSeriesContent:
+    def get_anime_tv_series_seasons(
+        self,
+        params: ParamsSeason,
+    ) -> AnimeTvSeriesSeasonsContent:
+        return AnimeTvSeriesSeasonsContent(
+            **get_request(self, ANIME_TV_SERIES_SEASONS, params),
+        )
+
+    def get_anime_tv_series_episodes(
+        self,
+        params: ParamsEpisode,
+    ) -> AnimeTvSeriesEpisodesContent:
+        return AnimeTvSeriesEpisodesContent(
+            **get_request(self, ANIME_TV_SERIES_EPISODES, params),
+        )
+
+    def get_show_tv_series(
+        self,
+        params: ParamsContent,
+    ) -> ShowTvSeriesContent:
         return ShowTvSeriesContent(**get_request(self, SHOW_TV_SERIES, params))
 
-    def get_show_tv_series_season(self, params: ParamsSeason) -> ShowTvSeriesSeasonsContent:
-        return ShowTvSeriesSeasonsContent(**get_request(self, SHOW_TV_SERIES_SEASONS, params))
-
-    def get_show_tv_series_episodes(self, params: ParamsEpisode) -> ShowTvSeriesEpisodesContent:
-        return ShowTvSeriesEpisodesContent(**get_request(self, SHOW_TV_SERIES_EPISODES, params))
+    def get_show_tv_series_season(
+        self,
+        params: ParamsSeason,
+    ) -> ShowTvSeriesSeasonsContent:
+        return ShowTvSeriesSeasonsContent(
+            **get_request(self, SHOW_TV_SERIES_SEASONS, params),
+        )
+
+    def get_show_tv_series_episodes(
+        self,
+        params: ParamsEpisode,
+    ) -> ShowTvSeriesEpisodesContent:
+        return ShowTvSeriesEpisodesContent(
+            **get_request(self, SHOW_TV_SERIES_EPISODES, params),
+        )
```

### Comparing `videocdn_tv-0.1.9/videocdn_tv/params/content.py` & `videocdn_tv-0.2.0/videocdn_tv/params/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 from dataclasses import dataclass
+from typing import Optional
 
 from videocdn_tv.type.direction import Direction
-from videocdn_tv.type.field import Field
 from videocdn_tv.type.ordering import Ordering
 
 
 @dataclass
-class ParamsContent:
+class BaseParams:
     ordering: Ordering = Ordering.ID
     direction: Direction = Direction.ASC
-    field: Field = None
-    query: str = None
-    translation: int = None
-    year: int = None
-    page: int = None
+    page: Optional[int] = None
     limit: int = 10
 
-    def __str__(self):
+    def validate(self) -> None:
         if self.limit < 0 or self.limit > 100:
             raise ValueError("Limit больше 100 или меньше 0")
 
-        return {'ordering': self.ordering.value,
-                'direction': self.direction.value,
-                'field': self.field.value if self.field is not None else None,
-                'query': self.query,
-                'translation': self.translation,
-                'year': self.year,
-                'page': self.page,
-                'limit': self.limit}
+    def as_dict(self) -> dict:
+        return {
+            "ordering": self.ordering.value,
+            "direction": self.direction.value,
+            "page": self.page,
+            "limit": self.limit,
+        }
```

### Comparing `videocdn_tv-0.1.9/videocdn_tv/request.py` & `videocdn_tv-0.2.0/videocdn_tv/request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import json
 from json import JSONDecodeError
-from typing import Union, Any
+from typing import Any, Optional, Union
 
-import requests
+import httpx
 
-from videocdn_tv.exception import ApiFailedException, ApiTokenInvalid
-from videocdn_tv.params import *
+from videocdn_tv.exception import ApiFailedError, ApiTokenInvalidError
+from videocdn_tv.params import ParamsContent, ParamsEpisode, ParamsSeason
 
 
-def get_request(self,
-                link: str,
-                params: Union[ParamsContent, ParamsSeason, ParamsEpisode] = None) -> Any:
+def get_request(
+    self,
+    link: str,
+    params: Optional[Union[ParamsContent, ParamsSeason, ParamsEpisode]] = None,
+) -> Any:
     if params is not None:
-        params = {**self.params, **params.__str__()}
+        params.validate()
+        params = {**self.params, **params.as_dict()}
     else:
         params = self.params
 
-    response = requests.get(link, params=params)
+    response = httpx.get(link, params=params, timeout=90)
 
     if response.status_code == 200:
         try:
             return json.loads(response.text)
-        except JSONDecodeError:
-            raise ApiTokenInvalid
+        except JSONDecodeError as error:
+            raise ApiTokenInvalidError(error) from error
     elif response.status_code == 500:
-        raise ApiFailedException(response.status_code, response.text)
+        raise ApiFailedError(response.status_code, response.text)
     else:
         raise Exception(response.status_code, response.text)
```

### Comparing `videocdn_tv-0.1.9/setup.py` & `videocdn_tv-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,107 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: videocdn-tv
+Version: 0.2.0
+Summary: Реализация Api для сервиса VideoCDN.tv
+Home-page: https://github.com/odi1n/VideoCDN
+License: MIT
+Keywords: videocdn,videocdn-tv
+Author: Your Name
+Author-email: you@example.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: pydantic (>=1.9.2,<2.0.0)
+Project-URL: Documentation, https://github.com/odi1n/VideoCDN/blob/master/README.md
+Project-URL: Repository, https://github.com/odi1n/VideoCDN
+Description-Content-Type: text/markdown
 
-packages = \
-['videocdn_tv',
- 'videocdn_tv.models',
- 'videocdn_tv.models.api',
- 'videocdn_tv.models.contents',
- 'videocdn_tv.models.episodes',
- 'videocdn_tv.models.seasons',
- 'videocdn_tv.params',
- 'videocdn_tv.type']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pydantic>=1.9.2,<2.0.0', 'requests==2.26.0']
-
-setup_kwargs = {
-    'name': 'videocdn-tv',
-    'version': '0.1.9',
-    'description': 'Реализация Api для сервиса VideoCDN.tv',
-    'long_description': '# VideoCND - API\n\nРеализация Api для сервиса VideoCDN.tv\n\nУстановка:```pip install videocdn-tv```\n\n## Методы\n\nВзаимодействие:\n\n```python\nfrom .videocdn import VideoCDN, ParamsContent, ParamsEpisode, ParamsSeason\nvideocdn = VideoCDN(api_token="KEY")\n```\n\n### translations\n\n```python\ndata = videocdn.get_translations()\n```\n\n### movies\n\n```python\ndata = videocdn.get_movies(ParamsContent(query="Аквамене"))\n```\n\n### animes\n\n```python\ndata = videocdn.get_animes(ParamsContent(query="Ван-Пис: Золото"))\n```\n\n### tv-series\n\n```python\ndata = videocdn.get_tv_series(ParamsContent(query="Игра Пристолов"))\n```\n\n### tv-series/seasons\n\n```python\ndata = videocdn.get_tv_series_seasons(ParamsSeason(tv_series_id=1))\n```\n\n### tv-series/episodes\n\n```python\ndata = videocdn.get_tv_series_episodes(ParamsEpisode(tv_series_id=1))\n```\n\n### anime-tv-series\n\n```python\ndata = videocdn.get_anime_tv_series(ParamsContent(query="Доктор Стоун"))\n```\n\n### anime-tv-series/seasons\n\n```python\ndata = videocdn.get_anime_tv_series_seasons(ParamsSeason(tv_series_id=1))\n```\n\n### anime-tv-series/episodes\n\n```python\ndata = videocdn.get_anime_tv_series_episodes(ParamsEpisode(tv_series_id=1))\n```\n\n### show-tv-series\n\n```python\ndata = videocdn.get_show_tv_series(ParamsContent(query="Зовите шефа"))\n```\n\n### show-tv-series/seasons\n\n```python\ndata = videocdn.get_show_tv_series_season(ParamsSeason(tv_series_id=1))\n```\n\n### show-tv-series/episodes\n\n```python\ndata = videocdn.get_show_tv_series_episodes(ParamsEpisode(tv_series_id=1))\n```',
-    'author': 'Your Name',
-    'author_email': 'you@example.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/odi1n/VideoCDN',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+# VideoCND - API
 
+Реализация Api для сервиса VideoCDN.tv
 
-setup(**setup_kwargs)
+Установка:```pip install videocdn-tv```
+
+## Методы
+
+Взаимодействие:
+
+```python
+from .videocdn import VideoCDN, ParamsContent, ParamsEpisode, ParamsSeason
+videocdn = VideoCDN(api_token="KEY")
+```
+
+### translations
+
+```python
+data = videocdn.get_translations()
+```
+
+### movies
+
+```python
+data = videocdn.get_movies(ParamsContent(query="Аквамене"))
+```
+
+### animes
+
+```python
+data = videocdn.get_animes(ParamsContent(query="Ван-Пис: Золото"))
+```
+
+### tv-series
+
+```python
+data = videocdn.get_tv_series(ParamsContent(query="Игра Пристолов"))
+```
+
+### tv-series/seasons
+
+```python
+data = videocdn.get_tv_series_seasons(ParamsSeason(tv_series_id=1))
+```
+
+### tv-series/episodes
+
+```python
+data = videocdn.get_tv_series_episodes(ParamsEpisode(tv_series_id=1))
+```
+
+### anime-tv-series
+
+```python
+data = videocdn.get_anime_tv_series(ParamsContent(query="Доктор Стоун"))
+```
+
+### anime-tv-series/seasons
+
+```python
+data = videocdn.get_anime_tv_series_seasons(ParamsSeason(tv_series_id=1))
+```
+
+### anime-tv-series/episodes
+
+```python
+data = videocdn.get_anime_tv_series_episodes(ParamsEpisode(tv_series_id=1))
+```
+
+### show-tv-series
+
+```python
+data = videocdn.get_show_tv_series(ParamsContent(query="Зовите шефа"))
+```
+
+### show-tv-series/seasons
+
+```python
+data = videocdn.get_show_tv_series_season(ParamsSeason(tv_series_id=1))
+```
+
+### show-tv-series/episodes
+
+```python
+data = videocdn.get_show_tv_series_episodes(ParamsEpisode(tv_series_id=1))
+```
```

