# Comparing `tmp/D47crunch-2.0.3.tar.gz` & `tmp/D47crunch-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D47crunch-2.0.3.tar", last modified: Sun Feb 27 13:38:09 2022, max compression
+gzip compressed data, was "D47crunch-2.0.4.tar", last modified: Thu May 11 12:01:01 2023, max compression
```

## Comparing `D47crunch-2.0.3.tar` & `D47crunch-2.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0   123715 2022-02-27 13:37:25.734973 D47crunch-2.0.3/D47crunch/__init__.py
--rwxr-xr-x   0        0        0     1745 2021-08-16 13:26:49.000000 D47crunch-2.0.3/build_doc.py
--rw-r--r--   0        0        0     1526 2022-02-27 13:04:41.592865 D47crunch-2.0.3/changelog.md
--rw-r--r--   0        0        0    50472 2021-08-16 13:26:49.000000 D47crunch-2.0.3/docs/D47_plot_Session_03.png
--rw-r--r--   0        0        0       18 2021-08-08 12:24:57.000000 D47crunch-2.0.3/docs/discussion.md
--rwxr-xr-x   0        0        0    18181 2022-02-27 13:37:25.736979 D47crunch-2.0.3/docs/howto.md
--rw-r--r--   0        0        0  1836066 2022-02-27 13:37:25.743250 D47crunch-2.0.3/docs/index.html
--rwxr-xr-x   0        0        0    23317 2021-08-08 12:24:57.000000 D47crunch-2.0.3/docs/old_documentation.md
--rw-r--r--   0        0        0    71913 2021-08-16 13:26:49.000000 D47crunch-2.0.3/docs/residuals.png
--rw-r--r--   0        0        0    45344 2021-08-16 13:26:49.000000 D47crunch-2.0.3/docs/time_distribution.png
--rw-r--r--   0        0        0     8880 2022-02-27 13:37:25.745183 D47crunch-2.0.3/docs/tutorial.md
--rwxr-xr-x   0        0        0     1416 2020-09-30 14:23:48.000000 D47crunch-2.0.3/examples/example.py
--rwxr-xr-x   0        0        0     1595 2020-09-30 14:45:55.000000 D47crunch-2.0.3/examples/rawdata.csv
--rw-r--r--   0        0        0     1503 2021-08-08 12:24:57.000000 D47crunch-2.0.3/license.md
--rw-r--r--   0        0        0      254 2021-08-16 13:26:49.000000 D47crunch-2.0.3/pdoc_templates/module.html.jinja2
--rw-r--r--   0        0        0      666 2022-02-27 13:04:41.599156 D47crunch-2.0.3/pyproject.toml
--rwxr-xr-x   0        0        0     1746 2021-08-08 21:02:48.000000 D47crunch-2.0.3/readme.md
--rwxr-xr-x   0        0        0    25494 2021-09-10 17:19:44.000000 D47crunch-2.0.3/tests/test_D47crunch.py
--rw-r--r--   0        0        0      552 2022-02-27 13:04:41.599875 D47crunch-2.0.3/todo.md
--rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 D47crunch-2.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0   124228 2023-05-11 12:00:54.571642 D47crunch-2.0.4/D47crunch/__init__.py
+-rwxr-xr-x   0        0        0     1745 2021-08-16 13:26:49.000000 D47crunch-2.0.4/build_doc.py
+-rw-r--r--   0        0        0     1711 2023-05-11 12:00:54.572165 D47crunch-2.0.4/changelog.md
+-rw-r--r--   0        0        0    50472 2021-08-16 13:26:49.000000 D47crunch-2.0.4/docs/D47_plot_Session_03.png
+-rw-r--r--   0        0        0       18 2021-08-08 12:24:57.000000 D47crunch-2.0.4/docs/discussion.md
+-rwxr-xr-x   0        0        0    18179 2023-05-11 09:02:14.247100 D47crunch-2.0.4/docs/howto.md
+-rw-r--r--   0        0        0  2651519 2023-05-11 12:00:54.580914 D47crunch-2.0.4/docs/index.html
+-rwxr-xr-x   0        0        0    23317 2021-08-08 12:24:57.000000 D47crunch-2.0.4/docs/old_documentation.md
+-rw-r--r--   0        0        0    71913 2021-08-16 13:26:49.000000 D47crunch-2.0.4/docs/residuals.png
+-rw-r--r--   0        0        0    45344 2021-08-16 13:26:49.000000 D47crunch-2.0.4/docs/time_distribution.png
+-rw-r--r--   0        0        0     8877 2023-05-11 09:02:14.255148 D47crunch-2.0.4/docs/tutorial.md
+-rwxr-xr-x   0        0        0     1416 2020-09-30 14:23:48.000000 D47crunch-2.0.4/examples/example.py
+-rwxr-xr-x   0        0        0     1595 2020-09-30 14:45:55.000000 D47crunch-2.0.4/examples/rawdata.csv
+-rw-r--r--   0        0        0     1503 2021-08-08 12:24:57.000000 D47crunch-2.0.4/license.md
+-rw-r--r--   0        0        0      254 2021-08-16 13:26:49.000000 D47crunch-2.0.4/pdoc_templates/module.html.jinja2
+-rw-r--r--   0        0        0      666 2022-02-27 13:04:41.599156 D47crunch-2.0.4/pyproject.toml
+-rwxr-xr-x   0        0        0     1746 2021-08-08 21:02:48.000000 D47crunch-2.0.4/readme.md
+-rwxr-xr-x   0        0        0    25494 2021-09-10 17:19:44.000000 D47crunch-2.0.4/tests/test_D47crunch.py
+-rw-r--r--   0        0        0      552 2022-02-27 13:04:41.599875 D47crunch-2.0.4/todo.md
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 D47crunch-2.0.4/PKG-INFO
```

### Comparing `D47crunch-2.0.3/D47crunch/__init__.py` & `D47crunch-2.0.4/D47crunch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 
 The **tutorial** section takes you through a series of simple steps to import/process data and print out the results.
 The **how-to** section provides instructions applicable to various specific tasks.
 
 .. include:: ../docs/tutorial.md
 .. include:: ../docs/howto.md
 
