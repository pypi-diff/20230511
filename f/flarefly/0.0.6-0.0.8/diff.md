# Comparing `tmp/flarefly-0.0.6.tar.gz` & `tmp/flarefly-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarefly-0.0.6.tar", last modified: Fri Jan 27 14:11:10 2023, max compression
+gzip compressed data, was "flarefly-0.0.8.tar", last modified: Thu May 11 07:43:14 2023, max compression
```

## Comparing `flarefly-0.0.6.tar` & `flarefly-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 14:11:10.034211 flarefly-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-27 14:10:55.000000 flarefly-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 14:10:55.000000 flarefly-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-01-27 14:11:10.034211 flarefly-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-01-27 14:10:55.000000 flarefly-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 14:11:10.034211 flarefly-0.0.6/flarefly/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-27 14:10:55.000000 flarefly-0.0.6/flarefly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-01-27 14:10:55.000000 flarefly-0.0.6/flarefly/custom_pdfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12402 2023-01-27 14:10:55.000000 flarefly-0.0.6/flarefly/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    76661 2023-01-27 14:10:55.000000 flarefly-0.0.6/flarefly/fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-01-27 14:10:55.000000 flarefly-0.0.6/flarefly/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 14:11:10.034211 flarefly-0.0.6/flarefly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-01-27 14:11:09.000000 flarefly-0.0.6/flarefly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-01-27 14:11:10.000000 flarefly-0.0.6/flarefly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 14:11:09.000000 flarefly-0.0.6/flarefly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-27 14:11:09.000000 flarefly-0.0.6/flarefly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-01-27 14:11:09.000000 flarefly-0.0.6/flarefly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-27 14:11:09.000000 flarefly-0.0.6/flarefly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 14:11:10.034211 flarefly-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-01-27 14:10:55.000000 flarefly-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:43:14.116884 flarefly-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-11 07:43:01.000000 flarefly-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 07:43:01.000000 flarefly-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-11 07:43:14.116884 flarefly-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-11 07:43:01.000000 flarefly-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:43:14.112884 flarefly-0.0.8/flarefly/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-11 07:43:01.000000 flarefly-0.0.8/flarefly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-11 07:43:01.000000 flarefly-0.0.8/flarefly/custom_pdfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-05-11 07:43:01.000000 flarefly-0.0.8/flarefly/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95113 2023-05-11 07:43:01.000000 flarefly-0.0.8/flarefly/fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-11 07:43:01.000000 flarefly-0.0.8/flarefly/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:43:14.116884 flarefly-0.0.8/flarefly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-11 07:43:14.000000 flarefly-0.0.8/flarefly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-11 07:43:14.000000 flarefly-0.0.8/flarefly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 07:43:14.000000 flarefly-0.0.8/flarefly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 07:43:14.000000 flarefly-0.0.8/flarefly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-11 07:43:14.000000 flarefly-0.0.8/flarefly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 07:43:14.000000 flarefly-0.0.8/flarefly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 07:43:14.116884 flarefly-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-11 07:43:01.000000 flarefly-0.0.8/setup.py
```

### Comparing `flarefly-0.0.6/LICENSE` & `flarefly-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `flarefly-0.0.6/README.md` & `flarefly-0.0.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -9,7 +9,15 @@
 
 # Introduction
 FLexible And REliable Fitting LibrarY is a library to perform fits to distributions for particle physics analysis
 
 # Documentation
 
 [https://flarefly.github.io/flarefly/index.html](https://flarefly.github.io/flarefly/index.html)
+
+## Tutorial
+
+If you want to get familiar with flarefly, the following tutorial is available:
+
+| Type | Link |
+| -------------- | ------------- |
+| Binned invariant mass fit |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/flarefly/flarefly/blob/main/tutorials/flarefly_tutorial_Bzero.ipynb) |
```

### Comparing `flarefly-0.0.6/flarefly/custom_pdfs.py` & `flarefly-0.0.8/flarefly/custom_pdfs.py`

 * *Files identical despite different names*

### Comparing `flarefly-0.0.6/flarefly/data_handler.py` & `flarefly-0.0.8/flarefly/data_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,57 +17,64 @@
 
     def __init__(self, data=None, var_name='', limits=None, use_zfit=True, **kwargs):
         """
         Initialize the DataHandler class
 
         Parameters
         ------------------------------------------------
-        data: numpy array
+        data: numpy.array / pandas.DataFrame / uproot.behaviors.TH1.Histogram / string
             Data or path to data to be used in the fit
         var_name: str
             Name of the variable used in the fit
         limits: list of floats
             Limits of the x axis used in the fit
         use_zfit: bool
             If True, zfit package is used to fit the data
 
         **kwargs: dict
             Additional optional arguments:
 
             - nbins: int
                 Number of bins chosen by user to bin data in case of unbinned data
 
+            - rebin: int
+                Rebin factor in case of binned data
+
             - histoname: str
                 Name of the histogram to be used in the fit in case of ROOT file
 
             - treename: str
                 Name of the tree to be used in the fit in case of ROOT file
         """
         nbins = kwargs.get('nbins', 100)
+        rebin = kwargs.get('rebin', 1)
 
         self._input_ = data
         self._var_name_ = var_name
         self._limits_ = limits if limits is not None else [-1, -1]
         self._use_zfit_ = use_zfit
         self._obs_ = None
         self._data_ = None
         self._binned_data_ = None
         self._nbins_ = nbins
         self._isbinned_ = False
         self._norm_ = 1.
+        self._rebin_ = rebin
 
         if use_zfit:
             if isinstance(data, str):
                 if data.endswith('.root'):
                     self.__format__ = 'root'
                     if 'histoname' in kwargs:
                         hist = uproot.open(data)[kwargs['histoname']]
+                        hist = hist.to_hist()
+                        hist = eval(f"hist[::{self._rebin_}j]") # pylint: disable=eval-used
                         hist_array = hist.to_numpy()
                         if limits is None:
-                            self._binned_data_ = zfit.data.BinnedData.from_hist(hist.to_hist())
+                            self._binned_data_ = zfit.data.BinnedData.from_hist(hist)
                             self._nbins_ = len(hist_array[1]) - 1
                             self._limits_[0] = hist_array[1][0]
                             self._limits_[1] = hist_array[1][-1]
                             idx_min = 0
                             idx_max = len(hist_array[1])-1
                         else:
                             idx_min = np.argmin(np.abs(hist_array[1]-self._limits_[0]))
@@ -79,16 +86,15 @@
                             self._nbins_,
                             self._limits_[0],
                             self._limits_[1],
                             name="xaxis"
                         )
                         self._obs_ = zfit.Space("xaxis", binning=binning)
                         self._binned_data_ = zfit.data.BinnedData.from_tensor(
-                            self._obs_, hist.values()[idx_min:idx_max],
-                            [err**2 for err in hist.errors()[idx_min:idx_max]])
+                            self._obs_, hist.values()[idx_min:idx_max], hist.variances()[idx_min:idx_max])
                         self._isbinned_ = True
                     elif 'treename' in kwargs:
                         input_df = uproot.open(data)[kwargs['treename']].arrays(library='pd')
                         if limits is None:
                             self._limits_[0] = min(input_df[self._var_name_])
                             self._limits_[1] = max(input_df[self._var_name_])
                         self._obs_ = zfit.Space(self._var_name_, limits=(self._limits_[0], self._limits_[1]))
@@ -119,14 +125,43 @@
                 self.__format__ = 'pandas'
                 if limits is None:
                     self._limits_[0] = min(data[self._var_name_])
                     self._limits_[1] = max(data[self._var_name_])
                 self._obs_ = zfit.Space(self._var_name_, limits=(self._limits_[0], self._limits_[1]))
                 self._data_ = zfit.data.Data.from_pandas(obs=self._obs_, df=data)
 
+            elif isinstance(data, uproot.behaviors.TH1.Histogram):
+                self.__format__ = 'uproot'
+                hist = data.to_hist()
+                hist = eval(f"hist[::{self._rebin_}j]") # pylint: disable=eval-used
+                hist_array = hist.to_numpy()
+                if limits is None:
+                    self._binned_data_ = zfit.data.BinnedData.from_hist(hist)
+                    self._nbins_ = len(hist_array[1]) - 1
+                    self._limits_[0] = hist_array[1][0]
+                    self._limits_[1] = hist_array[1][-1]
+                    idx_min = 0
+                    idx_max = len(hist_array[1])-1
+                else:
+                    idx_min = np.argmin(np.abs(hist_array[1]-self._limits_[0]))
+                    idx_max = np.argmin(np.abs(hist_array[1]-self._limits_[1]))
+                    self._nbins_ = len(hist_array[1][idx_min:idx_max])
+                    self._limits_[0] = hist_array[1][idx_min]
+                    self._limits_[1] = hist_array[1][idx_max]
+                binning = zfit.binned.RegularBinning(
+                    self._nbins_,
+                    self._limits_[0],
+                    self._limits_[1],
+                    name="xaxis"
+                )
+                self._obs_ = zfit.Space("xaxis", binning=binning)
+                self._binned_data_ = zfit.data.BinnedData.from_tensor(
+                    self._obs_, hist.values()[idx_min:idx_max], hist.variances()[idx_min:idx_max])
+                self._isbinned_ = True
+
             else:
                 Logger('Data format not supported', 'FATAL')
 
             if self._isbinned_:
                 self._norm_ = float(sum(self._binned_data_.values()))
             else:
                 self._norm_ = float(len(self._data_.to_pandas()))
