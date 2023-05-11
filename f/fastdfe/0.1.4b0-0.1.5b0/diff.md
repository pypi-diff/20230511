# Comparing `tmp/fastdfe-0.1.4b0.tar.gz` & `tmp/fastdfe-0.1.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastdfe-0.1.4b0.tar", max compression
+gzip compressed data, was "fastdfe-0.1.5b0.tar", max compression
```

## Comparing `fastdfe-0.1.4b0.tar` & `fastdfe-0.1.5b0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      322 2023-05-02 08:38:16.143704 fastdfe-0.1.4b0/README.md
--rw-r--r--   0        0        0     2603 2023-05-04 15:03:08.858314 fastdfe-0.1.4b0/fastdfe/__init__.py
--rw-r--r--   0        0        0    18451 2023-05-04 14:38:07.386884 fastdfe-0.1.4b0/fastdfe/abstract_inference.py
--rw-r--r--   0        0        0    44975 2023-05-04 14:38:07.369531 fastdfe-0.1.4b0/fastdfe/base_inference.py
--rw-r--r--   0        0        0     4762 2023-04-29 08:09:34.806177 fastdfe-0.1.4b0/fastdfe/bootstrap.py
--rw-r--r--   0        0        0     9934 2023-05-03 08:58:25.701024 fastdfe-0.1.4b0/fastdfe/config.py
--rw-r--r--   0        0        0    15051 2023-05-02 14:22:16.509178 fastdfe-0.1.4b0/fastdfe/discretization.py
--rw-r--r--   0        0        0     3902 2023-04-29 08:09:34.792156 fastdfe-0.1.4b0/fastdfe/json_handlers.py
--rw-r--r--   0        0        0     1541 2023-04-29 08:10:05.029271 fastdfe-0.1.4b0/fastdfe/mle.py
--rw-r--r--   0        0        0    35979 2023-05-04 07:31:00.022451 fastdfe-0.1.4b0/fastdfe/optimization.py
--rw-r--r--   0        0        0    21091 2023-05-02 08:38:16.182403 fastdfe-0.1.4b0/fastdfe/parametrization.py
--rw-r--r--   0        0        0    11316 2023-04-29 08:12:55.242293 fastdfe-0.1.4b0/fastdfe/parser.py
--rw-r--r--   0        0        0    12467 2023-05-02 08:38:16.183198 fastdfe-0.1.4b0/fastdfe/polydfe.py
--rw-r--r--   0        0        0     5254 2023-04-29 07:57:26.449161 fastdfe-0.1.4b0/fastdfe/polydfe_utils.py
--rw-r--r--   0        0        0    40670 2023-05-04 14:38:07.348375 fastdfe-0.1.4b0/fastdfe/shared_inference.py
--rw-r--r--   0        0        0    17957 2023-04-28 16:01:50.245576 fastdfe-0.1.4b0/fastdfe/spectrum.py
--rw-r--r--   0        0        0    30801 2023-05-02 11:01:44.227968 fastdfe-0.1.4b0/fastdfe/visualization.py
--rw-r--r--   0        0        0      642 2023-05-04 15:03:08.851472 fastdfe-0.1.4b0/pyproject.toml
--rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 fastdfe-0.1.4b0/PKG-INFO
+-rw-r--r--   0        0        0      795 2023-05-11 10:05:21.534399 fastdfe-0.1.5b0/README.md
+-rw-r--r--   0        0        0     2570 2023-05-11 10:05:21.702400 fastdfe-0.1.5b0/fastdfe/__init__.py
+-rw-r--r--   0        0        0    20068 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/abstract_inference.py
+-rw-r--r--   0        0        0    45394 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/base_inference.py
+-rw-r--r--   0        0        0     4869 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/bootstrap.py
+-rw-r--r--   0        0        0    10146 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/config.py
+-rw-r--r--   0        0        0    15067 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/discretization.py
+-rw-r--r--   0        0        0    41939 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/joint_inference.py
+-rw-r--r--   0        0        0     3902 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/json_handlers.py
+-rw-r--r--   0        0        0     1541 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/mle.py
+-rw-r--r--   0        0        0    36389 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/optimization.py
+-rw-r--r--   0        0        0    21093 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/parametrization.py
+-rw-r--r--   0        0        0    19733 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/parser.py
+-rw-r--r--   0        0        0    12485 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/polydfe.py
+-rw-r--r--   0        0        0     5254 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/polydfe_utils.py
+-rw-r--r--   0        0        0    17957 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/spectrum.py
+-rw-r--r--   0        0        0    28157 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/visualization.py
+-rw-r--r--   0        0        0      642 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/pyproject.toml
+-rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 fastdfe-0.1.5b0/PKG-INFO
```

### Comparing `fastdfe-0.1.4b0/fastdfe/__init__.py` & `fastdfe-0.1.5b0/fastdfe/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 fastDFE package.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-03-10"
 
-__version__ = '0.1.4-beta'
+__version__ = '0.1.5-beta'
 
 import logging
 import sys
 import warnings
 
 import jsonpickle
 import numpy as np
@@ -26,15 +26,14 @@
 jsonpickle.handlers.registry.register(np.ndarray, NumpyArrayHandler)
 
 # configure logger
 logger = logging.getLogger('fastdfe')
 handler = logging.StreamHandler(sys.stdout)
 handler.setFormatter(logging.Formatter('%(levelname)s:%(name)s:%(message)s'))
 logger.addHandler(handler)
-logger.setLevel(logging.INFO)
 
 # whether to disable the progress bar
 disable_pbar = False
 
 
 def raise_on_warning(message, category, filename, lineno, file=None, line=None):
     """
@@ -51,36 +50,36 @@
 
 # load class from modules
 from .parametrization import Parametrization, GammaExpParametrization, DiscreteParametrization, \
     GammaDiscreteParametrization, DisplacedGammaParametrization
 from .config import Config
 from .abstract_inference import Inference
 from .base_inference import BaseInference, InferenceResults
-from .shared_inference import SharedInference, SharedParams
+from .joint_inference import JointInference, SharedParams
 from .optimization import Covariate
 from .visualization import Visualization
 from .spectrum import Spectrum, Spectra
 from .parser import Parser, BaseTransitionStratification, BaseContextStratification, DegeneracyStratification, \
-    TransitionTransversionStratification, ReferenceBaseStratification
+    TransitionTransversionStratification, AncestralBaseStratification
 
 __all__ = [
     'Parametrization',
     'GammaExpParametrization',
     'DiscreteParametrization',
     'GammaDiscreteParametrization',
     'DisplacedGammaParametrization',
     'Config',
     'Inference',
     'BaseInference',
-    'SharedInference',
+    'JointInference',
     'SharedParams',
     'Covariate',
     'Visualization',
     'Spectrum',
     'Spectra',
     'Parser',
     'BaseTransitionStratification',
     'BaseContextStratification',
     'DegeneracyStratification',
     'TransitionTransversionStratification',
-    'ReferenceBaseStratification'
+    'AncestralBaseStratification'
 ]
```

### Comparing `fastdfe-0.1.4b0/fastdfe/abstract_inference.py` & `fastdfe-0.1.5b0/fastdfe/abstract_inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-03-12"
 
 from abc import ABC, abstractmethod
-from typing import List, Optional, Literal
+from typing import List, Optional, Literal, Tuple, Dict
 from typing_extensions import Self
 
 import jsonpickle
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 
@@ -122,16 +122,16 @@
         :param ax: Axes of the plot.
         :param kwargs: Additional arguments for the plot.
         :return: Axes of the plot.
         """
         # get data from inference objects
         values = []
         errors = []
