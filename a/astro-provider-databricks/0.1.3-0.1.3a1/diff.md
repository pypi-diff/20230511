# Comparing `tmp/astro_provider_databricks-0.1.3.tar.gz` & `tmp/astro_provider_databricks-0.1.3a1.tar.gz`

## Comparing `astro_provider_databricks-0.1.3.tar` & `astro_provider_databricks-0.1.3a1.tar`

### file list

```diff
@@ -1,65 +1,68 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.deepsource.toml
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/CHANGELOG.rst
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/Tiltfile
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/codecov.yml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/mlc-config.json
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/noxfile.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/yamllint-config.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.github/CODEOWNERS
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.github/ci-test-connections.yaml
--rwxr-xr-x   0        0        0      696 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.github/scripts/verify_tag_and_version.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.github/workflows/astro-deploy.yml
--rw-r--r--   0        0        0     6610 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.github/workflows/docs.yml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.github/workflows/mlc_config.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/dev/.dockerignore
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/dev/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/dev/Dockerfile
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/dev/docker-compose.yaml
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/dev/packages.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/dev/requirements.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/dev/.astro/config.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/Makefile
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/conf.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/contributing.rst
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/index.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/make.bat
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/requirements.txt
--rw-r--r--   0        0        0   737260 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/banner.png
--rw-r--r--   0        0        0   146128 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/dbt_dag.png
--rw-r--r--   0        0        0   361967 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/dbt_task_group.png
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/logo-dark.png
--rw-r--r--   0        0        0    11220 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/logo-light.png
--rw-r--r--   0        0        0    80206 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/connections_doc/bigquery_airflow_connection.png
--rw-r--r--   0        0        0    82236 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/connections_doc/databricks_airflow_connection.png
--rw-r--r--   0        0        0    72389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/connections_doc/postgres_airflow_connection.png
--rw-r--r--   0        0        0    75178 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/connections_doc/redshift_airflow_connection.png
--rw-r--r--   0        0        0   108877 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/connections_doc/snowflake_airflow_connection.png
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/_static/css/custom.css
--rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/assets/images/dbutils-notebook-success.png
--rw-r--r--   0        0        0    73030 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/assets/images/repair-all-failed.png
--rw-r--r--   0        0        0   140389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/docs/assets/images/repair-single-failed.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/astro_databricks/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/astro_databricks/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/astro_databricks/operators/__init__.py
--rw-r--r--   0        0        0    12957 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/astro_databricks/operators/notebook.py
--rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/astro_databricks/operators/workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/astro_databricks/plugins/__init__.py
--rw-r--r--   0        0        0    17286 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/astro_databricks/plugins/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/pytest.ini
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/test_example_dags.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/databricks/__init__.py
--rw-r--r--   0        0        0    14882 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/databricks/test_notebook.py
--rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/databricks/test_plugin.py
--rw-r--r--   0        0        0    10682 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/tests/databricks/test_workflow.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/LICENSE
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/README.md
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    10055 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/.deepsource.toml
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/CHANGELOG.rst
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/Tiltfile
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/codecov.yml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/mlc-config.json
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/noxfile.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/yamllint-config.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/.github/ci-test-connections.yaml
+-rwxr-xr-x   0        0        0      696 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/.github/scripts/verify_tag_and_version.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/.github/workflows/astro-deploy.yml
+-rw-r--r--   0        0        0     7449 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/.github/workflows/mlc_config.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/dev/.dockerignore
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/dev/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/dev/Dockerfile
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/dev/docker-compose.yaml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/dev/packages.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/dev/requirements.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/dev/.astro/config.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/Makefile
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/conf.py
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/contributing.rst
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/index.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/make.bat
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/requirements.txt
+-rw-r--r--   0        0        0   737260 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/_static/banner.png
+-rw-r--r--   0        0        0   146128 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/_static/dbt_dag.png
+-rw-r--r--   0        0        0   361967 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/_static/dbt_task_group.png
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/_static/logo-dark.png
+-rw-r--r--   0        0        0    11220 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/_static/logo-light.png
+-rw-r--r--   0        0        0    80206 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/_static/connections_doc/bigquery_airflow_connection.png
+-rw-r--r--   0        0        0    82236 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/_static/connections_doc/databricks_airflow_connection.png
+-rw-r--r--   0        0        0    72389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/_static/connections_doc/postgres_airflow_connection.png
+-rw-r--r--   0        0        0    75178 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/_static/connections_doc/redshift_airflow_connection.png
+-rw-r--r--   0        0        0   108877 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/_static/connections_doc/snowflake_airflow_connection.png
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/_static/css/custom.css
+-rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/assets/images/dbutils-notebook-success.png
+-rw-r--r--   0        0        0    73030 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/assets/images/repair-all-failed.png
+-rw-r--r--   0        0        0   140389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/docs/assets/images/repair-single-failed.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/example_dags/.airflowignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/example_dags/__init__.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/example_dags/example_databricks_notebook.py
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/example_dags/example_databricks_workflow.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/astro_databricks/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/astro_databricks/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/astro_databricks/operators/__init__.py
+-rw-r--r--   0        0        0    12957 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/astro_databricks/operators/notebook.py
+-rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/astro_databricks/operators/workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/astro_databricks/plugins/__init__.py
+-rw-r--r--   0        0        0    17286 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/astro_databricks/plugins/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/tests/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/tests/conftest.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/tests/pytest.ini
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/tests/test_example_dags.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/tests/databricks/__init__.py
+-rw-r--r--   0        0        0    14882 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/tests/databricks/test_notebook.py
+-rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/tests/databricks/test_plugin.py
+-rw-r--r--   0        0        0    10682 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/tests/databricks/test_workflow.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/LICENSE
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/README.md
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/pyproject.toml
+-rw-r--r--   0        0        0    10065 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a1/PKG-INFO
```

