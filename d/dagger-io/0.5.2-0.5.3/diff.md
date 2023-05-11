# Comparing `tmp/dagger_io-0.5.2.tar.gz` & `tmp/dagger_io-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagger_io-0.5.2.tar", max compression
+gzip compressed data, was "dagger_io-0.5.3.tar", max compression
```

## Comparing `dagger_io-0.5.2.tar` & `dagger_io-0.5.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    10758 2023-04-28 17:39:56.098465 dagger_io-0.5.2/LICENSE
--rw-r--r--   0        0        0     4727 2023-04-28 17:39:56.098465 dagger_io-0.5.2/README.md
--rw-r--r--   0        0        0     6344 2023-04-28 17:41:23.691286 dagger_io-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      313 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/__init__.py
--rw-r--r--   0        0        0       49 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/__main__.py
--rw-r--r--   0        0        0       69 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/api/.gitattributes
--rw-r--r--   0        0        0        0 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/api/__init__.py
--rw-r--r--   0        0        0    10984 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/api/base.py
--rw-r--r--   0        0        0    83180 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/api/gen.py
--rw-r--r--   0        0        0    82872 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/api/gen_sync.py
--rw-r--r--   0        0        0     1650 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/cli.py
--rw-r--r--   0        0        0    18459 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/codegen.py
--rw-r--r--   0        0        0     1291 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/config.py
--rw-r--r--   0        0        0     1585 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/connection.py
--rw-r--r--   0        0        0      964 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/context.py
--rw-r--r--   0        0        0       37 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/engine/.gitattributes
--rw-r--r--   0        0        0       35 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/engine/__init__.py
--rw-r--r--   0        0        0       64 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/engine/_version.py
--rw-r--r--   0        0        0     4188 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/engine/cli.py
--rw-r--r--   0        0        0     2068 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/engine/conn.py
--rw-r--r--   0        0        0     8163 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/engine/download.py
--rw-r--r--   0        0        0     3042 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/exceptions.py
--rw-r--r--   0        0        0      677 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/log.py
--rw-r--r--   0        0        0        0 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/py.typed
--rw-r--r--   0        0        0     2320 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/server/__init__.py
--rw-r--r--   0        0        0      849 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/server/cli.py
--rw-r--r--   0        0        0      865 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/server/converter.py
--rw-r--r--   0        0        0     3892 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/session.py
--rw-r--r--   0        0        0        0 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/transport/__init__.py
--rw-r--r--   0        0        0     5820 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/transport/httpx.py
--rw-r--r--   0        0        0     5951 1970-01-01 00:00:00.000000 dagger_io-0.5.2/setup.py
--rw-r--r--   0        0        0     6524 1970-01-01 00:00:00.000000 dagger_io-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-05-11 19:41:57.916076 dagger_io-0.5.3/LICENSE
+-rw-r--r--   0        0        0     4727 2023-05-11 19:41:57.916076 dagger_io-0.5.3/README.md
+-rw-r--r--   0        0        0     6344 2023-05-11 19:43:04.841204 dagger_io-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      313 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/__main__.py
+-rw-r--r--   0        0        0       69 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/api/.gitattributes
+-rw-r--r--   0        0        0        0 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/api/__init__.py
+-rw-r--r--   0        0        0    11434 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/api/base.py
+-rw-r--r--   0        0        0    83180 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/api/gen.py
+-rw-r--r--   0        0        0    82872 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/api/gen_sync.py
+-rw-r--r--   0        0        0     1683 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/cli.py
+-rw-r--r--   0        0        0    18459 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/codegen.py
+-rw-r--r--   0        0        0     1302 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/config.py
+-rw-r--r--   0        0        0     1585 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/connection.py
+-rw-r--r--   0        0        0      964 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/context.py
+-rw-r--r--   0        0        0       37 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/engine/.gitattributes
+-rw-r--r--   0        0        0       35 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/engine/__init__.py
+-rw-r--r--   0        0        0       64 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/engine/_version.py
+-rw-r--r--   0        0        0     4202 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/engine/cli.py
+-rw-r--r--   0        0        0     2068 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/engine/conn.py
+-rw-r--r--   0        0        0     8163 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/engine/download.py
+-rw-r--r--   0        0        0     3042 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/exceptions.py
+-rw-r--r--   0        0        0      677 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/log.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/py.typed
+-rw-r--r--   0        0        0     2320 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/server/__init__.py
+-rw-r--r--   0        0        0      911 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/server/cli.py
+-rw-r--r--   0        0        0      865 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/server/converter.py
+-rw-r--r--   0        0        0     3892 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/session.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/transport/__init__.py
+-rw-r--r--   0        0        0     5820 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/transport/httpx.py
+-rw-r--r--   0        0        0     5951 1970-01-01 00:00:00.000000 dagger_io-0.5.3/setup.py
+-rw-r--r--   0        0        0     6524 1970-01-01 00:00:00.000000 dagger_io-0.5.3/PKG-INFO
```

### Comparing `dagger_io-0.5.2/LICENSE` & `dagger_io-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.2/README.md` & `dagger_io-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.2/pyproject.toml` & `dagger_io-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dagger-io"
-version = "0.5.2"
+version = "0.5.3"
 description = "A client package for running Dagger pipelines in Python."
 license = "Apache-2.0"
 authors = ["Dagger <hello@dagger.io>"]
 readme = "README.md"
 homepage = "https://dagger.io"
 documentation = "https://docs.dagger.io/sdk/python"
 repository = "https://github.com/dagger/dagger/tree/main/sdk/python"
