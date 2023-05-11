# Comparing `tmp/groqflow-2.5.2.tar.gz` & `tmp/groqflow-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groqflow-2.5.2.tar", last modified: Mon Jan 30 15:23:10 2023, max compression
+gzip compressed data, was "groqflow-3.0.2.tar", last modified: Thu May 11 15:26:06 2023, max compression
```

## Comparing `groqflow-2.5.2.tar` & `groqflow-3.0.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 15:23:10.149025 groqflow-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-01-30 15:23:10.145025 groqflow-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-01-30 15:22:58.000000 groqflow-2.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 15:23:10.141025 groqflow-2.5.2/groqflow/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 15:23:10.145025 groqflow-2.5.2/groqflow/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20255 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/common/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/common/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/common/onnx_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/common/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/common/quantization_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/common/sdk_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/common/tensor_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 15:23:10.145025 groqflow-2.5.2/groqflow/groqmodel/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/groqmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/groqmodel/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)    21949 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/groqmodel/groqmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/groqmodel/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 15:23:10.145025 groqflow-2.5.2/groqflow/justgroqit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/justgroqit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/justgroqit/assemble_multichip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/justgroqit/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)    23970 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/justgroqit/export.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6074 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/justgroqit/groqit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/justgroqit/hummingbird.py
--rw-r--r--   0 runner    (1001) docker     (123)    28713 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/justgroqit/ignition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/justgroqit/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-30 15:22:58.000000 groqflow-2.5.2/groqflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 15:23:10.141025 groqflow-2.5.2/groqflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-01-30 15:23:10.000000 groqflow-2.5.2/groqflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-01-30 15:23:10.000000 groqflow-2.5.2/groqflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 15:23:10.000000 groqflow-2.5.2/groqflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-30 15:23:10.000000 groqflow-2.5.2/groqflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-30 15:23:10.000000 groqflow-2.5.2/groqflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-30 15:22:58.000000 groqflow-2.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 15:23:10.149025 groqflow-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-01-30 15:22:58.000000 groqflow-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:26:06.202463 groqflow-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-11 15:26:06.202463 groqflow-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-11 15:25:55.000000 groqflow-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:26:06.194463 groqflow-3.0.2/groqflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:26:06.198463 groqflow-3.0.2/groqflow/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19995 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/onnx_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/quantization_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/sdk_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/tensor_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/tf_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:26:06.198463 groqflow-3.0.2/groqflow/groqmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/groqmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/groqmodel/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22107 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/groqmodel/groqmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/groqmodel/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:26:06.202463 groqflow-3.0.2/groqflow/justgroqit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/justgroqit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/justgroqit/assemble_multichip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/justgroqit/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24108 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/justgroqit/export.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6101 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/justgroqit/groqit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/justgroqit/hummingbird.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28555 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/justgroqit/ignition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/justgroqit/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:26:06.194463 groqflow-3.0.2/groqflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-11 15:26:06.000000 groqflow-3.0.2/groqflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-11 15:26:06.000000 groqflow-3.0.2/groqflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:26:06.000000 groqflow-3.0.2/groqflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-11 15:26:06.000000 groqflow-3.0.2/groqflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 15:26:06.000000 groqflow-3.0.2/groqflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-11 15:25:56.000000 groqflow-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:26:06.202463 groqflow-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-11 15:25:56.000000 groqflow-3.0.2/setup.py
```

### Comparing `groqflow-2.5.2/groqflow/common/build.py` & `groqflow-3.0.2/groqflow/common/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,39 +9,32 @@
 import dataclasses
 import hashlib
 import yaml
 import torch
 import numpy as np
 import sklearn.base
 import groqflow.common.exceptions as exp
+import groqflow.common.tf_helpers as tf_helpers
 
-try:
-    import tensorflow as tf
-except ModuleNotFoundError as module_error:
-    raise exp.GroqitEnvError(
-        "GroqFlow added a dependence on tensorflow in version 2.1.2. "
-        "You must install tensorflow to continue."
-    )
+
+class Groqcard(enum.Enum):
+    A14 = "A1.4"
+    A11 = "A1.1"
 
 
 UnionValidModelInstanceTypes = Union[
     None,
     str,
     torch.nn.Module,
     torch.jit.ScriptModule,
-    tf.keras.Model,
+    "tf.keras.Model",
     sklearn.base.BaseEstimator,
 ]
 
 
