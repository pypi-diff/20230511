# Comparing `tmp/audioviz-0.2.0.tar.gz` & `tmp/audioviz-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioviz-0.2.0.tar", last modified: Wed May 10 10:19:20 2023, max compression
+gzip compressed data, was "audioviz-0.2.1.tar", last modified: Thu May 11 03:30:06 2023, max compression
```

## Comparing `audioviz-0.2.0.tar` & `audioviz-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-10 10:19:20.492996 audioviz-0.2.0/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1933 2023-05-10 10:19:20.492996 audioviz-0.2.0/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1208 2023-05-07 03:19:43.000000 audioviz-0.2.0/README.md
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-10 10:19:20.492996 audioviz-0.2.0/audioviz/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8548 2023-04-27 03:14:29.000000 audioviz-0.2.0/audioviz/BeatAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8706 2023-05-10 10:18:06.000000 audioviz-0.2.0/audioviz/ChordAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2679 2023-04-30 07:22:36.000000 audioviz-0.2.0/audioviz/GeneralAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2165 2023-05-09 06:50:18.000000 audioviz-0.2.0/audioviz/Panel.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.2.0/audioviz/PitchAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.2.0/audioviz/StructureAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.2.0/audioviz/TimbreAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      304 2023-05-07 07:11:37.000000 audioviz-0.2.0/audioviz/__init__.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1591 2023-04-27 03:14:12.000000 audioviz-0.2.0/audioviz/colabInterface.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1094 2023-05-07 03:14:17.000000 audioviz-0.2.0/audioviz/utils.py
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-10 10:19:20.492996 audioviz-0.2.0/audioviz.egg-info/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1933 2023-05-10 10:19:20.000000 audioviz-0.2.0/audioviz.egg-info/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      464 2023-05-10 10:19:20.000000 audioviz-0.2.0/audioviz.egg-info/SOURCES.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-05-10 10:19:20.000000 audioviz-0.2.0/audioviz.egg-info/dependency_links.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.2.0/audioviz.egg-info/not-zip-safe
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       62 2023-05-10 10:19:20.000000 audioviz-0.2.0/audioviz.egg-info/requires.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-05-10 10:19:20.000000 audioviz-0.2.0/audioviz.egg-info/top_level.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-05-10 10:19:20.492996 audioviz-0.2.0/setup.cfg
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1324 2023-05-10 10:16:12.000000 audioviz-0.2.0/setup.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-11 03:30:06.867854 audioviz-0.2.1/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1933 2023-05-11 03:30:06.867854 audioviz-0.2.1/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1208 2023-05-07 03:19:43.000000 audioviz-0.2.1/README.md
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-11 03:30:06.867854 audioviz-0.2.1/audioviz/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8574 2023-05-11 03:27:58.000000 audioviz-0.2.1/audioviz/BeatAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8706 2023-05-10 10:18:06.000000 audioviz-0.2.1/audioviz/ChordAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2679 2023-04-30 07:22:36.000000 audioviz-0.2.1/audioviz/GeneralAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2165 2023-05-09 06:50:18.000000 audioviz-0.2.1/audioviz/Panel.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.2.1/audioviz/PitchAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.2.1/audioviz/StructureAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.2.1/audioviz/TimbreAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      304 2023-05-07 07:11:37.000000 audioviz-0.2.1/audioviz/__init__.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1593 2023-05-11 03:27:06.000000 audioviz-0.2.1/audioviz/colabInterface.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1094 2023-05-07 03:14:17.000000 audioviz-0.2.1/audioviz/utils.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-11 03:30:06.867854 audioviz-0.2.1/audioviz.egg-info/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1933 2023-05-11 03:30:06.000000 audioviz-0.2.1/audioviz.egg-info/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      464 2023-05-11 03:30:06.000000 audioviz-0.2.1/audioviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-05-11 03:30:06.000000 audioviz-0.2.1/audioviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.2.1/audioviz.egg-info/not-zip-safe
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       62 2023-05-11 03:30:06.000000 audioviz-0.2.1/audioviz.egg-info/requires.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-05-11 03:30:06.000000 audioviz-0.2.1/audioviz.egg-info/top_level.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-05-11 03:30:06.867854 audioviz-0.2.1/setup.cfg
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1354 2023-05-11 03:29:58.000000 audioviz-0.2.1/setup.py
```

### Comparing `audioviz-0.2.0/PKG-INFO` & `audioviz-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.2.0
+Version: 0.2.1
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
 Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `audioviz-0.2.0/README.md` & `audioviz-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `audioviz-0.2.0/audioviz/BeatAnalysis.py` & `audioviz-0.2.1/audioviz/BeatAnalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     # Save onset-to-time info
     result = np.round(times[onset_frames].T, 3)
     save_and_downloader('beats.csv', np.array(['Time']), result)
 
     # Save the processed audio
     y_onset_clicks = librosa.clicks(frames=onset_frames, sr=sr, length=len(y))