@@ -311,18 +346,16 @@
         Logger('Data format not supported yet for pandas conversion.', 'ERROR')
         return None
 
     def to_hist(self, **kwargs):
         """
         returns data in NamedHist
 
-        Returns
-        -------------------------------------------------
-        hist: Hist
-            The data in a hist.Hist
+        Parameters
+        ------------------------------------------------
         **kwargs: dict
             Additional optional arguments:
 
             - lower_edge: float
                 lower edge (only used in case of originally unbinned data)
 
             - upper_edge: float
@@ -332,14 +365,19 @@
                 number of bins (only used in case of originally unbinned data)
 
             - axis_title: str
                 label of x-axis (only used in case of originally unbinned data)
 
             - varname: str
                 name of variable (needed in case of originally unbinned data)
+
+        Returns
+        -------------------------------------------------
+        hist: Hist
+            The data in a hist.Hist
         """
 
         if self._isbinned_:
             return self._binned_data_.to_hist()
 
         if 'varname' not in kwargs:
             Logger('Name of variable needed in case of unbinned data.', 'FATAL')
```

### Comparing `flarefly-0.0.6/flarefly/fitter.py` & `flarefly-0.0.8/flarefly/fitter.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 # pylint: disable=too-many-instance-attributes, too-many-lines, too-many-public-methods
 class F2MassFitter:
     """
     Class used to perform mass fits with the zfit library
     https://github.com/zfit/zfit
     """
 
-    def __init__(self, data_handler, name_signal_pdf, name_background_pdf, name="", chi2_loss=False):
+    # pylint: disable=too-many-statements
+    def __init__(self, data_handler, name_signal_pdf, name_background_pdf, **kwargs):
         """
         Initialize the F2MassFitter class
         Parameters
         -------------------------------------------------
         data_handler: flarefly.DataHandler
             The data handler containing the data to fit
 
@@ -50,14 +51,16 @@
 
             - 'kde_grid' (requires to set the datasample and options)
 
             - 'kde_fft' (requires to set the datasample and options)
 
             - 'kde_isj' (requires to set the datasample and options)
 
+            - 'hist' (only for binned fits, requires to set the datasample)
+
         name_background_pdf: list
             The list of names of the background pdfs. The possible options are:
 
             - 'nobkg'
 
             - 'expo'
 
@@ -71,60 +74,94 @@
 
             - 'kde_grid' (requires to set the datasample and options)
 
             - 'kde_fft' (requires to set the datasample and options)
 
             - 'kde_isj' (requires to set the datasample and options)
 
-        name: str
-            Optional name for the fitter,
-            needed in case of multiple fitters defined in the same script
-
-        chi2_loss: bool
-            chi2 minimization if True, nll minmization else
-            Default value to False
+            - 'hist' (only for binned fits, requires to set the datasample)
+
+        **kwargs: dict
+            Additional optional arguments:
+
+            - name_refl_pdf: list
+                The list of names of the signal pdfs. It must have the same length as the signal list.
+                The possible options are:
+
+                - 'kde_exact' (requires to set the datasample and options)
+
+                - 'kde_grid' (requires to set the datasample and options)
+
+                - 'kde_fft' (requires to set the datasample and options)
+
+                - 'kde_isj' (requires to set the datasample and options)
+
+                - 'hist' (only for binned fits, requires to set the datasample)
+
+            - name: str
+                Optional name for the fitter,
+                needed in case of multiple fitters defined in the same script
+
+            - chi2_loss: bool
+                chi2 minimization if True, nll minmization else
+                Default value to False
         """
 
         self._data_handler_ = data_handler
         self._name_signal_pdf_ = name_signal_pdf
         self._name_background_pdf_ = name_background_pdf
         self._signal_pdf_ = [None for _ in enumerate(name_signal_pdf)]
+        self._hist_signal_sample_ = [None for _ in enumerate(name_signal_pdf)]
         self._kde_signal_sample_ = [None for _ in enumerate(name_signal_pdf)]
         self._kde_signal_option_ = [None for _ in enumerate(name_signal_pdf)]
-        if self._name_background_pdf_[0] == "nobkg":
+        if self._name_background_pdf_[0] == 'nobkg':
             self._background_pdf_ = []
+            self._hist_bkg_sample_ = []
             self._kde_bkg_sample_ = []
             self._kde_bkg_option_ = []
         else:
             self._background_pdf_ = [None for _ in enumerate(name_background_pdf)]
+            self._hist_bkg_sample_ = [None for _ in enumerate(name_background_pdf)]
             self._kde_bkg_sample_ = [None for _ in enumerate(name_background_pdf)]
             self._kde_bkg_option_ = [None for _ in enumerate(name_background_pdf)]
+        self._name_refl_pdf_ = kwargs.get('name_refl_pdf', [None for _ in enumerate(name_signal_pdf)])
+        if len(self._name_refl_pdf_) != len(self._name_signal_pdf_):
+            Logger('List of pdfs for signals and reflections different! Exit', 'FATAL')
+        self._refl_pdf_ = [None for _ in enumerate(name_signal_pdf)]
+        self._hist_refl_sample_ = [None for _ in enumerate(name_signal_pdf)]
+        self._kde_refl_sample_ = [None for _ in enumerate(name_signal_pdf)]
+        self._kde_refl_option_ = [None for _ in enumerate(name_signal_pdf)]
+        self._refl_over_sgn_ = [0. for _ in enumerate(name_signal_pdf)]
         self._total_pdf_ = None
         self._total_pdf_binned_ = None
         self._fit_result_ = None
         self._init_sgn_pars_ = [{} for _ in enumerate(name_signal_pdf)]
         self._init_bkg_pars_ = [{} for _ in enumerate(name_signal_pdf)]
         self._limits_sgn_pars_ = [{} for _ in enumerate(name_signal_pdf)]
         self._limits_bkg_pars_ = [{} for _ in enumerate(name_signal_pdf)]
         self._fix_sgn_pars_ = [{} for _ in enumerate(name_signal_pdf)]
         self._fix_bkg_pars_ = [{} for _ in enumerate(name_signal_pdf)]
         self._sgn_pars_ = [{} for _ in enumerate(name_signal_pdf)]
         self._bkg_pars_ = [{} for _ in enumerate(name_background_pdf)]
-        if self._name_background_pdf_[0] == "nobkg":
-            self._fracs_ = [None for _ in range(len(name_signal_pdf) - 1)]
+        if self._name_background_pdf_[0] == 'nobkg':
+            self._fracs_ = [None for _ in range(2 * len(name_signal_pdf) - 1)]
         else:
-            self._fracs_ = [None for _ in range(len(name_signal_pdf) + len(name_background_pdf) - 1)]
+            self._fracs_ = [None for _ in range(2 * len(name_signal_pdf) + len(name_background_pdf) - 1)]
         self._rawyield_ = [0. for _ in enumerate(name_signal_pdf)]
         self._rawyield_err_ = [0. for _ in enumerate(name_signal_pdf)]
         self._minimizer_ = zfit.minimize.Minuit(verbosity=7)
-        self._name_ = name
+        self._name_ = kwargs.get('name', '')
         self._ndf_ = None
-        self._chi2_loss_ = chi2_loss
+        self._chi2_loss_ = kwargs.get('chi2_loss', False)
         self._base_sgn_cmap_ = plt.cm.get_cmap('viridis', len(self._signal_pdf_) * 4)
         self._sgn_cmap_ = ListedColormap(self._base_sgn_cmap_(np.linspace(0.4, 0.65, len(self._signal_pdf_))))
