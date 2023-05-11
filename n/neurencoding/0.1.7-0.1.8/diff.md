# Comparing `tmp/neurencoding-0.1.7.tar.gz` & `tmp/neurencoding-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurencoding-0.1.7.tar", last modified: Thu Feb 23 15:17:25 2023, max compression
+gzip compressed data, was "neurencoding-0.1.8.tar", last modified: Thu May 11 11:30:07 2023, max compression
```

## Comparing `neurencoding-0.1.7.tar` & `neurencoding-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 berk      (1000) berk      (1000)        0 2023-02-23 15:17:25.498972 neurencoding-0.1.7/
--rw-r--r--   0 berk      (1000) berk      (1000)     1081 2022-11-24 11:55:57.000000 neurencoding-0.1.7/LICENSE
--rw-rw-r--   0 berk      (1000) berk      (1000)     1427 2023-02-23 15:17:25.494972 neurencoding-0.1.7/PKG-INFO
--rw-r--r--   0 berk      (1000) berk      (1000)      733 2023-02-22 12:11:22.000000 neurencoding-0.1.7/README.md
-drwxrwxr-x   0 berk      (1000) berk      (1000)        0 2023-02-23 15:17:25.494972 neurencoding-0.1.7/neurencoding/
--rw-r--r--   0 berk      (1000) berk      (1000)       77 2022-11-24 11:55:57.000000 neurencoding-0.1.7/neurencoding/__init__.py
--rw-r--r--   0 berk      (1000) berk      (1000)    11599 2022-11-24 11:55:57.000000 neurencoding-0.1.7/neurencoding/_models.py
--rw-rw-r--   0 berk      (1000) berk      (1000)    22719 2023-02-23 11:57:42.000000 neurencoding-0.1.7/neurencoding/design_matrix.py
--rw-r--r--   0 berk      (1000) berk      (1000)     4134 2022-11-24 11:55:57.000000 neurencoding-0.1.7/neurencoding/linear.py
--rw-r--r--   0 berk      (1000) berk      (1000)     4595 2022-11-24 11:55:57.000000 neurencoding-0.1.7/neurencoding/poisson.py
--rw-r--r--   0 berk      (1000) berk      (1000)    15406 2023-02-23 15:16:43.000000 neurencoding-0.1.7/neurencoding/utils.py
-drwxrwxr-x   0 berk      (1000) berk      (1000)        0 2023-02-23 15:17:25.494972 neurencoding-0.1.7/neurencoding.egg-info/
--rw-rw-r--   0 berk      (1000) berk      (1000)     1427 2023-02-23 15:17:25.000000 neurencoding-0.1.7/neurencoding.egg-info/PKG-INFO
--rw-rw-r--   0 berk      (1000) berk      (1000)      380 2023-02-23 15:17:25.000000 neurencoding-0.1.7/neurencoding.egg-info/SOURCES.txt
--rw-rw-r--   0 berk      (1000) berk      (1000)        1 2023-02-23 15:17:25.000000 neurencoding-0.1.7/neurencoding.egg-info/dependency_links.txt
--rw-rw-r--   0 berk      (1000) berk      (1000)       62 2023-02-23 15:17:25.000000 neurencoding-0.1.7/neurencoding.egg-info/requires.txt
--rw-rw-r--   0 berk      (1000) berk      (1000)       13 2023-02-23 15:17:25.000000 neurencoding-0.1.7/neurencoding.egg-info/top_level.txt
--rw-rw-r--   0 berk      (1000) berk      (1000)     1201 2023-02-23 15:17:10.000000 neurencoding-0.1.7/pyproject.toml
--rw-rw-r--   0 berk      (1000) berk      (1000)       38 2023-02-23 15:17:25.498972 neurencoding-0.1.7/setup.cfg
-drwxrwxr-x   0 berk      (1000) berk      (1000)        0 2023-02-23 15:17:25.494972 neurencoding-0.1.7/tests/
--rw-r--r--   0 berk      (1000) berk      (1000)    10791 2022-11-24 11:55:57.000000 neurencoding-0.1.7/tests/test_design.py
+drwxrwxr-x   0 berk      (1000) berk      (1000)        0 2023-05-11 11:30:07.043729 neurencoding-0.1.8/
+-rw-r--r--   0 berk      (1000) berk      (1000)     1081 2022-11-24 11:55:57.000000 neurencoding-0.1.8/LICENSE
+-rw-rw-r--   0 berk      (1000) berk      (1000)     1427 2023-05-11 11:30:07.043729 neurencoding-0.1.8/PKG-INFO
+-rw-r--r--   0 berk      (1000) berk      (1000)      733 2023-02-22 12:11:22.000000 neurencoding-0.1.8/README.md
+drwxrwxr-x   0 berk      (1000) berk      (1000)        0 2023-05-11 11:30:07.043729 neurencoding-0.1.8/neurencoding/
+-rw-r--r--   0 berk      (1000) berk      (1000)      215 2023-02-23 15:25:57.000000 neurencoding-0.1.8/neurencoding/__init__.py
+-rw-r--r--   0 berk      (1000) berk      (1000)    11915 2023-02-27 14:26:44.000000 neurencoding-0.1.8/neurencoding/_models.py
+-rw-rw-r--   0 berk      (1000) berk      (1000)    23199 2023-02-27 11:34:09.000000 neurencoding-0.1.8/neurencoding/design_matrix.py
+-rw-r--r--   0 berk      (1000) berk      (1000)     4607 2023-02-27 16:08:25.000000 neurencoding-0.1.8/neurencoding/linear.py
+-rw-r--r--   0 berk      (1000) berk      (1000)     5213 2023-02-27 14:42:00.000000 neurencoding-0.1.8/neurencoding/poisson.py
+-rw-r--r--   0 berk      (1000) berk      (1000)    16602 2023-04-03 14:21:57.000000 neurencoding-0.1.8/neurencoding/utils.py
+drwxrwxr-x   0 berk      (1000) berk      (1000)        0 2023-05-11 11:30:07.043729 neurencoding-0.1.8/neurencoding.egg-info/
+-rw-rw-r--   0 berk      (1000) berk      (1000)     1427 2023-05-11 11:30:07.000000 neurencoding-0.1.8/neurencoding.egg-info/PKG-INFO
+-rw-rw-r--   0 berk      (1000) berk      (1000)      380 2023-05-11 11:30:07.000000 neurencoding-0.1.8/neurencoding.egg-info/SOURCES.txt
+-rw-rw-r--   0 berk      (1000) berk      (1000)        1 2023-05-11 11:30:07.000000 neurencoding-0.1.8/neurencoding.egg-info/dependency_links.txt
+-rw-rw-r--   0 berk      (1000) berk      (1000)       62 2023-05-11 11:30:07.000000 neurencoding-0.1.8/neurencoding.egg-info/requires.txt
+-rw-rw-r--   0 berk      (1000) berk      (1000)       13 2023-05-11 11:30:07.000000 neurencoding-0.1.8/neurencoding.egg-info/top_level.txt
+-rw-rw-r--   0 berk      (1000) berk      (1000)     1201 2023-05-11 11:29:55.000000 neurencoding-0.1.8/pyproject.toml
+-rw-rw-r--   0 berk      (1000) berk      (1000)       38 2023-05-11 11:30:07.043729 neurencoding-0.1.8/setup.cfg
+drwxrwxr-x   0 berk      (1000) berk      (1000)        0 2023-05-11 11:30:07.043729 neurencoding-0.1.8/tests/
+-rw-r--r--   0 berk      (1000) berk      (1000)    10791 2022-11-24 11:55:57.000000 neurencoding-0.1.8/tests/test_design.py
```

### Comparing `neurencoding-0.1.7/LICENSE` & `neurencoding-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `neurencoding-0.1.7/PKG-INFO` & `neurencoding-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurencoding
-Version: 0.1.7
+Version: 0.1.8
 Summary: Neural encoding models made easy. Describe neuronal activity as a function of other variables
 Author-email: Berk Gercek <berkgercek@duck.com>
 Project-URL: Homepage, https://github.com/berkgercek/neurencoding
 Project-URL: Bug Tracker, https://github.com/berkgercek/neurencoding/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neurencoding-0.1.7/README.md` & `neurencoding-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `neurencoding-0.1.7/neurencoding/_models.py` & `neurencoding-0.1.8/neurencoding/_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,34 +3,37 @@
 
 # Third party libraries
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 from scipy.special import xlogy
 from sklearn.metrics import r2_score
