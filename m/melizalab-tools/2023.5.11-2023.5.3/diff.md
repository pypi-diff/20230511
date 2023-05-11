# Comparing `tmp/melizalab-tools-2023.5.11.tar.gz` & `tmp/melizalab-tools-2023.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melizalab-tools-2023.5.11.tar", last modified: Thu May 11 13:56:20 2023, max compression
+gzip compressed data, was "melizalab-tools-2023.5.3.tar", last modified: Wed May  3 15:07:50 2023, max compression
```

## Comparing `melizalab-tools-2023.5.11.tar` & `melizalab-tools-2023.5.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-05-11 13:56:20.084080 melizalab-tools-2023.5.11/
--rw-r--r--   0 dmeliza    (503) staff       (20)     1379 2023-05-11 13:56:20.084187 melizalab-tools-2023.5.11/PKG-INFO
--rw-r--r--   0 dmeliza    (503) staff       (20)      852 2023-03-17 16:55:38.000000 melizalab-tools-2023.5.11/README.md
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-05-11 13:56:20.067637 melizalab-tools-2023.5.11/dlab/
--rw-r--r--   0 dmeliza    (503) staff       (20)       24 2022-10-13 22:35:34.000000 melizalab-tools-2023.5.11/dlab/__init__.py
--rw-r--r--   0 dmeliza    (503) staff       (20)      898 2023-03-16 17:12:17.000000 melizalab-tools-2023.5.11/dlab/cache.py
--rw-r--r--   0 dmeliza    (503) staff       (20)      122 2023-05-11 13:56:07.000000 melizalab-tools-2023.5.11/dlab/core.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     1838 2023-03-16 17:04:03.000000 melizalab-tools-2023.5.11/dlab/extracellular.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     6024 2023-03-16 17:04:03.000000 melizalab-tools-2023.5.11/dlab/extract_waveforms.py
--rw-r--r--   0 dmeliza    (503) staff       (20)    18006 2023-05-11 13:56:07.000000 melizalab-tools-2023.5.11/dlab/kilo.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     6483 2023-05-03 15:03:04.000000 melizalab-tools-2023.5.11/dlab/nbank.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     2034 2023-03-10 23:03:29.000000 melizalab-tools-2023.5.11/dlab/plotting.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     5200 2023-05-03 15:00:58.000000 melizalab-tools-2023.5.11/dlab/pprox.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     1790 2023-03-10 23:03:29.000000 melizalab-tools-2023.5.11/dlab/signal.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     4213 2023-05-03 15:00:58.000000 melizalab-tools-2023.5.11/dlab/spikes.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     2055 2023-03-16 17:04:03.000000 melizalab-tools-2023.5.11/dlab/util.py
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-05-11 13:56:20.072773 melizalab-tools-2023.5.11/melizalab_tools.egg-info/
--rw-r--r--   0 dmeliza    (503) staff       (20)     1379 2023-05-11 13:56:19.000000 melizalab-tools-2023.5.11/melizalab_tools.egg-info/PKG-INFO
--rw-r--r--   0 dmeliza    (503) staff       (20)      572 2023-05-11 13:56:20.000000 melizalab-tools-2023.5.11/melizalab_tools.egg-info/SOURCES.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)        1 2023-05-11 13:56:19.000000 melizalab-tools-2023.5.11/melizalab_tools.egg-info/dependency_links.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)       65 2023-05-11 13:56:19.000000 melizalab-tools-2023.5.11/melizalab_tools.egg-info/entry_points.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)        1 2022-10-12 18:42:40.000000 melizalab-tools-2023.5.11/melizalab_tools.egg-info/not-zip-safe
--rw-r--r--   0 dmeliza    (503) staff       (20)      131 2023-05-11 13:56:19.000000 melizalab-tools-2023.5.11/melizalab_tools.egg-info/requires.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)        5 2023-05-11 13:56:20.000000 melizalab-tools-2023.5.11/melizalab_tools.egg-info/top_level.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)      121 2023-02-16 22:14:18.000000 melizalab-tools-2023.5.11/pyproject.toml
--rw-r--r--   0 dmeliza    (503) staff       (20)     1087 2023-05-11 13:56:20.085229 melizalab-tools-2023.5.11/setup.cfg
--rw-r--r--   0 dmeliza    (503) staff       (20)      106 2020-11-05 14:34:56.000000 melizalab-tools-2023.5.11/setup.py
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-05-11 13:56:20.083628 melizalab-tools-2023.5.11/tests/
--rw-r--r--   0 dmeliza    (503) staff       (20)     8722 2023-05-03 15:00:58.000000 melizalab-tools-2023.5.11/tests/test_pprox.py
--rw-r--r--   0 dmeliza    (503) staff       (20)      506 2023-03-10 19:08:55.000000 melizalab-tools-2023.5.11/tests/test_signal.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     1601 2023-04-19 14:41:51.000000 melizalab-tools-2023.5.11/tests/test_spikes.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-05-03 15:07:50.464938 melizalab-tools-2023.5.3/
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1378 2023-05-03 15:07:50.465088 melizalab-tools-2023.5.3/PKG-INFO
+-rw-r--r--   0 dmeliza    (503) staff       (20)      852 2023-03-17 16:55:38.000000 melizalab-tools-2023.5.3/README.md
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-05-03 15:07:50.450790 melizalab-tools-2023.5.3/dlab/
+-rw-r--r--   0 dmeliza    (503) staff       (20)       24 2022-10-13 22:35:34.000000 melizalab-tools-2023.5.3/dlab/__init__.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)      898 2023-03-16 17:12:17.000000 melizalab-tools-2023.5.3/dlab/cache.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)      122 2023-05-03 15:07:13.000000 melizalab-tools-2023.5.3/dlab/core.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1838 2023-03-16 17:04:03.000000 melizalab-tools-2023.5.3/dlab/extracellular.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     6024 2023-03-16 17:04:03.000000 melizalab-tools-2023.5.3/dlab/extract_waveforms.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)    18016 2023-05-03 15:00:58.000000 melizalab-tools-2023.5.3/dlab/kilo.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     6483 2023-05-03 15:03:04.000000 melizalab-tools-2023.5.3/dlab/nbank.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2034 2023-03-10 23:03:29.000000 melizalab-tools-2023.5.3/dlab/plotting.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     5200 2023-05-03 15:00:58.000000 melizalab-tools-2023.5.3/dlab/pprox.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1790 2023-03-10 23:03:29.000000 melizalab-tools-2023.5.3/dlab/signal.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     4213 2023-05-03 15:00:58.000000 melizalab-tools-2023.5.3/dlab/spikes.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2055 2023-03-16 17:04:03.000000 melizalab-tools-2023.5.3/dlab/util.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-05-03 15:07:50.458987 melizalab-tools-2023.5.3/melizalab_tools.egg-info/
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1378 2023-05-03 15:07:50.000000 melizalab-tools-2023.5.3/melizalab_tools.egg-info/PKG-INFO
+-rw-r--r--   0 dmeliza    (503) staff       (20)      572 2023-05-03 15:07:50.000000 melizalab-tools-2023.5.3/melizalab_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        1 2023-05-03 15:07:50.000000 melizalab-tools-2023.5.3/melizalab_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)       65 2023-05-03 15:07:50.000000 melizalab-tools-2023.5.3/melizalab_tools.egg-info/entry_points.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        1 2022-10-12 18:42:40.000000 melizalab-tools-2023.5.3/melizalab_tools.egg-info/not-zip-safe
+-rw-r--r--   0 dmeliza    (503) staff       (20)      131 2023-05-03 15:07:50.000000 melizalab-tools-2023.5.3/melizalab_tools.egg-info/requires.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        5 2023-05-03 15:07:50.000000 melizalab-tools-2023.5.3/melizalab_tools.egg-info/top_level.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)      121 2023-02-16 22:14:18.000000 melizalab-tools-2023.5.3/pyproject.toml
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1087 2023-05-03 15:07:50.467892 melizalab-tools-2023.5.3/setup.cfg
+-rw-r--r--   0 dmeliza    (503) staff       (20)      106 2020-11-05 14:34:56.000000 melizalab-tools-2023.5.3/setup.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-05-03 15:07:50.464156 melizalab-tools-2023.5.3/tests/
+-rw-r--r--   0 dmeliza    (503) staff       (20)     8722 2023-05-03 15:00:58.000000 melizalab-tools-2023.5.3/tests/test_pprox.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)      506 2023-03-10 19:08:55.000000 melizalab-tools-2023.5.3/tests/test_signal.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1601 2023-04-19 14:41:51.000000 melizalab-tools-2023.5.3/tests/test_spikes.py
```

### Comparing `melizalab-tools-2023.5.11/PKG-INFO` & `melizalab-tools-2023.5.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melizalab-tools
-Version: 2023.5.11
+Version: 2023.5.3
 Summary: Meliza lab scripts and modules for auditory neurophysiology
 Home-page: https://github.com/melizalab/melizalab-tools
 Author: Dan Meliza
 Author-email: dan@meliza.org
 Maintainer: Dan Meliza
 Maintainer-email: dan@meliza.org
 License: BSD 3-Clause License