-class Groqcard(enum.Enum):
-    A14 = "A1.4"
-    A11 = "A1.1"
-
-
 # WARNING: The "internal" env var may cause unexpected behavior if enabled
 # outside of the internal Groq dev environment.
 environment_variables = {
     "cache_dir": "GROQFLOW_CACHE_DIR",
     "rebuild": "GROQIT_REBUILD_POLICY",
     "dont_use_sdk": "GROQFLOW_BAKE_SDK",
     "target_a11": "GROQFLOW_LEGACY_A11",
@@ -240,15 +233,15 @@
         value = inputs[key]
         if (
             isinstance(
                 value,
                 (list, tuple),
             )
             or torch.is_tensor(value)
-            or tf.is_tensor(value)
+            or tf_helpers.is_keras_tensor(value)
         ):
             shapes[key] = np.array(value).shape
             dtypes[key] = np.array(value).dtype.name
         elif isinstance(value, np.ndarray):
             shapes[key] = value.shape
             dtypes[key] = value.dtype.name
         elif isinstance(value, (bool, int, float)):
@@ -523,19 +516,18 @@
         state_dict["info"]["backend"] = self.info.backend.value
 
         # During actual execution, quantization_samples in the state
         # stores the actual quantization samples.
         # However, we do not save quantization samples
         # Instead, we save a boolean to indicate whether the model
         # stored has been quantized by some samples.
-        for key, value in vars(self).items():
-            if key == "quantization_samples" and value is not None:
-                state_dict["quantization_samples"] = True
-            else:
-                state_dict["quantization_samples"] = False
+        if self.quantization_samples:
+            state_dict["quantization_samples"] = True
+        else:
+            state_dict["quantization_samples"] = False
 
         with open(
             state_file(self.cache_dir, self.config.build_name), "w", encoding="utf8"
         ) as outfile:
             yaml.dump(state_dict, outfile)
```

### Comparing `groqflow-2.5.2/groqflow/common/cache.py` & `groqflow-3.0.2/groqflow/common/cache.py`

 * *Files identical despite different names*

### Comparing `groqflow-2.5.2/groqflow/common/exceptions.py` & `groqflow-3.0.2/groqflow/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `groqflow-2.5.2/groqflow/common/onnx_helpers.py` & `groqflow-3.0.2/groqflow/common/onnx_helpers.py`

 * *Files identical despite different names*

### Comparing `groqflow-2.5.2/groqflow/common/printing.py` & `groqflow-3.0.2/groqflow/common/printing.py`

 * *Files identical despite different names*

### Comparing `groqflow-2.5.2/groqflow/common/quantization_helpers.py` & `groqflow-3.0.2/groqflow/common/quantization_helpers.py`

 * *Files identical despite different names*

### Comparing `groqflow-2.5.2/groqflow/common/sdk_helpers.py` & `groqflow-3.0.2/groqflow/common/sdk_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 """
 Helper functions for interfacing with the GroqWare SDK
 """
 
 import os
-import re
 import enum
 import subprocess
 import shutil
 from typing import Type, Union
 from pkg_resources import parse_version
 import groqflow.common.build as build
 import groqflow.common.exceptions as exp
-import groqflow.common.printing as printing
 
 
-# Older than min release version fails
-# Not equal to current release version is unsupported and warns
-# but may still work
-MIN_RELEASE_VERSION = "0.9.2"
-CURRENT_RELEASE_VERSION = "0.9.2"
-VALID_VERSIONS = [CURRENT_RELEASE_VERSION, "test"]
+MIN_RELEASE_VERSION = "0.9.2.1"
 
 
 class OS(enum.Enum):
     UBUNTU = "Ubuntu"
     ROCKY = "Rocky Linux"
 
 
@@ -110,69 +103,54 @@
         # The following exception will only be raised if a GroqFlow dev forgets to update
         # _installed_package_version() when adding support for a new OS
         raise exp.GroqitEnvError(
             f"_installed_package_version not implemented for {os_version}"
         )
 
 
-def is_release_candidate(sdkv: str) -> bool:
+def version_a_less_than_b(version_a, version_b: str):
     """
-    This function returns true if the SDK number provided corresponds to a release candidate
-    SDK release candidates use the format major.minor.patch~release_candidate_number
+    Return true if version_a >= version_b, following the scheme:
+        major.minor.patch.patchpatch~release_candidate_number
+
+    The release_candidate_number should be ignored.
     """
-    return re.match(r"^[0-9]+\.[0-9]+\.[0-9]+~[0-9]+$", sdkv) is not None
+
+    # Strip the release candidate number, if any
+    clean_version_a = version_a.split("~")[0]
+    clean_version_b = version_b.split("~")[0]
+
+    return parse_version(clean_version_a) < parse_version(clean_version_b)
 
 
 def version_is_valid(
     sdkv: Union[str, bool],
     required: bool,
     requirement_name: str,
     exception_type: Type[Exception] = exp.GroqitEnvError,
     hint: str = "",
-) -> bool:
+):
+    """
+    Raise an exception if the required version number is not installed
+    """
+
     msg = (
         f"{requirement_name}>={MIN_RELEASE_VERSION} is a required dependency "
         "for this part of GroqFlow"
     )
 
     # Package not found
-    if not sdkv:
-        if required:
-            msg = msg + f". However, {requirement_name} was not found. "
-            raise exception_type(msg + hint)
-        else:
-            return False
-    # Package found, but version is not acceptable
-    elif sdkv not in VALID_VERSIONS and not is_release_candidate(sdkv):
-        if required:
-            if parse_version(sdkv) < parse_version(MIN_RELEASE_VERSION):
-                msg = msg + f" ({sdkv} is installed). "
-                raise exception_type(msg + hint)
-            else:
-                msg = (
-                    "This version of Groqflow is only officially supported with "
-                    f"{requirement_name}=={CURRENT_RELEASE_VERSION} but the installed "
-                    f"{requirement_name} is version {sdkv}. This may still work but "
-                    f"ensure you are using {CURRENT_RELEASE_VERSION} before "
-                    "opening a support ticket."
-                )
-                printing.log_warning(msg)
-        else:
-            return False
-    # User has a release candidate installed
-    elif is_release_candidate(sdkv):
-        msg = (
-            "This machine has a GroqWare SDK release candidate installed. "
-            "If you encounter unexpected behavior, please try again with the "
-            f"officially supported SDK version, {CURRENT_RELEASE_VERSION}."
-        )
-        printing.log_warning(msg)
+    if not sdkv and required:
+        msg = msg + f". However, {requirement_name} was not found. "
+        raise exception_type(msg + hint)
 
-    # Package found and has a valid version
-    return True
+    # Package found, but version is not acceptable
+    elif version_a_less_than_b(sdkv, MIN_RELEASE_VERSION) and required:
+        msg = msg + f" ({sdkv} is installed). "
+        raise exception_type(msg + hint)
 
 
 def validate_os_version() -> OS:
 
     supported_os_names = [x.value for x in OS]
     unsupported_os_msg = (
         "Your OS must be one of the following Linux distributions: "
@@ -201,75 +179,79 @@
 def validate_devtools(
     os_version: OS,
     required=False,
     exception_type: Type[Exception] = exp.GroqitEnvError,
 ) -> Union[bool, str]:
     version = _installed_package_version("groq-devtools", os_version)
     hint = "Please contact sales@groq.com to get access to groq-devtools."
-    return version_is_valid(version, required, "groq-devtools", exception_type, hint)
+    version_is_valid(version, required, "groq-devtools", exception_type, hint)
 
 
 def validate_runtime(
     os_version: OS,
     required=False,
     exception_type: Type[Exception] = exp.GroqitEnvError,
 ) -> Union[bool, str]:
     version = _installed_package_version("groq-runtime", os_version)
     hint = "Please contact sales@groq.com to get access to groq-runtime."
-    return version_is_valid(version, required, "groq-runtime", exception_type, hint)
+    version_is_valid(version, required, "groq-runtime", exception_type, hint)
 
 
-# Return the result of bake groot
-def _bake_groot():
+# Returns the root directory of the current git repo and any associated
+# error from running the git command
+def get_repo_root():
     p = subprocess.Popen(
-        ["bake", "groot"],
+        ["git", "rev-parse", "--show-toplevel"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
-    repo, err = p.communicate()
-    repo = repo.decode("utf-8")
+    out, err = p.communicate()
+    repo = out.decode("utf-8")
+    repo = repo.rstrip("\n")
     err = err.decode("utf-8")
-
     return repo, err
 
 
 def validate_bake():
     if not shutil.which("bake"):
         raise exp.GroqitEnvError(
             (
                 "Bake must be available when the env var "
                 f'{build.environment_variables["dont_use_sdk"]} is set to True'
             )
         )
 
-    repo, err = _bake_groot()
+    # bake commands require Groq to be current git repo
+    repo, err = get_repo_root()
+    groq_root = repo.split("/")[-1] == "Groq"
 
-    if err and repo:
+    if err:
         raise exp.GroqitEnvError(
             (
                 "You must be inside the Groq repo when the env var "
                 f'{build.environment_variables["dont_use_sdk"]} is set to True. '
-                f"groqit() detected you are inside repo {repo}"
+                f"groqit() returned with error {err}"
             )
         )
 
-    if err:
+    elif not groq_root:
         raise exp.GroqitEnvError(
             (
                 "You must be inside the Groq repo when the env var "
-                f'{build.environment_variables["dont_use_sdk"]} is set to True'
+                f'{build.environment_variables["dont_use_sdk"]} is set to True. '
+                f"groqit() detected you are inside repo {repo}"
             )
         )
 
 
 def check_dependencies(
     require_devtools: bool = False,
     require_runtime: bool = False,
     exception_type: Type[Exception] = exp.GroqitEnvError,
-) -> bool:
+):
 
     # Skip dependency check if necessary
     if os.environ.get("GROQFLOW_SKIP_SDK_CHECK") == "True":
         return True
 
     # Check for bake if SDK is not being used
     if not build.USE_SDK:
@@ -284,9 +266,7 @@
             exception_type=exception_type,
         )
         validate_runtime(
             os_version=os_version,
             required=require_runtime,
             exception_type=exception_type,
         )
-
-    return True
```

### Comparing `groqflow-2.5.2/groqflow/common/tensor_helpers.py` & `groqflow-3.0.2/groqflow/common/tensor_helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,22 +4,15 @@
 
 import os
 import copy
 import torch
 import numpy as np
 import groqflow.common.exceptions as exp
 import groqflow.common.build as build
-
-try:
-    import tensorflow as tf
-except ModuleNotFoundError as module_error:
-    raise exp.GroqitEnvError(
-        "GroqFlow added a dependence on tensorflow in version 2.1.2. "
-        "You must install tensorflow to continue."
-    )
+import groqflow.common.tf_helpers as tf_helpers
 
 # Checks whether a given input has the expected shape
 def check_shapes_and_dtypes(inputs, expected_shapes, expected_dtypes):
     current_shapes, current_dtypes = build.get_shapes_and_dtypes(inputs)
     if not expected_shapes == current_shapes:
         msg = f"""
         Groq Model compiled to always take input of shape
@@ -43,15 +36,15 @@
             k: v for k, v in inputs_converted[i].items() if v is not None
         }
         for k in inputs_converted[i].keys():
             if not hasattr(inputs_converted[i][k], "dtype"):
                 continue
             if torch.is_tensor(inputs_converted[i][k]):
                 inputs_converted[i][k] = inputs_converted[i][k].cpu().detach().numpy()
