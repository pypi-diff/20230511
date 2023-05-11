# Comparing `tmp/seas-0.0.4.tar.gz` & `tmp/seas-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seas-0.0.4.tar", last modified: Fri Apr 28 00:59:05 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `seas-0.0.4.tar` & `seas-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,62 @@
-drwxrwxr-x   0 sydney    (1000) sydney    (1000)        0 2023-04-28 00:59:05.101721 seas-0.0.4/
--rw-rw-r--   0 sydney    (1000) sydney    (1000)     1074 2023-04-16 18:10:49.000000 seas-0.0.4/LICENSE
--rw-rw-r--   0 sydney    (1000) sydney    (1000)      539 2023-04-28 00:59:05.101721 seas-0.0.4/PKG-INFO
--rw-rw-r--   0 sydney    (1000) sydney    (1000)     3017 2023-04-16 18:10:49.000000 seas-0.0.4/README.md
-drwxrwxr-x   0 sydney    (1000) sydney    (1000)        0 2023-04-28 00:59:05.097721 seas-0.0.4/seas/
--rw-rw-r--   0 sydney    (1000) sydney    (1000)      544 2023-04-28 00:54:23.000000 seas-0.0.4/seas/__init__.py
--rw-rw-r--   0 sydney    (1000) sydney    (1000)     5651 2023-04-19 17:20:49.000000 seas-0.0.4/seas/colormaps.py
--rw-rw-r--   0 sydney    (1000) sydney    (1000)     5862 2023-04-16 18:45:28.000000 seas-0.0.4/seas/defaults.py
--rw-rw-r--   0 sydney    (1000) sydney    (1000)    24292 2023-04-28 00:54:50.000000 seas-0.0.4/seas/domains.py
--rw-rw-r--   0 sydney    (1000) sydney    (1000)    18320 2023-04-16 19:58:37.000000 seas-0.0.4/seas/experiment.py
--rw-rw-r--   0 sydney    (1000) sydney    (1000)    12195 2023-04-16 19:37:25.000000 seas-0.0.4/seas/filemanager.py
--rw-rw-r--   0 sydney    (1000) sydney    (1000)    69392 2023-04-28 00:48:56.000000 seas-0.0.4/seas/gui.py
--rw-rw-r--   0 sydney    (1000) sydney    (1000)    17569 2023-04-28 00:54:23.000000 seas-0.0.4/seas/hdf5manager.py
--rw-rw-r--   0 sydney    (1000) sydney    (1000)    26572 2023-04-17 02:36:45.000000 seas-0.0.4/seas/ica.py
--rw-rw-r--   0 sydney    (1000) sydney    (1000)    10425 2023-04-17 03:51:43.000000 seas-0.0.4/seas/rois.py
--rw-rw-r--   0 sydney    (1000) sydney    (1000)    14195 2023-04-28 00:54:23.000000 seas-0.0.4/seas/signalanalysis.py
--rw-rw-r--   0 sydney    (1000) sydney    (1000)    38898 2023-04-17 04:11:37.000000 seas-0.0.4/seas/video.py
--rw-rw-r--   0 sydney    (1000) sydney    (1000)    36496 2023-04-17 03:28:33.000000 seas-0.0.4/seas/waveletAnalysis.py
--rw-rw-r--   0 sydney    (1000) sydney    (1000)    17275 2023-04-28 00:54:24.000000 seas-0.0.4/seas/waveletFunctions.py
-drwxrwxr-x   0 sydney    (1000) sydney    (1000)        0 2023-04-28 00:59:05.097721 seas-0.0.4/seas.egg-info/
--rw-rw-r--   0 sydney    (1000) sydney    (1000)      539 2023-04-28 00:59:05.000000 seas-0.0.4/seas.egg-info/PKG-INFO
--rw-rw-r--   0 sydney    (1000) sydney    (1000)      538 2023-04-28 00:59:05.000000 seas-0.0.4/seas.egg-info/SOURCES.txt
--rw-rw-r--   0 sydney    (1000) sydney    (1000)        1 2023-04-28 00:59:05.000000 seas-0.0.4/seas.egg-info/dependency_links.txt
--rw-rw-r--   0 sydney    (1000) sydney    (1000)       74 2023-04-28 00:59:05.000000 seas-0.0.4/seas.egg-info/requires.txt
--rw-rw-r--   0 sydney    (1000) sydney    (1000)       11 2023-04-28 00:59:05.000000 seas-0.0.4/seas.egg-info/top_level.txt
--rw-rw-r--   0 sydney    (1000) sydney    (1000)       79 2023-04-28 00:59:05.101721 seas-0.0.4/setup.cfg
--rw-rw-r--   0 sydney    (1000) sydney    (1000)      907 2023-04-28 00:56:33.000000 seas-0.0.4/setup.py
-drwxrwxr-x   0 sydney    (1000) sydney    (1000)        0 2023-04-28 00:59:05.097721 seas-0.0.4/tests/
--rw-rw-r--   0 sydney    (1000) sydney    (1000)        1 2023-04-16 18:10:49.000000 seas-0.0.4/tests/__init__.py
--rw-rw-r--   0 sydney    (1000) sydney    (1000)     2221 2023-04-16 18:10:49.000000 seas-0.0.4/tests/colormaps_test.py
--rw-rw-r--   0 sydney    (1000) sydney    (1000)     2284 2023-04-16 18:48:08.000000 seas-0.0.4/tests/experiment_test.py
--rw-rw-r--   0 sydney    (1000) sydney    (1000)      970 2023-04-16 18:10:49.000000 seas-0.0.4/tests/filemanager_test.py
--rw-rw-r--   0 sydney    (1000) sydney    (1000)     1017 2023-04-16 18:10:49.000000 seas-0.0.4/tests/video_test.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 seas-0.0.5/developer_notes.md
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 seas-0.0.5/requirements.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 seas-0.0.5/setup.cfg
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 seas-0.0.5/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 seas-0.0.5/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 seas-0.0.5/.pytest_cache/README.md
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 seas-0.0.5/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 seas-0.0.5/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 seas-0.0.5/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 seas-0.0.5/docs/.readthedocs.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 seas-0.0.5/docs/Makefile
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 seas-0.0.5/docs/conf.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 seas-0.0.5/docs/doc-requirements.txt
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 seas-0.0.5/docs/examples.rst
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 seas-0.0.5/docs/index.rst
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 seas-0.0.5/docs/install.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 seas-0.0.5/docs/make.bat
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 seas-0.0.5/docs/modules.rst
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 seas-0.0.5/docs/seas.rst
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 seas-0.0.5/examples/.fuse_hidden000000f200000001
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 seas-0.0.5/examples/README.md
+-rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 seas-0.0.5/examples/domain_map.py
+-rw-r--r--   0        0        0    10438 2020-02-02 00:00:00.000000 seas-0.0.5/examples/hdf5manager.py
+-rw-r--r--   0        0        0    14872 2020-02-02 00:00:00.000000 seas-0.0.5/examples/ica_figures.py
+-rw-r--r--   0        0        0    11300 2020-02-02 00:00:00.000000 seas-0.0.5/examples/ica_project.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 seas-0.0.5/examples/play_dfof_movie.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 seas-0.0.5/examples/view_components.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 seas-0.0.5/seas/__init__.py
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 seas-0.0.5/seas/colormaps.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 seas-0.0.5/seas/config.txt
+-rw-r--r--   0        0        0     5862 2020-02-02 00:00:00.000000 seas-0.0.5/seas/defaults.py
+-rw-r--r--   0        0        0    24292 2020-02-02 00:00:00.000000 seas-0.0.5/seas/domains.py
+-rw-r--r--   0        0        0    18320 2020-02-02 00:00:00.000000 seas-0.0.5/seas/experiment.py
+-rw-r--r--   0        0        0    12195 2020-02-02 00:00:00.000000 seas-0.0.5/seas/filemanager.py
+-rw-r--r--   0        0        0    69486 2020-02-02 00:00:00.000000 seas-0.0.5/seas/gui.py
+-rw-r--r--   0        0        0    17569 2020-02-02 00:00:00.000000 seas-0.0.5/seas/hdf5manager.py
+-rw-r--r--   0        0        0    26572 2020-02-02 00:00:00.000000 seas-0.0.5/seas/ica.py
+-rw-r--r--   0        0        0    10425 2020-02-02 00:00:00.000000 seas-0.0.5/seas/rois.py
+-rw-r--r--   0        0        0    15671 2020-02-02 00:00:00.000000 seas-0.0.5/seas/signalanalysis.py
+-rw-r--r--   0        0        0    38898 2020-02-02 00:00:00.000000 seas-0.0.5/seas/video.py
+-rw-r--r--   0        0        0    25541 2020-02-02 00:00:00.000000 seas-0.0.5/seas/waveletAnalysis.py
+-rw-r--r--   0        0        0    17203 2020-02-02 00:00:00.000000 seas-0.0.5/seas/waveletFunctions.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 seas-0.0.5/seas/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 seas-0.0.5/seas/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 seas-0.0.5/seas/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 seas-0.0.5/seas/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 seas-0.0.5/seas/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 seas-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 seas-0.0.5/tests/colormaps_test.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 seas-0.0.5/tests/experiment_test.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 seas-0.0.5/tests/filemanager_test.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 seas-0.0.5/tests/video_test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 seas-0.0.5/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 seas-0.0.5/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 seas-0.0.5/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 seas-0.0.5/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 seas-0.0.5/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 seas-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 seas-0.0.5/LICENSE
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 seas-0.0.5/README.md
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 seas-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 seas-0.0.5/PKG-INFO
```

### Comparing `seas-0.0.4/LICENSE` & `seas-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `seas-0.0.4/seas/colormaps.py` & `seas-0.0.5/seas/colormaps.py`

 * *Files identical despite different names*

