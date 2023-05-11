# Comparing `tmp/mitzu-0.6.0rc6.tar.gz` & `tmp/mitzu-0.6.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitzu-0.6.0rc6.tar", max compression
+gzip compressed data, was "mitzu-0.6.0rc7.tar", max compression
```

## Comparing `mitzu-0.6.0rc6.tar` & `mitzu-0.6.0rc7.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1082 2023-05-06 19:51:27.994575 mitzu-0.6.0rc6/LICENSE.txt
--rw-r--r--   0        0        0     2235 2023-05-06 19:51:27.994575 mitzu-0.6.0rc6/README.md
--rw-r--r--   0        0        0     6148 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/.DS_Store
--rw-r--r--   0        0        0      865 2023-05-06 19:52:36.707001 mitzu-0.6.0rc6/mitzu/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/__init__.py
--rw-r--r--   0        0        0     1762 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/adapter_factory.py
--rw-r--r--   0        0        0     5234 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/athena_adapter.py
--rw-r--r--   0        0        0     6072 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/databricks_adapter.py
--rw-r--r--   0        0        0     2261 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/file_adapter.py
--rw-r--r--   0        0        0     2563 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/generic_adapter.py
--rw-r--r--   0        0        0      898 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/helper.py
--rw-r--r--   0        0        0     3422 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/mysql_adapter.py
--rw-r--r--   0        0        0     2297 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/postgresql_adapter.py
--rw-r--r--   0        0        0     4085 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/redshift_adapter.py
--rw-r--r--   0        0        0     3344 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/snowflake_adapter.py
--rw-r--r--   0        0        0        0 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      660 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/__init__.py
--rw-r--r--   0        0        0      701 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5071 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6415 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
--rw-r--r--   0        0        0     9751 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1844 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
--rw-r--r--   0        0        0      672 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/__init__.py
--rw-r--r--   0        0        0      713 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5010 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6601 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
--rw-r--r--   0        0        0    10073 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1848 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
--rw-r--r--   0        0        0    39764 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy_adapter.py
--rw-r--r--   0        0        0     5009 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlite_adapter.py
--rw-r--r--   0        0        0     6687 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/trino_adapter.py
--rw-r--r--   0        0        0     1835 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/helper.py
--rw-r--r--   0        0        0    53852 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/model.py
--rw-r--r--   0        0        0        0 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/notebook/__init__.py
--rw-r--r--   0        0        0     6818 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/notebook/model_loader.py
--rw-r--r--   0        0        0     5424 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/project_discovery.py
--rw-r--r--   0        0        0     2102 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/project_serialization.py
--rw-r--r--   0        0        0      785 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/samples/__init__.py
--rw-r--r--   0        0        0     3794 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/samples/data_ingestion.py
--rw-r--r--   0        0        0    10141 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/samples/sample_data_generator.py
--rw-r--r--   0        0        0    11926 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/serialization.py
--rw-r--r--   0        0        0        0 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/__init__.py
--rw-r--r--   0        0        0     7022 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/charts.py
--rw-r--r--   0        0        0     1866 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/common.py
--rw-r--r--   0        0        0      941 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/labels.py
--rw-r--r--   0        0        0     7802 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/plot.py
--rw-r--r--   0        0        0     5767 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/titles.py
--rw-r--r--   0        0        0     3181 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/tooltips.py
--rw-r--r--   0        0        0     3339 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/transform_conv.py
--rw-r--r--   0        0        0     1278 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/transform_retention.py
--rw-r--r--   0        0        0     6148 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/webapp/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/webapp/__init__.py
--rw-r--r--   0        0        0     5347 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/webapp/assets/explore_page.css
--rw-r--r--   0        0        0   147145 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/favicon.ico
--rw-r--r--   0        0        0    46702 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/logo.png
--rw-r--r--   0        0        0    43472 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/mitzu-logo-light.svg
--rw-r--r--   0        0        0    49422 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/athena.png
--rw-r--r--   0        0        0    10321 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/clickhouse.png
--rw-r--r--   0        0        0   119554 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/databricks.png
--rw-r--r--   0        0        0     3008 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/mysql.png
--rw-r--r--   0        0        0     2446 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/pandas.png
--rw-r--r--   0        0        0     5338 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/postgresql.png
--rw-r--r--   0        0        0     8512 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/redshift.png
--rw-r--r--   0        0        0    93500 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/snowflake.png
--rw-r--r--   0        0        0    48681 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/sqlite.png
--rw-r--r--   0        0        0    34219 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/trino.png
--rw-r--r--   0        0        0    13737 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/auth/authorizer.py
--rw-r--r--   0        0        0     3557 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/auth/cognito.py
--rw-r--r--   0        0        0     1594 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/auth/decorator.py
--rw-r--r--   0        0        0     2777 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/auth/google.py
--rw-r--r--   0        0        0     7481 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/cache.py
--rw-r--r--   0        0        0     2966 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/caching_dataset_adapter.py
--rw-r--r--   0        0        0     1403 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/configs.py
--rw-r--r--   0        0        0     3088 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/dependencies.py
--rw-r--r--   0        0        0     4833 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/helper.py
--rw-r--r--   0        0        0     8375 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/model.py
--rw-r--r--   0        0        0      408 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/navbar.py
--rw-r--r--   0        0        0     5802 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/offcanvas.py
--rw-r--r--   0        0        0        0 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/connections/__init__.py
--rw-r--r--   0        0        0    15464 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/connections/manage_connections_component.py
--rw-r--r--   0        0        0     4527 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/connections_page.py
--rw-r--r--   0        0        0        0 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/dashboards/__init__.py
--rw-r--r--   0        0        0    21140 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
--rw-r--r--   0        0        0     9846 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/dashboards.py
--rw-r--r--   0        0        0    14654 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/edit_user.py
--rw-r--r--   0        0        0        0 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/__init__.py
--rw-r--r--   0        0        0     5724 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/complex_segment_handler.py
--rw-r--r--   0        0        0     6488 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/dates_selector_handler.py
--rw-r--r--   0        0        0     5564 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/event_segment_handler.py
--rw-r--r--   0        0        0    21781 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/explore_page.py
--rw-r--r--   0        0        0     9604 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/graph_handler.py
--rw-r--r--   0        0        0    10940 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/metric_config_handler.py
--rw-r--r--   0        0        0     2375 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/metric_segments_handler.py
--rw-r--r--   0        0        0     1565 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/metric_type_handler.py
--rw-r--r--   0        0        0     9783 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/simple_segment_handler.py
--rw-r--r--   0        0        0     4644 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/toolbar_handler.py
--rw-r--r--   0        0        0     1347 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore_project.py
--rw-r--r--   0        0        0     1751 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/home.py
--rw-r--r--   0        0        0     4107 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/login.py
--rw-r--r--   0        0        0     5027 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/manage_connection.py
--rw-r--r--   0        0        0     1315 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/manage_dashboard.py
--rw-r--r--   0        0        0    10191 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/manage_event_defs.py
--rw-r--r--   0        0        0    11849 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/manage_project.py
--rw-r--r--   0        0        0     9629 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/manage_saved_metrics.py
--rw-r--r--   0        0        0     1738 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/paths.py
--rw-r--r--   0        0        0        0 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/projects/__init__.py
--rw-r--r--   0        0        0    36159 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/projects/event_tables_config.py
--rw-r--r--   0        0        0      587 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/projects/helper.py
--rw-r--r--   0        0        0     9400 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/projects/manage_project_component.py
--rw-r--r--   0        0        0     5155 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/projects_page.py
--rw-r--r--   0        0        0     3185 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/users.py
--rw-r--r--   0        0        0        0 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/service/__init__.py
--rw-r--r--   0        0        0     2207 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/service/events_service.py
--rw-r--r--   0        0        0     5302 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/service/navbar_service.py
--rw-r--r--   0        0        0      670 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/service/notification_service.py
--rw-r--r--   0        0        0     2105 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/service/secret_service.py
--rw-r--r--   0        0        0     4719 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/service/user_service.py
--rw-r--r--   0        0        0    21352 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/storage.py
--rw-r--r--   0        0        0    25830 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/storage_model.py
--rw-r--r--   0        0        0     4625 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/webapp.py
--rw-r--r--   0        0        0     2943 2023-05-06 19:52:36.707001 mitzu-0.6.0rc6/pyproject.toml
--rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 mitzu-0.6.0rc6/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-11 19:37:51.874891 mitzu-0.6.0rc7/LICENSE.txt
+-rw-r--r--   0        0        0     2235 2023-05-11 19:37:51.874891 mitzu-0.6.0rc7/README.md
+-rw-r--r--   0        0        0     6148 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/.DS_Store
+-rw-r--r--   0        0        0      865 2023-05-11 19:38:51.574270 mitzu-0.6.0rc7/mitzu/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/__init__.py
+-rw-r--r--   0        0        0     1762 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/adapter_factory.py
+-rw-r--r--   0        0        0     5234 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/athena_adapter.py
+-rw-r--r--   0        0        0     6072 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/databricks_adapter.py
+-rw-r--r--   0        0        0     2261 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/file_adapter.py
+-rw-r--r--   0        0        0     2563 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/generic_adapter.py
+-rw-r--r--   0        0        0      898 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/helper.py
+-rw-r--r--   0        0        0     3422 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/mysql_adapter.py
+-rw-r--r--   0        0        0     2297 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/postgresql_adapter.py
+-rw-r--r--   0        0        0     4085 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/redshift_adapter.py
+-rw-r--r--   0        0        0     3344 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/snowflake_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      660 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/athena/__init__.py
+-rw-r--r--   0        0        0      701 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5071 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6415 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0     9751 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1844 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
+-rw-r--r--   0        0        0      672 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/databricks/__init__.py
+-rw-r--r--   0        0        0      713 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5010 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6601 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0    10073 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1848 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
+-rw-r--r--   0        0        0    39764 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy_adapter.py
+-rw-r--r--   0        0        0     5009 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/sqlite_adapter.py
+-rw-r--r--   0        0        0     6687 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/adapters/trino_adapter.py
+-rw-r--r--   0        0        0     1835 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/helper.py
+-rw-r--r--   0        0        0    53852 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/model.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/notebook/__init__.py
+-rw-r--r--   0        0        0     6818 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/notebook/model_loader.py
+-rw-r--r--   0        0        0     5424 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/project_discovery.py
+-rw-r--r--   0        0        0     2102 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/project_serialization.py
+-rw-r--r--   0        0        0      785 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/samples/__init__.py
+-rw-r--r--   0        0        0     3794 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/samples/data_ingestion.py
+-rw-r--r--   0        0        0    10141 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/samples/sample_data_generator.py
+-rw-r--r--   0        0        0    11926 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/serialization.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/visualization/__init__.py
+-rw-r--r--   0        0        0     7022 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/visualization/charts.py
+-rw-r--r--   0        0        0     1866 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/visualization/common.py
+-rw-r--r--   0        0        0      941 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/visualization/labels.py
+-rw-r--r--   0        0        0     7802 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/visualization/plot.py
+-rw-r--r--   0        0        0     5767 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/visualization/titles.py
+-rw-r--r--   0        0        0     3181 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/visualization/tooltips.py
+-rw-r--r--   0        0        0     3339 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/visualization/transform_conv.py
+-rw-r--r--   0        0        0     1278 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/visualization/transform_retention.py
+-rw-r--r--   0        0        0     6148 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/webapp/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/webapp/__init__.py
+-rw-r--r--   0        0        0     5347 2023-05-11 19:37:52.298909 mitzu-0.6.0rc7/mitzu/webapp/assets/explore_page.css
+-rw-r--r--   0        0        0   147145 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/assets/favicon.ico
+-rw-r--r--   0        0        0    46702 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/assets/logo.png
+-rw-r--r--   0        0        0    43472 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/assets/mitzu-logo-light.svg
+-rw-r--r--   0        0        0    49422 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/athena.png
+-rw-r--r--   0        0        0    10321 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/clickhouse.png
+-rw-r--r--   0        0        0   119554 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/databricks.png
+-rw-r--r--   0        0        0     3008 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/mysql.png
+-rw-r--r--   0        0        0     2446 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/pandas.png
+-rw-r--r--   0        0        0     5338 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/postgresql.png
+-rw-r--r--   0        0        0     8512 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/redshift.png
+-rw-r--r--   0        0        0    93500 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/snowflake.png
+-rw-r--r--   0        0        0    48681 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/sqlite.png
+-rw-r--r--   0        0        0    34219 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/trino.png
+-rw-r--r--   0        0        0    13611 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/auth/authorizer.py
+-rw-r--r--   0        0        0     3557 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/auth/cognito.py
+-rw-r--r--   0        0        0     1594 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/auth/decorator.py
+-rw-r--r--   0        0        0     2777 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/auth/google.py
+-rw-r--r--   0        0        0     7481 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/cache.py
+-rw-r--r--   0        0        0     2966 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/caching_dataset_adapter.py
+-rw-r--r--   0        0        0     1462 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/configs.py
+-rw-r--r--   0        0        0     3088 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/dependencies.py
+-rw-r--r--   0        0        0     4833 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/helper.py
+-rw-r--r--   0        0        0     8375 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/model.py
+-rw-r--r--   0        0        0      408 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/navbar.py
+-rw-r--r--   0        0        0     5802 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/offcanvas.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/pages/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/pages/connections/__init__.py
+-rw-r--r--   0        0        0    15464 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/pages/connections/manage_connections_component.py
+-rw-r--r--   0        0        0     4527 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/pages/connections_page.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/pages/dashboards/__init__.py
+-rw-r--r--   0        0        0    21140 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
+-rw-r--r--   0        0        0     9846 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/pages/dashboards.py
+-rw-r--r--   0        0        0    14654 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/pages/edit_user.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/pages/explore/__init__.py
+-rw-r--r--   0        0        0     5724 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/pages/explore/complex_segment_handler.py
+-rw-r--r--   0        0        0     6488 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/pages/explore/dates_selector_handler.py
+-rw-r--r--   0        0        0     5564 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/pages/explore/event_segment_handler.py
+-rw-r--r--   0        0        0    21781 2023-05-11 19:37:52.302909 mitzu-0.6.0rc7/mitzu/webapp/pages/explore/explore_page.py
+-rw-r--r--   0        0        0     9604 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/explore/graph_handler.py
+-rw-r--r--   0        0        0    10940 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/explore/metric_config_handler.py
+-rw-r--r--   0        0        0     2375 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/explore/metric_segments_handler.py
+-rw-r--r--   0        0        0     1565 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/explore/metric_type_handler.py
+-rw-r--r--   0        0        0     9783 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/explore/simple_segment_handler.py
+-rw-r--r--   0        0        0     4644 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/explore/toolbar_handler.py
+-rw-r--r--   0        0        0     1347 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/explore_project.py
+-rw-r--r--   0        0        0     1751 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/home.py
+-rw-r--r--   0        0        0     4107 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/login.py
+-rw-r--r--   0        0        0     5027 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/manage_connection.py
+-rw-r--r--   0        0        0     1315 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/manage_dashboard.py
+-rw-r--r--   0        0        0    10191 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/manage_event_defs.py
+-rw-r--r--   0        0        0    11849 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/manage_project.py
+-rw-r--r--   0        0        0     9629 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/manage_saved_metrics.py
+-rw-r--r--   0        0        0     1738 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/paths.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/projects/__init__.py
+-rw-r--r--   0        0        0    36159 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/projects/event_tables_config.py
+-rw-r--r--   0        0        0      587 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/projects/helper.py
+-rw-r--r--   0        0        0     9400 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/projects/manage_project_component.py
+-rw-r--r--   0        0        0     5155 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/projects_page.py
+-rw-r--r--   0        0        0     3185 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/pages/users.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/service/__init__.py
+-rw-r--r--   0        0        0     2207 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/service/events_service.py
+-rw-r--r--   0        0        0     5302 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/service/navbar_service.py
+-rw-r--r--   0        0        0      670 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/service/notification_service.py
+-rw-r--r--   0        0        0     2105 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/service/secret_service.py
+-rw-r--r--   0        0        0     4719 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/service/user_service.py
+-rw-r--r--   0        0        0    21352 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/storage.py
+-rw-r--r--   0        0        0    25830 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/storage_model.py
+-rw-r--r--   0        0        0     4625 2023-05-11 19:37:52.306909 mitzu-0.6.0rc7/mitzu/webapp/webapp.py
+-rw-r--r--   0        0        0     2943 2023-05-11 19:38:51.574270 mitzu-0.6.0rc7/pyproject.toml
+-rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 mitzu-0.6.0rc7/PKG-INFO
```

### Comparing `mitzu-0.6.0rc6/LICENSE.txt` & `mitzu-0.6.0rc7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/README.md` & `mitzu-0.6.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/.DS_Store` & `mitzu-0.6.0rc7/mitzu/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/__init__.py` & `mitzu-0.6.0rc7/mitzu/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     TimeWindow,
     TimeGroup,
     DiscoverySettings,
     WebappSettings,
 )
 from mitzu.samples import get_sample_discovered_project
 