-    ipd.Audio(y_onset_clicks, rate=sr)
+    ipd.display(ipd.Audio(y_onset_clicks, rate=sr))
     audio_save_and_downloader('onset_click.wav', y_onset_clicks, sr)
 
 
 def plot_onset_strength(y: npt.ArrayLike, sr:int, standard: bool = True, custom_mel: bool = False, cqt: bool = False) :
 
     '''
     To plot the onset strength of the input signal with time-axis
@@ -118,15 +118,15 @@
 
     # Save beat-to-time info
     result = np.round(times[beats].T, 3)
     save_and_downloader('beats.csv', np.array(['Time']), result)
 
     # Save processed audio
     y_beats = librosa.clicks(frames=beats, sr=sr, length=len(y))
-    ipd.Audio(y_beats, rate=sr)
+    ipd.display(ipd.Audio(y_beats, rate=sr))
     audio_save_and_downloader('beat_click.wav', y_beats, sr)
 
 
 def predominant_local_pulses(y: npt.ArrayLike, sr:int) -> None :
 
     '''
     To plot the predominant local pulses of the input signal with time-axis
```

### Comparing `audioviz-0.2.0/audioviz/ChordAnalysis.py` & `audioviz-0.2.1/audioviz/ChordAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.2.0/audioviz/GeneralAnalysis.py` & `audioviz-0.2.1/audioviz/GeneralAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.2.0/audioviz/Panel.py` & `audioviz-0.2.1/audioviz/Panel.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.2.0/audioviz/PitchAnalysis.py` & `audioviz-0.2.1/audioviz/PitchAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.2.0/audioviz/StructureAnalysis.py` & `audioviz-0.2.1/audioviz/StructureAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.2.0/audioviz/TimbreAnalysis.py` & `audioviz-0.2.1/audioviz/TimbreAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.2.0/audioviz/colabInterface.py` & `audioviz-0.2.1/audioviz/colabInterface.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     buttonDownload = widgets.Button(description = '.csv Download & Save')
     buttonCancel =  widgets.Button(description = 'Cancel') 
     buttonDownload.on_click(functools.partial(core_download_and_save, filename, header_of_file, result_array))
     buttonCancel.on_click(noMsg)
 
     display(buttonDownload)
-    display(buttonCancel)
+    #display(buttonCancel)
 
 def core_audio_download_and_save(filename: str, audio_array: npt.ArrayLike, sr: int, arg) :
     
     sf.write(filename, audio_array, sr, subtype='PCM_24')
     files.download(filename)
 
 
@@ -43,8 +43,8 @@
 
     buttonDownload = widgets.Button(description = 'Audio Download & Save')
     buttonCancel =  widgets.Button(description = 'Cancel') 
     buttonDownload.on_click(functools.partial(core_audio_download_and_save, filename, audio_array, sr))
     buttonCancel.on_click(noMsg)
 
     display(buttonDownload)
-    display(buttonCancel)
+    #display(buttonCancel)
```

### Comparing `audioviz-0.2.0/audioviz/utils.py` & `audioviz-0.2.1/audioviz/utils.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.2.0/audioviz.egg-info/PKG-INFO` & `audioviz-0.2.1/audioviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.2.0
+Version: 0.2.1
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
 Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `audioviz-0.2.0/setup.py` & `audioviz-0.2.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='audioviz',
     packages=['audioviz'],
-    version='0.2.0',
+    version='0.2.1',
     
     description='An user-friendly music information retrieval tools interfacing with Google Colab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     
     url='https://github.com/TrangDuLam/audioviz',
     author='ayTrang',
@@ -24,15 +24,15 @@
                         "pandas",
                         "scipy", 
                         "librosa", 
                         "libfmp", 
                         "plotly",
                         "soundfile",
                         ],
-
+    include_package_data=True,
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'Topic :: Multimedia :: Sound/Audio :: Analysis',
         'Topic :: Education',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.9',
```