-        for i, inference in enumerate(inferences):
-            val, errs = inference.get_discretized(
+        for i, inf in enumerate(inferences):
+            val, errs = inf.get_discretized(
                 intervals=intervals,
                 confidence_intervals=confidence_intervals,
                 ci_level=ci_level,
                 bootstrap_type=bootstrap_type
             )
 
             values.append(val)
@@ -181,15 +181,15 @@
         if len(inferences) == 0:
             raise ValueError('No inference objects given.')
 
         # get sorted list of parameter names
         param_names = sorted(list(inferences[0].get_bootstrap_param_names()))
 
         # get errors and values
-        errors, values = Inference.get_errors_and_values(
+        errors, values = Inference.get_errors_params_mle(
             bootstrap_type=bootstrap_type,
             ci_level=ci_level,
             confidence_intervals=confidence_intervals,
             inferences=inferences,
             labels=labels,
             param_names=param_names
         )
@@ -204,24 +204,62 @@
             labels=labels,
             scale=scale,
             legend=len(labels) > 1,
             ax=ax
         )
 
     @staticmethod
-    def get_errors_and_values(
+    def get_cis_params_mle(
+            bootstrap_type: Literal['percentile', 'bca'],
+            ci_level: float,
+            inferences: List['AbstractInference'],
+            labels: list | np.ndarray,
+            param_names: list | np.ndarray
+    ) -> dict[str, Optional[Dict[str, Tuple[float, float]]]]:
+        """
+        Get confidence intervals for the MLE parameters.
+
+        :param bootstrap_type: Type of bootstrap to use for confidence intervals.
+        :param ci_level: Confidence level for confidence intervals.
+        :param inferences: List of inference objects.
+        :param labels: Labels for the DFEs.
+        :param param_names: Names of the parameters.
+        :return: Dictionary of confidence intervals indexed by labels.
+        """
+        cis = {}
+        for label, inf in zip(labels, inferences):
+
+            if inf.bootstraps is not None:
+
+                values = list(inf.get_bootstrap_params()[k] for k in param_names)
+
+                res = Bootstrap.get_errors(
+                    values=values,
+                    bs=inf.bootstraps[param_names].to_numpy(),
+                    bootstrap_type=bootstrap_type,
+                    ci_level=ci_level
+                )
+
+                cis[label] = {k: tuple(res[1][:, i]) for i, k in enumerate(param_names)}
+            else:
+                cis[label] = None
+
+        return cis
+
+    @staticmethod
+    def get_errors_params_mle(
             bootstrap_type: Literal['percentile', 'bca'],
             ci_level: float,
             confidence_intervals: bool,
             inferences: List['AbstractInference'],
             labels: list | np.ndarray,
             param_names: list | np.ndarray
     ):
         """
-        Get errors and values for inferences.
+        Get errors and values for MLE params of inferences.
 
         :param bootstrap_type: Type of bootstrap to use.
         :param ci_level: Confidence level for confidence intervals.
         :param confidence_intervals: Whether to compute confidence intervals.
         :param inferences: List of inference objects.
         :param labels: Labels for the inferences.
         :param param_names: Names of the parameters to get errors and values for.
@@ -250,64 +288,70 @@
             else:
                 errors[label] = None
 
         return errors, values
 
     @staticmethod
     def get_discretized(
-            bootstraps: pd.DataFrame,
-            params: dict,
-            model: Parametrization,
+            inferences: List['AbstractInference'],
+            labels: list | np.ndarray,
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile'
 
-    ) -> (np.ndarray, np.ndarray):
+    ) -> (np.ndarray, Optional[np.ndarray]):
         """
-        Get discretized DFE.
+        Get values and errors of discretized DFE.
 
-        :param bootstraps: Bootstrap samples
-        :param params: Parameters of the model
-        :param model: DFE parametrization
+        :param inferences: List of inference objects.
+        :param labels: Labels for the DFEs.
         :param bootstrap_type: Type of bootstrap to use
         :param ci_level: Confidence interval level
         :param confidence_intervals: Whether to compute confidence intervals
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bars.
-        :return: Values, errors
+        :return: Array of values and array of errors
         """
-        if confidence_intervals and bootstraps is not None:
-            # get bootstraps and errors if specified
-            errors, _, bs, means, values = Inference.get_errors_discretized_dfe(
-                params=params,
-                bootstraps=bootstraps,
-                model=model,
-                ci_level=ci_level,
-                intervals=intervals,
-                bootstrap_type=bootstrap_type
-            )
-        else:
-            # otherwise just get discretized values
-            values = Inference.compute_histogram(
-                params=params,
-                model=model,
-                intervals=intervals
-            )
-            errors, means, bs = None, None, None
+        values = {}
+        errors = {}
 
-        # whether to use the mean of all bootstraps instead of the original values
-        use_means = confidence_intervals and bootstraps is not None and bootstrap_type == 'percentile'
+        for label, inf in zip(labels, inferences):
+
+            if confidence_intervals and inf.bootstraps is not None:
+                # get bootstraps and errors if specified
+                errs, _, bs, means, vals = Inference.get_stats_discretized(
+                    params=inf.get_bootstrap_params(),
+                    bootstraps=inf.bootstraps,
+                    model=inf.model,
+                    ci_level=ci_level,
+                    intervals=intervals,
+                    bootstrap_type=bootstrap_type
+                )
+            else:
+                # otherwise just get discretized values
+                vals = Inference.compute_histogram(
+                    params=inf.get_bootstrap_params(),
+                    model=inf.model,
+                    intervals=intervals
+                )
+                errs, means, bs = None, None, None
 
-        if use_means:
-            values = np.mean(bs, axis=0)
+            # whether to use the mean of all bootstraps instead of the original values
+            use_means = confidence_intervals and inf.bootstraps is not None and bootstrap_type == 'percentile'
+
+            if use_means:
+                vals = np.mean(bs, axis=0)
+
+            values[label] = vals
+            errors[label] = errs
 
         return values, errors
 
     @staticmethod
-    def get_errors_discretized_dfe(
+    def get_stats_discretized(
             params: dict,
             bootstraps: pd.DataFrame,
             model: Parametrization | str,
             ci_level: float = 0.05,
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile'
 
@@ -345,15 +389,15 @@
     @staticmethod
     def compute_histogram(
             model: Parametrization | str,
             params: dict,
             intervals: np.ndarray
     ) -> np.ndarray:
         """
-        Discretize the DFE given the DFE parametrization and the parameters.
+        Discretize the DFE given a DFE parametrization and its parameter values.
 
         :param model: DFE parametrization
         :param params: Parameters of the model
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bins.
         :return: Discretized DFE
         """
         # discrete DFE
@@ -375,72 +419,49 @@
         :param kwargs: Keyword arguments
         """
         self.bootstraps: Optional[pd.DataFrame] = None
         self.params_mle: Optional[dict] = None
         self.model: Optional[Parametrization] = None
 
     @abstractmethod
-    def get_bootstrap_params(self) -> dict:
+    def get_bootstrap_params(self) -> Dict[str, float]:
         """
         Get the parameters to be included in the bootstraps.
 
         :return: Parameters to be included in the bootstraps
         """
         pass
 
-    def get_errors_discretized_dfe(
-            self,
-            ci_level: float = 0.05,
-            intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
-            bootstrap_type: Literal['percentile', 'bca'] = 'percentile'
-    ) -> (np.ndarray, np.ndarray, np.ndarray, np.ndarray):
-        """
-        Compute errors and confidence interval for a discretized DFE.
-
-        :param ci_level: Confidence interval level
-        :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bins.
-        :param bootstrap_type: Type of bootstrap
-        :return: Arrays of errors, confidence intervals, bootstraps, means and values
-        """
-        return Inference.get_errors_discretized_dfe(
-            params=self.get_bootstrap_params(),
-            bootstraps=self.bootstraps,
-            model=self.model,
-            ci_level=ci_level,
-            intervals=intervals,
-            bootstrap_type=bootstrap_type
-        )
-
     def get_discretized(
             self,
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile'
-
     ) -> (np.ndarray, np.ndarray):
         """
         Get discretized DFE.
 
         :param bootstrap_type: Type of bootstrap
         :param ci_level: Confidence interval level
         :param confidence_intervals: Whether to return confidence intervals
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bins.
-        :return: Discretized DFE
+        :return: Array of values and array of errors
         """
-        return Inference.get_discretized(
-            bootstraps=self.bootstraps,
-            params=self.get_bootstrap_params(),
-            model=self.model,
+        values, errors = Inference.get_discretized(
+            inferences=[self],
+            labels=['all'],
             intervals=intervals,
             confidence_intervals=confidence_intervals,
             ci_level=ci_level,
             bootstrap_type=bootstrap_type
         )
 
+        return values['all'], errors['all']
+
     def plot_discretized(
             self,
             file: str = None,
             show: bool = True,
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
@@ -469,14 +490,39 @@
             confidence_intervals=confidence_intervals,
             ci_level=ci_level,
             bootstrap_type=bootstrap_type,
             title=title,
             ax=ax
         )
 
+    def get_cis_params_mle(
+            self,
+            bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
+            ci_level: float = 0.05,
+            param_names: Optional[list[str]] = None
+    ):
+        """
+        Get confidence intervals for the parameters.
+
+        :param bootstrap_type: Type of bootstrap
+        :param ci_level: Confidence interval level
+        :param param_names: Names of the parameters to return confidence intervals for
+        :return: Confidence intervals for the parameters
+        """
+        if param_names is None:
+            param_names = self.get_bootstrap_param_names()
+
+        return Inference.get_cis_params_mle(
+            inferences=[self],
+            bootstrap_type=bootstrap_type,
+            ci_level=ci_level,
+            param_names=param_names,
+            labels=['all']
+        )['all']
+
     def to_json(self) -> str:
         """
         Serialize object.
 
         :return: JSON string
         """
         return jsonpickle.encode(self, indent=4, warn=True)
```

### Comparing `fastdfe-0.1.4b0/fastdfe/base_inference.py` & `fastdfe-0.1.5b0/fastdfe/base_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from typing_extensions import Self
 
 from . import parametrization, optimization
 from .abstract_inference import AbstractInference, Inference
 from .config import Config
 from .discretization import Discretization
 from .json_handlers import CustomEncoder
-from .optimization import Optimization, flatten_dict, pack_params, expand_fixed, scale_values, unpack_shared
+from .optimization import Optimization, flatten_dict, pack_params, expand_fixed, unpack_shared
 from .parametrization import Parametrization, from_string
 from .spectrum import Spectrum, Spectra
 from .spectrum import standard_kingman
 from .visualization import Visualization
 
 # get logger
 logger = logging.getLogger('fastdfe')
@@ -93,18 +93,20 @@
             optimization: Optimization = None,
             locked: bool = False,
             **kwargs
     ):
         """
         Create BaseInference instance.
 
-        :param sfs_neut: The neutral SFS. Spectra | Spectrum
-        :param sfs_sel: The selected SFS.
+        :param sfs_neut: The neutral SFS. Note that we require monomorphic counts to be specified in order to infer
+            the mutation rate.
+        :param sfs_sel: The selected SFS. Note that we require monomorphic counts to be specified in order to infer
+            the mutation rate.
         :param intervals_del: ``(start, stop, n_interval)`` for deleterious population-scaled
-        selection coefficients. The intervals will be log10-spaced.
+            selection coefficients. The intervals will be log10-spaced.
         :param intervals_ben: Same as for intervals_del but for beneficial selection coefficients.
         :param model: Instance of DFEParametrization which parametrized the DFE
         :param seed: Seed for the random number generator.
         :param x0: Dictionary of initial values in the form {'all': {param: value}}
         :param bounds: Bounds for the optimization in the form {param: (lower, upper)}
         :param scales: Scales for the optimization in the form {param: scale}
         :param loss_type: Type of loss function to use for optimization.
@@ -133,14 +135,19 @@
         if isinstance(sfs_sel, Spectra):
             #: Selected SFS
             self.sfs_sel: Spectrum = sfs_sel.all
         else:
             # assume we have Spectrum object
             self.sfs_sel: Spectrum = sfs_sel
 
+        # check that we have monomorphic counts
+        if self.sfs_neut.to_list()[0] == 0 or self.sfs_sel.to_list()[0] == 0:
+            raise ValueError('Some of the provided SFS have zero ancestral monomorphic counts. '
+                             'Note that we require monomorphic counts in order to infer the mutation rate.')
+
         #: Sample size
         self.n: int = sfs_neut.n
 
         #: The DFE parametrization
         self.model: Parametrization = parametrization.from_string(model)
 
         if discretization is None:
@@ -394,21 +401,19 @@
         """
         return dict(all=lambda params: self.model_sfs(
             params,
             sfs_neut=self.sfs_neut,
             sfs_sel=self.sfs_sel
         ))
 
-    def evaluate_likelihood(self, params: dict) -> float:
+    def evaluate_likelihood(self, params: Dict[str, Dict[str, float]]) -> float:
         """
-        Get loss function.
-        Note that the order of the parameters has to be the same as in
-        params_mle. The types also need to be specified here. For a
-        BaseInference objects, the mean we need to pass dict(all=...).
+        Evaluate likelihood function at given parameters.
 
+        :param params: Parameters indexed by type and parameter name.
         :return: The likelihood.
         """
         x0_cached = self.optimization.x0
         self.optimization.x0 = params
 
         # prepare parameters
         params = pack_params(self.optimization.scale_values(flatten_dict(params)))
@@ -433,15 +438,15 @@
         # get SFS for MLE parameters
         counts_mle, _ = self.model_sfs(
             params=params_mle,
             sfs_neut=self.sfs_neut,
             sfs_sel=self.sfs_sel
         )
 
-        # add monomorphic classes and create Spectrum object
+        # create spectrum object from polymorphic counts
         self.sfs_mle = Spectrum.from_polymorphic(counts_mle)
 
         # L2 norm of fit minus observed SFS
         self.L2_residual = norm(self.sfs_mle.polymorphic - self.sfs_sel.polymorphic, 2)
 
     @staticmethod
     def report_result(result: OptimizeResult, params: dict):
@@ -901,15 +906,15 @@
         Get the discretized DFE errors.
 
         :param ci_level: Confidence interval level.
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bins.
         :param bootstrap_type: Type of bootstrap to use.
         :return: Arrays of errors, confidence intervals, bootstraps, means and values
         """
-        return Inference.get_errors_discretized_dfe(
+        return Inference.get_stats_discretized(
             params=self.params_mle,
             bootstraps=self.bootstraps,
             model=self.model,
             ci_level=ci_level,
             intervals=intervals,
             bootstrap_type=bootstrap_type
         )
```

### Comparing `fastdfe-0.1.4b0/fastdfe/bootstrap.py` & `fastdfe-0.1.5b0/fastdfe/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,17 @@
         """
         Get the (1 - a)% confidence intervals using the percentile bootstrap.
 
         :param bootstraps: List of bootstraps
         :param a: Confidence level
         :return: lower bound and upper bound
         """
+        if not 0 <= a <= 0.5:
+            raise ValueError('Confidence level must be between 0 and 0.5.')
+
         return Bootstrap.get_bounds_from_quantile(np.sort(bootstraps), a, 1 - a, len(bootstraps))
 
     @staticmethod
     def get_ci_bca(bootstraps: list | np.ndarray, original: float, a: float) -> (float, float):
         """
         Get the (1 - a)% confidence intervals using the BCa method.
         cf. An Introduction to the Bootstrap, Bradley Efron, Robert J. Tibshirani, section 14.2.
```

### Comparing `fastdfe-0.1.4b0/fastdfe/config.py` & `fastdfe-0.1.5b0/fastdfe/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 logger = logging.getLogger('fastdfe')
 
 
 class Config:
     """
     Configuration class to be used for :class:``~fastdfe.base_inference.BaseInference`` and
-    :class:``fastdfe.shared_inference.SharedInference``.
+    :class:``fastdfe.joint_inference.JointInference``.
     """
 
     def __init__(
             self,
             polydfe_spectra_config: str = None,
             polydfe_init_file: str = None,
             polydfe_init_file_id: int = 1,
@@ -56,29 +56,31 @@
     ):
         """
         Create config object.
 
         :param polydfe_spectra_config: Path to polyDFE SFS config file.
         :param polydfe_init_file: Path to polyDFE init file.
         :param polydfe_init_file_id: ID of polyDFE init file.
-        :param sfs_neut: Neutral SFS.
-        :param sfs_sel: Selected SFS.
+        :param sfs_neut: Neutral SFS. Note that we require monomorphic counts to be specified in order to infer
+            the mutation rate.
+        :param sfs_sel: Selected SFS. Note that we require monomorphic counts to be specified in order to infer
+            the mutation rate.
         :param intervals_del: Integration intervals for deleterious mutations in log space.
         :param intervals_ben: Integration intervals for beneficial mutations in log space.
         :param integration_mode: Integration mode.
         :param linearized: Whether to use the linearized version of the DFE.
         :param model: Parametrization of the DFE.
         :param seed: Seed for the random number generator.
         :param x0: Dictionary of initial values in the form ``{type: {param: value}}``
         :param bounds: Bounds for the optimization in the form {param: (lower, upper)}
         :param scales: Scales for the optimization in the form {param: scale}
         :param loss_type: Loss function to use.
         :param opts_mle: Options for the optimization.
         :param n_runs: Number of optimization runs. Number of optimization runs.
-        The first run will use the initial values if provided.
+            The first run will use the initial values if provided.
         :param fixed_params: Fixed parameters for the optimization.
         :param shared_params: Shared parameters for the optimization.
         :param covariates: Covariates for the optimization.
         :param do_bootstrap: Whether to do bootstrapping automatically.
         :param n_bootstraps: Number of bootstraps.
         :param parallelize: Whether to parallelize the optimization.
         """
```

### Comparing `fastdfe-0.1.4b0/fastdfe/discretization.py` & `fastdfe-0.1.5b0/fastdfe/discretization.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,18 +33,18 @@
 
     return s, interval_sizes
 
 
 def get_bins(intervals_del: tuple, intervals_ben: tuple) -> np.ndarray:
     """
     Get bins using log-spaced distances for positive and negative
-    values of S given by intervals_ben and intervals_del, respectively.
+    values of S given by ``intervals_ben`` and ``intervals_del``, respectively.
 
-    :param intervals_del: (min, max, n) for negative values of S where we use log-spaced distances
-    :param intervals_ben: (min, max, n) for positive values of S where we use log-spaced distances
+    :param intervals_del: ``(min, max, n)`` for negative values of S where we use log-spaced distances
+    :param intervals_ben: ``(min, max, n)`` for positive values of S where we use log-spaced distances
     :return: Bins
     """
     bins_del = -np.logspace(np.log10(np.abs(intervals_del[0])),
                             np.log10(np.abs(intervals_del[1])), intervals_del[2] + 1)
 
     bins_ben = np.logspace(np.log10(intervals_ben[0]), np.log10(intervals_ben[1]), intervals_ben[2] + 1)
```

### Comparing `fastdfe-0.1.4b0/fastdfe/json_handlers.py` & `fastdfe-0.1.5b0/fastdfe/json_handlers.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.4b0/fastdfe/mle.py` & `fastdfe-0.1.5b0/fastdfe/mle.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.4b0/fastdfe/optimization.py` & `fastdfe-0.1.5b0/fastdfe/optimization.py`

 * *Files 3% similar despite different names*

```diff
@@ -316,23 +316,25 @@
     return result
 
 
 def correct_values(
         params: Dict[str, float],
         bounds: Dict[str, Tuple[float, float]],
         scales: Dict[str, Literal['lin', 'log', 'symlog']],
-        warn: bool = False
+        warn: bool = False,
+        threshold: float = 1e-6
 ) -> Dict[str, float]:
     """
     Correct initial values so that they are within the specified bounds.
 
     :param bounds: Dictionary of bounds
     :param params: Flattened dictionary of parameters
     :param scales: Dictionary of scales
     :param warn: Whether to warn if values are corrected
+    :param threshold: Threshold for the error to trigger a warning
     :return: Corrected dictionary
     """
     # create a copy of params
     corrected = params.copy()
 
     for key, value in params.items():
         # get base name
@@ -344,19 +346,29 @@
         # correct value if outside bounds
         if value < bound[0]:
             corrected[key] = bound[0]
         elif value > bound[1]:
             corrected[key] = bound[1]
 
     # differences between the original and corrected dictionaries
-    differences = {key: f"{params[key]} -> {corrected[key]}" for key in params if params[key] != corrected[key]}
+    differences = {key: (params[key], corrected[key]) for key in params if params[key] != corrected[key]}
 
-    # warn if there are differences
-    if differences and warn:
-        logger.warning(f'Given initial values outside bounds. Adjusting {differences}.')
+    # warn if there are differences that exceed the threshold
+    exceeded_threshold = {}
+    for key, (old_val, new_val) in differences.items():
+
+        # calculate relative error
+        err = np.abs(new_val - old_val)
+
+        # add if it exceeds the relative error
+        if err > threshold:
+            exceeded_threshold[key] = f"{old_val} -> {new_val}"
+
+    if exceeded_threshold and warn:
+        logger.warning(f'Given initial values outside bounds. Adjusting {exceeded_threshold}.')
 
     return corrected
 
 
 def get_real_bounds(bounds: Tuple[float, float], scale: Literal['lin', 'log', 'symlog']) -> Tuple[float, float]:
     """
     Get real bounds from the given bounds.
@@ -394,15 +406,15 @@
 
 def to_symlog(x: float, linthresh: float = 1e-5) -> float:
     """
     Convert a value to the symlog scale.
 
     :param x: The input value on the original scale.
     :param linthresh: The positive value that determines the range within which the
-                      symlog scale is linear. Must be greater than 0.
+        symlog scale is linear. Must be greater than 0.
     :return: The value on the symlog scale.
     """
     sign = np.sign(x)
     abs_x = np.abs(x)
     log_x = np.log10(abs_x + linthresh) - np.log10(linthresh)
 
     return sign * (abs_x / linthresh if abs_x <= linthresh else log_x)
@@ -410,15 +422,15 @@
 
 def from_symlog(y: float, linthresh: float = 1e-5) -> float:
     """
     Convert a value from the symlog scale back to the original scale.
 
     :param y: The input value on the symlog scale.
     :param linthresh: The positive value that determines the range within which the
-                      symlog scale is linear. Must be greater than 0.
+        symlog scale is linear. Must be greater than 0.
     :return: The value on the original scale.
     """
     sign = np.sign(y)
     abs_y = np.abs(y)
     exp_y = np.power(10, abs_y + np.log10(linthresh)) - linthresh
 
     return sign * (abs_y * linthresh if abs_y <= 1 else exp_y)
@@ -768,15 +780,15 @@
         Perform the optimization procedure.
 
         :param scales: Scales of the parameters
         :param bounds: Bounds of the parameters
         :param pbar: Whether to show a progress bar
         :param print_info: Whether to inform the user about the bounds
         :param n_runs: Number of optimization runs. Number of optimization runs. The first run will use the
-        initial values if provided.
+            initial values if provided.
         :param x0: Dictionary of initial values in the form ``{type: {param: value}}``
         :param get_counts: Dictionary of functions to evaluate counts for each type
         :param debug_iterations: Whether to print debug messages for each iteration
         :return: The optimization result and the likelihoods
         """
         # number of optimization runs
         self.n_runs = n_runs
```

### Comparing `fastdfe-0.1.4b0/fastdfe/parametrization.py` & `fastdfe-0.1.5b0/fastdfe/parametrization.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 class Parametrization:
     """
     Base class for parametrizing a DFE by a set of parameters.
     Note that :func:`get_pdf` is not required to be implemented, provided that the
     linearized mode of fastDFE is used (which is highly recommended).
     """
+
     #: Default initial parameters
     x0 = {}
 
     #: Default parameter bounds
     bounds = {}
 
     #: The kind of submodels supported by holding some parameters fixed
@@ -514,15 +515,15 @@
     such that :math:`\sum_{i=1}^{k} S_i = 1,`
 
     where :math:`B_i` and :math:`c_i` are interval :math:`i` and the width of interval :math:`i`, respectively.
 
     This parametrization has the advantage of not imposing a shape on the DFE. For a reasonably fine parametrization,
     the number of parameters is larger than those of the other models, however. We generally also observe larger
     confidence intervals for this parametrization, and the optimization procedure may well be less efficient as
-    we have to renormalize the parameters to make sure they sum up to 1.
+    we have to re-normalize the parameters to make sure they sum up to 1.
     """
 
     def __init__(
             self,
             intervals: np.ndarray = np.array([-100000, -100, -10, -1, 0, 1, 1000])
     ):
         """
```

### Comparing `fastdfe-0.1.4b0/fastdfe/parser.py` & `fastdfe-0.1.5b0/fastdfe/polydfe.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,391 +1,421 @@
 """
-Parser module.
+polyDFE wrapper utilities.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
-__date__ = "2023-03-26"
+__date__ = "2023-02-26"
 
-import gzip
-import itertools
+import copy
+import json
 import logging
-from abc import ABC, abstractmethod
-from typing import List, Callable, Literal, Optional, TextIO
+import subprocess
+import tempfile
+import time
+from typing import Callable, List, Optional, Literal, Dict
 
 import numpy as np
-from cyvcf2 import VCF, Variant
-from pyfaidx import Fasta
-from tqdm import tqdm
-
-from .spectrum import Spectra
+import pandas as pd
+import rpy2.robjects as ro
+from matplotlib import pyplot as plt
+from rpy2.robjects.packages import importr
+from rpy2.robjects.vectors import ListVector
+from typing_extensions import Self
+
+from .abstract_inference import AbstractInference, Inference
+from .config import Config
+from .parametrization import from_string, Parametrization, DiscreteParametrization
+from .polydfe_utils import create_sfs_config, models
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
-#: the DNA bases
-bases = ["A", "C", "G", "T"]
-
-
-class NoTypeException(BaseException):
-    """
-    Exception thrown when no type can be determined.
-    """
-    pass
-
 
-class Stratification(ABC):
+class PolyDFEResult:
     """
-    Abstract class for Stratifying the SFS by determining
-    a site's type based on its properties.
+    Class for parsing polyDFE output.
     """
+    # default postprocessing source
+    default_postprocessing_source = '../resources/polydfe/postprocessing/script.R'
 
-    @abstractmethod
-    def get_type(self, variant: Variant) -> Optional[str]:
-        """
-        Get type of given Variant. Only the types
-        given by :meth:`get_types()` are valid, or ``None`` if
-        no type could be determined.
-
-        :param variant: The vcf site
-        :return: Type of the variant
-        """
-        pass
+    # mapping of polyDFE params to new name
+    param_mapping = dict(
+        eps_an='eps'
+    )
 
-    @abstractmethod
-    def get_types(self) -> List[str]:
+    def __init__(
+            self,
+            output_file: str,
+            additional_data: dict = {},
+            postprocessing_source: str = default_postprocessing_source
+    ):
         """
-        Get all possible types.
+        Create summary object.
 
-        :return: List of types
+        :param output_file: Path to polyDFE output file
+        :param additional_data: Additional data to add to summary
+        :param postprocessing_source: Path to polyDFE postprocessing script
         """
-        pass
-
-
-class BaseContextStratification(Stratification):
-    """
-    Stratify the SFS by the base context of the mutation. The number of flanking bases
-    can be configured.
-    """
-
-    def __init__(self, fasta_file: str, n_flanking: int = 1):
-        self.fasta_file = fasta_file
-        self.n_flanking = n_flanking
+        self.output_file = output_file
+        self.postprocessing_source = postprocessing_source
 
-        # load reference genome
-        self.reference = Fasta(self.fasta_file)
+        self.data = self.parse_output() | additional_data
 
-    def get_type(self, variant: Variant) -> str:
+    @staticmethod
+    def map_name(name: str) -> str:
         """
-        Get the base context for a given mutation with k flanking bases.
+        Map polyDFE parameter name to new name.
 
-        :param variant: The vcf site
-        :return: Base context of the mutation with k flanking bases
+        :param name: polyDFE parameter name
+        :return: New name
         """
-        pos = variant.POS - 1
-        ref = variant.REF
-
-        # retrieve the sequence of the chromosome from the reference genome
-        sequence = self.reference[variant.CHROM][:].seq
-
-        if pos < 0 or pos >= len(sequence):
-            raise NoTypeException("Invalid position: Position must be within the bounds of the sequence.")
-
-        upstream_start = max(0, pos - self.n_flanking)
-        upstream_bases = sequence[upstream_start:pos]
-
-        downstream_end = min(len(sequence), pos + self.n_flanking + 1)
-        downstream_bases = sequence[pos + 1:downstream_end]
+        if name in PolyDFEResult.param_mapping:
+            return PolyDFEResult.param_mapping[name]
 
-        return f"{upstream_bases}{ref}{downstream_bases}"
+        return name
 
-    def get_types(self) -> List[str]:
+    def parse_output(self) -> dict:
         """
-        Create all possible base context with for self.k flanking bases.
-        If self.use_transitions is True, include the transition to the alternate base.
+        Parse output from polyDFE output file.
 
-        :return: List of contexts
+        :return: Dictionary of parsed data
         """
-        return [''.join(c) for c in itertools.product(bases, repeat=2 * self.n_flanking + 1)]
+        # use the polyDFE R postprocessing script to parse the output file
+        output = self.get_postprocessing_wrapper().parseOutput(self.output_file)[0]
 
+        # convert to JSON
+        rj = importr('RJSONIO')
+        json_str = rj.toJSON(output)[0]
 
-class BaseTransitionStratification(Stratification):
-    """
-    Stratify the SFS by the base transition of the mutation, i.e. A>T.
-    """
+        # load dict from JSON string
+        data = json.loads(json_str)
 
-    def get_type(self, variant: Variant) -> str:
-        """
-        Get the base context for a given mutation with k flanking bases.
+        return dict(
+            output_file=data['input'],
+            model=data['model'],
+            likelihood=data['lk'],
+            criteria=data['criteria'],
+            params_mle=dict(
+                # non-nuisance parameters
+                # map polyDFE param name to new name
+                (PolyDFEResult.map_name(k), v) for k, v in data['values'][0].items() if not k.startswith('r ')
+            ) | dict(
+                # nuisance parameters
+                r=[data['values'][0][f"r {i}"] for i in range(2, data['n'])]
+            ),
+            n=data['n'],
+            expec=data['expec'][0],
+            alpha=self.get_alpha(output)
+        )
 
-        :param variant: The vcf site
-        :return: Base context of the mutation with k flanking bases
+    def get_alpha(self, parsed_output: ListVector) -> float:
         """
-        # assume there is at most one alternate allele
-        alt = variant.ALT[0] if len(variant.ALT) != 0 else variant.REF
-
-        return f"{variant.REF}>{alt}"
+        Get alpha, the proportion of beneficial non-synonymous substitutions.
 
-    def get_types(self) -> List[str]:
+        :return: Parsed output from polyDFE
         """
-        Create all possible base context with for self.k flanking bases.
+        return self.get_postprocessing_wrapper().estimateAlpha(parsed_output)[0]
 
-        :return: List of contexts
+    def get_postprocessing_wrapper(self) -> ro.R:
         """
-        return ['>'.join(c) for c in itertools.product(bases, repeat=2)]
+        Get the wrapped polyDFE postprocessing source.
 
+        :return: R object
+        """
+        ps = ro.r
+        ps.source(self.postprocessing_source)
 
-class ReferenceBaseStratification(Stratification):
-    """
-    Stratify the SFS by the base context of the mutation: the reference base.
-    """
+        return ps
 
-    def get_type(self, variant: Variant) -> str:
+    def to_json(self) -> str:
         """
-        Get the base of the reference allele.
+        Convert object to JSON.
 
-        :param variant: The vcf site
-        :return: Base context of the mutation with k flanking bases
+        :return: JSON string
         """
-        return variant.REF
+        return json.dumps(self.data, indent=4)
 
-    def get_types(self) -> List[str]:
+    def to_file(self, file: str):
         """
-        Create all possible base context with for self.k flanking bases.
+        Save object to file.
 
-        :return: List of contexts
+        :return: File path to save to
         """
-        return bases
+        with open(file, 'w') as fh:
+            fh.write(self.to_json())
 
 
-class TransitionTransversionStratification(BaseTransitionStratification):
+class PolyDFE(AbstractInference):
     """
-    Stratify the SFS by whether we have a transition or transversion.
+    polyDFE wrapper.
+
+    Note that this class has dependencies outside of pip.
+    Currently only model C is fully implemented.
     """
 
-    def get_type(self, variant: Variant) -> str:
+    def __init__(self, config: Config):
         """
-        Get the mutation type (transition or transversion) for a given mutation.
+        Create polyDFE wrapper.
 
-        :param variant: The vcf site
-        :return: Mutation type ("transition" or "transversion")
+        :param config: Config object
         """
-        # assume there is at most one alternate allele
-        alt = variant.ALT[0] if len(variant.ALT) != 0 else variant.REF
+        super().__init__()
 
-        ref = variant.REF
-        if (ref, alt) in [('A', 'G'), ('G', 'A'), ('C', 'T'), ('T', 'C')]:
-            return "transition"
-        else:
-            return "transversion"
+        self.config = config
 
-    def get_types(self) -> List[str]:
-        """
-        Create all possible mutation types (transition and transversion).
+        # polyDFE output file
+        self.output_file: Optional[str] = None
 
-        :return: List of mutation types
-        """
-        return ["transition", "transversion"]
+        # the total execution time in seconds
+        self.execution_time: float = 0
 
+        # polyDFE summary
+        self.summary: Optional[PolyDFEResult] = None
 
-class DegeneracyStratification(Stratification):
-    """
-    Stratify SFS by degeneracy, i.e. whether a site is 4-fold degenerate (neutral) or 0-fold degenerate (selected).
-    """
+        # bootstrap samples
+        self.bootstraps: Optional[pd.DataFrame] = None
 
-    def __init__(self, custom_callback: Callable[[Variant], str] = None):
+    @staticmethod
+    def map_polydfe_model(model: str) -> str:
         """
-        Initialize the stratification.
+        Map polyDFE model name to native equivalent.
 
-        :param custom_callback: Custom callback to determine the type of mutation
+        :param model: polyDFE model name
+        :return: Native model name
         """
-        self.get_degeneracy = custom_callback if custom_callback is not None else self.get_degeneracy_default
+        return {v: k for k, v in models.items()}[model]
 
-    @staticmethod
-    def get_degeneracy_default(variant: Variant) -> Optional[Literal['neutral', 'selected']]:
+    @classmethod
+    def from_config(cls, config: Config) -> Self:
         """
-        Get degeneracy based on 'Degeneracy' tag.
+        Load from config object.
 
-        :param variant: The vcf site
-        :return: Type of the mutation
+        :param config: Config object
         """
-        degeneracy = variant.INFO.get('Degeneracy')
-
-        if degeneracy is None:
-            raise NoTypeException("Degeneracy tag not found.")
-        else:
-            if degeneracy == 4:
-                return 'neutral'
-
-            if degeneracy == 0:
-                return 'selected'
+        return cls(config)
 
-            raise NoTypeException(f"Degeneracy tag has invalid value: {degeneracy}")
-
-    def get_type(self, variant: Variant) -> Literal['neutral', 'selected']:
+    @classmethod
+    def from_config_file(cls, file: str) -> Self:
         """
-        Get the base context for a given mutation with k flanking bases.
-
-        :param variant: The vcf site
-        :return: Type of the mutation
-        :raises NoTypeException: If the mutation is not synonymous or non-synonymous
+        Load from config object.
         """
-        return self.get_degeneracy(variant)
+        return cls.from_config(Config.from_file(file))
 
-    def get_types(self) -> List[str]:
+    def run(
+            self,
+            output_file: str,
+            bin: str = 'polydfe',
+            wd: str = None,
+            execute: Callable = None,
+            postprocessing_source: str = PolyDFEResult.default_postprocessing_source
+    ) -> PolyDFEResult:
         """
-        Return possible types
-        :return: List of contexts
+        Run polyDFE.
+
+        :param postprocessing_source: polyDFE postprocessing source
+        :param execute: Function for executing shell commands
+        :param wd: Working directory
+        :param bin: polyDFE binary
+        :param output_file: Output file
+        :return: polyDFE summary
         """
-        return ['neutral', 'selected']
+        start_time = time.time()
 
+        def shell(command: str):
+            """
+            Execute shell command.
 
-class Parser:
-    def __init__(
-            self,
-            vcf_file: str,
-            n: int,
-            info_ancestral: str = 'AA',
-            stratifications: List[Stratification] = [
-                DegeneracyStratification()
-            ],
-            max_sites=np.inf,
-            seed: int = 0
-    ):
+            :param command: Command string
+            """
+            return subprocess.run(command, check=True, cwd=wd, shell=True)
 
-        self.n = n
-        self.vcf_file = vcf_file
+        # define default function for executing command
+        if execute is None:
+            execute = shell
 
-        self.info_ancestral = info_ancestral
+        # save the spectra and init file, so they can be reviewed if necessary
+        # use tempfile to generate the file name.
+        with open(tempfile.NamedTemporaryFile().name, 'w') as spectra_file:
+            with open(tempfile.NamedTemporaryFile().name, 'w') as init_file:
+                # save files
+                self.config.create_polydfe_sfs_config(spectra_file.name)
+                self.config.create_polydfe_init_file(init_file.name, n=self.config.data['sfs_neut'].n)
 
-        self.stratifications = stratifications
+                # add number of fragment if model is DiscreteParametrization
+                model = from_string(self.config.data['model'])
+                k = str(model.k - 1) + ' ' if isinstance(model, DiscreteParametrization) else ''
 
-        self.max_sites = max_sites
-        self.seed = seed
+                # construct command string
+                command = (f"{bin} "
+                           f"-d {spectra_file.name} "
+                           f"-m {self.config.get_polydfe_model()} {k}"
+                           f"-i {init_file.name} 1 "
+                           f"-v 1 > {output_file}")
 
-        # get a random generator instance
-        self.rng = np.random.default_rng(seed=seed)
+                # log command signature
+                logger.info(f"Running: {command}")
 
-        self.sfs = self.create_sfs_dictionary()
+                # execute command
+                execute(command)
 
-    @staticmethod
-    def open_file(file: str) -> TextIO:
-        """
-        Open a file, either gzipped or not.
-        :param file:
-        :return: stream
-        """
-        if file.endswith('.gz'):
-            return gzip.open(file, "rt")
+        # add execution time
+        self.execution_time += time.time() - start_time
+
+        # create summary from output file
+        self.summary = PolyDFEResult(
+            output_file=output_file,
+            additional_data=dict(execution_time=self.execution_time),
+            postprocessing_source=postprocessing_source
+        )
 
-        return open(file, 'r')
+        return self.summary
 
-    def count_lines_vcf(self):
+    def create_bootstrap(self) -> Config:
         """
-        Count the number of sites in the VCF file.
+        Create a bootstrap sample using polyDFE's resampling.
+
+        :return: Config object
         """
-        from . import disable_pbar
+        if self.summary is None:
+            raise Exception('PolyDFE needs to be run before creating bootstrap samples.')
 
-        i = 0
+        # postprocessing wrapper
+        ps = self.summary.get_postprocessing_wrapper()
 
-        logger.info('Counting number of sites.')
+        # create temporary SFS config file
+        with tempfile.NamedTemporaryFile() as tmp:
+            create_sfs_config(
+                file=tmp.name,
+                sfs_neut=self.config.data['sfs_neut']['all'],
+                sfs_sel=self.config.data['sfs_sel']['all']
+            )
 
-        with self.open_file(self.vcf_file) as f:
+            # create bootstrap SFS config
+            ps.bootstrapData(tmp.name, rep=1)
 
-            with tqdm(disable=disable_pbar) as pbar:
-                for line in f:
-                    if not line.startswith('#'):
-                        i += 1
-                        pbar.update()
+            # file name of resampled SFS config
+            sfs_config_file = tmp.name + '_1'
 
-                    # stop counting if max_sites was reached
-                    if i >= self.max_sites:
-                        break
+            # use exiting config as template and load init and SFS file
+            config = copy.deepcopy(self.config)
+            config.parse_polydfe_sfs_config(sfs_config_file)
+            config.data['x0'] = dict(all=self.summary.data['params_mle'])
 
-        return i
+        return config
 
-    def create_sfs_dictionary(self) -> dict:
+    def add_bootstraps(self, bootstraps: 'List[PolyDFE]'):
         """
-        Create an SFS dictionary initialized with all possible base contexts.
+        Add bootstraps samples.
 
-        :return: SFS dictionary
+        :param bootstraps: List of bootstrap samples
         """
-        types = [s.get_types() for s in self.stratifications]
-        # define the DNA bases
-        contexts = ['.'.join(t) for t in itertools.product(*types)]
+        # load MLE params into dataframe
+        self.bootstraps = pd.DataFrame([bs.get_bootstrap_params() for bs in bootstraps])
 
-        # create dict
-        sfs = {}
-        for context in contexts:
-            sfs[context] = np.zeros(self.n + 1)
+        # drop nuisance parameters and eps_cont
+        self.bootstraps.drop(columns=['r', 'eps_cont'], inplace=True)
 
-        return sfs
+        # update execution time
+        self.summary.data['execution_time'] += np.sum([bs.summary.data['execution_time'] for bs in bootstraps])
 
-    def parse(self) -> Spectra:
+    def plot_all(self, show: bool = True):
         """
-        Parse the VCF file and return the SFS.
-        :return: the spectra for the different stratifications
+        Plot everything.
         """
+        self.plot_inferred_parameters(show=show)
+        self.plot_discretized(show=show)
 
-        from . import disable_pbar
-
-        sfs = self.create_sfs_dictionary()
-
-        representation = '.'.join(['[' + ','.join(s.get_types()) + ']' for s in self.stratifications])
-        logger.info(f'Using stratification: {representation}.')
-
-        n_sites = self.count_lines_vcf()
-
-        # parse VCF file
-        vcf = VCF(self.vcf_file)
+    def plot_inferred_parameters(
+            self,
+            confidence_intervals: bool = True,
+            ci_level: float = 0.05,
+            bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
+            file: str = None,
+            show: bool = True,
+            title: str = 'parameter estimates',
+            scale: Literal['lin', 'log', 'symlog'] = 'log',
+            legend: bool = True,
+            ax: plt.Axes = None,
+    ) -> plt.Axes:
+        """
+        Visualize the inferred parameters and their confidence intervals.
 
-        logger.info(f'Starting to parse.')
+        :param scale: Scale of the y-axis
+        :param legend: Show legend
+        :param ax: Axes object
+        :param title: Title of the plot
+        :param show: Show the plot
+        :param file: File to save the plot to
+        :param show: Show the plot
+        :param ax: Axes object
+        :return: Axes object
+        """
+        return Inference.plot_inferred_parameters(
+            inferences=[self],
+            labels=['all'],
+            confidence_intervals=confidence_intervals,
+            ci_level=ci_level,
+            bootstrap_type=bootstrap_type,
+            file=file,
+            show=show,
+            title=title,
+            legend=legend,
+            scale=scale,
+            ax=ax
+        )
 
-        with tqdm(total=n_sites, disable=disable_pbar) as pbar:
-            for i, variant in enumerate(vcf):
+    def get_bootstrap_param_names(self) -> List[str]:
+        """
+        Parameter names for parameters included in bootstraps.
 
-                # stop if max_sites was reached
-                if i >= self.max_sites:
-                    break
+        :return: List of parameter names
+        """
+        return from_string(self.config.data['model']).param_names + ['eps', 'alpha']
 
-                # just update beforehand
-                pbar.update()
+    def get_bootstrap_params(self) -> Dict[str, float]:
+        """
+        Get the parameters to be included in the bootstraps.
 
-                n_samples = variant.ploidy * variant.num_called
+        :return: Dict of parameters
+        """
+        params = self.summary.data['params_mle'] | dict(alpha=self.summary.data['alpha'])
 
-                if n_samples < self.n:
-                    continue
+        # filter params
+        return dict((k, params[k]) for k in self.get_bootstrap_param_names())
 
-                # determine reference allele count
-                # this doesn't work for polyploids
-                n_ref = variant.ploidy * variant.num_hom_ref + variant.num_het
+    @property
+    def params_mle(self) -> dict:
+        """
+        Get the maximum likelihood estimate of the parameters.
 
-                # swap reference and alternative allele if the AA info field
-                # is defined and indicates so
-                aa = variant.INFO.get(self.info_ancestral)
+        :return: Dict of parameters
+        """
+        return self.summary.data['params_mle']
 
-                if aa is None:
-                    logger.warning(f'No ancestral allele defined for {variant.CHROM}:{variant.POS}.')
-                else:
-                    # adjust orientation if different
-                    if aa != variant.REF:
-                        variant.REF = aa
+    @params_mle.setter
+    def params_mle(self, value):
+        """
+        Set the maximum likelihood estimate of the parameters.
 
-                        if len(variant.ALT) != 0:
-                            variant.ALT[0] = variant.REF
+        :param value: Dict of parameters
+        """
+        pass
 
-                        n_ref = n_samples - n_ref
+    @property
+    def model(self) -> Parametrization:
+        """
+        Get the DFE parametrization.
 
-                # determine down-projected allele count
-                k = self.rng.hypergeometric(ngood=n_samples - n_ref, nbad=n_ref, nsample=self.n)
+        :return: Parametrization
+        """
 
-                # try to obtain type
-                try:
-                    t = '.'.join([s.get_type(variant) for s in self.stratifications])
-                except NoTypeException:
-                    continue
+        return from_string(self.config.data['model'])
 
-                # add count by 1 if context is defined
-                if t in sfs:
-                    sfs[t][k] += 1
+    @model.setter
+    def model(self, value):
+        """
+        Set the DFE parametrization.
 
-        return Spectra(sfs)
+        :param value: Parametrization
+        """
+        pass
```

### Comparing `fastdfe-0.1.4b0/fastdfe/polydfe_utils.py` & `fastdfe-0.1.5b0/fastdfe/polydfe_utils.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.4b0/fastdfe/shared_inference.py` & `fastdfe-0.1.5b0/fastdfe/joint_inference.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Shared inference module.
+Joint inference module.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-02-26"
 
 import copy
@@ -20,24 +20,24 @@
 from scipy.optimize import OptimizeResult
 from numpy.linalg import norm
 
 from . import Config
 from .abstract_inference import Inference
 from .base_inference import BaseInference
 from .optimization import Optimization, SharedParams, pack_shared, expand_shared, \
-    Covariate, flatten_dict, merge_dicts, correct_values, parallelize as parallelize_func, expand_fixed, collapse_fixed, \
-    unpack_shared
+    Covariate, flatten_dict, merge_dicts, correct_values, parallelize as parallelize_func, expand_fixed, \
+    collapse_fixed, unpack_shared
 from .parametrization import Parametrization
 from .spectrum import Spectrum, Spectra
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
 
-class SharedInference(BaseInference):
+class JointInference(BaseInference):
     """
     Enabling the sharing of parameters among several Inference objects.
     """
 
     def __init__(
             self,
             sfs_neut: Spectra,
@@ -61,19 +61,21 @@
             do_bootstrap: bool = False,
             n_bootstraps: int = 100,
             parallelize: bool = True,
     ):
         """
         Create instance.
 
-        :param sfs_neut: Neutral SFS
-        :param sfs_sel: Selected SFS
+        :param sfs_neut: Neutral SFS. Note that we require monomorphic counts to be specified in order to infer
+            the mutation rate.
+        :param sfs_sel: Selected SFS. Note that we require monomorphic counts to be specified in order to infer
+            the mutation rate.
         :param include_divergence: Whether to include divergence in the likelihood
         :param intervals_del: ``(start, stop, n_interval)`` for deleterious population-scaled
-        selection coefficients. The intervals will be log10-spaced.
+            selection coefficients. The intervals will be log10-spaced.
         :param intervals_ben: Same as intervals_del but for beneficial selection coefficients
         :param integration_mode: Integration mode
         :param linearized: Whether to use the linearized model
         :param model: DFE parametrization
         :param seed: Random seed
         :param x0: Dictionary of initial values in the form ``{type: {param: value}}``
         :param bounds: Bounds for the optimization in the form {param: (lower, upper)}
@@ -503,15 +505,15 @@
             correct_values(self.add_covariates(params, t), self.bounds, self.scales),
             sfs_neut=self.joint_inferences[t].sfs_neut,
             sfs_sel=self.joint_inferences[t].sfs_sel
         ))) for t, inf in self.joint_inferences.items())
 
     @BaseInference.run_if_required_wrapper
     @functools.lru_cache
-    def run_joint_without_covariates(self, do_bootstrap: bool = True) -> 'SharedInference':
+    def run_joint_without_covariates(self, do_bootstrap: bool = True) -> 'JointInference':
         """
         Run joint inference without covariates. Note that the result of this function is cached.
 
         :return: Joint inference instance devoid of covariates.
         """
         config = self.create_config()
 
@@ -519,15 +521,15 @@
         config.update(
             shared_params=self.shared_params,
             covariates={},
             do_bootstrap=do_bootstrap
         )
 
         # create copy
-        other = SharedInference.from_config(config)
+        other = JointInference.from_config(config)
 
         # issue notice
         logger.info('Running joint inference without covariates.')
 
         # run inference
         other.run()
 
@@ -566,15 +568,15 @@
     def perform_lrt_covariates(self, do_bootstrap: bool = True) -> float:
         """
         Perform likelihood ratio test against joint inference without covariates.
         In the simple model we share parameters across types. Low p-values indicate that
         the covariates provide a significant improvement in the fit.
 
         :param do_bootstrap: Whether to bootstrap. This improves the accuracy of the p-value. Note
-        that if bootstrapping was performed previously without updating the likelihood, this won't have any effect.
+            that if bootstrapping was performed previously without updating the likelihood, this won't have any effect.
         :return: Likelihood ratio test statistic.
         """
         if len(self.covariates) == 0:
             raise ValueError('No covariates were specified.')
 
         # bootstrap if required
         if do_bootstrap:
@@ -769,23 +771,23 @@
 
         # add parameters for covariates and return
         return merge_dicts(packed, {':'.join(self.types): self.x0_cov})
 
     @BaseInference.run_if_required_wrapper
     def perform_lrt_shared(self, do_bootstrap: bool = True) -> float:
         """
-        Compare likelihood of shared inference with product of marginal likelihoods.
+        Compare likelihood of joint inference with product of marginal likelihoods.
         This provides information about the goodness of fit achieved by the parameter sharing.
         Low p-values indicate that parameter sharing is not justified, i.e., that the marginal
         inferences provide a better fit to the data. Note that it is more difficult to properly
         optimize the joint likelihood, which makes this test conservative, i.e., the p-value
         might be larger than it should be.
 
         :param do_bootstrap: Whether to perform bootstrapping. This improves the accuracy of the p-value. Note
-        that if bootstrapping was performed previously without updating the likelihood, this won't have any effect.
+            that if bootstrapping was performed previously without updating the likelihood, this won't have any effect.
         :return: p-value
         """
         if do_bootstrap:
             self.bootstrap_if_required()
 
         # determine likelihood of marginal inferences
         ll_marginal = sum([inf.likelihood for inf in self.marginals_without_all().values()])
@@ -993,49 +995,73 @@
         :param ax: Axes object
         :return: Axes object
         """
         labels, inferences = zip(*self.get_inferences(labels=labels).items())
 
         return Inference.plot_inferred_parameters(**locals())
 
-    def get_bootstrap_params(self) -> Dict[str, float]:
+    def get_cis_params_mle(
+            self,
+            bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
+            ci_level: float = 0.05,
+            param_names: Optional[list[str]] = None
+    ):
         """
-        Get bootstrap parameters.
+        Get confidence intervals for the parameters.
 
-        :return: Bootstrap parameters
+        :return: Confidence intervals for the parameters
         """
-        return flatten_dict(dict((t, self.joint_inferences[t].get_bootstrap_params()) for t in self.types))
+        # get dict of inferences
+        inferences = self.get_inferences()
 
-    @BaseInference.run_if_required_wrapper
-    def plot_covariates(
+        # get param names if not given
+        if param_names is None:
+            param_names = list(inferences.values())[0].get_bootstrap_param_names()
+
+        return Inference.get_cis_params_mle(
+            inferences=list(inferences.values()),
+            bootstrap_type=bootstrap_type,
+            ci_level=ci_level,
+            param_names=param_names,
+            labels=list(inferences.keys())
+        )
+
+    def get_discretized(
             self,
-            file: str = None,
-            show: bool = True,
-            axs: List[plt.Axes] = None
-    ) -> List[plt.Axes]:
+            intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
+            confidence_intervals: bool = True,
+            ci_level: float = 0.05,
+            bootstrap_type: Literal['percentile', 'bca'] = 'percentile'
+    ) -> Dict[str, Tuple[np.ndarray, np.ndarray]]:
         """
-        Plot inferred parameters of joint inference vs inferred
-        parameters of marginal inferences side by side.
+        Get discretized DFEs.
 
-        :param file: File to save plot to
-        :param show: Whether to show plot
-        :param axs: List of axes object, one for each covariate
-        :return: Axes object
+        :param bootstrap_type: Type of bootstrap
+        :param ci_level: Confidence interval level
+        :param confidence_intervals: Whether to return confidence intervals
+        :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bins.
+        :return: Dictionary of array of values and array of errors indexed by inference type
         """
-        from . import Visualization
-
-        return Visualization.plot_covariates(
-            covariates=self.covariates,
-            params_marginal=dict((t, inf.params_mle) for t, inf in self.marginal_inferences.items()),
-            params_joint=self.params_mle,
-            file=file,
-            show=show,
-            axs=axs
+        return Inference.get_discretized(
+            inferences=list(self.get_inferences().values()),
+            labels=list(self.get_inferences().keys()),
+            intervals=intervals,
+            confidence_intervals=confidence_intervals,
+            ci_level=ci_level,
+            bootstrap_type=bootstrap_type
         )
 
+    def get_bootstrap_params(self) -> Dict[str, float]:
+        """
+        Get bootstrap parameters.
+
+        :return: Bootstrap parameters
+        """
+        return flatten_dict(dict((t, self.joint_inferences[t].get_bootstrap_params()) for t in self.types))
+
     def to_json(self) -> str:
         """
         Serialize object. Note that the deserialized inference objects no
         longer share the same optimization instance among other things.
 
         :return: JSON string
         """
```

### Comparing `fastdfe-0.1.4b0/fastdfe/spectrum.py` & `fastdfe-0.1.5b0/fastdfe/spectrum.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.4b0/fastdfe/visualization.py` & `fastdfe-0.1.5b0/fastdfe/visualization.py`

 * *Files 7% similar despite different names*

```diff
@@ -337,20 +337,22 @@
         :param file: File path to save plot to
         :param show: Whether to show plot
         :param ax: Axes to plot on
         :return: Axes
         """
         # plot modelled vs observed non-neutral SFS
         ax = Visualization.plot_spectra(
+            ax=ax,
             spectra=spectra,
             labels=labels,
             use_subplots=use_subplots,
             show_monomorphic=show_monomorphic,
             title=title,
-            ax=ax
+            file=file,
+            show=show
         )
 
         return ax
 
     @staticmethod
     @clear_show_save
     def plot_inferred_parameters(
@@ -512,44 +514,40 @@
         prefix = labels[i].split('.')[0]
         prefix_index = list(prefixes).index(prefix)
 
         return hatch_styles[prefix_index % len(hatch_styles)]
 
     @staticmethod
     def plot_spectra(
-            spectra: List[Spectrum],
             ax: plt.Axes,
+            spectra: List[Spectrum],
             labels: List[str] = [],
             log_scale: bool = False,
             use_subplots: bool = False,
             show_monomorphic: bool = False,
             title: str = None,
             n_ticks=10,
             file: str = None,
             show: bool = True
     ) -> plt.Axes:
         """
         Plot the given 1D spectra.
 
         :param show_monomorphic: Whether to show monomorphic site counts
         :param n_ticks: Number of x-ticks to use
-        :param ax: Axes to plot on
+        :param ax: Axes to plot on, only if ``use_subplots`` is ``False``
         :param use_subplots: Whether to use subplots
         :param title: Title of plot
         :param spectra: List of spectra to plot
         :param labels: List of labels for each spectrum
         :param log_scale: Whether to use logarithmic y-scale
         :param file: File to save plot to
         :param show: Whether to show the plot
         :return: Axes
         """
-        if ax is None:
-            plt.clf()
-            _, ax = plt.subplots()
-
         if use_subplots:
             n_plots = len(spectra)
             n_rows = int(np.ceil(np.sqrt(n_plots)))
             n_cols = int(np.ceil(np.sqrt(n_plots)))
             fig = plt.figure(figsize=(6.4 * n_cols ** (1 / 3), 4.8 * n_rows ** (1 / 3)))
             axes = fig.subplots(ncols=n_cols, nrows=n_rows, squeeze=False).flatten()
 
@@ -557,25 +555,30 @@
             for i in range(n_plots):
                 Visualization.plot_spectra(
                     spectra=[spectra[i]],
                     labels=[labels[i]] if len(labels) else [],
                     ax=axes[i],
                     n_ticks=15 // min(2, n_cols),
                     log_scale=log_scale,
-                    show_monomorphic=show_monomorphic
+                    show_monomorphic=show_monomorphic,
+                    show=False
                 )
 
             # make empty plots invisible
             [ax.set_visible(False) for ax in axes[n_plots:]]
 
             # show and save plot
             Visualization.show_and_save(file, show)
 
             return plt.gca()
 
+        if ax is None:
+            plt.clf()
+            _, ax = plt.subplots()
+
         # determine sample size and width
         n = spectra[0].n
         width_total = 0.9
         width = width_total / len(spectra)
 
         x = np.arange(n + 1) if show_monomorphic else np.arange(1, n)
 
@@ -868,104 +871,14 @@
         ax.set_yticklabels([l.replace('_', ' ') for l in labels_y], rotation=0)
 
         # set title
         ax.set_title(title)
 
         return ax
 
-    @staticmethod
-    def plot_covariates(
-            covariates: Dict[str, 'Covariate'],
-            params_marginal: Dict[str, Dict[str, float]],
-            params_joint: Dict[str, Dict[str, float]],
-            axs: List[plt.Axes],
-            scale: Literal['lin', 'log', 'symlog'] = 'log',
-            file: str = None,
-            show: bool = True,
-            **kwargs
-    ) -> List[plt.Axes]:
-        """
-        Plot covariates.
-
-        :param covariates: Covariates to plot
-        :param params_marginal: Marginal parameters indexed by type
-        :param params_joint: Unpacked joint parameters indexed by type
-        :param axs: List of axes, one for each covariate
-        :param scale: Scale of y-axis
-        :param file: File to save plot to
-        :param show: Whether to show plot
-        :return: Axes
-        """
-        if len(covariates) == 0:
-            logger.info("There are no covariates to be plotted.")
-
-            return axs
-
-        types = list(params_joint.keys())
-
-        num_covariates = len(covariates)
-
-        n_cols = min(3, num_covariates)
-        n_rows = int(np.ceil(num_covariates / n_cols))
-
-        # create axes if not provided
-        if not isinstance(axs, np.ndarray | list):
-            plt.clf()
-            _, axs = plt.subplots(n_rows, n_cols, figsize=(6.4 * n_cols, 4.8 * n_rows), squeeze=False)
-
-        n_intervals = len(types)
-        width_total = 0.9
-        width = width_total / 2
-
-        for i, (p, cov) in enumerate(covariates.items()):
-            ax = axs[i // n_cols, i % n_cols]
-
-            x = np.arange(n_intervals)
-
-            y1 = np.abs([params_marginal[t][cov.param] for t in types])
-            y2 = np.abs([params_joint[t][cov.param] for t in types])
-
-            # plot bars for marginal inference
-            ax.bar(
-                x=x,
-                height=y1,
-                width=width,
-                label='marginal'
-            )
-
-            # plot bars for joint inference
-            ax.bar(
-                x=x + width,
-                height=y2,
-                width=width,
-                label='joint'
-            )
-
-            # proper representation of parameter
-            param_repr = f'${cov.param}$' if params_marginal[types[0]][cov.param] >= 0 else f'$-{cov.param}$'
-
-            # set title
-            ax.set_title(f"param={param_repr}, {p}={params_joint[types[0]][p]}")
-
-            # adjust ticks
-            ax.set_xticks(np.arange(len(types)) + width / 2)
-            ax.set_xticklabels(types)
-
-            # set legend
-            ax.legend()
-
-            # set y-scale
-            if scale == 'log':
-                ax.set_yscale('log')
-
-        # show and save plot
-        Visualization.show_and_save(file, show)
-
-        return axs
-
     @clear_show_save
     def plot_interval_density(
             self,
             ax: plt.Axes,
             density: np.ndarray,
             intervals: list | np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             interval_labels: List[str] = None,
```

### Comparing `fastdfe-0.1.4b0/pyproject.toml` & `fastdfe-0.1.5b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastdfe"
-version = "0.1.4-beta"
+version = "0.1.5-beta"
 description = "Fast, flexible, and hierarchical inference of the distribution of fitness effects"
 authors = ["Sendrowski <sendrowski.janek@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