+        self._base_bkg_cmap_ = plt.cm.get_cmap('gist_heat', len(self._background_pdf_) * 2)
+        self._bkg_cmap_ = ListedColormap(self._base_bkg_cmap_(np.linspace(0.3, 0.8, len(self._background_pdf_))))
+        self._base_refl_cmap_ = plt.cm.get_cmap('summer', len(self._refl_pdf_) * 2)
+        self._refl_cmap_ = ListedColormap(self._base_refl_cmap_(np.linspace(0., 0.6, len(self._refl_pdf_))))
 
         zfit.settings.advanced_warnings.all = False
         zfit.settings.changed_warnings.all = False
 
     # pylint: disable=too-many-branches, too-many-statements
     def __build_signal_pdfs(self, obs):
         """
@@ -344,14 +381,24 @@
                     elif pdf_name == 'kde_isj':
                         self._signal_pdf_[ipdf] = zfit.pdf.KDE1DimISJ(self._kde_signal_sample_[ipdf].get_data(),
                                                                       obs=self._kde_signal_sample_[ipdf].get_obs(),
                                                                       name=f'{self._name_}_kde_signal{ipdf}',
                                                                       **self._kde_signal_option_[ipdf])
                 else:
                     Logger(f'Missing datasample for Kernel Density Estimation of signal {ipdf}!', 'FATAL')
+            elif pdf_name == 'hist':
+                if self._hist_signal_sample_[ipdf]:
+                    self._signal_pdf_[ipdf] = zfit.pdf.SplinePDF(
+                        zfit.pdf.HistogramPDF(self._hist_signal_sample_[ipdf].get_binned_data(),
+                                              name=f'{self._name_}_hist_signal{ipdf}'),
+                        order=3,
+                        obs=obs
+                    )
+                else:
+                    Logger(f'Missing datasample for histogram template of signal {ipdf}!', 'FATAL')
             else:
                 Logger(f'Signal pdf {pdf_name} not supported', 'FATAL')
 
     def __build_background_pdfs(self, obs):
         """
         Helper function to compose the background pdfs
         """
@@ -453,29 +500,95 @@
                         self._background_pdf_[ipdf] = zfit.pdf.KDE1DimISJ(self._kde_bkg_sample_[ipdf].get_data(),
                                                                           obs=self._kde_bkg_sample_[ipdf].get_obs(),
                                                                           name=f'{self._name_}_kde_bkg{ipdf}',
                                                                           **self._kde_bkg_option_[ipdf])
 
                 else:
                     Logger(f'Missing datasample for Kernel Density Estimation of background {ipdf}!', 'FATAL')
+            elif pdf_name == 'hist':
+                if self._hist_bkg_sample_[ipdf]:
+                    self._background_pdf_[ipdf] = zfit.pdf.SplinePDF(
+                        zfit.pdf.HistogramPDF(self._hist_bkg_sample_[ipdf].get_binned_data(),
+                                              name=f'{self._name_}_hist_background{ipdf}'),
+                        order=3,
+                        obs=obs
+                    )
+                else:
+                    Logger(f'Missing datasample for histogram template of background {ipdf}!', 'FATAL')
             else:
                 Logger(f'Background pdf {pdf_name} not supported', 'FATAL')
 
+    # pylint: disable=too-many-branches, too-many-statements
+    def __build_reflection_pdfs(self, obs):
+        """
+        Helper function to compose the reflection pdfs
+        """
+
+        for ipdf, pdf_name in enumerate(self._name_refl_pdf_):
+            if pdf_name is None: # by default we put a dummy pdf
+                low = zfit.Parameter(f'{self._name_}_low_refl{ipdf}',
+                                     self._data_handler_.get_limits()[0],
+                                     self._data_handler_.get_limits()[0]*0.99,
+                                     self._data_handler_.get_limits()[0]*1.01,
+                                     floating=False)
+                high = zfit.Parameter(f'{self._name_}_high_refl{ipdf}',
+                                      self._data_handler_.get_limits()[1],
+                                      self._data_handler_.get_limits()[1]*0.99,
+                                      self._data_handler_.get_limits()[1]*1.01,
+                                      floating=False)
+                self._refl_pdf_[ipdf] = zfit.pdf.Uniform(obs=obs, low=low, high=high)
+            elif 'kde' in pdf_name:
+                if self._kde_refl_sample_[ipdf]:
+                    if pdf_name == 'kde_exact':
+                        self._refl_pdf_[ipdf] = zfit.pdf.KDE1DimExact(self._kde_refl_sample_[ipdf].get_data(),
+                                                                      obs=self._kde_refl_sample_[ipdf].get_obs(),
+                                                                      name=f'{self._name_}_kde_refl{ipdf}',
+                                                                      **self._kde_refl_option_[ipdf])
+                    elif pdf_name == 'kde_grid':
+                        self._refl_pdf_[ipdf] = zfit.pdf.KDE1DimGrid(self._kde_refl_sample_[ipdf].get_data(),
+                                                                     obs=self._kde_refl_sample_[ipdf].get_obs(),
+                                                                     name=f'{self._name_}_kde_refl{ipdf}',
+                                                                     **self._kde_refl_option_[ipdf])
+                    elif pdf_name == 'kde_fft':
+                        self._refl_pdf_[ipdf] = zfit.pdf.KDE1DimFFT(self._kde_refl_sample_[ipdf].get_data(),
+                                                                    obs=self._kde_refl_sample_[ipdf].get_obs(),
+                                                                    name=f'{self._name_}_kde_refl{ipdf}',
+                                                                    **self._kde_refl_option_[ipdf])
+                    elif pdf_name == 'kde_isj':
+                        self._refl_pdf_[ipdf] = zfit.pdf.KDE1DimISJ(self._kde_refl_sample_[ipdf].get_data(),
+                                                                    obs=self._kde_refl_sample_[ipdf].get_obs(),
+                                                                    name=f'{self._name_}_kde_refl{ipdf}',
+                                                                    **self._kde_refl_option_[ipdf])
+                else:
+                    Logger(f'Missing datasample for Kernel Density Estimation of reflection {ipdf}!', 'FATAL')
+            elif pdf_name == 'hist':
+                if self._hist_refl_sample_[ipdf]:
+                    self._refl_pdf_[ipdf] = zfit.pdf.SplinePDF(
+                        zfit.pdf.HistogramPDF(self._hist_refl_sample_[ipdf].get_binned_data(),
+                                              name=f'{self._name_}_hist_refl{ipdf}'),
+                        order=3,
+                        obs=obs
+                    )
+                else:
+                    Logger(f'Missing datasample for histogram template of reflections {ipdf}!', 'FATAL')
+            else:
+                Logger(f'Reflection pdf {pdf_name} not supported', 'FATAL')
 
     def __build_total_pdf(self):
         """
         Helper function to compose the total pdf
         """
 
         obs = self._data_handler_.get_obs()
 
         # order of the pdfs is signal, background
 
         self.__build_signal_pdfs(obs)
         self.__build_background_pdfs(obs)
+        self.__build_reflection_pdfs(obs)
 
         if len(self._signal_pdf_) + len(self._background_pdf_) == 1:
             self._total_pdf_ = self._signal_pdf_[0]
             return
 
         for ipdf, _ in enumerate(self._signal_pdf_):
             self._init_sgn_pars_[ipdf].setdefault('frac', 0.1)
@@ -485,28 +598,36 @@
                 continue
             self._fracs_[ipdf] = zfit.Parameter(f'{self._name_}_frac_signal{ipdf}',
                                                 self._init_sgn_pars_[ipdf]['frac'],
                                                 self._limits_sgn_pars_[ipdf]['frac'][0],
                                                 self._limits_sgn_pars_[ipdf]['frac'][1],
                                                 floating=not self._fix_sgn_pars_[ipdf]['frac'])
 
+            # normalisation of reflection fixed to the one of the signal
+            def func_mult(params):
+                return params['ros'] * params['s']
+            self._fracs_[ipdf + len(self._signal_pdf_)] = zfit.ComposedParameter(
+                f'{self._name_}_frac_refl{ipdf}',
+                func_mult, params={'ros' : self._refl_over_sgn_[ipdf],
+                                   's' : self._fracs_[ipdf]}
+            )
+
         if len(self._background_pdf_) > 1:
             for ipdf, _ in enumerate(self._background_pdf_):
                 self._init_bkg_pars_[ipdf].setdefault('frac', 0.1)
                 self._fix_bkg_pars_[ipdf].setdefault('frac', False)
                 self._limits_bkg_pars_[ipdf].setdefault('frac', [0, 1.])
-                self._fracs_[ipdf + len(self._signal_pdf_)] = zfit.Parameter(
+                self._fracs_[ipdf + 2 * len(self._signal_pdf_)] = zfit.Parameter(
                     f'{self._name_}_frac_bkg{ipdf}',
                     self._init_bkg_pars_[ipdf]['frac'],
                     self._limits_bkg_pars_[ipdf]['frac'][0],
                     self._limits_bkg_pars_[ipdf]['frac'][1],
                     floating=not self._fix_bkg_pars_[ipdf]['frac'])
 
-        self._total_pdf_ = zfit.pdf.SumPDF(
-            self._signal_pdf_+self._background_pdf_, self._fracs_)
+        self._total_pdf_ = zfit.pdf.SumPDF(self._signal_pdf_+self._refl_pdf_+self._background_pdf_, self._fracs_)
 
     def __build_total_pdf_binned(self):
         """
         Helper function to compose the total pdf binned from unbinned
         """
 
         # for binned data, obs already contains the wanted binning
@@ -532,30 +653,43 @@
 
         Returns
         -------------------------------------------------
         signal_fracs: list
             fractions of the signal pdfs
         background_fracs: list
             fractions of the background pdfs
+        refl_fracs: list
+            fractions of the reflected signal pdfs
         signal_err_fracs: list
             errors of fractions of the signal pdfs
         bkg_err_fracs: list
             errors of fractions of the background pdfs
+        refl_err_fracs: list
+            errors of fractions of the reflected signal pdfs
         """
