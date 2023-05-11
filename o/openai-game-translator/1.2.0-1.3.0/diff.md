# Comparing `tmp/openai-game-translator-1.2.0.tar.gz` & `tmp/openai-game-translator-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-game-translator-1.2.0.tar", last modified: Fri May  5 04:13:29 2023, max compression
+gzip compressed data, was "openai-game-translator-1.3.0.tar", last modified: Thu May 11 19:41:58 2023, max compression
```

## Comparing `openai-game-translator-1.2.0.tar` & `openai-game-translator-1.3.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-05 04:13:29.626423 openai-game-translator-1.2.0/
--rw-r--r--   0 arika      (501) staff       (20)    11357 2023-03-21 20:15:17.000000 openai-game-translator-1.2.0/LICENSE
--rw-r--r--   0 arika      (501) staff       (20)    17867 2023-05-05 04:13:29.626189 openai-game-translator-1.2.0/PKG-INFO
--rw-r--r--   0 arika      (501) staff       (20)     4263 2023-05-05 01:27:26.000000 openai-game-translator-1.2.0/README.md
-drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-05 04:13:29.620702 openai-game-translator-1.2.0/game_translator/
--rw-r--r--   0 arika      (501) staff       (20)      295 2023-04-07 04:06:17.000000 openai-game-translator-1.2.0/game_translator/__init__.py
--rw-r--r--   0 arika      (501) staff       (20)       42 2023-04-07 04:06:17.000000 openai-game-translator-1.2.0/game_translator/__main__.py
--rw-r--r--   0 arika      (501) staff       (20)       22 2023-05-05 03:44:24.000000 openai-game-translator-1.2.0/game_translator/_version.py
-drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-05 04:13:29.620991 openai-game-translator-1.2.0/game_translator/audio/
--rw-r--r--   0 arika      (501) staff       (20)       29 2023-04-07 04:06:17.000000 openai-game-translator-1.2.0/game_translator/audio/__init__.py
--rw-r--r--   0 arika      (501) staff       (20)     3112 2023-05-04 18:51:36.000000 openai-game-translator-1.2.0/game_translator/audio/record.py
-drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-05 04:13:29.621552 openai-game-translator-1.2.0/game_translator/aws_streaming_transcription/
--rw-r--r--   0 arika      (501) staff       (20)        0 2023-04-05 01:22:22.000000 openai-game-translator-1.2.0/game_translator/aws_streaming_transcription/__init__.py
--rw-r--r--   0 arika      (501) staff       (20)     2406 2023-05-05 01:25:40.000000 openai-game-translator-1.2.0/game_translator/aws_streaming_transcription/live_stream.py
--rw-r--r--   0 arika      (501) staff       (20)     2811 2023-05-05 01:25:40.000000 openai-game-translator-1.2.0/game_translator/aws_streaming_transcription/prerecorded_stream.py
--rw-r--r--   0 arika      (501) staff       (20)     1717 2023-05-05 01:25:40.000000 openai-game-translator-1.2.0/game_translator/aws_streaming_transcription/settings.py
--rw-r--r--   0 arika      (501) staff       (20)     9775 2023-05-05 04:08:39.000000 openai-game-translator-1.2.0/game_translator/game_translator.py
-drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-05 04:13:29.621861 openai-game-translator-1.2.0/game_translator/openai_translation/
--rw-r--r--   0 arika      (501) staff       (20)       37 2023-04-07 04:06:17.000000 openai-game-translator-1.2.0/game_translator/openai_translation/__init__.py
--rw-r--r--   0 arika      (501) staff       (20)      681 2023-05-03 19:14:25.000000 openai-game-translator-1.2.0/game_translator/openai_translation/chat.py
-drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-05 04:13:29.622320 openai-game-translator-1.2.0/game_translator/xunfei_speed_transcription/
--rw-r--r--   0 arika      (501) staff       (20)       70 2023-04-05 01:22:22.000000 openai-game-translator-1.2.0/game_translator/xunfei_speed_transcription/__init__.py
--rw-r--r--   0 arika      (501) staff       (20)     7697 2023-05-03 21:28:32.000000 openai-game-translator-1.2.0/game_translator/xunfei_speed_transcription/ost_fast.py
--rw-r--r--   0 arika      (501) staff       (20)     7608 2023-05-03 19:13:14.000000 openai-game-translator-1.2.0/game_translator/xunfei_speed_transcription/seve_file.py
-drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-05 04:13:29.623472 openai-game-translator-1.2.0/openai_game_translator.egg-info/
--rw-r--r--   0 arika      (501) staff       (20)    17867 2023-05-05 04:13:29.000000 openai-game-translator-1.2.0/openai_game_translator.egg-info/PKG-INFO
--rw-r--r--   0 arika      (501) staff       (20)     1153 2023-05-05 04:13:29.000000 openai-game-translator-1.2.0/openai_game_translator.egg-info/SOURCES.txt
--rw-r--r--   0 arika      (501) staff       (20)        1 2023-05-05 04:13:29.000000 openai-game-translator-1.2.0/openai_game_translator.egg-info/dependency_links.txt
--rw-r--r--   0 arika      (501) staff       (20)       67 2023-05-05 04:13:29.000000 openai-game-translator-1.2.0/openai_game_translator.egg-info/entry_points.txt
--rw-r--r--   0 arika      (501) staff       (20)      242 2023-05-05 04:13:29.000000 openai-game-translator-1.2.0/openai_game_translator.egg-info/requires.txt
--rw-r--r--   0 arika      (501) staff       (20)       16 2023-05-05 04:13:29.000000 openai-game-translator-1.2.0/openai_game_translator.egg-info/top_level.txt
--rw-r--r--   0 arika      (501) staff       (20)     1216 2023-05-05 03:44:24.000000 openai-game-translator-1.2.0/pyproject.toml
--rw-r--r--   0 arika      (501) staff       (20)       38 2023-05-05 04:13:29.626490 openai-game-translator-1.2.0/setup.cfg
--rw-r--r--   0 arika      (501) staff       (20)       38 2023-04-07 04:06:17.000000 openai-game-translator-1.2.0/setup.py
-drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-05 04:13:29.625755 openai-game-translator-1.2.0/tests/
--rw-r--r--   0 arika      (501) staff       (20)     2047 2023-05-03 18:29:32.000000 openai-game-translator-1.2.0/tests/test_all.py
--rw-r--r--   0 arika      (501) staff       (20)     1899 2023-05-04 21:43:02.000000 openai-game-translator-1.2.0/tests/test_aws_live.py
--rw-r--r--   0 arika      (501) staff       (20)     1038 2023-05-04 21:47:09.000000 openai-game-translator-1.2.0/tests/test_aws_pre.py
--rw-r--r--   0 arika      (501) staff       (20)     2499 2023-05-04 20:00:09.000000 openai-game-translator-1.2.0/tests/test_game_translator.py
--rw-r--r--   0 arika      (501) staff       (20)     1041 2023-05-04 21:51:09.000000 openai-game-translator-1.2.0/tests/test_openai.py
--rw-r--r--   0 arika      (501) staff       (20)     1037 2023-05-04 20:02:02.000000 openai-game-translator-1.2.0/tests/test_record.py
--rw-r--r--   0 arika      (501) staff       (20)     1130 2023-05-04 21:51:33.000000 openai-game-translator-1.2.0/tests/test_xunfei.py
+drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-11 19:41:58.894536 openai-game-translator-1.3.0/
+-rw-r--r--   0 arika      (501) staff       (20)    11357 2023-03-21 20:15:17.000000 openai-game-translator-1.3.0/LICENSE
+-rw-r--r--   0 arika      (501) staff       (20)    19152 2023-05-11 19:41:58.894327 openai-game-translator-1.3.0/PKG-INFO
+-rw-r--r--   0 arika      (501) staff       (20)     5548 2023-05-11 19:25:47.000000 openai-game-translator-1.3.0/README.md
+drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-11 19:41:58.889496 openai-game-translator-1.3.0/game_translator/
+-rw-r--r--   0 arika      (501) staff       (20)      295 2023-04-07 04:06:17.000000 openai-game-translator-1.3.0/game_translator/__init__.py
+-rw-r--r--   0 arika      (501) staff       (20)       42 2023-04-07 04:06:17.000000 openai-game-translator-1.3.0/game_translator/__main__.py
+-rw-r--r--   0 arika      (501) staff       (20)       22 2023-05-11 19:41:39.000000 openai-game-translator-1.3.0/game_translator/_version.py
+drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-11 19:41:58.889791 openai-game-translator-1.3.0/game_translator/audio/
+-rw-r--r--   0 arika      (501) staff       (20)       29 2023-04-07 04:06:17.000000 openai-game-translator-1.3.0/game_translator/audio/__init__.py
+-rw-r--r--   0 arika      (501) staff       (20)     3112 2023-05-05 04:19:14.000000 openai-game-translator-1.3.0/game_translator/audio/record.py
+drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-11 19:41:58.890823 openai-game-translator-1.3.0/game_translator/aws_streaming_transcription/
+-rw-r--r--   0 arika      (501) staff       (20)        0 2023-04-05 01:22:22.000000 openai-game-translator-1.3.0/game_translator/aws_streaming_transcription/__init__.py
+-rw-r--r--   0 arika      (501) staff       (20)     2406 2023-05-05 04:19:14.000000 openai-game-translator-1.3.0/game_translator/aws_streaming_transcription/live_stream.py
+-rw-r--r--   0 arika      (501) staff       (20)     2811 2023-05-05 04:19:14.000000 openai-game-translator-1.3.0/game_translator/aws_streaming_transcription/prerecorded_stream.py
+-rw-r--r--   0 arika      (501) staff       (20)     1717 2023-05-05 04:19:14.000000 openai-game-translator-1.3.0/game_translator/aws_streaming_transcription/settings.py
+-rw-r--r--   0 arika      (501) staff       (20)     9775 2023-05-05 04:19:14.000000 openai-game-translator-1.3.0/game_translator/game_translator.py
+drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-11 19:41:58.891217 openai-game-translator-1.3.0/game_translator/openai_translation/
+-rw-r--r--   0 arika      (501) staff       (20)       37 2023-04-07 04:06:17.000000 openai-game-translator-1.3.0/game_translator/openai_translation/__init__.py
+-rw-r--r--   0 arika      (501) staff       (20)      681 2023-05-05 04:19:14.000000 openai-game-translator-1.3.0/game_translator/openai_translation/chat.py
+drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-11 19:41:58.891759 openai-game-translator-1.3.0/game_translator/xunfei_speed_transcription/
+-rw-r--r--   0 arika      (501) staff       (20)       70 2023-04-05 01:22:22.000000 openai-game-translator-1.3.0/game_translator/xunfei_speed_transcription/__init__.py
+-rw-r--r--   0 arika      (501) staff       (20)     7697 2023-05-05 04:19:14.000000 openai-game-translator-1.3.0/game_translator/xunfei_speed_transcription/ost_fast.py
+-rw-r--r--   0 arika      (501) staff       (20)     7608 2023-05-05 04:19:14.000000 openai-game-translator-1.3.0/game_translator/xunfei_speed_transcription/seve_file.py
+drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-11 19:41:58.892754 openai-game-translator-1.3.0/openai_game_translator.egg-info/
+-rw-r--r--   0 arika      (501) staff       (20)    19152 2023-05-11 19:41:58.000000 openai-game-translator-1.3.0/openai_game_translator.egg-info/PKG-INFO
+-rw-r--r--   0 arika      (501) staff       (20)     1153 2023-05-11 19:41:58.000000 openai-game-translator-1.3.0/openai_game_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 arika      (501) staff       (20)        1 2023-05-11 19:41:58.000000 openai-game-translator-1.3.0/openai_game_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 arika      (501) staff       (20)       67 2023-05-11 19:41:58.000000 openai-game-translator-1.3.0/openai_game_translator.egg-info/entry_points.txt
+-rw-r--r--   0 arika      (501) staff       (20)      242 2023-05-11 19:41:58.000000 openai-game-translator-1.3.0/openai_game_translator.egg-info/requires.txt
+-rw-r--r--   0 arika      (501) staff       (20)       16 2023-05-11 19:41:58.000000 openai-game-translator-1.3.0/openai_game_translator.egg-info/top_level.txt
+-rw-r--r--   0 arika      (501) staff       (20)     1216 2023-05-11 19:41:39.000000 openai-game-translator-1.3.0/pyproject.toml
+-rw-r--r--   0 arika      (501) staff       (20)       38 2023-05-11 19:41:58.894596 openai-game-translator-1.3.0/setup.cfg
+-rw-r--r--   0 arika      (501) staff       (20)       38 2023-04-07 04:06:17.000000 openai-game-translator-1.3.0/setup.py
+drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-11 19:41:58.894023 openai-game-translator-1.3.0/tests/
+-rw-r--r--   0 arika      (501) staff       (20)     2047 2023-05-05 04:19:14.000000 openai-game-translator-1.3.0/tests/test_all.py
+-rw-r--r--   0 arika      (501) staff       (20)     1899 2023-05-05 04:19:14.000000 openai-game-translator-1.3.0/tests/test_aws_live.py
+-rw-r--r--   0 arika      (501) staff       (20)     1038 2023-05-05 04:19:14.000000 openai-game-translator-1.3.0/tests/test_aws_pre.py
+-rw-r--r--   0 arika      (501) staff       (20)     2499 2023-05-05 04:19:14.000000 openai-game-translator-1.3.0/tests/test_game_translator.py
+-rw-r--r--   0 arika      (501) staff       (20)     1041 2023-05-05 04:19:14.000000 openai-game-translator-1.3.0/tests/test_openai.py
+-rw-r--r--   0 arika      (501) staff       (20)     1037 2023-05-05 04:19:14.000000 openai-game-translator-1.3.0/tests/test_record.py
+-rw-r--r--   0 arika      (501) staff       (20)     1130 2023-05-05 04:19:14.000000 openai-game-translator-1.3.0/tests/test_xunfei.py
```

### Comparing `openai-game-translator-1.2.0/LICENSE` & `openai-game-translator-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai-game-translator-1.2.0/PKG-INFO` & `openai-game-translator-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-game-translator
-Version: 1.2.0
+Version: 1.3.0
 Summary: an openai based game audio translator
 Author-email: Yuhan Xia <yx2729@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -275,11 +275,51 @@
 from game_translator import gameTranslator
 
 openai.api_key = "<openai_key>"
 translator = gameTranslator("aws_live", input_language="chinese", output_language="english")
 translator.openai_translation()
 ```
 
+## Examples
+### Shell xunfei prerecorded example
+```shell
+translate --openai_key <openai_key>  -o english -i chinese xunfei --xunfei_appid <xunfei_appid> --xunfei_apikey  <xunfei_apikey> --xunfei_apisecret <xunfei_apisecret> --file audio_sample_little.wav --pre_recorded
+```
+```shell
+****************************************
+Transcription model : xunfei
+Using prerecorded audio file : audio_sample_little.wav
+Input  language : chinese
+Output language : english
+****************************************
+transcription success...
+科大讯飞是中国最大的智能语音技术提供商。
+translation success...
+iFlytek is the largest intelligent voice technology provider in China.
+Elapsed time: 3.813 seconds
+```
+### Script AWS live example
+```python
+translator = gameTranslator("aws_live")
+translator.openai_translation()
+```
+```shell
+****************************************
+Transcription model : aws_live
+Using prerecorded audio file : None
+Input  language : chinese
+Output language : english
+****************************************
+start detecting audio...
+current rms: ##                  |
+detecting finished...
+transcription success...
+明天的期末考试我能考多少
+translation success...
+How much can I score on tomorrow's final exam?
+Elapsed time: 9.155 seconds
+```
+
 ## Contributing
 See more at [CONTRIBUTING.md](./CONTRIBUTING.md)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openai-game-translator-1.2.0/README.md` & `openai-game-translator-1.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -57,11 +57,51 @@
 from game_translator import gameTranslator
 
 openai.api_key = "<openai_key>"
 translator = gameTranslator("aws_live", input_language="chinese", output_language="english")
 translator.openai_translation()
 ```
 