-__version__ = "0.6.0-rc.6"
+__version__ = "0.6.0-rc.7"
 
 
 __all__ = [
     "Connection",
     "ConnectionType",
     "Project",
     "EventDataTable",
```

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/adapter_factory.py` & `mitzu-0.6.0rc7/mitzu/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/athena_adapter.py` & `mitzu-0.6.0rc7/mitzu/adapters/athena_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/databricks_adapter.py` & `mitzu-0.6.0rc7/mitzu/adapters/databricks_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/file_adapter.py` & `mitzu-0.6.0rc7/mitzu/adapters/file_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/generic_adapter.py` & `mitzu-0.6.0rc7/mitzu/adapters/generic_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/helper.py` & `mitzu-0.6.0rc7/mitzu/adapters/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/mysql_adapter.py` & `mitzu-0.6.0rc7/mitzu/adapters/mysql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/postgresql_adapter.py` & `mitzu-0.6.0rc7/mitzu/adapters/postgresql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/redshift_adapter.py` & `mitzu-0.6.0rc7/mitzu/adapters/redshift_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/snowflake_adapter.py` & `mitzu-0.6.0rc7/mitzu/adapters/snowflake_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/__init__.py` & `mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py` & `mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py` & `mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py` & `mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py` & `mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py` & `mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/__init__.py` & `mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py` & `mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py` & `mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py` & `mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py` & `mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py` & `mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy_adapter.py` & `mitzu-0.6.0rc7/mitzu/adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/sqlite_adapter.py` & `mitzu-0.6.0rc7/mitzu/adapters/sqlite_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/adapters/trino_adapter.py` & `mitzu-0.6.0rc7/mitzu/adapters/trino_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/helper.py` & `mitzu-0.6.0rc7/mitzu/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/model.py` & `mitzu-0.6.0rc7/mitzu/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/notebook/model_loader.py` & `mitzu-0.6.0rc7/mitzu/notebook/model_loader.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/project_discovery.py` & `mitzu-0.6.0rc7/mitzu/project_discovery.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/project_serialization.py` & `mitzu-0.6.0rc7/mitzu/project_serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/samples/__init__.py` & `mitzu-0.6.0rc7/mitzu/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/samples/data_ingestion.py` & `mitzu-0.6.0rc7/mitzu/samples/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/samples/sample_data_generator.py` & `mitzu-0.6.0rc7/mitzu/samples/sample_data_generator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/serialization.py` & `mitzu-0.6.0rc7/mitzu/serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/visualization/charts.py` & `mitzu-0.6.0rc7/mitzu/visualization/charts.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/visualization/common.py` & `mitzu-0.6.0rc7/mitzu/visualization/common.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/visualization/labels.py` & `mitzu-0.6.0rc7/mitzu/visualization/labels.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/visualization/plot.py` & `mitzu-0.6.0rc7/mitzu/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/visualization/titles.py` & `mitzu-0.6.0rc7/mitzu/visualization/titles.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/visualization/tooltips.py` & `mitzu-0.6.0rc7/mitzu/visualization/tooltips.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/visualization/transform_conv.py` & `mitzu-0.6.0rc7/mitzu/visualization/transform_conv.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/visualization/transform_retention.py` & `mitzu-0.6.0rc7/mitzu/visualization/transform_retention.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/.DS_Store` & `mitzu-0.6.0rc7/mitzu/webapp/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/assets/explore_page.css` & `mitzu-0.6.0rc7/mitzu/webapp/assets/explore_page.css`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/assets/favicon.ico` & `mitzu-0.6.0rc7/mitzu/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/assets/logo.png` & `mitzu-0.6.0rc7/mitzu/webapp/assets/logo.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/assets/mitzu-logo-light.svg` & `mitzu-0.6.0rc7/mitzu/webapp/assets/mitzu-logo-light.svg`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/athena.png` & `mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/athena.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/clickhouse.png` & `mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/databricks.png` & `mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/databricks.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/mysql.png` & `mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/mysql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/pandas.png` & `mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/pandas.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/postgresql.png` & `mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/postgresql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/redshift.png` & `mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/redshift.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/snowflake.png` & `mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/snowflake.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/sqlite.png` & `mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/sqlite.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/trino.png` & `mitzu-0.6.0rc7/mitzu/webapp/assets/warehouse/trino.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/auth/authorizer.py` & `mitzu-0.6.0rc7/mitzu/webapp/auth/authorizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,18 +109,14 @@
             P.UNAUTHORIZED_URL,
             P.SIGN_OUT_URL,
             P.HEALTHCHECK_PATH,
             "/assets/",
         ]
     )
 
-    def get_home_url(self):
-        url = flask.request.host_url
-        return url[:-1] if url.endswith("/") else url
-
     @classmethod
     def create(cls, config: AuthConfig) -> OAuthAuthorizer:
         return OAuthAuthorizer(
             _config=config,
         )
 
     def _get_unauthenticated_response(
@@ -169,15 +165,15 @@
             "utf-8",
         )
         secret_hash = base64.b64encode(message).decode()
         payload = {
             "grant_type": "authorization_code",
             "client_id": self._config.oauth.client_id,
             "code": auth_code,
-            "redirect_uri": f"{self.get_home_url()}{P.OAUTH_CODE_URL}",
+            "redirect_uri": f"{configs.HOME_URL}{P.OAUTH_CODE_URL}",
         }
         headers = {
             "Content-Type": "application/x-www-form-urlencoded",
             "Authorization": f"Basic {secret_hash}",
         }
 
         resp = requests.post(
@@ -350,15 +346,15 @@
         token = self._generate_new_token_for_identity(user.id, role=user.role)
 
         if response:
             self.set_cookie(response, self._config.token_cookie_name, token)
             self.clear_cookie(response, self._config.redirect_cookie_name)
 
         return flask.request.cookies.get(
-            self._config.redirect_cookie_name, self.get_home_url()
+            self._config.redirect_cookie_name, configs.HOME_URL
         )
 
     def get_current_user_id(self) -> Optional[str]:
         auth_token = flask.request.cookies.get(self._config.token_cookie_name)
         if auth_token is None:
             return None
         token_claims = self._validate_token(auth_token)
```

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/auth/cognito.py` & `mitzu-0.6.0rc7/mitzu/webapp/auth/cognito.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/auth/decorator.py` & `mitzu-0.6.0rc7/mitzu/webapp/auth/decorator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/auth/google.py` & `mitzu-0.6.0rc7/mitzu/webapp/auth/google.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/cache.py` & `mitzu-0.6.0rc7/mitzu/webapp/cache.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/caching_dataset_adapter.py` & `mitzu-0.6.0rc7/mitzu/webapp/caching_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/configs.py` & `mitzu-0.6.0rc7/mitzu/webapp/configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
 from typing import Tuple, Optional
 
+HOME_URL = os.getenv("HOME_URL", "http://localhost:8082")
+
 # dash
 GRAPH_POLL_INTERVAL_MS = int(os.getenv("GRAPH_POLL_INTERVAL_MS", 300))
 DASH_TITLE = os.getenv("DASH_TITLE", "Mitzu")
 DASH_FAVICON_PATH = os.getenv("DASH_FAVICON_PATH", "assets/favicon.ico")
 DASH_LOGO_PATH = os.getenv("DASH_LOGO_PATH", "/assets/mitzu-logo-light.svg")
```

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/dependencies.py` & `mitzu-0.6.0rc7/mitzu/webapp/dependencies.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/helper.py` & `mitzu-0.6.0rc7/mitzu/webapp/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/model.py` & `mitzu-0.6.0rc7/mitzu/webapp/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/offcanvas.py` & `mitzu-0.6.0rc7/mitzu/webapp/offcanvas.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/connections/manage_connections_component.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/connections/manage_connections_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/connections_page.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/connections_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/dashboards/manage_dashboards_component.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/dashboards/manage_dashboards_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/dashboards.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/dashboards.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/edit_user.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/edit_user.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/complex_segment_handler.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/explore/complex_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/dates_selector_handler.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/explore/dates_selector_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/event_segment_handler.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/explore/event_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/explore_page.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/explore/explore_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/graph_handler.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/explore/graph_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/metric_config_handler.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/explore/metric_config_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/metric_segments_handler.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/explore/metric_segments_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/metric_type_handler.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/explore/metric_type_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/simple_segment_handler.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/explore/simple_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/toolbar_handler.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/explore/toolbar_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/explore_project.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/explore_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/home.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/home.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/login.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/login.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/manage_connection.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/manage_connection.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/manage_dashboard.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/manage_dashboard.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/manage_event_defs.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/manage_event_defs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/manage_project.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/manage_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/manage_saved_metrics.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/manage_saved_metrics.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/paths.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/paths.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/projects/event_tables_config.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/projects/event_tables_config.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/projects/helper.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/projects/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/projects/manage_project_component.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/projects/manage_project_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/projects_page.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/projects_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/pages/users.py` & `mitzu-0.6.0rc7/mitzu/webapp/pages/users.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/service/events_service.py` & `mitzu-0.6.0rc7/mitzu/webapp/service/events_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/service/navbar_service.py` & `mitzu-0.6.0rc7/mitzu/webapp/service/navbar_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/service/notification_service.py` & `mitzu-0.6.0rc7/mitzu/webapp/service/notification_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/service/secret_service.py` & `mitzu-0.6.0rc7/mitzu/webapp/service/secret_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/service/user_service.py` & `mitzu-0.6.0rc7/mitzu/webapp/service/user_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/storage.py` & `mitzu-0.6.0rc7/mitzu/webapp/storage.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/storage_model.py` & `mitzu-0.6.0rc7/mitzu/webapp/storage_model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/mitzu/webapp/webapp.py` & `mitzu-0.6.0rc7/mitzu/webapp/webapp.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc6/pyproject.toml` & `mitzu-0.6.0rc7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mitzu"
-version = "0.6.0-rc.6"
+version = "0.6.0-rc.7"
 description = "Product analytics over your data warehouse"
 authors = ["Istvan Meszaros <istvan.meszaros.88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mitzu.io"
 repository = "https://github.com/mitzu-io/mitzu"
 documentation = "https://mitzu.io/documentation/"
```

### Comparing `mitzu-0.6.0rc6/PKG-INFO` & `mitzu-0.6.0rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitzu
-Version: 0.6.0rc6
+Version: 0.6.0rc7
 Summary: Product analytics over your data warehouse
 Home-page: https://mitzu.io
 License: MIT
 Author: Istvan Meszaros
 Author-email: istvan.meszaros.88@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