-        signal_fracs, bkg_fracs, signal_err_fracs, bkg_err_fracs = ([] for _ in range(4))
+        signal_fracs, bkg_fracs, refl_fracs, signal_err_fracs, bkg_err_fracs, refl_err_fracs = ([] for _ in range(6))
         for frac_par in self._fracs_:
+            if frac_par is None:
+                continue
             par_name = frac_par.name
             if f'{self._name_}_frac_signal' in par_name:
                 signal_fracs.append(self._fit_result_.params[par_name]['value'])
                 signal_err_fracs.append(self._fit_result_.params[par_name]['hesse']['error'])
+                isgn = int(par_name.split(sep=f'{self._name_}_frac_signal')[-1])
+                refl_fracs.append(signal_fracs[-1] * self._refl_over_sgn_[isgn])
+                refl_err_fracs.append(signal_err_fracs[-1] * self._refl_over_sgn_[isgn])
             elif f'{self._name_}_frac_bkg' in par_name:
                 bkg_fracs.append(self._fit_result_.params[par_name]['value'])
                 bkg_err_fracs.append(self._fit_result_.params[par_name]['hesse']['error'])
 
-        return signal_fracs, bkg_fracs, signal_err_fracs, bkg_err_fracs
+        if len(signal_fracs) == len(bkg_fracs) == len(refl_fracs) == 0:
+            signal_fracs.append(1.)
+            signal_err_fracs.append(0.)
+
+        return signal_fracs, bkg_fracs, refl_fracs, signal_err_fracs, bkg_err_fracs, refl_err_fracs
 
     def mass_zfit(self):
         """
         Perform a mass fit with the zfit library
 
         Returns
         -------------------------------------------------
@@ -570,31 +704,28 @@
         self.__build_total_pdf_binned()
         # pylint: disable=fixme
         self.__prefit() #TODO: implement me
 
         if self._data_handler_.get_is_binned():
             # chi2 loss
             if self._chi2_loss_:
-                loss = zfit.loss.BinnedChi2(self._total_pdf_binned_,
-                                            self._data_handler_.get_binned_data())
+                loss = zfit.loss.BinnedChi2(self._total_pdf_binned_, self._data_handler_.get_binned_data())
             # nll loss
             else:
-                loss = zfit.loss.BinnedNLL(self._total_pdf_binned_,
-                                            self._data_handler_.get_binned_data())
+                loss = zfit.loss.BinnedNLL(self._total_pdf_binned_, self._data_handler_.get_binned_data())
         else:
-            loss = zfit.loss.UnbinnedNLL(
-                model=self._total_pdf_, data=self._data_handler_.get_data())
+            loss = zfit.loss.UnbinnedNLL(model=self._total_pdf_, data=self._data_handler_.get_data())
 
         self._fit_result_ = self._minimizer_.minimize(loss=loss)
+        Logger(self._fit_result_, 'RESULT')
+
         if self._fit_result_.hesse() == {}:
             if self._fit_result_.hesse(method='hesse_np') == {}:
                 Logger('Impossible to compute hesse error', 'FATAL')
 
-        Logger(self._fit_result_, 'RESULT')
-
         norm = self._data_handler_.get_norm()
         if len(self._fracs_) == 0:
             self._rawyield_ = self._data_handler_.get_norm()
             self._rawyield_err_ = np.sqrt(self._rawyield_)
         else:
             for ipdf, _ in enumerate(self._signal_pdf_):
                 if len(self._background_pdf_) > 0 or ipdf < len(self._signal_pdf_) - 1:
@@ -633,22 +764,25 @@
             - figsize: tuple
                 size of the figure
 
             - axis_title: str
                 x-axis title
 
             - show_extra_info: bool
-                show chi2/ndf, signal, bkg, signal/bkg, significance
+                show mu, sigma, chi2/ndf, signal, bkg, signal/bkg, significance
 
-            - extra_info_massrange: list
-                mass range limits for extra info
-
-            - extra_info_masssigma: float
+            - extra_info_massnsigma: float
                 number of sigmas for extra info
 
+            - extra_info_massnhwhm: float
+                number of hwhms for extra info (alternative to extra_info_massnsigma)
+
+            - extra_info_massrange: list
+                mass range limits for extra info (alternative to extra_info_massnsigma)
+
             - extra_info_loc: list
                 location of extra info (one for chi2 and one for other info)
 
             - num: int
                 number of bins to plot pdfs converted into histograms
 
         Returns
@@ -661,15 +795,16 @@
         logy = kwargs.get('logy', False)
         figsize = kwargs.get('figsize', (7, 7))
         bins = self._data_handler_.get_nbins()
         axis_title = kwargs.get('axis_title', self._data_handler_.get_var_name())
         show_extra_info = kwargs.get('show_extra_info', False)
         num = kwargs.get('num', 10000)
         mass_range = kwargs.get('extra_info_massrange', None)
-        nsigma = kwargs.get('extra_info_masssigma', 3)
+        nhwhm = kwargs.get('extra_info_massnhwhm', None)
+        nsigma = kwargs.get('extra_info_massnsigma', 3)
         loc = kwargs.get('extra_info_loc', ['upper left', 'lower right'])
 
         mplhep.style.use(style)
 
         obs = self._data_handler_.get_obs()
         limits = self._data_handler_.get_limits()
 
@@ -682,44 +817,46 @@
 
         hdata.plot(yerr=True, color='black', histtype='errorbar', label='data')
         bin_sigma = (limits[1] - limits[0]) / bins
         norm = self._data_handler_.get_norm() * bin_sigma
 
         x_plot = np.linspace(limits[0], limits[1], num=num)
         total_func = zfit.run(self._total_pdf_.pdf(x_plot, norm_range=obs))
-        signal_funcs, signal_fracs, bkg_funcs, bkg_fracs = ([] for _ in range(4))
+        signal_funcs, refl_funcs, bkg_funcs = ([] for _ in range(3))
         for signal_pdf in self._signal_pdf_:
             signal_funcs.append(zfit.run(signal_pdf.pdf(x_plot, norm_range=obs)))
+        for refl_pdf in self._refl_pdf_:
+            refl_funcs.append(zfit.run(refl_pdf.pdf(x_plot, norm_range=obs)))
         for bkg_pdf in self._background_pdf_:
             bkg_funcs.append(zfit.run(bkg_pdf.pdf(x_plot, norm_range=obs)))
-        for frac_par in self._fracs_:
-            par_name = frac_par.name
-            if f'{self._name_}_frac_signal' in par_name:
-                signal_fracs.append(self._fit_result_.params[par_name]['value'])
-            elif f'{self._name_}_frac_bkg' in par_name:
-                bkg_fracs.append(self._fit_result_.params[par_name]['value'])
-        if len(signal_fracs) == 0:
-            signal_fracs.append(1.)
+
+        signal_fracs, bkg_fracs, refl_fracs, _, _, _ = self.__get_all_fracs()
 
         # first draw backgrounds
-        base_bkg_cmap = plt.cm.get_cmap('gist_heat', len(bkg_funcs) * 2)
-        bkg_cmap = ListedColormap(base_bkg_cmap(np.linspace(0.3, 0.8, len(bkg_funcs))))
         for ibkg, bkg_func in enumerate(bkg_funcs):
             if ibkg < len(bkg_fracs) - 1:
-                plt.plot(x_plot, bkg_func * norm * bkg_fracs[ibkg], color=bkg_cmap(ibkg),
+                plt.plot(x_plot, bkg_func * norm * bkg_fracs[ibkg], color=self._bkg_cmap_(ibkg),
                          ls='--', label=f'background {ibkg}')
             else:
-                plt.plot(x_plot, bkg_func * norm * (1-sum(bkg_fracs)-sum(signal_fracs)),
+                plt.plot(x_plot, bkg_func * norm * (1-sum(bkg_fracs)-sum(signal_fracs)-sum(refl_fracs)),
                          color='firebrick', ls='--', label=f'background {ibkg}')
         # then draw signals
-        for isgn, (frac, signal_func) in enumerate(zip(signal_funcs, signal_fracs)):
+        for isgn, (signal_func, frac) in enumerate(zip(signal_funcs, signal_fracs)):
             plt.plot(x_plot, signal_func * norm * frac, color=self._sgn_cmap_(isgn))
             plt.fill_between(x_plot, signal_func * norm * frac, color=self._sgn_cmap_(isgn),
                              alpha=0.5, label=f'signal {isgn}')
 
+        # finally draw reflected signals (if any)
+        for irefl, (refl_func, frac) in enumerate(zip(refl_funcs, refl_fracs)):
+            if self._name_refl_pdf_[irefl] is None:
+                continue
+            plt.plot(x_plot, refl_func * norm * frac, color=self._refl_cmap_(irefl))
+            plt.fill_between(x_plot, refl_func * norm * frac, color=self._refl_cmap_(irefl),
+                             alpha=0.5, label=f'reflected signal {irefl}')
+
         plt.plot(x_plot, total_func * norm, color='xkcd:blue', label='total fit')
         plt.xlim(limits[0], limits[1])
         plt.xlabel(axis_title)
         plt.ylabel(rf'counts / {(limits[1]-limits[0])/bins*1000:0.1f} MeV/$c^2$')
         plt.legend(loc='best')
         if logy:
             plt.yscale('log')
@@ -731,37 +868,57 @@
             ndf = self.get_ndf()
             anchored_text_chi2 = AnchoredText(fr'$\chi^2 / \mathrm{{ndf}} =${chi2:.2f} / {ndf}',
                                               loc = loc[0],
                                               frameon=False)
             # signal and background info for all signals
             text = []
             for idx, _ in enumerate(self._name_signal_pdf_):
+                mass, mass_unc = self.get_mass(idx)
+                sigma, sigma_unc = None, None
+                gamma, gamma_unc = None, None
+                if self._name_signal_pdf_[idx] in ['gaussian', 'crystalball', 'voigtian', 'hist']:
+                    sigma, sigma_unc = self.get_sigma(idx)
+                if self._name_signal_pdf_[idx] in ['cauchy', 'voigtian']:
+                    gamma, gamma_unc = self.get_signal_parameter(idx, 'gamma')
+                extra_info = fr'signal{idx}''\n' + fr'  $\mu = {mass*1000:.1f}\pm{mass_unc*1000:.1f}$ MeV$/c^2$''\n'
+                if sigma is not None:
+                    extra_info += fr'  $\sigma = {sigma*1000:.1f}\pm{sigma_unc*1000:.1f}$ MeV$/c^2$''\n'
+                if gamma is not None:
+                    extra_info += fr'  $\Gamma = {gamma*1000:.1f}\pm{gamma_unc*1000:.1f}$ MeV$/c^2$''\n'
                 if mass_range is not None:
                     signal, signal_err = self.get_signal(idx=idx, min=mass_range[0], max=mass_range[1])
                     bkg, bkg_err = self.get_background(idx=idx, min=mass_range[0], max=mass_range[1])
                     s_over_b, s_over_b_err = self.get_signal_over_background(idx=idx, min=mass_range[0],
                                                                              max=mass_range[1])
-                    significance, significance_err = self.get_significance(idx=idx, min=mass_range[0],
+                    signif, signif_err = self.get_significance(idx=idx, min=mass_range[0],
                                                                            max=mass_range[1])
                     interval = f'[{mass_range[0]:.3f}, {mass_range[1]:.3f}]'
-                    text.append(fr'signal{idx}''\n'
-                            fr'  $S({interval})={signal:.0f} \pm {signal_err:.0f}$''\n'
-                            fr'  $B({interval})={bkg:.0f} \pm {bkg_err:.0f}$''\n'
-                            fr'  $S/B({interval})={s_over_b:.2f} \pm {s_over_b_err:.2f}$''\n'
-                            fr'  Signif.$({interval})={significance:.1f} \pm {significance_err:.1f}$')
+                    extra_info += fr'  $S({interval})={signal:.0f} \pm {signal_err:.0f}$''\n'
+                    extra_info += fr'  $B({interval})={bkg:.0f} \pm {bkg_err:.0f}$''\n'
+                    extra_info += fr'  $S/B({interval})={s_over_b:.2f} \pm {s_over_b_err:.2f}$''\n'
+                    extra_info += fr'  Signif.$({interval})={signif:.1f} \pm {signif_err:.1f}$'
+                elif nhwhm is not None:
+                    signal, signal_err = self.get_signal(idx=idx, nhwhm=nhwhm)
+                    bkg, bkg_err = self.get_background(idx=idx, nhwhm=nhwhm)
+                    s_over_b, s_over_b_err = self.get_signal_over_background(idx=idx, nhwhm=nhwhm)
+                    signif, signif_err = self.get_significance(idx=idx, nhwhm=nhwhm)
+                    extra_info += fr'  $S=${signal:.0f} $\pm$ {signal_err:.0f}''\n'
+                    extra_info += fr'  $B({nhwhm}~\mathrm{{HWHM}})=${bkg:.0f} $\pm$ {bkg_err:.0f}''\n'
+                    extra_info += fr'  $S/B({nhwhm}~\mathrm{{HWHM}})=${s_over_b:.2f} $\pm$ {s_over_b_err:.2f}''\n'
+                    extra_info += fr'  Signif.$({nhwhm}~\mathrm{{HWHM}})=${signif:.1f} $\pm$ {signif_err:.1f}'
                 else:
                     signal, signal_err = self.get_signal(idx=idx, nsigma=nsigma)
                     bkg, bkg_err = self.get_background(idx=idx, nsigma=nsigma)
                     s_over_b, s_over_b_err = self.get_signal_over_background(idx=idx, nsigma=nsigma)
-                    significance, significance_err = self.get_significance(idx=idx, nsigma=nsigma)
-                    text.append(fr'signal{idx}''\n'
-                                fr'  $S=${signal:.0f} $\pm$ {signal_err:.0f}''\n'
-                                fr'  $B({nsigma}\sigma)=${bkg:.0f} $\pm$ {bkg_err:.0f}''\n'
-                                fr'  $S/B({nsigma}\sigma)=${s_over_b:.2f} $\pm$ {s_over_b_err:.2f}''\n'
-                                fr'  Signif.$({nsigma}\sigma)=${significance:.1f} $\pm$ {significance_err:.1f}')
+                    signif, signif_err = self.get_significance(idx=idx, nsigma=nsigma)
+                    extra_info += fr'  $S=${signal:.0f} $\pm$ {signal_err:.0f}''\n'
+                    extra_info += fr'  $B({nsigma}\sigma)=${bkg:.0f} $\pm$ {bkg_err:.0f}''\n'
+                    extra_info += fr'  $S/B({nsigma}\sigma)=${s_over_b:.2f} $\pm$ {s_over_b_err:.2f}''\n'
+                    extra_info += fr'  Signif.$({nsigma}\sigma)=${signif:.1f} $\pm$ {signif_err:.1f}'
+                text.append(extra_info)
             concatenated_text = '\n'.join(text)
             anchored_text_signal = AnchoredText(concatenated_text, loc = loc[1], frameon=False)
 
             axs.add_artist(anchored_text_chi2)
             axs.add_artist(anchored_text_signal)
 
         return fig
@@ -809,47 +966,51 @@
 
         bin_sigma = (limits[1] - limits[0]) / bins
         norm = self._data_handler_.get_norm() * bin_sigma
         x_plot = np.linspace(limits[0], limits[1], num=num)
 
         total_func = zfit.run(self._total_pdf_.pdf(x_plot, norm_range=obs))
         # write total_func
-        self.__write_pdf(histname=f'total_func{suffix}', weight=total_func, num=num,
+        self.__write_pdf(histname=f'total_func{suffix}', weight=total_func * norm, num=num,
                          filename=filename, option='update')
 
-        signal_funcs, signal_fracs, bkg_funcs, bkg_fracs = ([] for _ in range(4))
+        signal_funcs, bkg_funcs, refl_funcs = ([] for _ in range(3))
         for signal_pdf in self._signal_pdf_:
             signal_funcs.append(zfit.run(signal_pdf.pdf(x_plot, norm_range=obs)))
+        for refl_pdf in self._refl_pdf_:
+            refl_funcs.append(zfit.run(refl_pdf.pdf(x_plot, norm_range=obs)))
         for bkg_pdf in self._background_pdf_:
             bkg_funcs.append(zfit.run(bkg_pdf.pdf(x_plot, norm_range=obs)))
-        for frac_par in self._fracs_:
-            par_name = frac_par.name
-            if f'{self._name_}_frac_signal' in par_name:
-                signal_fracs.append(self._fit_result_.params[par_name]['value'])
-            elif f'{self._name_}_frac_bkg' in par_name:
-                bkg_fracs.append(self._fit_result_.params[par_name]['value'])
-        if len(signal_fracs) == 0:
-            signal_fracs.append(1.)
+
+        signal_fracs, bkg_fracs, refl_fracs, _, _, _ = self.__get_all_fracs()
 
         # first write backgrounds
         for ibkg, bkg_func in enumerate(bkg_funcs):
             if ibkg < len(bkg_fracs) - 1:
                 self.__write_pdf(histname=f'bkg_{ibkg}{suffix}',
                                  weight=bkg_func * norm * bkg_fracs[ibkg],
                                  num=num, filename=filename, option='update')
             else:
                 self.__write_pdf(histname=f'bkg_{ibkg}{suffix}',
-                               weight=bkg_func * norm * (1-sum(bkg_fracs)-sum(signal_fracs)),
+                               weight=bkg_func * norm * (1-sum(bkg_fracs)-sum(signal_fracs)-sum(refl_fracs)),
                                num=num, filename=filename, option='update')
         # then write signals
         for isgn, (frac, signal_func) in enumerate(zip(signal_funcs, signal_fracs)):
             self.__write_pdf(histname=f'signal_{isgn}{suffix}',
                            weight=signal_func * norm * frac,
                            num=num, filename=filename, option='update')
 
+        # finally write reflected signals
+        for irefl, (frac, refl_func) in enumerate(zip(refl_funcs, refl_fracs)):
+            if self._name_refl_pdf_[irefl] is None:
+                continue
+            self.__write_pdf(histname=f'refl_{irefl}{suffix}',
+                           weight=refl_func * norm * frac,
+                           num=num, filename=filename, option='update')
+
     @property
     def get_fit_result(self):
         """
         Get the fit result
 
         Returns
         -------------------------------------------------
