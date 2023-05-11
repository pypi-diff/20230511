# Comparing `tmp/summerepi2-1.2.2.tar.gz` & `tmp/summerepi2-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "summerepi2-1.2.2.tar", max compression
+gzip compressed data, was "summerepi2-1.2.3.tar", max compression
```

## Comparing `summerepi2-1.2.2.tar` & `summerepi2-1.2.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1512 2022-09-01 20:25:00.648111 summerepi2-1.2.2/LICENSE.txt
--rw-r--r--   0        0        0     1930 2023-04-12 23:08:21.398477 summerepi2-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     4101 2023-04-12 23:09:18.690955 summerepi2-1.2.2/README.md
--rw-r--r--   0        0        0      280 2022-09-01 05:32:07.966265 summerepi2-1.2.2/summer2/__init__.py
--rw-r--r--   0        0        0     4095 2022-09-01 05:32:07.967266 summerepi2-1.2.2/summer2/adjust.py
--rw-r--r--   0        0        0     4782 2022-09-01 05:32:07.967769 summerepi2-1.2.2/summer2/compartment.py
--rw-r--r--   0        0        0      137 2022-08-26 06:17:31.101047 summerepi2-1.2.2/summer2/compute_bak/__init__.py
--rw-r--r--   0        0        0     2151 2022-08-27 21:20:06.649159 summerepi2-1.2.2/summer2/compute_bak/compute_jax.py
--rw-r--r--   0        0        0    11683 2022-09-01 05:32:07.968765 summerepi2-1.2.2/summer2/derived_outputs.py
--rw-r--r--   0        0        0    10490 2023-04-05 00:33:04.716810 summerepi2-1.2.2/summer2/experimental/model_builder.py
--rw-r--r--   0        0        0      553 2023-04-05 00:33:04.726311 summerepi2-1.2.2/summer2/extras/test_models.py
--rw-r--r--   0        0        0    19144 2022-09-01 05:32:07.970266 summerepi2-1.2.2/summer2/flows.py
--rw-r--r--   0        0        0      203 2023-02-10 00:07:02.891606 summerepi2-1.2.2/summer2/functions/__init__.py
--rw-r--r--   0        0        0     4620 2023-01-17 01:08:37.545738 summerepi2-1.2.2/summer2/functions/interpolate.py
--rw-r--r--   0        0        0     3453 2023-02-09 22:50:26.022665 summerepi2-1.2.2/summer2/functions/time.py
--rw-r--r--   0        0        0     3670 2023-04-12 21:11:57.753156 summerepi2-1.2.2/summer2/functions/util.py
--rw-r--r--   0        0        0     6019 2022-10-11 00:26:22.994134 summerepi2-1.2.2/summer2/inspect.py
--rw-r--r--   0        0        0    51975 2023-04-05 00:33:04.735811 summerepi2-1.2.2/summer2/model.py
--rw-r--r--   0        0        0       22 2022-10-11 01:49:59.803947 summerepi2-1.2.2/summer2/parameters/__init__.py
--rw-r--r--   0        0        0    10693 2022-10-11 00:26:23.922637 summerepi2-1.2.2/summer2/parameters/param_impl.py
--rw-r--r--   0        0        0     4255 2023-04-05 00:33:04.747809 summerepi2-1.2.2/summer2/parameters/params.py
--rw-r--r--   0        0        0     4804 2022-09-01 05:32:07.974766 summerepi2-1.2.2/summer2/population.py
--rw-r--r--   0        0        0       40 2022-09-01 05:32:07.975265 summerepi2-1.2.2/summer2/runner/__init__.py
--rw-r--r--   0        0        0        0 2022-09-01 05:32:07.975767 summerepi2-1.2.2/summer2/runner/jax/__init__.py
--rw-r--r--   0        0        0     5107 2022-11-30 22:02:39.158382 summerepi2-1.2.2/summer2/runner/jax/derived_outputs.py
--rw-r--r--   0        0        0    24105 2023-04-11 21:29:43.015787 summerepi2-1.2.2/summer2/runner/jax/model_impl.py
--rw-r--r--   0        0        0    11588 2023-04-05 00:33:04.765810 summerepi2-1.2.2/summer2/runner/jax/ode.py
--rw-r--r--   0        0        0    11222 2022-10-12 17:29:54.983503 summerepi2-1.2.2/summer2/runner/jax/ode2.py
--rw-r--r--   0        0        0     2736 2022-11-30 22:02:39.159369 summerepi2-1.2.2/summer2/runner/jax/solvers.py
--rw-r--r--   0        0        0     5111 2022-09-01 05:32:08.044494 summerepi2-1.2.2/summer2/runner/jax/stratify.py
--rw-r--r--   0        0        0     8170 2022-12-02 02:13:10.114800 summerepi2-1.2.2/summer2/runner/model_runner.py
--rw-r--r--   0        0        0     6277 2022-10-11 01:50:00.034457 summerepi2-1.2.2/summer2/solver.py
--rw-r--r--   0        0        0    17065 2022-09-01 05:47:20.176421 summerepi2-1.2.2/summer2/stratification.py
--rw-r--r--   0        0        0      472 2022-09-01 05:32:08.049501 summerepi2-1.2.2/summer2/tracker.py
--rw-r--r--   0        0        0     1799 2022-09-01 05:32:08.050495 summerepi2-1.2.2/summer2/utils.py
--rw-r--r--   0        0        0     5622 1970-01-01 00:00:00.000000 summerepi2-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1512 2022-09-01 20:25:00.648111 summerepi2-1.2.3/LICENSE.txt
+-rw-r--r--   0        0        0     1930 2023-05-11 01:54:34.520878 summerepi2-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4101 2023-04-12 23:09:18.690955 summerepi2-1.2.3/README.md
+-rw-r--r--   0        0        0      280 2022-09-01 05:32:07.966265 summerepi2-1.2.3/summer2/__init__.py
+-rw-r--r--   0        0        0     4095 2022-09-01 05:32:07.967266 summerepi2-1.2.3/summer2/adjust.py
+-rw-r--r--   0        0        0     4782 2022-09-01 05:32:07.967769 summerepi2-1.2.3/summer2/compartment.py
+-rw-r--r--   0        0        0      137 2022-08-26 06:17:31.101047 summerepi2-1.2.3/summer2/compute_bak/__init__.py
+-rw-r--r--   0        0        0     2151 2022-08-27 21:20:06.649159 summerepi2-1.2.3/summer2/compute_bak/compute_jax.py
+-rw-r--r--   0        0        0    11683 2022-09-01 05:32:07.968765 summerepi2-1.2.3/summer2/derived_outputs.py
+-rw-r--r--   0        0        0    10490 2023-04-05 00:33:04.716810 summerepi2-1.2.3/summer2/experimental/model_builder.py
+-rw-r--r--   0        0        0     2603 2023-04-19 22:25:13.644705 summerepi2-1.2.3/summer2/extras/test_models.py
+-rw-r--r--   0        0        0    19144 2022-09-01 05:32:07.970266 summerepi2-1.2.3/summer2/flows.py
+-rw-r--r--   0        0        0      203 2023-02-10 00:07:02.891606 summerepi2-1.2.3/summer2/functions/__init__.py
+-rw-r--r--   0        0        0     4620 2023-01-17 01:08:37.545738 summerepi2-1.2.3/summer2/functions/interpolate.py
+-rw-r--r--   0        0        0     3453 2023-02-09 22:50:26.022665 summerepi2-1.2.3/summer2/functions/time.py
+-rw-r--r--   0        0        0     3670 2023-04-12 21:11:57.753156 summerepi2-1.2.3/summer2/functions/util.py
+-rw-r--r--   0        0        0     6019 2022-10-11 00:26:22.994134 summerepi2-1.2.3/summer2/inspect.py
+-rw-r--r--   0        0        0    53798 2023-05-11 03:19:13.430929 summerepi2-1.2.3/summer2/model.py
+-rw-r--r--   0        0        0       22 2022-10-11 01:49:59.803947 summerepi2-1.2.3/summer2/parameters/__init__.py
+-rw-r--r--   0        0        0    10987 2023-04-18 23:12:23.096368 summerepi2-1.2.3/summer2/parameters/param_impl.py
+-rw-r--r--   0        0        0     4255 2023-04-05 00:33:04.747809 summerepi2-1.2.3/summer2/parameters/params.py
+-rw-r--r--   0        0        0     4804 2022-09-01 05:32:07.974766 summerepi2-1.2.3/summer2/population.py
+-rw-r--r--   0        0        0       40 2022-09-01 05:32:07.975265 summerepi2-1.2.3/summer2/runner/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-01 05:32:07.975767 summerepi2-1.2.3/summer2/runner/jax/__init__.py
+-rw-r--r--   0        0        0     5240 2023-05-02 00:15:48.813286 summerepi2-1.2.3/summer2/runner/jax/derived_outputs.py
+-rw-r--r--   0        0        0    25476 2023-05-11 03:24:09.889928 summerepi2-1.2.3/summer2/runner/jax/model_impl.py
+-rw-r--r--   0        0        0    11588 2023-04-05 00:33:04.765810 summerepi2-1.2.3/summer2/runner/jax/ode.py
+-rw-r--r--   0        0        0    11222 2022-10-12 17:29:54.983503 summerepi2-1.2.3/summer2/runner/jax/ode2.py
+-rw-r--r--   0        0        0     2736 2022-11-30 22:02:39.159369 summerepi2-1.2.3/summer2/runner/jax/solvers.py
+-rw-r--r--   0        0        0     5111 2022-09-01 05:32:08.044494 summerepi2-1.2.3/summer2/runner/jax/stratify.py
+-rw-r--r--   0        0        0     8170 2022-12-02 02:13:10.114800 summerepi2-1.2.3/summer2/runner/model_runner.py
+-rw-r--r--   0        0        0     6277 2022-10-11 01:50:00.034457 summerepi2-1.2.3/summer2/solver.py
+-rw-r--r--   0        0        0    17065 2023-04-18 23:09:58.702374 summerepi2-1.2.3/summer2/stratification.py
+-rw-r--r--   0        0        0      472 2022-09-01 05:32:08.049501 summerepi2-1.2.3/summer2/tracker.py
+-rw-r--r--   0        0        0     3760 2023-05-11 02:02:50.793367 summerepi2-1.2.3/summer2/utils.py
+-rw-r--r--   0        0        0     5622 1970-01-01 00:00:00.000000 summerepi2-1.2.3/PKG-INFO
```

### Comparing `summerepi2-1.2.2/LICENSE.txt` & `summerepi2-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/pyproject.toml` & `summerepi2-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "summerepi2"
-version = "1.2.2"
+version = "1.2.3"
 readme = "README.md"
 license = "BSD-2-Clause"
 homepage = "http://summerepi.com/"
 documentation = "http://summerepi.com/"
 repository = "https://github.com/monash-emu/summer2"
 keywords = [
     "epidemiology",
```

### Comparing `summerepi2-1.2.2/README.md` & `summerepi2-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/adjust.py` & `summerepi2-1.2.3/summer2/adjust.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/compartment.py` & `summerepi2-1.2.3/summer2/compartment.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/compute_bak/compute_jax.py` & `summerepi2-1.2.3/summer2/compute_bak/compute_jax.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/derived_outputs.py` & `summerepi2-1.2.3/summer2/derived_outputs.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/experimental/model_builder.py` & `summerepi2-1.2.3/summer2/experimental/model_builder.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/flows.py` & `summerepi2-1.2.3/summer2/flows.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/functions/interpolate.py` & `summerepi2-1.2.3/summer2/functions/interpolate.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/functions/time.py` & `summerepi2-1.2.3/summer2/functions/time.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/functions/util.py` & `summerepi2-1.2.3/summer2/functions/util.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/inspect.py` & `summerepi2-1.2.3/summer2/inspect.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/model.py` & `summerepi2-1.2.3/summer2/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,25 +25,24 @@
 from summer2.parameters import params, DerivedOutput
 
 from summer2.parameters.param_impl import finalize_parameters
 from summer2.runner import ModelBackend
 from summer2.runner.jax.model_impl import StepResults
 from summer2.solver import SolverType, solve_ode
 from summer2.stratification import Stratification
-from summer2.utils import get_scenario_start_index, ref_times_to_dti, clean_compartment_values
+from summer2.utils import get_scenario_start_index, ref_times_to_dti, Epoch
 from summer2.population import get_unique_strat_groups, filter_by_strata
 from summer2.tracker import ModelBuildTracker, ActionType
 
 logger = logging.getLogger()
 
 FlowRateFunction = Callable[[List[Compartment], np.ndarray, np.ndarray, float], np.ndarray]
 OutputSource = Union[str, DerivedOutput]
 
 
-
 class BackendType:
     PYTHON = "python"
     JAX = "jax"
 
 
 class CompartmentalModel:
     """
@@ -85,28 +84,38 @@
         self,
         times: Tuple[int, int],
         compartments: List[str],
         infectious_compartments: List[str],
         timestep: float = 1.0,
         ref_date: datetime = None,
     ):
+        # Set the ref_date; the datetime object equivalent to times[0]
+        self.ref_date = ref_date
+
+        # If a ref_date was supplied, we can use datetime objects for the time range here,
+        # we just need to convert them first
+
+        if all([isinstance(t, datetime) for t in times]):
+            if epoch := self.get_epoch():
+                start_t, end_t = times
+                times = (epoch.datetime_to_number(start_t), epoch.datetime_to_number(end_t))
+            else:
+                raise TypeError("Times supplied as datetime but no ref_date set")
+
         start_t, end_t = times
         assert end_t > start_t, "End time must be greater than start time"
         time_period = end_t - start_t
         num_steps = 1 + (time_period / timestep)
         msg = f"Time step {timestep} must be less than time period {time_period}"
         assert num_steps >= 1, msg
         msg = f"Time step {timestep} must be a factor of time period {time_period}"
         assert num_steps % 1 == 0, msg
         self.times = np.linspace(start_t, end_t, num=int(num_steps))
         self.timestep = timestep
 
-        # Set the ref_date; the datetime object equivalent to times[0]
-        self.ref_date = ref_date
-
         if isinstance(infectious_compartments, str):
             infectious_compartments = [infectious_compartments]
         error_msg = "Infectious compartments must be a subset of compartments"
         assert all(n in compartments for n in infectious_compartments), error_msg
         self.compartments = [Compartment(n, idx=i) for i, n in enumerate(compartments)]
         for c in self.compartments:
             if c in infectious_compartments:
@@ -797,15 +806,14 @@
             msg = "Mixing matrices only allowed for full stratification."
             assert strat.compartments == self._original_compartment_names, msg
 
             for age_idx in range(len(ages) - 1):
                 start_age = int(ages[age_idx])
                 end_age = int(ages[age_idx + 1])
                 for comp in prev_compartment_names:
-
                     source = comp.stratify(strat.name, str(start_age))
                     dest = comp.stratify(strat.name, str(end_age))
                     ageing_rate = 1.0 / (end_age - start_age)
                     self.add_transition_flow(
                         name=f"ageing_{source}_to_{dest}",
                         fractional_rate=ageing_rate,
                         source=source.name,
@@ -1190,15 +1198,17 @@
             "request_type": DerivedOutputRequest.CUMULATIVE,
             "source": source,
             "start_time": start_time,
             "save_results": save_results,
         }
         return DerivedOutput(name, request)
 
-    def request_function_output(self, name: str, func: params.Function, save_results: bool = True) -> DerivedOutput:
+    def request_function_output(
+        self, name: str, func: params.Function, save_results: bool = True
+    ) -> DerivedOutput:
         """
         Request a generic Function output
 
         Args:
             name: The name of the derived output
             func: The Function, whose args are GraphObjects
             save_results: Whether these results should be available in the final output
@@ -1240,15 +1250,15 @@
         self._derived_output_graph.add_node(name)
         self._derived_output_requests[name] = request = {
             "request_type": DerivedOutputRequest.COMPUTED_VALUE,
             "name": name,
             "save_results": save_results,
         }
         return DerivedOutput(name, request)
-    
+
     def request_track_modelled_value(self, name: str, f: GraphObject) -> DerivedOutput:
         """
         Save the output of a computegraph Function as a derived output
 
         Args:
             name: Name (key) of derived output
             f: The GraphObject to save
@@ -1274,30 +1284,36 @@
     def _get_ref_idx(self):
         if self.ref_date:
             times = ref_times_to_dti(self.ref_date, self.times)
         else:
             times = self.times
         return times
 
+    def get_epoch(self):
+        if self.ref_date:
+            return Epoch(self.ref_date)
+        else:
+            return None
+
     def get_outputs_df(self):
         idx = self._get_ref_idx()
         column_str = [str(c) for c in self.compartments]
         return pd.DataFrame(self.outputs, index=idx, columns=column_str)
 
     def get_derived_outputs_df(self):
         idx = self._get_ref_idx()
         return pd.DataFrame(self.derived_outputs, index=idx)
 
     def get_input_parameters(self) -> set:
         self.finalize()
         all_in_var = set(self.graph.get_input_variables())
         all_in_var = all_in_var.union(set(self._do_tracker_graph.get_input_variables()))
         return set([v.key for v in all_in_var if v.source == "parameters"])
-    
-    def set_default_parameters(self, parameters:dict):
+
+    def set_default_parameters(self, parameters: dict):
         self._runner = None
         self._default_parameters = parameters
 
     def get_default_parameters(self) -> dict:
         return self._default_parameters
 
     def query_compartments(self, query: dict = None, tags: List = None, as_idx=False):
@@ -1314,29 +1330,46 @@
     ):
         from summer2.inspect import query_flows
 
         return query_flows(self, flow_name, source, dest, tags)
 
 
 class ModelResults:
-    def __init__(self, model, run_func, runner_dict=None):
+    def __init__(self, model: CompartmentalModel, run_func, runner_dict=None):
         self.model = model
         self._run_func = run_func
+        self.function = run_func
         self._input_params = model.get_input_parameters()
         self._derived_outputs_idx_cache = None
         self._runner_dict = runner_dict
+        self.impl_dict = runner_dict
         self.default_parameters = model.get_default_parameters() or {}
+        self.ref_idx = model._get_ref_idx()
 
     def get_outputs_df(self):
         return self.model.get_outputs_df()
 
     def get_derived_outputs_df(self):
         return self.model.get_derived_outputs_df()
 
     def run(self, parameters: dict, filter=True, expand=True, ret_raw=True):
+        """Run the model for a set of input parameters
+           This is mostly a wrapper for the AuTuMN toolkit, and is not threadsafe!
+           New clients should call run_model instead
+
+        Args:
+            parameters: Input parameters for this run
+            filter: Filter the input parameters dictionary so that only
+                    valid input params are passed to the model
+            expand: Expand a nested dictionary into flat parameters
+            ret_raw: Return the outputs of the (jax) _run_func directly
+
+        Returns:
+            (optional) returned jax structure from _run_func
+        """
         if expand:
             parameters = expand_nested_dict(parameters)
         if filter:
             parameters = {k: v for k, v in parameters.items() if k in self._input_params}
             if self.model.builder:
                 parameters = {k: self.model._type_validators[k](v) for k, v in parameters.items()}
 
@@ -1349,20 +1382,38 @@
         self.outputs = np.array(results["outputs"])
         self.derived_outputs = {k: np.array(v) for k, v in results["derived_outputs"].items()}
         self.model.outputs = self.outputs
         self.model.derived_outputs = self.derived_outputs
         if ret_raw:
             return results
 
+    def run_model(self, parameters):
+        """_summary_
+
+        Args:
+            parameters (_type_): _description_
+            out_format (str, optional): _description_. Defaults to "pandas".
+
+        Returns:
+            _type_: _description_
+        """
+        results = self._run_func(parameters=parameters)
+
+        derived_outputs = {k: np.array(v) for k, v in results["derived_outputs"].items()}
+        return pd.DataFrame(derived_outputs, index=self.ref_idx)
+
+
 # Additional validation functions
 
+
 def _validate_flowparam(param):
     if not (isinstance(param, GraphObject) or isinstance(param, Real)):
         raise TypeError(f"Flow parameter must be GraphObject or float, not {type(param)}")
 
+
 def _resolve_source(src: OutputSource) -> str:
     if isinstance(src, DerivedOutput):
         return src.key
-    elif isinstance (src, str):
+    elif isinstance(src, str):
         return src
     else:
-        raise TypeError("Invalid derived output source type", src, type(src))
+        raise TypeError("Invalid derived output source type", src, type(src))
```

### Comparing `summerepi2-1.2.2/summer2/parameters/param_impl.py` & `summerepi2-1.2.3/summer2/parameters/param_impl.py`

 * *Files 5% similar despite different names*

```diff
@@ -135,28 +135,33 @@
 
 
 def get_reparameterized_dict(d):
     return {k: get_modelparameter_from_param(v) for k, v in d.items()}
 
 
 def map_flow_keys(m: CompartmentalModel) -> dict:
-
     from summer2.adjust import Overwrite
 
     realised_flows = {}
 
     for i, f in enumerate(m.flows):
         full_flow = [f.param.obj]
         for a in f.adjustments:
             if isinstance(a, Overwrite):
                 full_flow = [a.param.obj]
             else:
                 full_flow.append(a.param.obj)
         out_func = full_flow[0]
         for fparam in full_flow[1:]:
+            # In the case of simply mulitplying by a scalar,
+            # we unbox the value from the GraphObject,
+            # to avoid cluttering up the graph
+            if isinstance(fparam, Data):
+                if isinstance(fparam.data, Real):
+                    fparam = fparam.data
             out_func = out_func * fparam
         realised_flows[i] = GraphObjectParameter(out_func)
 
     return realised_flows
 
 
 def register_object_key(obj_table, obj, base_name, unique=False):
```

### Comparing `summerepi2-1.2.2/summer2/parameters/params.py` & `summerepi2-1.2.3/summer2/parameters/params.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/population.py` & `summerepi2-1.2.3/summer2/population.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/runner/jax/derived_outputs.py` & `summerepi2-1.2.3/summer2/runner/jax/derived_outputs.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,28 +7,27 @@
     - evaluation times
     - compartment sizes for each time
     - flow rates for each time
 
 """
 import logging
 
-from jax import numpy as jnp
+from jax import numpy as jnp, jit
 import numpy as np
 
 from computegraph import ComputeGraph
 from computegraph.utils import relabel_tree
 from computegraph.types import local
 
 from summer2.parameters import Function, ModelVariable
 
 logger = logging.getLogger()
 
 
 def build_flow_output(request, name, times, model_flows, idx_cache=None):
-
     flow_indices = []
     for flow_idx, flow in enumerate(model_flows):
         is_matching_flow = (
             flow.name == request["flow_name"]
             and ((not flow.source) or flow.source.has_strata(request["source_strata"]))
             and ((not flow.dest) or flow.dest.has_strata(request["dest_strata"]))
         )
@@ -54,15 +53,14 @@
             midpoint_output = midpoint_output.at[1:].set(interp_vals)
             return midpoint_output
 
     return Function(get_flow_output, [ModelVariable("flows")])
 
 
 def build_compartment_output(request, name, compartments):
-
     req_compartments = request["compartments"]
     strata = request["strata"]
     comps = ((i, c) for i, c in enumerate(compartments) if c.has_name_in_list(req_compartments))
     indices = [i for i, c in comps if c.is_match(c.name, strata)]
 
     def summed_compartment_outputs(outputs):
         return outputs[:, indices].sum(axis=1)
@@ -112,15 +110,15 @@
     return Function(func, inputs)
 
 
 def build_computed_value_output(request, name):
     return Function(lambda x: x[name], [ModelVariable("computed_values")])
 
 
-def build_derived_outputs_runner(model):
+def build_derived_outputs_runner(model, whitelist=None, jit_compile=False):
     graph_dict = {}
     out_keys = []
     for name, request in model._derived_output_requests.items():
         req_type = request["request_type"]
         if req_type == "comp":
             graph_dict[name] = build_compartment_output(request, name, model.compartments)
         elif req_type == "param_func":
@@ -138,12 +136,18 @@
         else:
             raise NotImplementedError(request)
         if request["save_results"]:
             out_keys.append(name)
 
     cg = ComputeGraph(graph_dict)
 
-    if model._derived_outputs_whitelist:
-        out_keys = model._derived_outputs_whitelist
+    whitelist = whitelist or model._derived_outputs_whitelist
+
+    if whitelist:
+        out_keys = whitelist
         cg = cg.filter(targets=out_keys)
 
-    return cg, cg.get_callable(targets=out_keys)
+    out_func = cg.get_callable(targets=out_keys)
+    if jit_compile:
+        out_func = jit(out_func)
+
+    return cg, out_func
```

### Comparing `summerepi2-1.2.2/summer2/runner/jax/model_impl.py` & `summerepi2-1.2.3/summer2/runner/jax/model_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Implementation of CompartmentalModel and ModelBackend internals in Jax
 
 This is a mess right now!
 """
 
-from functools import partial
 from dataclasses import dataclass
 
 import numpy as np
 
-from jax import lax, jit, numpy as jnp
+from jax import lax, numpy as jnp
 
 from summer2.runner.jax import ode
 
 # from jax.experimental import ode
 from summer2.runner.jax import solvers
 
 from summer2.adjust import Overwrite
@@ -72,27 +71,25 @@
         raise NotImplementedError("No support for mixed infection frequency/density")
 
     # FIXME: This could desparately use a tidy-up - all the indexing is a nightmare
 
     def get_infectious_multipliers(
         time, compartment_values, cur_graph_outputs, compartment_infectiousness
     ):
-
         infection_frequency = {}
         infection_density = {}
 
         full_multipliers = jnp.ones(len(runner.infectious_flow_indices))
 
         mixing_matrix = cur_graph_outputs["mixing_matrix"]
         category_populations = compartment_values[population_cat_indexer].sum(axis=1)
 
         per_strain_out = {}
 
         for strain_idx, strain in enumerate(runner.model._disease_strains):
-
             strain_compartment_infectiousness = compartment_infectiousness[strain]
             strain_infectious_idx = runner._strain_infectious_indexers[strain]
             strain_category_indexer = runner._strain_category_indexers[strain]
 
             strain_infectious_values = compartment_values[strain_infectious_idx]
             strain_values = get_force_of_infection(
                 strain_infectious_values,
@@ -144,27 +141,25 @@
         else:
             return full_multipliers
 
     return get_infectious_multipliers
 
 
 def build_get_flow_weights(runner: ModelBackend):
-
     m = runner.model
 
     if "model_variables.time" in m.graph.dag:
         tvkeys = list(m.graph.filter(sources="model_variables.time").dag)
         tv_flow_map = {
             k: m._flow_key_map[k] for k in set(m._flow_key_map).intersection(set(tvkeys))
         }
     else:
         tv_flow_map = {}
 
     def get_flow_weights(cur_graph_outputs, static_flow_weights):
-
         flow_weights = jnp.copy(static_flow_weights)
 
         for k, v in tv_flow_map.items():
             val = cur_graph_outputs[k]
             flow_weights = flow_weights.at[v].set(val)
 
         return flow_weights
@@ -182,27 +177,25 @@
 
         return computed_values
 
     return calc_computed_values
 
 
 def build_get_flow_rates(runner, ts_graph_func, get_infectious_multipliers=None, debug=False):
-
     # calc_computed_values = build_calc_computed_values(runner)
     get_flow_weights = build_get_flow_weights(runner)
 
     infect_proc_type = runner._infection_process_type
     # if infect_proc_type:
     #    get_infectious_multipliers = build_get_infectious_multipliers(runner)
 
     population_idx = np.array(runner.population_idx)
     infectious_flow_indices = jnp.array(runner.infectious_flow_indices)
 
     def get_flow_rates(compartment_values: jnp.array, time, static_graph_vals, model_data):
-
         compartment_values = clean_compartments(compartment_values)
 
         sources = {
             "model_variables": {"time": time, "compartment_values": compartment_values},
             "static_inputs": static_graph_vals,
         }
 
@@ -255,26 +248,25 @@
 
 def build_get_compartment_rates(runner):
     accum_maps = get_accumulation_maps(runner)
 
     def get_compartment_rates(compartment_values, flow_rates):
         comp_rates = jnp.zeros_like(compartment_values)
 
-        for (flow_src, comp_target) in accum_maps["positive"]:
+        for flow_src, comp_target in accum_maps["positive"]:
             comp_rates = comp_rates.at[comp_target].add(flow_rates[flow_src])
-        for (flow_src, comp_target) in accum_maps["negative"]:
+        for flow_src, comp_target in accum_maps["negative"]:
             comp_rates = comp_rates.at[comp_target].add(-flow_rates[flow_src])
 
         return comp_rates
 
     return get_compartment_rates
 
 
 def build_get_rates(runner, ts_graph_func):
-
     get_infectious_multipliers = build_get_infectious_multipliers(runner)
     get_flow_rates = build_get_flow_rates(runner, ts_graph_func, get_infectious_multipliers)
     get_flow_rates_debug = build_get_flow_rates(
         runner, ts_graph_func, get_infectious_multipliers, True
     )
     get_compartment_rates = build_get_compartment_rates(runner)
 
@@ -304,15 +296,15 @@
     pos_map = [mflow for mflow in runner._pos_flow_map]
     neg_map = [mflow for mflow in runner._neg_flow_map]
 
     def peel_flow_map(flow_map):
         targets = []
         src_idx = []
         remainder = []
-        for (src_flow, target) in flow_map:
+        for src_flow, target in flow_map:
             if target not in targets:
                 targets.append(target)
                 src_idx.append(src_flow)
             else:
                 remainder.append((src_flow, target))
         return np.array(src_idx), np.array(targets), remainder
 
@@ -333,15 +325,14 @@
     of the strain specified by strain
     """
 
     # This is run during prepare_dynamic
     # i.e. it is done once at the start of a model run, but
     # is parameterized (non-structural)
     def get_compartment_infectiousness(static_graph_values):
-
         # Find the infectiousness multipliers for each compartment being implemented in the model.
         compartment_infectiousness = jnp.ones(len(model.compartments))
 
         # Apply infectiousness adjustments
         for strat in model._stratifications:
             for comp_name, adjustments in strat.infectiousness_adjustments.items():
                 for stratum, adjustment in adjustments.items():
@@ -378,29 +369,33 @@
             strain_comp_inf[strain] = compartment_infectiousness[strain_infect_comps]
 
         return strain_comp_inf
 
     return get_compartment_infectiousness
 
 
+# Returned by the one_step runner function - the complete internal state
+# of the model at a given timestep
+# Does not include derived outputs - these are a post-process
 @dataclass
 class StepResults:
     flow_rates: jnp.array
     comp_rates: jnp.array
     comp_vals: jnp.array
     static_graph_vals: dict
     ts_graph_vals: dict
     initial_population: jnp.array
     model_data: dict
     infectious_multipliers: jnp.array
     infect_mul_per_strain: dict
 
 
-def build_run_model(runner, base_params=None, dyn_params=None, solver=None, solver_args=None):
-
+def build_run_model(
+    runner, base_params=None, dyn_params=None, solver=None, solver_args=None, derived_outputs=None
+):
     if dyn_params is None:
         dyn_params = runner.model.get_input_parameters()
 
     dyn_params = [f"parameters.{p}" if not p.startswith("parameters.") else p for p in dyn_params]
 
     # dyn_params may contain parameters only used in derived outputs, that do not show up
     # in the main graph.  These need to be filtered out; they will be computed every time,
@@ -480,15 +475,17 @@
         raise NotImplementedError("Incompatible SolverType for Jax runner", solver)
 
     times = jnp.array(runner.model.times)
 
     calc_initial_pop = get_calculate_initial_pop(runner.model)
     get_compartment_infectiousness = build_get_compartment_infectiousness(runner.model)
 
-    do_cg, calc_derived_outputs = build_derived_outputs_runner(runner.model)
+    do_cg, calc_derived_outputs = build_derived_outputs_runner(
+        runner.model, whitelist=derived_outputs
+    )
 
     m = runner.model
     if "model_variables.time" in m.graph.dag:
         tv_keys = list(m.graph.filter(sources="model_variables.time").dag)
     else:
         tv_keys = []
 
@@ -499,32 +496,15 @@
     # In the case of parameters used by derived outputs that are _not_ supplised in dyn_params,
     # we need to capture these from the original base_params
     do_params = set(
         [v.key for v in m._do_tracker_graph.get_input_variables() if v.source == "parameters"]
     )
     do_base_params = {k: v for k, v in base_params.items() if k in do_params}
 
-    def run_model(parameters):
-
-        static_graph_vals = static_graph_func(parameters=parameters)
-        initial_population = calc_initial_pop(static_graph_vals)
-
-        static_flow_weights = jnp.zeros(len(runner.model.flows))
-        for k, v in static_flow_map.items():
-            val = static_graph_vals[k]
-            static_flow_weights = static_flow_weights.at[v].set(val)
-
-        compartment_infectiousness = get_compartment_infectiousness(static_graph_vals)
-        model_data = {
-            "compartment_infectiousness": compartment_infectiousness,
-            "static_flow_weights": static_flow_weights,
-        }
-
-        outputs = get_ode_solution(initial_population, times, static_graph_vals, model_data)
-
+    def get_flows_for_outputs(outputs, static_graph_vals, model_data):
         # Empty array to kick-start flow rates from outputs
         flow_rates_full = jnp.empty((len(m.times), len(m.flows)))
 
         # And likewise for computed values (but as a dict)
         cv_out = {}
         for k in m._computed_values_graph_dict:
             cv_out[k] = jnp.empty((len(m.times),))
@@ -538,15 +518,55 @@
                 cur_cv[k] = cur_cv[k].at[i].set(v)
             return (frate_full, cur_cv), None
 
         (out_flows, out_cv), _ = lax.scan(
             f, (flow_rates_full, cv_out), jnp.array(range(len(m.times)))
         )
 
-        # out_flows, out_cv = get_flows_for_outputs(outputs, times, static_graph_vals, model_data)
+        return out_flows, out_cv
+
+    def run_model(parameters):
+        static_graph_vals = static_graph_func(parameters=parameters)
+        initial_population = calc_initial_pop(static_graph_vals)
+
+        static_flow_weights = jnp.zeros(len(runner.model.flows))
+        for k, v in static_flow_map.items():
+            val = static_graph_vals[k]
+            static_flow_weights = static_flow_weights.at[v].set(val)
+
+        compartment_infectiousness = get_compartment_infectiousness(static_graph_vals)
+        model_data = {
+            "compartment_infectiousness": compartment_infectiousness,
+            "static_flow_weights": static_flow_weights,
+        }
+
+        outputs = get_ode_solution(initial_population, times, static_graph_vals, model_data)
+
+        # # Empty array to kick-start flow rates from outputs
+        # flow_rates_full = jnp.empty((len(m.times), len(m.flows)))
+
+        # # And likewise for computed values (but as a dict)
+        # cv_out = {}
+        # for k in m._computed_values_graph_dict:
+        #     cv_out[k] = jnp.empty((len(m.times),))
+
+        # def f(carry, i):
+        #     frate_full, cur_cv = carry
+        #     t = model_times[i]
+        #     frates, cvals = get_flow_rates(outputs[i], t, static_graph_vals, model_data)
+        #     frate_full = frate_full.at[i].set(frates)
+        #     for k, v in cvals.items():
+        #         cur_cv[k] = cur_cv[k].at[i].set(v)
+        #     return (frate_full, cur_cv), None
+
+        # (out_flows, out_cv), _ = lax.scan(
+        #     f, (flow_rates_full, cv_out), jnp.array(range(len(m.times)))
+        # )
+
+        out_flows, out_cv = get_flows_for_outputs(outputs, static_graph_vals, model_data)
 
         model_variables = {"outputs": outputs, "flows": out_flows, "computed_values": out_cv}
 
         do_full_params = do_base_params.copy()
         do_full_params.update(parameters)
 
         derived_outputs = calc_derived_outputs(
@@ -558,15 +578,14 @@
             "outputs": outputs,
             "derived_outputs": derived_outputs,
         }  # "model_data": model_data}
 
     ons_get_inf_mul = build_get_infectious_multipliers(runner, True)
 
     def one_step(parameters: dict = None, t: float = None, comp_vals=None):
-
         static_graph_vals = static_graph_func(parameters=parameters)
 
         if t is None:
             t = runner.model.times[0]
 
         if comp_vals is None:
             comp_vals = calc_initial_pop(static_graph_vals)
@@ -614,18 +633,18 @@
     runner_dict = {
         "get_rates": get_rates,
         "get_flow_rates": get_flow_rates,
         "get_comp_rates": get_comp_rates,
         "calc_initial_pop": calc_initial_pop,
         "get_compartment_infectiousness": get_compartment_infectiousness,
         "get_ode_solution": get_ode_solution,
-        "calc_derived_outputs": calc_derived_outputs,
-        "timestep_graph_func": timestep_graph_func,
-        "timestep_cg": timestep_cg,
-        "static_cg": static_cg,
-        "static_graph_func": static_graph_func,
-        "one_step": one_step,
-        "derived_outputs_cg": do_cg,
+        "calc_derived_outputs": calc_derived_outputs,  # Callable for derived outputs
+        "timestep_cg": timestep_cg,  # Computegraph for time-varying processes
+        "timestep_graph_func": timestep_graph_func,  # Callable for timestep graph
+        "static_cg": static_cg,  # Computegraph for static portion of model
+        "static_graph_func": static_graph_func,  # Callable for static graph
+        "one_step": one_step,  # Single (euler) step run function
+        "derived_outputs_cg": do_cg,  # DerivedOutputs computegraph
         "get_rates_debug": rates_funcs["get_rates_debug"],
     }
 
     return run_model, runner_dict
```

### Comparing `summerepi2-1.2.2/summer2/runner/jax/ode.py` & `summerepi2-1.2.3/summer2/runner/jax/ode.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/runner/jax/ode2.py` & `summerepi2-1.2.3/summer2/runner/jax/ode2.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/runner/jax/solvers.py` & `summerepi2-1.2.3/summer2/runner/jax/solvers.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/runner/jax/stratify.py` & `summerepi2-1.2.3/summer2/runner/jax/stratify.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/runner/model_runner.py` & `summerepi2-1.2.3/summer2/runner/model_runner.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/solver.py` & `summerepi2-1.2.3/summer2/solver.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/summer2/stratification.py` & `summerepi2-1.2.3/summer2/stratification.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.2/PKG-INFO` & `summerepi2-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: summerepi2
-Version: 1.2.2
+Version: 1.2.3
 Summary: Summer is a compartmental disease modelling framework, written in Python. It provides a high-level API to build and run models.
 Home-page: http://summerepi.com/
 License: BSD-2-Clause
 Keywords: epidemiology,disease,compartmental,infectious
 Author: James Trauer
 Author-email: james.trauer@monash.edu
 Requires-Python: >=3.8.0
```