-## D47crunch API
+## API Documentation
 '''
 
 __docformat__ = "restructuredtext"
 __author__    = 'Mathieu Daëron'
 __contact__   = 'daeron@lsce.ipsl.fr'
-__copyright__ = 'Copyright (c) 2022 Mathieu Daëron'
+__copyright__ = 'Copyright (c) 2023 Mathieu Daëron'
 __license__   = 'Modified BSD License - https://opensource.org/licenses/BSD-3-Clause'
-__date__      = '2022-02-27'
-__version__   = '2.0.3'
+__date__      = '2023-05-11'
+__version__   = '2.0.4'
 
 import os
 import numpy as np
 from statistics import stdev
 from scipy.stats import t as tstudent
 from scipy.stats import levene
 from scipy.interpolate import interp1d
@@ -970,14 +970,15 @@
 
 	def __init__(self, l = [], mass = '47', logfile = '', session = 'mySession', verbose = False):
 		'''
 		**Parameters**
 
 		+ `l`: a list of dictionaries, with each dictionary including at least the keys
 		`Sample`, `d45`, `d46`, and `d47` or `d48`.
+		+ `mass`: `'47'` or `'48'`
 		+ `logfile`: if specified, write detailed logs to this file path when calling `D4xdata` methods.
 		+ `session`: define session name for analyses without a `Session` key
 		+ `verbose`: if `True`, print out detailed logs when calling `D4xdata` methods.
 
 		Returns a `D4xdata` object derived from `list`.
 		'''
 		self._4x = mass
@@ -1591,15 +1592,18 @@
 
 		self.standardization_method = method
 		self.assign_timestamps()
 
 		if method == 'pooled':
 			if weighted_sessions:
 				for session_group in weighted_sessions:
-					X = D4xdata([r for r in self if r['Session'] in session_group], mass = self._4x)
+					if self._4x == '47':
+						X = D47data([r for r in self if r['Session'] in session_group])
+					elif self._4x == '48':
+						X = D48data([r for r in self if r['Session'] in session_group])
 					X.Nominal_D4x = self.Nominal_D4x.copy()
 					X.refresh()
 					result = X.standardize(method = 'pooled', weighted_sessions = [], consolidate = False)
 					w = np.sqrt(result.redchi)
 					self.msg(f'Session group {session_group} MRSWD = {w:.4f}')
 					for r in X:
 						r[f'wD{self._4x}raw'] *= w
@@ -2690,22 +2694,25 @@
 
 		session = self[0]['Session']
 		x1 = 0
 # 		ymax = np.max([1e3 * (r['D47'] - self.samples[r['Sample']]['D47']) for r in self])
 		x_sessions = {}
 		one_or_more_singlets = False
 		one_or_more_multiplets = False
+		multiplets = set()
 		for k,r in enumerate(self):
 			if r['Session'] != session:
 				x2 = k-1
 				x_sessions[session] = (x1+x2)/2
 				ppl.axvline(k - 0.5, color = 'k', lw = .5)
 				session = r['Session']
 				x1 = k
 			singlet = len(self.samples[r['Sample']]['data']) == 1
+			if not singlet:
+				multiplets.add(r['Sample'])
 			if r['Sample'] in self.unknowns:
 				if singlet:
 					one_or_more_singlets = True
 				else:
 					one_or_more_multiplets = True
 			kw = dict(
 				marker = 'x' if singlet else '+',
@@ -2778,15 +2785,15 @@
 
 		ppl.ylabel('Δ$_{47}$ residuals (ppm)')
 		ppl.xticks([])
 		ppl.axis([-1, len(self), None, None])
 
 		if hist:
 			ppl.sca(ax2)
-			X = [1e3 * (r['D47'] - self.samples[r['Sample']]['D47']) for r in self]
+			X = [1e3 * (r['D47'] - self.samples[r['Sample']]['D47']) for r in self if r['Sample'] in multiplets]
 			ppl.hist(
 				X,
 				orientation = 'horizontal',
 				histtype = 'stepfilled',
 				ec = [.4]*3,
 				fc = [.25]*3,
 				alpha = .25,
@@ -2821,65 +2828,74 @@
 
 	def simulate(self, *args, **kwargs):
 		'''
 		Legacy function with warning message pointing to `virtual_data()`
 		'''
 		raise DeprecationWarning('D4xdata.simulate is deprecated and has been replaced by virtual_data()')
 
-	def plot_distribution_of_analyses(self, dir = 'output', filename = None, vs_time = False, output = None):
+	def plot_distribution_of_analyses(
+		self,
+		dir = 'output',
+		filename = None,
+		vs_time = False,
+		figsize = (6,4),
+		subplots_adjust = (0.02, 0.13, 0.85, 0.8),
+		output = None,
+		):
 		'''
 		Plot temporal distribution of all analyses in the data set.
 		
 		**Parameters**
 
 		+ `vs_time`: if `True`, plot as a function of `TimeTag` rather than sequentially.
 		'''
 
 		asamples = [s for s in self.anchors]
 		usamples = [s for s in self.unknowns]
 		if output is None or output == 'fig':
-			fig = ppl.figure(figsize = (6,4))
-			ppl.subplots_adjust(0.02, 0.03, 0.9, 0.8)
+			fig = ppl.figure(figsize = figsize)
+			ppl.subplots_adjust(*subplots_adjust)
+		Xmin = min([r['TimeTag'] if vs_time else j for j,r in enumerate(self)])
 		Xmax = max([r['TimeTag'] if vs_time else j for j,r in enumerate(self)])
+		Xmax += (Xmax-Xmin)/40
+		Xmin -= (Xmax-Xmin)/41
 		for k, s in enumerate(asamples + usamples):
 			if vs_time:
 				X = [r['TimeTag'] for r in self if r['Sample'] == s]
 			else:
 				X = [x for x,r in enumerate(self) if r['Sample'] == s]
-			Y = [k for x in X]
-			ppl.plot(X, Y, 'o', mec = None, mew = 0, mfc = 'b' if s in usamples else 'r', ms = 3, alpha = .5)
-			ppl.axhline(k, color = 'b' if s in usamples else 'r', lw = .5, alpha = .25)
-			ppl.text(Xmax, k, f'  {s}', va = 'center', ha = 'left', size = 7)
-		if vs_time:
-			t = [r['TimeTag'] for r in self]
-			t1, t2 = min(t), max(t)
-			tspan = t2 - t1
-			t1 -= tspan / len(self)
-			t2 += tspan / len(self)
-			ppl.axis([t1, t2, -1, k+1])
-		else:
-			ppl.axis([-1, len(self), -1, k+1])
+			Y = [-k for x in X]
+			ppl.plot(X, Y, 'o', mec = None, mew = 0, mfc = 'b' if s in usamples else 'r', ms = 3, alpha = .75)
+			ppl.axhline(-k, color = 'b' if s in usamples else 'r', lw = .5, alpha = .25)
+			ppl.text(Xmax, -k, f'   {s}', va = 'center', ha = 'left', size = 7, color = 'b' if s in usamples else 'r')
+		ppl.axis([Xmin, Xmax, -k-1, 1])
+		ppl.xlabel('\ntime')
+		ppl.gca().annotate('',
+			xy = (0.6, -0.02),
+			xycoords = 'axes fraction',
+			xytext = (.4, -0.02), 
+            arrowprops = dict(arrowstyle = "->", color = 'k'),
+            )
 			
 
-		x2 = 0
+		x2 = -1
 		for session in self.sessions:
 			x1 = min([r['TimeTag'] if vs_time else j for j,r in enumerate(self) if r['Session'] == session])
 			if vs_time:
 				ppl.axvline(x1, color = 'k', lw = .75)
-			if k:
-				if vs_time:
-					ppl.axvspan(x1,x2,color = 'k', zorder = -100, alpha = .2)
-				else:
-					ppl.axvline((x1+x2)/2, color = 'k', lw = .75)
+			if x2 > -1:
+				if not vs_time:
+					ppl.axvline((x1+x2)/2, color = 'k', lw = .75, alpha = .5)
 			x2 = max([r['TimeTag'] if vs_time else j for j,r in enumerate(self) if r['Session'] == session])
 # 			from xlrd import xldate_as_datetime
 # 			print(session, xldate_as_datetime(x1, 0), xldate_as_datetime(x2, 0))
 			if vs_time:
 				ppl.axvline(x2, color = 'k', lw = .75)
-			ppl.text((2*x1+x2)/3, k+1, session, ha = 'left', va = 'bottom', rotation = 45, size = 8)
+				ppl.axvspan(x1,x2,color = 'k', zorder = -100, alpha = .15)
+			ppl.text((x1+x2)/2, 1, f' {session}', ha = 'left', va = 'bottom', rotation = 45, size = 8)
 
 		ppl.xticks([])
 		ppl.yticks([])
 
 		if output is None:
 			if not os.path.exists(dir):
 				os.makedirs(dir)
```

### Comparing `D47crunch-2.0.3/build_doc.py` & `D47crunch-2.0.4/build_doc.py`

 * *Files identical despite different names*

### Comparing `D47crunch-2.0.3/changelog.md` & `D47crunch-2.0.4/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Changelog
 
+## v2.0.4
+*Released on 2023-05-11*
+
+### Changes
+* Graphically improved `D4xdata.plot_distribution_of_analyses()`
+
+### Bugfix
+* Fix `D4xdata.standardize()` when using weighted sessions
+
 ## v2.0.3
 *Released on 2022-02-27*
 
 ### New feature
 * `D4xdata.covar_table()` allows exporting the variance-covariance matrix or the correlation matrix for the Δ<sub>4x</sub> values of unknwon samples.
 
 ### Changes
```

### Comparing `D47crunch-2.0.3/docs/D47_plot_Session_03.png` & `D47crunch-2.0.4/docs/D47_plot_Session_03.png`

 * *Files identical despite different names*

### Comparing `D47crunch-2.0.3/docs/howto.md` & `D47crunch-2.0.4/docs/howto.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-## 2. How-to
+# 2. How-to
 
-### 2.1 Simulate a virtual data set to play with
+## 2.1 Simulate a virtual data set to play with
 
 It is sometimes convenient to quickly build a virtual data set of analyses, for instance to assess the final analytical precision achievable for a given combination of anchor and unknown analyses (see also Fig. 6 of [Daëron, 2021](https://doi.org/10.1029/2020GC009592)).
 
 This can be achieved with `virtual_data()`. The example below creates a dataset with four sessions, each of which comprises four analyses of anchor ETH-1, five of ETH-2, six of ETH-3, and two analyses of an unknown sample named `FOO` with an arbitrarily defined isotopic composition. Analytical repeatabilities for Δ47 and Δ48 are also specified arbitrarily. See the `virtual_data()` documentation for additional configuration parameters.
 
 ```py
 from D47crunch import *
@@ -38,15 +38,15 @@
 D.standardize()
 
 D.table_of_sessions(verbose = True, save_to_file = False)
 D.table_of_samples(verbose = True, save_to_file = False)
 D.table_of_analyses(verbose = True, save_to_file = False)
 ```
 
-### 2.2 Control data quality
+## 2.2 Control data quality
 
 `D47crunch` offers several tools to visualize processed data. The examples below use the same virtual data set, generated with:
 
 ```py
 from D47crunch import *
 from random import shuffle
 
@@ -77,45 +77,45 @@
 data47 = D47data(data)
 
 # process D47data instance:
 data47.crunch()
 data47.standardize()
 ```
 
-#### 2.1.1 Plotting the distribution of analyses through time
+### 2.2.1 Plotting the distribution of analyses through time
 
 ```py
 data47.plot_distribution_of_analyses(filename = 'time_distribution.pdf')
 ```
 
 ![time_distribution.png](time_distribution.png)
 
 The plot above shows the succession of analyses as if they were all distributed at regular time intervals. See `D4xdata.plot_distribution_of_analyses()` for how to plot analyses as a function of “true” time (based on the `TimeTag` for each analysis).
 
-#### 2.1.2 Generating session plots
+### 2.2.2 Generating session plots
 
 ```py
 data47.plot_sessions()
 ```
 
 Below is one of the resulting sessions plots. Each cross marker is an analysis. Anchors are in red and unknowns in blue. Short horizontal lines show the nominal Δ47 value for anchors, in red, or the average Δ47 value for unknowns, in blue (overall average for all sessions). Curved grey contours correspond to Δ47 standardization errors in this session.
 
 ![D47_plot_Session_03.png](D47_plot_Session_03.png)
 
-#### 2.1.3 Plotting Δ47 or Δ48 residuals
+### 2.2.3 Plotting Δ47 or Δ48 residuals
 
 ```py
 data47.plot_residuals(filename = 'residuals.pdf')
 ```
 
 ![residuals.png](residuals.png)
 
 Again, note that this plot only shows the succession of analyses as if they were all distributed at regular time intervals.
 
-### 2.3 Use a different set of anchors, change anchor nominal values, and/or change 17O correction parameters
+## 2.3 Use a different set of anchors, change anchor nominal values, and/or change oxygen-17 correction parameters
 
 Nominal values for various carbonate standards are defined in four places:
 
 * `D4xdata.Nominal_d13C_VPDB`
 * `D4xdata.Nominal_d18O_VPDB`
 * `D47data.Nominal_D4x` (also accessible through `D47data.Nominal_D47`)
 * `D48data.Nominal_D4x` (also accessible through `D48data.Nominal_D48`)
@@ -226,15 +226,15 @@
 bar.standardize() # compute absolute Δ47 values
 
 # and compare the final results:
 foo.table_of_samples(verbose = True, save_to_file = False)
 bar.table_of_samples(verbose = True, save_to_file = False)
 ```
 
-### 2.4 Process paired Δ47 and Δ48 values
+## 2.4 Process paired Δ47 and Δ48 values
 
 Purely in terms of data processing, it is not obvious why Δ47 and Δ48 data should not be handled separately. For now, `D47crunch` uses two independent classes — `D47data` and `D48data` — which crunch numbers and deal with standardization in very similar ways. The following example demonstrates how to print out combined outputs for `D47data` and `D48data`.
 
 ```py
 from D47crunch import *
 
 # generate virtual data:
```

### Comparing `D47crunch-2.0.3/docs/old_documentation.md` & `D47crunch-2.0.4/docs/old_documentation.md`

 * *Files identical despite different names*

### Comparing `D47crunch-2.0.3/docs/residuals.png` & `D47crunch-2.0.4/docs/residuals.png`

 * *Files identical despite different names*

### Comparing `D47crunch-2.0.3/docs/time_distribution.png` & `D47crunch-2.0.4/docs/time_distribution.png`

 * *Files identical despite different names*

### Comparing `D47crunch-2.0.3/docs/tutorial.md` & `D47crunch-2.0.4/docs/tutorial.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-## 1. Tutorial
+# 1. Tutorial
 
-### 1.1 Installation
+## 1.1 Installation
 
 The easy option is to use `pip`; open a shell terminal and simply type:
 
 ```
 python -m pip install D47crunch
 ```
 
@@ -20,15 +20,15 @@
 import sys
 sys.path.append('/foo/bar')
 import D47crunch
 ```
 
 Documentation for the development version can be downloaded [here](https://github.com/mdaeron/D47crunch/raw/dev/docs/index.html) (save html file and open it locally).
 
-### 1.2 Usage
+## 1.2 Usage
 
 Start by creating a file named `rawdata.csv` with the following contents:
 
 ```html
 UID,  Sample,           d45,       d46,        d47,        d48,       d49
 A01,  ETH-1,        5.79502,  11.62767,   16.89351,   24.56708,   0.79486
 A02,  MYSAMPLE-1,   6.21907,  11.49107,   17.27749,   24.58270,   1.56318
```

### Comparing `D47crunch-2.0.3/examples/example.py` & `D47crunch-2.0.4/examples/example.py`

 * *Files identical despite different names*

### Comparing `D47crunch-2.0.3/examples/rawdata.csv` & `D47crunch-2.0.4/examples/rawdata.csv`

 * *Files identical despite different names*

### Comparing `D47crunch-2.0.3/license.md` & `D47crunch-2.0.4/license.md`

 * *Files identical despite different names*

### Comparing `D47crunch-2.0.3/pyproject.toml` & `D47crunch-2.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `D47crunch-2.0.3/readme.md` & `D47crunch-2.0.4/readme.md`

 * *Files identical despite different names*

### Comparing `D47crunch-2.0.3/tests/test_D47crunch.py` & `D47crunch-2.0.4/tests/test_D47crunch.py`

 * *Files identical despite different names*

### Comparing `D47crunch-2.0.3/todo.md` & `D47crunch-2.0.4/todo.md`

 * *Files identical despite different names*

### Comparing `D47crunch-2.0.3/PKG-INFO` & `D47crunch-2.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: D47crunch
-Version: 2.0.3
+Version: 2.0.4
 Summary: Standardization and analytical error propagation of Δ47 and Δ48 clumped-isotope measurements
 Author-email: Mathieu Daëron <mathieu@daeron.fr>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

