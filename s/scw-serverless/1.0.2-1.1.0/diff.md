# Comparing `tmp/scw_serverless-1.0.2.tar.gz` & `tmp/scw_serverless-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scw_serverless-1.0.2.tar", max compression
+gzip compressed data, was "scw_serverless-1.1.0.tar", max compression
```

## Comparing `scw_serverless-1.0.2.tar` & `scw_serverless-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,29 @@
--rw-r--r--   0        0        0      617 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     1065 2023-05-04 12:54:46.772897 scw_serverless-1.0.2/LICENSE
--rw-r--r--   0        0        0     2673 2023-05-04 12:54:46.772897 scw_serverless-1.0.2/README.md
--rw-r--r--   0        0        0     2981 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       54 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/scw_serverless/__init__.py
--rw-r--r--   0        0        0     5001 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/scw_serverless/app.py
--rw-r--r--   0        0        0     6100 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/scw_serverless/cli.py
--rw-r--r--   0        0        0       31 2023-05-04 12:54:46.776897 scw_serverless-1.0.2/scw_serverless/config/__init__.py
--rw-r--r--   0        0        0     5109 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/scw_serverless/config/function.py
--rw-r--r--   0        0        0      138 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/scw_serverless/config/generators/__init__.py
--rw-r--r--   0        0        0      219 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/scw_serverless/config/generators/generator.py
--rw-r--r--   0        0        0     4169 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/scw_serverless/config/generators/serverless_framework.py
--rw-r--r--   0        0        0     7045 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/scw_serverless/config/generators/terraform.py
--rw-r--r--   0        0        0     1247 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/config/route.py
--rw-r--r--   0        0        0       14 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/config/templates/.gitignore
--rw-r--r--   0        0        0      414 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/config/templates/serverless.yml
--rw-r--r--   0        0        0      426 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/config/templates/terraform.tf.json
--rw-r--r--   0        0        0      327 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/config/utils.py
--rw-r--r--   0        0        0     3532 2023-05-05 15:21:28.107228 scw_serverless-1.0.2/scw_serverless/dependencies_manager.py
--rw-r--r--   0        0        0        0 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/deploy/__init__.py
--rw-r--r--   0        0        0      172 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/deploy/backends/__init__.py
--rw-r--r--   0        0        0    11072 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/deploy/backends/scaleway_api_backend.py
--rw-r--r--   0        0        0      524 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/deploy/backends/serverless_backend.py
--rw-r--r--   0        0        0     1700 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/deploy/backends/serverless_framework_backend.py
--rw-r--r--   0        0        0        0 2023-05-04 12:54:46.776897 scw_serverless-1.0.2/scw_serverless/gateway/__init__.py
--rw-r--r--   0        0        0     1359 2023-05-04 12:54:46.776897 scw_serverless-1.0.2/scw_serverless/gateway/gateway_api_client.py
--rw-r--r--   0        0        0     2341 2023-05-04 12:54:46.776897 scw_serverless-1.0.2/scw_serverless/gateway/gateway_manager.py
--rw-r--r--   0        0        0     2262 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/logger.py
--rw-r--r--   0        0        0      137 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/triggers/__init__.py
--rw-r--r--   0        0        0     1405 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/triggers/cron.py
--rw-r--r--   0        0        0        0 2023-05-04 12:54:46.776897 scw_serverless-1.0.2/scw_serverless/utils/__init__.py
--rw-r--r--   0        0        0      239 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/utils/commands.py
--rw-r--r--   0        0        0     1864 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/utils/credentials.py
--rw-r--r--   0        0        0      590 2023-05-04 12:54:46.776897 scw_serverless-1.0.2/scw_serverless/utils/files.py
--rw-r--r--   0        0        0     1476 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/utils/loader.py
--rw-r--r--   0        0        0      761 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/utils/string.py
--rw-r--r--   0        0        0     4086 1970-01-01 00:00:00.000000 scw_serverless-1.0.2/setup.py
--rw-r--r--   0        0        0     4219 1970-01-01 00:00:00.000000 scw_serverless-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1181 2023-05-11 13:07:19.008204 scw_serverless-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1065 2023-05-11 13:07:19.008204 scw_serverless-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3154 2023-05-11 13:07:19.008204 scw_serverless-1.1.0/README.md
+-rw-r--r--   0        0        0     3038 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/__init__.py
+-rw-r--r--   0        0        0     5081 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/app.py
+-rw-r--r--   0        0        0     4889 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/cli.py
+-rw-r--r--   0        0        0       31 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/config/__init__.py
+-rw-r--r--   0        0        0     3831 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/config/function.py
+-rw-r--r--   0        0        0     1320 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/config/route.py
+-rw-r--r--   0        0        0     1405 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/config/triggers.py
+-rw-r--r--   0        0        0     3684 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/dependencies_manager.py
+-rw-r--r--   0        0        0      261 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/deployment/__init__.py
+-rw-r--r--   0        0        0     7144 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/deployment/api_wrapper.py
+-rw-r--r--   0        0        0     1829 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/deployment/client.py
+-rw-r--r--   0        0        0     8237 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/deployment/deployment_manager.py
+-rw-r--r--   0        0        0      434 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/deployment/exceptions.py
+-rw-r--r--   0        0        0      564 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/deployment/runtime.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/gateway/__init__.py
+-rw-r--r--   0        0        0     1359 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/gateway/gateway_api_client.py
+-rw-r--r--   0        0        0     2341 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/gateway/gateway_manager.py
+-rw-r--r--   0        0        0     1573 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/loader.py
+-rw-r--r--   0        0        0     1384 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/local_app.py
+-rw-r--r--   0        0        0      430 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/logger.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/utils/__init__.py
+-rw-r--r--   0        0        0      590 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/utils/files.py
+-rw-r--r--   0        0        0      427 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/utils/string.py
+-rw-r--r--   0        0        0     4466 1970-01-01 00:00:00.000000 scw_serverless-1.1.0/setup.py
+-rw-r--r--   0        0        0     4724 1970-01-01 00:00:00.000000 scw_serverless-1.1.0/PKG-INFO
```

### Comparing `scw_serverless-1.0.2/LICENSE` & `scw_serverless-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.2/README.md` & `scw_serverless-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,28 @@
 def hello_world(event, context):
     return requests.get(API_URL)
 ```
 
 The configuration is done by passing arguments to the decorator.
 To view which arguments are supported, head over to this [documentation](https://serverless-api-framework-python.readthedocs.io/) page.
 
+### Local testing
+
+Before deploying, you can run your functions locally with the dev command:
+
+```console
+scw-serverless dev app.py
+```
+
+This runs a local Flask server with your Serverless handlers. If no `relative_url` is defined for a function, it will be served on `/name` with `name` being the name of your Python function.
+
+By default, this runs Flask in debug mode which includes hot-reloading. You can disable this behavior by passing the `--no-debug` flag.
+
+### Deploying
+
 When you are ready, you can deploy your function with the `scw-serverless` CLI tool:
 
 ```console
 scw-serverless deploy app.py
 ```
 
 The tool will use your Scaleway credentials from your environment and config file.
```