```

### Comparing `dagger_io-0.5.2/src/dagger/api/base.py` & `dagger_io-0.5.3/src/dagger/api/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import attrs
 import cattrs
 import graphql
 import httpx
 from beartype import beartype
 from beartype.door import TypeHint
 from beartype.roar import BeartypeCallHintViolation
-from beartype.vale import IsInstance
+from beartype.vale import Is, IsInstance
 from cattrs.preconf.json import make_converter
 from gql.client import AsyncClientSession, SyncClientSession
 from gql.dsl import DSLField, DSLQuery, DSLSchema, DSLSelectable, DSLType, dsl_gql
 from gql.transport.exceptions import (
     TransportClosed,
     TransportProtocolError,
     TransportQueryError,
@@ -223,22 +223,41 @@
         return self.__class__.__name__
 
 
 class Input(Object):
     """Input object type."""
 
 
+InputType = Annotated[Input, Is[lambda o: attrs.has(o)]]
+InputTypeSeq = Annotated[Sequence[InputType], ~IsInstance[str]]
+
+InputHint = TypeHint(InputType)
+InputSeqHint = TypeHint(InputTypeSeq)
+
+
+def as_input_arg(val):
+    if InputHint.is_bearable(val):
+        return attrs.asdict(val)
+    if InputSeqHint.is_bearable(val):
+        return [attrs.asdict(v) for v in val]
+    return val
+
+
 @attrs.define
 class Type(Object):
     """Object type."""
 
     _ctx: Context
 
     def _select(self, field_name: str, args: typing.Sequence[Arg]) -> Context:
-        _args = {arg.name: arg.value for arg in args if arg.value is not arg.default}
+        _args = {
+            arg.name: as_input_arg(arg.value)
+            for arg in args
+            if arg.value is not arg.default
+        }
         return self._ctx.select(self.graphql_name, field_name, _args)
 
     def with_(self, cb: Callable[[Self], Self]) -> Self:
         """
         Use a callable to add to the current object.
 
         This allows reusing funcionality (e.g., adding mounts)
```

### Comparing `dagger_io-0.5.2/src/dagger/api/gen.py` & `dagger_io-0.5.3/src/dagger/api/gen.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.2/src/dagger/api/gen_sync.py` & `dagger_io-0.5.3/src/dagger/api/gen_sync.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.2/src/dagger/cli.py` & `dagger_io-0.5.3/src/dagger/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Optional
+from typing import Annotated, Optional
 
 import rich
 import typer
 from graphql import GraphQLSchema
 
 import dagger
 from dagger import codegen
@@ -14,22 +14,24 @@
 
 
 @app.callback()
 def main():
     """Dagger client."""
 
 
-output_opt = typer.Option(None, help="File to write generated code")
-sync_opt = typer.Option(False, help="Generate a client for sync code")
-
-
 @app.command()
 def generate(
-    output: Optional[Path] = output_opt,  # noqa: UP007
-    sync: bool = sync_opt,
+    output: Annotated[
+        Optional[Path],  # noqa: UP007
+        typer.Option(help="File to write generated code"),
+    ] = None,
+    sync: Annotated[
+        bool,
+        typer.Option(help="Generate a client for sync code"),
+    ] = False,
 ):
     """Generate a client for the Dagger API."""
     # not using `dagger.Connection` because codegen is
     # generating the client that it returns
 
     schema = _get_schema()
     code = codegen.generate(schema, sync)
```

### Comparing `dagger_io-0.5.2/src/dagger/codegen.py` & `dagger_io-0.5.3/src/dagger/codegen.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.2/src/dagger/config.py` & `dagger_io-0.5.3/src/dagger/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import pathlib
 import typing
+from os import PathLike
 
 import attrs
 import httpx
 
 
 @attrs.define
 class Config:
@@ -21,16 +21,16 @@
         The maximum time in seconds for establishing a connection to the server.
     execute_timeout:
         The maximum time in seconds for the execution of a request before an
         ExecuteTimeoutError is raised. Passing None results in waiting forever for a
         response (default).
     """
 
-    workdir: pathlib.Path | str = ""
-    config_path: pathlib.Path | str = ""
+    workdir: PathLike[str] | str = ""
+    config_path: PathLike[str] | str = ""
     log_output: typing.TextIO | None = None
     timeout: int = 10
     execute_timeout: int | float | None = None
 
 
 @attrs.define
 class ConnectParams:
```

### Comparing `dagger_io-0.5.2/src/dagger/connection.py` & `dagger_io-0.5.3/src/dagger/connection.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.2/src/dagger/context.py` & `dagger_io-0.5.3/src/dagger/context.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.2/src/dagger/engine/cli.py` & `dagger_io-0.5.3/src/dagger/engine/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         # See this golang issue (which itself links to bug reports in other
         # langs and the kernel): https://github.com/golang/go/issues/22315
         # Unfortunately, this sort of retry loop is the best workaround. The
         # case is obscure enough that it should not be hit very often at all.
         for _ in range(10):
             try:
                 proc = subprocess.Popen(
-                    args,
+                    args,  # noqa: S603
                     bufsize=0,
                     stdin=subprocess.PIPE,
                     stdout=subprocess.PIPE,
                     stderr=self.cfg.log_output or subprocess.PIPE,
                     encoding="utf-8",
                 )
             except OSError as e:
```

### Comparing `dagger_io-0.5.2/src/dagger/engine/conn.py` & `dagger_io-0.5.3/src/dagger/engine/conn.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.2/src/dagger/engine/download.py` & `dagger_io-0.5.3/src/dagger/engine/download.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.2/src/dagger/exceptions.py` & `dagger_io-0.5.3/src/dagger/exceptions.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.2/src/dagger/log.py` & `dagger_io-0.5.3/src/dagger/log.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.2/src/dagger/server/__init__.py` & `dagger_io-0.5.3/src/dagger/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.2/src/dagger/server/cli.py` & `dagger_io-0.5.3/src/dagger/server/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import logging
 import sys
+from typing import Annotated
 
 import anyio
 import typer
 
 from dagger.log import configure_logging
 
 from . import Server
 
 app = typer.Typer()
 
 
 @app.command()
 def main(
-    schema: bool = typer.Option(False, "-schema", help="Save schema to file and exit"),
+    schema: Annotated[
+        bool,
+        typer.Option("-schema", help="Save schema to file and exit"),
+    ] = False
 ):
     """Entrypoint for a dagger extension."""
     sys.path.insert(0, ".")
 
     try:
         from main import server
     except ImportError as e:
```

### Comparing `dagger_io-0.5.2/src/dagger/server/converter.py` & `dagger_io-0.5.3/src/dagger/server/converter.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.2/src/dagger/session.py` & `dagger_io-0.5.3/src/dagger/session.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.2/src/dagger/transport/httpx.py` & `dagger_io-0.5.3/src/dagger/transport/httpx.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.2/setup.py` & `dagger_io-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'typing_extensions>=4.4.0']
 
 extras_require = \
 {'server': ['strawberry-graphql>=0.133.5']}
 
 setup_kwargs = {
     'name': 'dagger-io',
-    'version': '0.5.2',
+    'version': '0.5.3',
     'description': 'A client package for running Dagger pipelines in Python.',
     'long_description': '# Dagger Python SDK\n\n[![PyPI Version](https://img.shields.io/pypi/v/dagger-io)](https://pypi.org/project/dagger-io/) \n[![Conda Version](https://img.shields.io/conda/vn/conda-forge/dagger-io.svg)](https://anaconda.org/conda-forge/dagger-io)\n[![Supported Python Versions](https://img.shields.io/pypi/pyversions/dagger-io.svg)](https://pypi.org/project/dagger-io/)\n[![License](https://img.shields.io/pypi/l/dagger-io.svg)](https://pypi.python.org/pypi/dagger-io)\n[![Code style](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)\n\nA client package for running [Dagger](https://dagger.io/) pipelines.\n\n## What is the Dagger Python SDK?\n\nThe Dagger Python SDK contains everything you need to develop CI/CD pipelines in Python, and run them on any OCI-compatible container runtime.\n\n## Requirements\n\n- Python 3.10 or later\n- [Docker](https://docs.docker.com/engine/install/), or another OCI-compatible container runtime\n\nA compatible version of the  [Dagger CLI](https://docs.dagger.io/cli) is automatically downloaded and run by the SDK for you, although it’s possible to manage it manually.\n\n## Installation\n\nFrom [PyPI](https://pypi.org/project/dagger-io/), using `pip`:\n\n```shell\npip install dagger-io\n```\n\nYou can also install via [Conda](https://anaconda.org/conda-forge/dagger-io), from the [conda-forge](https://conda-forge.org/docs/user/introduction.html#how-can-i-install-packages-from-conda-forge) channel:\n\n```shell\nconda install dagger-io\n```\n\n## Example\n\nCreate a `main.py` file:\n\n```python\nimport sys\n\nimport anyio\nimport dagger\n\n\nasync def main(args: list[str]):\n    async with dagger.Connection() as client:\n        # build container with cowsay entrypoint\n        ctr = (\n            client.container()\n            .from_("python:alpine")\n            .with_exec(["pip", "install", "cowsay"])\n            .with_entrypoint(["cowsay"])\n        )\n\n        # run cowsay with requested message\n        result = await ctr.with_exec(args).stdout()\n\n    print(result)\n\n\nanyio.run(main, sys.argv[1:])\n```\n\nRun with:\n\n```console\n$ python main.py "Simple is better than complex"\n  _____________________________\n| Simple is better than complex |\n  =============================\n                             \\\n                              \\\n                                ^__^\n                                (oo)\\_______\n                                (__)\\       )\\/\\\n                                    ||----w |\n                                    ||     ||\n```\n\n> **Note**\n> It may take a while for it to finish, especially on first run with cold cache.\n\nIf you need to debug, you can stream the logs from the engine with the `log_output`  config:\n\n```python\nconfig = dagger.Config(log_output=sys.stderr)\nasync with dagger.Connection(config) as client:\n    ...\n```\n\n## Learn more\n\n- [Documentation](https://docs.dagger.io/sdk/python)\n- [API Reference](https://dagger-io.readthedocs.org)\n- [Source code](https://github.com/dagger/dagger/tree/main/sdk/python)\n\n## Development\n\nThis library is maintained with [Poetry](https://python-poetry.org/docs/).\n\nIf you already have a [Python 3.10 or later](https://docs.python.org/3/using/index.html) interpreter in your `$PATH`, you can let [Poetry manage](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment) the [virtual environment](https://packaging.python.org/en/latest/tutorials/installing-packages/#creating-virtual-environments) automatically. Otherwise you need to activate it first, before installing dependencies:\n\n```shell\npoetry install\n```\n\nThe following commands are available:\n- `poe test`: Run tests.\n- `poe fmt`: Re-format code following common styling conventions.\n- `poe lint`: Check for linting violations.\n- `poe generate`: Regenerate API client after changes to the codegen.\n- `poe docs`: Build reference docs locally.\n\n### Engine changes\n\nTesting and regenerating the client may fail if there’s changes in the engine code that haven’t been released yet. \n\nThe simplest way to run those commands locally with the most updated engine version is to build it using [Dagger’s CI pipelines](https://github.com/dagger/dagger/blob/main/internal/mage/sdk/python.go) :\n\n```shell\n../../hack/make sdk:python:test\n../../hack/make sdk:python:generate\n```\n\nYou can also build the CLI and use it directly within the Python SDK:\n\n```shell\n../../hack/dev poe test\n```\n\nOr build it separately and tell the SDK to use it directly (or any other CLI binary):\n\n```shell\n../../hack/make\n_EXPERIMENTAL_DAGGER_CLI_BIN=../../bin/dagger poe test\n```\n\n',
     'author': 'Dagger',
     'author_email': 'hello@dagger.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://dagger.io',
```

### Comparing `dagger_io-0.5.2/PKG-INFO` & `dagger_io-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagger-io
-Version: 0.5.2
+Version: 0.5.3
 Summary: A client package for running Dagger pipelines in Python.
 Home-page: https://dagger.io
 License: Apache-2.0
 Author: Dagger
 Author-email: hello@dagger.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