+from sklearn.base import MetaEstimatorMixin
 
 # Neurencoding repo imports
 import neurencoding
 from .utils import bincount2D, neglog
 
 
 class EphysModel:
     """
     Parent class for multiple types of neural models. Contains core methods for extracting
     trial-relevant spike times and binning spikes, as well as making sure that the design matrix
     being used makes sense.
     """
 
-    def __init__(self,
-                 design_matrix: neurencoding.design_matrix.DesignMatrix,
-                 spk_times: npt.ArrayLike,
-                 spk_clu: npt.ArrayLike,
-                 binwidth: float = 0.02,
-                 mintrials: int = 100,
-                 stepwise: bool = False):
+    def __init__(
+        self,
+        design_matrix: neurencoding.design_matrix.DesignMatrix,
+        spk_times: npt.ArrayLike,
+        spk_clu: npt.ArrayLike,
+        binwidth: float = 0.02,
+        mintrials: int = 100,
+        stepwise: bool = False,
+    ):
         """
         Construct GLM object using information about all trials, and the relevant spike times.
         Only ingests data, and further object methods must be called to describe kernels, gain
         terms, etc. as components of the model.
 
         Parameters
         ----------
@@ -52,32 +55,32 @@
             incorporate only some parameters, to see which regressors actually improve
             explainability. Defaults to False.
         """
         # Data checks #
         if not len(spk_times) == len(spk_clu):
             raise IndexError("Spike times and cluster IDs are not same length")
         if not design_matrix.compiled:
-            raise AttributeError('Design matrix object must be compiled before passing to fit')
+            raise AttributeError("Design matrix object must be compiled before passing to fit")
 
         # Filter out cells which don't meet the criteria for minimum spiking, while doing trial
         # assignment
         base_df = design_matrix.base_df
         clu_ids = np.unique(spk_clu).flatten()
-        trbounds = base_df[['trial_start', 'trial_end']]  # Get the start/end of trials
+        trbounds = base_df[["trial_start", "trial_end"]]  # Get the start/end of trials
         # Initialize a Cells x Trials bool array to easily see how many trials a clu spiked
         trialspiking = np.zeros((base_df.index.max() + 1, clu_ids.max() + 1), dtype=bool)
         # Empty trial duration value to use later
         # Iterate through each trial, and store the relevant spikes for that trial into a dict
         # Along with the cluster labels. This makes binning spikes and accessing spikes easier.
         spks = {}
         clu = {}
         st_endlast = 0
         for i, (start, end) in trbounds.iterrows():
             st_startind = np.searchsorted(spk_times[st_endlast:], start) + st_endlast
-            st_endind = np.searchsorted(spk_times[st_endlast:], end, side='right') + st_endlast
+            st_endind = np.searchsorted(spk_times[st_endlast:], end, side="right") + st_endlast
             st_endlast = st_endind
             trial_clu = np.unique(spk_clu[st_startind:st_endind])
             trialspiking[i, trial_clu] = True
             spks[i] = spk_times[st_startind:st_endind] - start
             clu[i] = spk_clu[st_startind:st_endind]
 
         # Set model parameters to begin with
@@ -85,31 +88,32 @@
         self.spikes = spks
         self.clu = clu
         self.clu_ids = np.argwhere(np.sum(trialspiking, axis=0) > mintrials).flatten()
         self.stepwise = stepwise
         self.binwidth = binwidth
 
         if len(self.clu_ids) == 0:
-            raise UserWarning('No neuron fired a spike in a minimum number.')
+            raise UserWarning("No neuron fired a spike in a minimum number.")
 
         # Bin spikes
         spkarrs, arrdiffs = [], []
         for i in self.design.trialsdf.index:
-            duration = self.design.trialsdf.loc[i, 'duration']
+            duration = self.design.trialsdf.loc[i, "duration"]
             durmod = duration % self.binwidth
             if durmod > (self.binwidth / 2):
                 duration = duration - (self.binwidth / 2)
             if len(self.spikes[i]) == 0:
                 arr = np.zeros((self.binf(duration), len(self.clu_ids)))
                 spkarrs.append(arr)
                 continue
             spks = self.spikes[i]
             clu = self.clu[i]
-            arr = bincount2D(spks, clu, xbin=self.binwidth, ybin=self.clu_ids, xlim=[0,
-                                                                                     duration])[0]
+            arr = bincount2D(spks, clu, xbin=self.binwidth, ybin=self.clu_ids, xlim=[0, duration])[
+                0
+            ]
             arrdiffs.append(arr.shape[1] - self.binf(duration))
             spkarrs.append(arr.T)
         y = np.vstack(spkarrs)
         assert y.shape[0] == self.design.dm.shape[0], "Oh shit. Indexing error."
         self.binnedspikes = y
 
     def combine_weights(self, peaksonly=False) -> pd.DataFrame:
@@ -122,60 +126,65 @@
         pandas.DataFrame
             DataFrame in which each row is the fit weights for a given spiking unit. Columns are
             individual covariates added during the construction process. Indices are the cluster
             IDs for each of the cells that were fit (NOT a simple range(start, stop) index.)
         """
         outputs = {}
         for var in self.design.covar.keys():
-            if self.design.covar[var]['bases'] is None:
-                wind = self.design.covar[var]['dmcol_idx']
+            if self.design.covar[var]["bases"] is None:
+                wind = self.design.covar[var]["dmcol_idx"]
                 outputs[var] = self.coefs.apply(lambda w: w[wind])
                 continue
-            winds = self.design.covar[var]['dmcol_idx']
-            bases = self.design.covar[var]['bases']
-            offset = self.design.covar[var]['offset']
+            winds = self.design.covar[var]["dmcol_idx"]
+            bases = self.design.covar[var]["bases"]
+            offset = self.design.covar[var]["offset"]
             tlen = bases.shape[0] * self.binwidth
             tstamps = np.linspace(0 + offset, tlen + offset, bases.shape[0])
             if peaksonly:
                 peakinds = np.argmax(bases, axis=0)
                 peakvals = np.max(bases, axis=0)
                 tstamps = tstamps[peakinds]
                 weights = self.coefs.apply(lambda w: w[winds] * peakvals)
             else:
                 weights = self.coefs.apply(lambda w: np.sum(w[winds] * bases, axis=1))
-            outputs[var] = pd.DataFrame(weights.values.tolist(),
-                                        index=weights.index,
-                                        columns=tstamps)
+            outputs[var] = pd.DataFrame(
+                weights.values.tolist(), index=weights.index, columns=tstamps
+            )
         self.combined_weights = outputs
         self.peaksonly_weights = peaksonly
         return outputs
 
     def _scorer(self, wt, bias, dm, y):
         """
         Score a single target y
         """
         pred = self.link(dm @ wt + bias).flatten()
-        if self.metric == 'dsq':
+        if self.metric == "dsq":
             null_pred = np.ones_like(pred) * np.mean(y)
             null_deviance = 2 * np.sum(xlogy(y, y / null_pred.flat) - y + null_pred.flat)
-            with np.errstate(invalid='ignore', divide='ignore'):
+            with np.errstate(invalid="ignore", divide="ignore"):
                 full_deviance = 2 * np.sum(xlogy(y, y / pred.flat) - y + pred.flat)
             return 1 - (full_deviance / null_deviance)
-        elif self.metric == 'msespike':
-            residuals = (y - pred)**2
+        elif self.metric == "msespike":
+            residuals = (y - pred) ** 2
             return residuals.sum() / y.sum()
-        elif self.metric == 'rsq':
+        elif self.metric == "rsq":
             return r2_score(y, pred)
-        elif self.metric == 'nllspike':
+        elif self.metric == "nllspike":
             biasdm = np.pad(dm, ((0, 0), (1, 0)), constant_values=1)
             return -neglog(np.vstack((bias, wt)).flatten(), biasdm, y) / np.sum(y)
         else:
-            raise AttributeError('No valid metric exists in the instance for use by _scorer()')
+            raise AttributeError("No valid metric exists in the instance for use by _scorer()")
 
-    def fit(self, train_idx: Optional[npt.ArrayLike] = None, printcond: bool = True):
+    def fit(
+        self,
+        train_idx: Optional[npt.ArrayLike] = None,
+        printcond: bool = True,
+        bestparams: bool = False,
+    ):
         """
         Fit the current set of binned spikes as a function of the current design matrix. Requires
         NeuralGLM.bin_spike_trains and NeuralGLM.compile_design_matrix to be run first. Will store
         the fit weights to an internal variable. To access these fit weights in a pandas DataFrame
         use the NeuralGLM.combine_weights method.
 
         Parameters
