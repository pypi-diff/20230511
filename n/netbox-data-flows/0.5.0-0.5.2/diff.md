# Comparing `tmp/netbox-data-flows-0.5.0.tar.gz` & `tmp/netbox-data-flows-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-data-flows-0.5.0.tar", last modified: Wed May 10 22:36:21 2023, max compression
+gzip compressed data, was "netbox-data-flows-0.5.2.tar", last modified: Thu May 11 20:32:05 2023, max compression
```

## Comparing `netbox-data-flows-0.5.0.tar` & `netbox-data-flows-0.5.2.tar`

### file list

```diff
@@ -1,108 +1,107 @@
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.060640 netbox-data-flows-0.5.0/
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)    10174 2022-10-31 14:13:19.000000 netbox-data-flows-0.5.0/LICENSE.txt
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)       53 2022-11-30 19:02:39.000000 netbox-data-flows-0.5.0/MANIFEST.in
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      193 2023-05-10 22:36:21.060640 netbox-data-flows-0.5.0/PKG-INFO
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     3157 2023-05-10 21:36:06.000000 netbox-data-flows-0.5.0/README.md
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.056640 netbox-data-flows-0.5.0/netbox_data_flows/
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      533 2023-05-10 21:44:26.000000 netbox-data-flows-0.5.0/netbox_data_flows/__init__.py
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.056640 netbox-data-flows-0.5.0/netbox_data_flows/api/
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)        0 2022-11-05 12:25:55.000000 netbox-data-flows-0.5.0/netbox_data_flows/api/__init__.py
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.056640 netbox-data-flows-0.5.0/netbox_data_flows/api/serializers/
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      126 2022-11-30 17:09:14.000000 netbox-data-flows-0.5.0/netbox_data_flows/api/serializers/__init__.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1494 2022-11-30 17:09:14.000000 netbox-data-flows-0.5.0/netbox_data_flows/api/serializers/applications.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     2055 2022-12-21 22:49:38.000000 netbox-data-flows-0.5.0/netbox_data_flows/api/serializers/dataflows.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1467 2022-12-29 16:31:23.000000 netbox-data-flows-0.5.0/netbox_data_flows/api/serializers/groups.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     2904 2022-11-30 20:02:16.000000 netbox-data-flows-0.5.0/netbox_data_flows/api/serializers/nested.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1387 2023-02-12 15:21:32.000000 netbox-data-flows-0.5.0/netbox_data_flows/api/serializers/objectaliases.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      563 2022-11-30 17:09:14.000000 netbox-data-flows-0.5.0/netbox_data_flows/api/urls.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     2149 2022-11-30 17:09:14.000000 netbox-data-flows-0.5.0/netbox_data_flows/api/views.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1583 2023-02-19 17:48:26.000000 netbox-data-flows-0.5.0/netbox_data_flows/choices.py
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.056640 netbox-data-flows-0.5.0/netbox_data_flows/filtersets/
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      104 2022-11-30 17:09:14.000000 netbox-data-flows-0.5.0/netbox_data_flows/filtersets/__init__.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1746 2022-12-21 22:47:54.000000 netbox-data-flows-0.5.0/netbox_data_flows/filtersets/addins.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1278 2022-12-29 17:58:30.000000 netbox-data-flows-0.5.0/netbox_data_flows/filtersets/applications.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     7434 2022-12-29 15:30:12.000000 netbox-data-flows-0.5.0/netbox_data_flows/filtersets/dataflows.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      588 2022-12-21 22:28:37.000000 netbox-data-flows-0.5.0/netbox_data_flows/filtersets/filters.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1859 2022-12-29 16:38:41.000000 netbox-data-flows-0.5.0/netbox_data_flows/filtersets/groups.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     2840 2022-12-22 23:03:49.000000 netbox-data-flows-0.5.0/netbox_data_flows/filtersets/objectaliases.py
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.056640 netbox-data-flows-0.5.0/netbox_data_flows/forms/
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      136 2022-11-30 17:09:14.000000 netbox-data-flows-0.5.0/netbox_data_flows/forms/__init__.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1481 2023-05-10 19:58:44.000000 netbox-data-flows-0.5.0/netbox_data_flows/forms/applicationroles.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     2758 2023-05-10 20:06:08.000000 netbox-data-flows-0.5.0/netbox_data_flows/forms/applications.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)    14256 2023-05-10 21:12:53.000000 netbox-data-flows-0.5.0/netbox_data_flows/forms/dataflows.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     5404 2023-05-10 20:30:39.000000 netbox-data-flows-0.5.0/netbox_data_flows/forms/groups.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     3667 2023-05-10 20:08:02.000000 netbox-data-flows-0.5.0/netbox_data_flows/forms/objectaliases.py
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.056640 netbox-data-flows-0.5.0/netbox_data_flows/graphql/
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      906 2022-11-30 17:09:14.000000 netbox-data-flows-0.5.0/netbox_data_flows/graphql/__init__.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      536 2022-11-27 16:25:41.000000 netbox-data-flows-0.5.0/netbox_data_flows/graphql/applications.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      300 2022-11-30 17:09:14.000000 netbox-data-flows-0.5.0/netbox_data_flows/graphql/dataflows.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      320 2022-11-30 17:09:14.000000 netbox-data-flows-0.5.0/netbox_data_flows/graphql/groups.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      544 2022-11-30 17:09:14.000000 netbox-data-flows-0.5.0/netbox_data_flows/graphql/objectaliases.py
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.056640 netbox-data-flows-0.5.0/netbox_data_flows/management/
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)        0 2023-02-19 17:29:49.000000 netbox-data-flows-0.5.0/netbox_data_flows/management/__init__.py
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.056640 netbox-data-flows-0.5.0/netbox_data_flows/management/commands/
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)        0 2023-02-19 17:29:56.000000 netbox-data-flows-0.5.0/netbox_data_flows/management/commands/__init__.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1078 2023-02-19 17:48:26.000000 netbox-data-flows-0.5.0/netbox_data_flows/management/commands/delete_orphaned_aliases.py
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.056640 netbox-data-flows-0.5.0/netbox_data_flows/migrations/
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)    14554 2023-05-10 19:31:42.000000 netbox-data-flows-0.5.0/netbox_data_flows/migrations/0001_initial.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      437 2023-05-10 19:31:42.000000 netbox-data-flows-0.5.0/netbox_data_flows/migrations/0002_alter_objectalias_options.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1724 2023-05-10 19:31:42.000000 netbox-data-flows-0.5.0/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      290 2023-05-10 19:31:42.000000 netbox-data-flows-0.5.0/netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      917 2023-05-10 19:31:42.000000 netbox-data-flows-0.5.0/netbox_data_flows/migrations/0005_dataflowgroup_slug.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      850 2023-05-10 19:31:42.000000 netbox-data-flows-0.5.0/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      347 2023-05-10 19:31:42.000000 netbox-data-flows-0.5.0/netbox_data_flows/migrations/0007_remove_objectalias_size.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      531 2023-05-10 19:31:42.000000 netbox-data-flows-0.5.0/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)        0 2022-11-29 16:29:46.000000 netbox-data-flows-0.5.0/netbox_data_flows/migrations/__init__.py
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.056640 netbox-data-flows-0.5.0/netbox_data_flows/models/
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      104 2022-11-30 17:09:14.000000 netbox-data-flows-0.5.0/netbox_data_flows/models/__init__.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1549 2023-05-10 21:19:17.000000 netbox-data-flows-0.5.0/netbox_data_flows/models/applications.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     6280 2023-01-29 15:55:16.000000 netbox-data-flows-0.5.0/netbox_data_flows/models/dataflows.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     4287 2023-01-29 15:55:16.000000 netbox-data-flows-0.5.0/netbox_data_flows/models/groups.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     7881 2023-02-19 17:20:50.000000 netbox-data-flows-0.5.0/netbox_data_flows/models/objectaliases.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     2011 2023-05-10 19:31:28.000000 netbox-data-flows-0.5.0/netbox_data_flows/navigation.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1045 2022-12-29 18:11:10.000000 netbox-data-flows-0.5.0/netbox_data_flows/search.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      483 2023-02-19 17:48:26.000000 netbox-data-flows-0.5.0/netbox_data_flows/signals.py
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.056640 netbox-data-flows-0.5.0/netbox_data_flows/tables/
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      104 2022-11-30 17:09:14.000000 netbox-data-flows-0.5.0/netbox_data_flows/tables/__init__.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     2001 2023-05-10 21:22:36.000000 netbox-data-flows-0.5.0/netbox_data_flows/tables/applications.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     3906 2023-05-10 21:24:28.000000 netbox-data-flows-0.5.0/netbox_data_flows/tables/dataflows.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1510 2023-05-10 21:25:06.000000 netbox-data-flows-0.5.0/netbox_data_flows/tables/groups.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     2336 2023-02-12 15:21:16.000000 netbox-data-flows-0.5.0/netbox_data_flows/tables/objectaliases.py
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.056640 netbox-data-flows-0.5.0/netbox_data_flows/templates/
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.056640 netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     2069 2022-12-29 18:00:24.000000 netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/application.html
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1608 2022-11-05 12:25:55.000000 netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/applicationrole.html
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     3644 2023-02-12 16:27:44.000000 netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/dataflow.html
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1455 2022-11-05 12:25:55.000000 netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/dataflow_edit.html
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      649 2022-11-05 13:28:01.000000 netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      480 2022-12-29 15:41:30.000000 netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1877 2023-02-12 16:38:03.000000 netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     2619 2022-12-21 21:02:25.000000 netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.056640 netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/inc/
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     5945 2022-11-05 12:25:55.000000 netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/inc/dataflow_specifications.html
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      411 2023-02-12 16:49:25.000000 netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/inc/objectaliastarget_actions.html
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     2606 2022-11-30 17:09:14.000000 netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/objectalias.html
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1529 2022-11-30 17:09:14.000000 netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      483 2022-12-29 15:42:01.000000 netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/objectalias_tab.html
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     4405 2023-01-29 19:25:40.000000 netbox-data-flows-0.5.0/netbox_data_flows/urls.py
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.056640 netbox-data-flows-0.5.0/netbox_data_flows/utils/
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)        0 2022-11-30 17:09:14.000000 netbox-data-flows-0.5.0/netbox_data_flows/utils/__init__.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     8124 2023-02-12 20:24:42.000000 netbox-data-flows-0.5.0/netbox_data_flows/utils/aliases.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     1381 2022-12-22 23:44:33.000000 netbox-data-flows-0.5.0/netbox_data_flows/utils/helpers.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      444 2023-01-29 21:46:24.000000 netbox-data-flows-0.5.0/netbox_data_flows/utils/tables.py
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.060640 netbox-data-flows-0.5.0/netbox_data_flows/views/
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      136 2022-11-30 17:09:14.000000 netbox-data-flows-0.5.0/netbox_data_flows/views/__init__.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     2146 2023-01-29 19:15:33.000000 netbox-data-flows-0.5.0/netbox_data_flows/views/applicationroles.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     2603 2023-01-29 19:14:13.000000 netbox-data-flows-0.5.0/netbox_data_flows/views/applications.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     5636 2023-02-12 17:16:09.000000 netbox-data-flows-0.5.0/netbox_data_flows/views/dataflows.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     3136 2023-01-29 19:11:21.000000 netbox-data-flows-0.5.0/netbox_data_flows/views/groups.py
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     5238 2023-01-29 19:27:52.000000 netbox-data-flows-0.5.0/netbox_data_flows/views/objectaliases.py
-drwxr-xr-x   0 tsfx      (1000) tsfx      (1000)        0 2023-05-10 22:36:21.056640 netbox-data-flows-0.5.0/netbox_data_flows.egg-info/
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      193 2023-05-10 22:36:21.000000 netbox-data-flows-0.5.0/netbox_data_flows.egg-info/PKG-INFO
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)     3866 2023-05-10 22:36:21.000000 netbox-data-flows-0.5.0/netbox_data_flows.egg-info/SOURCES.txt
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)        1 2023-05-10 22:36:21.000000 netbox-data-flows-0.5.0/netbox_data_flows.egg-info/dependency_links.txt
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)        1 2022-11-30 19:02:08.000000 netbox-data-flows-0.5.0/netbox_data_flows.egg-info/not-zip-safe
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)       18 2023-05-10 22:36:21.000000 netbox-data-flows-0.5.0/netbox_data_flows.egg-info/top_level.txt
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)       30 2022-11-05 12:25:55.000000 netbox-data-flows-0.5.0/pyproject.toml
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)       38 2023-05-10 22:36:21.060640 netbox-data-flows-0.5.0/setup.cfg
--rw-r--r--   0 tsfx      (1000) tsfx      (1000)      339 2023-05-10 21:44:09.000000 netbox-data-flows-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.314914 netbox-data-flows-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-11 20:32:05.314914 netbox-data-flows-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.302914 netbox-data-flows-0.5.2/netbox_data_flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.306914 netbox-data-flows-0.5.2/netbox_data_flows/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.306914 netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/objectaliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.306914 netbox-data-flows-0.5.2/netbox_data_flows/filtersets/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/filtersets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/filtersets/addins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/filtersets/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/filtersets/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/filtersets/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/filtersets/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/filtersets/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.306914 netbox-data-flows-0.5.2/netbox_data_flows/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/forms/applicationroles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/forms/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14256 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/forms/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/forms/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/forms/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.306914 netbox-data-flows-0.5.2/netbox_data_flows/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/graphql/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/graphql/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/graphql/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/graphql/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.306914 netbox-data-flows-0.5.2/netbox_data_flows/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.306914 netbox-data-flows-0.5.2/netbox_data_flows/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/management/commands/delete_orphaned_aliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.310914 netbox-data-flows-0.5.2/netbox_data_flows/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/0002_alter_objectalias_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/0005_dataflowgroup_slug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/0007_remove_objectalias_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.310914 netbox-data-flows-0.5.2/netbox_data_flows/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/models/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/models/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/models/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/models/objectaliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.310914 netbox-data-flows-0.5.2/netbox_data_flows/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/tables/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/tables/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/tables/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/tables/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.302914 netbox-data-flows-0.5.2/netbox_data_flows/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.310914 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/application.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/applicationrole.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.310914 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/inc/dataflow_specifications.html
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/inc/objectaliastarget_actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/objectalias.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/objectalias_tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.314914 netbox-data-flows-0.5.2/netbox_data_flows/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/utils/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.314914 netbox-data-flows-0.5.2/netbox_data_flows/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/views/applicationroles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/views/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/views/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/views/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/views/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.306914 netbox-data-flows-0.5.2/netbox_data_flows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-11 20:32:05.000000 netbox-data-flows-0.5.2/netbox_data_flows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-11 20:32:05.000000 netbox-data-flows-0.5.2/netbox_data_flows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:32:05.000000 netbox-data-flows-0.5.2/netbox_data_flows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:32:05.000000 netbox-data-flows-0.5.2/netbox_data_flows.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 20:32:05.000000 netbox-data-flows-0.5.2/netbox_data_flows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:32:05.314914 netbox-data-flows-0.5.2/setup.cfg
```

### Comparing `netbox-data-flows-0.5.0/LICENSE.txt` & `netbox-data-flows-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/__init__.py` & `netbox-data-flows-0.5.2/netbox_data_flows/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from extras.plugins import PluginConfig
 
