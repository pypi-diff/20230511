# Comparing `tmp/chronus-0.3.6.tar.gz` & `tmp/chronus-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chronus-0.3.6.tar", max compression
+gzip compressed data, was "chronus-0.3.7.tar", max compression
```

## Comparing `chronus-0.3.6.tar` & `chronus-0.3.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1072 2023-04-28 08:15:27.618142 chronus-0.3.6/LICENSE
--rw-r--r--   0        0        0    10584 2023-05-10 09:58:34.046336 chronus-0.3.6/README.md
--rw-r--r--   0        0        0        1 2023-04-28 08:15:27.622142 chronus-0.3.6/chronus/SystemIntegration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.6/chronus/SystemIntegration/application_runners/__init__.py
--rw-r--r--   0        0        0     6026 2023-05-06 16:21:47.233103 chronus-0.3.6/chronus/SystemIntegration/application_runners/hpcg.py
--rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.6/chronus/SystemIntegration/cpu_info_services/__init__.py
--rw-r--r--   0        0        0     2714 2023-05-10 09:48:21.426509 chronus-0.3.6/chronus/SystemIntegration/cpu_info_services/cpu_info_service.py
--rw-r--r--   0        0        0        0 2023-05-05 13:33:24.644402 chronus-0.3.6/chronus/SystemIntegration/optimizers/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/SystemIntegration/optimizers/bruteforce_optmizer.py
--rw-r--r--   0        0        0     3672 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/SystemIntegration/optimizers/linear_regression.py
--rw-r--r--   0        0        0     2924 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/SystemIntegration/optimizers/random_tree_forrest.py
--rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.6/chronus/SystemIntegration/repositories/__init__.py
--rw-r--r--   0        0        0     2559 2023-05-05 17:12:11.384766 chronus-0.3.6/chronus/SystemIntegration/repositories/csv_repository.py
--rw-r--r--   0        0        0    14565 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/SystemIntegration/repositories/sqlite_repository.py
--rw-r--r--   0        0        0        0 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/SystemIntegration/settings_interface/__init__.py
--rw-r--r--   0        0        0     1336 2023-05-10 11:09:21.787582 chronus-0.3.6/chronus/SystemIntegration/settings_interface/etc_storage.py
--rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.6/chronus/SystemIntegration/system_service_interfaces/__init__.py
--rw-r--r--   0        0        0     1776 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/SystemIntegration/system_service_interfaces/ipmi_system_service.py
--rw-r--r--   0        0        0      330 2023-04-28 08:15:27.622142 chronus-0.3.6/chronus/__init__.py
--rw-r--r--   0        0        0    11726 2023-05-10 10:06:00.337846 chronus-0.3.6/chronus/__main__.py
--rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.6/chronus/application/__init__.py
--rw-r--r--   0        0        0     3710 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/application/benchmark_service.py
--rw-r--r--   0        0        0     2437 2023-05-10 10:47:43.600083 chronus-0.3.6/chronus/application/init_model_service.py
--rw-r--r--   0        0        0     1531 2023-05-10 10:47:43.600083 chronus-0.3.6/chronus/application/load_model_service.py
--rw-r--r--   0        0        0      602 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/application/run_model_service.py
--rw-r--r--   0        0        0        0 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/cli/__init__.py
--rw-r--r--   0        0        0      742 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/cli/setup.py
--rw-r--r--   0        0        0      197 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/domain/LocalSettings.py
--rw-r--r--   0        0        0     2195 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/domain/Run.py
--rw-r--r--   0        0        0        0 2023-04-28 08:15:27.622142 chronus-0.3.6/chronus/domain/__init__.py
--rw-r--r--   0        0        0      461 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/domain/benchmark.py
--rw-r--r--   0        0        0     1181 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/domain/configuration.py
--rw-r--r--   0        0        0      523 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/domain/cpu_info.py
--rw-r--r--   0        0        0        0 2023-04-28 08:15:27.622142 chronus-0.3.6/chronus/domain/interfaces/__init__.py
--rw-r--r--   0        0        0      520 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/domain/interfaces/application_runner_interface.py
--rw-r--r--   0        0        0      158 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/domain/interfaces/cpu_info_service_interface.py
--rw-r--r--   0        0        0      918 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/domain/interfaces/optimizer_interface.py
--rw-r--r--   0        0        0      986 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/domain/interfaces/repository_interface.py
--rw-r--r--   0        0        0      499 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/domain/interfaces/settings_interface.py
--rw-r--r--   0        0        0      160 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/domain/interfaces/system_service_interface.py
--rw-r--r--   0        0        0      274 2023-05-10 10:33:20.168286 chronus-0.3.6/chronus/domain/model.py
--rw-r--r--   0        0        0      369 2023-05-10 09:48:21.430509 chronus-0.3.6/chronus/domain/system_sample.py
--rw-r--r--   0        0        0     3757 2023-05-10 11:09:37.087576 chronus-0.3.6/pyproject.toml
--rw-r--r--   0        0        0    11888 1970-01-01 00:00:00.000000 chronus-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-28 09:33:02.453690 chronus-0.3.7/LICENSE
+-rw-r--r--   0        0        0    10584 2023-05-10 22:28:32.413515 chronus-0.3.7/README.md
+-rw-r--r--   0        0        0        1 2023-04-17 10:44:37.558827 chronus-0.3.7/chronus/SystemIntegration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:32:38.744446 chronus-0.3.7/chronus/SystemIntegration/application_runners/__init__.py
+-rw-r--r--   0        0        0     6026 2023-05-09 18:12:52.822503 chronus-0.3.7/chronus/SystemIntegration/application_runners/hpcg.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:32:38.745392 chronus-0.3.7/chronus/SystemIntegration/cpu_info_services/__init__.py
+-rw-r--r--   0        0        0     2714 2023-05-09 18:12:52.823004 chronus-0.3.7/chronus/SystemIntegration/cpu_info_services/cpu_info_service.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:32:38.746076 chronus-0.3.7/chronus/SystemIntegration/optimizers/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-09 18:12:52.823479 chronus-0.3.7/chronus/SystemIntegration/optimizers/bruteforce_optmizer.py
+-rw-r--r--   0        0        0     3672 2023-05-09 18:12:52.823972 chronus-0.3.7/chronus/SystemIntegration/optimizers/linear_regression.py
+-rw-r--r--   0        0        0     2924 2023-05-09 18:12:52.824428 chronus-0.3.7/chronus/SystemIntegration/optimizers/random_tree_forrest.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:32:38.747440 chronus-0.3.7/chronus/SystemIntegration/repositories/__init__.py
+-rw-r--r--   0        0        0     2559 2023-05-09 18:12:52.824856 chronus-0.3.7/chronus/SystemIntegration/repositories/csv_repository.py
+-rw-r--r--   0        0        0    14565 2023-05-09 18:12:52.825422 chronus-0.3.7/chronus/SystemIntegration/repositories/sqlite_repository.py
+-rw-r--r--   0        0        0        0 2023-05-09 18:12:52.825786 chronus-0.3.7/chronus/SystemIntegration/settings_interface/__init__.py
+-rw-r--r--   0        0        0     1336 2023-05-10 22:28:32.414909 chronus-0.3.7/chronus/SystemIntegration/settings_interface/etc_storage.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:32:38.748509 chronus-0.3.7/chronus/SystemIntegration/system_service_interfaces/__init__.py
+-rw-r--r--   0        0        0     1776 2023-05-09 18:12:52.826886 chronus-0.3.7/chronus/SystemIntegration/system_service_interfaces/ipmi_system_service.py
+-rw-r--r--   0        0        0      330 2023-04-17 10:14:26.979910 chronus-0.3.7/chronus/__init__.py
+-rw-r--r--   0        0        0    11863 2023-05-10 22:29:56.935967 chronus-0.3.7/chronus/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:32:38.751240 chronus-0.3.7/chronus/application/__init__.py
+-rw-r--r--   0        0        0     3710 2023-05-09 18:12:52.829093 chronus-0.3.7/chronus/application/benchmark_service.py
+-rw-r--r--   0        0        0     2437 2023-05-10 22:28:32.417384 chronus-0.3.7/chronus/application/init_model_service.py
+-rw-r--r--   0        0        0     1531 2023-05-10 22:28:32.434971 chronus-0.3.7/chronus/application/load_model_service.py
+-rw-r--r--   0        0        0      602 2023-05-09 18:12:52.830000 chronus-0.3.7/chronus/application/run_model_service.py
+-rw-r--r--   0        0        0        0 2023-05-09 18:12:52.831125 chronus-0.3.7/chronus/cli/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-09 18:12:52.831474 chronus-0.3.7/chronus/cli/setup.py
+-rw-r--r--   0        0        0      197 2023-05-09 18:12:52.831885 chronus-0.3.7/chronus/domain/LocalSettings.py
+-rw-r--r--   0        0        0     2195 2023-05-09 18:12:52.832474 chronus-0.3.7/chronus/domain/Run.py
+-rw-r--r--   0        0        0        0 2023-04-17 10:14:26.980936 chronus-0.3.7/chronus/domain/__init__.py
+-rw-r--r--   0        0        0      461 2023-05-09 18:12:52.833265 chronus-0.3.7/chronus/domain/benchmark.py
+-rw-r--r--   0        0        0     1181 2023-05-09 18:12:52.833778 chronus-0.3.7/chronus/domain/configuration.py
+-rw-r--r--   0        0        0      523 2023-05-09 18:12:52.834308 chronus-0.3.7/chronus/domain/cpu_info.py
+-rw-r--r--   0        0        0        0 2023-04-23 12:44:06.746442 chronus-0.3.7/chronus/domain/interfaces/__init__.py
+-rw-r--r--   0        0        0      520 2023-05-09 18:12:52.835812 chronus-0.3.7/chronus/domain/interfaces/application_runner_interface.py
+-rw-r--r--   0        0        0      158 2023-05-09 18:12:52.836343 chronus-0.3.7/chronus/domain/interfaces/cpu_info_service_interface.py
+-rw-r--r--   0        0        0      918 2023-05-09 18:12:52.836840 chronus-0.3.7/chronus/domain/interfaces/optimizer_interface.py
+-rw-r--r--   0        0        0      986 2023-05-09 18:12:52.837275 chronus-0.3.7/chronus/domain/interfaces/repository_interface.py
+-rw-r--r--   0        0        0      499 2023-05-09 18:12:52.837640 chronus-0.3.7/chronus/domain/interfaces/settings_interface.py
+-rw-r--r--   0        0        0      160 2023-05-09 18:12:52.838125 chronus-0.3.7/chronus/domain/interfaces/system_service_interface.py
+-rw-r--r--   0        0        0      274 2023-05-09 18:12:52.838563 chronus-0.3.7/chronus/domain/model.py
+-rw-r--r--   0        0        0      369 2023-05-09 18:12:52.839123 chronus-0.3.7/chronus/domain/system_sample.py
+-rw-r--r--   0        0        0     3757 2023-05-10 22:30:35.407039 chronus-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0    11888 1970-01-01 00:00:00.000000 chronus-0.3.7/PKG-INFO
```

### Comparing `chronus-0.3.6/LICENSE` & `chronus-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/README.md` & `chronus-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/SystemIntegration/application_runners/hpcg.py` & `chronus-0.3.7/chronus/SystemIntegration/application_runners/hpcg.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/SystemIntegration/cpu_info_services/cpu_info_service.py` & `chronus-0.3.7/chronus/SystemIntegration/cpu_info_services/cpu_info_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/SystemIntegration/optimizers/bruteforce_optmizer.py` & `chronus-0.3.7/chronus/SystemIntegration/optimizers/bruteforce_optmizer.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/SystemIntegration/optimizers/linear_regression.py` & `chronus-0.3.7/chronus/SystemIntegration/optimizers/linear_regression.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/SystemIntegration/optimizers/random_tree_forrest.py` & `chronus-0.3.7/chronus/SystemIntegration/optimizers/random_tree_forrest.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/SystemIntegration/repositories/csv_repository.py` & `chronus-0.3.7/chronus/SystemIntegration/repositories/csv_repository.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/SystemIntegration/repositories/sqlite_repository.py` & `chronus-0.3.7/chronus/SystemIntegration/repositories/sqlite_repository.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/SystemIntegration/settings_interface/etc_storage.py` & `chronus-0.3.7/chronus/SystemIntegration/settings_interface/etc_storage.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/SystemIntegration/system_service_interfaces/ipmi_system_service.py` & `chronus-0.3.7/chronus/SystemIntegration/system_service_interfaces/ipmi_system_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/__main__.py` & `chronus-0.3.7/chronus/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,32 +236,37 @@
 
 
 @dataclasses.dataclass
 class ConfigDto:
     cores: int
     frequency: int
     threads_per_core: int