@@ -194,52 +203,58 @@
         intercepts : list
             List of intercepts (bias terms) fit.
         """
         # Input checks
         if train_idx is None:
             train_idx = self.design.trialsdf.index
         if not np.all(np.isin(train_idx, self.design.trialsdf.index)):
-            raise IndexError('Not all train indices in the trials of design matrix')
+            raise IndexError("Not all train indices in the trials of design matrix")
+        if bestparams and not isinstance(self.estimator, MetaEstimatorMixin):
+            raise ValueError("bestparams is only valid when using GridSearchCV as the estimator")
 
         # Store training and test indices for self so that .score() method will know what to
         # operate on. If all data indices are in train indices, train and test are the same set.
         self.traininds = train_idx
         if not np.all(np.isin(self.design.trialsdf.index, train_idx)):
             self.testinds = self.design.trialsdf.index.difference(train_idx)
         else:
             self.testinds = train_idx
 
         # Mask for training data
         trainmask = np.isin(self.design.trlabels, train_idx).flatten()
         trainbinned = self.binnedspikes[trainmask]
         if printcond:
-            print(f'Condition of design matrix is {np.linalg.cond(self.design[trainmask])}')
+            print(f"Condition of design matrix is {np.linalg.cond(self.design[trainmask])}")
 
         traindm = self.design[trainmask]
-        coefs, intercepts, = self._fit(traindm, trainbinned)
+        if not bestparams:
+            coefs, intercepts, = self._fit(traindm, trainbinned)
+        else:
+            coefs, intercepts, alphas = self._fit(traindm, trainbinned, bestparams=bestparams)
+            self.alphas = alphas
         self.coefs, self.intercepts = coefs, intercepts
         return
 
     def score(self, testinds: Optional[npt.ArrayLike] = None):
         """
         Score model using chosen metric
 
         Returns
         -------
         pandas.Series
             Score using chosen metric (defined at instantiation) for each unit fit by the model.
         """
-        if not hasattr(self, 'coefs'):
-            raise AttributeError('Model has not been fit yet.')
+        if not hasattr(self, "coefs"):
+            raise AttributeError("Model has not been fit yet.")
         if testinds is None:
             testinds = self.testinds
         testmask = np.isin(self.design.trlabels, testinds).flatten()
         dm, binned = self.design[testmask, :], self.binnedspikes[testmask]
 
-        scores = pd.Series(index=self.coefs.index, name='scores', dtype=np.float64)
+        scores = pd.Series(index=self.coefs.index, name="scores", dtype=np.float64)
         for cell in self.coefs.index:
             cell_idx = np.argwhere(self.clu_ids == cell)[0, 0]
             wt = self.coefs.loc[cell].reshape(-1, 1)
             bias = self.intercepts.loc[cell]
             y = binned[:, cell_idx]
             scores.at[cell] = self._scorer(wt, bias, dm, y)
         return scores
```

### Comparing `neurencoding-0.1.7/neurencoding/design_matrix.py` & `neurencoding-0.1.8/neurencoding/design_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,19 +349,22 @@
             Description of the covariate for reference purposes, by default '' (empty)
         """
         if covlabel in self.covar:
             raise AttributeError(f'Covariate {covlabel} already exists in model.')
         self._compile_check()
         # Test for mismatch in length of regressor vs trials
         mismatch = np.zeros(len(self.trialsdf.index), dtype=bool)
+        nans = np.zeros(self.trialsdf.index.max(), dtype=bool)
         for i in self.trialsdf.index:
             currtr = self.trialsdf.loc[i]
             nT = self.binf(currtr.duration)
             if regressor.loc[i].shape[0] != nT:
                 mismatch[i] = True
+            if np.any(np.isnan(regressor.loc[i])):
+                nans[i - 1] = True
 
         if np.any(mismatch):
             raise ValueError('Length mismatch between regressor and trial on trials'
                              f'{np.argwhere(mismatch)}.')
 
         # Initialize containers for the covariate dicts
         if not hasattr(self, 'currcol'):
@@ -370,14 +373,20 @@
             try:
                 cond = self.trialsdf.index[self.trialsdf.apply(cond, axis=1)].to_numpy()
             except AttributeError:
                 cond = self.trialsdf.index[self.trialsdf.apply(cond, axis=1)]
         if not all(regressor.index == self.trialsdf.index):
             raise IndexError('Indices of regressor and trials dataframes do not match.')
 