@@ -950,18 +1111,18 @@
         else:
             data_values = self._data_handler_.get_binned_data_from_unbinned_data()
             variances = data_values # poissonian errors
             obs = self._data_handler_.get_binned_obs_from_unbinned_data()
 
         # get background fractions
         if len(self._background_pdf_) == 1:
-            signal_fracs, _, _, _ = self.__get_all_fracs()
-            bkg_fracs = [1 - sum(signal_fracs)]
+            signal_fracs, _, refl_fracs, _, _, _ = self.__get_all_fracs()
+            bkg_fracs = [1 - sum(signal_fracs) - sum(refl_fracs)]
         else:
-            _, bkg_fracs, _, _ = self.__get_all_fracs()
+            _, bkg_fracs, _, _, _, _ = self.__get_all_fracs()
         # access model predicted values for background
         for ipdf, _ in enumerate(self._name_background_pdf_):
             background_pdf_binned_[ipdf] = zfit.pdf.BinnedFromUnbinnedPDF(self._background_pdf_[ipdf], obs)
             model_bkg_values[ipdf] = background_pdf_binned_[ipdf].values()*bkg_fracs[ipdf]*norm
         # compute residuals
         for ibin, data in enumerate(data_values):
             residuals[ibin] = float(data)
@@ -1021,30 +1182,46 @@
             label = "residuals"
         )
         bins = self._data_handler_.get_nbins()
         bin_sigma = (limits[1] - limits[0]) / bins
         norm = self._data_handler_.get_norm() * bin_sigma
 
         x_plot = np.linspace(limits[0], limits[1], num=1000)