### Comparing `astro_provider_databricks-0.1.3/.pre-commit-config.yaml` & `astro_provider_databricks-0.1.3a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/CHANGELOG.rst` & `astro_provider_databricks-0.1.3a1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/CODE_OF_CONDUCT.md` & `astro_provider_databricks-0.1.3a1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/Tiltfile` & `astro_provider_databricks-0.1.3a1/Tiltfile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/noxfile.py` & `astro_provider_databricks-0.1.3a1/noxfile.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/.github/scripts/verify_tag_and_version.py` & `astro_provider_databricks-0.1.3a1/.github/scripts/verify_tag_and_version.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/.github/workflows/astro-deploy.yml` & `astro_provider_databricks-0.1.3a1/.github/workflows/astro-deploy.yml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/.github/workflows/ci.yml` & `astro_provider_databricks-0.1.3a1/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 env:
   AIRFLOW__CORE__ALLOWED_DESERIALIZATION_CLASSES: "airflow.* astro.* astro_databricks.*"
   CI_ENABLED: true
 
 jobs:
   Markdown-Link-Check:
-    if: github.event.action != 'labeled'
+    #if: github.event.action != 'labeled'
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: gaurav-nelson/github-action-markdown-link-check@v1
         with:
           config-file: '.github/workflows/mlc_config.json'
 
@@ -51,156 +51,179 @@
 #          path: |
 #            ~/.cache/pip
 #            .nox
 #          key: ${{ runner.os }}-${{ hashFiles('pyproject.toml') }}
 #      - run: pip3 install nox
 #      - run: nox -s type_check
 
