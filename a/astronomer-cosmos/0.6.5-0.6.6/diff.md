# Comparing `tmp/astronomer_cosmos-0.6.5.tar.gz` & `tmp/astronomer_cosmos-0.6.6.tar.gz`

## Comparing `astronomer_cosmos-0.6.5.tar` & `astronomer_cosmos-0.6.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/core/__init__.py
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/core/tests/test_airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/__init__.py
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/constants.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/dag.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/dataset.py
--rw-r--r--   0        0        0    10510 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/render.py
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/community/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/community/profiles/__init__.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/community/profiles/exasol.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/community/profiles/spark.py
--rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/community/profiles/trino.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/__init__.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/__init__.py
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/base.py
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/docker.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/kubernetes.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/lazy_load.py
--rw-r--r--   0        0        0     9359 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/local.py
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/tests/test_docker.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/tests/test_local.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/__init__.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/bigquery.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/databricks.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/postgres.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/redshift.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/snowflake.py
--rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/tests/test_profiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/__init__.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/profiles_generator.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/warn_parsing.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/parser/__init__.py
--rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/parser/project.py
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/parser/tests/test_project.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/tests/test_dataset.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/tests/test_export.py
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/tests/test_render.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/tests/test_version.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/LICENSE
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/README.rst
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/core/tests/test_airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/__init__.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/constants.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/dag.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/dataset.py
+-rw-r--r--   0        0        0    10510 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/render.py
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/community/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/community/profiles/__init__.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/community/profiles/exasol.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/community/profiles/spark.py
+-rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/community/profiles/trino.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/__init__.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/__init__.py
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/base.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/docker.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/kubernetes.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/lazy_load.py
+-rw-r--r--   0        0        0    11398 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/local.py
+-rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/tests/test_docker.py
+-rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/tests/test_local.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/__init__.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/bigquery.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/databricks.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/postgres.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/redshift.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/snowflake.py
+-rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/tests/test_profiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/__init__.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/profiles_generator.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/warn_parsing.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/parser/__init__.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/parser/project.py
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/parser/tests/test_project.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/tests/test_dataset.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/tests/test_export.py
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/tests/test_render.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/tests/test_version.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/LICENSE
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/README.rst
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/PKG-INFO
```

### Comparing `astronomer_cosmos-0.6.5/cosmos/core/airflow.py` & `astronomer_cosmos-0.6.6/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/core/graph/entities.py` & `astronomer_cosmos-0.6.6/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/core/tests/test_airflow.py` & `astronomer_cosmos-0.6.6/cosmos/core/tests/test_airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/__init__.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/dag.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/dag.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/render.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/render.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/task_group.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/task_group.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/community/profiles/exasol.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/community/profiles/exasol.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/community/profiles/spark.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/community/profiles/spark.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/community/profiles/trino.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/community/profiles/trino.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/__init__.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/base.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/docker.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/kubernetes.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/local.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/local.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 
 import logging
 import os
 import shutil
 import signal
 import tempfile
 from collections import namedtuple
+from pathlib import Path
 from typing import Callable, Optional, Sequence
 
 import yaml
 from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException, AirflowSkipException
 from airflow.utils.context import Context