-        signal_funcs, signal_fracs, _, _ = ([] for _ in range(4))
+        signal_funcs, refl_funcs = ([] for _ in range(2))
         for signal_pdf in self._signal_pdf_:
             signal_funcs.append(zfit.run(signal_pdf.pdf(x_plot, norm_range=obs)))
-        for frac_par in self._fracs_:
-            par_name = frac_par.name
-            if f'{self._name_}_frac_signal' in par_name:
-                signal_fracs.append(self._fit_result_.params[par_name]['value'])
-        if len(signal_fracs) == 0:
-            signal_fracs.append(1.)
+        for refl_pdf in self._refl_pdf_:
+            refl_funcs.append(zfit.run(refl_pdf.pdf(x_plot, norm_range=obs)))
+
+        signal_fracs, _, refl_fracs, _, _, _ = self.__get_all_fracs()
 
         # draw signals
         for isgn, (signal_func, frac) in enumerate(zip(signal_funcs, signal_fracs)):
             plt.plot(x_plot, signal_func * norm * frac, color=self._sgn_cmap_(isgn))
             plt.fill_between(x_plot, signal_func * norm * frac, color=self._sgn_cmap_(isgn),
                              alpha=0.5, label=f'signal {isgn}')
 
+        # finally draw reflected signals (if any)
+        is_there_refl = False
+        for irefl, (refl_func, frac) in enumerate(zip(refl_funcs, refl_fracs)):
+            if self._name_refl_pdf_[irefl] is None:
+                continue
+            is_there_refl = True
+            plt.plot(x_plot, refl_func * norm * frac, color=self._refl_cmap_(irefl))
+            plt.fill_between(x_plot, refl_func * norm * frac, color=self._refl_cmap_(irefl),
+                             alpha=0.5, label=f'reflected signal {irefl}')
+
+        # draw signal + reflected signals (if any)
+        if is_there_refl:
+            for isgn, (signal_func, refl_func, frac_sgn, frac_refl) in enumerate(
+                zip(signal_funcs, refl_funcs, signal_fracs, refl_fracs)):
+                plt.plot(x_plot, (signal_func * frac_sgn + frac_refl * refl_func) * norm,
+                        color='xkcd:blue', label='total - bkg')
+
+
         plt.xlim(limits[0], limits[1])
         plt.xlabel(axis_title)
         plt.ylabel(rf'(data - fitted bkg) / {(limits[1]-limits[0])/bins*1000:0.1f} MeV/$c^2$')
         plt.legend(loc='best')
 
         return fig
 
@@ -1177,21 +1354,29 @@
         Returns
         -------------------------------------------------
         mass: float
             The mass value obtained from the fit
         mass_err: float
             The mass error obtained from the fit
         """
-        mass_name = 'm' if self._name_signal_pdf_[idx] == 'cauchy' else 'mu'
-        if self._fix_sgn_pars_[idx][mass_name]:
-            mass = self._init_sgn_pars_[idx][mass_name]
+        if 'hist' in self._name_signal_pdf_[idx]:
+            hist = self._signal_pdf_[idx].to_hist()
+            bin_limits = hist.to_numpy()[1]
+            centres = [0.5 * (minn + maxx) for minn, maxx in zip(bin_limits[1:],  bin_limits[:-1])]
+            counts = hist.values()
+            mass = np.average(centres, weights=counts)
             mass_err = 0.
         else:
-            mass = self._fit_result_.params[f'{self._name_}_{mass_name}_signal{idx}']['value']
-            mass_err = self._fit_result_.params[f'{self._name_}_{mass_name}_signal{idx}']['hesse']['error']
+            mass_name = 'm' if self._name_signal_pdf_[idx] == 'cauchy' else 'mu'
+            if self._fix_sgn_pars_[idx][mass_name]:
+                mass = self._init_sgn_pars_[idx][mass_name]
+                mass_err = 0.
+            else:
+                mass = self._fit_result_.params[f'{self._name_}_{mass_name}_signal{idx}']['value']
+                mass_err = self._fit_result_.params[f'{self._name_}_{mass_name}_signal{idx}']['hesse']['error']
 
         return mass, mass_err
 
     def get_sigma(self, idx=0):
         """
         Get the sigma and its error
 
