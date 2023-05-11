# Comparing `tmp/chainbench-0.1.2.tar.gz` & `tmp/chainbench-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainbench-0.1.2.tar", max compression
+gzip compressed data, was "chainbench-0.2.0.tar", max compression
```

## Comparing `chainbench-0.1.2.tar` & `chainbench-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-05-04 10:39:14.437426 chainbench-0.1.2/LICENSE
--rw-r--r--   0        0        0     6162 2023-05-04 10:39:14.437426 chainbench-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/__init__.py
--rw-r--r--   0        0        0       39 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/__main__.py
--rw-r--r--   0        0        0     5241 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/main.py
--rw-r--r--   0        0        0        0 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/profile/__init__.py
--rw-r--r--   0        0        0     3417 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/profile/avalanche.py
--rw-r--r--   0        0        0     2512 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/profile/bsc.py
--rw-r--r--   0        0        0     2794 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/profile/ethereum.py
--rw-r--r--   0        0        0     1829 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/profile/oasis.py
--rw-r--r--   0        0        0     2730 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/profile/polygon.py
--rw-r--r--   0        0        0      168 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/test_data/__init__.py
--rw-r--r--   0        0        0     4705 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/test_data/base.py
--rw-r--r--   0        0        0      166 2023-05-04 10:39:14.437426 chainbench-0.1.2/chainbench/test_data/dummy.py
--rw-r--r--   0        0        0     2596 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/test_data/evm.py
--rw-r--r--   0        0        0        0 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/user/__init__.py
--rw-r--r--   0        0        0     3438 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/user/base.py
--rw-r--r--   0        0        0     1225 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/user/evm.py
--rw-r--r--   0        0        0        0 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/util/__init__.py
--rw-r--r--   0        0        0     2499 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/util/cli.py
--rw-r--r--   0        0        0     2532 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/util/event.py
--rw-r--r--   0        0        0     3463 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/util/notify.py
--rw-r--r--   0        0        0      320 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/util/rpc.py
--rw-r--r--   0        0        0      438 2023-05-04 10:39:14.441426 chainbench-0.1.2/chainbench/util/timer.py
--rw-r--r--   0        0        0      746 2023-05-04 10:39:14.441426 chainbench-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6628 1970-01-01 00:00:00.000000 chainbench-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-11 11:14:19.492029 chainbench-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7622 2023-05-11 11:14:19.496029 chainbench-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/__init__.py
+-rw-r--r--   0        0        0       39 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/__main__.py
+-rw-r--r--   0        0        0     5735 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/main.py
+-rw-r--r--   0        0        0        0 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/profile/__init__.py
+-rw-r--r--   0        0        0     3417 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/profile/avalanche.py
+-rw-r--r--   0        0        0     2512 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/profile/bsc.py
+-rw-r--r--   0        0        0     2734 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/profile/ethereum.py
+-rw-r--r--   0        0        0      723 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/profile/evm/heavy.py
+-rw-r--r--   0        0        0     1592 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/profile/evm/light.py
+-rw-r--r--   0        0        0     1829 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/profile/oasis.py
+-rw-r--r--   0        0        0     2670 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/profile/polygon.py
+-rw-r--r--   0        0        0      168 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/test_data/__init__.py
+-rw-r--r--   0        0        0     4705 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/test_data/base.py
+-rw-r--r--   0        0        0      166 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/test_data/dummy.py
+-rw-r--r--   0        0        0     2596 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/test_data/evm.py
+-rw-r--r--   0        0        0        0 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/user/__init__.py
+-rw-r--r--   0        0        0     3410 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/user/base.py
+-rw-r--r--   0        0        0     1225 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/user/evm.py
+-rw-r--r--   0        0        0        0 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/util/__init__.py
+-rw-r--r--   0        0        0     3015 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/util/cli.py
+-rw-r--r--   0        0        0     2512 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/util/event.py
+-rw-r--r--   0        0        0     3463 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/util/notify.py
+-rw-r--r--   0        0        0      320 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/util/rpc.py
+-rw-r--r--   0        0        0      438 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/util/timer.py
+-rw-r--r--   0        0        0      746 2023-05-11 11:14:19.496029 chainbench-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8088 1970-01-01 00:00:00.000000 chainbench-0.2.0/PKG-INFO
```

### Comparing `chainbench-0.1.2/LICENSE` & `chainbench-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.2/README.md` & `chainbench-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -99,16 +99,40 @@
 - `--workers`: This flag sets the number of worker threads to use for the benchmark.
 - `--test-time`: This flag sets the duration of the test to run.
 - `--target`: This flag specifies the target blockchain node URL that the benchmark will connect to.
 - `--headless`: This flag runs the benchmark in headless mode, meaning that no graphical user interface (GUI) will be displayed during the test. This is useful for running the test on a remote server or when the GUI is not needed.
 - `--autoquit`: This flag tells the Chainbench tool to automatically quit after the test has finished. This is useful for running the benchmark in an automated environment where manual intervention is not desired.
 - `--help`: This flag displays the help message.
 