### Comparing `seas-0.0.4/seas/defaults.py` & `seas-0.0.5/seas/defaults.py`

 * *Files identical despite different names*

### Comparing `seas-0.0.4/seas/domains.py` & `seas-0.0.5/seas/domains.py`

 * *Files identical despite different names*

### Comparing `seas-0.0.4/seas/experiment.py` & `seas-0.0.5/seas/experiment.py`

 * *Files identical despite different names*

### Comparing `seas-0.0.4/seas/filemanager.py` & `seas-0.0.5/seas/filemanager.py`

 * *Files identical despite different names*

### Comparing `seas-0.0.4/seas/gui.py` & `seas-0.0.5/seas/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import matplotlib
 import tkinter as tk
 import tkinter.messagebox
 
 # Set the matplotlib backend to tk figures.
 # If imported, cannot plot to regular matplotlib figures!
-matplotlib.use("TkAgg")
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 from matplotlib.figure import Figure
 
 from seas.signalanalysis import lag_n_autocorr, sort_noise, short_time_fourier_transform
 from seas.waveletAnalysis import waveletAnalysis
 from seas.hdf5manager import hdf5manager
 from seas.defaults import config
@@ -38,26 +37,26 @@
         rotate: An integer number of counterclockwise rotations.
         savepath: Where to save or load component information from.
         default_assignment: The default assignment of which components are signal or artifact.
 
     Returns:
         components: The components dict, updated with any new region assignment, or artifact assignment, if applicable. 
     '''
-
     print('\nStarting ICA Component Selection GUI\n-----------------------')
     print(
         'If you experience problems with this GUI, check your tk version with the following terminal command:'
     )
     print('\tpython -m tkinter')
     print(
         'This will launch a GUI that tells you your tk version.  Make sure it is >=8.6'
     )
     print(
         "If installed using conda, use 'conda install -c anaconda tk' to update"
     )
+    matplotlib.use("TkAgg")
 
     if type(components) is str:
         f = hdf5manager(components)
         print('loading components...')
         components = f.load()
         load_hdf5 = True
     else:
@@ -337,33 +336,35 @@
             label = tk.Label(self,
                              text='Select Components to Remove:',
                              font=LARGE_FONT)
 
             # Initialize navigation buttons.
             navbuttons = tk.Frame(self)
             self.llbutton = tk.Button(navbuttons,
-                                      text='<<< {0} PCs'.format(4 *
-                                                                self.n_images),
+                                      text='<<< {0} Components'.format(
+                                          4 * self.n_images),
                                       command=lambda: self.changeComponentPage(
                                           self.current_page_number - 4))
             self.lbutton = tk.Button(navbuttons,
-                                     text='<<< {0} PCs'.format(self.n_images),
+                                     text='<<< {0} Components'.format(
+                                         self.n_images),
                                      command=lambda: self.changeComponentPage(
                                          self.current_page_number - 1))
             self.homebutton = tk.Button(
                 navbuttons,
                 text='Home',
                 command=lambda: self.changeComponentPage(0))
             self.rbutton = tk.Button(navbuttons,
-                                     text='{0} PCs >>>'.format(self.n_images),
+                                     text='{0} Components >>>'.format(
+                                         self.n_images),
                                      command=lambda: self.changeComponentPage(
                                          self.current_page_number + 1))
             self.rrbutton = tk.Button(navbuttons,
-                                      text='{0} PCs >>>'.format(4 *
-                                                                self.n_images),
+                                      text='{0} Components >>>'.format(
+                                          4 * self.n_images),
                                       command=lambda: self.changeComponentPage(
                                           self.current_page_number + 4))
 
             # Make frame for pc max value controller.
             pccontrol = tk.Frame(self)
             upper_limit = tk.StringVar()
             upper_limit.set(str(maxval))
@@ -577,15 +578,15 @@
                             'Index exceeds range')
                         assert int(newvalue) >= 0, 'Index below 0'
                         self.component_id[0] = int(newvalue)
                         self.selected_component.set(str(self.component_id[0]))
                         fig.update_figures(self.component_id[0])
 
                     except:
-                        print('Not changing upper PC cutoff.')
+                        print('Not changing upper Component cutoff.')
                         self.selected_component.set(str(self.component_id[0]))
                         # Reset text box to previous value.
 
             # Initialize PC info page.
             tk.Frame.__init__(self, parent)
             label = tk.Label(self, text='Component Viewer:', font=LARGE_FONT)
             label.pack(pady=10, padx=10)
@@ -753,15 +754,15 @@
                     f = Figure(figsize=(4, 4), dpi=100, frameon=False)
                     self.fig = f
                     self.ax = f.add_subplot(111)
                     f.subplots_adjust(left=0.2,
                                       bottom=0.15,
                                       right=0.85,
                                       top=0.85)
-                    self.ax.set_title('PC Timecourse')
+                    self.ax.set_title('Component Timecourse')
                     self.ax.set_xlabel('Time (s)')
                     self.ax.set_ylabel('Sum Intensity (dFoF)')
                     self.ax.plot([])
                     self.canvas = FigureCanvasTkAgg(f, frame)
                     self.canvas.mpl_connect(
                         'button_press_event',
                         lambda event: self.on_key_press(event))
@@ -1042,15 +1043,15 @@
                         self.component_id[0] = int(newvalue)
                         self.selected_component.set(str(self.component_id[0]))
                         fig.update_figures(self.component_id[0])
 
                     except Exception as e:
                         print('Error!')
                         print('\t', e)
-                        print('Not changing upper PC cutoff.')
+                        print('Not changing upper Component cutoff.')
                         self.selected_component.set(str(self.component_id[0]))
                         # Reset text box to previous value.
 
             # Initialize PC info page.
             tk.Frame.__init__(self, parent)
             label = tk.Label(self, text='Domain ROI Viewer:', font=LARGE_FONT)
             label.pack(pady=10, padx=10)
```

### Comparing `seas-0.0.4/seas/hdf5manager.py` & `seas-0.0.5/seas/hdf5manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,16 +245,16 @@
 
         if target is None:
             if verbose:
                 print('No target key specified; loading all datasets')
             keys = f.keys()
             attrs = f.attrs
         else:
-            assert (type(target) is str) or (type(target)
-                                             is list), 'invalid target'
+            assert (type(target) is str) or (type(target) is
+                                             list), 'invalid target'
             if type(target) is str:
                 target = [target]
 
             keys = []
             attrs = []
 
             for item in target:
```

### Comparing `seas-0.0.4/seas/ica.py` & `seas-0.0.5/seas/ica.py`

 * *Files identical despite different names*

### Comparing `seas-0.0.4/seas/rois.py` & `seas-0.0.5/seas/rois.py`

 * *Files identical despite different names*

### Comparing `seas-0.0.4/seas/signalanalysis.py` & `seas-0.0.5/seas/signalanalysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -156,69 +156,75 @@
     if high is not None:
         b, a = butter_lowpass(high, fps, order=order)
         data = signal.filtfilt(b, a, data)
 
     return data
 
 
-def local_max(x_values: np.ndarray, array1d: np.ndarray, sig=None):
+def local_max(x_values: np.ndarray,
+              array1d: np.ndarray,
+              sig: np.ndarray = None) -> Tuple[np.ndarray, np.ndarray]:
     '''
     Finds the local max array values and their respective position (xvalues)