+from airflow.utils.session import NEW_SESSION, provide_session
+from sqlalchemy.orm import Session
 
 from cosmos.providers.dbt.core.operators.base import DbtBaseOperator
 from cosmos.providers.dbt.core.utils.adapted_subprocesshook import (
     FullOutputSubprocessHook,
 )
 from cosmos.providers.dbt.core.utils.warn_parsing import (
     extract_log_issues,
@@ -32,22 +35,26 @@
 class DbtLocalBaseOperator(DbtBaseOperator):
     """
     Executes a dbt core cli command locally.
 
     :param install_deps: If true, install dependencies before running the command
     """
 
-    template_fields: Sequence[str] = DbtBaseOperator.template_fields
+    template_fields: Sequence[str] = DbtBaseOperator.template_fields + ("compiled_sql",)
+    template_fields_renderers = {
+        "compiled_sql": "sql",
+    }
 
     def __init__(
         self,
         install_deps: bool = False,
         **kwargs,
     ) -> None:
         self.install_deps = install_deps
+        self.compiled_sql = ""
         super().__init__(**kwargs)
 
     @cached_property
     def subprocess_hook(self):
         """Returns hook for running the bash command."""
         return FullOutputSubprocessHook()
 
@@ -57,18 +64,59 @@
                 f"dbt command returned exit code {self.skip_exit_code}. Skipping."
             )
         elif result.exit_code != 0:
             raise AirflowException(
                 f"dbt command failed. The command returned a non-zero exit code {result.exit_code}."
             )
 
+    @provide_session
+    def store_compiled_sql(
+        self, tmp_project_dir: str, context: Context, session: Session = NEW_SESSION
+    ) -> None:
+        """
+        Takes the compiled SQL files from the dbt run and stores them in the compiled_sql rendered template.
+        Gets called after every dbt run.
+        """
+        compiled_queries = {}
+        # dbt compiles sql files and stores them in the target directory
+        for root, _, files in os.walk(os.path.join(tmp_project_dir, "target")):
+            for file in files:
+                if not file.endswith(".sql"):
+                    continue
+
+                compiled_sql_path = Path(os.path.join(root, file))
+                compiled_sql = compiled_sql_path.read_text(encoding="utf-8")
+                compiled_queries[file] = compiled_sql.strip()
+
+        for name, query in compiled_queries.items():
+            self.compiled_sql += f"-- {name}\n{query}\n\n"
+
+        self.compiled_sql = self.compiled_sql.strip()
+
+        # need to refresh the rendered task field record in the db because Airflow only does this
+        # before executing the task, not after
+        from airflow.models.renderedtifields import RenderedTaskInstanceFields
+
+        ti = context["ti"]
+        ti.task.template_fields = self.template_fields
+        rtif = RenderedTaskInstanceFields(ti, render_templates=False)
+
+        # delete the old records
+        session.query(RenderedTaskInstanceFields).filter(
+            RenderedTaskInstanceFields.dag_id == self.dag_id,
+            RenderedTaskInstanceFields.task_id == self.task_id,
+            RenderedTaskInstanceFields.run_id == ti.run_id,
+        ).delete()
+        session.add(rtif)
+
     def run_command(
         self,
         cmd: list[str],
         env: dict[str, str],
+        context: Context,
     ) -> FullOutputSubprocessResult:
         """
         Copies the dbt project to a temporary directory and runs the command.
         """
         with tempfile.TemporaryDirectory() as tmp_dir:
             # need a subfolder because shutil.copytree will fail if the destination dir already exists
             tmp_project_dir = os.path.join(tmp_dir, "dbt_project")
@@ -90,22 +138,23 @@
                 command=cmd,
                 env=env,
                 output_encoding=self.output_encoding,
                 cwd=tmp_project_dir,
             )
 
             self.exception_handling(result)
+            self.store_compiled_sql(tmp_project_dir, context)
 
             return result
 
     def build_and_run_cmd(
         self, context: Context, cmd_flags: list[str] | None = None
     ) -> FullOutputSubprocessResult:
         dbt_cmd, env = self.build_cmd(context=context, cmd_flags=cmd_flags)
-        return self.run_command(cmd=dbt_cmd, env=env)
+        return self.run_command(cmd=dbt_cmd, env=env, context=context)
 
     def execute(self, context: Context) -> str:
         # TODO is this going to put loads of unnecessary stuff in to xcom?
         return self.build_and_run_cmd(context=context).output
 
     def on_kill(self) -> None:
         if self.cancel_query_on_kill:
```

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/tests/test_docker.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/tests/test_local.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/__init__.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/bigquery.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/bigquery.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/databricks.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/databricks.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/postgres.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/postgres.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/redshift.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/redshift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/snowflake.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/snowflake.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/tests/test_profiles.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/profiles_generator.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/profiles_generator.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/warn_parsing.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/warn_parsing.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/parser/project.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/parser/tests/test_project.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/parser/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/tests/test_dataset.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/tests/test_export.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/cosmos/providers/dbt/tests/test_render.py` & `astronomer_cosmos-0.6.6/cosmos/providers/dbt/tests/test_render.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,20 +21,19 @@
 
 def test_render_project_default():
     computed = render_project(
         dbt_project_name="jaffle_shop", dbt_root_path=DBT_PROJECT_PATH
     )
     assert isinstance(computed, Group)
     assert computed.id == "jaffle_shop"
-    assert len(computed.entities) == 9
+    assert len(computed.entities) == 8
     entities_ids = [entity.id for entity in computed.entities]
     expected_ids = [
         "customers",
         "orders",
-        "orders_snapshot_timestamp_snapshot",
         "raw_customers_seed",
         "raw_orders_seed",
         "raw_payments_seed",
         "stg_customers",
         "stg_orders",
         "stg_payments",
     ]
@@ -45,20 +44,19 @@
     computed = render_project(
         dbt_project_name="jaffle_shop",
         dbt_root_path=DBT_PROJECT_PATH,
         test_behavior="none",
     )
     assert isinstance(computed, Group)
     assert computed.id == "jaffle_shop"
-    assert len(computed.entities) == 9
+    assert len(computed.entities) == 8
     entities_ids = [entity.id for entity in computed.entities]
     expected_ids = [
         "customers_run",
         "orders_run",
-        "orders_snapshot_timestamp_snapshot",
         "raw_customers_seed",
         "raw_orders_seed",
         "raw_payments_seed",
         "stg_customers_run",
         "stg_orders_run",
         "stg_payments_run",
     ]
@@ -69,21 +67,20 @@
     computed = render_project(
         dbt_project_name="jaffle_shop",
         dbt_root_path=DBT_PROJECT_PATH,
         test_behavior="after_all",
     )
     assert isinstance(computed, Group)
     assert computed.id == "jaffle_shop"
-    assert len(computed.entities) == 10
+    assert len(computed.entities) == 9
     entities_ids = [entity.id for entity in computed.entities]
     expected_ids = [
         "customers_run",
         "jaffle_shop_test",
         "orders_run",
-        "orders_snapshot_timestamp_snapshot",
         "raw_customers_seed",
         "raw_orders_seed",
         "raw_payments_seed",
         "stg_customers_run",
         "stg_orders_run",
         "stg_payments_run",
     ]
@@ -130,18 +127,17 @@
 
 def test_render_project_select_models_by_excluding_path():
     computed = render_project(
         dbt_project_name="jaffle_shop",
         dbt_root_path=DBT_PROJECT_PATH,
         exclude={"paths": ["models/staging/"]},
     )
-    assert len(computed.entities) == 6
+    assert len(computed.entities) == 5
     entities_ids = [entity.id for entity in computed.entities]
     expected_ids = [
         "customers",
         "orders",
-        "orders_snapshot_timestamp_snapshot",
         "raw_customers_seed",
         "raw_orders_seed",
         "raw_payments_seed",
     ]
     assert sorted(entities_ids) == expected_ids
```

### Comparing `astronomer_cosmos-0.6.5/.gitignore` & `astronomer_cosmos-0.6.6/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
-reference/_generated/
+docs/reference/_generated/
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `astronomer_cosmos-0.6.5/LICENSE` & `astronomer_cosmos-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/README.rst` & `astronomer_cosmos-0.6.6/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/pyproject.toml` & `astronomer_cosmos-0.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.5/PKG-INFO` & `astronomer_cosmos-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-cosmos
-Version: 0.6.5
+Version: 0.6.6
 Summary: Render 3rd party workflows in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags,dbt
```