@@ -1203,27 +1388,79 @@
         Returns
         -------------------------------------------------
         sigma: float
             The sigma value obtained from the fit
         sigma_err: float
             The sigma error obtained from the fit
         """
-        if self._name_signal_pdf_[idx] not in ['gaussian', 'crystalball']:
+        if self._name_signal_pdf_[idx] not in ['gaussian', 'crystalball', 'voigtian', 'hist']:
             Logger(f'Sigma parameter not defined for {self._name_signal_pdf_[idx]} pdf!', 'ERROR')
             return 0., 0.
 
-        if self._fix_sgn_pars_[idx]['sigma']:
-            sigma = self._init_sgn_pars_[idx]['sigma']
+        # if histogram, the rms is used as proxy
+        if 'hist' in self._name_signal_pdf_[idx]:
+            Logger(f'RMS used as proxy for sigma parameter of {self._name_signal_pdf_[idx]} pdf!', 'WARNING')
+            mean = self.get_mass(idx)[0]
+            hist = self._signal_pdf_[idx].to_hist()
+            bin_limits = hist.to_numpy()[1]
+            centres = [0.5 * (minn + maxx) for minn, maxx in zip(bin_limits[1:],  bin_limits[:-1])]
+            counts = hist.values()
+            sigma = np.sqrt(np.average((centres - mean)**2, weights=counts))
             sigma_err = 0.
         else:
-            sigma = self._fit_result_.params[f'{self._name_}_sigma_signal{idx}']['value']
-            sigma_err = self._fit_result_.params[f'{self._name_}_sigma_signal{idx}']['hesse']['error']
+            if self._fix_sgn_pars_[idx]['sigma']:
+                sigma = self._init_sgn_pars_[idx]['sigma']
+                sigma_err = 0.
+            else:
+                sigma = self._fit_result_.params[f'{self._name_}_sigma_signal{idx}']['value']
+                sigma_err = self._fit_result_.params[f'{self._name_}_sigma_signal{idx}']['hesse']['error']
 
         return sigma, sigma_err
 
+    def get_hwhm(self, idx=0):
+        """
+        Get the half width half maximum and its error
+
+        Parameters
+        -------------------------------------------------
+        idx: int
+            Index of the sigma to be returned (default: 0)
+
+        Returns
+        -------------------------------------------------
+        hwhm: float
+            The sigma value obtained from the fit
+        hwhm_err: float
+            The sigma error obtained from the fit
+        """
+        if self._name_signal_pdf_[idx] not in ['gaussian', 'cauchy', 'voigtian']:
+            Logger(f'HFWM parameter not defined for {self._name_signal_pdf_[idx]} pdf!', 'ERROR')
+            return 0., 0.
+
+        if self._name_signal_pdf_[idx] == 'gaussian':
+            mult_fact = np.sqrt(2 * np.log(2))
+            hwhm, hwhm_err = self.get_sigma(idx)
+            hwhm *= mult_fact
+            hwhm_err *= mult_fact
+        elif self._name_signal_pdf_[idx] == 'cauchy':
+            hwhm, hwhm_err = self.get_signal_parameter(idx, 'gamma')
+        elif self._name_signal_pdf_[idx] == 'voigtian':
+            mult_fact = np.sqrt(2 * np.log(2))
+            sigma, sigma_err = self.get_sigma(idx)
+            sigma *= mult_fact
+            sigma_err *= mult_fact
+            gamma, gamma_err = self.get_signal_parameter(idx, 'gamma')
+            hwhm = 0.5346 * gamma + np.sqrt(0.2166 * gamma**2 + sigma**2)
+            # we neglect the correlation between sigma and gamma
+            der_sigma = sigma / np.sqrt(0.0721663 + sigma**2)
+            der_gamma = 0.5346 + (0.2166 * gamma) / np.sqrt(0.2166 * gamma**2 + sigma**2)
+            hwhm_err = np.sqrt(der_sigma**2 * sigma_err**2 + der_gamma**2 * gamma_err**2)
+
+        return hwhm, hwhm_err
+
     def get_signal_parameter(self, idx, par):
         """
         Get a signal parameter and its error
 
         Parameters
         -------------------------------------------------
         idx: int
@@ -1288,14 +1525,18 @@
             Index of the signal to be returned
         **kwargs: dict
             Additional optional arguments:
 
             - nsigma: float
                 nsigma invariant-mass window around mean for signal computation
 
+            - nhwhm: float
+                number of hwhm invariant-mass window around mean for signal and background computation
+                (alternative to nsigma)
+
             - min: float
                 minimum value of invariant-mass for signal computation (alternative to nsigma)
 
             - max: float
                 maximum value of invariant-mass for signal computation (alternative to nsigma)
 
         Returns
@@ -1303,43 +1544,62 @@
         signal: float
             The signal value obtained from the fit
         signal_err: float
             The signal error obtained from the fit
         """
 
         nsigma = kwargs.get('nsigma', 3.)
+        nhwhm = kwargs.get('nhwhm', None)
         min_value = kwargs.get('min', None)
         max_value = kwargs.get('max', None)
+        use_nsigma = True
+
+        if nhwhm is not None and (min_value is not None or max_value is not None):
+            Logger('I cannot compute the signal within a fixed mass interval and a number of HWFM', 'ERROR')
+            return 0., 0.
 
-        if min_value is None or max_value is None:
-            if self._name_signal_pdf_[idx] not in ['gaussian', 'crystalball']:
+        if min_value is not None and max_value is not None:
+            use_nsigma = False
+
+        if nhwhm is not None:
+            use_nsigma = False
+            if self._name_signal_pdf_[idx] not in ['gaussian', 'cauchy', 'voigtian']:
+                Logger('HWHM not defined, I cannot compute the signal for this pdf', 'ERROR')
+                return 0., 0.
+            mass, _ = self.get_mass(idx)
+            hwhm, _ = self.get_hwhm(idx)
+            min_value = mass - nhwhm * hwhm
+            max_value = mass + nhwhm * hwhm
+
+        if use_nsigma:
+            if self._name_signal_pdf_[idx] not in ['gaussian', 'crystalball', 'hist']:
                 Logger('Sigma not defined, I cannot compute the signal for this pdf', 'ERROR')
                 return 0., 0.
             mass, _ = self.get_mass(idx)
             sigma, _ = self.get_sigma(idx)
             min_value = mass - nsigma * sigma
             max_value = mass + nsigma * sigma
 
         # pylint: disable=missing-kwoa
         signal = self._signal_pdf_[idx].integrate((min_value, max_value))
 
-        signal_fracs, _, signal_err_fracs, _ = self.__get_all_fracs()
+        signal_fracs, refl_fracs, _, signal_err_fracs, _, _ = self.__get_all_fracs()
 
         if len(self._background_pdf_) > 0:
             frac = signal_fracs[idx]
             frac_err = signal_err_fracs[idx]
         else:
             if len(self._signal_pdf_) == 1:
                 frac = 1.
                 frac_err = 0.
             if idx < len(signal_fracs):
                 frac = signal_fracs[idx]
                 frac_err = signal_err_fracs[idx]
             else:
-                frac = 1. - sum(signal_fracs)
+                frac = 1. - sum(signal_fracs) - sum(refl_fracs)
                 frac_err = np.sqrt(sum(list(err**2 for err in signal_err_fracs)))
 
         norm = self._data_handler_.get_norm()
         norm_err = norm * frac_err
         norm *= frac
 
         return float(signal * norm), float(signal * norm_err)
@@ -1354,14 +1614,18 @@
             Index of the signal to be used to compute nsigma window
         **kwargs: dict
             Additional optional arguments:
 
             - nsigma: float
                 nsigma invariant-mass window around mean for background computation
 
+            - nhwhm: float
+                number of hwhm invariant-mass window around mean for signal and background computation
+                (alternative to nsigma)
+
             - min: float
                 minimum value of invariant-mass for background computation (alternative to nsigma)
 
             - max: float
                 maximum value of invariant-mass for background computation (alternative to nsigma)
 
         Returns
@@ -1373,34 +1637,53 @@
         """
 
         if not self._background_pdf_:
             Logger('Background not fitted', 'ERROR')
             return 0., 0.
 
         nsigma = kwargs.get('nsigma', 3.)
+        nhwhm = kwargs.get('nhwhm', None)
         min_value = kwargs.get('min', None)
         max_value = kwargs.get('max', None)
+        use_nsigma = True
 
-        if min_value is None or max_value is None:
-            if self._name_signal_pdf_[idx] not in ['gaussian', 'crystalball']:
+        if nhwhm is not None and (min_value is not None or max_value is not None):
+            Logger('I cannot compute the signal within a fixed mass interval and a number of HWFM', 'ERROR')
+            return 0., 0.
+
+        if min_value is not None and max_value is not None:
+            use_nsigma = False
+
+        if nhwhm is not None:
+            use_nsigma = False
+            if self._name_signal_pdf_[idx] not in ['gaussian', 'cauchy', 'voigtian']:
+                Logger('HWHM not defined, I cannot compute the signal for this pdf', 'ERROR')
+                return 0., 0.
+            mass, _ = self.get_mass(idx)
+            hwhm, _ = self.get_hwhm(idx)
+            min_value = mass - nhwhm * hwhm
+            max_value = mass + nhwhm * hwhm
+
+        if use_nsigma:
+            if self._name_signal_pdf_[idx] not in ['gaussian', 'crystalball', 'hist']:
                 Logger('Sigma not defined, I cannot compute the signal for this pdf', 'ERROR')
                 return 0., 0.
             mass, _ = self.get_mass(idx)
             sigma, _ = self.get_sigma(idx)
             min_value = mass - nsigma * sigma
             max_value = mass + nsigma * sigma
 