-    by giving a significance cuttoff value array of the same size as the array1d, this will also return
-    the cutoff significance at each local maxima.
-
-    TODO(@brmullen): Add documentation here.
+    by giving a significance cuttoff value array of the same size as the array1d, 
+    this will also return the cutoff significance at each local maxima.
 
     Args:
-        x_values:
-        array1d:
-        sig:
+        x_values: positional information (i.e. time, sequence, etc.)
+        array1d: data values (i.e. Dfof, etc.)
+        sig: third list, significance of signal, that is returned 
+            (in realitity this could be any array of equal len as array1d) 
 
     Returns:
+        xvalues of where the local max 
+        data values of the local max
+        third list of significance of where the local max
 
     '''
     if sig is not None:
-        i = np.r_[True, array1d[1:] > array1d[:-1]] & np.r_[array1d[:-1] >
-                                                            array1d[1:], True]
+        i = np.r_[True, array1d[1:] > array1d[:-1]] & np.r_[
+            array1d[:-1] > array1d[1:], True]
         return list(compress(x_values,
                              i)), list(compress(array1d,
                                                 i)), list(compress(sig, i))
     else:
-        i = np.r_[True, array1d[1:] > array1d[:-1]] & np.r_[array1d[:-1] >
-                                                            array1d[1:], True]
+        i = np.r_[True, array1d[1:] > array1d[:-1]] & np.r_[
+            array1d[:-1] > array1d[1:], True]
         return list(compress(x_values, i)), list(compress(array1d, i))
 
 
 def local_min(x_values: np.ndarray,
               array1d: np.ndarray,
               sig=None) -> Tuple[List[np.ndarray], List[np.ndarray]]:
     '''
     Finds the local min array values and their respective position (xvalues)