+By default, Chainbench uses `constant_pacing` wait time with a value of 10 seconds. 
+This means a load test with 100 users will have a theoretical maximum of 10 rps. This allows us to have a target rps in a test, 
+and the result rps lower than the target rps means performance deterioration.
+
 ### Profiles
-Profiles are located in the [`profile`](chainbench/profile) directory. For a tutorial on how to create custom profiles, please refer to [this document](docs/PROFILE.md).
+Default profiles are located in the [`profile`](chainbench/profile) directory. For a tutorial on how to create custom profiles, please refer to [this document](docs/PROFILE.md).
+
+You can also use the `--profile-dir` flag to specify a custom directory with profiles. For example:
+```shell
+chainbench start --profile-dir /path/to/profiles --profile my-profile --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
+```
+This will run a load test using `/path/to/profiles/my-profile.py` profile.
+
+It's possible to group profiles into directories. For example, you can create a directory called `bsc` and put all the BSC profiles there. Then you can run a load test using the following command:
+```shell
+chainbench start --profile-dir /path/to/profiles --profile bsc.my-profile --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
+```
+
+Chainbench will look for the profile in `/path/to/profiles/bsc/my-profile.py`. Currently, only one level of nesting is supported.
+
+There are built-in `evm.light` and `evm.heavy` profiles for EVM-compatible chains.
+
+Here's an example of how to run a load test for Ethereum using the `evm.light` profile:
+```shell
+chainbench start --profile evm.light --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
+```
 
 ### Web UI Mode
 
 Run the following command to run a load test for BSC in UI mode. It will start a web server on port 8089. 
 Target is not required as you can specify it in the UI along with the number of users, spawn rate and test time.
 
 ```shell
```

### Comparing `chainbench-0.1.2/chainbench/main.py` & `chainbench-0.2.0/chainbench/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import logging
+import os
 import shlex
 import subprocess
 import sys
 from pathlib import Path
 
 import click
 
 from chainbench.util.cli import (
     ContextData,
     ensure_results_dir,
+    get_base_path,
     get_master_command,
     get_profile_path,
     get_worker_command,
 )
 from chainbench.util.notify import NoopNotifier, Notifier
 
 # Default values for arguments
@@ -44,14 +46,17 @@
 )
 @click.option(
     "--profile",
     default=DEFAULT_PROFILE,
     help="Profile to run",
     show_default=True,
 )
