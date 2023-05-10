# Comparing `tmp/videocdn_tv-0.2.0.tar.gz` & `tmp/videocdn_tv-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "videocdn_tv-0.2.0.tar", max compression
+gzip compressed data, was "videocdn_tv-0.2.1.tar", max compression
```

## Comparing `videocdn_tv-0.2.0.tar` & `videocdn_tv-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1367 2023-05-10 22:36:32.679967 videocdn_tv-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1691 2022-08-12 11:19:16.287103 videocdn_tv-0.2.0/README.md
--rw-r--r--   0        0        0      108 2023-05-10 19:06:24.105020 videocdn_tv-0.2.0/videocdn_tv/__init__.py
--rw-r--r--   0        0        0      250 2023-05-10 22:35:59.019892 videocdn_tv-0.2.0/videocdn_tv/exception.py
--rw-r--r--   0        0        0      648 2022-08-12 09:28:59.934718 videocdn_tv-0.2.0/videocdn_tv/link.py
--rw-r--r--   0        0        0     3301 2023-05-10 22:37:07.804833 videocdn_tv-0.2.0/videocdn_tv/main.py
--rw-r--r--   0        0        0        0 2022-08-12 09:18:44.417239 videocdn_tv-0.2.0/videocdn_tv/models/__init__.py
--rw-r--r--   0        0        0      259 2023-05-10 22:37:07.806834 videocdn_tv-0.2.0/videocdn_tv/models/api/__init__.py
--rw-r--r--   0        0        0      415 2023-05-10 22:10:37.476870 videocdn_tv-0.2.0/videocdn_tv/models/api/anime.py
--rw-r--r--   0        0        0      465 2023-05-10 20:06:48.842008 videocdn_tv-0.2.0/videocdn_tv/models/api/anime_tv_series.py
--rw-r--r--   0        0        0      541 2023-05-10 22:14:28.572780 videocdn_tv-0.2.0/videocdn_tv/models/api/base_api.py
--rw-r--r--   0        0        0      336 2023-05-10 22:07:15.807383 videocdn_tv-0.2.0/videocdn_tv/models/api/movie.py
--rw-r--r--   0        0        0      367 2023-05-10 20:06:48.822008 videocdn_tv-0.2.0/videocdn_tv/models/api/show_tv_series.py
--rw-r--r--   0        0        0      184 2023-05-10 22:37:07.155195 videocdn_tv-0.2.0/videocdn_tv/models/api/translations.py
--rw-r--r--   0        0        0      396 2023-05-10 22:14:35.553293 videocdn_tv-0.2.0/videocdn_tv/models/api/tv_series.py
--rw-r--r--   0        0        0      446 2023-05-10 22:37:07.173195 videocdn_tv-0.2.0/videocdn_tv/models/base.py
--rw-r--r--   0        0        0      158 2023-05-10 19:05:27.111647 videocdn_tv-0.2.0/videocdn_tv/models/contents/__init__.py
--rw-r--r--   0        0        0      500 2023-05-10 22:12:55.033915 videocdn_tv-0.2.0/videocdn_tv/models/contents/episode.py
--rw-r--r--   0        0        0      578 2023-05-10 22:12:26.391122 videocdn_tv-0.2.0/videocdn_tv/models/contents/media.py
--rw-r--r--   0        0        0      172 2023-05-10 21:41:58.313353 videocdn_tv-0.2.0/videocdn_tv/models/contents/qualitie.py
--rw-r--r--   0        0        0      454 2023-05-10 22:13:50.130699 videocdn_tv-0.2.0/videocdn_tv/models/contents/translation.py
--rw-r--r--   0        0        0      697 2023-05-10 19:43:24.019711 videocdn_tv-0.2.0/videocdn_tv/models/episodes.py
--rw-r--r--   0        0        0     1448 2023-05-10 22:37:07.829833 videocdn_tv-0.2.0/videocdn_tv/models/response.py
--rw-r--r--   0        0        0      583 2023-05-10 20:06:48.832008 videocdn_tv-0.2.0/videocdn_tv/models/seasons.py
--rw-r--r--   0        0        0      130 2023-05-10 19:06:24.150021 videocdn_tv-0.2.0/videocdn_tv/params/__init__.py
--rw-r--r--   0        0        0      716 2023-05-10 22:37:07.143196 videocdn_tv-0.2.0/videocdn_tv/params/base.py
--rw-r--r--   0        0        0      618 2023-05-10 21:16:53.372997 videocdn_tv-0.2.0/videocdn_tv/params/content.py
--rw-r--r--   0        0        0      636 2023-05-10 20:07:56.776517 videocdn_tv-0.2.0/videocdn_tv/params/episode.py
--rw-r--r--   0        0        0      348 2023-05-10 20:06:49.560522 videocdn_tv-0.2.0/videocdn_tv/params/season.py
--rw-r--r--   0        0        0      983 2023-05-10 22:35:59.002509 videocdn_tv-0.2.0/videocdn_tv/request.py
--rw-r--r--   0        0        0        0 2022-08-12 09:20:37.606339 videocdn_tv-0.2.0/videocdn_tv/type/__init__.py
--rw-r--r--   0        0        0       82 2023-05-10 19:00:45.033647 videocdn_tv-0.2.0/videocdn_tv/type/direction.py
--rw-r--r--   0        0        0      156 2023-05-10 19:00:45.040646 videocdn_tv-0.2.0/videocdn_tv/type/field.py
--rw-r--r--   0        0        0      117 2023-05-10 20:06:49.497524 videocdn_tv-0.2.0/videocdn_tv/type/ordering.py
--rw-r--r--   0        0        0     2411 1970-01-01 00:00:00.000000 videocdn_tv-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1367 2023-05-10 22:48:13.672660 videocdn_tv-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1691 2022-08-12 11:19:16.287103 videocdn_tv-0.2.1/README.md
+-rw-r--r--   0        0        0      108 2023-05-10 19:06:24.105020 videocdn_tv-0.2.1/videocdn_tv/__init__.py
+-rw-r--r--   0        0        0      250 2023-05-10 22:35:59.019892 videocdn_tv-0.2.1/videocdn_tv/exception.py
+-rw-r--r--   0        0        0      648 2022-08-12 09:28:59.934718 videocdn_tv-0.2.1/videocdn_tv/link.py
+-rw-r--r--   0        0        0     3301 2023-05-10 22:37:07.804833 videocdn_tv-0.2.1/videocdn_tv/main.py
+-rw-r--r--   0        0        0        0 2022-08-12 09:18:44.417239 videocdn_tv-0.2.1/videocdn_tv/models/__init__.py
+-rw-r--r--   0        0        0      259 2023-05-10 22:37:07.806834 videocdn_tv-0.2.1/videocdn_tv/models/api/__init__.py
+-rw-r--r--   0        0        0      415 2023-05-10 22:10:37.476870 videocdn_tv-0.2.1/videocdn_tv/models/api/anime.py
+-rw-r--r--   0        0        0      465 2023-05-10 20:06:48.842008 videocdn_tv-0.2.1/videocdn_tv/models/api/anime_tv_series.py
+-rw-r--r--   0        0        0      541 2023-05-10 22:14:28.572780 videocdn_tv-0.2.1/videocdn_tv/models/api/base_api.py
+-rw-r--r--   0        0        0      336 2023-05-10 22:07:15.807383 videocdn_tv-0.2.1/videocdn_tv/models/api/movie.py
+-rw-r--r--   0        0        0      367 2023-05-10 20:06:48.822008 videocdn_tv-0.2.1/videocdn_tv/models/api/show_tv_series.py
+-rw-r--r--   0        0        0      184 2023-05-10 22:37:07.155195 videocdn_tv-0.2.1/videocdn_tv/models/api/translations.py
+-rw-r--r--   0        0        0      396 2023-05-10 22:14:35.553293 videocdn_tv-0.2.1/videocdn_tv/models/api/tv_series.py
+-rw-r--r--   0        0        0      446 2023-05-10 22:37:07.173195 videocdn_tv-0.2.1/videocdn_tv/models/base.py
+-rw-r--r--   0        0        0      158 2023-05-10 19:05:27.111647 videocdn_tv-0.2.1/videocdn_tv/models/contents/__init__.py
+-rw-r--r--   0        0        0      500 2023-05-10 22:12:55.033915 videocdn_tv-0.2.1/videocdn_tv/models/contents/episode.py
+-rw-r--r--   0        0        0      578 2023-05-10 22:12:26.391122 videocdn_tv-0.2.1/videocdn_tv/models/contents/media.py
+-rw-r--r--   0        0        0      172 2023-05-10 21:41:58.313353 videocdn_tv-0.2.1/videocdn_tv/models/contents/qualitie.py
+-rw-r--r--   0        0        0      454 2023-05-10 22:13:50.130699 videocdn_tv-0.2.1/videocdn_tv/models/contents/translation.py
+-rw-r--r--   0        0        0      697 2023-05-10 19:43:24.019711 videocdn_tv-0.2.1/videocdn_tv/models/episodes.py
+-rw-r--r--   0        0        0     1448 2023-05-10 22:37:07.829833 videocdn_tv-0.2.1/videocdn_tv/models/response.py
+-rw-r--r--   0        0        0      583 2023-05-10 20:06:48.832008 videocdn_tv-0.2.1/videocdn_tv/models/seasons.py
+-rw-r--r--   0        0        0      130 2023-05-10 19:06:24.150021 videocdn_tv-0.2.1/videocdn_tv/params/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-10 22:37:07.143196 videocdn_tv-0.2.1/videocdn_tv/params/base.py
+-rw-r--r--   0        0        0      618 2023-05-10 21:16:53.372997 videocdn_tv-0.2.1/videocdn_tv/params/content.py
+-rw-r--r--   0        0        0      636 2023-05-10 20:07:56.776517 videocdn_tv-0.2.1/videocdn_tv/params/episode.py
+-rw-r--r--   0        0        0      348 2023-05-10 20:06:49.560522 videocdn_tv-0.2.1/videocdn_tv/params/season.py
+-rw-r--r--   0        0        0      983 2023-05-10 22:35:59.002509 videocdn_tv-0.2.1/videocdn_tv/request.py
+-rw-r--r--   0        0        0        0 2022-08-12 09:20:37.606339 videocdn_tv-0.2.1/videocdn_tv/type/__init__.py
+-rw-r--r--   0        0        0       82 2023-05-10 19:00:45.033647 videocdn_tv-0.2.1/videocdn_tv/type/direction.py
+-rw-r--r--   0        0        0      156 2023-05-10 19:00:45.040646 videocdn_tv-0.2.1/videocdn_tv/type/field.py
+-rw-r--r--   0        0        0      117 2023-05-10 20:06:49.497524 videocdn_tv-0.2.1/videocdn_tv/type/ordering.py
+-rw-r--r--   0        0        0     2411 1970-01-01 00:00:00.000000 videocdn_tv-0.2.1/PKG-INFO
```

### Comparing `videocdn_tv-0.2.0/pyproject.toml` & `videocdn_tv-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "videocdn_tv"
-version = "0.2.0"
+version = "0.2.1"
 description = "Реализация Api для сервиса VideoCDN.tv"
 authors = ["Your Name <you@example.com>"]
 license = "MIT"
 readme = 'README.md'
 repository = 'https://github.com/odi1n/VideoCDN'
 documentation = "https://github.com/odi1n/VideoCDN/blob/master/README.md"
 keywords = ['videocdn', 'videocdn-tv']
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^1.9.2"
-httpx = "^0.24.0"
+httpx = "^0.23.3"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.1"
 
 [build-system]