-    by giving a significance cutoff value array of the same size as the array1d, this will also return
-    the cutoff significance at each local minima
-
-    TODO(@brmullen): Add documentation here.
+    by giving a significance cuttoff value array of the same size as the array1d, 
+    this will also return the cutoff significance at each local maxima.
 
     Args:
-        x_values:
-        array1d:
-        sig:
+        x_values: positional information (i.e. time, sequence, etc.)
+        array1d: data values (i.e. Dfof, etc.)
+        sig: third list, significance of signal, that is returned 
+            (in realitity this could be any array of equal len as array1d) 
 
     Returns:
-
+        xvalues of where the local min 
+        data values of the local min
+        third list of significance of where the local min
     '''
+
     if sig is not None:
-        i = np.r_[True, array1d[1:] < array1d[:-1]] & np.r_[array1d[:-1] <
-                                                            array1d[1:], True]
+        i = np.r_[True, array1d[1:] < array1d[:-1]] & np.r_[
+            array1d[:-1] < array1d[1:], True]
         return list(compress(x_values,
                              i)), list(compress(array1d,
                                                 i)), list(compress(sig, i))
     else:
-        i = np.r_[True, array1d[1:] < array1d[:-1]] & np.r_[array1d[:-1] <
-                                                            array1d[1:], True]
+        i = np.r_[True, array1d[1:] < array1d[:-1]] & np.r_[
+            array1d[:-1] < array1d[1:], True]
         return list(compress(x_values, i)), list(compress(array1d, i))
 
 
 def abline(slope: float,
            intercept: float,
            x_max: float,
            label: str = None,
@@ -256,31 +262,33 @@
         time: The time, or x axis to fit the linear regression to.
         signal: The signal, or y axis to fit the linear regression to.
         verbose: Whether to print a verbose output specifying the fit results.
 
     Returns:
         slope: The linear regression slope.
         intercept: The linear regression intercept.
-
-    TODO(@brmullen): Check documentation.
     '''
     regr = linear_model.LinearRegression(fit_intercept=True)
     regr.fit(time.reshape(-1, 1), signal.reshape(-1, 1))
     wsumpred = regr.predict(signal.reshape(-1, 1))
     slope = regr.coef_[0]
     intercept = regr.intercept_[0]
     if verbose:
         print('Coefficients: \n', regr.coef_)
         print('Mean squared error: %.2f' % mean_squared_error(signal, wsumpred))
         print('Variance score: %.2f' % r2_score(signal, wsumpred))
 
     return slope, intercept
 
 
-def tdelay_correlation(vectors, n, max_offset=150, return_window=False):
+def tdelay_correlation(
+        vectors: np.ndarray,
+        n: int,
+        max_offset: int = 150,
+        return_window: bool = False) -> Tuple[np.ndarray, np.ndarray]:
     '''
     Calculates correlations of timecourses stored in an array 'vectors', of shape 
     (m, t) against the 'n'th element of the array, or an input vector of size 't'.  
     Returns 
 
     Arguments:
         vectors: a (m,t) numpy array containing all time series, including the one to compare to.
@@ -289,16 +297,14 @@
         return_window: Whether to return the maximum correlation value in the context of the correlation window.
 
     Returns:
         x_corr: the correlation of each vector with vector 'n', and time offset.
         t_delay: The time delay which maximizes the correlation value.
         corr_window: Returns the maximum correlation at the given time delay for each time series,
             all other values are zero.  Only returned if return_window is True.
-
-    TODO(@brmullen): Check documentation.
     '''
 
     if type(n) is int:
         tc = vectors[n].copy()
 
     elif type(n) is np.ndarray:
         if vectors.ndim == 1:
@@ -336,33 +342,58 @@
 
     if return_window:
         return x_corr, t_delay, corr_window
     else:
         return x_corr, t_delay
 
 
-def gaussian_smooth_2d(matrix, dj, dt):
+def gaussian_smooth_2d(matrix: np.ndarray, dj: float, dt: float) -> np.ndarray:
     '''
-    TODO(@brmullen): Write documentation.
+    This takes a 2-d matrix and applies a smoothing gaussian
+    filter defined by the two sigma variables (dj, dt)
+
+    Arguments:
+        matrix: 2d matrix of values to smooth
+        dj = sigma to define the first dimension gaussian
+        dt = sigma to define the second dimension gaussian
+
+    Returns:
+        Smoothed 2d matrix
+
     '''
     sigma = [dj, dt]
     smooth_matrix = gaussian_filter(matrix.real, sigma=sigma)
     smooth_matrix += gaussian_filter(matrix.imag, sigma=sigma).imag
 
     return smooth_matrix
 
 