+## Examples
+### Shell xunfei prerecorded example
+```shell
+translate --openai_key <openai_key>  -o english -i chinese xunfei --xunfei_appid <xunfei_appid> --xunfei_apikey  <xunfei_apikey> --xunfei_apisecret <xunfei_apisecret> --file audio_sample_little.wav --pre_recorded
+```
+```shell
+****************************************
+Transcription model : xunfei
+Using prerecorded audio file : audio_sample_little.wav
+Input  language : chinese
+Output language : english
+****************************************
+transcription success...
+科大讯飞是中国最大的智能语音技术提供商。
+translation success...
+iFlytek is the largest intelligent voice technology provider in China.
+Elapsed time: 3.813 seconds
+```
+### Script AWS live example
+```python
+translator = gameTranslator("aws_live")
+translator.openai_translation()
+```
+```shell
+****************************************
+Transcription model : aws_live
+Using prerecorded audio file : None
+Input  language : chinese
+Output language : english
+****************************************
+start detecting audio...
+current rms: ##                  |
+detecting finished...
+transcription success...
+明天的期末考试我能考多少
+translation success...
+How much can I score on tomorrow's final exam?
+Elapsed time: 9.155 seconds
+```
+
 ## Contributing
 See more at [CONTRIBUTING.md](./CONTRIBUTING.md)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openai-game-translator-1.2.0/game_translator/audio/record.py` & `openai-game-translator-1.3.0/game_translator/audio/record.py`

 * *Files identical despite different names*

### Comparing `openai-game-translator-1.2.0/game_translator/aws_streaming_transcription/live_stream.py` & `openai-game-translator-1.3.0/game_translator/aws_streaming_transcription/live_stream.py`

 * *Files identical despite different names*

### Comparing `openai-game-translator-1.2.0/game_translator/aws_streaming_transcription/prerecorded_stream.py` & `openai-game-translator-1.3.0/game_translator/aws_streaming_transcription/prerecorded_stream.py`

 * *Files identical despite different names*

### Comparing `openai-game-translator-1.2.0/game_translator/aws_streaming_transcription/settings.py` & `openai-game-translator-1.3.0/game_translator/aws_streaming_transcription/settings.py`

 * *Files identical despite different names*

### Comparing `openai-game-translator-1.2.0/game_translator/game_translator.py` & `openai-game-translator-1.3.0/game_translator/game_translator.py`

 * *Files identical despite different names*

### Comparing `openai-game-translator-1.2.0/game_translator/openai_translation/chat.py` & `openai-game-translator-1.3.0/game_translator/openai_translation/chat.py`

 * *Files identical despite different names*

### Comparing `openai-game-translator-1.2.0/game_translator/xunfei_speed_transcription/ost_fast.py` & `openai-game-translator-1.3.0/game_translator/xunfei_speed_transcription/ost_fast.py`

 * *Files identical despite different names*

### Comparing `openai-game-translator-1.2.0/game_translator/xunfei_speed_transcription/seve_file.py` & `openai-game-translator-1.3.0/game_translator/xunfei_speed_transcription/seve_file.py`

 * *Files identical despite different names*

### Comparing `openai-game-translator-1.2.0/openai_game_translator.egg-info/PKG-INFO` & `openai-game-translator-1.3.0/openai_game_translator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-game-translator
-Version: 1.2.0
+Version: 1.3.0
 Summary: an openai based game audio translator
 Author-email: Yuhan Xia <yx2729@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -275,11 +275,51 @@
 from game_translator import gameTranslator
 
 openai.api_key = "<openai_key>"
 translator = gameTranslator("aws_live", input_language="chinese", output_language="english")
 translator.openai_translation()
 ```
 
+## Examples
+### Shell xunfei prerecorded example
+```shell
+translate --openai_key <openai_key>  -o english -i chinese xunfei --xunfei_appid <xunfei_appid> --xunfei_apikey  <xunfei_apikey> --xunfei_apisecret <xunfei_apisecret> --file audio_sample_little.wav --pre_recorded
+```
+```shell
+****************************************
+Transcription model : xunfei
+Using prerecorded audio file : audio_sample_little.wav
+Input  language : chinese
+Output language : english
+****************************************
+transcription success...
+科大讯飞是中国最大的智能语音技术提供商。
+translation success...
+iFlytek is the largest intelligent voice technology provider in China.
+Elapsed time: 3.813 seconds
+```
+### Script AWS live example
+```python
+translator = gameTranslator("aws_live")
+translator.openai_translation()
+```
+```shell
+****************************************
+Transcription model : aws_live
+Using prerecorded audio file : None
+Input  language : chinese
+Output language : english
+****************************************
+start detecting audio...
+current rms: ##                  |
+detecting finished...
+transcription success...
+明天的期末考试我能考多少
+translation success...
+How much can I score on tomorrow's final exam?
+Elapsed time: 9.155 seconds
+```
+
 ## Contributing
 See more at [CONTRIBUTING.md](./CONTRIBUTING.md)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openai-game-translator-1.2.0/openai_game_translator.egg-info/SOURCES.txt` & `openai-game-translator-1.3.0/openai_game_translator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai-game-translator-1.2.0/pyproject.toml` & `openai-game-translator-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openai-game-translator"
-version = "1.2.0"
+version = "1.3.0"
 authors = [
   { name="Yuhan Xia", email="yx2729@columbia.edu" },
 ]
 description = "an openai based game audio translator"
 readme = "README.md"
 requires-python = ">=3.9, <3.11"
 classifiers = [
```

### Comparing `openai-game-translator-1.2.0/tests/test_all.py` & `openai-game-translator-1.3.0/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `openai-game-translator-1.2.0/tests/test_aws_live.py` & `openai-game-translator-1.3.0/tests/test_aws_live.py`

 * *Files identical despite different names*

### Comparing `openai-game-translator-1.2.0/tests/test_aws_pre.py` & `openai-game-translator-1.3.0/tests/test_aws_pre.py`

 * *Files identical despite different names*

### Comparing `openai-game-translator-1.2.0/tests/test_game_translator.py` & `openai-game-translator-1.3.0/tests/test_game_translator.py`

 * *Files identical despite different names*

### Comparing `openai-game-translator-1.2.0/tests/test_openai.py` & `openai-game-translator-1.3.0/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `openai-game-translator-1.2.0/tests/test_record.py` & `openai-game-translator-1.3.0/tests/test_record.py`

 * *Files identical despite different names*

### Comparing `openai-game-translator-1.2.0/tests/test_xunfei.py` & `openai-game-translator-1.3.0/tests/test_xunfei.py`

 * *Files identical despite different names*