+@click.option(
+    "--profile-dir", default=None, type=click.Path(), help="Profile directory"
+)
 @click.option("--host", default=MASTER_HOST, help="Host to run on", show_default=True)
 @click.option("--port", default=MASTER_PORT, help="Port to run on", show_default=True)
 @click.option(
     "--workers",
     default=WORKER_COUNT,
     help="Number of workers to run",
     show_default=True,
@@ -72,14 +77,15 @@
 @click.option("--target", default=None, help="Endpoint to test")
 @click.option("--run-id", default=None, help="ID of the test")
 @click.option("--notify", default=None, help="Notify when test is finished")
 @click.pass_context
 def start(
     ctx: click.Context,
     profile: str,
+    profile_dir: Path | None,
     host: str,
     port: int,
     workers: int,
     test_time: str,
     users: int,
     spawn_rate: int,
     log_level: str,
@@ -98,15 +104,18 @@
 
     ctx.obj.notifier = notifier
 
     if headless and target is None:
         click.echo("Target is required when running in headless mode")
         sys.exit(1)
 
-    profile_path = get_profile_path(profile, __file__)
+    if not profile_dir:
+        profile_dir = get_base_path(__file__)
+
+    profile_path = get_profile_path(profile_dir, profile)
 
     if not profile_path.exists():
         click.echo(f"Profile file {profile_path} does not exist")
         sys.exit(1)
 
     results_dir = Path(results_dir).resolve()
 
@@ -127,54 +136,62 @@
         users=users,
         spawn_rate=spawn_rate,
         log_level=log_level,
         results_path=results_path,
         workers=workers,
         headless=headless,
         target=target,
+        # TODO: Add support for tags in the CLI
+        exclude_tags=["trace", "debug"],
     )
     if headless:
         click.echo(f"Starting master in headless mode for {profile}")
     else:
         click.echo(f"Starting master for {profile}")
-    master_args = shlex.split(master_command)
+
+    is_posix = os.name == "posix"
+
+    master_args = shlex.split(master_command, posix=is_posix)
     master_process = subprocess.Popen(master_args)
     ctx.obj.master = master_process
     # Start the Locust workers
     for worker_id in range(workers):
         worker_command = get_worker_command(
             profile_path=profile_path,
             host=host,
             port=port,
             results_path=results_path,
             headless=headless,
             target=target,
             worker_id=worker_id,
             log_level=log_level,
+            # TODO: Add support for tags in the CLI
+            exclude_tags=["trace", "debug"],
         )
-        worker_args = shlex.split(worker_command)
+        worker_args = shlex.split(worker_command, posix=is_posix)
         worker_process = subprocess.Popen(worker_args)
         ctx.obj.workers.append(worker_process)
         click.echo(f"Starting worker {worker_id + 1} for {profile}")
-        # Print out the URL to access the test
     if headless:
         click.echo(f"Running test in headless mode for {profile}")
         ctx.obj.notifier.notify(
             title="Test started",
             message=f"Running test in headless mode for {profile}",
             tags=["loudspeaker"],
         )
     else:
+        # Print out the URL to access the test
         click.echo(f"Run test: http://127.0.0.1:8089 {profile}")
 
     for process in ctx.obj.workers:
         process.wait()
 
     if autoquit:
-        click.echo("Quitting when test is finished")
+        ctx.obj.master.wait()
+        click.echo("Quitting...")
         ctx.obj.master.terminate()
 
     ctx.obj.notifier.notify(
         title="Test finished", message=f"Test finished for {profile}", tags=["tada"]
     )
```

### Comparing `chainbench-0.1.2/chainbench/profile/avalanche.py` & `chainbench-0.2.0/chainbench/profile/avalanche.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.2/chainbench/profile/bsc.py` & `chainbench-0.2.0/chainbench/profile/bsc.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.2/chainbench/profile/ethereum.py` & `chainbench-0.2.0/chainbench/profile/ethereum.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "eth_getBalance" : 12
     "eth_chainId" : 11
     "eth_getBlockByNumber" : 9
     "eth_getTransactionByHash" : 8
     "Others" : 12
 ```
 """
-from locust import task
+from locust import tag, task
 
 from chainbench.user.evm import EVMBenchUser
 
 
 class EthereumProfile(EVMBenchUser):
     @task(100)
     def call_task(self):
@@ -87,16 +87,16 @@
     def get_logs_task(self):
         self.make_call(
             name="get_logs",
             method="eth_getLogs",
             params=self._get_logs_params_factory(),
         ),
 
-    # TODO: introduce tags to make it possible to filter out unsupported methods
-    # @task(3)
+    @tag("debug")
+    @task(3)
     def trace_transaction_task(self):
         self.make_call(
             name="trace_transaction",
             method="debug_traceTransaction",
             params=[],
         ),
```

### Comparing `chainbench-0.1.2/chainbench/profile/oasis.py` & `chainbench-0.2.0/chainbench/profile/oasis.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.2/chainbench/profile/polygon.py` & `chainbench-0.2.0/chainbench/profile/polygon.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "eth_getBlockByNumber" : 17
     "eth_blockNumber" : 16
     "eth_getTransactionByHash" : 11
     "eth_getLogs" : 11
     "Others" : 9
 ```
 """
-from locust import task
+from locust import tag, task
 
 from chainbench.user.evm import EVMBenchUser
 
 
 class PolygonProfile(EVMBenchUser):
     @task(100)
     def call_task(self):
@@ -90,15 +90,15 @@
     def get_balance_task(self):
         self.make_call(
             name="get_balance",
             method="eth_getBalance",
             params=self._get_balance_params_factory_latest(),
         ),
 
-    # TODO: introduce tags to make it possible to filter out unsupported methods
-    # @task(2)
+    @tag("trace")
+    @task(2)
     def block_task(self):
         self.make_call(
             name="block",
             method="trace_block",
             params=self._block_by_number_params_factory(),
         ),
```

### Comparing `chainbench-0.1.2/chainbench/test_data/base.py` & `chainbench-0.2.0/chainbench/test_data/base.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.2/chainbench/test_data/evm.py` & `chainbench-0.2.0/chainbench/test_data/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.2/chainbench/user/base.py` & `chainbench-0.2.0/chainbench/user/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,23 +32,23 @@
         self.test_data.wait()
 
     def on_stop(self):
         self.test_data.close()
 
     def check_fatal(self, response: RestResponseContextManager):
         if response.status_code == 401:
-            self.logger.critical(f"⛔️ Unauthorized request to {response.url}")
+            self.logger.critical(f"Unauthorized request to {response.url}")
         elif response.status_code == 404:
-            self.logger.critical(f"⛔️ Not found: {response.url}")
+            self.logger.critical(f"Not found: {response.url}")
         elif 500 <= response.status_code <= 599:
             self.logger.critical(
-                f"⛔️ Got internal server error when requesting {response.url}"
+                f"Got internal server error when requesting {response.url}"
             )
         elif 300 <= response.status_code <= 399:
-            self.logger.critical(f"⛔️ Redirect error: {response.url}")
+            self.logger.critical(f"Redirect error: {response.url}")
 
     def check_response(self, response: RestResponseContextManager):
         """Check the response for errors."""
         if response.status_code != 200:
             self.logger.info(f"Request failed with {response.status_code} code")
             self.logger.debug(
                 f"Request to {response.url} failed with {response.status_code} code: {response.text}"  # noqa: E501
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `chainbench-0.1.2/chainbench/user/evm.py` & `chainbench-0.2.0/chainbench/user/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.2/chainbench/util/event.py` & `chainbench-0.2.0/chainbench/util/event.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,38 +28,38 @@
 # Listener for the test stop event
 def on_test_stop(environment, **_kwargs):
     # It will be called for any runner (master, worker, local)
     runner = environment.runner
     if not isinstance(runner, MasterRunner):
         # Print worker details to the log
         logger.info(
-            f"🏁 Worker[{runner.worker_index:02d}]: Tests completed in "
+            f"Worker[{runner.worker_index:02d}]: Tests completed in "
             f"{Timer.get_time_diff(runner.worker_index):>.3f} seconds"
         )
     else:
         # Print master details to the log
-        logger.info("🏁 Master: The test is stopped")
+        logger.info("Master: The test is stopped")
 
 
 # Listener for the init event
 def on_init(environment, **_kwargs):
     # It will be called for any runner (master, worker, local)
     logger.debug("init.add_listener: Init is started")
     logger.debug("init.add_listener: Environment: %s", environment.runner)
     logger.debug("init.add_listener: Host: %s", environment.host)
 
     host_under_test = environment.host or "Default host"
 
     if isinstance(environment.runner, MasterRunner):
         # Print master details to the log
-        logger.info("🤖 I'm a master. Running tests for %s", host_under_test)
+        logger.info("I'm a master. Running tests for %s", host_under_test)
 
     if isinstance(environment.runner, WorkerRunner):
         # Print worker details to the log
-        logger.info("🤖 I'm a worker. Running tests for %s", host_under_test)
+        logger.info("I'm a worker. Running tests for %s", host_under_test)
         logger.info("Initializing test data...")
         for user in environment.runner.user_classes:
             if not hasattr(user, "test_data"):
                 continue
 
             user.test_data.update(environment.host)
             logger.info("Test data is ready")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `chainbench-0.1.2/chainbench/util/notify.py` & `chainbench-0.2.0/chainbench/util/notify.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.2/pyproject.toml` & `chainbench-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainbench"
-version = "0.1.2"
+version = "0.2.0"
 description = ""
 authors = ["Egor Molodik <egor.molodik@chainstack.com>"]
 readme = "README.md"
 packages = [{include = "chainbench"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `chainbench-0.1.2/PKG-INFO` & `chainbench-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainbench
-Version: 0.1.2
+Version: 0.2.0
 Summary: 
 Author: Egor Molodik
 Author-email: egor.molodik@chainstack.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -114,16 +114,40 @@
 - `--workers`: This flag sets the number of worker threads to use for the benchmark.
 - `--test-time`: This flag sets the duration of the test to run.
 - `--target`: This flag specifies the target blockchain node URL that the benchmark will connect to.
 - `--headless`: This flag runs the benchmark in headless mode, meaning that no graphical user interface (GUI) will be displayed during the test. This is useful for running the test on a remote server or when the GUI is not needed.
 - `--autoquit`: This flag tells the Chainbench tool to automatically quit after the test has finished. This is useful for running the benchmark in an automated environment where manual intervention is not desired.
 - `--help`: This flag displays the help message.
 
+By default, Chainbench uses `constant_pacing` wait time with a value of 10 seconds. 
+This means a load test with 100 users will have a theoretical maximum of 10 rps. This allows us to have a target rps in a test, 
+and the result rps lower than the target rps means performance deterioration.
+
 ### Profiles
-Profiles are located in the [`profile`](chainbench/profile) directory. For a tutorial on how to create custom profiles, please refer to [this document](docs/PROFILE.md).
+Default profiles are located in the [`profile`](chainbench/profile) directory. For a tutorial on how to create custom profiles, please refer to [this document](docs/PROFILE.md).
+
+You can also use the `--profile-dir` flag to specify a custom directory with profiles. For example:
+```shell
+chainbench start --profile-dir /path/to/profiles --profile my-profile --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
+```
+This will run a load test using `/path/to/profiles/my-profile.py` profile.
+
+It's possible to group profiles into directories. For example, you can create a directory called `bsc` and put all the BSC profiles there. Then you can run a load test using the following command:
+```shell
+chainbench start --profile-dir /path/to/profiles --profile bsc.my-profile --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
+```
+
+Chainbench will look for the profile in `/path/to/profiles/bsc/my-profile.py`. Currently, only one level of nesting is supported.
+
+There are built-in `evm.light` and `evm.heavy` profiles for EVM-compatible chains.
+
+Here's an example of how to run a load test for Ethereum using the `evm.light` profile:
+```shell
+chainbench start --profile evm.light --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
+```
 
 ### Web UI Mode
 
 Run the following command to run a load test for BSC in UI mode. It will start a web server on port 8089. 
 Target is not required as you can specify it in the UI along with the number of users, spawn rate and test time.
 
 ```shell
```