```

### Comparing `melizalab-tools-2023.5.11/README.md` & `melizalab-tools-2023.5.3/README.md`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.5.11/dlab/cache.py` & `melizalab-tools-2023.5.3/dlab/cache.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.5.11/dlab/extracellular.py` & `melizalab-tools-2023.5.3/dlab/extracellular.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.5.11/dlab/extract_waveforms.py` & `melizalab-tools-2023.5.3/dlab/extract_waveforms.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.5.11/dlab/kilo.py` & `melizalab-tools-2023.5.3/dlab/kilo.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         message = row["message"].decode("utf-8")
         m = re_start.match(message)
         if m is not None:
             stim_name = Path(m.group(1)).stem
             yield Stimulus(stim_name, time)
 
 
+@lru_cache(maxsize=None)
 async def stim_duration(session: AsyncClient, stim_name: str) -> float:
     """
     Returns the duration of a stimulus (in s). This can only really be done by
     downloading the stimulus from the registry, because the start/stop times are
     not reliable. We try to speed this up by memoizing the function and caching
     the downloaded files.
 
@@ -216,15 +217,15 @@
     import argparse
     import os
 
     from dlab.core import __version__
     from dlab.extracellular import entry_metadata, iter_entries
     from dlab.util import json_serializable
 
-    version = "2023.05.11"
+    version = "2023.04.26"
 
     p = argparse.ArgumentParser(
         description="group kilosorted spikes into pprox files based on cluster and trial"
     )
     p.add_argument(
         "-v",
         "--version",
@@ -282,18 +283,18 @@
         "--artifact-reject-thresh",
         type=float,
         default=6.0,
         help="threshold for rejecting artifact spikes (max absolute amplitude"
         " more than x times max absolute amplitude of the mean spike)",
     )
     p.add_argument(
-        "--no-waveforms",
+        "--save-waveforms",
         "-W",
         action="store_true",
-        help="if set, do not save representative waveforms from each unit's main channel in an hdf5 file",
+        help="save representative waveforms from each unit's main channel in an hdf5 file",
     )
     p.add_argument(
         "--waveform-pre-peak",
         type=float,
         default=2.0,
         help="samples before the spike to keep (default %(default).1f ms)",
     )
@@ -449,15 +450,15 @@
                 kilosort_n_spikes=clust_info["n_spikes"],
                 entry_metadata=entry_attrs,
                 **resource_info["metadata"],
             )
             if not args.dry_run:
                 with open(outfile, "wt") as ofp:
                     json.dump(clust_trials, ofp, default=json_serializable)
-                if not args.no_waveforms:
+                if args.save_waveforms:
                     outfile = args.output / (outfile.stem + "_spikes.h5")
                     logging.info(
                         "    - waveforms on channel %d -> %s",
                         clust_info["ch"],
                         outfile,
                     )
                     save_waveforms(
```