+        nantrials = pd.Series({i: np.any(np.isnan(regressor.loc[i])) for i in self.trialsdf.index})
+        if cond is not None and np.any(nantrials.loc[cond]):
+            raise ValueError('NaNs in regressor on trials')
+        elif cond is None and np.any(nantrials):
+            raise ValueError('NaNs in regressor on trials')
+
         cov = {
             'description':
                 desc,
             'bases':
                 bases,
             'valid_trials':
                 cond if cond is not None else self.trialsdf.index,
```

### Comparing `neurencoding-0.1.7/neurencoding/linear.py` & `neurencoding-0.1.8/neurencoding/linear.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+# Standard library
+import logging
+
 # Third party libraries
+import joblib
 import numpy as np
 import pandas as pd
 from sklearn.base import BaseEstimator, MetaEstimatorMixin
 from sklearn.linear_model import LinearRegression
 
 # Neurencoding repo imports
 from ._models import EphysModel
 
+_logger = logging.getLogger("neurencoding")
+
 
 class LinearGLM(EphysModel):
 
     def __init__(self,
                  design_matrix,
                  spk_times,
                  spk_clu,
@@ -30,15 +36,15 @@
             1-D Array of spike times
         spk_clu : np.array
             1-D Array, same shape as spk_times, assigning cluster identities to each spike time
         binwidth : float, optional
             Length of the bins to be used to count spikes, by default 0.02
         metric : str, optional
             Scoring metric which to use for the models .score() method. Can be rsq, dsq, msepike,
-            by default 'rsq'
+            nllspike, by default 'rsq'
         estimator : sklearn.linear_model estimator, optional
             Estimator to use for model fitting. If None will default to pure linear regression.
             Must have a .fit(X, y) method and after fitting contain .coef_ and .intercept_
             attributes. By default None.
         train : float, optional
             Proportion of data to use as training set, by default 0.8
         blocktrain : bool, optional
@@ -47,21 +53,22 @@
             Minimum number of trials in which a neuron must fire >0 spikes to be considered for
             fitting, by default 100
         """
         super().__init__(design_matrix, spk_times, spk_clu, binwidth, mintrials)
         if estimator is None:
             estimator = LinearRegression()
         if not isinstance(estimator, BaseEstimator):
-            raise ValueError('Estimator must be a scikit-learn estimator, e.g. LinearRegression')
+            _logger.warn("Estimator is not a sklearn estimator, may not work as expected."
+                         " Trying anyway.")
         self.metric = metric
         self.estimator = estimator
         self.link = lambda x: x
         self.invlink = self.link
 
-    def _fit(self, dm, binned, cells=None):
+    def _fit(self, dm, binned, cells=None, bestparams=False):
         """
         Fitting primitive that brainbox.EphysModel.fit method will call
 
         Parameters
         ----------
         dm : np.ndarray
             Design matrix to use for fitting
@@ -83,19 +90,25 @@
         if cells is None:
             cells = self.clu_ids.flatten()
         if cells.shape[0] != binned.shape[1]:
             raise ValueError('Length of cells does not match shape of binned')
 
         coefs = pd.Series(index=cells, name='coefficients', dtype=object)
         intercepts = pd.Series(index=cells, name='intercepts', dtype=np.float64)
+        if isinstance(self.estimator, MetaEstimatorMixin):
+            pars = pd.Series(index=cells, name='intercepts', dtype=np.float64)
 
-        lm = self.estimator.fit(dm, binned)
-        if isinstance(lm, MetaEstimatorMixin):
-            est = lm.best_estimator_
-            weight, intercept = est.coef_, est.intercept_
-        else:
-            weight, intercept = lm.coef_, lm.intercept_
         for cell in cells:
             cell_idx = np.argwhere(cells == cell)[0, 0]
-            coefs.at[cell] = weight[cell_idx, :]
-            intercepts.at[cell] = intercept[cell_idx]
+            lm = self.estimator.fit(dm, binned[:, cell_idx])
+            if isinstance(lm, MetaEstimatorMixin):
+                est = lm.best_estimator_
+                weight, intercept = est.coef_.copy(), est.intercept_
+                pars.loc[cell] = lm.best_params_["alpha"]
+                del est
+            else:
+                weight, intercept = lm.coef_.copy(), lm.intercept_
+            coefs.at[cell] = weight
+            intercepts.at[cell] = intercept
+        if bestparams:
+            return coefs, intercepts, pars
         return coefs, intercepts
```

### Comparing `neurencoding-0.1.7/neurencoding/poisson.py` & `neurencoding-0.1.8/neurencoding/poisson.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # Standard library
-from warnings import catch_warnings, warn
+import logging
+from warnings import catch_warnings
 
 # Third party libraries
 import numpy as np
 import pandas as pd
 from sklearn.linear_model import PoissonRegressor
+from sklearn.model_selection import GridSearchCV
 from tqdm import tqdm
 
 # Neurencoding repo imports
 from ._models import EphysModel
 
+_logger = logging.getLogger("neurencoding")
 
-class PoissonGLM(EphysModel):
 
-    def __init__(self,
-                 design_matrix,
-                 spk_times,
-                 spk_clu,
-                 binwidth=0.02,
-                 metric='dsq',
-                 fit_intercept=True,
-                 alpha=0,
-                 mintrials=100):
+class PoissonGLM(EphysModel):
+    def __init__(
+        self,
+        design_matrix,
+        spk_times,
+        spk_clu,
+        binwidth=0.02,
+        metric="dsq",
+        fit_intercept=True,
+        alpha=0,
+        mintrials=100,
+    ):
         """
         Fit a poisson model using a DesignMatrix and spiking rate.
         Uses the sklearn.linear_model.PoissonRegressor to perform fitting.
 
         Parameters
         ----------
         design_matrix : neurencoding.DesignMatrix
@@ -39,30 +44,41 @@
         binwidth : float, optional
             Spikes in input will be binned into non-overlapping bins, this is the width of those
             bins, by default 0.02
         metric : str, optional
             Choice of metric for use by PoissonGLM.score, by default 'dsq'
         fit_intercept : bool, optional
             Whether or not to fit a bias term in the poisson model, by default True
-        alpha : float, optional
+        alpha : float or array, optional
             Regularization strength for the poisson regression, determines the strength of the
-            L2 penalty in the objective for fitting, by default 0
+            L2 penalty in the objective for fitting. If an array of values is passed,
+            sklearn's GridSearchCV will be used to test all values and choose the best via
+            cross-validation, by default 0
         mintrials : int, optional
             Minimum number of trials in which a unit must fire at least one spike in order to be
             included in the fitting, by default 100
         """
         super().__init__(design_matrix, spk_times, spk_clu, binwidth, mintrials)
-        # TODO: Implement grid search over alphas to find optimal value
         self.metric = metric
         self.fit_intercept = fit_intercept
-        self.alpha = alpha
+        if hasattr(alpha, "shape"):
+            self._alpha_grid = alpha
+            self.estimator = GridSearchCV(
+                PoissonRegressor(fit_intercept=fit_intercept), {"alpha": alpha}, max_iter=300
+            )
+        else:
+            self.alpha = alpha
+            self.estimator = PoissonRegressor(
+                fit_intercept=fit_intercept, alpha=alpha, max_iter=300
+            )
+
         self.link = np.exp
         self.invlink = np.log
 
-    def _fit(self, dm, binned, cells=None, noncovwarn=False):
+    def _fit(self, dm, binned, cells=None, noncovwarn=True, bestparams=False):
         """
         Fit a GLM using scikit-learn implementation of PoissonRegressor. Uses a regularization
         strength parameter alpha, which is the strength of ridge regularization term.
 
         Parameters
         ----------
         dm : numpy.ndarray
@@ -72,36 +88,40 @@
             Vector of observed spike counts which we seek to predict. Must be of the same length
             as dm.shape[0]
         alpha : float
             Regularization strength, applied as multiplicative constant on ridge regularization.
         cells : list
             List of cells labels for columns in binned. Will default to all cells in model if None
             is passed. Must be of the same length as columns in binned. By default None.
+        bestparams: bool
+            Whether or not to
         """
         if cells is None:
             cells = self.clu_ids.flatten()
         if cells.shape[0] != binned.shape[1]:
-            raise ValueError('Length of cells does not match shape of binned')
+            raise ValueError("Length of cells does not match shape of binned")
 
-        # TODO: Make this malleable to accept either an estimator or a GridSearchCV meta-estimator
-        coefs = pd.Series(index=cells, name='coefficients', dtype=object)
-        intercepts = pd.Series(index=cells, name='intercepts')
+        coefs = pd.Series(index=cells, name="coefficients", dtype=object)
+        intercepts = pd.Series(index=cells, name="intercepts")
+        alphas = pd.Series(index=cells, name="alphas")
         nonconverged = []
-        for cell in tqdm(cells, 'Fitting units:', leave=False):
+        for cell in tqdm(cells, "Fitting units:", leave=False):
             cell_idx = np.argwhere(cells == cell)[0, 0]
             cellbinned = binned[:, cell_idx]
             with catch_warnings(record=True) as w:
-                fitobj = PoissonRegressor(alpha=self.alpha,
-                                          max_iter=300,
-                                          fit_intercept=self.fit_intercept).fit(dm, cellbinned)
+                fitobj = self.estimator.fit(dm, cellbinned)
             if len(w) != 0:
                 nonconverged.append(cell)
+            if isinstance(self.estimator, GridSearchCV):
+                alphas.at[cell] = fitobj.best_params_["alpha"]
+                fitobj = fitobj.best_estimator_
             coefs.at[cell] = fitobj.coef_
             if self.fit_intercept:
                 intercepts.at[cell] = fitobj.intercept_
             else:
                 intercepts.at[cell] = 0
         if noncovwarn:
             if len(nonconverged) != 0:
-                warn(f'Fitting did not converge for some units: {nonconverged}')
-
+                _logger.warn("Non-converged cells: {}".format(nonconverged))
+        if bestparams:
+            return coefs, intercepts, alphas
         return coefs, intercepts
```

### Comparing `neurencoding-0.1.7/neurencoding/utils.py` & `neurencoding-0.1.8/neurencoding/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Third party libraries
 import numpy as np
 import pandas as pd
 from numpy.matlib import repmat
 from tqdm import tqdm
+from copy import deepcopy
 
 
 def raised_cosine(duration, nbases, binfun):
     """
     Create raised cosine basis functions of durection `duration` with `nbases` bases.
     
     The `binfun` argument is a function that takes a duration in seconds and returns the number of
@@ -131,14 +132,52 @@
         r = np.zeros((ybin.size, r.shape[1]))
         r[iout, :] = _r[ir, :]
         yscale = ybin
 
     return r, xscale, yscale
 
 
+def remove_regressors(design, regressors):
+    """
+    Removes regressors from a design matrix, and reindexes the remaining regressors.
+    Then compiles the resulting modified DM. Useful for doing testing.
+
+
+    Parameters
+    ----------
+    design : neurencoding.DesignMatrix
+        Original design matrix to modify. Must have every element of `regressors` in the
+        `covar` attribute.
+    regressors : list
+        List of string keys to remove from the design matrix.
+
+    Returns
+    -------
+    neurencoding.DesignMatrix
+        Compiled design matrix with the specified regressors removed.
+    """
+    newd = deepcopy(design)
+    newcol_max = 0
+    dkeys = list(newd.covar.keys())
+    for r in dkeys:
+        bases = newd.covar[r]["bases"]
+        if r in regressors:
+            del newd.covar[r]
+            continue
+        if bases is not None:
+            newd.covar[r]["dmcol_idx"] = np.arange(newcol_max, newcol_max + bases.shape[1])
+            newcol_max += bases.shape[1]
+        else:
+            newd.covar[r]["dmcol_idx"] = newcol_max
+            newcol_max += 1
+    newd.currcol = newcol_max
+    newd.compile_design_matrix()
+    return newd
+
+
 class SequentialSelector:
     def __init__(self, model, n_features_to_select=None, direction="forward", scoring=None):
         """
         Sequential feature selection for neural models
 
         Parameters
         ----------
```

### Comparing `neurencoding-0.1.7/neurencoding.egg-info/PKG-INFO` & `neurencoding-0.1.8/neurencoding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurencoding
-Version: 0.1.7
+Version: 0.1.8
 Summary: Neural encoding models made easy. Describe neuronal activity as a function of other variables
 Author-email: Berk Gercek <berkgercek@duck.com>
 Project-URL: Homepage, https://github.com/berkgercek/neurencoding
 Project-URL: Bug Tracker, https://github.com/berkgercek/neurencoding/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neurencoding-0.1.7/pyproject.toml` & `neurencoding-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neurencoding"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
     {name="Berk Gercek", email="berkgercek@duck.com"},
 ]
 description="Neural encoding models made easy. Describe neuronal activity as a function of other variables"
 readme="README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `neurencoding-0.1.7/tests/test_design.py` & `neurencoding-0.1.8/tests/test_design.py`

 * *Files identical despite different names*