-  Build-Docs:
-    if: github.event.action != 'labeled'
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v3
-        with:
-          python-version: '3.9'
-          architecture: 'x64'
-      - uses: actions/cache@v3
-        with:
-          path: |
-            ~/.cache/pip
-            .nox
-          key: ${{ runner.os }}-${{ hashFiles('pyproject.toml') }}
-      - run: pip3 install nox
-      - run: nox -s build_docs
-
-  Run-Unit-Tests:
-    strategy:
-      fail-fast: false
-      matrix:
-        python: [ '3.8', '3.9', '3.10' ]
-        airflow: [ 2.5 ]
-    if: >-
-      github.event_name == 'push' ||
-      (
-        github.event_name == 'pull_request' &&
-        github.event.pull_request.head.repo.fork == false
-      ) ||
-      (
-        github.event_name == 'pull_request_target' &&
-        contains(github.event.pull_request.labels.*.name, 'safe to test')
-      ) ||
-      (
-        github.event_name == 'release'
-      )
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
-        if: github.event_name != 'pull_request_target'
-
-      - name: Checkout pull/${{ github.event.number }}
-        uses: actions/checkout@v3
-        with:
-          ref: ${{ github.event.pull_request.head.sha }}
-        if: github.event_name == 'pull_request_target'
-      - uses: actions/setup-python@v3
-        with:
-          python-version: ${{ matrix.python }}
-          architecture: 'x64'
-      - uses: actions/cache@v3
-        with:
-          path: |
-            ~/.cache/pip
-            .nox
-          key: unit-tests-os-${{ runner.os }}-python-${{ matrix.python }}-airflow-${{ matrix.airflow }}-deps-${{ hashFiles('pyproject.toml') }}-version-${{ hashFiles('src/astro_databricks/__init__.py') }}
-      - run: pip3 install nox
-      - run: nox -s "test-${{ matrix.python }}(airflow='${{ matrix.airflow }}')" -- --ignore "tests/test_example_dags.py" --cov-report=xml
-      - name: Upload coverage
-        uses: actions/upload-artifact@v2
-        with:
-          name: coverage-unit-tests-${{ matrix.python }}-${{ matrix.airflow }}
-          path: ./.coverage
-
-  Run-Example-DAGs:
-    strategy:
-      fail-fast: false
-      matrix:
-        python: [ '3.8', '3.9', '3.10' ]
-        airflow: [ '2.2.4', '2.3', '2.4', '2.5' ]
-
-    if: >-
-      github.event_name == 'push' ||
-      (
-        github.event_name == 'pull_request' &&
-        github.event.pull_request.head.repo.fork == false
-      ) ||
-      (
-        github.event_name == 'pull_request_target' &&
-        contains(github.event.pull_request.labels.*.name, 'safe to test')
-      )||
-      (
-        github.event_name == 'release'
-      )
+#  Build-Docs:
+#    if: github.event.action != 'labeled'
+#    runs-on: ubuntu-latest
+#    steps:
+#      - uses: actions/checkout@v3
+#      - uses: actions/setup-python@v3
+#        with:
+#          python-version: '3.9'
+#          architecture: 'x64'
+#      - uses: actions/cache@v3
+#        with:
+#          path: |
+#            ~/.cache/pip
+#            .nox
+#          key: ${{ runner.os }}-${{ hashFiles('pyproject.toml') }}
+#      - run: pip3 install nox
+#      - run: nox -s build_docs
+#
+#  Run-Unit-Tests:
+#    strategy:
+#      fail-fast: false
+#      matrix:
+#        python: [ '3.8', '3.9', '3.10' ]
+#        airflow: [ 2.5 ]
+#    if: >-
+#      github.event_name == 'push' ||
+#      (
+#        github.event_name == 'pull_request' &&
+#        github.event.pull_request.head.repo.fork == false
+#      ) ||
+#      (
+#        github.event_name == 'pull_request_target' &&
+#        contains(github.event.pull_request.labels.*.name, 'safe to test')
+#      ) ||
+#      (
+#        github.event_name == 'release'
+#      )
+#    runs-on: ubuntu-latest
+#    steps:
+#      - uses: actions/checkout@v3
+#        if: github.event_name != 'pull_request_target'
+#
+#      - name: Checkout pull/${{ github.event.number }}
+#        uses: actions/checkout@v3
+#        with:
+#          ref: ${{ github.event.pull_request.head.sha }}
+#        if: github.event_name == 'pull_request_target'
+#      - uses: actions/setup-python@v3
+#        with:
+#          python-version: ${{ matrix.python }}
+#          architecture: 'x64'
+#      - uses: actions/cache@v3
+#        with:
+#          path: |
+#            ~/.cache/pip
+#            .nox
+#          key: unit-tests-os-${{ runner.os }}-python-${{ matrix.python }}-airflow-${{ matrix.airflow }}-deps-${{ hashFiles('pyproject.toml') }}-version-${{ hashFiles('src/astro_databricks/__init__.py') }}
+#      - run: pip3 install nox
+#      - run: nox -s "test-${{ matrix.python }}(airflow='${{ matrix.airflow }}')" -- --ignore "tests/test_example_dags.py" --cov-report=xml
+#      - name: Upload coverage
+#        uses: actions/upload-artifact@v2
+#        with:
+#          name: coverage-unit-tests-${{ matrix.python }}-${{ matrix.airflow }}
+#          path: ./.coverage
+#
+#  Run-Example-DAGs:
+#    strategy:
+#      fail-fast: false
+#      matrix:
+#        python: [ '3.8', '3.9', '3.10' ]
+#        airflow: [ '2.2.4', '2.3', '2.4', '2.5' ]
+#
+#    if: >-
+#      github.event_name == 'push' ||
+#      (
+#        github.event_name == 'pull_request' &&
+#        github.event.pull_request.head.repo.fork == false
+#      ) ||
+#      (
+#        github.event_name == 'pull_request_target' &&
+#        contains(github.event.pull_request.labels.*.name, 'safe to test')
+#      )||
+#      (
+#        github.event_name == 'release'
+#      )
+#    runs-on: ubuntu-latest
+#    steps:
+#      - uses: actions/checkout@v3
+#        if: github.event_name != 'pull_request_target'
+#
+#      - name: Checkout pull/${{ github.event.number }}
+#        uses: actions/checkout@v3
+#        with:
+#          ref: ${{ github.event.pull_request.head.sha }}
+#        if: github.event_name == 'pull_request_target'
+#
+#      - uses: actions/setup-python@v3
+#        with:
+#          python-version: ${{ matrix.python }}
+#          architecture: 'x64'
+#      - uses: actions/cache@v3
+#        with:
+#          path: |
+#            ~/.cache/pip
+#            .nox
+#          key: example-dags-os-${{ runner.os }}-python-${{ matrix.python }}-airflow-${{ matrix.airflow }}-deps-${{ hashFiles('pyproject.toml') }}-version-${{ hashFiles('src/astro_databricks/__init__.py') }}
+#      - run: cat .github/ci-test-connections.yaml > test-connections.yaml
+#      - run: sqlite3 /tmp/sqlite_default.db "VACUUM;"
+#      - run: pip3 install nox
+#      - run: DATABRICKS_GROUP_ID="${{github.run_id}}_${{matrix.python}}_${{matrix.airflow}}" nox -s "test-${{ matrix.python }}(airflow='${{ matrix.airflow }}')" -- "tests/test_example_dags.py" --cov-report=xml
+#      - name: Upload coverage
+#        uses: actions/upload-artifact@v2
+#        with:
+#          name: coverage-example-dags-${{ matrix.python }}-${{ matrix.airflow }}
+#          path: ./.coverage
+#    env:
+#      DATABRICKS_CONN_TOKEN: ${{ secrets.DATABRICKS_CONN_TOKEN }}
+#      DATABRICKS_CONN_HOST: https://dbc-9c390870-65ef.cloud.databricks.com/
+#
+#  Code-Coverage:
+#    if: github.event.action != 'labeled'
+#    needs:
+#      - Run-Unit-Tests
+#      - Run-Example-DAGs
+#    runs-on: ubuntu-latest
+#    steps:
+#      - uses: actions/checkout@v3
+#      - name: Set up Python 3.8
+#        uses: actions/setup-python@v3
+#        with:
+#          python-version: 3.8
+#      - name: Install coverage
+#        run: |
+#          pip3 install coverage
+#      - name: Download all artifacts
+#        uses: actions/download-artifact@v2
+#        with:
+#          path: ./coverage
+#      - name: Run coverage
+#        run: |
+#          coverage combine ./coverage/coverage*/.coverage
+#          coverage report
+#          coverage xml
+#      - name: Upload coverage
+#        uses: codecov/codecov-action@v2
+#        with:
+#          fail_ci_if_error: true
+#          token: ${{ secrets.CODECOV_TOKEN }}
+#          files: ./coverage.xml
+
+  Publish-Package:
+    #if: github.event_name == 'release'
+    name: Build and publish Python 🐍 distributions 📦 to PyPI
+      #    needs:
+      #      - Markdown-Link-Check
+      #      - Build-Docs
+      #      - Run-Unit-Tests
+      #      - Run-Example-DAGs
+      #      - Code-Coverage
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
-        if: github.event_name != 'pull_request_target'
-
-      - name: Checkout pull/${{ github.event.number }}
-        uses: actions/checkout@v3
-        with:
-          ref: ${{ github.event.pull_request.head.sha }}
-        if: github.event_name == 'pull_request_target'
-
-      - uses: actions/setup-python@v3
-        with:
-          python-version: ${{ matrix.python }}
-          architecture: 'x64'
-      - uses: actions/cache@v3
-        with:
-          path: |
-            ~/.cache/pip
-            .nox
-          key: example-dags-os-${{ runner.os }}-python-${{ matrix.python }}-airflow-${{ matrix.airflow }}-deps-${{ hashFiles('pyproject.toml') }}-version-${{ hashFiles('src/astro_databricks/__init__.py') }}
-      - run: cat .github/ci-test-connections.yaml > test-connections.yaml
-      - run: sqlite3 /tmp/sqlite_default.db "VACUUM;"
-      - run: pip3 install nox
-      - run: DATABRICKS_GROUP_ID="${{github.run_id}}_${{matrix.python}}_${{matrix.airflow}}" nox -s "test-${{ matrix.python }}(airflow='${{ matrix.airflow }}')" -- "tests/test_example_dags.py" --cov-report=xml
-      - name: Upload coverage
-        uses: actions/upload-artifact@v2
-        with:
-          name: coverage-example-dags-${{ matrix.python }}-${{ matrix.airflow }}
-          path: ./.coverage
+    - uses: actions/checkout@v2
+    - uses: actions/setup-python@v2
+      with:
+        python-version: '3.8'
+        architecture: 'x64'
+    - run: pip3 install hatch
+    - run: hatch build
+    - run: hatch publish -u __token__ -a ${{ secrets.PYPI_TOKEN }} -y
     env:
-      DATABRICKS_CONN_TOKEN: ${{ secrets.DATABRICKS_CONN_TOKEN }}
-      DATABRICKS_CONN_HOST: https://dbc-9c390870-65ef.cloud.databricks.com/
-
-  Code-Coverage:
-    if: github.event.action != 'labeled'
-    needs:
-      - Run-Unit-Tests
-      - Run-Example-DAGs
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
-      - name: Set up Python 3.8
-        uses: actions/setup-python@v3
-        with:
-          python-version: 3.8
-      - name: Install coverage
-        run: |
-          pip3 install coverage
-      - name: Download all artifacts
-        uses: actions/download-artifact@v2
-        with:
-          path: ./coverage
-      - name: Run coverage
-        run: |
-          coverage combine ./coverage/coverage*/.coverage
-          coverage report
-          coverage xml
-      - name: Upload coverage
-        uses: codecov/codecov-action@v2
-        with:
-          fail_ci_if_error: true
-          token: ${{ secrets.CODECOV_TOKEN }}
-          files: ./coverage.xml
+      HATCH_INDEX_USER: __token__
+      HATCH_INDEX_AUTH: ${{ secrets.PYPI_TOKEN }}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `astro_provider_databricks-0.1.3/.github/workflows/docs.yml` & `astro_provider_databricks-0.1.3a1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/dev/Dockerfile` & `astro_provider_databricks-0.1.3a1/dev/Dockerfile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/dev/docker-compose.yaml` & `astro_provider_databricks-0.1.3a1/dev/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/docs/Makefile` & `astro_provider_databricks-0.1.3a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/docs/conf.py` & `astro_provider_databricks-0.1.3a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/docs/contributing.rst` & `astro_provider_databricks-0.1.3a1/docs/contributing.rst`

 * *Files 19% similar despite different names*