-    disable_plug: bool
 
 
 @app.command(name="slurm-config")
 def get_config(cpu: str = typer.Argument(..., help="The cpu model to get the config for")):
     local_storage = EtcLocalStorage(Permission.READ)
     optimizer_type = local_storage.get_settings().loaded_model.type
     run_model = RunModelService(
         optimizer=_choose_optimizer(optimizer_type), local_storage=local_storage
     )
     conf = run_model.run()
-
-    outgoing = ConfigDto(
-        cores=conf.cores,
-        frequency=conf.frequency,
-        threads_per_core=conf.threads_per_core,
-        disable_plug=True,
-    )
+    disabled = True
+    if disabled:
+        outgoing = ConfigDto(
+            cores=-1,
+            frequency=-1,
+            threads_per_core=-1,
+        )
+    else:
+        outgoing = ConfigDto(
+            cores=conf.cores,
+            frequency=conf.frequency,
+            threads_per_core=conf.threads_per_core,
+        )
     console.print(json.dumps(dataclasses.asdict(outgoing)))
 
 
 # add partician compute
 
 
 @app.command(name="run")
```

### Comparing `chronus-0.3.6/chronus/application/benchmark_service.py` & `chronus-0.3.7/chronus/application/benchmark_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/application/init_model_service.py` & `chronus-0.3.7/chronus/application/init_model_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/application/load_model_service.py` & `chronus-0.3.7/chronus/application/load_model_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/application/run_model_service.py` & `chronus-0.3.7/chronus/application/run_model_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/cli/setup.py` & `chronus-0.3.7/chronus/cli/setup.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/domain/Run.py` & `chronus-0.3.7/chronus/domain/Run.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/domain/configuration.py` & `chronus-0.3.7/chronus/domain/configuration.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/domain/cpu_info.py` & `chronus-0.3.7/chronus/domain/cpu_info.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/domain/interfaces/application_runner_interface.py` & `chronus-0.3.7/chronus/domain/interfaces/application_runner_interface.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/domain/interfaces/optimizer_interface.py` & `chronus-0.3.7/chronus/domain/interfaces/optimizer_interface.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/chronus/domain/interfaces/repository_interface.py` & `chronus-0.3.7/chronus/domain/interfaces/repository_interface.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.6/pyproject.toml` & `chronus-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "chronus"
-version = "0.3.6"
+version = "0.3.7"
 description = "A energy scheduling model, build for HPC."
 readme = "README.md"
 authors = ["chronus <aaspringborg@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/AndersSpringborg/chronus"
 homepage = "https://github.com/AndersSpringborg/chronus"
```

### Comparing `chronus-0.3.6/PKG-INFO` & `chronus-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chronus
-Version: 0.3.6
+Version: 0.3.7
 Summary: A energy scheduling model, build for HPC.
 Home-page: https://github.com/AndersSpringborg/chronus
 License: MIT
 Author: chronus
 Author-email: aaspringborg@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