```

### Comparing `videocdn_tv-0.2.0/README.md` & `videocdn_tv-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `videocdn_tv-0.2.0/videocdn_tv/link.py` & `videocdn_tv-0.2.1/videocdn_tv/link.py`

 * *Files identical despite different names*

### Comparing `videocdn_tv-0.2.0/videocdn_tv/main.py` & `videocdn_tv-0.2.1/videocdn_tv/main.py`

 * *Files identical despite different names*

### Comparing `videocdn_tv-0.2.0/videocdn_tv/models/api/base_api.py` & `videocdn_tv-0.2.1/videocdn_tv/models/api/base_api.py`

 * *Files identical despite different names*

### Comparing `videocdn_tv-0.2.0/videocdn_tv/models/contents/media.py` & `videocdn_tv-0.2.1/videocdn_tv/models/contents/media.py`

 * *Files identical despite different names*

### Comparing `videocdn_tv-0.2.0/videocdn_tv/models/episodes.py` & `videocdn_tv-0.2.1/videocdn_tv/models/episodes.py`

 * *Files identical despite different names*

### Comparing `videocdn_tv-0.2.0/videocdn_tv/models/response.py` & `videocdn_tv-0.2.1/videocdn_tv/models/response.py`

 * *Files identical despite different names*

### Comparing `videocdn_tv-0.2.0/videocdn_tv/models/seasons.py` & `videocdn_tv-0.2.1/videocdn_tv/models/seasons.py`

 * *Files identical despite different names*