-def short_time_fourier_transform(data,
-                                 fps=10,
-                                 fft_len=100,
-                                 overlap=99,
-                                 verbose=False):
+def short_time_fourier_transform(data: np.ndarray,
+                                 fps: float = 10,
+                                 fft_len: int = 100,
+                                 overlap: int = 50,
+                                 verbose: bool = False) -> np.array:
     '''
-    TODO(@brmullen): Write documentation.
+    Creates a short time windowed fourier transform of a time series
+
+    Arguments:
+        data: Time series (1d vector)
+        fps: frames per second
+        fft_len: window length (number of data points to run fft)
+        overlap: Overlab between adjacent windows (number of datapoints that are 
+            similar between adajacent windows)
+        verbose: Boolean to be verbose or not
+
+    Returns:
+        result: 2d matrix of short time windowed Fourier transform
+        fps: frames per second used in fourier transform
+        nyq: nyquist frequency
+        maxData: location of the maxima of the 2d transform
     '''
+
     padEndSz = fft_len
     # The last segment can overlap the end of the data array by no more
     # than one window size.
     nyq = fps / 2  # Nyquist frequency.
 
     if verbose:
         print("Calculating STFT of window size {0} and an overlap of {1}\
```

### Comparing `seas-0.0.4/seas/video.py` & `seas-0.0.5/seas/video.py`

 * *Files identical despite different names*

### Comparing `seas-0.0.4/seas/waveletFunctions.py` & `seas-0.0.5/seas/waveletFunctions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,103 +1,112 @@
+'''
+Copyright (C) 1995-2004, Christopher Torrence and Gilbert P.Compo
+Python version of the code is written by Evgeniya Predybaylo in 2014
+
+  This software may be used, copied, or redistributed as long as it is not
+  sold and this copyright notice is reproduced on each copy made. This
+  routine is provided as is without any express or implied warranties
+  whatsoever.
+
+Notice: Please acknowledge the use of the above software in any publications:
+   ``Wavelet software was provided by C. Torrence and G. Compo,
+     and is available at URL: http://paos.colorado.edu/research/wavelets/''.
+
+Reference: Torrence, C. and G. P. Compo, 1998: A Practical Guide to
+           Wavelet Analysis. <I>Bull. Amer. Meteor. Soc.</I>, 79, 61-78.
+
+Please send a copy of such publications to either C. Torrence or G. Compo:
+ Dr. Christopher Torrence               Dr. Gilbert P. Compo
+ Research Systems, Inc.                 Climate Diagnostics Center
+ 4990 Pearl East Circle                 325 Broadway R/CDC1
+ Boulder, CO 80301, USA                 Boulder, CO 80305-3328, USA
+ E-mail: chris[AT]rsinc[DOT]com         E-mail: compo[AT]colorado[DOT]edu
+
+-------------------------------------------------------------------------------------------------------------------
+'''
 from scipy.special._ufuncs import gammainc, gamma
 import numpy as np
 from scipy.optimize import fminbound
 
 __author__ = 'Evgeniya Predybaylo'
 
-# Copyright (C) 1995-2004, Christopher Torrence and Gilbert P.Compo
-# Python version of the code is written by Evgeniya Predybaylo in 2014
-#
-#   This software may be used, copied, or redistributed as long as it is not
-#   sold and this copyright notice is reproduced on each copy made. This
-#   routine is provided as is without any express or implied warranties
-#   whatsoever.
-#
-# Notice: Please acknowledge the use of the above software in any publications:
-#    ``Wavelet software was provided by C. Torrence and G. Compo,
-#      and is available at URL: http://paos.colorado.edu/research/wavelets/''.
-#
-# Reference: Torrence, C. and G. P. Compo, 1998: A Practical Guide to
-#            Wavelet Analysis. <I>Bull. Amer. Meteor. Soc.</I>, 79, 61-78.
-#
-# Please send a copy of such publications to either C. Torrence or G. Compo:
-#  Dr. Christopher Torrence               Dr. Gilbert P. Compo
-#  Research Systems, Inc.                 Climate Diagnostics Center
-#  4990 Pearl East Circle                 325 Broadway R/CDC1
-#  Boulder, CO 80301, USA                 Boulder, CO 80305-3328, USA
-#  E-mail: chris[AT]rsinc[DOT]com         E-mail: compo[AT]colorado[DOT]edu
-#
-#-------------------------------------------------------------------------------------------------------------------
-
-# # WAVELET  1D Wavelet transform with optional significance testing
-#   wave, period, scale, coi = wavelet(Y, dt, pad, dj, s0, J1, mother, param)
-#
-#   Computes the wavelet transform of the vector Y (length N),
-#   with sampling rate DT.
-#
-#   By default, the Morlet wavelet (k0=6) is used.
-#   The wavelet basis is normalized to have total energy=1 at all scales.
-#
-# INPUTS:
-#
-#    Y = the time series of length N.
-#    DT = amount of time between each Y value, i.e. the sampling time.
-#
-# OUTPUTS:
-#
-#    WAVE is the WAVELET transform of Y. This is a complex array
-#    of dimensions (N,J1+1). FLOAT(WAVE) gives the WAVELET amplitude,
-#    ATAN(IMAGINARY(WAVE),FLOAT(WAVE) gives the WAVELET phase.
-#    The WAVELET power spectrum is ABS(WAVE)**2.
-#    Its units are sigma**2 (the time series variance).
-#
-# OPTIONAL INPUTS:
-#
-# *** Note *** if none of the optional variables is set up, then the program
-#   uses default values of -1.
-#
-#    PAD = if set to 1 (default is 0), pad time series with enough zeroes to get
-#         N up to the next higher power of 2. This prevents wraparound
-#         from the end of the time series to the beginning, and also
-#         speeds up the FFT's used to do the wavelet transform.
-#         This will not eliminate all edge effects (see COI below).
-#
-#    DJ = the spacing between discrete scales. Default is 0.25.
-#         A smaller # will give better scale resolution, but be slower to plot.
-#
-#    S0 = the smallest scale of the wavelet.  Default is 2*DT.
-#
-#    J1 = the # of scales minus one. Scales range from S0 up to S0*2**(J1*DJ),
-#        to give a total of (J1+1) scales. Default is J1 = (LOG2(N DT/S0))/DJ.
-#
-#    MOTHER = the mother wavelet function.
-#             The choices are 'MORLET', 'PAUL', or 'DOG'
-#
-#    PARAM = the mother wavelet parameter.
-#            For 'MORLET' this is k0 (wavenumber), default is 6.
-#            For 'PAUL' this is m (order), default is 4.
-#            For 'DOG' this is m (m-th derivative), default is 2.
-#
-#
-# OPTIONAL OUTPUTS:
-#
-#    PERIOD = the vector of "Fourier" periods (in time units) that corresponds
-#           to the SCALEs.
-#
-#    SCALE = the vector of scale indices, given by S0*2**(j*DJ), j=0...J1
-#            where J1+1 is the total # of scales.
-#
-#    COI = if specified, then return the Cone-of-Influence, which is a vector
-#        of N points that contains the maximum period of useful information
-#        at that particular time.
-#        Periods greater than this are subject to edge effects.
 
+def wavelet(Y,
+            dt: int,
+            pad: int = 0,
+            dj: float = -1,
+            s0: float = -1,
+            J1: float = -1,
+            mother: str = -1,
+            param: int = -1):
+    '''
+    WAVELET  1D Wavelet transform with optional significance testing
+      wave, period, scale, coi = wavelet(Y, dt, pad, dj, s0, J1, mother, param)
+
+      Computes the wavelet transform of the vector Y (length N),
+      with sampling rate DT.
+
+      By default, the Morlet wavelet (k0=6) is used.
+      The wavelet basis is normalized to have total energy=1 at all scales.
+
+    INPUTS:
+
+       Y = the time series of length N.
+       DT = amount of time between each Y value, i.e. the sampling time.
+
+    OUTPUTS:
+
+       WAVE is the WAVELET transform of Y. This is a complex array
+       of dimensions (N,J1+1). FLOAT(WAVE) gives the WAVELET amplitude,
+       ATAN(IMAGINARY(WAVE),FLOAT(WAVE) gives the WAVELET phase.
+       The WAVELET power spectrum is ABS(WAVE)**2.
+       Its units are sigma**2 (the time series variance).
+
+    OPTIONAL INPUTS:
+
+    *** Note *** if none of the optional variables is set up, then the program
+      uses default values of -1.
+
+       PAD = if set to 1 (default is 0), pad time series with enough zeroes to get
+            N up to the next higher power of 2. This prevents wraparound
+            from the end of the time series to the beginning, and also
+            speeds up the FFT's used to do the wavelet transform.
+            This will not eliminate all edge effects (see COI below).
+
+       DJ = the spacing between discrete scales. Default is 0.25.
+            A smaller # will give better scale resolution, but be slower to plot.
+
+       S0 = the smallest scale of the wavelet.  Default is 2*DT.
+
+       J1 = the # of scales minus one. Scales range from S0 up to S0*2**(J1*DJ),
+           to give a total of (J1+1) scales. Default is J1 = (LOG2(N DT/S0))/DJ.
+
+       MOTHER = the mother wavelet function.
+                The choices are 'MORLET', 'PAUL', or 'DOG'
+
+       PARAM = the mother wavelet parameter.
+               For 'MORLET' this is k0 (wavenumber), default is 6.
+               For 'PAUL' this is m (order), default is 4.
+               For 'DOG' this is m (m-th derivative), default is 2.
+
+
+    OPTIONAL OUTPUTS:
+
+       PERIOD = the vector of "Fourier" periods (in time units) that corresponds
+              to the SCALEs.
+
+       SCALE = the vector of scale indices, given by S0*2**(j*DJ), j=0...J1
+               where J1+1 is the total # of scales.
+
+       COI = if specified, then return the Cone-of-Influence, which is a vector
+           of N points that contains the maximum period of useful information
+           at that particular time.
+           Periods greater than this are subject to edge effects.
+    '''
 
-# def wavelet(Y, dt, pad=0, dj=-1, s0=-1, J1=-1, mother=-1, param=-1):
-def wavelet(Y, dt, pad=0, dj=-1, s0=-1, J1=-1, mother=-1, param=-1):
     n1 = len(Y)
 
     if s0 == -1:
         s0 = 2 * dt
     if dj == -1:
         dj = 1. / 4.
     if J1 == -1:
@@ -141,40 +150,38 @@
          np.insert(np.flipud(np.arange(0, n1 / 2 - 1)), [-1],
                    [1E-5])))  # COI [Sec.3g]
     wave = wave[:, :n1]  # get rid of padding before returning
 
     return wave, period, scale, coi
 
 