-            if tf.is_tensor(inputs_converted[i][k]):
+            if tf_helpers.is_keras_tensor(inputs_converted[i][k]):
                 inputs_converted[i][k] = inputs_converted[i][k].numpy()
             if downcast:
                 if input_dtypes is not None and input_dtypes[k] is not None:
                     inputs_converted[i][k] = inputs_converted[i][k].astype(
                         input_dtypes[k]
                     )
                     continue
```

### Comparing `groqflow-2.5.2/groqflow/groqmodel/execute.py` & `groqflow-3.0.2/groqflow/groqmodel/execute.py`

 * *Files identical despite different names*

### Comparing `groqflow-2.5.2/groqflow/groqmodel/groqmodel.py` & `groqflow-3.0.2/groqflow/groqmodel/groqmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,34 +5,20 @@
 import pathlib
 from typing import Optional, Dict, List, Tuple, Any
 from collections.abc import Collection
 from dataclasses import dataclass
 import numpy as np
 import torch
 
-# TODO: Remove try block once GroqFlow "remote" and "cloud" become part of the release
-try:
-    import groqflow.groqmodel.cloud as cloud
-    import groqflow.groqmodel.remote as remote
-except ModuleNotFoundError:
-    # Proper exceptions are raised if we attempt to use this module on a release branch
-    pass
 import groqflow.common.exceptions as exp
 import groqflow.common.printing as printing
 import groqflow.common.build as build
 import groqflow.common.sdk_helpers as sdk
 import groqflow.common.tensor_helpers as tensor_helpers