### Comparing `videocdn_tv-0.2.0/videocdn_tv/params/base.py` & `videocdn_tv-0.2.1/videocdn_tv/params/base.py`

 * *Files identical despite different names*

### Comparing `videocdn_tv-0.2.0/videocdn_tv/params/content.py` & `videocdn_tv-0.2.1/videocdn_tv/params/content.py`

 * *Files identical despite different names*

### Comparing `videocdn_tv-0.2.0/videocdn_tv/params/episode.py` & `videocdn_tv-0.2.1/videocdn_tv/params/episode.py`

 * *Files identical despite different names*

### Comparing `videocdn_tv-0.2.0/videocdn_tv/request.py` & `videocdn_tv-0.2.1/videocdn_tv/request.py`

 * *Files identical despite different names*

### Comparing `videocdn_tv-0.2.0/PKG-INFO` & `videocdn_tv-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: videocdn-tv
-Version: 0.2.0
+Version: 0.2.1
 Summary: Реализация Api для сервиса VideoCDN.tv
 Home-page: https://github.com/odi1n/VideoCDN
 License: MIT
 Keywords: videocdn,videocdn-tv
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: pydantic (>=1.9.2,<2.0.0)
 Project-URL: Documentation, https://github.com/odi1n/VideoCDN/blob/master/README.md
 Project-URL: Repository, https://github.com/odi1n/VideoCDN
 Description-Content-Type: text/markdown
 
 # VideoCND - API
```