```diff
@@ -88,7 +88,22 @@
     hatch version minor
 
 
 hatch will automatically update the version for you. Then, create a new release on GitHub with the new version. The release will be automatically deployed to PyPI.
 
 .. note::
     You can update the version in a few different ways. Check out the `hatch docs <https://hatch.pypa.io/latest/version/#updating>`_ to learn more.
+
+
+To validate a release locally, it is possible to build it using:
+
+.. code-block:: bash
+
+    hatch build
+
+To publish a release to PyPI, use:
+
+.. code-block:: bash
+
+    hatch publish
+
+
```

### Comparing `astro_provider_databricks-0.1.3/docs/index.rst` & `astro_provider_databricks-0.1.3a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/docs/make.bat` & `astro_provider_databricks-0.1.3a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/docs/_static/banner.png` & `astro_provider_databricks-0.1.3a1/docs/_static/banner.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/docs/_static/dbt_dag.png` & `astro_provider_databricks-0.1.3a1/docs/_static/dbt_dag.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/docs/_static/dbt_task_group.png` & `astro_provider_databricks-0.1.3a1/docs/_static/dbt_task_group.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/docs/_static/logo-dark.png` & `astro_provider_databricks-0.1.3a1/docs/_static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/docs/_static/logo-light.png` & `astro_provider_databricks-0.1.3a1/docs/_static/logo-light.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/docs/_static/connections_doc/bigquery_airflow_connection.png` & `astro_provider_databricks-0.1.3a1/docs/_static/connections_doc/bigquery_airflow_connection.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/docs/_static/connections_doc/databricks_airflow_connection.png` & `astro_provider_databricks-0.1.3a1/docs/_static/connections_doc/databricks_airflow_connection.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/docs/_static/connections_doc/postgres_airflow_connection.png` & `astro_provider_databricks-0.1.3a1/docs/_static/connections_doc/postgres_airflow_connection.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/docs/_static/connections_doc/redshift_airflow_connection.png` & `astro_provider_databricks-0.1.3a1/docs/_static/connections_doc/redshift_airflow_connection.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/docs/_static/connections_doc/snowflake_airflow_connection.png` & `astro_provider_databricks-0.1.3a1/docs/_static/connections_doc/snowflake_airflow_connection.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/docs/assets/images/dbutils-notebook-success.png` & `astro_provider_databricks-0.1.3a1/docs/assets/images/dbutils-notebook-success.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/docs/assets/images/repair-all-failed.png` & `astro_provider_databricks-0.1.3a1/docs/assets/images/repair-all-failed.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/docs/assets/images/repair-single-failed.png` & `astro_provider_databricks-0.1.3a1/docs/assets/images/repair-single-failed.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/astro_databricks/operators/notebook.py` & `astro_provider_databricks-0.1.3a1/astro_databricks/operators/notebook.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/astro_databricks/operators/workflow.py` & `astro_provider_databricks-0.1.3a1/astro_databricks/operators/workflow.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/astro_databricks/plugins/plugin.py` & `astro_provider_databricks-0.1.3a1/astro_databricks/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/tests/conftest.py` & `astro_provider_databricks-0.1.3a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/tests/test_example_dags.py` & `astro_provider_databricks-0.1.3a1/tests/test_example_dags.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/tests/utils.py` & `astro_provider_databricks-0.1.3a1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/tests/databricks/test_notebook.py` & `astro_provider_databricks-0.1.3a1/tests/databricks/test_notebook.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/tests/databricks/test_plugin.py` & `astro_provider_databricks-0.1.3a1/tests/databricks/test_plugin.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/tests/databricks/test_workflow.py` & `astro_provider_databricks-0.1.3a1/tests/databricks/test_workflow.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/.gitignore` & `astro_provider_databricks-0.1.3a1/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/LICENSE` & `astro_provider_databricks-0.1.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/README.md` & `astro_provider_databricks-0.1.3a1/README.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3/pyproject.toml` & `astro_provider_databricks-0.1.3a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "apache-airflow>=2.2.4",
     "databricks-sql-connector>=2.0.4;python_version>='3.10'",
-    "databricks-cli",
+    "databricks-cli>=0.17.7",
     "apache-airflow-providers-databricks>=2.2.0",
     "mergedeep"
 ]
 
 [project.optional-dependencies]
 docs =[
     "pydata_sphinx_theme",
```

### Comparing `astro_provider_databricks-0.1.3/PKG-INFO` & `astro_provider_databricks-0.1.3a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-provider-databricks
-Version: 0.1.3
+Version: 0.1.3a1
 Summary: Affordable Databricks Workflows in Apache Airflow
 Project-URL: Homepage, https://github.com/astronomer/astro-provider-databricks/
 Project-URL: Documentation, https://github.com/astronomer/astro-provider-databricks/
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Requires-Dist: apache-airflow-providers-databricks>=2.2.0
 Requires-Dist: apache-airflow>=2.2.4
-Requires-Dist: databricks-cli
+Requires-Dist: databricks-cli>=0.17.7
 Requires-Dist: databricks-sql-connector>=2.0.4; python_version >= '3.10'
 Requires-Dist: mergedeep
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-autobuild; extra == 'docs'
 Requires-Dist: sphinx-tabs; extra == 'docs'
```