### Comparing `melizalab-tools-2023.5.11/dlab/nbank.py` & `melizalab-tools-2023.5.3/dlab/nbank.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.5.11/dlab/plotting.py` & `melizalab-tools-2023.5.3/dlab/plotting.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.5.11/dlab/pprox.py` & `melizalab-tools-2023.5.3/dlab/pprox.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.5.11/dlab/signal.py` & `melizalab-tools-2023.5.3/dlab/signal.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.5.11/dlab/spikes.py` & `melizalab-tools-2023.5.3/dlab/spikes.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.5.11/dlab/util.py` & `melizalab-tools-2023.5.3/dlab/util.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.5.11/melizalab_tools.egg-info/PKG-INFO` & `melizalab-tools-2023.5.3/melizalab_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melizalab-tools
-Version: 2023.5.11
+Version: 2023.5.3
 Summary: Meliza lab scripts and modules for auditory neurophysiology
 Home-page: https://github.com/melizalab/melizalab-tools
 Author: Dan Meliza
 Author-email: dan@meliza.org
 Maintainer: Dan Meliza
 Maintainer-email: dan@meliza.org
 License: BSD 3-Clause License
```

### Comparing `melizalab-tools-2023.5.11/melizalab_tools.egg-info/SOURCES.txt` & `melizalab-tools-2023.5.3/melizalab_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.5.11/setup.cfg` & `melizalab-tools-2023.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.5.11/tests/test_pprox.py` & `melizalab-tools-2023.5.3/tests/test_pprox.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.5.11/tests/test_spikes.py` & `melizalab-tools-2023.5.3/tests/test_spikes.py`

 * *Files identical despite different names*