-
-try:
-    import tensorflow as tf
-except ModuleNotFoundError as module_error:
-    raise exp.GroqModelEnvError(
-        "GroqFlow added a dependence on tensorflow in version 2.1.2. "
-        "You must install tensorflow to continue."
-    )
+import groqflow.common.tf_helpers as tf_helpers
 
 
 @dataclass
 class GroqEstimatedPerformance:
     pcie_input_latency: float
     compute_latency: float
     pcie_output_latency: float
@@ -285,35 +271,47 @@
                 print(
                     "Switching to GroqCloud server, since this machine has no GroqChip processors"
                 )
             else:
                 backend = build.Backend.LOCAL
 
         # Check if we are trying to use GroqFlow Remote/Cloud on a public release
-        if (
-            backend == build.Backend.CLOUD
-            and "groqflow.groqmodel.cloud" not in sys.modules
-        ) or (
-            backend == build.Backend.REMOTE
-            and "groqflow.groqmodel.remote" not in sys.modules
-        ):
-            raise exp.GroqModelEnvError(
-                (
-                    f"GroqFlow {backend.value} is not publicly available yet. "
-                    "Please set the environment variable GROQMODEL_BACKEND to 'local'."
+        if backend == build.Backend.CLOUD:
+            try:
+                import mlagility.api.cloud as cloud  # pylint: disable=import-error
+
+                sys.modules["cloud"] = cloud
+            except ModuleNotFoundError:
+                raise exp.GroqModelEnvError(
+                    (
+                        'To use GroqFlow "cloud" backend please install mlagility. '
+                        "You can find more information at github.com/groq/mlagility."
+                    )
+                )
+        elif backend == build.Backend.REMOTE:
+
+            try:
+                import groqflow.groqmodel.remote as remote
+
+                sys.modules["remote"] = remote
+            except ModuleNotFoundError:
+                raise exp.GroqModelEnvError(
+                    (
+                        f"GroqFlow {backend.value} is not publicly available yet. "
+                        "Please set the environment variable GROQMODEL_BACKEND to 'local'."
+                    )
                 )
-            )
 
         if backend == build.Backend.REMOTE and self.remote_client is None:
             # Setup remote client if needed
             remote_url = os.environ.get("GROQFLOW_REMOTE_URL")
             self.remote_client = (
-                remote.RemoteClient()
+                sys.modules["remote"].RemoteClient()
                 if remote_url is None
-                else remote.RemoteClient(remote_url)
+                else sys.modules["remote"].RemoteClient(remote_url)
             )
 
         return backend
 
     # Shared execution function
     def _execute(
         self, input_collection: Collection, repetitions: int
@@ -354,15 +352,15 @@
             os.remove(self.state.latency_file)
 
         bringup_topology = shared_state.topology_initialized(self.state.topology)
 
         # Select execution script according to backend
         backend = self._select_backend()
         if backend == build.Backend.CLOUD:
-            cloud.execute_groqchip_remotely(
+            sys.modules["cloud"].execute_groqchip_remotely(
                 bringup_topology, repetitions, self.state, self.log_execute_path
             )
         elif backend == build.Backend.REMOTE:
             try:
                 self.remote_client.execute(self.state, repetitions)
             except Exception as e:
                 raise exp.GroqModelRemoteError(
@@ -376,16 +374,20 @@
         return self.state.outputs_file, GroqMeasuredPerformance(self.state.latency_file)
 
     # Models with a single output are returned as either a torch.tensor,
     # tf.Tensor, or an np.array (see tensor_type)
     # Models with multiple outputs are returned as either a tuple of
     # torch.tensors, tf.Tensors, or np.arrays
     def _unpack_results(self, results: List[Dict], output_nodes, num_outputs):
-        if self.tensor_type is tf.Tensor:
-            unpacked_results = [tf.convert_to_tensor(results[x]) for x in output_nodes]
+        if tf_helpers.type_is_tf_tensor(self.tensor_type):
+            import tensorflow
+
+            unpacked_results = [
+                tensorflow.convert_to_tensor(results[x]) for x in output_nodes
+            ]
         else:
             unpacked_results = [self.tensor_type(results[x]) for x in output_nodes]
         return unpacked_results[0] if num_outputs == 1 else tuple(unpacked_results)
 
     def _unpack_results_file(self, packed_results: str) -> Any:
         """
         Unpack execution results from a file
@@ -527,15 +529,17 @@
     # Pytorch models are callable
     def __call__(self, **kwargs):
         return self.run(kwargs)
 
 
 class KerasModelWrapper(GroqModel):
     def __init__(self, state):
-        tensor_type = tf.Tensor
+        import tensorflow
+
+        tensor_type = tensorflow.Tensor
         super(KerasModelWrapper, self).__init__(state, tensor_type)
 
     # Keras models are callable
     def __call__(self, **kwargs):
         return self.run(kwargs)
```

### Comparing `groqflow-2.5.2/groqflow/groqmodel/remote.py` & `groqflow-3.0.2/groqflow/groqmodel/remote.py`

 * *Files identical despite different names*

### Comparing `groqflow-2.5.2/groqflow/justgroqit/assemble_multichip.py` & `groqflow-3.0.2/groqflow/justgroqit/assemble_multichip.py`

 * *Files identical despite different names*

### Comparing `groqflow-2.5.2/groqflow/justgroqit/compile.py` & `groqflow-3.0.2/groqflow/justgroqit/compile.py`

 * *Files identical despite different names*

### Comparing `groqflow-2.5.2/groqflow/justgroqit/export.py` & `groqflow-3.0.2/groqflow/justgroqit/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,14 @@
 import groqflow.common.exceptions as exp
 import groqflow.common.build as build
 import groqflow.common.tensor_helpers as tensor_helpers
 import groqflow.common.onnx_helpers as onnx_helpers
 import groqflow.common.sdk_helpers as sdk
 import groqflow.common.quantization_helpers as quant_helpers
 
-try:
-    import tensorflow as tf
-    import tf2onnx
-except ModuleNotFoundError as module_error:
-    raise exp.GroqitEnvError(
-        "GroqFlow added a dependence on tensorflow and tf2onnx in version 2.1.2. "
-        "You must install tensorflow and tf2onnx to continue."
-    )
-
 
 def _check_model(onnx_file, success_message, fail_message) -> bool:
     if os.path.isfile(onnx_file):
         print(success_message)
     else:
         print(fail_message)
         return False
@@ -40,17 +31,25 @@
         return True
     except onnx.checker.ValidationError as e:
         print("\tError while checking generated ONNX file")
         print(e)
         return False
 
 
-def get_output_names(onnx_model: Union[str, onnx.ModelProto]):
+def _warn_to_stdout(message, category, filename, line_number, _, line):
+    sys.stdout.write(
+        warnings.formatwarning(message, category, filename, line_number, line)
+    )
+
+
+def get_output_names(
+    onnx_model: Union[str, onnx.ModelProto]
+):  # pylint: disable=no-member
     # Get output names of ONNX file/model
-    if not isinstance(onnx_model, onnx.ModelProto):
+    if not isinstance(onnx_model, onnx.ModelProto):  # pylint: disable=no-member
         onnx_model = onnx.load(onnx_model)
     return [node.name for node in onnx_model.graph.output]  # pylint: disable=no-member
 
 
 class ReceiveOnnxModel(stage.GroqitStage):
     """
     Stage that takes an ONNX model as input.
@@ -232,21 +231,16 @@
             # Collect input names
             dummy_input_names = tuple(state.inputs.keys())
 
         state.info.opset = build.DEFAULT_ONNX_OPSET
 
         # Send torch export warnings to stdout (and therefore the log file)
         # so that they don't fill up the command line
-        def warn_to_stdout(message, category, filename, line_number, _, __):
-            sys.stdout.write(
-                warnings.formatwarning(message, category, filename, line_number)
-            )
-
         default_warnings = warnings.showwarning
-        warnings.showwarning = warn_to_stdout
+        warnings.showwarning = _warn_to_stdout
 
         # Export the model to ONNX
         torch.onnx.export(
             state.model,
             dummy_inputs,
             state.base_onnx_file,
             input_names=dummy_input_names,
@@ -306,14 +300,17 @@
     def __init__(self):
         super().__init__(
             unique_name="export_keras",
             monitor_message="Exporting Keras to ONNX",
         )
 
     def fire(self, state: build.State):
+        import tensorflow as tf
+        import tf2onnx
+
         if not isinstance(state.model, (tf.keras.Model)):
             msg = f"""
             The current stage (ExportKerasModel) is only compatible with
             models of type tf.keras.Model, however
             the stage received a model of type {type(state.model)}.
             """
             raise exp.GroqitStageError(msg)
@@ -547,14 +544,19 @@
 
         # Convert the model to FP16
         # Some ops will not be converted to fp16 because they are in a block list
         # The latest list can be found here. It is not neccesarily the list that
         # our version of onnxmltools sees
         # https://github.com/microsoft/onnxconverter-common/blob/master/onnxconverter_common/float16.py#L82
 
+        # Send onnxmltools warnings to stdout (and therefore the log file)
+        # so that they don't fill up the command line
+        default_warnings = warnings.showwarning
+        warnings.showwarning = _warn_to_stdout
+
         # Legalize ops are ops that have been or are currently in the block list
         # that we explicitly want removed
         legalize_ops = ["InstanceNormalization", "Resize", "Max"]
         op_block_list = onnxmltools.utils.float16_converter.DEFAULT_OP_BLOCK_LIST.copy()
         for op in legalize_ops:
             # Check to see that they are not in the block list before we remove them
             # Neccesary because the block list may be updated, and not in the state we expect
@@ -572,14 +574,17 @@
         # Save FP16 model (use external data format if needed)
         output_path = state.converted_onnx_file
         try:
             onnxmltools.utils.save_model(fp16_model, output_path)
         except ValueError:
             onnx.save_model(fp16_model, output_path, save_as_external_data=True)
 
+        # Restore default warnings behavior
+        warnings.showwarning = default_warnings
+
         # Check that the converted model is still valid
         success_msg = "\tSuccess converting ONNX model to fp16"
         fail_msg = "\tFailed converting ONNX model to fp16"
         state.info.converted_onnx_exported = _check_model(
             state.converted_onnx_file, success_msg, fail_msg
         )
```

### Comparing `groqflow-2.5.2/groqflow/justgroqit/groqit.py` & `groqflow-3.0.2/groqflow/justgroqit/groqit.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     (config, auto_name) = ignition.lock_config(
         build_name=build_name,
         compiler_flags=compiler_flags,
         assembler_flags=assembler_flags,
         groqview=groqview,
         groqcard=build.GROQCARD,
         num_chips=num_chips,
+        sequence=sequence,
     )
 
     # Analyze the user's model argument and lock in the model, inputs,
     # and sequence that will be used by the rest of groqit()
     (
         model_locked,
         inputs_locked,
```

### Comparing `groqflow-2.5.2/groqflow/justgroqit/hummingbird.py` & `groqflow-3.0.2/groqflow/justgroqit/hummingbird.py`

 * *Files identical despite different names*

### Comparing `groqflow-2.5.2/groqflow/justgroqit/ignition.py` & `groqflow-3.0.2/groqflow/justgroqit/ignition.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,28 +7,21 @@
 import types
 import torch
 from typeguard import typechecked
 import groqflow.common.build as build
 import groqflow.common.cache as cache
 import groqflow.common.exceptions as exp
 import groqflow.common.printing as printing
+import groqflow.common.tf_helpers as tf_helpers
 import groqflow.justgroqit.compile as compile
 import groqflow.justgroqit.export as export
 import groqflow.justgroqit.stage as stage
 import groqflow.justgroqit.hummingbird as hummingbird
 from groqflow import __version__ as groqflow_version
 
-try:
-    import tensorflow as tf
-except ModuleNotFoundError as module_error:
-    raise exp.GroqitEnvError(
-        "GroqFlow added a dependence on tensorflow in version 2.1.2. "
-        "You must install tensorflow to continue."
-    )
-
 default_pytorch_export_sequence = stage.Sequence(
     "default_pytorch_export_sequence",
     "Exporting PyTorch Model",
     [
         export.ExportPytorchModel(),
         export.OptimizeOnnxModel(),
         export.CheckOnnxCompatibility(),
@@ -617,16 +610,16 @@
                 groqit() received a model argument that was a path to a model file,
                 which returned a path to another file: {model}. However,
                 it is required for these returned paths to point to a ".onnx" file.
                 """
                 raise exp.GroqitIntakeError(msg)
 
         elif isinstance(
-            model, (torch.nn.Module, torch.jit.ScriptModule, tf.keras.Model)
-        ):
+            model, (torch.nn.Module, torch.jit.ScriptModule)
+        ) or tf_helpers.is_keras_model(model):
             return model, inputs, corpus
 
         else:
             msg = f"""
             groqit() received a model argument that was a path to a model.py file.
             All model.py files are required to return either an ONNX file path,
             a PyTorch model object, or a Keras model object, however the model.py
@@ -693,17 +686,17 @@
     # Validate that the model's type is supported by groqit()
     # and assign a ModelType tag
     if isinstance(model, (torch.nn.Module, torch.jit.ScriptModule)):
         model_type = build.ModelType.PYTORCH
     elif isinstance(model, str):
         if model.endswith(".onnx"):
             model_type = build.ModelType.ONNX_FILE
-    elif isinstance(model, tf.keras.Model):
+    elif tf_helpers.is_keras_model(model):
         model_type = build.ModelType.KERAS
-        if not tf.executing_eagerly():
+        if not tf_helpers.is_executing_eagerly():
             raise exp.GroqitIntakeError(
                 "`groqit()` requires Keras models to be run in eager execution mode. "
                 "Enable eager execution to continue."
             )
         if not model.built:
             raise exp.GroqitIntakeError(
                 "Keras model has not been built. Please call "
```

### Comparing `groqflow-2.5.2/groqflow/justgroqit/stage.py` & `groqflow-3.0.2/groqflow/justgroqit/stage.py`

 * *Files identical despite different names*

### Comparing `groqflow-2.5.2/groqflow.egg-info/SOURCES.txt` & `groqflow-3.0.2/groqflow.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 groqflow/common/cache.py
 groqflow/common/exceptions.py
 groqflow/common/onnx_helpers.py
 groqflow/common/printing.py
 groqflow/common/quantization_helpers.py
 groqflow/common/sdk_helpers.py
 groqflow/common/tensor_helpers.py
+groqflow/common/tf_helpers.py
 groqflow/groqmodel/__init__.py
 groqflow/groqmodel/execute.py
 groqflow/groqmodel/groqmodel.py
 groqflow/groqmodel/remote.py
 groqflow/justgroqit/__init__.py
 groqflow/justgroqit/assemble_multichip.py
 groqflow/justgroqit/compile.py
```

### Comparing `groqflow-2.5.2/setup.py` & `groqflow-3.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,31 +11,32 @@
     author="Groq",
     author_email="sales@groq.com",
     license="MIT",
     packages=find_packages(
         exclude=["*.__pycache__.*"],
     ),
     install_requires=[
-        "onnx==1.11.0",
+        "onnx>=1.11.0",
         "onnxmltools==1.10.0",
         "hummingbird-ml==0.4.4",
         "scikit-learn==1.1.1",
         "xgboost==1.6.1",
-        "onnxruntime==1.10.0",
+        "onnxruntime>=1.10.0",
         "paramiko==2.11.0",
         "torch>=1.12.1",
-        "protobuf==3.17.3",
-        "pyyaml==5.4",
-        "tensorflow-cpu>=2.9.1",
-        "tf2onnx>=1.12.0",
+        "protobuf>=3.17.3",
+        "pyyaml>=5.4",
         "typeguard>=2.3.13",
-        "packaging",
+        "packaging>=21.3",
     ],
+    extras_require={
+        "tensorflow": ["tensorflow-cpu>=2.8.1", "tf2onnx>=1.12.0"],
+    },
     classifiers=[],
     entry_points={
         "console_scripts": [
         ]
     },
-    python_requires="==3.8.*",
+    python_requires=">=3.8, <3.11",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
 )
```

