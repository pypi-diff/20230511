# Comparing `tmp/neon_stt_plugin_nemo-0.0.3a1-py3-none-any.whl.zip` & `tmp/neon_stt_plugin_nemo-0.0.3a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5012 bytes, number of entries: 8
--rw-r--r--  2.0 unx     3586 b- defN 23-May-05 22:21 neon_stt_plugin_nemo/__init__.py
--rw-r--r--  2.0 unx     1634 b- defN 23-May-05 22:21 neon_stt_plugin_nemo-0.0.3a1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      966 b- defN 23-May-05 22:21 neon_stt_plugin_nemo-0.0.3a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 22:21 neon_stt_plugin_nemo-0.0.3a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       73 b- defN 23-May-05 22:21 neon_stt_plugin_nemo-0.0.3a1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 23-May-05 22:21 neon_stt_plugin_nemo-0.0.3a1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-05 22:21 neon_stt_plugin_nemo-0.0.3a1.dist-info/zip-safe
--rw-rw-r--  2.0 unx      763 b- defN 23-May-05 22:21 neon_stt_plugin_nemo-0.0.3a1.dist-info/RECORD
-8 files, 7136 bytes uncompressed, 3640 bytes compressed:  49.0%
+Zip file size: 5126 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     3721 b- defN 23-May-11 19:41 neon_stt_plugin_nemo/__init__.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-May-11 19:41 neon_stt_plugin_nemo-0.0.3a2.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1057 b- defN 23-May-11 19:41 neon_stt_plugin_nemo-0.0.3a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-11 19:41 neon_stt_plugin_nemo-0.0.3a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       73 b- defN 23-May-11 19:41 neon_stt_plugin_nemo-0.0.3a2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-May-11 19:41 neon_stt_plugin_nemo-0.0.3a2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-11 19:41 neon_stt_plugin_nemo-0.0.3a2.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      764 b- defN 23-May-11 19:41 neon_stt_plugin_nemo-0.0.3a2.dist-info/RECORD
+8 files, 7363 bytes uncompressed, 3754 bytes compressed:  49.0%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: neon_stt_plugin_nemo/__init__.py
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.3a1.dist-info/LICENSE.md
+Filename: neon_stt_plugin_nemo-0.0.3a2.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.3a1.dist-info/METADATA
+Filename: neon_stt_plugin_nemo-0.0.3a2.dist-info/METADATA
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.3a1.dist-info/WHEEL
+Filename: neon_stt_plugin_nemo-0.0.3a2.dist-info/WHEEL
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.3a1.dist-info/entry_points.txt
+Filename: neon_stt_plugin_nemo-0.0.3a2.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.3a1.dist-info/top_level.txt
+Filename: neon_stt_plugin_nemo-0.0.3a2.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.3a1.dist-info/zip-safe
+Filename: neon_stt_plugin_nemo-0.0.3a2.dist-info/zip-safe
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.3a1.dist-info/RECORD
+Filename: neon_stt_plugin_nemo-0.0.3a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_stt_plugin_nemo/__init__.py

```diff
@@ -79,9 +79,10 @@
         self.transcriptions = model.stt(audio_buffer, audio.sample_rate)
 
         if not self.transcriptions:
             LOG.info("Transcription is empty")
             self.transcriptions = []
         else:
             LOG.debug("Audio had data")
-
-        return self.transcriptions
+        # TODO: Return a string since we currently only get one result and the
+        #   ovos-stt-server only handles strings here
+        return self.transcriptions[0]
```

## Comparing `neon_stt_plugin_nemo-0.0.3a1.dist-info/LICENSE.md` & `neon_stt_plugin_nemo-0.0.3a2.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_stt_plugin_nemo-0.0.3a1.dist-info/METADATA` & `neon_stt_plugin_nemo-0.0.3a2.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-stt-plugin-nemo
-Version: 0.0.3a1
+Version: 0.0.3a2
 Summary: Nemo STT plugin for Neon
 Home-page: https://github.com/NeonGeckoCom/neon-stt-plugin-nemo
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Keywords: mycroft plugin stt
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,16 @@
 License-File: LICENSE.md
 Requires-Dist: numpy
 Requires-Dist: ovos-plugin-manager (~=0.0.21)
 Requires-Dist: ovos-utils (~=0.0.30)
 Requires-Dist: streaming-stt-nemo (~=0.1)
 Requires-Dist: SpeechRecognition (~=3.8)
 Requires-Dist: mycroft-messagebus-client (~=0.10)
+Provides-Extra: docker
+Requires-Dist: ovos-stt-http-server (>=0.0.2a5) ; extra == 'docker'
 
 # NeonAI Nemo STT Plugin 
 [Mycroft](https://mycroft-ai.gitbook.io/docs/mycroft-technologies/mycroft-core/plugins) compatible
 Neon Nemo STT Plugin Speech-to-Text.
 
 # Configuration:
 ```yaml
```

## Comparing `neon_stt_plugin_nemo-0.0.3a1.dist-info/RECORD` & `neon_stt_plugin_nemo-0.0.3a2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-neon_stt_plugin_nemo/__init__.py,sha256=aOFVNOZfCrycYQRkwZH18LHGzqvlRuDXTQLBFh0nPnQ,3586
-neon_stt_plugin_nemo-0.0.3a1.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_stt_plugin_nemo-0.0.3a1.dist-info/METADATA,sha256=rcaRzPy9FSu-1u-7UyvEShJh16fThqG8wJhAVR5O_OU,966
-neon_stt_plugin_nemo-0.0.3a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_stt_plugin_nemo-0.0.3a1.dist-info/entry_points.txt,sha256=GrVSOmJbddTpT2Z2JC9Xt5vsgpTZRFpyfwQ1E-HZWKQ,73
-neon_stt_plugin_nemo-0.0.3a1.dist-info/top_level.txt,sha256=paHfnP5olm0mLnGfvMW0UuUMQK_0rBDMIWZGpoUEh78,21
-neon_stt_plugin_nemo-0.0.3a1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-neon_stt_plugin_nemo-0.0.3a1.dist-info/RECORD,,
+neon_stt_plugin_nemo/__init__.py,sha256=7d-SZ7W6wmvZ1YdUdrEC-CbmzP8zt-XcHwer0uSZz0o,3721
+neon_stt_plugin_nemo-0.0.3a2.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_stt_plugin_nemo-0.0.3a2.dist-info/METADATA,sha256=Unb_ZAdRy-mC7WWwEQNdMnghlbFWtSzfw7WQCQolu-A,1057
+neon_stt_plugin_nemo-0.0.3a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_stt_plugin_nemo-0.0.3a2.dist-info/entry_points.txt,sha256=GrVSOmJbddTpT2Z2JC9Xt5vsgpTZRFpyfwQ1E-HZWKQ,73
+neon_stt_plugin_nemo-0.0.3a2.dist-info/top_level.txt,sha256=paHfnP5olm0mLnGfvMW0UuUMQK_0rBDMIWZGpoUEh78,21
+neon_stt_plugin_nemo-0.0.3a2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+neon_stt_plugin_nemo-0.0.3a2.dist-info/RECORD,,
```