-__version__ = "0.5.0"
+__version__ = "0.5.2"
 
 
 class DataFlowsConfig(PluginConfig):
     name = "netbox_data_flows"
     verbose_name = "Data Flows"
-    description = "NetBox plugin to document applications and data flows"
+    description = "NetBox plugin to document data flows between systems and applications."
     version = __version__
     base_url = "data-flows"
     author = "Thomas Fargeix"
     required_settings = []
     default_settings = {}
     min_version = "3.4.2"
     max_version = "3.5.99"
```

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/api/serializers/applications.py` & `netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/api/serializers/dataflows.py` & `netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/api/serializers/groups.py` & `netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/api/serializers/nested.py` & `netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/nested.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/api/serializers/objectaliases.py` & `netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/api/urls.py` & `netbox-data-flows-0.5.2/netbox_data_flows/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/api/views.py` & `netbox-data-flows-0.5.2/netbox_data_flows/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/choices.py` & `netbox-data-flows-0.5.2/netbox_data_flows/choices.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/filtersets/addins.py` & `netbox-data-flows-0.5.2/netbox_data_flows/filtersets/addins.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/filtersets/applications.py` & `netbox-data-flows-0.5.2/netbox_data_flows/filtersets/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/filtersets/dataflows.py` & `netbox-data-flows-0.5.2/netbox_data_flows/filtersets/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/filtersets/filters.py` & `netbox-data-flows-0.5.2/netbox_data_flows/filtersets/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/filtersets/groups.py` & `netbox-data-flows-0.5.2/netbox_data_flows/filtersets/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/filtersets/objectaliases.py` & `netbox-data-flows-0.5.2/netbox_data_flows/filtersets/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/forms/applicationroles.py` & `netbox-data-flows-0.5.2/netbox_data_flows/forms/applicationroles.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/forms/applications.py` & `netbox-data-flows-0.5.2/netbox_data_flows/forms/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/forms/dataflows.py` & `netbox-data-flows-0.5.2/netbox_data_flows/forms/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/forms/groups.py` & `netbox-data-flows-0.5.2/netbox_data_flows/forms/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/forms/objectaliases.py` & `netbox-data-flows-0.5.2/netbox_data_flows/forms/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/graphql/__init__.py` & `netbox-data-flows-0.5.2/netbox_data_flows/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/graphql/applications.py` & `netbox-data-flows-0.5.2/netbox_data_flows/graphql/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/graphql/objectaliases.py` & `netbox-data-flows-0.5.2/netbox_data_flows/graphql/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/management/commands/delete_orphaned_aliases.py` & `netbox-data-flows-0.5.2/netbox_data_flows/management/commands/delete_orphaned_aliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/migrations/0001_initial.py` & `netbox-data-flows-0.5.2/netbox_data_flows/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py` & `netbox-data-flows-0.5.2/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/migrations/0005_dataflowgroup_slug.py` & `netbox-data-flows-0.5.2/netbox_data_flows/migrations/0005_dataflowgroup_slug.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py` & `netbox-data-flows-0.5.2/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py` & `netbox-data-flows-0.5.2/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/models/applications.py` & `netbox-data-flows-0.5.2/netbox_data_flows/models/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/models/dataflows.py` & `netbox-data-flows-0.5.2/netbox_data_flows/models/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/models/groups.py` & `netbox-data-flows-0.5.2/netbox_data_flows/models/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/models/objectaliases.py` & `netbox-data-flows-0.5.2/netbox_data_flows/models/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/navigation.py` & `netbox-data-flows-0.5.2/netbox_data_flows/navigation.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,45 +2,45 @@
 from utilities.choices import ButtonColorChoices
 
 
 #
 # Utility functions
 #
 
-APP_LABEL = "plugins:netbox_data_flows"
+APP_LABEL = "netbox_data_flows"
 
 
 # clone of netbox.navigation_menu.get_model_item, but for plugin
 def get_model_item(model_name, label, actions=("add", "import")):
     return PluginMenuItem(
-        link=f"{APP_LABEL}:{model_name}_list",
+        link=f"plugins:{APP_LABEL}:{model_name}_list",
         link_text=label,
         permissions=[f"{APP_LABEL}.view_{model_name}"],
         buttons=get_model_buttons(model_name, actions),
     )
 
 
 # clone of netbox.navigation_menu.get_model_buttons, but for plugin
 def get_model_buttons(model_name, actions=("add", "import")):
     buttons = []
 
     if "add" in actions:
         buttons.append(
             PluginMenuButton(
-                link=f"{APP_LABEL}:{model_name}_add",
+                link=f"plugins:{APP_LABEL}:{model_name}_add",
                 title="Add",
                 icon_class="mdi mdi-plus-thick",
                 permissions=[f"{APP_LABEL}.add_{model_name}"],
                 color=ButtonColorChoices.GREEN,
             )
         )
     if "import" in actions:
         buttons.append(
             PluginMenuButton(
-                link=f"{APP_LABEL}:{model_name}_import",
+                link=f"plugins:{APP_LABEL}:{model_name}_import",
                 title="Import",
                 icon_class="mdi mdi-upload",
                 permissions=[f"{APP_LABEL}.add_{model_name}"],
                 color=ButtonColorChoices.CYAN,
             )
         )
```

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/search.py` & `netbox-data-flows-0.5.2/netbox_data_flows/search.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/tables/applications.py` & `netbox-data-flows-0.5.2/netbox_data_flows/tables/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/tables/dataflows.py` & `netbox-data-flows-0.5.2/netbox_data_flows/tables/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/tables/groups.py` & `netbox-data-flows-0.5.2/netbox_data_flows/tables/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/tables/objectaliases.py` & `netbox-data-flows-0.5.2/netbox_data_flows/tables/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/application.html` & `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/application.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/applicationrole.html` & `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/applicationrole.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/dataflow.html` & `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/dataflow_edit.html` & `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html` & `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html` & `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html` & `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/inc/dataflow_specifications.html` & `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/inc/dataflow_specifications.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/objectalias.html` & `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/objectalias.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html` & `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/urls.py` & `netbox-data-flows-0.5.2/netbox_data_flows/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/utils/aliases.py` & `netbox-data-flows-0.5.2/netbox_data_flows/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/utils/helpers.py` & `netbox-data-flows-0.5.2/netbox_data_flows/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/views/applicationroles.py` & `netbox-data-flows-0.5.2/netbox_data_flows/views/applicationroles.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/views/applications.py` & `netbox-data-flows-0.5.2/netbox_data_flows/views/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/views/dataflows.py` & `netbox-data-flows-0.5.2/netbox_data_flows/views/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/views/groups.py` & `netbox-data-flows-0.5.2/netbox_data_flows/views/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows/views/objectaliases.py` & `netbox-data-flows-0.5.2/netbox_data_flows/views/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.0/netbox_data_flows.egg-info/SOURCES.txt` & `netbox-data-flows-0.5.2/netbox_data_flows.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-LICENSE.txt
+LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.py
 netbox_data_flows/__init__.py
 netbox_data_flows/choices.py
 netbox_data_flows/navigation.py
 netbox_data_flows/search.py
 netbox_data_flows/signals.py
 netbox_data_flows/urls.py
 netbox_data_flows.egg-info/PKG-INFO
```

