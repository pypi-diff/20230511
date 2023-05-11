# Comparing `tmp/neutone_sdk-1.1.3.tar.gz` & `tmp/neutone_sdk-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neutone_sdk-1.1.3.tar", max compression
+gzip compressed data, was "neutone_sdk-1.2.1.tar", max compression
```

## Comparing `neutone_sdk-1.1.3.tar` & `neutone_sdk-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0    26526 2022-04-26 09:40:10.074536 neutone_sdk-1.1.3/LICENSE
--rw-r--r--   0        0        0    12036 2023-03-24 09:03:52.527364 neutone_sdk-1.1.3/README.md
--rw-r--r--   0        0        0      118 2022-08-18 10:39:26.672878 neutone_sdk-1.1.3/neutone_sdk/__init__.py
--rw-r--r--   0        0        0   165792 2023-03-24 09:03:52.530608 neutone_sdk-1.1.3/neutone_sdk/assets/default_samples/sample_inst.mp3
--rw-r--r--   0        0        0   172033 2023-03-24 09:03:52.532422 neutone_sdk-1.1.3/neutone_sdk/assets/default_samples/sample_music.mp3
--rw-r--r--   0        0        0     7411 2023-03-25 04:28:17.982027 neutone_sdk-1.1.3/neutone_sdk/audio.py
--rw-r--r--   0        0        0      136 2023-03-24 09:03:52.533264 neutone_sdk-1.1.3/neutone_sdk/constants.py
--rw-r--r--   0        0        0     9784 2023-03-24 09:03:52.533666 neutone_sdk-1.1.3/neutone_sdk/core.py
--rw-r--r--   0        0        0     6511 2023-03-24 09:03:52.534042 neutone_sdk-1.1.3/neutone_sdk/metadata.py
--rw-r--r--   0        0        0     1073 2022-04-26 09:40:10.077426 neutone_sdk-1.1.3/neutone_sdk/parameter.py
--rw-r--r--   0        0        0        0 2022-04-26 09:40:10.077499 neutone_sdk-1.1.3/neutone_sdk/py.typed
--rw-r--r--   0        0        0     6743 2023-03-24 09:03:52.534417 neutone_sdk-1.1.3/neutone_sdk/queues.py
--rw-r--r--   0        0        0    13795 2023-03-24 09:03:52.534846 neutone_sdk-1.1.3/neutone_sdk/realtime_stft.py
--rw-r--r--   0        0        0     9869 2023-03-24 09:03:52.535241 neutone_sdk-1.1.3/neutone_sdk/sandwich.py
--rw-r--r--   0        0        0    16888 2023-03-24 09:03:52.535674 neutone_sdk-1.1.3/neutone_sdk/sqw.py
--rw-r--r--   0        0        0     5699 2023-03-24 09:03:52.536070 neutone_sdk-1.1.3/neutone_sdk/tcn_1d.py
--rw-r--r--   0        0        0    10778 2023-03-24 09:03:52.536473 neutone_sdk-1.1.3/neutone_sdk/utils.py
--rw-r--r--   0        0        0    15425 2023-03-02 08:01:35.147563 neutone_sdk-1.1.3/neutone_sdk/wavform_to_wavform.py
--rw-r--r--   0        0        0      669 2023-03-24 09:03:52.536820 neutone_sdk-1.1.3/pyproject.toml
--rw-r--r--   0        0        0    13149 1970-01-01 00:00:00.000000 neutone_sdk-1.1.3/setup.py
--rw-r--r--   0        0        0    12933 1970-01-01 00:00:00.000000 neutone_sdk-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0    26526 2022-04-26 09:40:10.074536 neutone_sdk-1.2.1/LICENSE
+-rw-r--r--   0        0        0    12204 2023-04-06 05:59:27.128733 neutone_sdk-1.2.1/README.md
+-rw-r--r--   0        0        0      118 2022-08-18 10:39:26.672878 neutone_sdk-1.2.1/neutone_sdk/__init__.py
+-rw-r--r--   0        0        0   165792 2023-03-24 09:03:52.530608 neutone_sdk-1.2.1/neutone_sdk/assets/default_samples/sample_inst.mp3
+-rw-r--r--   0        0        0   172033 2023-03-24 09:03:52.532422 neutone_sdk-1.2.1/neutone_sdk/assets/default_samples/sample_music.mp3
+-rw-r--r--   0        0        0     7408 2023-04-21 09:31:02.484224 neutone_sdk-1.2.1/neutone_sdk/audio.py
+-rw-r--r--   0        0        0      136 2023-05-11 06:35:50.563707 neutone_sdk-1.2.1/neutone_sdk/constants.py
+-rw-r--r--   0        0        0    10506 2023-04-21 09:31:02.485111 neutone_sdk-1.2.1/neutone_sdk/core.py
+-rw-r--r--   0        0        0    10878 2023-04-21 09:44:08.632457 neutone_sdk-1.2.1/neutone_sdk/filters.py
+-rw-r--r--   0        0        0     6533 2023-05-11 06:35:50.565356 neutone_sdk-1.2.1/neutone_sdk/metadata.py
+-rw-r--r--   0        0        0     1073 2022-04-26 09:40:10.077426 neutone_sdk-1.2.1/neutone_sdk/parameter.py
+-rw-r--r--   0        0        0        0 2022-04-26 09:40:10.077499 neutone_sdk-1.2.1/neutone_sdk/py.typed
+-rw-r--r--   0        0        0     6743 2023-03-24 09:03:52.534417 neutone_sdk-1.2.1/neutone_sdk/queues.py
+-rw-r--r--   0        0        0    13795 2023-03-24 09:03:52.534846 neutone_sdk-1.2.1/neutone_sdk/realtime_stft.py
+-rw-r--r--   0        0        0     9869 2023-03-24 09:03:52.535241 neutone_sdk-1.2.1/neutone_sdk/sandwich.py
+-rw-r--r--   0        0        0    18551 2023-04-21 09:31:02.486879 neutone_sdk-1.2.1/neutone_sdk/sqw.py
+-rw-r--r--   0        0        0     5699 2023-03-24 09:03:52.536070 neutone_sdk-1.2.1/neutone_sdk/tcn_1d.py
+-rw-r--r--   0        0        0    10985 2023-05-11 06:35:50.566967 neutone_sdk-1.2.1/neutone_sdk/utils.py
+-rw-r--r--   0        0        0    15660 2023-04-21 09:31:02.487661 neutone_sdk-1.2.1/neutone_sdk/wavform_to_wavform.py
+-rw-r--r--   0        0        0      669 2023-05-11 06:35:50.567359 neutone_sdk-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    13318 1970-01-01 00:00:00.000000 neutone_sdk-1.2.1/setup.py
+-rw-r--r--   0        0        0    13101 1970-01-01 00:00:00.000000 neutone_sdk-1.2.1/PKG-INFO
```

### Comparing `neutone_sdk-1.1.3/LICENSE` & `neutone_sdk-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neutone_sdk-1.1.3/README.md` & `neutone_sdk-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 <a name="examples"/>
 
 ## Examples and Notebooks
 
 - Full clipper distortion model example can be found [here](examples/example_clipper.py).
 - Example of a random overdrive model based on [micro-tcn](https://github.com/csteinmetz1/micro-tcn) can be found [here](examples/example_overdrive-random.py)
 - Notebooks for different models showing the entire workflow from training to exporting it using Neutone
-    - [DDSP](https://colab.research.google.com/drive/15FuafmtGWEyvTOOQbN1AMIQRhGLy23Pg)
-    - [RAVE](https://colab.research.google.com/drive/1hty5Bd7rJJ70hlI-5720sEY3kylNxBIt)
+    - [DDSP Timbre Transfer](https://colab.research.google.com/drive/1yPHU6PRWw1lRWZLUxXimIa6chFQ2JdRW?usp=sharing)
+    - [RAVE Timbre Transfer](https://colab.research.google.com/drive/1qlN6xLvDYrLcAwS8yh2ecmNG_bEKlVI9?usp=sharing)
+    - [TCN FX Emulation](https://colab.research.google.com/drive/1gHZ-AEoYmfmWrjlKpKkK_SW1xzfxD24-?usp=sharing)
 
 ## v1 Release
 
 The Neutone SDK is currently on version 1.0.0. Models exported with this version of the SDK will be incompatible with beta versions of the plugin to please make sure you are using the right version. 
 
 
 The restriction for a sampling rate of 48kHz and a buffer size of 2048 is now gone and the SDK contains a wrapper that supports on the fly resampling and queueing to accomodate the requirements of both the models and the DAW thanks to great work by [@christhetree](https://github.com/christhetree).
```

### Comparing `neutone_sdk-1.1.3/neutone_sdk/assets/default_samples/sample_inst.mp3` & `neutone_sdk-1.2.1/neutone_sdk/assets/default_samples/sample_inst.mp3`

 * *Files identical despite different names*

### Comparing `neutone_sdk-1.1.3/neutone_sdk/assets/default_samples/sample_music.mp3` & `neutone_sdk-1.2.1/neutone_sdk/assets/default_samples/sample_music.mp3`

 * *Files identical despite different names*

### Comparing `neutone_sdk-1.1.3/neutone_sdk/audio.py` & `neutone_sdk-1.2.1/neutone_sdk/audio.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 
         # otherwise resample to match audio
         else:
             assert params.shape == (model.MAX_N_PARAMS, input_sample.audio.size(1))
             params = torchaudio.transforms.Resample(input_sample.sr, preferred_sr)(
                 params
             )
-            params = torch.clamp(params, 0, 1)
+            params = tr.clamp(params, 0, 1)
 
         # padding and chunking parameters to match audio
         padded_params = nn.functional.pad(params, [0, padding_amount], mode="replicate")
         param_chunks = padded_params.split(buffer_size, dim=1)
 
         out_chunks = [
             model.forward(audio_chunk, param_chunk).clone()
```

### Comparing `neutone_sdk-1.1.3/neutone_sdk/core.py` & `neutone_sdk-1.2.1/neutone_sdk/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -223,14 +223,30 @@
         self.eval()
 
     @tr.jit.export
     def get_default_param_values(self) -> Tensor:
         return self.default_param_values
 
     @tr.jit.export
+    def get_default_param_names(self) -> List[str]:
+        return [x.name for x in self.get_neutone_parameters()]
+
+    @tr.jit.export
+    def get_default_param_descriptions(self) -> List[str]:
+        return [x.description for x in self.get_neutone_parameters()]
+
+    @tr.jit.export
+    def get_default_param_types(self) -> List[str]:
+        return [x.type.value for x in self.get_neutone_parameters()]
+
+    @tr.jit.export
+    def get_default_param_used(self) -> List[bool]:
+        return [x.used for x in self.get_neutone_parameters()]
+
+    @tr.jit.export
     def get_wet_default_value(self) -> float:
         return 1.0
 
     @tr.jit.export
     def get_dry_default_value(self) -> float:
         return 0.0
 
@@ -246,14 +262,18 @@
 
     @tr.jit.export
     def get_core_preserved_attributes(self) -> List[str]:
         return [
             "model",  # nn.Module
             "default_param_values",  # Registered buffer
             "get_default_param_values",
+            "get_default_param_names",
+            "get_default_param_descriptions",
+            "get_default_param_types",
+            "get_default_param_used",
             "get_wet_default_value",
             "get_dry_default_value",
             "get_input_gain_default_value",
             "get_output_gain_default_value",
             "get_core_preserved_attributes",
             "to_core_metadata",
         ]
```

### Comparing `neutone_sdk-1.1.3/neutone_sdk/metadata.py` & `neutone_sdk-1.2.1/neutone_sdk/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     except ValidationError as err:
         log.error(err)
         raise err
 
     # Check links return 200
     for link in metadata["technical_links"].values():
         try:
-            code = requests.head(link).status_code
+            code = requests.head(link, allow_redirects=True).status_code
             if code != 200:
                 log.error(f"Cannot access link {link}")
         except requests.exceptions.ConnectionError:
             log.error(f"Cannot access link {link}")
 
     # Check we can extract mp3s from the samples
     for audio_sample_pair in metadata["sample_sound_files"]:
```

### Comparing `neutone_sdk-1.1.3/neutone_sdk/parameter.py` & `neutone_sdk-1.2.1/neutone_sdk/parameter.py`

 * *Files identical despite different names*

### Comparing `neutone_sdk-1.1.3/neutone_sdk/queues.py` & `neutone_sdk-1.2.1/neutone_sdk/queues.py`

 * *Files identical despite different names*

### Comparing `neutone_sdk-1.1.3/neutone_sdk/realtime_stft.py` & `neutone_sdk-1.2.1/neutone_sdk/realtime_stft.py`

 * *Files identical despite different names*

### Comparing `neutone_sdk-1.1.3/neutone_sdk/sandwich.py` & `neutone_sdk-1.2.1/neutone_sdk/sandwich.py`

 * *Files identical despite different names*

### Comparing `neutone_sdk-1.1.3/neutone_sdk/sqw.py` & `neutone_sdk-1.2.1/neutone_sdk/sqw.py`

 * *Files 10% similar despite different names*

```diff
@@ -363,15 +363,15 @@
                     or model_bs in self.get_native_buffer_sizes()
                 )
         else:
             model_bs = self.select_best_model_buffer_size(
                 io_bs, self.get_native_buffer_sizes()
             )
 
-        self.w2w_base.set_buffer_size(model_bs)
+        self.w2w_base.set_sample_rate_and_buffer_size(model_sr, model_bs)
         self.daw_bs = daw_bs
         self.io_bs = io_bs
         self.model_bs = model_bs
 
         self.in_queue = CircularInplaceTensorQueue(
             self.in_n_ch,
             (2 * self.io_bs) + self.model_bs,
@@ -419,21 +419,72 @@
 
     @tr.jit.export
     def get_preserved_attributes(self) -> List[str]:
         return [
             "forward_bt",
             "is_input_mono",
             "is_output_mono",
+            "get_model_name",
+            "get_model_authors",
             "get_native_sample_rates",
             "get_native_buffer_sizes",
+            "get_wet_default_value",
+            "get_dry_default_value",
+            "get_default_param_values",
+            "get_input_gain_default_value",
+            "get_output_gain_default_value",
             "is_resampling",
             "calc_min_delay_samples",
             "set_daw_sample_rate_and_buffer_size",
             "reset",
             "get_preserved_attributes",
             "to_metadata",
             "w2w_base",
         ]
 
     @tr.jit.export
     def to_metadata(self) -> WaveformToWaveformMetadata:
         return self.w2w_base.to_metadata()
+
+    @tr.jit.export
+    def get_model_name(self) -> str:
+        return self.w2w_base.get_model_name()
+
+    @tr.jit.export
+    def get_model_authors(self) -> List[str]:
+        return self.w2w_base.get_model_authors()
+
+    @tr.jit.export
+    def get_wet_default_value(self) -> float:
+        return self.w2w_base.get_wet_default_value()
+
+    @tr.jit.export
+    def get_dry_default_value(self) -> float:
+        return self.w2w_base.get_dry_default_value()
+
+    @tr.jit.export
+    def get_default_param_values(self) -> Tensor:
+        return self.w2w_base.get_default_param_values()
+
+    @tr.jit.export
+    def get_default_param_names(self) -> List[str]:
+        return self.w2w_base.get_default_param_names()
+
+    @tr.jit.export
+    def get_default_param_descriptions(self) -> List[str]:
+        return self.w2w_base.get_default_param_descriptions()
+
+    @tr.jit.export
+    def get_default_param_types(self) -> List[str]:
+        return self.w2w_base.get_default_param_types()
+
+    @tr.jit.export
+    def get_default_param_used(self) -> List[bool]:
+        return self.w2w_base.get_default_param_used()
+
+    @tr.jit.export
+    def get_input_gain_default_value(self) -> float:
+        return self.w2w_base.get_input_gain_default_value()
+
+    @tr.jit.export
+    def get_output_gain_default_value(self) -> float:
+        return self.w2w_base.get_output_gain_default_value()
```

### Comparing `neutone_sdk-1.1.3/neutone_sdk/tcn_1d.py` & `neutone_sdk-1.2.1/neutone_sdk/tcn_1d.py`

 * *Files identical despite different names*

### Comparing `neutone_sdk-1.1.3/neutone_sdk/utils.py` & `neutone_sdk-1.2.1/neutone_sdk/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+import io
 import json
 import logging
 import os
 import random
 from pathlib import Path
 from typing import Tuple, Dict, List
 from neutone_sdk.audio import (
@@ -109,15 +110,21 @@
 
     with tr.no_grad():
         log.info("Converting model to torchscript...")
         script = model_to_torchscript(sqw, freeze=freeze, optimize=optimize)
 
         # We need to keep a copy because some models still don't implement reset
         # properly and when rendering the samples we might create unwanted state.
-        script_copy = copy.deepcopy(script)
+        # 
+        # We used to deepcopy but we found it breaks some models
+        # script_copy = copy.deepcopy(script)
+        buf = io.BytesIO()
+        tr.jit.save(script, buf)
+        buf.seek(0)
+        script_copy = tr.jit.load(buf)
 
         log.info("Extracting metadata...")
         metadata = script.to_metadata()._asdict()
         with open(root_dir / "metadata.json", "w") as f:
             json.dump(metadata, f, indent=4)
 
         log.info("Running model on audio samples...")
```

### Comparing `neutone_sdk-1.1.3/neutone_sdk/wavform_to_wavform.py` & `neutone_sdk-1.2.1/neutone_sdk/wavform_to_wavform.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         # These initializations are all temporary for TorchScript typing, otherwise they would be None
         # These variables are only used if get_look_behind_samples() is greater than 0
         self.curr_bs = -1
         self.in_queue = CircularInplaceTensorQueue(self.in_n_ch, 1)
         self.params_queue = CircularInplaceTensorQueue(self.MAX_N_PARAMS, 1)
         self.model_in_buffer = tr.zeros((self.in_n_ch, 1))
         self.params_buffer = tr.zeros((self.MAX_N_PARAMS, 1))
+        self.agg_params = tr.zeros((self.MAX_N_PARAMS, 1))
 
     @abstractmethod
     def is_input_mono(self) -> bool:
         pass
 
     @abstractmethod
     def is_output_mono(self) -> bool:
@@ -127,20 +128,23 @@
 
         Returns:
             int: The number of look-behind samples expected by the model.
                  Defaults to 0 (no look-behind buffer)
         """
         return 0
 
-    def set_model_buffer_size(self, n_samples: int) -> bool:
+    def set_model_sample_rate_and_buffer_size(
+        self, sample_rate: int, n_samples: int
+    ) -> bool:
         """
-        If the model supports dynamic buffer size resizing, add the
+        If the model supports dynamic sample rate or buffer size resizing, add the
         functionality here.
 
         Args:
+            sample_rate: The sample rate to use.
             n_samples: The number of samples to resize the buffer to.
 
         Returns:
             bool: True if successful, False if not supported or unsuccessful.
                   Defaults to False.
         """
         return False
@@ -163,18 +167,16 @@
         By default we take the mean value along dimension 1 to provide a single value for each parameter
         for the current buffer.
 
         For more fine grained control, override this method as required.
         """
         if self.use_debug_mode:
             assert params.ndim == 2
-        # This prevents memory allocation by re-using the space in the params tensor
-        agg_params = params[:, 0:1]
-        tr.mean(params, dim=1, keepdim=True, out=agg_params)
-        return agg_params
+        tr.mean(params, dim=1, keepdim=True, out=self.agg_params)
+        return self.agg_params
 
     def prepare_for_inference(self) -> None:
         """Prepare the wrapper and model for inference and to be converted to torchscript."""
         super().prepare_for_inference()
         self.in_queue.use_debug_mode = False
         self.params_queue.use_debug_mode = False
 
@@ -208,15 +210,15 @@
 
             if self.get_look_behind_samples():
                 # If a look behind buffer is being used, the queues and self.curr_bs must be initialized.
                 # This will only potentially trigger in the forward function when just the wrapper is being tested in
                 # python (because the SQW already sets the buffer size in its constructor when using the VST or SQW)
                 assert self.curr_bs != -1, (
                     "Model uses a look-behind buffer, but the incoming buffer size has not "
-                    "been set. Be sure to call `set_buffer_size` before using the model."
+                    "been set. Be sure to call `set_sample_rate_and_buffer_size` before using the model."
                 )
 
         if self.get_look_behind_samples():
             self.in_queue.push(x)
             self.params_queue.push(params)
             n = self.in_queue.size
             self.model_in_buffer[:, 0:-n] = 0
@@ -262,24 +264,26 @@
 
         This value may change if set_buffer_size() is used to change the buffer
         size, hence this is not a constant attribute.
         """
         return 0
 
     @tr.jit.export
-    def set_buffer_size(self, n_samples: int) -> bool:
+    def set_sample_rate_and_buffer_size(self, sample_rate: int, n_samples: int) -> bool:
         """
-        Sets the buffer size of the wrapper.
-        This should not be overwritten by SDK users, instead please check out the 'set_model_buffer_size' method.
+        Sets the sample_rate and buffer size of the wrapper.
+        This should not be overwritten by SDK users, instead please check out
+        the 'set_model_sample_rate_and_buffer_size' method.
 
         Args:
+            sample_rate: The sample rate to use.
             n_samples: The number of samples to use.
 
         Returns:
-            bool: True if 'set_model_buffer_size' is implemented and successful, otherwise False.
+            bool: True if 'set_model_sample_rate_and_buffer_size' is implemented and successful, otherwise False.
         """
         if self.use_debug_mode:
             if self.get_native_buffer_sizes():
                 assert (
                     n_samples in self.get_native_buffer_sizes()
                 ), f"The model does not support a native buffer size of {n_samples}"
 
@@ -294,30 +298,29 @@
                     self.MAX_N_PARAMS, queue_len, use_debug_mode=self.use_debug_mode
                 )
                 self.model_in_buffer = tr.zeros((self.in_n_ch, queue_len))
                 self.params_buffer = self.get_default_param_values().repeat(
                     1, queue_len
                 )
 
-        return self.set_model_buffer_size(n_samples)
+        return self.set_model_sample_rate_and_buffer_size(sample_rate, n_samples)
 
     @tr.jit.export
     def set_daw_sample_rate_and_buffer_size(
         self,
         daw_sr: int,
         daw_buffer_size: int,
         model_sr: Optional[int] = None,
         model_buffer_size: Optional[int] = None,
     ) -> None:
         """
         This method should only be used when testing the wrapper in the VST without the SampleQueueWrapper.
         It can be ignored by SDK users.
         """
-        # w2w only supports changing buffer size
-        self.set_buffer_size(daw_buffer_size)
+        self.set_sample_rate_and_buffer_size(daw_sr, daw_buffer_size)
 
     @tr.jit.export
     def reset(self) -> bool:
         """
         Resets the wrapper.
         This should not be overwritten by SDK users, instead please check out the 'reset_model' method.
 
@@ -338,15 +341,15 @@
             [
                 "is_input_mono",
                 "is_output_mono",
                 "get_native_sample_rates",
                 "get_native_buffer_sizes",
                 "is_resampling",
                 "calc_min_delay_samples",
-                "set_buffer_size",
+                "set_sample_rate_and_buffer_size",
                 "set_daw_sample_rate_and_buffer_size",
                 "reset",
                 "get_preserved_attributes",
                 "to_metadata",
             ]
         )
         return preserved_attrs
```

### Comparing `neutone_sdk-1.1.3/pyproject.toml` & `neutone_sdk-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neutone_sdk"
-version = "1.1.3"
+version = "1.2.1"
 description = "SDK for wrapping deep learning models for usage in the Neutone plugin"
 readme = "README.md"
 authors = ["Qosmo <contact@qosmo.jp>"]
 homepage = "https://github.com/QosmoInc/neutone_sdk.git"
 license = "LGPL"
 packages = [{include = "neutone_sdk"}]
```

### Comparing `neutone_sdk-1.1.3/setup.py` & `neutone_sdk-1.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'soundfile>=0.12.1',
  'torch>=1.11.0,<2.0.0',
  'torchaudio>=0.11.0,<2.0.0',
  'tqdm>=4.63.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'neutone-sdk',
-    'version': '1.1.3',
+    'version': '1.2.1',
     'description': 'SDK for wrapping deep learning models for usage in the Neutone plugin',
-    'long_description': '# Neutone SDK\n\nWe open source this SDK so researchers can wrap their own audio models and run them in a DAW using our [Neutone Plugin](https://neutone.space/). We offer both functionality for loading the models locally in the plugin as well as contributing them to the default list of models that is available to anyone running the plugin. We hope this will both give an opportunity for researchers to easily try their models in a DAW, but also provide creators with a collection of interesting models.\n\n<a name="examples"/>\n\n## Examples and Notebooks\n\n- Full clipper distortion model example can be found [here](examples/example_clipper.py).\n- Example of a random overdrive model based on [micro-tcn](https://github.com/csteinmetz1/micro-tcn) can be found [here](examples/example_overdrive-random.py)\n- Notebooks for different models showing the entire workflow from training to exporting it using Neutone\n    - [DDSP](https://colab.research.google.com/drive/15FuafmtGWEyvTOOQbN1AMIQRhGLy23Pg)\n    - [RAVE](https://colab.research.google.com/drive/1hty5Bd7rJJ70hlI-5720sEY3kylNxBIt)\n\n## v1 Release\n\nThe Neutone SDK is currently on version 1.0.0. Models exported with this version of the SDK will be incompatible with beta versions of the plugin to please make sure you are using the right version. \n\n\nThe restriction for a sampling rate of 48kHz and a buffer size of 2048 is now gone and the SDK contains a wrapper that supports on the fly resampling and queueing to accomodate the requirements of both the models and the DAW thanks to great work by [@christhetree](https://github.com/christhetree).\n\n\nThe following are known shortcomings:\n- Freezing models on save can cause instabilities, we recommend trying to save models both with and without freeze.\n- Displaying metadata information does not currently work with local model loading in the plugin.\n- Lookahead and on the fly STFT transforms will be implemented at the SDK level in the near future but is currently possible with additional code.\n- Windows and M1 acceleration are currently not supported.\n\nLogs are currently dumped to `/Users/<username>/Library/Application Support/Qosmo/Neutone/neutone.log`\n\n## Table of Contents\n- [Downloading the Neutone Plugin](#download)\n- [Installing the SDK](#install)\n- [SDK Description](#description)\n- [SDK Usage](#usage)\n- [Examples](#examples)\n- [Contributing to the SDK](#contributing)\n- [Credits](#credits)\n\n--- \n\n\n<a name="download"/>\n\n## Downloading the Plugin\n\nThe Neutone Plugin is available at [https://neutone.space](https://neutone.space). We currently offer VST3 and AU plugins that can be used to load the models created with this SDK. Please visit the website for more information.\n\n\n## Installing the SDK\n\n<a name="install"/>\n\nYou can install `neutone_sdk` using pip: \n\n```\npip install neutone_sdk\n```\n\n<a name="description"/>\n\n## SDK Description\n\nThe SDK provides functionality for wrapping existing PyTorch models in a way that can make them executable within the VST plugin. At its core the plugin is sending chunks of audio samples at a certain sample rate as an input and expects the same amount of samples at the output. Thus the simplest models also follow this input-output format and an example can be seen in [example_clipper.py](https://github.com/QosmoInc/neutone_sdk/blob/main/examples/example_clipper.py).\n\n<a name="usage"/>\n\n## SDK Usage\n\n### General Usage\n\nWe provide several models in the [examples](https://github.com/QosmoInc/neutone-sdk/blob/main/examples) directory. We will go through one of the simplest models, a distortion model, to illustrate.\n\nAssume we have the following PyTorch model. Parameters will be covered later on, we will focus on the inputs and outputs for now. Assume this model receives a Tensor of shape `(2, buffer_size)` as an input where `buffer_size` is a parameter that can be specified.\n\n```python\nclass ClipperModel(nn.Module):\n    def forward(self, x: Tensor, min_val: float, max_val: float, gain: float) -> Tensor:\n        return torch.clip(x, min=min_val * gain, max=max_val * gain)\n```\n\nTo run this inside the VST the simplest wrapper we can write is by subclassing the WaveformToWaveformBase baseclass.\n```python\nclass ClipperModelWrapper(WaveformToWaveformBase):\n    @torch.jit.export  \n    def is_input_mono(self) -> bool:\n        return False\n    \n    @torch.jit.export\n    def is_output_mono(self) -> bool:\n        return False\n    \n    @torch.jit.export\n    def get_native_sample_rates(self) -> List[int]:\n        return []  # Supports all sample rates\n    \n    @torch.jit.export\n    def get_native_buffer_sizes(self) -> List[int]:\n        return []  # Supports all buffer sizes\n\n    def do_forward_pass(self, x: Tensor, params: Dict[str, Tensor]) -> Tensor:\n        # ... Parameter unwrap logic\n        x = self.model.forward(x, min_val, max_val, gain)\n        return x\n ```\n\nThe method that does most of the work is `do_forward_pass`. In this case it is just a simple passthrough, but we will use it to handle parameters later on.\n\nBy default the VST runs as `stereo-stereo` but when mono is desired for the model we can use the `is_input_mono` and `is_output_mono` to inform the SDK and have the inputs and outputs converted automatically. If `is_input_mono` is toggled an averaged `(1, buffer_size)` shaped Tensor will be passed as an input instead of `(2, buffer_size)`. If `is_output_mono` is toggled, `do_forward_pass` is expected to return a mono Tensor (shape `(1, buffer_size)`) that will then be duplicated across both channels at the output of the VST. This is done within the SDK to avoid unnecessary memory allocations on each pass.\n\n`get_native_sample_rates` and `get_native_buffer_sizes` can be used to specify any preferred sample rates or buffer sizes. In most cases these are expected to only have one element but extra flexibility is provided for more complex models. In case multiple options are provided the SDK will try to find the best one for the current setting of the DAW. Whenever the sample rate or buffer size is different from the one of the DAW a wrapper is automatically triggered that converts to the correct sampling rate or implements a FIFO queue for the requested buffer size or both. This will incur a small performance penalty and add some amount of delay. In case a model is compatible with any sample rate and/or buffer_size these lists can be left empty.\n\nThis means that the tensor `x` in the `do_forward_pass` method is guaranteed to be of shape `(1 if is_input_mono else 2, buffer_size)`  where `buffer_size` will be chosen at runtime from the list provided in the `get_native_buffer_sizes` method.\n\n### Exporting models and loading in the plugin\n\nWe provide a `save_neutone_model` helper function that saves models to disk. By default this will convert models to TorchScript and run them through a series of checks to ensure they can be loaded by the plugin. The resulting `model.nm` file can be loaded within the plugin using the `load your own` button. Read below for how to submit models to the default collection.\n\n### Parameters\n\nFor models that can use conditioning signals we currently provide four configurable knob parameters. Within the `ClipperModelWrapper` defined above we can include the following:\n```python\nclass ClipperModelWrapper(WaveformToWaveformBase):\n    ...\n    \n    def get_neutone_parameters(self) -> List[NeutoneParameter]:\n        return [NeutoneParameter(name="min", description="min clip threshold", default_value=0.5),\n                NeutoneParameter(name="max", description="max clip threshold", default_value=1.0),\n                NeutoneParameter(name="gain", description="scale clip threshold", default_value=1.0)]\n         \n    def do_forward_pass(self, x: Tensor, params: Dict[str, Tensor]) -> Tensor:\n        min_val, max_val, gain = params["min"], params["max"], params["gain"]\n        x = self.model.forward(x, min_val, max_val, gain)\n        return x\n```\n\nDuring the forward pass the `params` variable will be a dictionary like the following:\n```python\n{\n    "min": torch.Tensor([0.5] * buffer_size),\n    "max": torch.Tensor([1.0] * buffer_size),\n    "gain": torch.Tensor([1.0] * buffer_size)\n}\n```\nThe keys of the dictionary are specified in the `get_parameters` function.\n\nThe parameters will always take values between 0 and 1 and the `do_forward_pass` function can be used to do any necessary rescaling before running the internal forward method of the model.\n\nMoreover, the parameters sent by the plugin come in at a sample level granularity. By default, we take the mean of each buffer and return a single float (as a Tensor), but the `aggregate_param` method can be used to override the aggregation method. See the full clipper export file for an example of preserving this granularity.\n\n\n### Submitting models\n\nThe plugin contains a default list of models aimed at creators that want to make use of them during their creative process. We encourage users to submit their models once they are happy with the results they get so they can be used by the community at large. For submission we require some additional metadata that will be used to display information about the model aimed at both creators and other researchers. This will be displayed on both the [Neutone website](https://neutone.space) and inside the plugin.\n\nSkipping the previous clipper model, here is a more realistic example based on a random TCN overdrive model inspired by [micro-tcn](https://github.com/csteinmetz1/micro-tcn).\n\n```python\nclass OverdriveModelWrapper(WaveformToWaveformBase):\n    def get_model_name(self) -> str:\n        return "conv1d-overdrive.random"\n\n    def get_model_authors(self) -> List[str]:\n        return ["Nao Tokui"]\n\n    def get_model_short_description(self) -> str:\n        return "Neural distortion/overdrive effect"\n\n    def get_model_long_description(self) -> str:\n        return "Neural distortion/overdrive effect through randomly initialized Convolutional Neural Network"\n\n    def get_technical_description(self) -> str:\n        return "Random distortion/overdrive effect through randomly initialized Temporal-1D-convolution layers. You\'ll get different types of distortion by re-initializing the weight or changing the activation function. Based on the idea proposed by Steinmetz et al."\n\n    def get_tags(self) -> List[str]:\n        return ["distortion", "overdrive"]\n\n    def get_model_version(self) -> str:\n        return "1.0.0"\n\n    def is_experimental(self) -> bool:\n        return False\n\n    def get_technical_links(self) -> Dict[str, str]:\n        return {\n            "Paper": "https://arxiv.org/abs/2010.04237",\n            "Code": "https://github.com/csteinmetz1/ronn"\n        }\n\n    def get_citation(self) -> str:\n        return "Steinmetz, C. J., & Reiss, J. D. (2020). Randomized overdrive neural networks. arXiv preprint arXiv:2010.04237."\n```\n\nCheck out the documentation of the methods inside [core.py](neutone_sdk/core.py), as well as the random overdrive model on the [website](https://neutone.space/models/) and in the plugin to understand where each field will be displayed.\n\nTo submit a model, please [open an issue on the GitHub repository](https://github.com/QosmoInc/neutone_sdk/issues/new?assignees=bogdanteleaga%2C+christhetree&labels=enhancement&template=request-add-model.md&title=%5BMODEL%5D+%3CNAME%3E). We currently need the following:\n- A short description of what the model does and how it can contribute to the community\n- A link to the `model.nm` file outputted by the `save_neutone_model` helper function\n\n<a name="contributing"/>\n\n## Contributing to the SDK\n\nWe welcome any contributions to the SDK. Please add types wherever possible and use the `black` formatter for readability.\n\nThe current roadmap is:\n- Additional testing and benchmarking of models during or after exporting\n- Implement lookahead and on the fly STFT transforms\n\n<a name="credits"/>\n\n## Credits\n\nThe audacitorch project was a major inspiration for the development of the SDK. [Check it out here](\nhttps://github.com/hugofloresgarcia/audacitorch)\n\n',
+    'long_description': '# Neutone SDK\n\nWe open source this SDK so researchers can wrap their own audio models and run them in a DAW using our [Neutone Plugin](https://neutone.space/). We offer both functionality for loading the models locally in the plugin as well as contributing them to the default list of models that is available to anyone running the plugin. We hope this will both give an opportunity for researchers to easily try their models in a DAW, but also provide creators with a collection of interesting models.\n\n<a name="examples"/>\n\n## Examples and Notebooks\n\n- Full clipper distortion model example can be found [here](examples/example_clipper.py).\n- Example of a random overdrive model based on [micro-tcn](https://github.com/csteinmetz1/micro-tcn) can be found [here](examples/example_overdrive-random.py)\n- Notebooks for different models showing the entire workflow from training to exporting it using Neutone\n    - [DDSP Timbre Transfer](https://colab.research.google.com/drive/1yPHU6PRWw1lRWZLUxXimIa6chFQ2JdRW?usp=sharing)\n    - [RAVE Timbre Transfer](https://colab.research.google.com/drive/1qlN6xLvDYrLcAwS8yh2ecmNG_bEKlVI9?usp=sharing)\n    - [TCN FX Emulation](https://colab.research.google.com/drive/1gHZ-AEoYmfmWrjlKpKkK_SW1xzfxD24-?usp=sharing)\n\n## v1 Release\n\nThe Neutone SDK is currently on version 1.0.0. Models exported with this version of the SDK will be incompatible with beta versions of the plugin to please make sure you are using the right version. \n\n\nThe restriction for a sampling rate of 48kHz and a buffer size of 2048 is now gone and the SDK contains a wrapper that supports on the fly resampling and queueing to accomodate the requirements of both the models and the DAW thanks to great work by [@christhetree](https://github.com/christhetree).\n\n\nThe following are known shortcomings:\n- Freezing models on save can cause instabilities, we recommend trying to save models both with and without freeze.\n- Displaying metadata information does not currently work with local model loading in the plugin.\n- Lookahead and on the fly STFT transforms will be implemented at the SDK level in the near future but is currently possible with additional code.\n- Windows and M1 acceleration are currently not supported.\n\nLogs are currently dumped to `/Users/<username>/Library/Application Support/Qosmo/Neutone/neutone.log`\n\n## Table of Contents\n- [Downloading the Neutone Plugin](#download)\n- [Installing the SDK](#install)\n- [SDK Description](#description)\n- [SDK Usage](#usage)\n- [Examples](#examples)\n- [Contributing to the SDK](#contributing)\n- [Credits](#credits)\n\n--- \n\n\n<a name="download"/>\n\n## Downloading the Plugin\n\nThe Neutone Plugin is available at [https://neutone.space](https://neutone.space). We currently offer VST3 and AU plugins that can be used to load the models created with this SDK. Please visit the website for more information.\n\n\n## Installing the SDK\n\n<a name="install"/>\n\nYou can install `neutone_sdk` using pip: \n\n```\npip install neutone_sdk\n```\n\n<a name="description"/>\n\n## SDK Description\n\nThe SDK provides functionality for wrapping existing PyTorch models in a way that can make them executable within the VST plugin. At its core the plugin is sending chunks of audio samples at a certain sample rate as an input and expects the same amount of samples at the output. Thus the simplest models also follow this input-output format and an example can be seen in [example_clipper.py](https://github.com/QosmoInc/neutone_sdk/blob/main/examples/example_clipper.py).\n\n<a name="usage"/>\n\n## SDK Usage\n\n### General Usage\n\nWe provide several models in the [examples](https://github.com/QosmoInc/neutone-sdk/blob/main/examples) directory. We will go through one of the simplest models, a distortion model, to illustrate.\n\nAssume we have the following PyTorch model. Parameters will be covered later on, we will focus on the inputs and outputs for now. Assume this model receives a Tensor of shape `(2, buffer_size)` as an input where `buffer_size` is a parameter that can be specified.\n\n```python\nclass ClipperModel(nn.Module):\n    def forward(self, x: Tensor, min_val: float, max_val: float, gain: float) -> Tensor:\n        return torch.clip(x, min=min_val * gain, max=max_val * gain)\n```\n\nTo run this inside the VST the simplest wrapper we can write is by subclassing the WaveformToWaveformBase baseclass.\n```python\nclass ClipperModelWrapper(WaveformToWaveformBase):\n    @torch.jit.export  \n    def is_input_mono(self) -> bool:\n        return False\n    \n    @torch.jit.export\n    def is_output_mono(self) -> bool:\n        return False\n    \n    @torch.jit.export\n    def get_native_sample_rates(self) -> List[int]:\n        return []  # Supports all sample rates\n    \n    @torch.jit.export\n    def get_native_buffer_sizes(self) -> List[int]:\n        return []  # Supports all buffer sizes\n\n    def do_forward_pass(self, x: Tensor, params: Dict[str, Tensor]) -> Tensor:\n        # ... Parameter unwrap logic\n        x = self.model.forward(x, min_val, max_val, gain)\n        return x\n ```\n\nThe method that does most of the work is `do_forward_pass`. In this case it is just a simple passthrough, but we will use it to handle parameters later on.\n\nBy default the VST runs as `stereo-stereo` but when mono is desired for the model we can use the `is_input_mono` and `is_output_mono` to inform the SDK and have the inputs and outputs converted automatically. If `is_input_mono` is toggled an averaged `(1, buffer_size)` shaped Tensor will be passed as an input instead of `(2, buffer_size)`. If `is_output_mono` is toggled, `do_forward_pass` is expected to return a mono Tensor (shape `(1, buffer_size)`) that will then be duplicated across both channels at the output of the VST. This is done within the SDK to avoid unnecessary memory allocations on each pass.\n\n`get_native_sample_rates` and `get_native_buffer_sizes` can be used to specify any preferred sample rates or buffer sizes. In most cases these are expected to only have one element but extra flexibility is provided for more complex models. In case multiple options are provided the SDK will try to find the best one for the current setting of the DAW. Whenever the sample rate or buffer size is different from the one of the DAW a wrapper is automatically triggered that converts to the correct sampling rate or implements a FIFO queue for the requested buffer size or both. This will incur a small performance penalty and add some amount of delay. In case a model is compatible with any sample rate and/or buffer_size these lists can be left empty.\n\nThis means that the tensor `x` in the `do_forward_pass` method is guaranteed to be of shape `(1 if is_input_mono else 2, buffer_size)`  where `buffer_size` will be chosen at runtime from the list provided in the `get_native_buffer_sizes` method.\n\n### Exporting models and loading in the plugin\n\nWe provide a `save_neutone_model` helper function that saves models to disk. By default this will convert models to TorchScript and run them through a series of checks to ensure they can be loaded by the plugin. The resulting `model.nm` file can be loaded within the plugin using the `load your own` button. Read below for how to submit models to the default collection.\n\n### Parameters\n\nFor models that can use conditioning signals we currently provide four configurable knob parameters. Within the `ClipperModelWrapper` defined above we can include the following:\n```python\nclass ClipperModelWrapper(WaveformToWaveformBase):\n    ...\n    \n    def get_neutone_parameters(self) -> List[NeutoneParameter]:\n        return [NeutoneParameter(name="min", description="min clip threshold", default_value=0.5),\n                NeutoneParameter(name="max", description="max clip threshold", default_value=1.0),\n                NeutoneParameter(name="gain", description="scale clip threshold", default_value=1.0)]\n         \n    def do_forward_pass(self, x: Tensor, params: Dict[str, Tensor]) -> Tensor:\n        min_val, max_val, gain = params["min"], params["max"], params["gain"]\n        x = self.model.forward(x, min_val, max_val, gain)\n        return x\n```\n\nDuring the forward pass the `params` variable will be a dictionary like the following:\n```python\n{\n    "min": torch.Tensor([0.5] * buffer_size),\n    "max": torch.Tensor([1.0] * buffer_size),\n    "gain": torch.Tensor([1.0] * buffer_size)\n}\n```\nThe keys of the dictionary are specified in the `get_parameters` function.\n\nThe parameters will always take values between 0 and 1 and the `do_forward_pass` function can be used to do any necessary rescaling before running the internal forward method of the model.\n\nMoreover, the parameters sent by the plugin come in at a sample level granularity. By default, we take the mean of each buffer and return a single float (as a Tensor), but the `aggregate_param` method can be used to override the aggregation method. See the full clipper export file for an example of preserving this granularity.\n\n\n### Submitting models\n\nThe plugin contains a default list of models aimed at creators that want to make use of them during their creative process. We encourage users to submit their models once they are happy with the results they get so they can be used by the community at large. For submission we require some additional metadata that will be used to display information about the model aimed at both creators and other researchers. This will be displayed on both the [Neutone website](https://neutone.space) and inside the plugin.\n\nSkipping the previous clipper model, here is a more realistic example based on a random TCN overdrive model inspired by [micro-tcn](https://github.com/csteinmetz1/micro-tcn).\n\n```python\nclass OverdriveModelWrapper(WaveformToWaveformBase):\n    def get_model_name(self) -> str:\n        return "conv1d-overdrive.random"\n\n    def get_model_authors(self) -> List[str]:\n        return ["Nao Tokui"]\n\n    def get_model_short_description(self) -> str:\n        return "Neural distortion/overdrive effect"\n\n    def get_model_long_description(self) -> str:\n        return "Neural distortion/overdrive effect through randomly initialized Convolutional Neural Network"\n\n    def get_technical_description(self) -> str:\n        return "Random distortion/overdrive effect through randomly initialized Temporal-1D-convolution layers. You\'ll get different types of distortion by re-initializing the weight or changing the activation function. Based on the idea proposed by Steinmetz et al."\n\n    def get_tags(self) -> List[str]:\n        return ["distortion", "overdrive"]\n\n    def get_model_version(self) -> str:\n        return "1.0.0"\n\n    def is_experimental(self) -> bool:\n        return False\n\n    def get_technical_links(self) -> Dict[str, str]:\n        return {\n            "Paper": "https://arxiv.org/abs/2010.04237",\n            "Code": "https://github.com/csteinmetz1/ronn"\n        }\n\n    def get_citation(self) -> str:\n        return "Steinmetz, C. J., & Reiss, J. D. (2020). Randomized overdrive neural networks. arXiv preprint arXiv:2010.04237."\n```\n\nCheck out the documentation of the methods inside [core.py](neutone_sdk/core.py), as well as the random overdrive model on the [website](https://neutone.space/models/) and in the plugin to understand where each field will be displayed.\n\nTo submit a model, please [open an issue on the GitHub repository](https://github.com/QosmoInc/neutone_sdk/issues/new?assignees=bogdanteleaga%2C+christhetree&labels=enhancement&template=request-add-model.md&title=%5BMODEL%5D+%3CNAME%3E). We currently need the following:\n- A short description of what the model does and how it can contribute to the community\n- A link to the `model.nm` file outputted by the `save_neutone_model` helper function\n\n<a name="contributing"/>\n\n## Contributing to the SDK\n\nWe welcome any contributions to the SDK. Please add types wherever possible and use the `black` formatter for readability.\n\nThe current roadmap is:\n- Additional testing and benchmarking of models during or after exporting\n- Implement lookahead and on the fly STFT transforms\n\n<a name="credits"/>\n\n## Credits\n\nThe audacitorch project was a major inspiration for the development of the SDK. [Check it out here](\nhttps://github.com/hugofloresgarcia/audacitorch)\n\n',
     'author': 'Qosmo',
     'author_email': 'contact@qosmo.jp',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/QosmoInc/neutone_sdk.git',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `neutone_sdk-1.1.3/PKG-INFO` & `neutone_sdk-1.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neutone-sdk
-Version: 1.1.3
+Version: 1.2.1
 Summary: SDK for wrapping deep learning models for usage in the Neutone plugin
 Home-page: https://github.com/QosmoInc/neutone_sdk.git
 License: LGPL
 Author: Qosmo
 Author-email: contact@qosmo.jp
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
@@ -29,16 +29,17 @@
 <a name="examples"/>
 
 ## Examples and Notebooks
 
 - Full clipper distortion model example can be found [here](examples/example_clipper.py).
 - Example of a random overdrive model based on [micro-tcn](https://github.com/csteinmetz1/micro-tcn) can be found [here](examples/example_overdrive-random.py)
 - Notebooks for different models showing the entire workflow from training to exporting it using Neutone
-    - [DDSP](https://colab.research.google.com/drive/15FuafmtGWEyvTOOQbN1AMIQRhGLy23Pg)
-    - [RAVE](https://colab.research.google.com/drive/1hty5Bd7rJJ70hlI-5720sEY3kylNxBIt)
+    - [DDSP Timbre Transfer](https://colab.research.google.com/drive/1yPHU6PRWw1lRWZLUxXimIa6chFQ2JdRW?usp=sharing)
+    - [RAVE Timbre Transfer](https://colab.research.google.com/drive/1qlN6xLvDYrLcAwS8yh2ecmNG_bEKlVI9?usp=sharing)
+    - [TCN FX Emulation](https://colab.research.google.com/drive/1gHZ-AEoYmfmWrjlKpKkK_SW1xzfxD24-?usp=sharing)
 
 ## v1 Release
 
 The Neutone SDK is currently on version 1.0.0. Models exported with this version of the SDK will be incompatible with beta versions of the plugin to please make sure you are using the right version. 
 
 
 The restriction for a sampling rate of 48kHz and a buffer size of 2048 is now gone and the SDK contains a wrapper that supports on the fly resampling and queueing to accomodate the requirements of both the models and the DAW thanks to great work by [@christhetree](https://github.com/christhetree).
```