-#-------------------------------------------------------------------------------------------------------------------
-# WAVE_BASES  1D Wavelet functions Morlet, Paul, or DOG
-#
-#  DAUGHTER,FOURIER_FACTOR,COI,DOFMIN = wave_bases(MOTHER,K,SCALE,PARAM)
-#
-#   Computes the wavelet function as a function of Fourier frequency,
-#   used for the wavelet transform in Fourier space.
-#   (This program is called automatically by WAVELET)
-#
-# INPUTS:
-#
-#    MOTHER = a string, equal to 'MORLET' or 'PAUL' or 'DOG'
-#    K = a vector, the Fourier frequencies at which to calculate the wavelet
-#    SCALE = a number, the wavelet scale
-#    PARAM = the nondimensional parameter for the wavelet function
-#
-# OUTPUTS:
-#
-#    DAUGHTER = a vector, the wavelet function
-#    FOURIER_FACTOR = the ratio of Fourier period to scale
-#    COI = a number, the cone-of-influence size at the scale
-#    DOFMIN = a number, degrees of freedom for each point in the wavelet power
-#             (either 2 for Morlet and Paul, or 1 for the DOG)
+def wave_bases(mother: str, k: np.ndarray, scale: int, param: int):
+    '''WAVE_BASES  1D Wavelet functions Morlet, Paul, or DOG
 
+     DAUGHTER,FOURIER_FACTOR,COI,DOFMIN = wave_bases(MOTHER,K,SCALE,PARAM)
 
-def wave_bases(mother, k, scale, param):
+      Computes the wavelet function as a function of Fourier frequency,
+      used for the wavelet transform in Fourier space.
+      (This program is called automatically by WAVELET)
+
+    INPUTS:
+
+       MOTHER = a string, equal to 'MORLET' or 'PAUL' or 'DOG'
+       K = a vector, the Fourier frequencies at which to calculate the wavelet
+       SCALE = a number, the wavelet scale
+       PARAM = the nondimensional parameter for the wavelet function
+
+    OUTPUTS:
+
+       DAUGHTER = a vector, the wavelet function
+       FOURIER_FACTOR = the ratio of Fourier period to scale
+       COI = a number, the cone-of-influence size at the scale
+       DOFMIN = a number, degrees of freedom for each point in the wavelet power
+                (either 2 for Morlet and Paul, or 1 for the DOG)
+    '''
     n = len(k)
     kplus = np.array(k > 0., dtype=float)
 
     if mother == 'MORLET':  #-----------------------------------  Morlet
 
         if param == -1:
             param = 6.