-        signal_fracs, bkg_fracs, signal_err_fracs, bkg_err_fracs = self.__get_all_fracs()
+        signal_fracs, bkg_fracs, refl_fracs, signal_err_fracs, bkg_err_fracs, _ = self.__get_all_fracs()
 
         # pylint: disable=missing-kwoa
         background, background_err = 0., 0.
         for idx2, bkg in enumerate(self._background_pdf_):
 
             if idx2 == len(self._background_pdf_) - 1:
-                frac = 1. - sum(signal_fracs)
+                frac = 1. - sum(signal_fracs) - sum(refl_fracs)
                 frac_err = np.sqrt(sum(list(err**2 for err in signal_err_fracs)))
             else:
                 frac = bkg_fracs[idx2]
                 frac_err = bkg_err_fracs[idx2]
 
             norm = self._data_handler_.get_norm()
             norm_err = norm * frac_err
@@ -1424,14 +1707,18 @@
             Index of the signal to be used to compute nsigma window
         **kwargs: dict
             Additional optional arguments:
 
             - nsigma: float
                 nsigma invariant-mass window around mean for signal and background computation
 
+            - nhwhm: float
+                number of hwhm invariant-mass window around mean for signal and background computation
+                (alternative to nsigma)
+
             - min: float
                 minimum value of invariant-mass for signal and background computation (alternative to nsigma)
 
             - max: float
                 maximum value of invariant-mass for signal and background computation (alternative to nsigma)
 
         Returns
@@ -1460,14 +1747,18 @@
             Index of the signal to be used to compute nsigma window
         **kwargs: dict
             Additional optional arguments:
 
             - nsigma: float
                 nsigma invariant-mass window around mean for signal and background computation
 
+            - nhwhm: float
+                number of hwhm invariant-mass window around mean for signal and background computation
+                (alternative to nsigma)
+
             - min: float
                 minimum value of invariant-mass for signal and background computation (alternative to nsigma)
 
             - max: float
                 maximum value of invariant-mass for signal and background computation (alternative to nsigma)
 
         Returns
@@ -1512,23 +1803,24 @@
             - limits: list
                 minimum and maximum limits for the mass parameter
 
             - fix: bool
                 fix the mass parameter
         """
         mass_name = 'm' if self._name_signal_pdf_[idx] == 'cauchy' else 'mu'
+        mass = 0.
         if 'mass' in kwargs:
             mass = kwargs['mass']
         elif 'pdg_id' in kwargs:
             mass = Particle.from_pdgid(kwargs['pdg_id']).mass*1e-3
         elif 'pdg_name' in kwargs:
             mass = Particle.from_name(kwargs['pdg_name']).mass*1e-3
         else:
             Logger(f'"mass", "pdg_id", and "pdg_name" not provided, mass value for signal {idx} will not be set',
-                         'ERROR')
+                   'ERROR')
         self._init_sgn_pars_[idx][mass_name] = mass
         if 'limits' in kwargs:
             self._limits_sgn_pars_[idx][mass_name] = kwargs['limits']
         if 'fix' in kwargs:
             self._fix_sgn_pars_[idx][mass_name] = kwargs['fix']
 
     def set_signal_initpar(self, idx, par_name, init_value, **kwargs):
@@ -1582,14 +1874,29 @@
         self._init_bkg_pars_[idx][par_name] = init_value
         if 'limits' in kwargs:
             self._limits_bkg_pars_[idx][par_name] = kwargs['limits']
         if 'fix' in kwargs:
             self._fix_bkg_pars_[idx][par_name] = kwargs['fix']
 
     # pylint: disable=line-too-long
+    def set_signal_template(self, idx, sample):
+        """
+        Set sample and options for signal template
+
+        Parameters
+        -------------------------------------------------
+        idx: int
+            Index of the signal
+        sample: flarefly.DataHandler
+            Data sample for histogram template
+        """
+
+        self._hist_signal_sample_[idx] = sample
+
+    # pylint: disable=line-too-long
     def set_signal_kde(self, idx, sample, **kwargs):
         """
         Set sample and options for signal kde
 
         Parameters
         -------------------------------------------------
         idx: int
@@ -1602,14 +1909,70 @@
             for more details
         """
 
         self._kde_signal_sample_[idx] = sample
         self._kde_signal_option_[idx] = kwargs
 
     # pylint: disable=line-too-long
+    def set_reflection_template(self, idx, sample, r_over_s):
+        """
+        Set sample and options for reflected signal template
+
+        Parameters
+        -------------------------------------------------
+        idx: int
+            Index of the reflected signal
+        sample: flarefly.DataHandler
+            Data sample for histogram template
+        r_over_s: float
+            R/S ratio
+        """
+
+        self._hist_refl_sample_[idx] = sample
+        self._refl_over_sgn_[idx] = r_over_s
+
+    # pylint: disable=line-too-long
+    def set_reflection_kde(self, idx, sample, r_over_s, **kwargs):
+        """
+        Set sample and options for reflected signal kde
+
+        Parameters
+        -------------------------------------------------
+        idx: int
+            Index of the signal
+        sample: flarefly.DataHandler
+            Data sample for Kernel Density Estimation
+        r_over_s: float
+            R/S ratio
+        **kwargs: dict
+            Arguments for kde options. See
+            https://zfit.readthedocs.io/en/latest/user_api/pdf/_generated/kde_api/zfit.pdf.KDE1DimGrid.html#zfit.pdf.KDE1DimGrid
+            for more details
+        """
+
+        self._kde_signal_sample_[idx] = sample
+        self._kde_signal_option_[idx] = kwargs
+        self._refl_over_sgn_[idx] = r_over_s
+
+    # pylint: disable=line-too-long
+    def set_background_template(self, idx, sample):
+        """
+        Set sample and options for background template histogram
+
+        Parameters
+        -------------------------------------------------
+        idx: int
+            Index of the background
+        sample: flarefly.DataHandler
+            Data sample for template histogram
+        """
+
+        self._hist_bkg_sample_[idx] = sample
+
+    # pylint: disable=line-too-long
     def set_background_kde(self, idx, sample, **kwargs):
         """
         Set sample and options for background kde
 
         Parameters
         -------------------------------------------------
         idx: int
```

### Comparing `flarefly-0.0.6/flarefly/utils.py` & `flarefly-0.0.8/flarefly/utils.py`

 * *Files identical despite different names*

### Comparing `flarefly-0.0.6/setup.py` & `flarefly-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         setup(**self.conf)
 
 
 SETUP = Setup(
     name="flarefly",
 
     # LAST-TAG is a placeholder. Automatically replaced at deploy time with the right tag
-    version="0.0.6",
+    version="0.0.8",
     description="FLexible And REliable Fitting LibrarY for particle physics analysis",
     url="https://github.com/flarefly/flarefly",
     author="flarefly-developers",
     author_email="flarefly@googlegroups.com",
     license="GPL",
 
     # See https://pypi.org/classifiers/
@@ -82,19 +82,19 @@
     # find_packages().
     packages=find_packages(exclude=['tutorials']),
 
     # List run-time dependencies here. These will be installed by pip when your project is
     # installed. For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     install_requires=[
-        "psutil", "dutil", "prophet==1.0.1", "numpy>=1.20", "pandas>=1.1.5", "uproot>=4.3.4",
-        "ipython>=7.16.1", "jedi==0.17.2", "zfit>=0.10", "mplhep>=0.3.25", "matplotlib>=3.1.3",
+        "psutil", "dutil", "prophet>=1.0.1", "numpy>=1.20", "pandas>=1.1.5", "uproot>=4.3.4",
+        "ipython>=7.16.1", "jedi==0.17.2", "zfit>=0.12.1", "mplhep>=0.3.25", "matplotlib>=3.1.3",
         "particle>=0.20.1", "scipy>=1.7.3"
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 
     # List additional groups of dependencies here (e.g. development dependencies). You can install
     # these using the following syntax, for example:
     # $ pip install -e .[dev,test]
     extras_require={
         "dev": [
             "pylint>=2.6.2", "flake8>=3.8.4", "pytest>=6.2.2", "twine>=3.3.0",
```