### Comparing `scw_serverless-1.0.2/pyproject.toml` & `scw_serverless-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scw-serverless"
-version = "1.0.2"
+version = "1.1.0"
 description = "Framework for writing serverless APIs in Python, using Scaleway functions and containers."
 authors = ["Scaleway Serverless Team <opensource@scaleway.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/scaleway/serverless-api-framework-python-python"
 documentation = "https://serverless-api-project.readthedocs.io/en/latest/"
 keywords = ["serverless", "scaleway", "functions", "cloud", "faas"]
@@ -23,39 +23,35 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 packages = [{ include = "scw_serverless" }]
-include = [
-    "scw_serverless/**/*.yaml",
-    "scw_serverless/**/*.json",
-    "CHANGELOG.md",
-]
+include = ["CHANGELOG.md"]
 
 [tool.poetry.scripts]
-scw-serverless = "scw_serverless.cli:main"
+scw-serverless = "scw_serverless.cli:cli"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.9,<3.12"
 click = "^8.1.3"
-scaleway = ">=0.7,<0.12"
+scaleway = ">=0.7,<0.13"
+scaleway-functions-python = "^0.2.0"
 requests = "^2.28.2"
 typing-extensions = { version = "^4.4.0", python = "<3.11" }
-pyyaml = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=2.21,<4.0"
 pytest = "^7.2.0"
 pytest-xdist = "^3.1.0"
 pylint = "^2.15.10"
 pylint-per-file-ignores = "^1.1.0"
 responses = ">=0.22,<0.24"
-boto3 = "^1.26.97"
+boto3 = "^1.26.130"
 
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
 myst_parser = "^1.0.0"
 sphinx = "^6.1.0"
@@ -74,14 +70,16 @@
 max-line-length = 89
 # Short and common names. e is commonly used for exceptions.
 good-names = "e,fp,i,s,s3"
 # Classes with a single responsibility are fine.
 min-public-methods = 1
 
 [tool.pylint-per-file-ignores]
+# Import aliases are prefered over unused imports or __all__
+"__init__.py" = "useless-import-alias"
 "/tests/" = "missing-function-docstring,protected-access"
 # Sphinx specific
 "/docs/" = "invalid-name,redefined-builtin"
 
 [tool.isort]
 profile = "black"
```

### Comparing `scw_serverless-1.0.2/scw_serverless/app.py` & `scw_serverless-1.1.0/scw_serverless/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from typing import Any, Callable, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, Optional, Union
 
-try:
-    from typing import Unpack
-except ImportError:
-    from typing_extensions import Unpack
-# pylint: disable=wrong-import-position # Conditional import considered a statement
+if TYPE_CHECKING:
+    try:
+        from typing import Unpack
+    except ImportError:
+        from typing_extensions import Unpack
+    # pylint: disable=wrong-import-position # Conditional import considered a statement
 
+from scw_serverless.config import triggers
 from scw_serverless.config.function import Function, FunctionKwargs
 from scw_serverless.config.route import HTTPMethod
-from scw_serverless.triggers import CronTrigger
 
 
 class Serverless:
     """Manage your Serverless Functions.
 
     Maps to a function namespace. Parameters will be scoped to the namespace.
 
@@ -30,15 +31,15 @@
         self.functions: list[Function] = []
         self.service_name: str = service_name
         self.env = env
         self.secret = secret
 
     def func(
         self,
-        **kwargs: Unpack[FunctionKwargs],
+        **kwargs: "Unpack[FunctionKwargs]",
     ) -> Callable:
         """Define a Serverless handler and its parameters from the keyword arguments.
 
         See :any:`FunctionKwargs` for all possible parameters.
 
         Example
         -------
@@ -61,17 +62,17 @@
 
             return handler
 
         return _decorator
 
     def schedule(
         self,
-        schedule: Union[str, CronTrigger],
+        schedule: Union[str, triggers.CronTrigger],
         inputs: Optional[dict[str, Any]] = None,
-        **kwargs: Unpack[FunctionKwargs],
+        **kwargs: "Unpack[FunctionKwargs]",
     ) -> Callable:
         """Define a scheduled handler with Cron, passing inputs as parameters.
 
         :param schedule: cron schedule to use
         :param inputs: parameters to be passed to the body
 
         Example
@@ -80,79 +81,79 @@
         .. code-block:: python
 
             app.schedule(schedule="5 4 * * sun", inputs={"foo": "bar"}, memory=1024)
             def handler(event, context)
                 ...
         """
         if isinstance(schedule, str):
-            schedule = CronTrigger(schedule, inputs)
+            schedule = triggers.CronTrigger(schedule, inputs)
         elif inputs:
             schedule.args = (schedule.args or {}) | inputs
         if "triggers" in kwargs and kwargs["triggers"]:
             kwargs["triggers"].append(schedule)
         else:
             kwargs["triggers"] = [schedule]
         return self.func(**kwargs)
 
-    def get(self, url: str, **kwargs: Unpack[FunctionKwargs]) -> Callable:
+    def get(self, url: str, **kwargs: "Unpack[FunctionKwargs]") -> Callable:
         """Define a routed handler which will respond to GET requests.
 
         :param url: relative url to trigger the function
 
         .. note::
 
             Requires an API gateway
 
             For more information, please consult the :doc:`gateway` page.
         """
         kwargs |= {"relative_url": url, "http_methods": [HTTPMethod.GET]}
         return self.func(**kwargs)
 
-    def post(self, url: str, **kwargs: Unpack[FunctionKwargs]) -> Callable:
+    def post(self, url: str, **kwargs: "Unpack[FunctionKwargs]") -> Callable:
         """Define a routed handler which will respond to POST requests.
 
         :param url: relative url to trigger the function
 
         .. note::
             Requires an API gateway
 
             For more information, please consult the :doc:`gateway` page.
         """
         kwargs |= {"relative_url": url, "http_methods": [HTTPMethod.POST]}
         return self.func(**kwargs)
 
-    def put(self, url: str, **kwargs: Unpack[FunctionKwargs]) -> Callable:
+    def put(self, url: str, **kwargs: "Unpack[FunctionKwargs]") -> Callable:
         """Define a routed handler which will respond to PUT requests.
 
         :param url: relative url to trigger the function
 
         .. note::
 
             Requires an API gateway
 
             For more information, please consult the :doc:`gateway` page.
         """
         kwargs |= {"relative_url": url, "http_methods": [HTTPMethod.PUT]}
         return self.func(**kwargs)
 
-    def delete(self, url: str, **kwargs: Unpack[FunctionKwargs]) -> Callable:
+    def delete(self, url: str, **kwargs: "Unpack[FunctionKwargs]") -> Callable:
         """Define a routed handler which will respond to DELETE requests.
 
         :param url: relative url to trigger the function
 
         .. note::
 
             Requires an API gateway
 
             For more information, please consult the :doc:`gateway` page.
         """
         kwargs |= {"relative_url": url, "http_methods": [HTTPMethod.DELETE]}
         return self.func(**kwargs)
 
-    def patch(self, url: str, **kwargs: Unpack[FunctionKwargs]) -> Callable:
+    def patch(self, url: str, **kwargs: "Unpack[FunctionKwargs]") -> Callable:
         """Define a routed handler which will respond to PATCH requests.
 
         :param url: relative url to trigger the function
 
         .. note::
 
             Requires an API gateway
```

### Comparing `scw_serverless-1.0.2/scw_serverless/config/function.py` & `scw_serverless-1.1.0/scw_serverless/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,138 +1,175 @@
-import sys
-from dataclasses import dataclass, field
-from typing import Callable, Literal, Optional, TypedDict
-
-import scaleway.function.v1beta1 as sdk
-
-from scw_serverless.config.route import GatewayRoute, HTTPMethod
-from scw_serverless.logger import get_logger
-from scw_serverless.triggers import Trigger
-from scw_serverless.utils.string import module_to_path, to_valid_fn_name
-
-MemoryLimit = Literal[128, 256, 512, 1024, 2048, 3072, 4096]
-Privacy = Literal["private", "public"]  # Stricter than FunctionPrivacy from the SDK
-HTTPOption = Literal["enabled", "redirected"]
+import logging
+from pathlib import Path
+from typing import Optional, cast
+
+import click
+from scaleway import ScalewayException
+
+import scw_serverless
+from scw_serverless import app, deployment, loader, local_app, logger
+from scw_serverless.dependencies_manager import DependenciesManager
+from scw_serverless.gateway.gateway_manager import GatewayManager
+
+CLICK_ARG_FILE = click.argument(
+    "file",
+    required=True,
+    type=click.Path(
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True,
+        path_type=Path,
+    ),
+)
+
+
+@click.group()
+@click.option("--verbose", is_flag=True, help="Enables verbose mode.")
+@click.option(
+    "--log-level",
+    type=click.Choice(["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]),
+    default="INFO",
+    show_default=True,
+    help="Set the log level.",
+)
+def cli(verbose: bool, log_level: str) -> None:
+    """Deploy your Serverless functions on Scaleway's Cloud.
 
+    Documentation:
+    https://serverless-api-project.readthedocs.io/en/latest/
+    """
+    logger.configure_logger(verbose, log_level=getattr(logging, log_level))
 
-def _get_current_runtime() -> sdk.FunctionRuntime:
-    runtime = sdk.FunctionRuntime.PYTHON310
-    version = f"python{sys.version_info.major}{sys.version_info.minor}"
-    try:
-        runtime = sdk.FunctionRuntime(version)
-    except ValueError:
-        get_logger().warning(
-            f"Unsupported Python version: {version}, selecting default: {runtime}"
-        )
-    return runtime
 
+@cli.command()
+@CLICK_ARG_FILE
+@click.option(
+    "--gateway-url",
+    default=None,
+    help="URL of a deployed API Gateway.",
+)
+@click.option(
+    "--gateway-api-key",
+    default=None,
+    help="API key used to manage the routes of the API Gateway.",
+)
+@click.option(
+    "--runtime",
+    default=None,
+    help="Python runtime to deploy with. Uses your Python version by default.",
+)
+@click.option(
+    "--single-source",
+    is_flag=True,
+    default=True,
+    help="Remove functions not present in the code being deployed",
+)
+@click.option(
+    "--profile",
+    "-p",
+    default=None,
+    help="Scaleway profile to use when loading credentials.",
+)
+@click.option(
+    "--project-id",
+    default=None,
+    help="""API Project ID used for the deployment.
+WARNING: Please use environment variables instead""",
+)
+@click.option(
+    "--region",
+    default=None,
+    help="Region to deploy to.",
+)
+# pylint: disable=too-many-arguments
+def deploy(
+    file: Path,
+    gateway_url: Optional[str],
+    gateway_api_key: Optional[str],
+    runtime: Optional[str],
+    single_source: bool,
+    profile: Optional[str] = None,
+    secret_key: Optional[str] = None,
+    project_id: Optional[str] = None,
+    region: Optional[str] = None,
+) -> None:
+    """Deploy your functions to Scaleway.
 
-class FunctionKwargs(TypedDict, total=False):
-    """Typed arguments supported by Scaleway functions.
+    FILE is the file containing your functions handlers
 
-    .. note::
+    If the credentials are not provided, the credentials will
+    be pulled from your Scaleway configuration.
+    """
+    # Get the serverless App instance
+    app_instance = loader.load_app_instance(file.resolve())
 
-        Some parameters may not be supported by a specific backend.
+    # Check if the application requires a Gateway
+    needs_gateway = any(function.gateway_route for function in app_instance.functions)
+    if needs_gateway and not gateway_url:
+        logging.debug("Prompting for Serverless Gateway URL...")
+        gateway_url = click.prompt(
+            "Please enter the URL of your Serverless Gateway", type=str
+        )
+    if needs_gateway and not gateway_api_key:
+        logging.debug("Prompting for Serverless Gateway API key...")
+        gateway_url = click.prompt(
+            "Please enter the API key to your Serverless Gateway",
+            hide_input=True,
+            type=str,
+        )
 
-    :param env: Environment variables to be made available in your function.
-    :param secret: Secret environment variables to be made available in your function.
-    :param min_scale: Minimum replicas for your function.
-    :param max_scale: Maximum replicas for your function.
-    :param memory_limit: Memory (in MB) allocated to your function.
-    :param timeout: Max duration to respond to a request.
-    :param description: Description. Defaults to the function docstring if defined.
-    :param http_option: Either "enabled" or "redirected".
-                        If "redirected" (default), allow http traffic to your function.
-                        Blocked otherwise.
+    client = deployment.get_scw_client(profile, secret_key, project_id, region)
 
-    .. seealso::
+    if not runtime:
+        runtime = deployment.get_current_runtime()
 
-        `Scaleway Developers Documentation
-        <https://developers.scaleway.com/en/products/functions/api/#create-a-function>`_
-    """
+    logging.info("Packaging dependencies...")
+    deps = DependenciesManager(file.parent, Path.cwd())
+    deps.generate_package_folder()
 
-    env: dict[str, str]
-    secret: dict[str, str]
-    min_scale: int
-    max_scale: int
-    memory_limit: MemoryLimit
-    timeout: str
-    custom_domains: list[str]
-    privacy: Privacy
-    description: str
-    http_option: HTTPOption
-    # Parameters for the Gateway
-    relative_url: str
-    http_methods: list[HTTPMethod]
-    # Triggers
-    triggers: list[Trigger]
-
-
-# pylint: disable=too-many-instance-attributes
-@dataclass
-class Function:
-    """Representation of a Scaleway function."""
-
-    name: str
-    handler: str  # Path to the handler
-    runtime: sdk.FunctionRuntime
-    environment_variables: Optional[dict[str, str]] = None
-    min_scale: Optional[int] = None
-    max_scale: Optional[int] = None
-    memory_limit: Optional[int] = None
-    timeout: Optional[str] = None
-    secret_environment_variables: Optional[list[sdk.Secret]] = None
-    privacy: Optional[sdk.FunctionPrivacy] = None
-    description: Optional[str] = None
-    http_option: Optional[sdk.FunctionHttpOption] = None
-    gateway_route: Optional[GatewayRoute] = None
-    domains: list[str] = field(default_factory=list)
-    triggers: list[Trigger] = field(default_factory=list)
-
-    @staticmethod
-    def from_handler(
-        handler: Callable,
-        args: FunctionKwargs,
-    ):
-        """Create a Scaleway function from a handler."""
-        description = args.get("description")
-        if not description and handler.__doc__:
-            description = handler.__doc__
-        secrets = None
-        if args_secret := args.get("secret"):
-            secrets = [sdk.Secret(key, value) for key, value in args_secret.items()]
-        privacy = None
-        if args_privacy := args.get("privacy"):
-            privacy = sdk.FunctionPrivacy(args_privacy)
-        http_option = None
-        if args_http_option := args.get("http_option"):
-            http_option = sdk.FunctionHttpOption(args_http_option)
-        gateway_route = None
-        if url := args.get("relative_url"):
-            gateway_route = GatewayRoute(url, http_methods=args.get("http_methods"))
-
-        return Function(
-            name=to_valid_fn_name(handler.__name__),
-            handler=module_to_path(handler.__module__) + "." + handler.__name__,
-            environment_variables=args.get("env"),
-            min_scale=args.get("min_scale"),
-            max_scale=args.get("max_scale"),
-            runtime=_get_current_runtime(),
-            memory_limit=args.get("memory_limit"),
-            timeout=args.get("timeout"),
-            secret_environment_variables=secrets,
-            privacy=privacy,
-            description=description,
-            http_option=http_option,
-            gateway_route=gateway_route,
-            domains=args.get("custom_domains") or [],
-            triggers=args.get("triggers") or [],
+    try:
+        deployment.DeploymentManager(
+            app_instance=app_instance,
+            sdk_client=client,
+            runtime=runtime,
+            single_source=single_source,
+        ).deploy()
+    except ScalewayException as e:
+        logging.debug(e, exc_info=True)
+        deployment.log_scaleway_exception(e)
+
+    if needs_gateway:
+        manager = GatewayManager(
+            app_instance=app_instance,
+            gateway_url=cast(str, gateway_url),
+            gateway_api_key=cast(str, gateway_api_key),
+            sdk_client=client,
         )
+        manager.update_routes()
+
 
-    def secrets_asdict(self) -> Optional[dict[str, str]]:
-        """Gets secret_environment_variables as a dictionary"""
-        if not self.secret_environment_variables:
-            return None
-        return {
-            secret.key: (secret.value or "")
-            for secret in self.secret_environment_variables
-        }
+@cli.command()
+@CLICK_ARG_FILE
+@click.option(
+    "--port",
+    "-p",
+    "port",
+    default=8080,
+    show_default=True,
+    help="Set port to listen on.",
+)
+@click.option(
+    "--debug/--no-debug",
+    "debug",
+    default=True,
+    show_default=True,
+    help="Run Flask in debug mode.",
+)
+def dev(file: Path, port: int, debug: bool) -> None:
+    """Run functions locally with Serverless Local Testing."""
+    app.Serverless = local_app.ServerlessLocal
+    scw_serverless.Serverless = local_app.ServerlessLocal
+    app_instance = cast(
+        local_app.ServerlessLocal, loader.load_app_instance(file.resolve())
+    )
+    app_instance.local_server.serve(port=port, debug=debug)
```

### Comparing `scw_serverless-1.0.2/scw_serverless/config/route.py` & `scw_serverless-1.1.0/scw_serverless/config/route.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Optional
 
-from scw_serverless.config.utils import _SerializableDataClass
-
 
 class HTTPMethod(Enum):
     """Enum of supported HTTP methods.
 
     .. seealso:: https://docs.python.org/3/library/http.html#http.HTTPMethod
     """
 
@@ -15,15 +13,15 @@
     POST = "POST"
     PUT = "PUT"
     DELETE = "DELETE"
     PATCH = "PATCH"
 
 
 @dataclass
-class GatewayRoute(_SerializableDataClass):
+class GatewayRoute:
     """Route to a function."""
 
     relative_url: str
     http_methods: Optional[list[HTTPMethod]] = None
     target: Optional[str] = None
 
     def validate(self) -> None:
@@ -33,11 +31,14 @@
         if not self.target:
             raise RuntimeError("Route target must be defined")
         for method in self.http_methods or []:
             if method not in HTTPMethod:
                 raise RuntimeError(f"Route contains invalid method {method.value}")
 
     def asdict(self) -> dict[str, Any]:
-        serialized = super().asdict()
+        """Return a dict representation of a route."""
+        serialized: dict[str, Any] = {"relative_url": self.relative_url}
         if self.http_methods:
             serialized["http_methods"] = [method.value for method in self.http_methods]
+        if self.target:
+            serialized["target"] = self.target
         return serialized
```

### Comparing `scw_serverless-1.0.2/scw_serverless/deploy/backends/scaleway_api_backend.py` & `scw_serverless-1.1.0/scw_serverless/deployment/deployment_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,136 +1,107 @@
+import logging
 import multiprocessing
 import os
 
+import click
 import requests
 import scaleway.function.v1beta1 as sdk
-from scaleway import Client
-from scaleway_core.utils import WaitForOptions
+from scaleway import Client, ScalewayException
 
 from scw_serverless.app import Serverless
 from scw_serverless.config.function import Function
-from scw_serverless.deploy.backends.serverless_backend import ServerlessBackend
-from scw_serverless.triggers import Trigger
+from scw_serverless.config.triggers import CronTrigger
+from scw_serverless.deployment.api_wrapper import FunctionAPIWrapper
 from scw_serverless.utils.files import create_zip_file
 
 TEMP_DIR = "./.scw"
 DEPLOYMENT_ZIP = f"{TEMP_DIR}/deployment.zip"
-UPLOAD_TIMEOUT = 600  # In seconds
-DEPLOY_TIMEOUT = 600
+UPLOAD_TIMEOUT_SECONDS = 600
 
 
-class ScalewayApiBackend(ServerlessBackend):
+class DeploymentManager:
     """Uses the API to deploy functions."""
 
     def __init__(
-        self, app_instance: Serverless, sdk_client: Client, single_source: bool
+        self,
+        app_instance: Serverless,
+        sdk_client: Client,
+        single_source: bool,
+        runtime: str,
     ):
-        super().__init__(app_instance, sdk_client)
+        self.api = FunctionAPIWrapper(api=sdk.FunctionV1Beta1API(sdk_client))
+        self.app_instance = app_instance
+        self.sdk_client = sdk_client
+        # Behavior configuration
         self.single_source = single_source
-        self.api = sdk.FunctionV1Beta1API(sdk_client)
+        self.runtime = sdk.FunctionRuntime(runtime)
 
     def _get_or_create_function(self, function: Function, namespace_id: str) -> str:
-        self.logger.default(f"Looking for an existing function {function.name}...")
-        created_function = None
+        logging.info("Looking for an existing function %s...", function.name)
         # Checking if a function already exists
-        for func in self.api.list_functions_all(namespace_id=namespace_id):
-            if func.name == function.name:
-                created_function = func
-        if not created_function:
-            self.logger.default(f"Creating a new function {function.name}...")
+        deployed_function = self.api.find_deployed_function(
+            namespace_id=namespace_id, function=function
+        )
+        if not deployed_function:
+            logging.info("Creating a new function %s...", function.name)
             # Creating a new function with the provided args
-            created_function = self.api.create_function(
-                namespace_id=namespace_id,
-                runtime=function.runtime,
-                privacy=function.privacy or sdk.FunctionPrivacy.PUBLIC,
-                http_option=sdk.FunctionHttpOption.REDIRECTED,
-                name=function.name,
-                environment_variables=function.environment_variables,
-                min_scale=function.min_scale,
-                max_scale=function.max_scale,
-                memory_limit=function.memory_limit,
-                timeout=function.timeout,
-                handler=function.handler,
-                description=function.description,
-                secret_environment_variables=function.secret_environment_variables,
+            deployed_function = self.api.create_function(
+                namespace_id=namespace_id, function=function, runtime=self.runtime
             )
         else:
             # Updating the function with the provided args
-            created_function = self.api.update_function(
-                function_id=created_function.id,
-                runtime=function.runtime,
-                privacy=function.privacy or sdk.FunctionPrivacy.PUBLIC,
-                http_option=sdk.FunctionHttpOption.REDIRECTED,
-                environment_variables=function.environment_variables,
-                min_scale=function.min_scale,
-                max_scale=function.max_scale,
-                memory_limit=function.memory_limit,
-                timeout=function.timeout,
-                handler=function.handler,
-                description=function.description,
-                secret_environment_variables=function.secret_environment_variables,
+            deployed_function = self.api.update_function(
+                function_id=deployed_function.id,
+                function=function,
+                runtime=self.runtime,
             )
-        return created_function.id
+        return deployed_function.id
 
     def _deploy_function(
         self, function: Function, namespace_id: str, zip_size: int
     ) -> sdk.Function:
         function_id = self._get_or_create_function(function, namespace_id)
 
         # Get an object storage pre-signed url
         try:
-            upload_url = self.api.get_function_upload_url(
-                function_id=function_id, content_length=zip_size
-            ).url
-        except Exception as exception:
-            self.logger.error(
+            upload_url = self.api.get_upload_url(
+                function_id=function_id, zip_size=zip_size
+            )
+        except ScalewayException as e:
+            logging.error(
                 "Unable to retrieve upload url... "
-                + "Verify that your function is less that 100 MB"
+                "Verify that your function is less that 100 MB"
             )
-            raise exception
+            raise e
 
-        self.logger.default(f"Uploading function {function.name}...")
+        logging.info("Uploading function %s...", function.name)
         self._upload_deployment_zip(upload_url, zip_size)
 
-        self.logger.default(f"Deploying function {function.name}...")
-        # deploy the newly uploaded function
-        self.api.deploy_function(function_id=function_id)
-
-        return self.api.wait_for_function(
-            function_id=function_id,
-            options=WaitForOptions(
-                timeout=DEPLOY_TIMEOUT,
-                stop=lambda f: (f.status != sdk.FunctionStatus.PENDING),
-            ),
-        )
+        logging.info("Deploying function %s...", function.name)
+        # Deploy the newly uploaded function
+        return self.api.deploy_function(function_id=function_id)
 
-    def _deploy_trigger(self, function_id: str, trigger: Trigger) -> sdk.Cron:
-        created_trigger = None
+    def _deploy_cron_trigger(self, function_id: str, trigger: CronTrigger) -> sdk.Cron:
         # Checking if a trigger already exists
-        for cron in self.api.list_crons_all(function_id=function_id):
-            if cron.name == trigger.name:
-                created_trigger = cron
-        if not created_trigger:
-            created_trigger = self.api.create_cron(
-                function_id=function_id,
-                schedule=trigger.schedule,
-                name=trigger.name,
-                args=trigger.args,
+        deployed_trigger = self.api.find_deployed_cron_trigger(
+            function_id=function_id, trigger=trigger
+        )
+        if not deployed_trigger:
+            deployed_trigger = self.api.create_cron_trigger(
+                function_id=function_id, trigger=trigger
             )
         else:
-            created_trigger = self.api.update_cron(
-                cron_id=created_trigger.id,
-                schedule=trigger.schedule,
-                args=trigger.args,
+            deployed_trigger = self.api.update_cron_trigger(
+                function_id=function_id, trigger=trigger
             )
-        return self.api.wait_for_cron(cron_id=created_trigger.id)
+        return deployed_trigger
 
     def _create_deployment_zip(self) -> int:
         """Create a ZIP archive containing the entire project."""
-        self.logger.default("Creating a deployment archive...")
+        logging.info("Creating a deployment archive...")
         if not os.path.exists(TEMP_DIR):
             os.mkdir(TEMP_DIR)
 
         if os.path.exists(DEPLOYMENT_ZIP):
             os.remove(DEPLOYMENT_ZIP)
 
         create_zip_file(DEPLOYMENT_ZIP, "./")
@@ -142,78 +113,51 @@
             req = requests.put(
                 upload_url,
                 data=file,
                 headers={
                     "Content-Type": "application/octet-stream",
                     "Content-Length": str(zip_size),
                 },
-                timeout=UPLOAD_TIMEOUT,
+                timeout=UPLOAD_TIMEOUT_SECONDS,
             )
             if req.status_code != 200:
                 raise RuntimeError("Unable to upload function code... Aborting...")
 
-    def _remove_missing_functions(self, namespace_id: str):
-        """Deletes functions no longer present in the code."""
-        function_names = [func.name for func in self.app_instance.functions]
-        for function in self.api.list_functions_all(namespace_id=namespace_id):
-            if function.name not in function_names:
-                self.logger.info(f"Deleting function {function.name}...")
-                self.api.delete_function(function_id=function.id)
-
-    def _remove_missing_triggers(self, namespace_id: str, deployed_triggers: set[str]):
-        """Deletes triggers no longer present in the code."""
-        for function in self.api.list_functions_all(namespace_id=namespace_id):
-            unmanaged = filter(
-                lambda c: c.id not in deployed_triggers,
-                self.api.list_crons_all(function_id=function.id),
-            )
-            for cron in unmanaged:
-                self.logger.info(f"Deleting Cron {cron.name}...")
-                self.api.delete_cron(cron_id=cron.id)
-
     def _get_or_create_namespace(self) -> str:
-        project_id = self.api.client.default_project_id
         namespace_name = self.app_instance.service_name
-        namespace = None
-        self.logger.default(
-            f"Looking for an existing namespace {namespace_name} in {project_id}..."
+        project_id = self.sdk_client.default_project_id
+        logging.debug(
+            "Looking for an existing namespace %s in project %s...",
+            namespace_name,
+            project_id,
         )
-        # Search in the user's namespace if one is matching the same name and region
-        for deployed_namespace in self.api.list_namespaces_all():
-            if deployed_namespace.name == self.app_instance.service_name:
-                namespace = deployed_namespace
-        secrets = [
-            sdk.Secret(key, value)
-            for key, value in (self.app_instance.secret or {}).items()
-        ]
-        if not namespace:
-            self.logger.default(
-                f"Creating a new namespace {namespace_name} in {project_id}..."
-            )
-            # Create a new namespace
-            namespace = self.api.create_namespace(
-                name=namespace_name,
-                environment_variables=self.app_instance.env,
-                secret_environment_variables=secrets,
+        deployed_namespace = self.api.find_deployed_namespace(
+            app_instance=self.app_instance
+        )
+        if not deployed_namespace:
+            logging.info(
+                "Creating a new namespace %s in %s...", namespace_name, project_id
+            )
+            deployed_namespace = self.api.create_namespace(
+                app_instance=self.app_instance
             )
         else:
-            self.logger.default("Updating namespace configuration...")
-            namespace = self.api.update_namespace(
-                namespace_id=namespace.id,
-                environment_variables=self.app_instance.env,
-                secret_environment_variables=secrets,
+            logging.debug("Updating namespace %s configuration...", namespace_name)
+            deployed_namespace = self.api.update_namespace(
+                namespace_id=deployed_namespace.id, app_instance=self.app_instance
             )
-        namespace = self.api.wait_for_namespace(namespace_id=namespace.id)
-        if namespace.status != sdk.NamespaceStatus.READY:
+        if deployed_namespace.status != sdk.NamespaceStatus.READY:
             raise ValueError(
-                f"Namespace {namespace.name} is not ready: {namespace.error_message}"
+                f"Namespace {deployed_namespace.name} is not ready: "
+                + (deployed_namespace.error_message or "")
             )
-        return namespace.id
+        return deployed_namespace.id
 
     def deploy(self) -> None:
+        """Deploy all configured functions using the Scaleway API."""
         namespace_id = self._get_or_create_namespace()
         # Create a zip containing the user's project
         file_size = self._create_deployment_zip()
 
         deploy_inputs = [
             (function, namespace_id, file_size)
             for function in self.app_instance.functions
@@ -229,35 +173,40 @@
         with multiprocessing.Pool(processes=n_proc) as pool:
             for function in pool.starmap(self._deploy_function, deploy_inputs):
                 if function.status is sdk.FunctionStatus.ERROR:
                     raise ValueError(
                         f"Function {function.name} is in error state: "
                         + (function.error_message or "")
                     )
-                self.logger.success(
+                click.secho(
                     f"Function {function.name} deployed to: "
-                    + f"https://{function.domain_name}"
+                    + f"https://{function.domain_name}",
+                    fg="green",
                 )
                 function_ids[function.name] = function.id
 
             if triggers_to_deploy:
-                self.logger.default("Deploying triggers...")
+                logging.info("Deploying triggers...")
 
             triggers_to_deploy = [
                 (function_ids[k], t)
                 for k, triggers in triggers_to_deploy.items()
                 for t in triggers
             ]
 
             deployed_triggers: set[str] = set()
-            for trigger in pool.starmap(self._deploy_trigger, triggers_to_deploy):
+            for trigger in pool.starmap(self._deploy_cron_trigger, triggers_to_deploy):
                 if trigger.status is sdk.CronStatus.ERROR:
                     raise ValueError(f"Trigger {trigger.name} is in error state")
                 deployed_triggers.add(trigger.id)
 
+        click.secho("Done! Functions have been successfully deployed!", fg="green")
+
         if self.single_source:
             # Remove functions no longer present in the code
-            self._remove_missing_functions(namespace_id)
+            self.api.delete_all_functions_from_ns_except(
+                namespace_id=namespace_id, function_ids=list(function_ids.values())
+            )
             # Remove triggers
-            self._remove_missing_triggers(namespace_id, deployed_triggers)
-
-        self.logger.success("Done! Functions have been successfully deployed!")
+            self.api.delete_all_crons_from_ns_except(
+                namespace_id=namespace_id, cron_ids=list(deployed_triggers)
+            )
```

### Comparing `scw_serverless-1.0.2/scw_serverless/gateway/gateway_api_client.py` & `scw_serverless-1.1.0/scw_serverless/gateway/gateway_api_client.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.2/scw_serverless/gateway/gateway_manager.py` & `scw_serverless-1.1.0/scw_serverless/gateway/gateway_manager.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.2/scw_serverless/triggers/cron.py` & `scw_serverless-1.1.0/scw_serverless/config/triggers.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.2/scw_serverless/utils/credentials.py` & `scw_serverless-1.1.0/scw_serverless/deployment/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
+import logging
 from importlib.metadata import version
 from typing import Optional
 
 from scaleway import Client
 from scaleway_core.bridge.region import REGION_FR_PAR
 
-from scw_serverless.logger import get_logger
-
 DEFAULT_REGION: str = REGION_FR_PAR
 
 
 def get_scw_client(
     profile_name: Optional[str],
     secret_key: Optional[str],
     project_id: Optional[str],
@@ -42,13 +41,13 @@
 ):
     """Update Client with defined CLI arguments."""
     client.user_agent = f'scw-serverless/{version("scw_serverless")}'
     client.secret_key = secret_key or client.secret_key
     client.default_project_id = project_id or client.default_project_id
     client.default_region = region or client.default_region
     if not client.default_region:
-        get_logger().info(f"No region was configured, using {DEFAULT_REGION}")
+        logging.info("No region was configured, using %s", DEFAULT_REGION)
         client.default_region = DEFAULT_REGION
 
     # Not used by the API framework
     # Can lead to issues if project_id does not belong to organization
     client.default_organization_id = None
```

### Comparing `scw_serverless-1.0.2/scw_serverless/utils/files.py` & `scw_serverless-1.1.0/scw_serverless/utils/files.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.2/scw_serverless/utils/loader.py` & `scw_serverless-1.1.0/scw_serverless/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import importlib.util
 import inspect
+import logging
 import sys
 from pathlib import Path
 
 from scw_serverless.app import Serverless
 
 
 def get_module_name(file: Path) -> str:
@@ -11,18 +12,19 @@
 
     file = file.resolve()
     return (
         str(file.relative_to(Path(".").resolve())).removesuffix(".py").replace("/", ".")
     )
 
 
-def get_app_instance(file: Path) -> Serverless:
+def load_app_instance(file: Path) -> Serverless:
     """Load the app instance from the client module."""
 
     module_name = get_module_name(file)
+    logging.debug("Loading the Serverless instance from module %s", module_name)
     parent_directory = str(file.parent.resolve())
 
     spec = importlib.util.spec_from_file_location(
         module_name,
         str(file.resolve()),
         submodule_search_locations=[parent_directory],
     )
```

### Comparing `scw_serverless-1.0.2/setup.py` & `scw_serverless-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['scw_serverless',
  'scw_serverless.config',
- 'scw_serverless.config.generators',
- 'scw_serverless.deploy',
- 'scw_serverless.deploy.backends',
+ 'scw_serverless.deployment',
  'scw_serverless.gateway',
- 'scw_serverless.triggers',
  'scw_serverless.utils']
 
 package_data = \
-{'': ['*'], 'scw_serverless.config': ['templates/*']}
+{'': ['*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0',
- 'pyyaml>=6.0,<7.0',
  'requests>=2.28.2,<3.0.0',
- 'scaleway>=0.7,<0.12']
+ 'scaleway-functions-python>=0.2.0,<0.3.0',
+ 'scaleway>=0.7,<0.13']
 
 extras_require = \
 {':python_version < "3.11"': ['typing-extensions>=4.4.0,<5.0.0']}
 
 entry_points = \
-{'console_scripts': ['scw-serverless = scw_serverless.cli:main']}
+{'console_scripts': ['scw-serverless = scw_serverless.cli:cli']}
 
 setup_kwargs = {
     'name': 'scw-serverless',
-    'version': '1.0.2',
+    'version': '1.1.0',
     'description': 'Framework for writing serverless APIs in Python, using Scaleway functions and containers.',
-    'long_description': '# Serverless API Framework\n\n[![PyPI version](https://badge.fury.io/py/scw-serverless.svg)](https://badge.fury.io/py/scw-serverless)\n[![Documentation Status](https://readthedocs.org/projects/serverless-api-project/badge/?version=latest)](https://serverless-api-project.readthedocs.io/en/latest/?badge=latest)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scaleway/serverless-api-framework-python/main.svg)](https://results.pre-commit.ci/latest/github/scaleway/serverless-api-framework-python/main)\n\nServerless API Framework is a tool that lets you write and deploy serverless functions in Python.\nIt bridges your code with the deployment configuration to make it a breeze to work with serverless functions.\n\nStarts by defining a simple Python function:\n\n```python\nfrom scw_serverless import Serverless\n\napp = Serverless("hello-namespace")\n\n@app.func(memory_limit=256)\ndef hello_world(event, context):\n    return "Hello World!"\n```\n\nDeploy it with `scw-serverless`:\n\n```console\nscw-serverless deploy app.py\n```\n\n## Quickstart\n\n### Install\n\n```console\npip install scw-serverless\n```\n\nThis will install the `scw-serverless` CLI:\n\n```console\nscw-serverless --help\n```\n\n### Writing and configuring functions\n\nYou can transform your Python functions into serverless functions by using decorators:\n\n```python\nimport os\nimport requests\nfrom scw_serverless import Serverless\n\napp = Serverless("hello-namespace")\nAPI_URL = os.environ["API_URL"]\n\n@app.func(memory_limit=256, env={"API_URL": API_URL})\ndef hello_world(event, context):\n    return requests.get(API_URL)\n```\n\nThe configuration is done by passing arguments to the decorator.\nTo view which arguments are supported, head over to this [documentation](https://serverless-api-framework-python.readthedocs.io/) page.\n\nWhen you are ready, you can deploy your function with the `scw-serverless` CLI tool:\n\n```console\nscw-serverless deploy app.py\n```\n\nThe tool will use your Scaleway credentials from your environment and config file.\n\n## What’s Next?\n\nTo learn more about the framework, have a look at the [documentation](https://serverless-api-project.readthedocs.io/).\nIf you want to see it in action, we provide some [examples](https://github.com/scaleway/serverless-api-framework-python-python/tree/main/examples) to get you started.\n\nTo run your Python functions locally, check out [Scaleway Functions Python](https://github.com/scaleway/serverless-functions-python).\n\n## Contributing\n\nWe welcome all contributions.\n\nThis project uses [pre-commit](https://pre-commit.com/) hooks to run code quality checks locally. We recommended installing them before contributing.\n\n```console\npre-commit install\n```\n',
+    'long_description': '# Serverless API Framework\n\n[![PyPI version](https://badge.fury.io/py/scw-serverless.svg)](https://badge.fury.io/py/scw-serverless)\n[![Documentation Status](https://readthedocs.org/projects/serverless-api-project/badge/?version=latest)](https://serverless-api-project.readthedocs.io/en/latest/?badge=latest)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scaleway/serverless-api-framework-python/main.svg)](https://results.pre-commit.ci/latest/github/scaleway/serverless-api-framework-python/main)\n\nServerless API Framework is a tool that lets you write and deploy serverless functions in Python.\nIt bridges your code with the deployment configuration to make it a breeze to work with serverless functions.\n\nStarts by defining a simple Python function:\n\n```python\nfrom scw_serverless import Serverless\n\napp = Serverless("hello-namespace")\n\n@app.func(memory_limit=256)\ndef hello_world(event, context):\n    return "Hello World!"\n```\n\nDeploy it with `scw-serverless`:\n\n```console\nscw-serverless deploy app.py\n```\n\n## Quickstart\n\n### Install\n\n```console\npip install scw-serverless\n```\n\nThis will install the `scw-serverless` CLI:\n\n```console\nscw-serverless --help\n```\n\n### Writing and configuring functions\n\nYou can transform your Python functions into serverless functions by using decorators:\n\n```python\nimport os\nimport requests\nfrom scw_serverless import Serverless\n\napp = Serverless("hello-namespace")\nAPI_URL = os.environ["API_URL"]\n\n@app.func(memory_limit=256, env={"API_URL": API_URL})\ndef hello_world(event, context):\n    return requests.get(API_URL)\n```\n\nThe configuration is done by passing arguments to the decorator.\nTo view which arguments are supported, head over to this [documentation](https://serverless-api-framework-python.readthedocs.io/) page.\n\n### Local testing\n\nBefore deploying, you can run your functions locally with the dev command:\n\n```console\nscw-serverless dev app.py\n```\n\nThis runs a local Flask server with your Serverless handlers. If no `relative_url` is defined for a function, it will be served on `/name` with `name` being the name of your Python function.\n\nBy default, this runs Flask in debug mode which includes hot-reloading. You can disable this behavior by passing the `--no-debug` flag.\n\n### Deploying\n\nWhen you are ready, you can deploy your function with the `scw-serverless` CLI tool:\n\n```console\nscw-serverless deploy app.py\n```\n\nThe tool will use your Scaleway credentials from your environment and config file.\n\n## What’s Next?\n\nTo learn more about the framework, have a look at the [documentation](https://serverless-api-project.readthedocs.io/).\nIf you want to see it in action, we provide some [examples](https://github.com/scaleway/serverless-api-framework-python-python/tree/main/examples) to get you started.\n\nTo run your Python functions locally, check out [Scaleway Functions Python](https://github.com/scaleway/serverless-functions-python).\n\n## Contributing\n\nWe welcome all contributions.\n\nThis project uses [pre-commit](https://pre-commit.com/) hooks to run code quality checks locally. We recommended installing them before contributing.\n\n```console\npre-commit install\n```\n',
     'author': 'Scaleway Serverless Team',
     'author_email': 'opensource@scaleway.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/scaleway/serverless-api-framework-python-python',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.9,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `scw_serverless-1.0.2/PKG-INFO` & `scw_serverless-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: scw-serverless
-Version: 1.0.2
+Version: 1.1.0
 Summary: Framework for writing serverless APIs in Python, using Scaleway functions and containers.
 Home-page: https://github.com/scaleway/serverless-api-framework-python-python
 License: MIT
 Keywords: serverless,scaleway,functions,cloud,faas
 Author: Scaleway Serverless Team
 Author-email: opensource@scaleway.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -19,17 +19,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: scaleway (>=0.7,<0.12)
+Requires-Dist: scaleway (>=0.7,<0.13)
+Requires-Dist: scaleway-functions-python (>=0.2.0,<0.3.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) ; python_version < "3.11"
 Project-URL: Documentation, https://serverless-api-project.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/scaleway/serverless-api-framework-python-python
 Description-Content-Type: text/markdown
 
 # Serverless API Framework
 
@@ -88,14 +88,28 @@
 def hello_world(event, context):
     return requests.get(API_URL)
 ```
 
 The configuration is done by passing arguments to the decorator.
 To view which arguments are supported, head over to this [documentation](https://serverless-api-framework-python.readthedocs.io/) page.
 
+### Local testing
+
+Before deploying, you can run your functions locally with the dev command:
+
+```console
+scw-serverless dev app.py
+```
+
+This runs a local Flask server with your Serverless handlers. If no `relative_url` is defined for a function, it will be served on `/name` with `name` being the name of your Python function.
+
+By default, this runs Flask in debug mode which includes hot-reloading. You can disable this behavior by passing the `--no-debug` flag.
+
+### Deploying
+
 When you are ready, you can deploy your function with the `scw-serverless` CLI tool:
 
 ```console
 scw-serverless deploy app.py
 ```
 
 The tool will use your Scaleway credentials from your environment and config file.
```