@@ -212,79 +219,78 @@
         dofmin = 1
     else:
         print('Mother must be one of MORLET, PAUL, DOG')
 
     return daughter, fourier_factor, coi, dofmin
 
 
-#-------------------------------------------------------------------------------------------------------------------
-# WAVE_SIGNIF  Significance testing for the 1D Wavelet transform WAVELET
-#
-#   SIGNIF = wave_signif(Y,DT,SCALE,SIGTEST,LAG1,SIGLVL,DOF,MOTHER,PARAM)
-#
-# INPUTS:
-#
-#    Y = the time series, or, the VARIANCE of the time series.
-#        (If this is a single number, it is assumed to be the variance...)
-#    DT = amount of time between each Y value, i.e. the sampling time.
-#    SCALE = the vector of scale indices, from previous call to WAVELET.
-#
-#
-# OUTPUTS:
-#
-#    SIGNIF = significance levels as a function of SCALE
-#    FFT_THEOR = output theoretical red-noise spectrum as fn of PERIOD
-#
-#
-# OPTIONAL INPUTS:
-# *** Note *** setting any of the following to -1 will cause the default
-#               value to be used.
-#
-#    SIGTEST = 0, 1, or 2.    If omitted, then assume 0.
-#
-#         If 0 (the default), then just do a regular chi-square test,
-#             i.e. Eqn (18) from Torrence & Compo.
-#         If 1, then do a "time-average" test, i.e. Eqn (23).
-#             In this case, DOF should be set to NA, the number
-#             of local wavelet spectra that were averaged together.
-#             For the Global Wavelet Spectrum, this would be NA=N,
-#             where N is the number of points in your time series.
-#         If 2, then do a "scale-average" test, i.e. Eqns (25)-(28).
-#             In this case, DOF should be set to a
-#             two-element vector [S1,S2], which gives the scale
-#             range that was averaged together.
-#             e.g. if one scale-averaged scales between 2 and 8,
-#             then DOF=[2,8].
-#
-#    LAG1 = LAG 1 Autocorrelation, used for SIGNIF levels. Default is 0.0
-#
-#    SIGLVL = significance level to use. Default is 0.95
-#
-#    DOF = degrees-of-freedom for signif test.
-#         IF SIGTEST=0, then (automatically) DOF = 2 (or 1 for MOTHER='DOG')
-#         IF SIGTEST=1, then DOF = NA, the number of times averaged together.
-#         IF SIGTEST=2, then DOF = [S1,S2], the range of scales averaged.
-#
-#       Note: IF SIGTEST=1, then DOF can be a vector (same length as SCALEs),
-#            in which case NA is assumed to vary with SCALE.
-#            This allows one to average different numbers of times
-#            together at different scales, or to take into account
-#            things like the Cone of Influence.
-#            See discussion following Eqn (23) in Torrence & Compo.
-
-
-def wave_signif(Y,
-                dt,
-                scale,
-                sigtest=-1,
-                lag1=-1,
-                siglvl=-1,
-                dof=-1,
-                mother=-1,
-                param=-1):
+def wave_signif(Y: np.ndarray,
+                dt: int,
+                scale: int,
+                sigtest: int = -1,
+                lag1: int = -1,
+                siglvl: float = -1,
+                dof: int = -1,
+                mother: str = -1,
+                param: int = -1):
+    '''
+    WAVE_SIGNIF  Significance testing for the 1D Wavelet transform WAVELET
+
+      SIGNIF = wave_signif(Y,DT,SCALE,SIGTEST,LAG1,SIGLVL,DOF,MOTHER,PARAM)
+
+    INPUTS:
+
+       Y = the time series, or, the VARIANCE of the time series.
+           (If this is a single number, it is assumed to be the variance...)
+       DT = amount of time between each Y value, i.e. the sampling time.
+       SCALE = the vector of scale indices, from previous call to WAVELET.
+
+
+    OUTPUTS:
+
+       SIGNIF = significance levels as a function of SCALE
+       FFT_THEOR = output theoretical red-noise spectrum as fn of PERIOD
+
+
+    OPTIONAL INPUTS:
+    *** Note *** setting any of the following to -1 will cause the default
+                  value to be used.
+
+       SIGTEST = 0, 1, or 2.    If omitted, then assume 0.
+
+            If 0 (the default), then just do a regular chi-square test,
+                i.e. Eqn (18) from Torrence & Compo.
+            If 1, then do a "time-average" test, i.e. Eqn (23).
+                In this case, DOF should be set to NA, the number
+                of local wavelet spectra that were averaged together.
+                For the Global Wavelet Spectrum, this would be NA=N,
+                where N is the number of points in your time series.
+            If 2, then do a "scale-average" test, i.e. Eqns (25)-(28).
+                In this case, DOF should be set to a
+                two-element vector [S1,S2], which gives the scale
+                range that was averaged together.
+                e.g. if one scale-averaged scales between 2 and 8,
+                then DOF=[2,8].
+
+       LAG1 = LAG 1 Autocorrelation, used for SIGNIF levels. Default is 0.0
+
+       SIGLVL = significance level to use. Default is 0.95
+
+       DOF = degrees-of-freedom for signif test.
+            IF SIGTEST=0, then (automatically) DOF = 2 (or 1 for MOTHER='DOG')
+            IF SIGTEST=1, then DOF = NA, the number of times averaged together.
+            IF SIGTEST=2, then DOF = [S1,S2], the range of scales averaged.
+
+          Note: IF SIGTEST=1, then DOF can be a vector (same length as SCALEs),
+               in which case NA is assumed to vary with SCALE.
+               This allows one to average different numbers of times
+               together at different scales, or to take into account
+               things like the Cone of Influence.
+               See discussion following Eqn (23) in Torrence & Compo.
+    '''
     n1 = len(np.atleast_1d(Y))
     J1 = len(scale) - 1
     s0 = np.min(scale)
     dj = np.log2(scale[1] / scale[0])
 
     if n1 == 1:
         variance = Y
@@ -385,28 +391,26 @@
         signif = (dj * dt / Cdelta / Savg) * fft_theor * chisquare  # [Eqn(26)]
     else:
         print('ERROR: sigtest must be either 0, 1, or 2')
 
     return signif
 
 
-#-------------------------------------------------------------------------------------------------------------------
-# CHISQUARE_INV  Inverse of chi-square cumulative distribution function (cdf).
-#
-#   X = chisquare_inv(P,V) returns the inverse of chi-square cdf with V
-#   degrees of freedom at fraction P.
-#   This means that P*100 percent of the distribution lies between 0 and X.
-#
-#   To check, the answer should satisfy:   P==gammainc(X/2,V/2)
-
-# Uses FMIN and CHISQUARE_SOLVE
-
+def chisquare_inv(P: float, V: float):
+    '''
+    CHISQUARE_INV  Inverse of chi-square cumulative distribution function (cdf).
+
+      X = chisquare_inv(P,V) returns the inverse of chi-square cdf with V
+      degrees of freedom at fraction P.
+      This means that P*100 percent of the distribution lies between 0 and X.
 
-def chisquare_inv(P, V):
+      To check, the answer should satisfy:   P==gammainc(X/2,V/2)
 
+    Uses FMIN and CHISQUARE_SOLVE
+    '''
     if (1 - P) < 1E-4:
         print('P must be < 0.9999')
 
     if P == 0.95 and V == 2:  # this is a no-brainer
         X = 5.9915
         return X
 
@@ -422,29 +426,24 @@
         MINN = MAXX
 
     X = X * V  # put back in the goofy V factor
 
     return X  # end of code
 
 
-#-------------------------------------------------------------------------------------------------------------------
-# CHISQUARE_SOLVE  Internal function used by CHISQUARE_INV
-#
-#   PDIFF=chisquare_solve(XGUESS,P,V)  Given XGUESS, a percentile P,
-#   and degrees-of-freedom V, return the difference between
-#   calculated percentile and P.
-
-# Uses GAMMAINC
-#
-# Written January 1998 by C. Torrence
-
-# extra factor of V is necessary because X is Normalized
-
+def chisquare_solve(XGUESS: float, P: float, V: float):
+    '''CHISQUARE_SOLVE  Internal function used by CHISQUARE_INV
 
-def chisquare_solve(XGUESS, P, V):
+      PDIFF=chisquare_solve(XGUESS,P,V)  Given XGUESS, a percentile P,
+      and degrees-of-freedom V, return the difference between
+      calculated percentile and P.
+    Uses GAMMAINC
+    Written January 1998 by C. Torrence
+    extra factor of V is necessary because X is Normalized
+    '''
 
     PGUESS = gammainc(V / 2, V * XGUESS / 2)  # incomplete Gamma function
 
     PDIFF = np.abs(PGUESS - P)  # error in calculated P
 
     TOL = 1E-4
     if PGUESS >= 1 - TOL:  # if P is very close to 1 (i.e. a bad guess)
```

### Comparing `seas-0.0.4/tests/colormaps_test.py` & `seas-0.0.5/tests/colormaps_test.py`

 * *Files identical despite different names*

### Comparing `seas-0.0.4/tests/experiment_test.py` & `seas-0.0.5/tests/experiment_test.py`

 * *Files identical despite different names*

### Comparing `seas-0.0.4/tests/filemanager_test.py` & `seas-0.0.5/tests/filemanager_test.py`

 * *Files identical despite different names*

### Comparing `seas-0.0.4/tests/video_test.py` & `seas-0.0.5/tests/video_test.py`

 * *Files identical despite different names*

