# Comparing `tmp/dagster-1.3.3.tar.gz` & `tmp/dagster-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.3.3.tar", last modified: Thu May  4 17:42:32 2023, max compression
+gzip compressed data, was "dagster-1.3.4.tar", last modified: Thu May 11 16:59:05 2023, max compression
```

## Comparing `dagster-1.3.3.tar` & `dagster-1.3.4.tar`

### file list

```diff
@@ -1,622 +1,624 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.720379 dagster-1.3.3/
--rw-r--r--   0 root         (0) root         (0)      549 2023-05-04 17:42:13.000000 dagster-1.3.3/COPYING
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-04 17:42:13.000000 dagster-1.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-04 17:42:13.000000 dagster-1.3.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8790 2023-05-04 17:42:32.720379 dagster-1.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7167 2023-05-04 17:42:13.000000 dagster-1.3.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.660379 dagster-1.3.3/dagster/
--rw-r--r--   0 root         (0) root         (0)    25858 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5456 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.660379 dagster-1.3.3/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     2900 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     1639 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_api/snapshot_job.py
--rw-r--r--   0 root         (0) root         (0)     5479 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.660379 dagster-1.3.3/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    51637 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.664379 dagster-1.3.3/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1101 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26765 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8186 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     2300 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     5718 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    29862 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     5852 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5135 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19909 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15661 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.664379 dagster-1.3.3/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28391 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.664379 dagster-1.3.3/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    14686 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    18799 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    15269 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    16886 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9466 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.664379 dagster-1.3.3/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)    70752 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)     6217 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/pythonic_config/utils.py
--rw-r--r--   0 root         (0) root         (0)    12143 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3267 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    16671 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.668379 dagster-1.3.3/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13645 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.668379 dagster-1.3.3/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.676379 dagster-1.3.3/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7626 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28864 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)     3817 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    36842 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     5686 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    47123 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/asset_reconciliation_sensor.py
--rw-r--r--   0 root         (0) root         (0)    17185 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7164 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    64928 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    24005 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/assets_job.py
--rw-r--r--   0 root         (0) root         (0)     3681 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    16105 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    45671 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4287 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    10845 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    20633 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    17905 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.676379 dagster-1.3.3/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42826 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8250 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10676 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    17845 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    14396 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8656 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    11936 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)     6695 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5275 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    20546 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    39903 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    31182 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21013 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)    10548 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/external_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     8010 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16178 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    44758 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6546 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3205 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    22898 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     5386 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)     5816 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/job_base.py
--rw-r--r--   0 root         (0) root         (0)    55438 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)    20308 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     6845 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      636 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8841 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.676379 dagster-1.3.3/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    32319 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8557 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)    55971 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    20758 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11927 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8041 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     2867 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    22629 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    19256 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)    18908 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    37618 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      196 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    46488 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)     8811 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3779 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)    30198 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/reconstruct.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.676379 dagster-1.3.3/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6670 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    18856 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    17401 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    16972 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    16162 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5398 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7806 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)    24309 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1445 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    14601 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    38400 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    36722 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     5189 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    10722 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    46040 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    14250 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2298 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1541 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/test_op_definition.py
--rw-r--r--   0 root         (0) root         (0)    10288 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    74641 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    15645 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)     7992 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     2930 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    25453 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)     6232 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.680379 dagster-1.3.3/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    64981 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7783 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.680379 dagster-1.3.3/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38808 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    29354 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    14156 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6326 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.684379 dagster-1.3.3/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21992 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    15991 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9369 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    26841 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    27417 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    33975 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    44193 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    18549 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/context_creation_job.py
--rw-r--r--   0 root         (0) root         (0)     5149 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5427 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     6479 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/execute_job_result.py
--rw-r--r--   0 root         (0) root         (0)     9183 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8643 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14467 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.684379 dagster-1.3.3/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23031 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    12550 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16275 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    27355 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    10051 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    37831 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5395 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7057 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    59386 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    15616 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    15920 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3796 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8186 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19377 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)    25847 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/results.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1651 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)    10329 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1172 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4233 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.684379 dagster-1.3.3/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5990 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     2840 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1509 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15667 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.684379 dagster-1.3.3/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14328 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.688379 dagster-1.3.3/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3078 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.688379 dagster-1.3.3/dagster/_core/host_representation/
--rw-r--r--   0 root         (0) root         (0)     2789 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/host_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33528 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/host_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    32103 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/host_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    69385 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/host_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)    11276 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/host_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/host_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/host_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1581 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/host_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)     4850 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/host_representation/job_index.py
--rw-r--r--   0 root         (0) root         (0)    17368 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/host_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     3606 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/host_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.688379 dagster-1.3.3/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   102059 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11577 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24318 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     4567 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.688379 dagster-1.3.3/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3639 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6628 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    17249 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     3691 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.688379 dagster-1.3.3/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1922 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    11030 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.688379 dagster-1.3.3/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    18194 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)     9410 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.692379 dagster-1.3.3/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1777 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.692379 dagster-1.3.3/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      305 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20251 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.692379 dagster-1.3.3/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2815 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     3999 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9421 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12099 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    16629 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/snap/job_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4495 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14452 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/snap/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.696379 dagster-1.3.3/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3057 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.696379 dagster-1.3.3/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6676 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.704379 dagster-1.3.3/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      311 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      530 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      634 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7205 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/base_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.704379 dagster-1.3.3/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4304 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8736 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16247 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9545 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    23527 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/dagster_run.py
--rw-r--r--   0 root         (0) root         (0)    11544 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.704379 dagster-1.3.3/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14274 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3630 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     7776 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     5090 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)    78141 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.704379 dagster-1.3.3/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.704379 dagster-1.3.3/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7408 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    18950 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10912 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)    13217 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8915 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10638 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    26162 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17301 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4293 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.704379 dagster-1.3.3/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14469 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    23189 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/root.py
--rw-r--r--   0 root         (0) root         (0)     8509 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/root_input_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.704379 dagster-1.3.3/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15454 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2291 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8635 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     5982 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    46394 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.704379 dagster-1.3.3/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.704379 dagster-1.3.3/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6822 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.708379 dagster-1.3.3/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5344 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4095 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     2776 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    19749 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.708379 dagster-1.3.3/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.708379 dagster-1.3.3/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1039 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3664 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7375 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4863 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     3085 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    11346 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.708379 dagster-1.3.3/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13981 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    14855 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    27932 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    18920 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.708379 dagster-1.3.3/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3163 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7298 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    35761 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4881 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/utility_ops.py
--rw-r--r--   0 root         (0) root         (0)     4003 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.712379 dagster-1.3.3/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4722 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    26620 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11881 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4684 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     3952 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.712379 dagster-1.3.3/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1930 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5235 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.712379 dagster-1.3.3/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6828 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9123 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     1936 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.712379 dagster-1.3.3/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     4422 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17726 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    10457 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.712379 dagster-1.3.3/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      215 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8365 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_daemon/monitoring/monitoring_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.712379 dagster-1.3.3/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16247 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    36568 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2860 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)     6639 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.712379 dagster-1.3.3/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.712379 dagster-1.3.3/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.656379 dagster-1.3.3/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.712379 dagster-1.3.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.712379 dagster-1.3.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.712379 dagster-1.3.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.712379 dagster-1.3.3/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.712379 dagster-1.3.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.716379 dagster-1.3.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.716379 dagster-1.3.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.716379 dagster-1.3.3/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.716379 dagster-1.3.3/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11665 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    38179 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    18501 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4202 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    22000 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.716379 dagster-1.3.3/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5394 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    55354 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5301 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    26359 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     2323 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.716379 dagster-1.3.3/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      438 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.716379 dagster-1.3.3/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     3781 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_loggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.716379 dagster-1.3.3/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31794 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1361 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.716379 dagster-1.3.3/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      629 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8004 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7467 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    37037 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.716379 dagster-1.3.3/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5496 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.716379 dagster-1.3.3/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.720379 dagster-1.3.3/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    23319 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8741 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     6965 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/backcompat.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     4116 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    23668 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     4094 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      883 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     2372 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)      344 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/internal_init.py
--rw-r--r--   0 root         (0) root         (0)     3227 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)     9813 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    12340 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)     3289 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.720379 dagster-1.3.3/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    10412 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     9330 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    23902 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.720379 dagster-1.3.3/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     3334 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-04 17:42:13.000000 dagster-1.3.3/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:42:32.660379 dagster-1.3.3/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8790 2023-05-04 17:42:32.000000 dagster-1.3.3/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24829 2023-05-04 17:42:32.000000 dagster-1.3.3/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:42:32.000000 dagster-1.3.3/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-05-04 17:42:32.000000 dagster-1.3.3/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1301 2023-05-04 17:42:32.000000 dagster-1.3.3/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-04 17:42:32.000000 dagster-1.3.3/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-05-04 17:42:32.724379 dagster-1.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6432 2023-05-04 17:42:14.000000 dagster-1.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.300600 dagster-1.3.4/
+-rw-r--r--   0 root         (0) root         (0)      549 2023-05-11 16:58:41.000000 dagster-1.3.4/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-05-11 16:58:41.000000 dagster-1.3.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-11 16:58:41.000000 dagster-1.3.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-05-11 16:59:05.300600 dagster-1.3.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7167 2023-05-11 16:58:41.000000 dagster-1.3.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.236600 dagster-1.3.4/dagster/
+-rw-r--r--   0 root         (0) root         (0)    26157 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5456 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.240600 dagster-1.3.4/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/snapshot_job.py
+-rw-r--r--   0 root         (0) root         (0)     5479 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.240600 dagster-1.3.4/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    51637 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.240600 dagster-1.3.4/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26783 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8186 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     5695 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    29862 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     5852 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19909 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15661 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.240600 dagster-1.3.4/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28391 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.240600 dagster-1.3.4/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    14686 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    18799 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    15269 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    16880 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9466 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.244600 dagster-1.3.4/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)    71379 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)     6217 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/pythonic_config/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12143 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    16671 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.244600 dagster-1.3.4/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13645 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.244600 dagster-1.3.4/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.256600 dagster-1.3.4/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7626 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29445 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)     3816 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    36842 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     5685 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    47566 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/asset_reconciliation_sensor.py
+-rw-r--r--   0 root         (0) root         (0)    18474 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    64232 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    24005 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/assets_job.py
+-rw-r--r--   0 root         (0) root         (0)     3681 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16105 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    45671 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4287 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    10845 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    20769 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    17905 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.256600 dagster-1.3.4/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42826 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8250 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9444 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10676 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    17845 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    14396 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8656 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    11936 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     6695 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5275 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    20546 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    39988 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    31576 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21013 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10548 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/external_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8010 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16195 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    44740 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    22898 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     5386 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/job_base.py
+-rw-r--r--   0 root         (0) root         (0)    50969 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    20308 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     6845 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      636 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8841 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.256600 dagster-1.3.4/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    32319 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8557 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)    55971 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    20758 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11927 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8041 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2867 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    22629 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19256 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7509 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/op_selection.py
+-rw-r--r--   0 root         (0) root         (0)    18908 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    37817 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      196 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    47274 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     8811 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)    27270 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/reconstruct.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.256600 dagster-1.3.4/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6670 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    18856 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    17401 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    16979 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    16162 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5398 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7806 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)    24105 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15824 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    38400 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    36722 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5189 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    10722 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    46040 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    14249 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/test_op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    12225 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    74641 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    15645 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7992 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    25453 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)     6232 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.256600 dagster-1.3.4/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    64981 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7783 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.260600 dagster-1.3.4/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38474 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    30251 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    14476 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6326 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.260600 dagster-1.3.4/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21992 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    15991 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9369 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    26845 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    27417 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    33974 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    44193 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    18544 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context_creation_job.py
+-rw-r--r--   0 root         (0) root         (0)     5149 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5426 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     9183 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8540 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    14467 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6487 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/job_execution_result.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.264600 dagster-1.3.4/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23031 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    12550 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16270 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    27355 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)     9984 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    37831 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    59386 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    15616 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    15920 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8186 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19377 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)    10329 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.264600 dagster-1.3.4/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15667 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.264600 dagster-1.3.4/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14328 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.264600 dagster-1.3.4/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.264600 dagster-1.3.4/dagster/_core/host_representation/
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33529 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    32103 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    69817 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)    11276 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/job_index.py
+-rw-r--r--   0 root         (0) root         (0)    17368 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     3606 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.264600 dagster-1.3.4/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   103988 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24318 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     4567 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.268600 dagster-1.3.4/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3639 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6629 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    17249 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.268600 dagster-1.3.4/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    11030 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.268600 dagster-1.3.4/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    21250 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)     9410 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.268600 dagster-1.3.4/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.268600 dagster-1.3.4/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18257 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.268600 dagster-1.3.4/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2815 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9421 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12099 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    16629 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/job_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14452 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/snap_to_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.276600 dagster-1.3.4/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.276600 dagster-1.3.4/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6676 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.284600 dagster-1.3.4/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      311 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      530 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      634 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7204 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/base_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.284600 dagster-1.3.4/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8736 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16247 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9545 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    23527 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/dagster_run.py
+-rw-r--r--   0 root         (0) root         (0)    11640 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14381 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3630 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     7911 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     5090 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)    78441 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7408 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    18950 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10912 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13217 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8915 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10638 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    26292 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17301 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14469 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    23189 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/root.py
+-rw-r--r--   0 root         (0) root         (0)     8509 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/root_input_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15454 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8635 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    46394 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5344 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4095 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    19749 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7375 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4863 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    11346 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13981 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    14855 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    27932 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    18920 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7298 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    35761 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/utility_ops.py
+-rw-r--r--   0 root         (0) root         (0)     4003 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4722 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    26620 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4684 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     3952 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5235 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6828 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9123 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     4399 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17726 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    10457 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10032 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/monitoring/monitoring_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16247 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    37649 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)     6639 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2722 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.232601 dagster-1.3.4/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28114 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    38178 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    18324 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4202 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    22000 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5394 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    54827 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5301 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    26359 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      222 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_loggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31794 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8004 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7467 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    37037 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5496 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.300600 dagster-1.3.4/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    23319 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8741 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     6965 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/backcompat.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    23982 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      883 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     2372 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)      344 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/internal_init.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)     9813 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    12340 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.300600 dagster-1.3.4/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    10412 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    23902 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.300600 dagster-1.3.4/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.236600 dagster-1.3.4/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-05-11 16:59:05.000000 dagster-1.3.4/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24949 2023-05-11 16:59:05.000000 dagster-1.3.4/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 16:59:05.000000 dagster-1.3.4/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-05-11 16:59:05.000000 dagster-1.3.4/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-05-11 16:59:05.000000 dagster-1.3.4/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-11 16:59:05.000000 dagster-1.3.4/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-05-11 16:59:05.304600 dagster-1.3.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6432 2023-05-11 16:58:41.000000 dagster-1.3.4/setup.py
```

### Comparing `dagster-1.3.3/COPYING` & `dagster-1.3.4/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/LICENSE` & `dagster-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/PKG-INFO` & `dagster-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.3.3
+Version: 1.3.4
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.3.3/README.md` & `dagster-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/__init__.py` & `dagster-1.3.4/dagster/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -435,15 +435,15 @@
     DagsterTypeLoaderContext as DagsterTypeLoaderContext,
     StepExecutionContext as StepExecutionContext,
     TypeCheckContext as TypeCheckContext,
 )
 from dagster._core.execution.execute_in_process_result import (
     ExecuteInProcessResult as ExecuteInProcessResult,
 )
-from dagster._core.execution.execute_job_result import ExecuteJobResult as ExecuteJobResult
+from dagster._core.execution.job_execution_result import JobExecutionResult as JobExecutionResult
 from dagster._core.execution.plan.external_step import (
     external_instance_from_step_run_ref as external_instance_from_step_run_ref,
     run_step_from_ref as run_step_from_ref,
     step_context_to_step_run_ref as step_context_to_step_run_ref,
     step_run_ref_to_step_context as step_run_ref_to_step_context,
 )
 from dagster._core.execution.validate_run_config import validate_run_config as validate_run_config
@@ -560,29 +560,35 @@
 # in `_DEPRECATED` is required  for us to generate the deprecation warning.
 
 if TYPE_CHECKING:
     ##### EXAMPLE
     # from dagster.some.module import (
     #     Foo as Foo,
     # )
-    pass
+
+    # JobExecutionResult used to be called ExecuteJobResult because it was only returned from
+    # `execute_job`.
+    from dagster._core.execution.job_execution_result import (
+        JobExecutionResult as ExecuteJobResult,  # noqa: F401
+    )
 
 
 _DEPRECATED: Final[Mapping[str, TypingTuple[str, str, str]]] = {
     ##### EXAMPLE
     # "Foo": (
     #     "dagster.some.module",
     #     "1.1.0",  # breaking version
     #     "Use Bar instead.",
     # ),
 }
 
 _DEPRECATED_RENAMED: Final[Mapping[str, TypingTuple[Callable, str]]] = {
     ##### EXAMPLE
     # "Foo": (Bar, "1.1.0"),
+    "ExecuteJobResult": (JobExecutionResult, "1.4.0"),
 }
 
 
 def __getattr__(name: str) -> TypingAny:
     if name in _DEPRECATED:
         module, breaking_version, additional_warn_text = _DEPRECATED[name]
         value = getattr(importlib.import_module(module), name)
```

### Comparing `dagster-1.3.3/dagster/_annotations.py` & `dagster-1.3.4/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_api/get_server_id.py` & `dagster-1.3.4/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_api/list_repositories.py` & `dagster-1.3.4/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_api/notebook_data.py` & `dagster-1.3.4/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_api/snapshot_execution_plan.py` & `dagster-1.3.4/dagster/_api/snapshot_execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_api/snapshot_job.py` & `dagster-1.3.4/dagster/_api/snapshot_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_api/snapshot_partition.py` & `dagster-1.3.4/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_api/snapshot_repository.py` & `dagster-1.3.4/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_api/snapshot_schedule.py` & `dagster-1.3.4/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_api/snapshot_sensor.py` & `dagster-1.3.4/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_check/README.md` & `dagster-1.3.4/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_check/__init__.py` & `dagster-1.3.4/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_cli/__init__.py` & `dagster-1.3.4/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_cli/api.py` & `dagster-1.3.4/dagster/_cli/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,16 +415,17 @@
             ).repository_load_data
         else:
             repository_load_data = None
 
         recon_job = (
             recon_job_from_origin(cast(JobPythonOrigin, dagster_run.job_code_origin))
             .with_repository_load_data(repository_load_data)
-            .subset_for_execution_from_existing_job(
-                dagster_run.solids_to_execute, dagster_run.asset_selection
+            .get_subset(
+                op_selection=dagster_run.solids_to_execute,
+                asset_selection=dagster_run.asset_selection,
             )
         )
 
         execution_plan = create_execution_plan(
             recon_job,
             run_config=dagster_run.run_config,
             step_keys_to_execute=args.step_keys_to_execute,
```

### Comparing `dagster-1.3.3/dagster/_cli/asset.py` & `dagster-1.3.4/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_cli/config_scaffolder.py` & `dagster-1.3.4/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_cli/debug.py` & `dagster-1.3.4/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_cli/dev.py` & `dagster-1.3.4/dagster/_cli/dev.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,17 +47,15 @@
 )
 @dev_command_options
 @click.option(
     "--code-server-log-level",
     help="Set the log level for code servers spun up by dagster services.",
     show_default=True,
     default="warning",
-    type=click.Choice(
-        ["critical", "error", "warning", "info", "debug", "trace"], case_sensitive=False
-    ),
+    type=click.Choice(["critical", "error", "warning", "info", "debug"], case_sensitive=False),
 )
 @click.option("--dagit-port", "-p", help="Port to use for the Dagit UI.", required=False)
 @click.option("--dagit-host", "-h", help="Host to use for the Dagit UI.", required=False)
 def dev_command(
     code_server_log_level: str,
     dagit_port: Optional[str],
     dagit_host: Optional[str],
```

### Comparing `dagster-1.3.3/dagster/_cli/instance.py` & `dagster-1.3.4/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_cli/job.py` & `dagster-1.3.4/dagster/_cli/job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_cli/load_handle.py` & `dagster-1.3.4/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_cli/project.py` & `dagster-1.3.4/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_cli/run.py` & `dagster-1.3.4/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_cli/schedule.py` & `dagster-1.3.4/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_cli/sensor.py` & `dagster-1.3.4/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_cli/utils.py` & `dagster-1.3.4/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_cli/workspace/cli_target.py` & `dagster-1.3.4/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_config/__init__.py` & `dagster-1.3.4/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_config/config_schema.py` & `dagster-1.3.4/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_config/config_type.py` & `dagster-1.3.4/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_config/errors.py` & `dagster-1.3.4/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_config/evaluate_value_result.py` & `dagster-1.3.4/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_config/field.py` & `dagster-1.3.4/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_config/field_utils.py` & `dagster-1.3.4/dagster/_config/field_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     :py:class:`~dagster.DagsterInvalidConfigError`.
 
     Args:
         fields (Dict[str, Field]):
             The specification of the config dict.
         field_aliases (Dict[str, str]):
             Maps a string key to an alias that can be used instead of the original key. For example,
-            an entry {"solids": "ops"} means that someone could use "ops" instead of "solids" as a
+            an entry {"foo": "bar"} means that someone could use "bar" instead of "foo" as a
             top level string key.
     """
 
     def __new__(
         cls,
         fields,
         description=None,
```

### Comparing `dagster-1.3.3/dagster/_config/post_process.py` & `dagster-1.3.4/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_config/primitive_mapping.py` & `dagster-1.3.4/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_config/pythonic_config/__init__.py` & `dagster-1.3.4/dagster/_config/pythonic_config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -630,43 +630,50 @@
         return coercible_to_resource.get_resource_definition()
     return coercible_to_resource
 
 
 class ConfigurableResourceFactoryResourceDefinition(ResourceDefinition, AllowDelayedDependencies):
     def __init__(
         self,
+        configurable_resource_cls: Type,
         resource_fn: ResourceFunction,
         config_schema: Any,
         description: Optional[str],
         resolve_resource_keys: Callable[[Mapping[int, str]], AbstractSet[str]],
         nested_resources: Mapping[str, CoercibleToResource],
     ):
         super().__init__(
             resource_fn=resource_fn,
             config_schema=config_schema,
             description=description,
         )
+        self._configurable_resource_cls = configurable_resource_cls
         self._resolve_resource_keys = resolve_resource_keys
         self._nested_resources = nested_resources
 
     @property
+    def configurable_resource_cls(self) -> Type:
+        return self._configurable_resource_cls
+
+    @property
     def nested_resources(
         self,
     ) -> Mapping[str, CoercibleToResource]:
         return self._nested_resources
 
     def _resolve_required_resource_keys(
         self, resource_mapping: Mapping[int, str]
     ) -> AbstractSet[str]:
         return self._resolve_resource_keys(resource_mapping)
 
 
 class ConfigurableIOManagerFactoryResourceDefinition(IOManagerDefinition, AllowDelayedDependencies):
     def __init__(
         self,
+        configurable_resource_cls: Type,
         resource_fn: ResourceFunction,
         config_schema: Any,
         description: Optional[str],
         resolve_resource_keys: Callable[[Mapping[int, str]], AbstractSet[str]],
         nested_resources: Mapping[str, CoercibleToResource],
         input_config_schema: Optional[Union[CoercableToConfigSchema, Type[Config]]] = None,
         output_config_schema: Optional[Union[CoercableToConfigSchema, Type[Config]]] = None,
@@ -686,14 +693,19 @@
             config_schema=config_schema,
             description=description,
             input_config_schema=input_config_schema_resolved,
             output_config_schema=output_config_schema_resolved,
         )
         self._resolve_resource_keys = resolve_resource_keys
         self._nested_resources = nested_resources
+        self._configurable_resource_cls = configurable_resource_cls
+
+    @property
+    def configurable_resource_cls(self) -> Type:
+        return self._configurable_resource_cls
 
     @property
     def nested_resources(
         self,
     ) -> Mapping[str, CoercibleToResource]:
         return self._nested_resources
 
@@ -831,14 +843,15 @@
 
     def _get_initialize_and_run_fn(self) -> Callable:
         return self._initialize_and_run_cm if self._is_cm_resource else self._initialize_and_run
 
     @cached_method
     def get_resource_definition(self) -> ConfigurableResourceFactoryResourceDefinition:
         return ConfigurableResourceFactoryResourceDefinition(
+            self.__class__,
             resource_fn=self._get_initialize_and_run_fn(),
             config_schema=self._config_schema,
             description=self.__doc__,
             resolve_resource_keys=self._resolve_required_resource_keys,
             nested_resources=self.nested_resources,
         )
 
@@ -1167,14 +1180,15 @@
         self,
     ) -> Mapping[str, CoercibleToResource]:
         return self._state__internal__.nested_resources
 
     @cached_method
     def get_resource_definition(self) -> ConfigurableResourceFactoryResourceDefinition:
         return ConfigurableResourceFactoryResourceDefinition(
+            self.__class__,
             resource_fn=self._state__internal__.resource_fn,
             config_schema=self._state__internal__.config_schema,
             description=self._state__internal__.description,
             resolve_resource_keys=self._resolve_required_resource_keys,
             nested_resources=self.nested_resources,
         )
 
@@ -1235,14 +1249,15 @@
     @abstractmethod
     def wrapped_resource(self) -> ResourceDefinition:
         raise NotImplementedError()
 
     @cached_method
     def get_resource_definition(self) -> ConfigurableResourceFactoryResourceDefinition:
         return ConfigurableResourceFactoryResourceDefinition(
+            self.__class__,
             resource_fn=self.wrapped_resource.resource_fn,
             config_schema=self._config_schema,
             description=self.__doc__,
             resolve_resource_keys=self._resolve_required_resource_keys,
             nested_resources=self.nested_resources,
         )
 
@@ -1312,14 +1327,15 @@
         set at runtime.
         """
         return PartialIOManager(cls, data=kwargs)
 
     @cached_method
     def get_resource_definition(self) -> ConfigurableIOManagerFactoryResourceDefinition:
         return ConfigurableIOManagerFactoryResourceDefinition(
+            self.__class__,
             resource_fn=self._get_initialize_and_run_fn(),
             config_schema=self._config_schema,
             description=self.__doc__,
             resolve_resource_keys=self._resolve_required_resource_keys,
             nested_resources=self.nested_resources,
             input_config_schema=self.__class__.input_config_schema(),
             output_config_schema=self.__class__.output_config_schema(),
@@ -1354,14 +1370,15 @@
             factory_cls: Type[ConfigurableIOManagerFactory] = cast(
                 Type[ConfigurableIOManagerFactory], self.resource_cls
             )
             input_config_schema = factory_cls.input_config_schema()
             output_config_schema = factory_cls.output_config_schema()
 
         return ConfigurableIOManagerFactoryResourceDefinition(
+            self.__class__,
             resource_fn=self._state__internal__.resource_fn,
             config_schema=self._state__internal__.config_schema,
             description=self._state__internal__.description,
             resolve_resource_keys=self._resolve_required_resource_keys,
             nested_resources=self._state__internal__.nested_resources,
             input_config_schema=input_config_schema,
             output_config_schema=output_config_schema,
@@ -1616,14 +1633,15 @@
         raise NotImplementedError(
             "Because we override resource_fn in the adapter, this is never called."
         )
 
     @cached_method
     def get_resource_definition(self) -> ConfigurableIOManagerFactoryResourceDefinition:
         return ConfigurableIOManagerFactoryResourceDefinition(
+            self.__class__,
             resource_fn=self.wrapped_io_manager.resource_fn,
             config_schema=self._config_schema,
             description=self.__doc__,
             resolve_resource_keys=self._resolve_required_resource_keys,
             nested_resources=self.nested_resources,
         )
 
@@ -1714,15 +1732,15 @@
     fields_to_omit = fields_to_omit or set()
 
     check.param_invariant(
         safe_is_subclass(model_cls, Config),
         "Config type annotation must inherit from dagster.Config",
     )
 
-    fields = {}
+    fields: Dict[str, Field] = {}
     for pydantic_field in model_cls.__fields__.values():
         if pydantic_field.name not in fields_to_omit:
             if isinstance(pydantic_field.default, Field):
                 raise DagsterInvalidDefinitionError(
                     "Using 'dagster.Field' is not supported within a Pythonic config or resource"
                     " definition. 'dagster.Field' should only be used in legacy Dagster config"
                     " schemas. Did you mean to use 'pydantic.Field' instead?"
@@ -1740,14 +1758,15 @@
                     is_resource=model_cls is not None
                     and safe_is_subclass(model_cls, ConfigurableResourceFactory),
                 )
 
     shape_cls = Permissive if model_cls.__config__.extra == Extra.allow else Shape
 
     docstring = model_cls.__doc__.strip() if model_cls.__doc__ else None
+
     return Field(config=shape_cls(fields), description=description or docstring)
 
 
 class SeparatedResourceParams(NamedTuple):
     resources: Dict[str, CoercibleToResource]
     non_resources: Dict[str, Any]
```

### Comparing `dagster-1.3.3/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.3.4/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.3.4/dagster/_config/pythonic_config/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_config/pythonic_config/utils.py` & `dagster-1.3.4/dagster/_config/pythonic_config/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_config/snap.py` & `dagster-1.3.4/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_config/source.py` & `dagster-1.3.4/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_config/stack.py` & `dagster-1.3.4/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_config/traversal_context.py` & `dagster-1.3.4/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_config/type_printer.py` & `dagster-1.3.4/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_config/validate.py` & `dagster-1.3.4/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/assets.py` & `dagster-1.3.4/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/code_pointer.py` & `dagster-1.3.4/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/container_context/config.py` & `dagster-1.3.4/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/debug.py` & `dagster-1.3.4/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/decorator_utils.py` & `dagster-1.3.4/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/__init__.py` & `dagster-1.3.4/dagster/_core/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/asset_graph.py` & `dagster-1.3.4/dagster/_core/definitions/asset_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import functools
 from collections import deque
+from datetime import datetime
 from heapq import heapify, heappop, heappush
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Callable,
     Dict,
     Iterable,
@@ -194,37 +195,43 @@
     def get_parents(self, asset_key: AssetKey) -> AbstractSet[AssetKey]:
         """Returns all assets that the given asset depends on."""
         return self._asset_dep_graph["upstream"][asset_key]
 
     def get_children_partitions(
         self,
         dynamic_partitions_store: DynamicPartitionsStore,
+        current_time: datetime,
         asset_key: AssetKey,
         partition_key: Optional[str] = None,
     ) -> AbstractSet[AssetKeyPartitionKey]:
         """Returns every partition in every of the given asset's children that depends on the given
         partition of that asset.
         """
         result: Set[AssetKeyPartitionKey] = set()
         for child_asset_key in self.get_children(asset_key):
             if self.is_partitioned(child_asset_key):
                 for child_partition_key in self.get_child_partition_keys_of_parent(
-                    dynamic_partitions_store, partition_key, asset_key, child_asset_key
+                    dynamic_partitions_store,
+                    partition_key,
+                    asset_key,
+                    child_asset_key,
+                    current_time,
                 ):
                     result.add(AssetKeyPartitionKey(child_asset_key, child_partition_key))
             else:
                 result.add(AssetKeyPartitionKey(child_asset_key))
         return result
 
     def get_child_partition_keys_of_parent(
         self,
         dynamic_partitions_store: DynamicPartitionsStore,
         parent_partition_key: Optional[str],
         parent_asset_key: AssetKey,
         child_asset_key: AssetKey,
+        current_time: datetime,
     ) -> Sequence[str]:
         """Converts a partition key from one asset to the corresponding partition keys in a downstream
         asset. Uses the existing partition mapping between the child asset and the parent asset.
 
         Args:
             parent_partition_key (Optional[str]): The partition key to convert.
             parent_asset_key (AssetKey): The asset key of the upstream asset, which the provided
@@ -255,47 +262,51 @@
             )
 
         partition_mapping = self.get_partition_mapping(child_asset_key, parent_asset_key)
         child_partitions_subset = partition_mapping.get_downstream_partitions_for_partitions(
             parent_partitions_def.empty_subset().with_partition_keys([parent_partition_key]),
             downstream_partitions_def=child_partitions_def,
             dynamic_partitions_store=dynamic_partitions_store,
+            current_time=current_time,
         )
 
         return list(child_partitions_subset.get_partition_keys())
 
     def get_parents_partitions(
         self,
         dynamic_partitions_store: DynamicPartitionsStore,
+        current_time: datetime,
         asset_key: AssetKey,
         partition_key: Optional[str] = None,
     ) -> AbstractSet[AssetKeyPartitionKey]:
         """Returns every partition in every of the given asset's parents that the given partition of
         that asset depends on.
         """
         result: Set[AssetKeyPartitionKey] = set()
         for parent_asset_key in self.get_parents(asset_key):
             if self.is_partitioned(parent_asset_key):
                 for parent_partition_key in self.get_parent_partition_keys_for_child(
                     partition_key,
                     parent_asset_key,
                     asset_key,
                     dynamic_partitions_store=dynamic_partitions_store,
+                    current_time=current_time,
                 ):
                     result.add(AssetKeyPartitionKey(parent_asset_key, parent_partition_key))
             else:
                 result.add(AssetKeyPartitionKey(parent_asset_key))
         return result
 
     def get_parent_partition_keys_for_child(
         self,
         partition_key: Optional[str],
         parent_asset_key: AssetKey,
         child_asset_key: AssetKey,
-        dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
+        dynamic_partitions_store: DynamicPartitionsStore,
+        current_time: datetime,
     ) -> Sequence[str]:
         """Converts a partition key from one asset to the corresponding partition keys in one of its
         parent assets. Uses the existing partition mapping between the child asset and the parent
         asset.
 
         Args:
             partition_key (Optional[str]): The partition key to convert.
@@ -323,14 +334,15 @@
             cast(PartitionsDefinition, child_partitions_def)
             .empty_subset()
             .with_partition_keys([partition_key])
             if partition_key
             else None,
             upstream_partitions_def=parent_partitions_def,
             dynamic_partitions_store=dynamic_partitions_store,
+            current_time=current_time,
         )
         return list(parent_partition_key_subset.get_partition_keys())
 
     def is_source(self, asset_key: AssetKey) -> bool:
         return asset_key in self.source_asset_keys or asset_key not in self.all_asset_keys
 
     def has_non_source_parents(self, asset_key: AssetKey) -> bool:
@@ -412,14 +424,15 @@
         return asset_key in self.get_parents(asset_key)
 
     def bfs_filter_subsets(
         self,
         dynamic_partitions_store: DynamicPartitionsStore,
         condition_fn: Callable[[AssetKey, Optional[PartitionsSubset]], bool],
         initial_subset: "AssetGraphSubset",
+        current_time: datetime,
     ) -> "AssetGraphSubset":
         """Returns asset partitions within the graph that satisfy supplied criteria.
 
         - Are >= initial_asset_partitions
         - Asset matches the condition_fn
         - Any of their ancestors >= initial_asset_partitions match the condition_fn.
 
@@ -466,14 +479,15 @@
                             queued_subsets_by_asset_key[child] = child_partitions_subset
                         else:
                             child_partitions_subset = (
                                 partition_mapping.get_downstream_partitions_for_partitions(
                                     partitions_subset,
                                     downstream_partitions_def=child_partitions_def,
                                     dynamic_partitions_store=dynamic_partitions_store,
+                                    current_time=current_time,
                                 )
                             )
                             prior_child_partitions_subset = queued_subsets_by_asset_key.get(child)
                             queued_subsets_by_asset_key[child] = (
                                 child_partitions_subset
                                 if not prior_child_partitions_subset
                                 else child_partitions_subset | prior_child_partitions_subset
@@ -490,14 +504,15 @@
     def bfs_filter_asset_partitions(
         self,
         dynamic_partitions_store: DynamicPartitionsStore,
         condition_fn: Callable[
             [Iterable[AssetKeyPartitionKey], AbstractSet[AssetKeyPartitionKey]], bool
         ],
         initial_asset_partitions: Iterable[AssetKeyPartitionKey],
+        evaluation_time: datetime,
     ) -> AbstractSet[AssetKeyPartitionKey]:
         """Returns asset partitions within the graph that satisfy supplied criteria.
 
         - Are >= initial_asset_partitions
         - Match the condition_fn
         - Any of their ancestors >= initial_asset_partitions match the condition_fn
 
@@ -517,15 +532,18 @@
             candidates_unit = queue.dequeue()
 
             if condition_fn(candidates_unit, result):
                 result.update(candidates_unit)
 
                 for candidate in candidates_unit:
                     for child in self.get_children_partitions(
-                        dynamic_partitions_store, candidate.asset_key, candidate.partition_key
+                        dynamic_partitions_store,
+                        evaluation_time,
+                        candidate.asset_key,
+                        candidate.partition_key,
                     ):
                         if child not in all_nodes:
                             queue.enqueue(child)
                             all_nodes.add(child)
 
         return result
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.3.4/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/asset_in.py` & `dagster-1.3.4/dagster/_core/definitions/asset_in.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
         check.invariant(
             not (key and key_prefix), "key and key_prefix cannot both be set on AssetIn"
         )
 
         return super(AssetIn, cls).__new__(
             cls,
-            key=AssetKey.from_coerceable(key) if key is not None else None,
+            key=AssetKey.from_coercible(key) if key is not None else None,
             metadata=check.opt_inst_param(metadata, "metadata", Mapping),
             key_prefix=check.opt_list_param(key_prefix, "key_prefix", of_type=str),
             input_manager_key=check.opt_str_param(input_manager_key, "input_manager_key"),
             partition_mapping=check.opt_inst_param(
                 partition_mapping, "partition_mapping", PartitionMapping
             ),
             dagster_type=NoValueSentinel
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/asset_layer.py` & `dagster-1.3.4/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/asset_out.py` & `dagster-1.3.4/dagster/_core/definitions/asset_out.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
     ):
         if isinstance(key_prefix, str):
             key_prefix = [key_prefix]
 
         return super(AssetOut, cls).__new__(
             cls,
-            key=AssetKey.from_coerceable(key) if key is not None else None,
+            key=AssetKey.from_coercible(key) if key is not None else None,
             key_prefix=check.opt_list_param(key_prefix, "key_prefix", of_type=str),
             dagster_type=NoValueSentinel
             if dagster_type is NoValueSentinel
             else resolve_dagster_type(dagster_type),
             description=check.opt_str_param(description, "description"),
             is_required=check.bool_param(is_required, "is_required"),
             io_manager_key=check.opt_str_param(
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/asset_reconciliation_sensor.py` & `dagster-1.3.4/dagster/_core/definitions/asset_reconciliation_sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,15 +324,17 @@
 
     result = AssetGraphSubset(asset_graph)
     for asset_backfill in asset_backfills:
         if asset_backfill.serialized_asset_backfill_data is None:
             check.failed("Asset backfill missing serialized_asset_backfill_data")
 
         asset_backfill_data = AssetBackfillData.from_serialized(
-            asset_backfill.serialized_asset_backfill_data, asset_graph
+            asset_backfill.serialized_asset_backfill_data,
+            asset_graph,
+            asset_backfill.backfill_timestamp,
         )
 
         result |= asset_backfill_data.target_subset
 
     return result
 
 
@@ -357,30 +359,37 @@
 
     for asset_key in target_asset_keys_and_parents:
         if asset_graph.is_source(asset_key):
             if asset_graph.is_observable(asset_key) and instance_queryer.new_version_exists(
                 observable_source_asset_key=asset_key, after_cursor=latest_storage_id
             ):
                 for child in asset_graph.get_children_partitions(
-                    instance_queryer, asset_key, partition_key=None
+                    dynamic_partitions_store=instance_queryer,
+                    current_time=instance_queryer.evaluation_time,
+                    asset_key=asset_key,
+                    partition_key=None,
                 ):
                     if child.asset_key in target_asset_keys:
                         result_asset_partitions.add(child)
 
             continue
 
         partitions_def = asset_graph.get_partitions_def(asset_key)
         latest_record = instance_queryer.get_latest_materialization_record(
             asset_key, after_cursor=latest_storage_id
         )
         if latest_record is None:
             continue
 
         if partitions_def is None:
-            for child in asset_graph.get_children_partitions(instance_queryer, asset_key):
+            for child in asset_graph.get_children_partitions(
+                dynamic_partitions_store=instance_queryer,
+                current_time=instance_queryer.evaluation_time,
+                asset_key=asset_key,
+            ):
                 if (
                     child.asset_key in target_asset_keys
                     and not instance_queryer.is_asset_planned_for_run(latest_record.run_id, child)
                 ):
                     result_asset_partitions.add(child)
         else:
             # for partitioned assets, we want the set of all asset partitions that have been
@@ -409,14 +418,15 @@
                     # the child asset
                     partition_mapping = asset_graph.get_partition_mapping(child, asset_key)
                     child_partitions_subset = (
                         partition_mapping.get_downstream_partitions_for_partitions(
                             partitions_subset,
                             downstream_partitions_def=child_partitions_def,
                             dynamic_partitions_store=instance_queryer,
+                            current_time=instance_queryer.evaluation_time,
                         )
                     )
                     for child_partition in child_partitions_subset.get_partition_keys():
                         # we need to see if the child is planned for the same run, but this is
                         # expensive, so we try to avoid doing so in as many situations as possible
                         child_asset_partition = AssetKeyPartitionKey(child, child_partition)
                         if not can_reconcile_fn(child_asset_partition):
@@ -447,15 +457,14 @@
 
 
 def find_never_materialized_or_requested_root_asset_partitions(
     instance_queryer: "CachingInstanceQueryer",
     cursor: AssetReconciliationCursor,
     target_asset_keys: AbstractSet[AssetKey],
     asset_graph: AssetGraph,
-    current_time: datetime.datetime,
 ) -> Tuple[
     Iterable[AssetKeyPartitionKey], AbstractSet[AssetKey], Mapping[AssetKey, AbstractSet[str]]
 ]:
     """Finds asset partitions that have never been materialized or requested and that have no
     parents.
 
     Returns:
@@ -473,16 +482,16 @@
         if asset_graph.is_partitioned(asset_key):
             auto_materialize_policy = check.not_none(
                 get_implicit_auto_materialize_policy(asset_graph, asset_key)
             )
             for partition_key in cursor.get_never_requested_never_materialized_partitions(
                 asset_key,
                 asset_graph,
-                instance_queryer,
-                current_time,
+                dynamic_partitions_store=instance_queryer,
+                current_time=instance_queryer.evaluation_time,
                 time_window_partition_scope=auto_materialize_policy.time_window_partition_scope,
             ):
                 asset_partition = AssetKeyPartitionKey(asset_key, partition_key)
                 if instance_queryer.get_latest_materialization_record(asset_partition, None):
                     newly_materialized_root_partitions_by_asset_key[asset_key].add(partition_key)
                 else:
                     never_materialized_or_requested.add(asset_partition)
@@ -503,31 +512,31 @@
 
 def determine_asset_partitions_to_reconcile(
     instance_queryer: "CachingInstanceQueryer",
     cursor: AssetReconciliationCursor,
     target_asset_keys: AbstractSet[AssetKey],
     target_asset_keys_and_parents: AbstractSet[AssetKey],
     asset_graph: AssetGraph,
-    current_time: datetime.datetime,
 ) -> Tuple[
     AbstractSet[AssetKeyPartitionKey],
     AbstractSet[AssetKey],
     Mapping[AssetKey, AbstractSet[str]],
     Optional[int],
 ]:
+    evaluation_time = instance_queryer.evaluation_time
+
     (
         never_materialized_or_requested_roots,
         newly_materialized_root_asset_keys,
         newly_materialized_root_partitions_by_asset_key,
     ) = find_never_materialized_or_requested_root_asset_partitions(
         instance_queryer=instance_queryer,
         cursor=cursor,
         target_asset_keys=target_asset_keys,
         asset_graph=asset_graph,
-        current_time=current_time,
     )
 
     # a filter for eliminating candidates
     def can_reconcile_candidate(candidate: AssetKeyPartitionKey) -> bool:
         auto_materialize_policy = get_implicit_auto_materialize_policy(
             asset_graph=asset_graph, asset_key=candidate.asset_key
         )
@@ -542,15 +551,15 @@
             and has_one_dimension_time_window_partitioning(partitions_def)
             and not can_reconcile_time_window_partition(
                 partitions_def=cast(
                     Union[TimeWindowPartitionsDefinition, MultiPartitionsDefinition], partitions_def
                 ),
                 partition_key=candidate.partition_key,
                 time_window_partition_scope=auto_materialize_policy.time_window_partition_scope,
-                current_time=current_time,
+                current_time=evaluation_time,
             )
         ):
             return False
         # the policy does not allow for materializing missing partitions and it's missing
         elif not auto_materialize_policy.on_missing and not instance_queryer.materialization_exists(
             candidate
         ):
@@ -576,17 +585,15 @@
         asset_graph: AssetGraph,
         candidate: AssetKeyPartitionKey,
         to_reconcile: AbstractSet[AssetKeyPartitionKey],
     ) -> bool:
         from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 
         for parent in asset_graph.get_parents_partitions(
-            instance_queryer,
-            candidate.asset_key,
-            candidate.partition_key,
+            instance_queryer, evaluation_time, candidate.asset_key, candidate.partition_key
         ):
             if instance_queryer.is_reconciled(asset_partition=parent, asset_graph=asset_graph):
                 continue
 
             if not (
                 parent in to_reconcile
                 # if they don't have the same partitioning, then we can't launch a run that
@@ -647,14 +654,15 @@
 
     to_reconcile = asset_graph.bfs_filter_asset_partitions(
         instance_queryer,
         lambda candidates_unit, to_reconcile: should_reconcile(
             asset_graph, candidates_unit, to_reconcile
         ),
         set(itertools.chain(never_materialized_or_requested_roots, stale_candidates)),
+        evaluation_time,
     )
 
     return (
         to_reconcile,
         newly_materialized_root_asset_keys,
         newly_materialized_root_partitions_by_asset_key,
         latest_storage_id,
@@ -841,15 +849,15 @@
     cursor: AssetReconciliationCursor,
     run_tags: Optional[Mapping[str, str]],
 ):
     from dagster._utils.caching_instance_queryer import CachingInstanceQueryer  # expensive import
 
     current_time = pendulum.now("UTC")
 
-    instance_queryer = CachingInstanceQueryer(instance=instance)
+    instance_queryer = CachingInstanceQueryer(instance=instance, evaluation_time=current_time)
 
     target_parent_asset_keys = {
         parent
         for target_asset_key in target_asset_keys
         for parent in asset_graph.get_parents(target_asset_key)
     }
     target_asset_keys_and_parents = target_asset_keys | target_parent_asset_keys
@@ -880,15 +888,14 @@
         latest_storage_id,
     ) = determine_asset_partitions_to_reconcile(
         instance_queryer=instance_queryer,
         asset_graph=asset_graph,
         cursor=cursor,
         target_asset_keys=target_asset_keys,
         target_asset_keys_and_parents=target_asset_keys_and_parents,
-        current_time=current_time,
     )
 
     run_requests = build_run_requests(
         asset_partitions_to_reconcile | asset_partitions_to_reconcile_for_freshness,
         asset_graph,
         run_tags,
     )
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/asset_selection.py` & `dagster-1.3.4/dagster/_core/definitions/asset_selection.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,20 @@
     fetch_sources,
     parse_clause,
 )
 from dagster._utils.backcompat import deprecation_warning
 
 from .asset_graph import AssetGraph
 from .assets import AssetsDefinition
-from .events import AssetKey, CoercibleToAssetKey
+from .events import (
+    AssetKey,
+    CoercibleToAssetKey,
+    CoercibleToAssetKeyPrefix,
+    key_prefix_from_coercible,
+)
 from .source_asset import SourceAsset
 
 CoercibleToAssetSelection: TypeAlias = Union[
     str,
     Sequence[str],
     Sequence[AssetKey],
     Sequence[Union["AssetsDefinition", "SourceAsset"]],
@@ -88,23 +93,39 @@
 
                 AssetSelection.keys("a", "b")
 
                 asset_key_list = [AssetKey(["a"]), AssetKey(["b"])]
                 AssetSelection.keys(*asset_key_list)
         """
         _asset_keys = [
-            AssetKey.from_user_string(key)
-            if isinstance(key, str)
-            else AssetKey.from_coerceable(key)
+            AssetKey.from_user_string(key) if isinstance(key, str) else AssetKey.from_coercible(key)
             for key in asset_keys
         ]
         return KeysAssetSelection(*_asset_keys)
 
     @public
     @staticmethod
+    def key_prefixes(*key_prefixes: CoercibleToAssetKeyPrefix) -> "KeyPrefixesAssetSelection":
+        """Returns a selection that includes assets that match any of the provided key prefixes.
+
+        Examples:
+            .. code-block:: python
+
+              # match any asset key where the first segment is equal to "a" or "b"
+              # e.g. AssetKey(["a", "b", "c"]) would match, but AssetKey(["abc"]) would not.
+              AssetSelection.key_prefixes("a", "b")
+
+              # match any asset key where the first two segments are ["a", "b"] or ["a", "c"]
+              AssetSelection.key_prefixes(["a", "b"], ["a", "c"])
+        """
+        _asset_key_prefixes = [key_prefix_from_coercible(key_prefix) for key_prefix in key_prefixes]
+        return KeyPrefixesAssetSelection(*_asset_key_prefixes)
+
+    @public
+    @staticmethod
     def groups(*group_strs) -> "GroupsAssetSelection":
         """Returns a selection that includes assets that belong to any of the provided groups."""
         check.tuple_param(group_strs, "group_strs", of_type=str)
         return GroupsAssetSelection(*group_strs)
 
     @public
     def downstream(
@@ -393,14 +414,26 @@
                 f"AssetKey(s) {invalid_keys} were selected, but no AssetsDefinition objects supply "
                 "these keys. Make sure all keys are spelled correctly, and all AssetsDefinitions "
                 "are correctly added to the `Definitions`."
             )
         return specified_keys
 
 
+class KeyPrefixesAssetSelection(AssetSelection):
+    def __init__(self, *key_prefixes: Sequence[str]):
+        self._key_prefixes = key_prefixes
+
+    def resolve_inner(self, asset_graph: AssetGraph) -> AbstractSet[AssetKey]:
+        return {
+            key
+            for key in asset_graph.all_asset_keys
+            if any(key.has_prefix(prefix) for prefix in self._key_prefixes)
+        }
+
+
 class OrAssetSelection(AssetSelection):
     def __init__(self, left: AssetSelection, right: AssetSelection):
         self._left = left
         self._right = right
 
     def resolve_inner(self, asset_graph: AssetGraph) -> AbstractSet[AssetKey]:
         return self._left.resolve_inner(asset_graph) | self._right.resolve_inner(asset_graph)
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.3.4/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/assets.py` & `dagster-1.3.4/dagster/_core/definitions/assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 from dagster._annotations import public
 from dagster._core.decorator_utils import get_function_params
 from dagster._core.definitions.asset_layer import get_dep_node_handles_of_graph_backed_asset
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.definitions.input import In
 from dagster._core.definitions.metadata import ArbitraryMetadataMapping
+from dagster._core.definitions.op_selection import get_graph_subset
 from dagster._core.definitions.time_window_partition_mapping import TimeWindowPartitionMapping
 from dagster._core.definitions.time_window_partitions import TimeWindowPartitionsDefinition
 from dagster._core.errors import DagsterInvalidDefinitionError, DagsterInvalidInvocationError
-from dagster._core.selector.subset_selector import SelectionTree
 from dagster._core.types.dagster_type import Nothing
 from dagster._utils import IHasInternalInit
 from dagster._utils.backcompat import (
     ExperimentalWarning,
     deprecation_warning,
     experimental_arg_warning,
 )
@@ -985,47 +985,31 @@
         )
 
     def _subset_graph_backed_asset(
         self,
         selected_asset_keys: AbstractSet[AssetKey],
     ):
         from dagster._core.definitions.graph_definition import GraphDefinition
-        from dagster._core.selector.subset_selector import (
-            convert_dot_separated_string_to_selection_tree,
-        )
-
-        from .job_definition import get_subselected_graph_definition
 
         if not isinstance(self.node_def, GraphDefinition):
             raise DagsterInvalidInvocationError(
                 "Method _subset_graph_backed_asset cannot subset an asset that is not a graph"
             )
 
         # All asset keys in selected_asset_keys are outputted from the same top-level graph backed asset
         dep_node_handles_by_asset_key = get_dep_node_handles_of_graph_backed_asset(
             self.node_def, self
         )
         op_selection: List[str] = []
         for asset_key in selected_asset_keys:
             dep_node_handles = dep_node_handles_by_asset_key[asset_key]
             for dep_node_handle in dep_node_handles:
-                str_op_path = ".".join(dep_node_handle.path[1:])
-                op_selection.append(str_op_path)
-
-        # Pass an op selection into the original job containing only the ops necessary to
-        # generate the selected assets. The ops should all be nested within a top-level graph
-        # node in the original job.
-
-        op_selection_tree: SelectionTree = {}
-        for item in op_selection:
-            convert_dot_separated_string_to_selection_tree(
-                op_selection_tree, splits=item.split(".")
-            )
+                op_selection.append(".".join(dep_node_handle.path[1:]))
 
-        return get_subselected_graph_definition(self.node_def, op_selection_tree)
+        return get_graph_subset(self.node_def, op_selection)
 
     def subset_for(
         self,
         selected_asset_keys: AbstractSet[AssetKey],
     ) -> "AssetsDefinition":
         """Create a subset of this AssetsDefinition that will only materialize the assets in the
         selected set.
@@ -1130,15 +1114,15 @@
         if len(self.keys) > 1:
             check.invariant(
                 key is not None,
                 "The 'key' argument is required when there are multiple assets to choose from",
             )
 
         if key is not None:
-            resolved_key = AssetKey.from_coerceable(key)
+            resolved_key = AssetKey.from_coercible(key)
             check.invariant(
                 resolved_key in self.keys, f"Key {resolved_key} not found in AssetsDefinition"
             )
         else:
             resolved_key = self.key
 
         output_names = [
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/assets_job.py` & `dagster-1.3.4/dagster/_core/definitions/assets_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.3.4/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.3.4/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/composition.py` & `dagster-1.3.4/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/config.py` & `dagster-1.3.4/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/configurable.py` & `dagster-1.3.4/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/data_time.py` & `dagster-1.3.4/dagster/_core/definitions/data_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
                     asset_key: datetime.datetime.fromtimestamp(
                         record_timestamp, tz=datetime.timezone.utc
                     )
                 }
             else:
                 return {}
 
-        data_time_by_key = {}
+        data_time_by_key: Dict[AssetKey, Optional[datetime.datetime]] = {}
         for parent_key, parent_record in upstream_records_by_key.items():
             # recurse to find the data times of this parent
             for upstream_key, data_time in self._calculate_data_time_by_key(
                 asset_key=parent_key,
                 record_id=parent_record.storage_id,
                 record_timestamp=parent_record.event_log_entry.timestamp,
                 record_tags=make_hashable(
@@ -231,16 +231,17 @@
                 ),
                 current_time=current_time,
             ).items():
                 # if root data is missing, this overrides other values
                 if data_time is None:
                     data_time_by_key[upstream_key] = None
                 else:
-                    data_time_by_key[upstream_key] = min(
-                        data_time_by_key.get(upstream_key, data_time), data_time
+                    cur_data_time = data_time_by_key.get(upstream_key, data_time)
+                    data_time_by_key[upstream_key] = (
+                        min(cur_data_time, data_time) if cur_data_time is not None else None
                     )
 
         return data_time_by_key
 
     ####################
     # OBSERVABLE SOURCE DATA TIME
     ####################
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/data_version.py` & `dagster-1.3.4/dagster/_core/definitions/data_version.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.3.4/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.3.4/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.3.4/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.3.4/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.3.4/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.3.4/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.3.4/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.3.4/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.3.4/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.3.4/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.3.4/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.3.4/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/definitions_class.py` & `dagster-1.3.4/dagster/_core/definitions/definitions_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/dependency.py` & `dagster-1.3.4/dagster/_core/definitions/dependency.py`

 * *Files 0% similar despite different names*

```diff
@@ -582,14 +582,18 @@
     def node_name(self) -> str:
         return self.node.name
 
     @property
     def is_dynamic(self) -> bool:
         return self.output_def.is_dynamic
 
+    @property
+    def output_name(self) -> str:
+        return self.output_def.name
+
 
 class DependencyType(Enum):
     DIRECT = "DIRECT"
     FAN_IN = "FAN_IN"
     DYNAMIC_COLLECT = "DYNAMIC_COLLECT"
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/events.py` & `dagster-1.3.4/dagster/_core/definitions/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,28 +155,31 @@
     def from_graphql_input(graphql_input_asset_key: Mapping[str, Sequence[str]]) -> "AssetKey":
         return AssetKey(graphql_input_asset_key["path"])
 
     def to_graphql_input(self) -> Mapping[str, Sequence[str]]:
         return {"path": self.path}
 
     @staticmethod
-    def from_coerceable(arg: "CoercibleToAssetKey") -> "AssetKey":
+    def from_coercible(arg: "CoercibleToAssetKey") -> "AssetKey":
         if isinstance(arg, AssetKey):
             return check.inst_param(arg, "arg", AssetKey)
         elif isinstance(arg, str):
             return AssetKey([arg])
         elif isinstance(arg, list):
             check.list_param(arg, "arg", of_type=str)
             return AssetKey(arg)
         elif isinstance(arg, tuple):
             check.tuple_param(arg, "arg", of_type=str)
             return AssetKey(arg)
         else:
             check.failed(f"Unexpected type for AssetKey: {type(arg)}")
 
+    def has_prefix(self, prefix: Sequence[str]) -> bool:
+        return len(self.path) >= len(prefix) and self.path[: len(prefix)] == prefix
+
 
 class AssetKeyPartitionKey(NamedTuple):
     """An AssetKey with an (optional) partition key. Refers either to a non-partitioned asset or a
     partition of a partitioned asset.
     """
 
     asset_key: AssetKey
@@ -186,26 +189,31 @@
 CoercibleToAssetKey = Union[AssetKey, str, Sequence[str]]
 CoercibleToAssetKeyPrefix = Union[str, Sequence[str]]
 
 
 def check_opt_coercible_to_asset_key_prefix_param(
     prefix: Optional[CoercibleToAssetKeyPrefix], param_name: str
 ) -> Optional[Sequence[str]]:
-    if prefix is None:
-        return prefix
-    elif isinstance(prefix, str):
-        return [prefix]
-    elif isinstance(prefix, list):
-        return prefix
-    else:
+    try:
+        return key_prefix_from_coercible(prefix) if prefix is not None else None
+    except check.CheckError:
         raise check.ParameterCheckError(
             f'Param "{param_name}" is not a string or a sequence of strings'
         )
 
 
+def key_prefix_from_coercible(key_prefix: CoercibleToAssetKeyPrefix) -> Sequence[str]:
+    if isinstance(key_prefix, str):
+        return [key_prefix]
+    elif isinstance(key_prefix, list):
+        return key_prefix
+    else:
+        check.failed(f"Unexpected type for key_prefix: {type(key_prefix)}")
+
+
 DynamicAssetKey = Callable[["OutputContext"], Optional[AssetKey]]
 
 
 @whitelist_for_serdes
 class AssetLineageInfo(
     NamedTuple("_AssetLineageInfo", [("asset_key", AssetKey), ("partitions", AbstractSet[str])])
 ):
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/executor_definition.py` & `dagster-1.3.4/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/external_asset_graph.py` & `dagster-1.3.4/dagster/_core/definitions/external_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/freshness_policy.py` & `dagster-1.3.4/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.3.4/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
                 new_cursor = FreshnessPolicySensorCursor({})
                 context.update_cursor(new_cursor.to_json())
                 yield SkipReason(f"Initializing {name}.")
                 return
 
             evaluation_time = pendulum.now("UTC")
             asset_graph = context.repository_def.asset_graph
-            instance_queryer = CachingInstanceQueryer(context.instance)
+            instance_queryer = CachingInstanceQueryer(context.instance, evaluation_time)
             data_time_resolver = CachingDataTimeResolver(
                 instance_queryer=instance_queryer, asset_graph=asset_graph
             )
             monitored_keys = asset_selection.resolve(asset_graph)
 
             # get the previous status from the cursor
             previous_minutes_late_by_key = FreshnessPolicySensorCursor.from_json(
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/graph_definition.py` & `dagster-1.3.4/dagster/_core/definitions/graph_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -642,15 +642,15 @@
             hook_defs=hooks,
             version_strategy=version_strategy,
             op_retry_policy=op_retry_policy,
             asset_layer=asset_layer,
             input_values=input_values,
             _subset_selection_data=_asset_selection_data,
             _was_explicitly_provided_resources=None,  # None means this is determined by whether resource_defs contains any explicitly provided resources
-        ).get_job_def_for_subset_selection(op_selection)
+        ).get_subset(op_selection=op_selection)
 
     def coerce_to_job(self) -> "JobDefinition":
         # attempt to coerce a Graph in to a Job, raising a useful error if it doesn't work
         try:
             return self.to_job()
         except DagsterInvalidDefinitionError as err:
             raise DagsterInvalidDefinitionError(
@@ -710,15 +710,15 @@
 
         ephemeral_job = JobDefinition(
             name=self._name,
             graph_def=self,
             executor_def=execute_in_process_executor,
             resource_defs=resource_defs,
             input_values=input_values,
-        ).get_job_def_for_subset_selection(op_selection)
+        ).get_subset(op_selection=op_selection)
 
         run_config = run_config if run_config is not None else {}
         op_selection = check.opt_sequence_param(op_selection, "op_selection", str)
 
         return ephemeral_job.execute_in_process(
             run_config=run_config,
             instance=instance,
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/hook_definition.py` & `dagster-1.3.4/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/hook_invocation.py` & `dagster-1.3.4/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/inference.py` & `dagster-1.3.4/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/input.py` & `dagster-1.3.4/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/instigation_logger.py` & `dagster-1.3.4/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/job_definition.py` & `dagster-1.3.4/dagster/_core/definitions/job_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,40 +11,35 @@
     Iterable,
     List,
     Mapping,
     Optional,
     Sequence,
     Set,
     Tuple,
-    Type,
     Union,
     cast,
 )
 
 from typing_extensions import Self
 
 import dagster._check as check
 from dagster._annotations import public
 from dagster._config import Field, Shape, StringSource
 from dagster._config.config_type import ConfigType
 from dagster._config.validate import validate_config
-from dagster._core.definitions.composition import MappedInputPlaceholder
 from dagster._core.definitions.dependency import (
-    DynamicCollectDependencyDefinition,
-    IDependencyDefinition,
-    MultiDependencyDefinition,
     Node,
     NodeHandle,
     NodeInputHandle,
     NodeInvocation,
-    NodeOutput,
 )
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.node_definition import NodeDefinition
 from dagster._core.definitions.op_definition import OpDefinition
+from dagster._core.definitions.op_selection import OpSelection, get_graph_subset
 from dagster._core.definitions.partition import DynamicPartitionsDefinition
 from dagster._core.definitions.policy import RetryPolicy
 from dagster._core.definitions.resource_requirement import (
     ResourceRequirement,
     ensure_requirements_satisfied,
 )
 from dagster._core.definitions.utils import check_valid_name
@@ -54,33 +49,28 @@
     DagsterInvalidInvocationError,
     DagsterInvalidSubsetError,
     DagsterInvariantViolationError,
 )
 from dagster._core.selector.subset_selector import (
     AssetSelectionData,
     OpSelectionData,
-    SelectionTreeBranch,
-    SelectionTreeLeaf,
-    parse_op_selection,
 )
 from dagster._core.storage.io_manager import IOManagerDefinition, io_manager
 from dagster._core.storage.tags import MEMOIZED_RUN_TAG
 from dagster._core.types.dagster_type import DagsterType
 from dagster._core.utils import str_format_set
 from dagster._utils import IHasInternalInit
 from dagster._utils.backcompat import deprecation_warning, experimental_class_warning
 from dagster._utils.merger import merge_dicts
 
 from .asset_layer import AssetLayer, build_asset_selection_job
 from .config import ConfigMapping
 from .dependency import (
-    DependencyDefinition,
     DependencyMapping,
     DependencyStructure,
-    GraphNode,
     OpNode,
 )
 from .executor_definition import ExecutorDefinition, multi_or_in_process_executor
 from .graph_definition import GraphDefinition, SubselectedGraphDefinition
 from .hook_definition import HookDefinition
 from .logger_definition import LoggerDefinition
 from .metadata import MetadataValue, RawMetadataValue, normalize_metadata
@@ -653,16 +643,17 @@
             description=self.description,
             partitions_def=self.partitions_def,
             metadata=self.metadata,
             _subset_selection_data=None,  # this is added below
             _was_explicitly_provided_resources=True,
         )
 
-        ephemeral_job = ephemeral_job.get_job_def_for_subset_selection(
-            op_selection, frozenset(asset_selection) if asset_selection else None
+        ephemeral_job = ephemeral_job.get_subset(
+            op_selection=op_selection,
+            asset_selection=frozenset(asset_selection) if asset_selection else None,
         )
 
         merged_tags = merge_dicts(self.tags, tags or {})
         if partition_key:
             if not (self.partitions_def and self.partitioned_config):
                 check.failed("Attempted to execute a partitioned run for a non-partitioned job")
             self.partitions_def.validate_partition_key(
@@ -704,20 +695,21 @@
         return (
             self._subset_selection_data
             if isinstance(self._subset_selection_data, AssetSelectionData)
             else None
         )
 
     @property
-    def is_subset_job(self) -> bool:
+    def is_subset(self) -> bool:
         return bool(self._subset_selection_data)
 
-    def get_job_def_for_subset_selection(
+    def get_subset(
         self,
-        op_selection: Optional[Sequence[str]] = None,
+        *,
+        op_selection: Optional[Iterable[str]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
     ) -> Self:
         check.invariant(
             not (op_selection and asset_selection),
             (
                 "op_selection and asset_selection cannot both be provided as args to"
                 " execute_in_process"
@@ -772,48 +764,45 @@
             tags=self.tags,
             asset_selection=asset_selection,
             asset_selection_data=asset_selection_data,
             config=self.config_mapping or self.partitioned_config,
         )
         return new_job
 
-    def _get_job_def_for_op_selection(self, op_selection: Sequence[str]) -> Self:
-        resolved_op_selection_dict = parse_op_selection(self, op_selection)
-
+    def _get_job_def_for_op_selection(self, op_selection: Iterable[str]) -> Self:
         try:
-            sub_graph = get_subselected_graph_definition(self.graph, resolved_op_selection_dict)
+            sub_graph = get_graph_subset(self.graph, op_selection)
 
             # if explicit config was passed the config_mapping that resolves the defaults implicitly is
             # very unlikely to work. The job will still present the default config in dagit.
             config = (
                 None
                 if self.run_config is not None
                 else self.config_mapping or self.partitioned_config
             )
 
             return self._copy(
                 config=config,
                 graph_def=sub_graph,
                 _subset_selection_data=OpSelectionData(
-                    op_selection=op_selection,
-                    resolved_op_selection=set(
-                        resolved_op_selection_dict.keys()
-                    ),  # equivalent to solids_to_execute. currently only gets top level nodes.
+                    op_selection=list(op_selection),
+                    resolved_op_selection=OpSelection(op_selection).resolve(self.graph),
                     parent_job_def=self,  # used by job snapshot lineage
                 ),
                 # TODO: subset this structure.
                 # https://github.com/dagster-io/dagster/issues/7541
                 asset_layer=self.asset_layer,
             )
         except DagsterInvalidDefinitionError as exc:
             # This handles the case when you construct a subset such that an unsatisfied
             # input cannot be loaded from config. Instead of throwing a DagsterInvalidDefinitionError,
             # we re-raise a DagsterInvalidSubsetError.
+            node_paths = OpSelection(op_selection).resolve(self.graph)
             raise DagsterInvalidSubsetError(
-                f"The attempted subset {str_format_set(resolved_op_selection_dict)} for graph "
+                f"The attempted subset {str_format_set(node_paths)} for graph "
                 f"{self.graph.name} results in an invalid graph."
             ) from exc
 
     @public
     def run_request_for_partition(
         self,
         partition_key: str,
@@ -964,14 +953,22 @@
 
     def with_executor_def(self, executor_def: ExecutorDefinition) -> "JobDefinition":
         return self._copy(executor_def=executor_def)
 
     def with_logger_defs(self, logger_defs: Mapping[str, LoggerDefinition]) -> "JobDefinition":
         return self._copy(logger_defs=logger_defs)
 
+    @property
+    def op_selection(self) -> Optional[AbstractSet[str]]:
+        return set(self.op_selection_data.op_selection) if self.op_selection_data else None
+
+    @property
+    def asset_selection(self) -> Optional[AbstractSet[AssetKey]]:
+        return self.asset_selection_data.asset_selection if self.asset_selection_data else None
+
 
 def _swap_default_io_man(resources: Mapping[str, ResourceDefinition], job: JobDefinition):
     """Used to create the user facing experience of the default io_manager
     switching to in-memory when using execute_in_process.
     """
     from dagster._core.storage.mem_io_manager import mem_io_manager
 
@@ -982,120 +979,14 @@
         updated_resources = dict(resources)
         updated_resources[DEFAULT_IO_MANAGER_KEY] = mem_io_manager
         return updated_resources
 
     return resources
 
 
-def _dep_key_of(node: Node) -> NodeInvocation:
-    return NodeInvocation(
-        name=node.definition.name,
-        alias=node.name,
-        tags=node.tags,
-        hook_defs=node.hook_defs,
-        retry_policy=node.retry_policy,
-    )
-
-
-def get_subselected_graph_definition(
-    graph: GraphDefinition,
-    resolved_op_selection_dict: SelectionTreeBranch,
-    parent_handle: Optional[NodeHandle] = None,
-) -> SubselectedGraphDefinition:
-    deps: Dict[
-        NodeInvocation,
-        Dict[str, IDependencyDefinition],
-    ] = {}
-
-    selected_nodes: List[Tuple[str, NodeDefinition]] = []
-
-    for node in graph.nodes_in_topological_order:
-        node_handle = NodeHandle(node.name, parent=parent_handle)
-        # skip if the node isn't selected
-        if node.name not in resolved_op_selection_dict:
-            continue
-
-        # rebuild graph if any nodes inside the graph are selected
-        definition: Union[SubselectedGraphDefinition, NodeDefinition]
-        selection_node = resolved_op_selection_dict[node.name]
-        if isinstance(node, GraphNode) and not isinstance(selection_node, SelectionTreeLeaf):
-            definition = get_subselected_graph_definition(
-                node.definition,
-                selection_node,
-                parent_handle=node_handle,
-            )
-        # use definition if the node as a whole is selected. this includes selecting the entire graph
-        else:
-            definition = node.definition
-        selected_nodes.append((node.name, definition))
-
-        # build dependencies for the node. we do it for both cases because nested graphs can have
-        # inputs and outputs too
-        deps[_dep_key_of(node)] = {}
-        for node_input in node.inputs():
-            if graph.dependency_structure.has_direct_dep(node_input):
-                node_output = graph.dependency_structure.get_direct_dep(node_input)
-                if node_output.node.name in resolved_op_selection_dict:
-                    deps[_dep_key_of(node)][node_input.input_def.name] = DependencyDefinition(
-                        node=node_output.node.name, output=node_output.output_def.name
-                    )
-            elif graph.dependency_structure.has_dynamic_fan_in_dep(node_input):
-                node_output = graph.dependency_structure.get_dynamic_fan_in_dep(node_input)
-                if node_output.node.name in resolved_op_selection_dict:
-                    deps[_dep_key_of(node)][
-                        node_input.input_def.name
-                    ] = DynamicCollectDependencyDefinition(
-                        node_name=node_output.node.name,
-                        output_name=node_output.output_def.name,
-                    )
-            elif graph.dependency_structure.has_fan_in_deps(node_input):
-                outputs = graph.dependency_structure.get_fan_in_deps(node_input)
-                multi_dependencies = [
-                    DependencyDefinition(
-                        node=output_handle.node.name, output=output_handle.output_def.name
-                    )
-                    for output_handle in outputs
-                    if (
-                        isinstance(output_handle, NodeOutput)
-                        and output_handle.node.name in resolved_op_selection_dict
-                    )
-                ]
-                deps[_dep_key_of(node)][node_input.input_def.name] = MultiDependencyDefinition(
-                    cast(
-                        List[Union[DependencyDefinition, Type[MappedInputPlaceholder]]],
-                        multi_dependencies,
-                    )
-                )
-            # else input is unconnected
-
-    # filter out unselected input/output mapping
-    new_input_mappings = list(
-        filter(
-            lambda input_mapping: input_mapping.maps_to.node_name
-            in [name for name, _ in selected_nodes],
-            graph._input_mappings,  # noqa: SLF001
-        )
-    )
-    new_output_mappings = list(
-        filter(
-            lambda output_mapping: output_mapping.maps_from.node_name
-            in [name for name, _ in selected_nodes],
-            graph._output_mappings,  # noqa: SLF001
-        )
-    )
-
-    return SubselectedGraphDefinition(
-        parent_graph_def=graph,
-        dependencies=deps,
-        node_defs=[definition for _, definition in selected_nodes],
-        input_mappings=new_input_mappings,
-        output_mappings=new_output_mappings,
-    )
-
-
 @io_manager(
     description="Built-in filesystem IO manager that stores and retrieves values using pickling."
 )
 def default_job_io_manager(init_context: "InitResourceContext"):
     # support overriding the default io manager via environment variables
     module_name = os.getenv("DAGSTER_DEFAULT_IO_MANAGER_MODULE")
     attribute_name = os.getenv("DAGSTER_DEFAULT_IO_MANAGER_ATTRIBUTE")
@@ -1322,15 +1213,15 @@
     )
     from .run_config_schema import RunConfigSchema
 
     # When executing with a subset job, include the missing nodes
     # from the original job as ignored to allow execution with
     # run config that is valid for the original
     ignored_nodes: Sequence[Node] = []
-    if job_def.is_subset_job:
+    if job_def.is_subset:
         if isinstance(job_def.graph, SubselectedGraphDefinition):  # op selection provided
             ignored_nodes = job_def.graph.get_top_level_omitted_nodes()
         elif job_def.asset_selection_data:
             parent_job = job_def
             while parent_job.asset_selection_data:
                 parent_job = parent_job.asset_selection_data.parent_job_def
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.3.4/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/logger_definition.py` & `dagster-1.3.4/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/logger_invocation.py` & `dagster-1.3.4/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/materialize.py` & `dagster-1.3.4/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.3.4/dagster/_core/definitions/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/metadata/table.py` & `dagster-1.3.4/dagster/_core/definitions/metadata/table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.3.4/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.3.4/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/node_container.py` & `dagster-1.3.4/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/node_definition.py` & `dagster-1.3.4/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/observe.py` & `dagster-1.3.4/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/op_definition.py` & `dagster-1.3.4/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/op_invocation.py` & `dagster-1.3.4/dagster/_core/definitions/op_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/output.py` & `dagster-1.3.4/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/partition.py` & `dagster-1.3.4/dagster/_core/definitions/partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,14 +347,18 @@
     def __init__(self, instance: DagsterInstance):
         self._instance = instance
 
     @cached_method
     def get_dynamic_partitions(self, partitions_def_name: str) -> Sequence[str]:
         return self._instance.get_dynamic_partitions(partitions_def_name)
 
+    @cached_method
+    def has_dynamic_partition(self, partitions_def_name: str, partition_key: str) -> bool:
+        return self._instance.has_dynamic_partition(partitions_def_name, partition_key)
+
 
 class DynamicPartitionsDefinition(
     PartitionsDefinition,
     NamedTuple(
         "_DynamicPartitionsDefinition",
         [
             (
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/partition_mapping.py` & `dagster-1.3.4/dagster/_core/definitions/partition_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import collections.abc
 import itertools
 import warnings
 from abc import ABC, abstractmethod
 from collections import defaultdict
+from datetime import datetime
 from typing import (
     Collection,
     Dict,
     List,
     Mapping,
     NamedTuple,
     Optional,
@@ -86,14 +87,15 @@
         """
 
     @public
     def get_upstream_partitions_for_partitions(
         self,
         downstream_partitions_subset: Optional[PartitionsSubset],
         upstream_partitions_def: PartitionsDefinition,
+        current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> PartitionsSubset:
         """Returns the subset of partition keys in the upstream asset that include data necessary
         to compute the contents of the given partition key subset in the downstream asset.
 
         Args:
             downstream_partitions_subset (Optional[PartitionsSubset]):
@@ -129,14 +131,15 @@
         )
 
     @public
     def get_downstream_partitions_for_partitions(
         self,
         upstream_partitions_subset: PartitionsSubset,
         downstream_partitions_def: PartitionsDefinition,
+        current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> PartitionsSubset:
         """Returns the subset of partition keys in the downstream asset that use the data in the given
         partition key subset of the upstream asset.
 
         Args:
             upstream_partitions_subset (Union[PartitionKeyRange, PartitionsSubset]): The
@@ -199,14 +202,15 @@
     downstream asset depends on all partitions of the usptream asset.
     """
 
     def get_upstream_partitions_for_partitions(
         self,
         downstream_partitions_subset: Optional[PartitionsSubset],
         upstream_partitions_def: PartitionsDefinition,
+        current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> PartitionsSubset:
         first = upstream_partitions_def.get_first_partition_key(
             current_time=None, dynamic_partitions_store=dynamic_partitions_store
         )
         last = upstream_partitions_def.get_last_partition_key(
             current_time=None, dynamic_partitions_store=dynamic_partitions_store
@@ -245,14 +249,15 @@
     downstream asset depends on the last partition of the upstream asset.
     """
 
     def get_upstream_partitions_for_partitions(
         self,
         downstream_partitions_subset: Optional[PartitionsSubset],
         upstream_partitions_def: PartitionsDefinition,
+        current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> PartitionsSubset:
         last = upstream_partitions_def.get_last_partition_key(
             current_time=None, dynamic_partitions_store=dynamic_partitions_store
         )
 
         empty_subset = upstream_partitions_def.empty_subset()
@@ -305,14 +310,15 @@
             ...
     """
 
     def get_upstream_partitions_for_partitions(
         self,
         downstream_partitions_subset: Optional[PartitionsSubset],
         upstream_partitions_def: PartitionsDefinition,
+        current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> PartitionsSubset:
         return upstream_partitions_def.subset_with_partition_keys(self.partition_keys)
 
     def get_upstream_partitions_for_partition_range(
         self,
         downstream_partition_key_range: Optional[PartitionKeyRange],
@@ -479,14 +485,15 @@
             upstream_partitions.add(partition_key.keys_by_dimension[partition_dimension_name])
         return upstream_partitions
 
     def get_upstream_partitions_for_partitions(
         self,
         downstream_partitions_subset: Optional[PartitionsSubset],
         upstream_partitions_def: PartitionsDefinition,
+        current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> PartitionsSubset:
         if downstream_partitions_subset is None:
             check.failed("downstream asset is not partitioned")
 
         (
             upstream_partitions_def,
@@ -516,14 +523,15 @@
                 )
             )
 
     def get_downstream_partitions_for_partitions(
         self,
         upstream_partitions_subset: PartitionsSubset,
         downstream_partitions_def: PartitionsDefinition,
+        current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> PartitionsSubset:
         if downstream_partitions_def is None:
             check.failed("downstream asset is not multi-partitioned")
 
         (
             _,
@@ -743,14 +751,15 @@
     def _get_dependency_partitions_subset(
         self,
         a_partitions_def: MultiPartitionsDefinition,
         a_partition_keys: Sequence[MultiPartitionKey],
         b_partitions_def: MultiPartitionsDefinition,
         a_upstream_of_b: bool,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
+        current_time: Optional[datetime] = None,
     ) -> PartitionsSubset:
         """Given two partitions definitions a_partitions_def and b_partitions_def that have a dependency
         relationship (a_upstream_of_b is True if a_partitions_def is upstream of b_partitions_def),
         and a_partition_keys, a list of partition keys in a_partitions_def, returns a list of
         partition keys in the partitions definition b_partitions_def that are
         dependencies of the partition keys in a_partition_keys.
         """
@@ -799,15 +808,16 @@
                         # downstream partition keys that are dependencies of that key
                         dep_b_keys_by_a_dim_and_key[a_dim_name][key] = list(
                             dimension_mapping.get_downstream_partitions_for_partitions(
                                 a_dimension_partitions_def.empty_subset().with_partition_keys(
                                     [key]
                                 ),
                                 b_dimension_partitions_def,
-                                dynamic_partitions_store,
+                                current_time=current_time,
+                                dynamic_partitions_store=dynamic_partitions_store,
                             ).get_partition_keys()
                         )
 
         else:
             # a_partitions_def is downstream of b_partitions_def, so we need to map the
             # dimension names of a_partitions_def to the corresponding dependency dimensions of
             # b_partitions_def
@@ -830,15 +840,16 @@
                     for key in keys:
                         dep_b_keys_by_a_dim_and_key[a_dim_name][key] = list(
                             partition_mapping.get_upstream_partitions_for_partitions(
                                 a_dimension_partitions_def.empty_subset().with_partition_keys(
                                     [key]
                                 ),
                                 b_dimension_partitions_def,
-                                dynamic_partitions_store,
+                                current_time=current_time,
+                                dynamic_partitions_store=dynamic_partitions_store,
                             ).get_partition_keys()
                         )
 
         b_partition_keys = set()
 
         mapped_a_dim_names = a_dim_to_dependency_b_dim.keys()
         mapped_b_dim_names = [mapping[0] for mapping in a_dim_to_dependency_b_dim.values()]
@@ -870,14 +881,15 @@
 
         return b_partitions_def.empty_subset().with_partition_keys(b_partition_keys)
 
     def get_upstream_partitions_for_partitions(
         self,
         downstream_partitions_subset: Optional[PartitionsSubset],
         upstream_partitions_def: PartitionsDefinition,
+        current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> PartitionsSubset:
         if downstream_partitions_subset is None:
             check.failed("downstream asset is not partitioned")
 
         self._check_all_dimensions_accounted_for(
             upstream_partitions_def,
@@ -894,14 +906,15 @@
             dynamic_partitions_store=dynamic_partitions_store,
         )
 
     def get_downstream_partitions_for_partitions(
         self,
         upstream_partitions_subset: PartitionsSubset,
         downstream_partitions_def: PartitionsDefinition,
+        current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> PartitionsSubset:
         if upstream_partitions_subset is None:
             check.failed("upstream asset is not partitioned")
 
         self._check_all_dimensions_accounted_for(
             upstream_partitions_subset.partitions_def,
@@ -999,28 +1012,30 @@
                 f" {extra_keys}"
             )
 
     def get_downstream_partitions_for_partitions(
         self,
         upstream_partitions_subset: PartitionsSubset,
         downstream_partitions_def: PartitionsDefinition,
+        current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> PartitionsSubset:
         self._check_downstream(downstream_partitions_def=downstream_partitions_def)
 
         downstream_subset = downstream_partitions_def.empty_subset()
         downstream_keys = set()
         for key in upstream_partitions_subset.get_partition_keys():
             downstream_keys.update(self._mapping[key])
         return downstream_subset.with_partition_keys(downstream_keys)
 
     def get_upstream_partitions_for_partitions(
         self,
         downstream_partitions_subset: Optional[PartitionsSubset],
         upstream_partitions_def: PartitionsDefinition,
+        current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> PartitionsSubset:
         self._check_upstream(upstream_partitions_def=upstream_partitions_def)
 
         upstream_subset = upstream_partitions_def.empty_subset()
         if downstream_partitions_subset is None:
             return upstream_subset
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.3.4/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/policy.py` & `dagster-1.3.4/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/reconstruct.py` & `dagster-1.3.4/dagster/_core/definitions/reconstruct.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from __future__ import annotations
 
 import inspect
+import json
 import os
 import sys
 from functools import lru_cache
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Callable,
+    Dict,
+    Iterable,
     List,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
     Tuple,
     TypeVar,
     Union,
     overload,
 )
 
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 import dagster._check as check
 import dagster._seven as seven
 from dagster._annotations import experimental
 from dagster._core.code_pointer import (
     CodePointer,
     CustomPointer,
@@ -34,16 +37,16 @@
 )
 from dagster._core.errors import DagsterInvariantViolationError
 from dagster._core.origin import (
     DEFAULT_DAGSTER_ENTRY_POINT,
     JobPythonOrigin,
     RepositoryPythonOrigin,
 )
-from dagster._core.selector import parse_solid_selection
 from dagster._serdes import pack_value, unpack_value, whitelist_for_serdes
+from dagster._serdes.serdes import NamedTupleSerializer
 from dagster._utils import hash_collection
 
 from .events import AssetKey
 from .job_base import IJob
 
 if TYPE_CHECKING:
     from dagster._core.definitions.assets import AssetsDefinition
@@ -169,177 +172,117 @@
     # - `ReconstructableRepository` has `Sequence` attributes that are unhashable by default
     def __hash__(self) -> int:
         if not hasattr(self, "_hash"):
             self._hash = hash_collection(self)
         return self._hash
 
 
+class ReconstructableJobSerializer(NamedTupleSerializer):
+    def before_unpack(self, _, unpacked_dict: Dict[str, Any]) -> Dict[str, Any]:
+        solid_selection_str = unpacked_dict.get("solid_selection_str")
+        solids_to_execute = unpacked_dict.get("solids_to_execute")
+        if solid_selection_str:
+            unpacked_dict["op_selection"] = json.loads(solid_selection_str)
+        elif solids_to_execute:
+            unpacked_dict["op_selection"] = solids_to_execute
+        return unpacked_dict
+
+    def after_pack(self, **packed_dict: Any) -> Dict[str, Any]:
+        if packed_dict["op_selection"]:
+            packed_dict["solid_selection_str"] = json.dumps(packed_dict["op_selection"]["__set__"])
+        else:
+            packed_dict["solid_selection_str"] = None
+        del packed_dict["op_selection"]
+        return packed_dict
+
+
 @whitelist_for_serdes(
+    serializer=ReconstructableJobSerializer,
     storage_name="ReconstructablePipeline",
     storage_field_names={
         "job_name": "pipeline_name",
     },
 )
 class ReconstructableJob(
     NamedTuple(
         "_ReconstructableJob",
         [
             ("repository", ReconstructableRepository),
             ("job_name", str),
-            ("solid_selection_str", Optional[str]),
-            ("solids_to_execute", Optional[AbstractSet[str]]),
+            ("op_selection", Optional[AbstractSet[str]]),
             ("asset_selection", Optional[AbstractSet[AssetKey]]),
         ],
     ),
     IJob,
 ):
     """Defines a reconstructable job. When your job must cross process boundaries, Dagster must know
     how to reconstruct the job on the other side of the process boundary.
 
     Args:
         repository (ReconstructableRepository): The reconstructable representation of the repository
             the job belongs to.
         job_name (str): The name of the job.
-        solid_selection_str (Optional[str]): The string value of a comma separated list of user-input
-            op selection. None if no selection is specified, i.e. the entire job will
-            be run.
-        solids_to_execute (Optional[FrozenSet[str]]): A set of op names to execute. None if no selection
-            is specified, i.e. the entire job will be run.
-        asset_selection (Optional[FrozenSet[AssetKey]]) A set of assets to execute. None if no selection
+        op_selection (Optional[AbstractSet[str]]): A set of op query strings. Ops matching any of
+            these queries will be selected. None if no selection is specified.
+        asset_selection (Optional[AbstractSet[AssetKey]]) A set of assets to execute. None if no selection
             is specified, i.e. the entire job will be run.
     """
 
     def __new__(
         cls,
         repository: ReconstructableRepository,
         job_name: str,
-        solid_selection_str: Optional[str] = None,
-        solids_to_execute: Optional[AbstractSet[str]] = None,
+        op_selection: Optional[Iterable[str]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
     ):
-        check.opt_set_param(solids_to_execute, "solids_to_execute", of_type=str)
-        check.opt_set_param(asset_selection, "asset_selection", AssetKey)
+        op_selection = set(op_selection) if op_selection else None
         return super(ReconstructableJob, cls).__new__(
             cls,
             repository=check.inst_param(repository, "repository", ReconstructableRepository),
             job_name=check.str_param(job_name, "job_name"),
-            solid_selection_str=check.opt_str_param(solid_selection_str, "solid_selection_str"),
-            solids_to_execute=solids_to_execute,
-            asset_selection=asset_selection,
+            op_selection=check.opt_nullable_set_param(op_selection, "op_selection", of_type=str),
+            asset_selection=check.opt_nullable_set_param(
+                asset_selection, "asset_selection", AssetKey
+            ),
         )
 
     def with_repository_load_data(
         self, metadata: Optional["RepositoryLoadData"]
     ) -> ReconstructableJob:
         return self._replace(repository=self.repository.with_repository_load_data(metadata))
 
-    @property
-    def solid_selection(self) -> Optional[Sequence[str]]:
-        return seven.json.loads(self.solid_selection_str) if self.solid_selection_str else None
-
     # Keep the most recent 1 definition (globally since this is a NamedTuple method)
     # This allows repeated calls to get_definition in execution paths to not reload the job
     @lru_cache(maxsize=1)
-    def get_definition(self) -> Union[JobDefinition, "JobDefinition"]:
+    def get_definition(self) -> JobDefinition:
         return self.repository.get_definition().get_maybe_subset_job_def(
             self.job_name,
-            self.solid_selection,
+            self.op_selection,
             self.asset_selection,
             self.solids_to_execute,
         )
 
     def get_reconstructable_repository(self) -> ReconstructableRepository:
         return self.repository
 
-    def _subset_for_execution(
-        self,
-        solids_to_execute: Optional[AbstractSet[str]],
-        solid_selection: Optional[Sequence[str]],
-        asset_selection: Optional[AbstractSet[AssetKey]],
-    ) -> "ReconstructableJob":
-        # no selection
-        if solid_selection is None and solids_to_execute is None and asset_selection is None:
-            return ReconstructableJob(
-                repository=self.repository,
-                job_name=self.job_name,
-            )
-
-        from dagster._core.definitions import JobDefinition
-
-        job_def = self.get_definition()
-        if isinstance(job_def, JobDefinition):
-            # jobs use pre-resolved selection
-            # when subselecting a job
-            # * job subselection depend on solid_selection rather than solids_to_execute
-            # * we'll resolve the op selection later in the stack
-            if solid_selection is None:
-                # when the pre-resolution info is unavailable (e.g. subset from existing run),
-                # we need to fill the solid_selection in order to pass the value down to deeper stack.
-                solid_selection = list(solids_to_execute) if solids_to_execute else None
-            return ReconstructableJob(
-                repository=self.repository,
-                job_name=self.job_name,
-                solid_selection_str=seven.json.dumps(solid_selection) if solid_selection else None,
-                solids_to_execute=None,
-                asset_selection=asset_selection,
-            )
-        elif isinstance(job_def, JobDefinition):
-            # when subselecting a job
-            # * job subselection depend on solids_to_excute rather than solid_selection
-            # * we resolve a list of solid selection queries to a frozenset of qualified solid names
-            #   e.g. ['foo_solid+'] to {'foo_solid', 'bar_solid'}
-            if solid_selection and solids_to_execute is None:
-                # when post-resolution query is unavailable, resolve the query
-                solids_to_execute = parse_solid_selection(job_def, solid_selection)
-            return ReconstructableJob(
-                repository=self.repository,
-                job_name=self.job_name,
-                solid_selection_str=seven.json.dumps(solid_selection) if solid_selection else None,
-                solids_to_execute=frozenset(solids_to_execute) if solids_to_execute else None,
-            )
-        else:
-            raise Exception(f"Unexpected job type {job_def.__class__.__name__}")
-
-    def subset_for_execution(
+    def get_subset(
         self,
-        solid_selection: Optional[Sequence[str]] = None,
+        *,
+        op_selection: Optional[Iterable[str]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
-    ) -> "ReconstructableJob":
-        # take a list of unresolved selection queries
-        check.opt_sequence_param(solid_selection, "solid_selection", of_type=str)
-        check.opt_set_param(asset_selection, "asset_selection", of_type=AssetKey)
-
-        check.invariant(
-            not (solid_selection and asset_selection),
-            "solid_selection and asset_selection cannot both be provided as arguments",
-        )
-
-        return self._subset_for_execution(
-            solids_to_execute=None, solid_selection=solid_selection, asset_selection=asset_selection
-        )
-
-    def subset_for_execution_from_existing_job(
-        self,
-        solids_to_execute: Optional[AbstractSet[str]] = None,
-        asset_selection: Optional[AbstractSet[AssetKey]] = None,
-    ) -> ReconstructableJob:
-        # take a frozenset of resolved solid names from an existing job
-        # so there's no need to parse the selection
-
-        check.invariant(
-            not (solids_to_execute and asset_selection),
-            "solids_to_execute and asset_selection cannot both be provided as arguments",
-        )
-
-        check.opt_set_param(solids_to_execute, "solids_to_execute", of_type=str)
-        check.opt_set_param(asset_selection, "asset_selection", of_type=AssetKey)
-
-        return self._subset_for_execution(
-            solids_to_execute=solids_to_execute,
-            solid_selection=None,
+    ) -> Self:
+        if op_selection and asset_selection:
+            check.failed(
+                "solid_selection and asset_selection cannot both be provided as arguments",
+            )
+        op_selection = set(op_selection) if op_selection else None
+        return ReconstructableJob(
+            repository=self.repository,
+            job_name=self.job_name,
+            op_selection=op_selection,
             asset_selection=asset_selection,
         )
 
     def describe(self) -> str:
         return '"{name}" in repository ({repo})'.format(
             repo=self.repository.pointer.describe, name=self.job_name
         )
@@ -378,14 +321,20 @@
         """Return the module the job is found in, the origin is a module code pointer."""
         pointer = self.get_python_origin().get_repo_pointer()
         if isinstance(pointer, ModuleCodePointer):
             return pointer.module
 
         return None
 
+    # Allow this to be hashed for `lru_cache` in `get_definition`
+    def __hash__(self) -> int:
+        if not hasattr(self, "_hash"):
+            self._hash = hash_collection(self)
+        return self._hash
+
 
 def reconstructable(target: Callable[..., "JobDefinition"]) -> ReconstructableJob:
     """Create a :py:class:`~dagster._core.definitions.reconstructable.ReconstructableJob` from a
     function that returns a :py:class:`~dagster.JobDefinition`/:py:class:`~dagster.JobDefinition`,
     or a function decorated with :py:func:`@job <dagster.job>`.
 
     When your job must cross process boundaries, e.g., for execution on multiple nodes or
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.3.4/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.3.4/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.3.4/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.3.4/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.3.4/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,20 +266,20 @@
                 i += 1
 
         return None
 
     def get_maybe_subset_job_def(
         self,
         job_name: str,
-        op_selection: Optional[Sequence[str]] = None,
+        op_selection: Optional[Iterable[str]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
         solids_to_execute: Optional[AbstractSet[str]] = None,
     ):
         defn = self.get_job(job_name)
-        return defn.get_job_def_for_subset_selection(op_selection, asset_selection)
+        return defn.get_subset(op_selection=op_selection, asset_selection=asset_selection)
 
     @public
     def load_asset_value(
         self,
         asset_key: CoercibleToAssetKey,
         *,
         python_type: Optional[Type] = None,
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.3.4/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.3.4/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/resource_annotation.py` & `dagster-1.3.4/dagster/_core/definitions/resource_annotation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/resource_definition.py` & `dagster-1.3.4/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/resource_invocation.py` & `dagster-1.3.4/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/resource_requirement.py` & `dagster-1.3.4/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/run_config.py` & `dagster-1.3.4/dagster/_core/definitions/run_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,19 +191,17 @@
                 asset_layer=creation_data.asset_layer,
                 node_input_source_assets=creation_data.graph_def.node_input_source_assets,
             ),
             description="Configure runtime parameters for ops or assets.",
         )
 
     fields["ops"] = nodes_field
-    field_aliases = {"ops": "solids"}
 
     return Shape(
         fields=remove_none_entries(fields),
-        field_aliases=field_aliases,
     )
 
 
 # Common pattern for a set of named definitions (e.g. executors)
 # to build a selector so that one of them is selected
 def selector_for_named_defs(named_defs) -> Selector:
     return Selector({named_def.name: def_config_field(named_def) for named_def in named_defs})
@@ -368,28 +366,27 @@
     ):
         return output_manager_def.output_config_schema.as_field()
 
     return None
 
 
 def node_config_field(fields: Mapping[str, Optional[Field]], ignored: bool) -> Optional[Field]:
-    field_aliases = {"ops": "solids"}
     trimmed_fields = remove_none_entries(fields)
     if trimmed_fields:
         if ignored:
             return Field(
-                Shape(trimmed_fields, field_aliases=field_aliases),
+                Shape(trimmed_fields),
                 is_required=False,
                 description=(
                     "This op is not present in the current op selection, "
                     "the config values are allowed but ignored."
                 ),
             )
         else:
-            return Field(Shape(trimmed_fields, field_aliases=field_aliases))
+            return Field(Shape(trimmed_fields))
     else:
         return None
 
 
 def construct_leaf_node_config(
     node: Node,
     handle: NodeHandle,
@@ -550,15 +547,15 @@
             ignored=True,
             asset_layer=asset_layer,
             input_source_assets=node_input_source_assets.get(node.name, {}),
         )
         if node_field:
             fields[node.name] = node_field
 
-    return Shape(fields, field_aliases={"ops": "solids"})
+    return Shape(fields)
 
 
 def iterate_node_def_config_types(node_def: NodeDefinition) -> Iterator[ConfigType]:
     if isinstance(node_def, OpDefinition):
         if node_def.has_config_field:
             yield from node_def.get_config_field().config_type.type_iterator()
     elif isinstance(node_def, GraphDefinition):
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/run_config_schema.py` & `dagster-1.3.4/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/run_request.py` & `dagster-1.3.4/dagster/_core/definitions/run_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from dagster._core.storage.dagster_run import DagsterRun, DagsterRunStatus
 from dagster._core.storage.tags import PARTITION_NAME_TAG
 from dagster._serdes.serdes import whitelist_for_serdes
 from dagster._utils.error import SerializableErrorInfo
 
 if TYPE_CHECKING:
     from dagster._core.definitions.job_definition import JobDefinition
+    from dagster._core.definitions.partition import PartitionsDefinition
     from dagster._core.definitions.run_config import RunConfig
     from dagster._core.definitions.unresolved_asset_job_definition import (
         UnresolvedAssetJobDefinition,
     )
 
 
 @whitelist_for_serdes(old_storage_names={"JobType"})
@@ -171,15 +172,14 @@
             Union[AddDynamicPartitionsRequest, DeleteDynamicPartitionsRequest]
         ],
         current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> "RunRequest":
         from dagster._core.definitions.job_definition import JobDefinition
         from dagster._core.definitions.partition import (
-            DynamicPartitionsDefinition,
             PartitionedConfig,
             PartitionsDefinition,
         )
 
         if self.partition_key is None:
             check.failed(
                 "Cannot resolve partition for run request without partition key",
@@ -201,53 +201,21 @@
             else PartitionedConfig.from_flexible_config(target_definition.config, partitions_def)
         )
         if partitioned_config is None:
             check.failed(
                 "Cannot resolve partition for run request on unpartitioned job",
             )
 
-        if isinstance(partitions_def, DynamicPartitionsDefinition) and partitions_def.name:
-            if not dynamic_partitions_store:
-                check.failed(
-                    "Cannot resolve partition for run request on dynamic partitions without"
-                    " dynamic_partitions_store"
-                )
-
-            add_partition_keys: Set[str] = set()
-            delete_partition_keys: Set[str] = set()
-            for req in dynamic_partitions_requests:
-                if isinstance(req, AddDynamicPartitionsRequest):
-                    if req.partitions_def_name == partitions_def.name:
-                        add_partition_keys.update(set(req.partition_keys))
-                elif isinstance(req, DeleteDynamicPartitionsRequest):
-                    if req.partitions_def_name == partitions_def.name:
-                        delete_partition_keys.update(set(req.partition_keys))
-
-            partition_keys_after_requests_resolved = (
-                set(
-                    dynamic_partitions_store.get_dynamic_partitions(
-                        partitions_def_name=partitions_def.name
-                    )
-                )
-                | add_partition_keys
-            ) - delete_partition_keys
-
-            if self.partition_key not in partition_keys_after_requests_resolved:
-                check.failed(
-                    f"Dynamic partition key {self.partition_key} for partitions def"
-                    f" '{partitions_def.name}' is invalid. After dynamic partitions requests are"
-                    " applied, it does not exist in the set of valid partition keys."
-                )
-
-        else:
-            partitions_def.validate_partition_key(
-                self.partition_key,
-                dynamic_partitions_store=dynamic_partitions_store,
-                current_time=current_time,
-            )
+        _check_valid_partition_key_after_dynamic_partitions_requests(
+            self.partition_key,
+            partitions_def,
+            dynamic_partitions_requests,
+            current_time,
+            dynamic_partitions_store,
+        )
 
         tags = {
             **(self.tags or {}),
             **partitioned_config.get_tags_for_partition_key(
                 self.partition_key,
                 job_name=target_definition.name,
             ),
@@ -262,14 +230,81 @@
 
     def has_resolved_partition(self) -> bool:
         # Backcompat run requests yielded via `run_request_for_partition` already have resolved
         # partitioning
         return self.tags.get(PARTITION_NAME_TAG) is not None if self.partition_key else True
 
 
+def _check_valid_partition_key_after_dynamic_partitions_requests(
+    partition_key: str,
+    partitions_def: "PartitionsDefinition",
+    dynamic_partitions_requests: Sequence[
+        Union[AddDynamicPartitionsRequest, DeleteDynamicPartitionsRequest]
+    ],
+    current_time: Optional[datetime] = None,
+    dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
+):
+    from dagster._core.definitions.multi_dimensional_partitions import MultiPartitionsDefinition
+    from dagster._core.definitions.partition import (
+        DynamicPartitionsDefinition,
+    )
+
+    if isinstance(partitions_def, MultiPartitionsDefinition):
+        multipartition_key = partitions_def.get_partition_key_from_str(partition_key)
+
+        for dimension in partitions_def.partitions_defs:
+            _check_valid_partition_key_after_dynamic_partitions_requests(
+                multipartition_key.keys_by_dimension[dimension.name],
+                dimension.partitions_def,
+                dynamic_partitions_requests,
+                current_time,
+                dynamic_partitions_store,
+            )
+
+    elif isinstance(partitions_def, DynamicPartitionsDefinition) and partitions_def.name:
+        if not dynamic_partitions_store:
+            check.failed(
+                "Cannot resolve partition for run request on dynamic partitions without"
+                " dynamic_partitions_store"
+            )
+
+        add_partition_keys: Set[str] = set()
+        delete_partition_keys: Set[str] = set()
+        for req in dynamic_partitions_requests:
+            if isinstance(req, AddDynamicPartitionsRequest):
+                if req.partitions_def_name == partitions_def.name:
+                    add_partition_keys.update(set(req.partition_keys))
+            elif isinstance(req, DeleteDynamicPartitionsRequest):
+                if req.partitions_def_name == partitions_def.name:
+                    delete_partition_keys.update(set(req.partition_keys))
+
+        partition_keys_after_requests_resolved = (
+            set(
+                dynamic_partitions_store.get_dynamic_partitions(
+                    partitions_def_name=partitions_def.name
+                )
+            )
+            | add_partition_keys
+        ) - delete_partition_keys
+
+        if partition_key not in partition_keys_after_requests_resolved:
+            check.failed(
+                f"Dynamic partition key {partition_key} for partitions def"
+                f" '{partitions_def.name}' is invalid. After dynamic partitions requests are"
+                " applied, it does not exist in the set of valid partition keys."
+            )
+
+    else:
+        partitions_def.validate_partition_key(
+            partition_key,
+            dynamic_partitions_store=dynamic_partitions_store,
+            current_time=current_time,
+        )
+
+
 @whitelist_for_serdes(
     storage_name="PipelineRunReaction",
     storage_field_names={
         "dagster_run": "pipeline_run",
     },
 )
 class DagsterRunReaction(
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.3.4/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/schedule_definition.py` & `dagster-1.3.4/dagster/_core/definitions/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.3.4/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/selector.py` & `dagster-1.3.4/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/sensor_definition.py` & `dagster-1.3.4/dagster/_core/definitions/sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/source_asset.py` & `dagster-1.3.4/dagster/_core/definitions/source_asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
         if resource_defs is not None:
             experimental_arg_warning("resource_defs", "SourceAsset.__new__")
 
         if io_manager_def is not None:
             experimental_arg_warning("io_manager_def", "SourceAsset.__new__")
 
-        self.key = AssetKey.from_coerceable(key)
+        self.key = AssetKey.from_coercible(key)
         metadata = check.opt_mapping_param(metadata, "metadata", key_type=str)
         self.raw_metadata = metadata
         self.metadata = normalize_metadata(metadata, allow_invalid=True)
         self.resource_defs = wrap_resources_for_execution(
             dict(check.opt_mapping_param(resource_defs, "resource_defs"))
         )
         self._io_manager_def = check.opt_inst_param(
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/step_launcher.py` & `dagster-1.3.4/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/target.py` & `dagster-1.3.4/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.3.4/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from dagster._core.definitions.partition_key_range import PartitionKeyRange
 from dagster._core.definitions.partition_mapping import PartitionMapping
 from dagster._core.definitions.time_window_partitions import (
     TimeWindow,
     TimeWindowPartitionsDefinition,
     TimeWindowPartitionsSubset,
 )
-from dagster._core.errors import DagsterInvalidDefinitionError
+from dagster._core.errors import DagsterInvalidDefinitionError, DagsterInvalidInvocationError
 from dagster._core.instance import DynamicPartitionsStore
 from dagster._serdes import whitelist_for_serdes
 
 
 @whitelist_for_serdes
 class TimeWindowPartitionMapping(
     PartitionMapping,
@@ -93,85 +93,99 @@
     ) -> PartitionKeyRange:
         raise NotImplementedError()
 
     def get_upstream_partitions_for_partitions(
         self,
         downstream_partitions_subset: Optional[PartitionsSubset],
         upstream_partitions_def: PartitionsDefinition,
+        current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> PartitionsSubset:
+        """Returns the partitions in the upstream asset that map to the given downstream partitions.
+
+        Raises an error if upstream partitions do not exist at the given current_time, fetching the
+        current time if not provided.
+        """
         if not isinstance(downstream_partitions_subset, TimeWindowPartitionsSubset):
             check.failed("downstream_partitions_subset must be a TimeWindowPartitionsSubset")
 
+        if not isinstance(upstream_partitions_def, TimeWindowPartitionsDefinition):
+            check.failed("upstream_partitions_def must be a TimeWindowPartitionsDefinition")
+
         return self._map_partitions(
-            downstream_partitions_subset.partitions_def,
+            cast(TimeWindowPartitionsDefinition, downstream_partitions_subset.partitions_def),
             upstream_partitions_def,
             downstream_partitions_subset,
             self.start_offset,
             self.end_offset,
+            raise_on_non_existent_partition=True,
+            current_time=current_time,
         )
 
     def get_downstream_partitions_for_partition_range(
         self,
         upstream_partition_key_range: PartitionKeyRange,
         downstream_partitions_def: Optional[PartitionsDefinition],
         upstream_partitions_def: PartitionsDefinition,
     ) -> PartitionKeyRange:
         raise NotImplementedError()
 
     def get_downstream_partitions_for_partitions(
         self,
         upstream_partitions_subset: PartitionsSubset,
         downstream_partitions_def: Optional[PartitionsDefinition],
+        current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> PartitionsSubset:
+        """Returns the partitions in the downstream asset that map to the given upstream partitions.
+
+        Filters for partitions that exist at the given current_time, fetching the current time
+        if not provided.
+        """
         if not isinstance(downstream_partitions_def, TimeWindowPartitionsDefinition):
             check.failed("downstream_partitions_def must be a TimeWindowPartitionsDefinitions")
 
         if not isinstance(upstream_partitions_subset, TimeWindowPartitionsSubset):
             check.failed("upstream_partitions_subset must be a TimeWindowPartitionsSubset")
 
         return self._map_partitions(
-            upstream_partitions_subset.partitions_def,
+            cast(TimeWindowPartitionsDefinition, upstream_partitions_subset.partitions_def),
             downstream_partitions_def,
             upstream_partitions_subset,
             -self.start_offset,
             -self.end_offset,
+            raise_on_non_existent_partition=False,
+            current_time=current_time,
         )
 
     def _map_partitions(
         self,
-        from_partitions_def: PartitionsDefinition,
-        to_partitions_def: PartitionsDefinition,
+        from_partitions_def: TimeWindowPartitionsDefinition,
+        to_partitions_def: TimeWindowPartitionsDefinition,
         from_partitions_subset: TimeWindowPartitionsSubset,
         start_offset: int,
         end_offset: int,
-    ) -> PartitionsSubset:
-        if not isinstance(from_partitions_def, TimeWindowPartitionsDefinition) or not isinstance(
-            to_partitions_def, TimeWindowPartitionsDefinition
-        ):
-            raise DagsterInvalidDefinitionError(
-                "TimeWindowPartitionMappings can only operate on TimeWindowPartitionsDefinitions"
-            )
-
+        raise_on_non_existent_partition: bool,
+        current_time: Optional[datetime] = None,
+    ) -> TimeWindowPartitionsSubset:
         if (start_offset != 0 or end_offset != 0) and (
             from_partitions_def.cron_schedule != to_partitions_def.cron_schedule
         ):
             raise DagsterInvalidDefinitionError(
                 "Can't use the start_offset or end_offset parameters of"
                 " TimeWindowPartitionMapping when the cron schedule of the upstream"
                 " PartitionsDefinition is different than the cron schedule of the downstream"
                 " one."
             )
 
         if to_partitions_def.timezone != from_partitions_def.timezone:
             raise DagsterInvalidDefinitionError("Timezones don't match")
 
         # skip fancy mapping logic in the simple case
-        if to_partitions_def == from_partitions_def and start_offset == 0 and end_offset == 0:
+        if from_partitions_def == to_partitions_def and start_offset == 0 and end_offset == 0:
             return from_partitions_subset
 
         time_windows = []
         for from_partition_time_window in from_partitions_subset.included_time_windows:
             from_start_dt, from_end_dt = from_partition_time_window
             offsetted_start_dt = _offsetted_datetime(
                 from_partitions_def, from_start_dt, start_offset
@@ -201,23 +215,47 @@
                 )
                 window_end = (
                     to_partitions_def.end_time_for_partition_key(to_end_partition_key)
                     if to_end_partition_key
                     else cast(TimeWindow, to_partitions_def.get_last_partition_window()).end
                 )
 
-                time_windows.append(TimeWindow(window_start, window_end))
+                if window_start < window_end:
+                    time_windows.append(TimeWindow(window_start, window_end))
+
+        first_window = to_partitions_def.get_first_partition_window(current_time=current_time)
+        last_window = to_partitions_def.get_last_partition_window(current_time=current_time)
+
+        filtered_time_windows = []
+
+        for time_window in time_windows:
+            if (
+                first_window
+                and last_window
+                and time_window.start <= last_window.start
+                and time_window.end >= first_window.end
+            ):
+                window_end = min(time_window.end, last_window.end)
+                window_start = max(time_window.start, first_window.start)
+                filtered_time_windows.append(TimeWindow(window_start, window_end))
+
+        if raise_on_non_existent_partition:
+            if filtered_time_windows != time_windows:
+                raise DagsterInvalidInvocationError(
+                    f"Provided time windows {time_windows} contain invalid time windows for"
+                    f" partitions definition {to_partitions_def}"
+                )
 
         return TimeWindowPartitionsSubset(
             to_partitions_def,
             num_partitions=sum(
                 len(to_partitions_def.get_partition_keys_in_time_window(time_window))
-                for time_window in time_windows
+                for time_window in filtered_time_windows
             ),
-            included_time_windows=time_windows,
+            included_time_windows=filtered_time_windows,
         )
 
 
 def _offsetted_datetime(
     partitions_def: TimeWindowPartitionsDefinition, dt: datetime, offset: int
 ) -> Optional[datetime]:
     for _ in range(abs(offset)):
```

### Comparing `dagster-1.3.3/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.3.4/dagster/_core/definitions/time_window_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.3.4/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/utils.py` & `dagster-1.3.4/dagster/_core/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/definitions/version_strategy.py` & `dagster-1.3.4/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/errors.py` & `dagster-1.3.4/dagster/_core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/event_api.py` & `dagster-1.3.4/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/events/__init__.py` & `dagster-1.3.4/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/events/log.py` & `dagster-1.3.4/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/events/utils.py` & `dagster-1.3.4/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/api.py` & `dagster-1.3.4/dagster/_core/execution/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     Sequence,
     Tuple,
     Union,
     cast,
 )
 
 import dagster._check as check
-from dagster._annotations import experimental
 from dagster._core.definitions import IJob, JobDefinition
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.job_base import InMemoryJob
 from dagster._core.definitions.reconstruct import ReconstructableJob
 from dagster._core.definitions.repository_definition import RepositoryLoadData
 from dagster._core.errors import DagsterExecutionInterruptedError, DagsterInvariantViolationError
 from dagster._core.events import DagsterEvent, EngineEventData
@@ -42,16 +41,15 @@
 from .context_creation_job import (
     ExecutionContextManager,
     PlanExecutionContextManager,
     PlanOrchestrationContextManager,
     orchestration_context_event_generator,
     scoped_job_context,
 )
-from .execute_job_result import ExecuteJobResult
-from .results import PipelineExecutionResult
+from .job_execution_result import JobExecutionResult
 
 ## Brief guide to the execution APIs
 # | function name               | operates over      | sync  | supports    | creates new DagsterRun  |
 # |                             |                    |       | reexecution | in instance             |
 # | --------------------------- | ------------------ | ----- | ----------- | ----------------------- |
 # | execute_job                 | ReconstructableJob | sync  | yes         | yes                     |
 # | execute_run_iterator        | DagsterRun         | async | (1)         | no                      |
@@ -138,16 +136,18 @@
             ),
         )
 
     if dagster_run.solids_to_execute or dagster_run.asset_selection:
         # when `execute_run_iterator` is directly called, the sub pipeline hasn't been created
         # note that when we receive the solids to execute via DagsterRun, it won't support
         # solid selection query syntax
-        job = job.subset_for_execution_from_existing_job(
-            frozenset(dagster_run.solids_to_execute) if dagster_run.solids_to_execute else None,
+        job = job.get_subset(
+            op_selection=list(dagster_run.solids_to_execute)
+            if dagster_run.solids_to_execute
+            else None,
             asset_selection=dagster_run.asset_selection,
         )
 
     execution_plan = _get_execution_plan_from_run(job, dagster_run, instance)
     if isinstance(job, ReconstructableJob):
         job = job.with_repository_load_data(execution_plan.repository_load_data)
 
@@ -172,28 +172,28 @@
 
 
 def execute_run(
     job: IJob,
     dagster_run: DagsterRun,
     instance: DagsterInstance,
     raise_on_error: bool = False,
-) -> PipelineExecutionResult:
+) -> JobExecutionResult:
     """Executes an existing job run synchronously.
 
     Synchronous version of execute_run_iterator.
 
     Args:
         job (IJob): The pipeline to execute.
         dagster_run (DagsterRun): The run to execute
         instance (DagsterInstance): The instance in which the run has been created.
         raise_on_error (Optional[bool]): Whether or not to raise exceptions when they occur.
             Defaults to ``False``.
 
     Returns:
-        PipelineExecutionResult: The result of the execution.
+        JobExecutionResult: The result of the execution.
     """
     if isinstance(job, JobDefinition):
         raise DagsterInvariantViolationError(
             "execute_run requires a reconstructable job but received job definition directly"
             " instead. To support hand-off to other processes please wrap your definition in a call"
             " to reconstructable(). Learn more about reconstructable here:"
             " https://docs.dagster.io/_apidocs/execution#dagster.reconstructable"
@@ -218,17 +218,19 @@
             dagster_run.job_name, dagster_run.run_id, dagster_run.status
         ),
     )
     if dagster_run.solids_to_execute or dagster_run.asset_selection:
         # when `execute_run` is directly called, the sub job hasn't been created
         # note that when we receive the solids to execute via DagsterRun, it won't support
         # solid selection query syntax
-        job = job.subset_for_execution_from_existing_job(
-            frozenset(dagster_run.solids_to_execute) if dagster_run.solids_to_execute else None,
-            dagster_run.asset_selection,
+        job = job.get_subset(
+            op_selection=list(dagster_run.solids_to_execute)
+            if dagster_run.solids_to_execute
+            else None,
+            asset_selection=dagster_run.asset_selection,
         )
 
     execution_plan = _get_execution_plan_from_run(job, dagster_run, instance)
     if isinstance(job, ReconstructableJob):
         job = job.with_repository_load_data(execution_plan.repository_load_data)
 
     output_capture: Optional[Dict[StepOutputHandle, Any]] = {}
@@ -246,26 +248,28 @@
             raise_on_error=raise_on_error,
             executor_defs=None,
             output_capture=output_capture,
         ),
     )
     event_list = list(_execute_run_iterable)
 
-    return PipelineExecutionResult(
+    # We need to reload the run object after execution for it to be accurate
+    reloaded_dagster_run = check.not_none(instance.get_run_by_id(dagster_run.run_id))
+
+    return JobExecutionResult(
         job.get_definition(),
-        dagster_run.run_id,
-        event_list,
-        lambda: scoped_job_context(  # type: ignore
+        scoped_job_context(
             execution_plan,
             job,
-            dagster_run.run_config,
-            dagster_run,
+            reloaded_dagster_run.run_config,
+            reloaded_dagster_run,
             instance,
         ),
-        output_capture=output_capture,
+        event_list,
+        reloaded_dagster_run,
     )
 
 
 @contextmanager
 def ephemeral_instance_if_missing(
     instance: Optional[DagsterInstance],
 ) -> Iterator[DagsterInstance]:
@@ -318,25 +322,24 @@
         # It is recalculated later by the re-execution machinery.
         step_keys_to_execute, _ = KnownExecutionState.build_resume_retry_reexecution(
             instance, parent_run=cast(DagsterRun, instance.get_run_by_id(run_id))
         )
         return ReexecutionOptions(parent_run_id=run_id, step_selection=step_keys_to_execute)
 
 
-@experimental
 def execute_job(
     job: ReconstructableJob,
     instance: "DagsterInstance",
     run_config: Any = None,
     tags: Optional[Mapping[str, Any]] = None,
     raise_on_error: bool = False,
     op_selection: Optional[Sequence[str]] = None,
     reexecution_options: Optional[ReexecutionOptions] = None,
     asset_selection: Optional[Sequence[AssetKey]] = None,
-) -> ExecuteJobResult:
+) -> JobExecutionResult:
     """Execute a job synchronously.
 
     This API represents dagster's python entrypoint for out-of-process
     execution. For most testing purposes, :py:meth:`~dagster.JobDefinition.
     execute_in_process` will be more suitable, but when wanting to run
     execution using an out-of-process executor (such as :py:class:`dagster.
     multiprocess_executor`), then `execute_job` is suitable.
@@ -437,53 +440,45 @@
             "re-execution and op selection cannot be used together at this time."
         )
 
     if reexecution_options:
         if run_config is None:
             run = check.not_none(instance.get_run_by_id(reexecution_options.parent_run_id))
             run_config = run.run_config
-        result = _reexecute_job(
+        return _reexecute_job(
             job_arg=job_def,
             parent_run_id=reexecution_options.parent_run_id,
             run_config=run_config,
             step_selection=list(reexecution_options.step_selection),
             tags=tags,
             instance=instance,
             raise_on_error=raise_on_error,
         )
     else:
-        result = _logged_execute_job(
+        return _logged_execute_job(
             job_arg=job_def,
             instance=instance,
             run_config=run_config,
             tags=tags,
             op_selection=op_selection,
             raise_on_error=raise_on_error,
             asset_selection=asset_selection,
         )
 
-    # We use PipelineExecutionResult to construct the JobExecutionResult.
-    return ExecuteJobResult(
-        job_def=cast(ReconstructableJob, job_def).get_definition(),
-        reconstruct_context=result.reconstruct_context(),
-        event_list=result.event_list,
-        dagster_run=instance.get_run_by_id(result.run_id),
-    )
-
 
 @telemetry_wrapper
 def _logged_execute_job(
     job_arg: Union[IJob, JobDefinition],
     instance: DagsterInstance,
     run_config: Optional[Mapping[str, object]] = None,
     tags: Optional[Mapping[str, str]] = None,
     op_selection: Optional[Sequence[str]] = None,
     raise_on_error: bool = True,
     asset_selection: Optional[Sequence[AssetKey]] = None,
-) -> PipelineExecutionResult:
+) -> JobExecutionResult:
     check.inst_param(instance, "instance", DagsterInstance)
 
     job_arg, repository_load_data = _job_with_repository_load_data(job_arg)
 
     (
         job_arg,
         run_config,
@@ -524,15 +519,15 @@
     job_arg: Union[IJob, JobDefinition],
     parent_run_id: str,
     run_config: Optional[Mapping[str, object]] = None,
     step_selection: Optional[Sequence[str]] = None,
     tags: Optional[Mapping[str, str]] = None,
     instance: Optional[DagsterInstance] = None,
     raise_on_error: bool = True,
-) -> PipelineExecutionResult:
+) -> JobExecutionResult:
     """Reexecute an existing job run."""
     check.opt_sequence_param(step_selection, "step_selection", of_type=str)
 
     check.str_param(parent_run_id, "parent_run_id")
 
     with ephemeral_instance_if_missing(instance) as execute_instance:
         job_arg, repository_load_data = _job_with_repository_load_data(job_arg)
@@ -559,16 +554,16 @@
                 job_arg,
                 run_config,
                 cast(DagsterRun, parent_dagster_run),
                 step_selection,
             )
 
         if parent_dagster_run.asset_selection:
-            job_arg = job_arg.subset_for_execution(
-                solid_selection=None, asset_selection=parent_dagster_run.asset_selection
+            job_arg = job_arg.get_subset(
+                op_selection=None, asset_selection=parent_dagster_run.asset_selection
             )
 
         dagster_run = execute_instance.create_run_for_job(
             job_def=job_arg.get_definition(),
             execution_plan=execution_plan,
             run_config=run_config,
             tags=tags,
@@ -847,15 +842,15 @@
             yield event
 
 
 class ExecuteRunWithPlanIterable:
     """Utility class to consolidate execution logic.
 
     This is a class and not a function because, e.g., in constructing a `scoped_pipeline_context`
-    for `PipelineExecutionResult`, we need to pull out the `pipeline_context` after we're done
+    for `JobExecutionResult`, we need to pull out the `pipeline_context` after we're done
     yielding events. This broadly follows a pattern we make use of in other places,
     cf. `dagster._utils.EventGenerationManager`.
     """
 
     def __init__(
         self,
         execution_plan: ExecutionPlan,
@@ -918,15 +913,15 @@
     tags = check.opt_mapping_param(tags, "tags", key_type=str)
     check.opt_sequence_param(op_selection, "solid_selection", of_type=str)
 
     tags = merge_dicts(job_def.tags, tags)
 
     # generate job subset from the given solid_selection
     if op_selection:
-        job_arg = job_arg.subset_for_execution(op_selection)
+        job_arg = job_arg.get_subset(op_selection=op_selection)
 
     return (
         job_arg,
         run_config,
         tags,
         job_arg.solids_to_execute,
         op_selection,
@@ -937,15 +932,15 @@
     instance: DagsterInstance,
     job: IJob,
     run_config: Optional[Mapping],
     parent_dagster_run: DagsterRun,
     step_selection: Sequence[str],
 ) -> ExecutionPlan:
     if parent_dagster_run.solid_selection:
-        job = job.subset_for_execution(parent_dagster_run.solid_selection, None)
+        job = job.get_subset(op_selection=parent_dagster_run.solid_selection)
 
     state = KnownExecutionState.build_for_reexecution(instance, parent_dagster_run)
 
     parent_plan = create_execution_plan(
         job,
         parent_dagster_run.run_config,
         known_state=state,
```

### Comparing `dagster-1.3.3/dagster/_core/execution/asset_backfill.py` & `dagster-1.3.4/dagster/_core/execution/asset_backfill.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from datetime import datetime
 from enum import Enum
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Dict,
     Iterable,
     List,
@@ -39,15 +40,15 @@
 from dagster._core.instance import DagsterInstance, DynamicPartitionsStore
 from dagster._core.storage.dagster_run import DagsterRunStatus, RunsFilter
 from dagster._core.storage.tags import BACKFILL_ID_TAG, PARTITION_NAME_TAG
 from dagster._core.workspace.context import (
     BaseWorkspaceRequestContext,
     IWorkspaceProcessContext,
 )
-from dagster._utils import hash_collection
+from dagster._utils import hash_collection, utc_datetime_from_timestamp
 from dagster._utils.caching_instance_queryer import CachingInstanceQueryer
 
 if TYPE_CHECKING:
     from .backfill import PartitionBackfill
 
 
 class AssetBackfillStatus(Enum):
@@ -108,14 +109,15 @@
 
     target_subset: AssetGraphSubset
     requested_runs_for_target_roots: bool
     latest_storage_id: Optional[int]
     materialized_subset: AssetGraphSubset
     requested_subset: AssetGraphSubset
     failed_and_downstream_subset: AssetGraphSubset
+    backfill_start_time: datetime
 
     def is_complete(self) -> bool:
         """The asset backfill is complete when all runs to be requested have finished (success,
         failure, or cancellation). Since the AssetBackfillData object stores materialization states
         per asset partition, the daemon continues to update the backfill data until all runs have
         finished in order to display the final partition statuses in the UI.
         """
@@ -255,34 +257,39 @@
         first_subset = next(iter(subsets))
         if any(subset != first_subset for subset in subsets):
             return None
 
         return list(first_subset.get_partition_keys())
 
     @classmethod
-    def empty(cls, target_subset: AssetGraphSubset) -> "AssetBackfillData":
+    def empty(
+        cls, target_subset: AssetGraphSubset, backfill_start_time: datetime
+    ) -> "AssetBackfillData":
         asset_graph = target_subset.asset_graph
         return cls(
             target_subset=target_subset,
             requested_runs_for_target_roots=False,
             requested_subset=AssetGraphSubset(asset_graph),
             materialized_subset=AssetGraphSubset(asset_graph),
             failed_and_downstream_subset=AssetGraphSubset(asset_graph),
             latest_storage_id=None,
+            backfill_start_time=backfill_start_time,
         )
 
     @classmethod
     def is_valid_serialization(cls, serialized: str, asset_graph: AssetGraph) -> bool:
         storage_dict = json.loads(serialized)
         return AssetGraphSubset.can_deserialize(
             storage_dict["serialized_target_subset"], asset_graph
         )
 
     @classmethod
-    def from_serialized(cls, serialized: str, asset_graph: AssetGraph) -> "AssetBackfillData":
+    def from_serialized(
+        cls, serialized: str, asset_graph: AssetGraph, backfill_start_timestamp: float
+    ) -> "AssetBackfillData":
         storage_dict = json.loads(serialized)
 
         return cls(
             target_subset=AssetGraphSubset.from_storage_dict(
                 storage_dict["serialized_target_subset"], asset_graph
             ),
             requested_runs_for_target_roots=storage_dict["requested_runs_for_target_roots"],
@@ -292,23 +299,25 @@
             materialized_subset=AssetGraphSubset.from_storage_dict(
                 storage_dict["serialized_materialized_subset"], asset_graph
             ),
             failed_and_downstream_subset=AssetGraphSubset.from_storage_dict(
                 storage_dict["serialized_failed_subset"], asset_graph
             ),
             latest_storage_id=storage_dict["latest_storage_id"],
+            backfill_start_time=utc_datetime_from_timestamp(backfill_start_timestamp),
         )
 
     @classmethod
     def from_asset_partitions(
         cls,
         asset_graph: AssetGraph,
         partition_names: Optional[Sequence[str]],
         asset_selection: Sequence[AssetKey],
         dynamic_partitions_store: DynamicPartitionsStore,
+        backfill_start_time: datetime,
         all_partitions: bool,
     ) -> "AssetBackfillData":
         check.invariant(
             partition_names is None or all_partitions is False,
             "Can't provide both a set of partitions and all_partitions=True",
         )
 
@@ -352,19 +361,20 @@
                 target_subset |= asset_graph.bfs_filter_subsets(
                     dynamic_partitions_store,
                     lambda asset_key, _: asset_key in partitioned_asset_keys,
                     AssetGraphSubset(
                         asset_graph,
                         partitions_subsets_by_asset_key={root_asset_key: root_partitions_subset},
                     ),
+                    current_time=backfill_start_time,
                 )
         else:
             check.failed("Either partition_names must not be None or all_partitions must be True")
 
-        return cls.empty(target_subset)
+        return cls.empty(target_subset, backfill_start_time)
 
     def serialize(self, dynamic_partitions_store: DynamicPartitionsStore) -> str:
         storage_dict = {
             "requested_runs_for_target_roots": self.requested_runs_for_target_roots,
             "serialized_target_subset": self.target_subset.to_storage_dict(
                 dynamic_partitions_store=dynamic_partitions_store
             ),
@@ -398,24 +408,25 @@
     asset_graph = ExternalAssetGraph.from_workspace(
         workspace_process_context.create_request_context()
     )
     if backfill.serialized_asset_backfill_data is None:
         check.failed("Asset backfill missing serialized_asset_backfill_data")
 
     asset_backfill_data = AssetBackfillData.from_serialized(
-        backfill.serialized_asset_backfill_data, asset_graph
+        backfill.serialized_asset_backfill_data, asset_graph, backfill.backfill_timestamp
     )
 
     result = None
     for result in execute_asset_backfill_iteration_inner(
         backfill_id=backfill.backfill_id,
         asset_backfill_data=asset_backfill_data,
         instance=instance,
         asset_graph=asset_graph,
         run_tags=backfill.tags,
+        backfill_start_time=utc_datetime_from_timestamp(backfill.backfill_timestamp),
     ):
         yield None
 
     if not isinstance(result, AssetBackfillIterationResult):
         check.failed(
             "Expected execute_asset_backfill_iteration_inner to return an"
             " AssetBackfillIterationResult"
@@ -540,24 +551,27 @@
 
 def execute_asset_backfill_iteration_inner(
     backfill_id: str,
     asset_backfill_data: AssetBackfillData,
     asset_graph: ExternalAssetGraph,
     instance: DagsterInstance,
     run_tags: Mapping[str, str],
+    backfill_start_time: datetime,
 ) -> Iterable[Optional[AssetBackfillIterationResult]]:
     """Core logic of a backfill iteration. Has no side effects.
 
     Computes which runs should be requested, if any, as well as updated bookkeeping about the status
     of asset partitions targeted by the backfill.
 
     This is a generator so that we can return control to the daemon and let it heartbeat during
     expensive operations.
     """
-    instance_queryer = CachingInstanceQueryer(instance=instance)
+    instance_queryer = CachingInstanceQueryer(
+        instance=instance, evaluation_time=backfill_start_time
+    )
 
     initial_candidates: Set[AssetKeyPartitionKey] = set()
     request_roots = not asset_backfill_data.requested_runs_for_target_roots
     if request_roots:
         initial_candidates.update(asset_backfill_data.get_target_root_asset_partitions())
 
         next_latest_storage_id = instance_queryer.get_latest_storage_id(
@@ -615,14 +629,15 @@
             asset_graph.bfs_filter_asset_partitions(
                 instance_queryer,
                 lambda asset_partitions, _: any(
                     asset_partition in asset_backfill_data.target_subset
                     for asset_partition in asset_partitions
                 ),
                 _get_failed_asset_partitions(instance_queryer, backfill_id),
+                evaluation_time=backfill_start_time,
             ),
             asset_graph,
         )
 
         yield None
 
     asset_partitions_to_request = asset_graph.bfs_filter_asset_partitions(
@@ -631,16 +646,18 @@
             candidates_unit=unit,
             asset_partitions_to_request=visited,
             asset_graph=asset_graph,
             materialized_subset=updated_materialized_subset,
             target_subset=asset_backfill_data.target_subset,
             failed_and_downstream_subset=failed_and_downstream_subset,
             dynamic_partitions_store=instance_queryer,
+            current_time=backfill_start_time,
         ),
         initial_asset_partitions=initial_candidates,
+        evaluation_time=backfill_start_time,
     )
 
     run_requests = build_run_requests(
         asset_partitions_to_request, asset_graph, {**run_tags, BACKFILL_ID_TAG: backfill_id}
     )
 
     if request_roots:
@@ -653,40 +670,44 @@
         target_subset=asset_backfill_data.target_subset,
         latest_storage_id=next_latest_storage_id or asset_backfill_data.latest_storage_id,
         requested_runs_for_target_roots=asset_backfill_data.requested_runs_for_target_roots
         or request_roots,
         materialized_subset=updated_materialized_subset,
         failed_and_downstream_subset=failed_and_downstream_subset,
         requested_subset=asset_backfill_data.requested_subset | asset_partitions_to_request,
+        backfill_start_time=backfill_start_time,
     )
     yield AssetBackfillIterationResult(run_requests, updated_asset_backfill_data)
 
 
 def should_backfill_atomic_asset_partitions_unit(
     asset_graph: ExternalAssetGraph,
     candidates_unit: Iterable[AssetKeyPartitionKey],
     asset_partitions_to_request: AbstractSet[AssetKeyPartitionKey],
     target_subset: AssetGraphSubset,
     materialized_subset: AssetGraphSubset,
     failed_and_downstream_subset: AssetGraphSubset,
     dynamic_partitions_store: DynamicPartitionsStore,
+    current_time: datetime,
 ) -> bool:
     """Args:
     candidates_unit: A set of asset partitions that must all be materialized if any is
         materialized.
     """
     for candidate in candidates_unit:
         if (
             candidate not in target_subset
             or candidate in failed_and_downstream_subset
             or candidate in materialized_subset
         ):
             return False
 
-        for parent in asset_graph.get_parents_partitions(dynamic_partitions_store, *candidate):
+        for parent in asset_graph.get_parents_partitions(
+            dynamic_partitions_store, current_time, *candidate
+        ):
             can_run_with_parent = (
                 parent in asset_partitions_to_request
                 and asset_graph.have_same_partitioning(parent.asset_key, candidate.asset_key)
                 and parent.partition_key == candidate.partition_key
                 and asset_graph.get_repository_handle(candidate.asset_key)
                 is asset_graph.get_repository_handle(parent.asset_key)
             )
```

### Comparing `dagster-1.3.3/dagster/_core/execution/backfill.py` & `dagster-1.3.4/dagster/_core/execution/backfill.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 )
 from dagster._core.execution.bulk_actions import BulkActionType
 from dagster._core.host_representation.origin import ExternalPartitionSetOrigin
 from dagster._core.instance import DynamicPartitionsStore
 from dagster._core.storage.tags import USER_TAG
 from dagster._core.workspace.workspace import IWorkspace
 from dagster._serdes import whitelist_for_serdes
+from dagster._utils import utc_datetime_from_timestamp
 from dagster._utils.error import SerializableErrorInfo
 
 from .asset_backfill import (
     AssetBackfillData,
     PartitionedAssetBackfillStatus,
     UnpartitionedAssetBackfillStatus,
 )
@@ -148,14 +149,15 @@
             return []
 
         if self.serialized_asset_backfill_data is not None:
             try:
                 asset_backfill_data = AssetBackfillData.from_serialized(
                     self.serialized_asset_backfill_data,
                     ExternalAssetGraph.from_workspace(workspace),
+                    self.backfill_timestamp,
                 )
             except DagsterDefinitionChangedDeserializationError:
                 return []
 
             return asset_backfill_data.get_backfill_status_per_asset_key()
         else:
             return []
@@ -167,14 +169,15 @@
             return None
 
         if self.serialized_asset_backfill_data is not None:
             try:
                 asset_backfill_data = AssetBackfillData.from_serialized(
                     self.serialized_asset_backfill_data,
                     ExternalAssetGraph.from_workspace(workspace),
+                    self.backfill_timestamp,
                 )
             except DagsterDefinitionChangedDeserializationError:
                 return None
 
             return asset_backfill_data.get_target_root_partitions_subset()
         else:
             return None
@@ -184,14 +187,15 @@
             return 0
 
         if self.serialized_asset_backfill_data is not None:
             try:
                 asset_backfill_data = AssetBackfillData.from_serialized(
                     self.serialized_asset_backfill_data,
                     ExternalAssetGraph.from_workspace(workspace),
+                    self.backfill_timestamp,
                 )
             except DagsterDefinitionChangedDeserializationError:
                 return 0
 
             return asset_backfill_data.get_num_partitions()
         else:
             if self.partition_names is None:
@@ -204,14 +208,15 @@
             return []
 
         if self.serialized_asset_backfill_data is not None:
             try:
                 asset_backfill_data = AssetBackfillData.from_serialized(
                     self.serialized_asset_backfill_data,
                     ExternalAssetGraph.from_workspace(workspace),
+                    self.backfill_timestamp,
                 )
             except DagsterDefinitionChangedDeserializationError:
                 return None
 
             return asset_backfill_data.get_partition_names()
         else:
             if self.partition_names is None:
@@ -340,9 +345,10 @@
             asset_selection=asset_selection,
             serialized_asset_backfill_data=AssetBackfillData.from_asset_partitions(
                 asset_graph=asset_graph,
                 partition_names=partition_names,
                 asset_selection=asset_selection,
                 dynamic_partitions_store=dynamic_partitions_store,
                 all_partitions=all_partitions,
+                backfill_start_time=utc_datetime_from_timestamp(backfill_timestamp),
             ).serialize(dynamic_partitions_store=dynamic_partitions_store),
         )
```

### Comparing `dagster-1.3.3/dagster/_core/execution/build_resources.py` & `dagster-1.3.4/dagster/_core/execution/build_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/compute_logs.py` & `dagster-1.3.4/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/context/compute.py` & `dagster-1.3.4/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/context/hook.py` & `dagster-1.3.4/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/context/init.py` & `dagster-1.3.4/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/context/input.py` & `dagster-1.3.4/dagster/_core/execution/context/input.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,16 +408,16 @@
                 ),
             )
 
         time_windows = subset.included_time_windows
         if len(time_windows) != 1:
             check.failed(
                 (
-                    "Tried to access asset_partition_key_range, but there are "
-                    f"({len(time_windows)}) partitions associated with this input."
+                    "Tried to access asset_partitions_time_window, but there are "
+                    f"({len(time_windows)}) time windows associated with this input."
                 ),
             )
 
         return time_windows[0]
 
     @public
     def get_identifier(self) -> Sequence[str]:
@@ -588,15 +588,15 @@
     metadata = check.opt_mapping_param(metadata, "metadata", key_type=str)
     upstream_output = check.opt_inst_param(upstream_output, "upstream_output", OutputContext)
     dagster_type = check.opt_inst_param(dagster_type, "dagster_type", DagsterType)
     resource_config = check.opt_mapping_param(resource_config, "resource_config", key_type=str)
     resources = check.opt_mapping_param(resources, "resources", key_type=str)
     op_def = check.opt_inst_param(op_def, "op_def", OpDefinition)
     step_context = check.opt_inst_param(step_context, "step_context", StepExecutionContext)
-    asset_key = AssetKey.from_coerceable(asset_key) if asset_key else None
+    asset_key = AssetKey.from_coercible(asset_key) if asset_key else None
     partition_key = check.opt_str_param(partition_key, "partition_key")
     asset_partition_key_range = check.opt_inst_param(
         asset_partition_key_range, "asset_partition_key_range", PartitionKeyRange
     )
     asset_partitions_def = check.opt_inst_param(
         asset_partitions_def, "asset_partitions_def", PartitionsDefinition
     )
```

### Comparing `dagster-1.3.3/dagster/_core/execution/context/invocation.py` & `dagster-1.3.4/dagster/_core/execution/context/invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/context/logger.py` & `dagster-1.3.4/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/context/output.py` & `dagster-1.3.4/dagster/_core/execution/context/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -853,15 +853,15 @@
     run_id = check.opt_str_param(run_id, "run_id", default=RUN_ID_PLACEHOLDER)
     mapping_key = check.opt_str_param(mapping_key, "mapping_key")
     dagster_type = check.opt_inst_param(dagster_type, "dagster_type", DagsterType)
     version = check.opt_str_param(version, "version")
     resource_config = check.opt_mapping_param(resource_config, "resource_config", key_type=str)
     resources = check.opt_mapping_param(resources, "resources", key_type=str)
     op_def = check.opt_inst_param(op_def, "op_def", OpDefinition)
-    asset_key = AssetKey.from_coerceable(asset_key) if asset_key else None
+    asset_key = AssetKey.from_coercible(asset_key) if asset_key else None
     partition_key = check.opt_str_param(partition_key, "partition_key")
 
     return OutputContext(
         step_key=step_key,
         name=name,
         job_name=None,
         run_id=run_id,
```

### Comparing `dagster-1.3.3/dagster/_core/execution/context/system.py` & `dagster-1.3.4/dagster/_core/execution/context/system.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/context_creation_job.py` & `dagster-1.3.4/dagster/_core/execution/context_creation_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,15 +407,15 @@
     raise_on_error: Optional[bool] = False,
 ) -> Generator[PlanExecutionContext, None, None]:
     """Utility context manager which acts as a very thin wrapper around
     `pipeline_initialization_manager`, iterating through all the setup/teardown events and
     discarding them.  It yields the resulting `pipeline_context`.
 
     Should only be used where we need to reconstruct the pipeline context, ignoring any yielded
-    events (e.g. PipelineExecutionResult, dagstermill, unit tests, etc)
+    events (e.g. JobExecutionResult, dagstermill, unit tests, etc)
     """
     check.inst_param(execution_plan, "execution_plan", ExecutionPlan)
     check.inst_param(job, "job", IJob)
     check.mapping_param(run_config, "run_config", key_type=str)
     check.inst_param(dagster_run, "dagster_run", DagsterRun)
     check.inst_param(instance, "instance", DagsterInstance)
     check.callable_param(scoped_resources_builder_cm, "scoped_resources_builder_cm")
```

### Comparing `dagster-1.3.3/dagster/_core/execution/execute_in_process.py` & `dagster-1.3.4/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.3.4/dagster/_core/execution/execute_in_process_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         return super(ExecuteInProcessResult, self).output_for_node(
             node_str, output_name=output_name
         )
 
     @public
     def asset_value(self, asset_key: CoercibleToAssetKey) -> Any:
         node_output_handle = self._job_def.asset_layer.node_output_handle_for_asset(
-            AssetKey.from_coerceable(asset_key)
+            AssetKey.from_coercible(asset_key)
         )
         return self.output_for_node(
             node_str=str(node_output_handle.node_handle), output_name=node_output_handle.output_name
         )
 
     @public
     def output_value(self, output_name: str = DEFAULT_OUTPUT) -> Any:
```

### Comparing `dagster-1.3.3/dagster/_core/execution/execute_job_result.py` & `dagster-1.3.4/dagster/_core/execution/job_execution_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from dagster._core.events import DagsterEvent
 from dagster._core.execution.plan.utils import build_resources_for_manager
 from dagster._core.storage.dagster_run import DagsterRun
 
 from .execution_result import ExecutionResult
 
 
-class ExecuteJobResult(ExecutionResult):
+class JobExecutionResult(ExecutionResult):
     """Result object returned by :py:func:`dagster.execute_job`.
 
     Used for retrieving run success, events, and outputs from `execute_job`.
     Users should not directly instantiate this class.
 
     Events and run information can be retrieved off of the object directly. In
     order to access outputs, the `ExecuteJobResult` object needs to be opened
@@ -27,15 +27,15 @@
     def __init__(self, job_def, reconstruct_context, event_list, dagster_run):
         self._job_def = job_def
         self._reconstruct_context = reconstruct_context
         self._context = None
         self._event_list = event_list
         self._dagster_run = dagster_run
 
-    def __enter__(self) -> "ExecuteJobResult":
+    def __enter__(self) -> "JobExecutionResult":
         context = self._reconstruct_context.__enter__()
         self._context = context
         return self
 
     def __exit__(self, *exc):
         exit_result = self._reconstruct_context.__exit__(*exc)
         self._context = None
@@ -70,15 +70,15 @@
         Args:
             output_name (Optional[str]): The name of the output to retrieve. Defaults to `result`,
                 the default output name in dagster.
 
         Returns:
             Any: The value of the retrieved output.
         """
-        return super(ExecuteJobResult, self).output_value(output_name=output_name)
+        return super(JobExecutionResult, self).output_value(output_name=output_name)
 
     @public
     def output_for_node(self, node_str: str, output_name: str = DEFAULT_OUTPUT) -> Any:
         """Retrieves output value with a particular name from the run of the job.
 
         In order to use this method, the `ExecuteJobResult` object must be opened as a context manager. If this method is used without opening the context manager, it will result in a :py:class:`DagsterInvariantViolationError`.
 
@@ -87,15 +87,15 @@
                 graph/op is nested within another graph, the syntax is `outer_graph.inner_node`.
             output_name (Optional[str]): Name of the output on the op/graph to retrieve. Defaults to
                 `result`, the default output name in dagster.
 
         Returns:
             Any: The value of the retrieved output.
         """
-        return super(ExecuteJobResult, self).output_for_node(node_str, output_name=output_name)
+        return super(JobExecutionResult, self).output_for_node(node_str, output_name=output_name)
 
     def _get_output_for_handle(self, handle: NodeHandle, output_name: str) -> Any:
         if not self._context:
             raise DagsterInvariantViolationError(
                 "In order to access output objects, the result of `execute_job` must be opened as a"
                 " context manager: 'with execute_job(...) as result:"
             )
```

### Comparing `dagster-1.3.3/dagster/_core/execution/execution_result.py` & `dagster-1.3.4/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/host_mode.py` & `dagster-1.3.4/dagster/_core/execution/host_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,18 +185,16 @@
         dagster_run.status == DagsterRunStatus.NOT_STARTED
         or dagster_run.status == DagsterRunStatus.STARTING,
         desc="Pipeline run {} ({}) in state {}, expected NOT_STARTED or STARTING".format(
             dagster_run.job_name, dagster_run.run_id, dagster_run.status
         ),
     )
 
-    recon_job = recon_job.subset_for_execution_from_existing_job(
-        solids_to_execute=frozenset(dagster_run.solids_to_execute)
-        if dagster_run.solids_to_execute
-        else None,
+    recon_job = recon_job.get_subset(
+        op_selection=dagster_run.solids_to_execute,
         asset_selection=dagster_run.asset_selection,
     )
 
     execution_plan_snapshot = instance.get_execution_plan_snapshot(
         check.not_none(dagster_run.execution_plan_snapshot_id)
     )
     execution_plan = ExecutionPlan.rebuild_from_snapshot(
```

### Comparing `dagster-1.3.3/dagster/_core/execution/job_backfill.py` & `dagster-1.3.4/dagster/_core/execution/job_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/memoization.py` & `dagster-1.3.4/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/plan/active.py` & `dagster-1.3.4/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/plan/compute.py` & `dagster-1.3.4/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.3.4/dagster/_core/execution/plan/compute_generator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.3.4/dagster/_core/execution/plan/execute_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
             An unexpected error occurred. Either there has been an internal error in the framework
             OR we have forgotten to put a user code error boundary around invoked user-space code.
 
 
     The "raised_dagster_errors" context manager can be used to force these errors to be
     re-raised and surfaced to the user. This is mostly to get sensible errors in test and
     ad-hoc contexts, rather than forcing the user to wade through the
-    PipelineExecutionResult API in order to find the step that failed.
+    JobExecutionResult API in order to find the step that failed.
 
     For tools, however, this option should be false, and a sensible error message
     signaled to the user within that tool.
 
     When we launch a step that has a step launcher, we use this function on both the host process
     and the remote process. When we run the step in the remote process, to prevent an infinite loop
     of launching steps that then launch steps, and so on, the remote process will run this with
```

### Comparing `dagster-1.3.3/dagster/_core/execution/plan/execute_step.py` & `dagster-1.3.4/dagster/_core/execution/plan/execute_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/plan/external_step.py` & `dagster-1.3.4/dagster/_core/execution/plan/external_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                     container_image=recon_job.repository.container_image,
                     executable_path=recon_job.repository.executable_path,
                     entry_point=recon_job.repository.entry_point,
                     container_context=recon_job.repository.container_context,
                     repository_load_data=step_context.plan_data.execution_plan.repository_load_data,
                 ),
                 job_name=recon_job.job_name,
-                solids_to_execute=recon_job.solids_to_execute,
+                op_selection=recon_job.op_selection,
             )
 
     return StepRunRef(
         run_config=step_context.run_config,
         dagster_run=step_context.dagster_run,
         run_id=step_context.dagster_run.run_id,
         step_key=step_context.step.key,
@@ -184,16 +184,16 @@
 ) -> StepExecutionContext:
     check.inst_param(instance, "instance", DagsterInstance)
 
     job = step_run_ref.recon_job
 
     solids_to_execute = step_run_ref.dagster_run.solids_to_execute
     if solids_to_execute or step_run_ref.dagster_run.asset_selection:
-        job = step_run_ref.recon_job.subset_for_execution_from_existing_job(
-            frozenset(solids_to_execute) if solids_to_execute else None,
+        job = step_run_ref.recon_job.get_subset(
+            op_selection=solids_to_execute,
             asset_selection=step_run_ref.dagster_run.asset_selection,
         )
 
     execution_plan = create_execution_plan(
         job,
         step_run_ref.run_config,
         step_keys_to_execute=[step_run_ref.step_key],
```

### Comparing `dagster-1.3.3/dagster/_core/execution/plan/handle.py` & `dagster-1.3.4/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/plan/inputs.py` & `dagster-1.3.4/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.3.4/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/plan/objects.py` & `dagster-1.3.4/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/plan/outputs.py` & `dagster-1.3.4/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/plan/plan.py` & `dagster-1.3.4/dagster/_core/execution/plan/plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/plan/state.py` & `dagster-1.3.4/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/plan/step.py` & `dagster-1.3.4/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/plan/utils.py` & `dagster-1.3.4/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.3.4/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/resolve_versions.py` & `dagster-1.3.4/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/resources_init.py` & `dagster-1.3.4/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/retries.py` & `dagster-1.3.4/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.3.4/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/stats.py` & `dagster-1.3.4/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/tags.py` & `dagster-1.3.4/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/validate_run_config.py` & `dagster-1.3.4/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/watch_orphans.py` & `dagster-1.3.4/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/execution/with_resources.py` & `dagster-1.3.4/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/executor/base.py` & `dagster-1.3.4/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/executor/child_process_executor.py` & `dagster-1.3.4/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/executor/in_process.py` & `dagster-1.3.4/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/executor/init.py` & `dagster-1.3.4/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/executor/multiprocess.py` & `dagster-1.3.4/dagster/_core/executor/multiprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.3.4/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.3.4/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/host_representation/__init__.py` & `dagster-1.3.4/dagster/_core/host_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/host_representation/code_location.py` & `dagster-1.3.4/dagster/_core/host_representation/code_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,17 +386,17 @@
         )
         check.opt_inst_param(known_state, "known_state", KnownExecutionState)
         check.opt_inst_param(instance, "instance", DagsterInstance)
 
         execution_plan = create_execution_plan(
             job=self.get_reconstructable_job(
                 external_job.repository_handle.repository_name, external_job.name
-            ).subset_for_execution_from_existing_job(
-                external_job.solids_to_execute,
-                external_job.asset_selection,
+            ).get_subset(
+                op_selection=external_job.solids_to_execute,
+                asset_selection=external_job.asset_selection,
             ),
             run_config=run_config,
             step_keys_to_execute=step_keys_to_execute,
             known_state=known_state,
             instance_ref=instance.get_ref() if instance and instance.is_persistent else None,
         )
         return ExternalExecutionPlan(
```

### Comparing `dagster-1.3.3/dagster/_core/host_representation/external.py` & `dagster-1.3.4/dagster/_core/host_representation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/host_representation/external_data.py` & `dagster-1.3.4/dagster/_core/host_representation/external_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     List,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
     Set,
     Tuple,
+    Type,
     Union,
     cast,
 )
 
 import pendulum
 from typing_extensions import Final
 
@@ -1560,14 +1561,19 @@
     else:
         return {
             k: NestedResource(NestedResourceType.TOP_LEVEL, k)
             for k in resource_def.required_resource_keys
         }
 
 
+def _get_class_name(cls: Type) -> str:
+    """Returns the fully qualified class name of the given class."""
+    return str(cls)[8:-2]
+
+
 def external_resource_data_from_def(
     name: str,
     resource_def: ResourceDefinition,
     nested_resources: Mapping[str, NestedResource],
     parent_resources: Mapping[str, str],
     resource_asset_usage_map: Mapping[str, List[AssetKey]],
     resource_job_usage_map: ResourceJobUsageMap,
@@ -1600,15 +1606,25 @@
     configured_values = {
         k: external_resource_value_from_raw(v) for k, v in config_schema_default.items()
     }
 
     resource_type_def = resource_def
     if isinstance(resource_type_def, ResourceWithKeyMapping):
         resource_type_def = resource_type_def.wrapped_resource
-    resource_type = str(type(resource_type_def))[8:-2]
+
+    resource_type = _get_class_name(type(resource_type_def))
+
+    if isinstance(
+        resource_type_def,
+        (
+            ConfigurableResourceFactoryResourceDefinition,
+            ConfigurableIOManagerFactoryResourceDefinition,
+        ),
+    ):
+        resource_type = _get_class_name(resource_type_def.configurable_resource_cls)
 
     return ExternalResourceData(
         name=name,
         resource_snapshot=build_resource_def_snap(name, resource_def),
         configured_values=configured_values,
         config_field_snaps=unconfigured_config_type_snap.fields or [],
         config_schema_snap=config_type.get_schema_snapshot(),
```

### Comparing `dagster-1.3.3/dagster/_core/host_representation/grpc_server_registry.py` & `dagster-1.3.4/dagster/_core/host_representation/grpc_server_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/host_representation/grpc_server_state_subscriber.py` & `dagster-1.3.4/dagster/_core/host_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/host_representation/handle.py` & `dagster-1.3.4/dagster/_core/host_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/host_representation/historical.py` & `dagster-1.3.4/dagster/_core/host_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/host_representation/job_index.py` & `dagster-1.3.4/dagster/_core/host_representation/job_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/host_representation/origin.py` & `dagster-1.3.4/dagster/_core/host_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/host_representation/represented.py` & `dagster-1.3.4/dagster/_core/host_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/instance/__init__.py` & `dagster-1.3.4/dagster/_core/instance/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 import logging.config
 import os
 import sys
 import time
 import weakref
+from abc import abstractmethod
 from collections import defaultdict
 from enum import Enum
 from tempfile import TemporaryDirectory
 from types import TracebackType
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
@@ -262,21 +263,21 @@
 
         # Store a weakref to avoid a circular reference / enable GC
         self._instance_weakref = weakref.ref(instance)
 
 
 @runtime_checkable
 class DynamicPartitionsStore(Protocol):
+    @abstractmethod
     def get_dynamic_partitions(self, partitions_def_name: str) -> Sequence[str]:
-        return self.get_dynamic_partitions(partitions_def_name=partitions_def_name)
+        ...
 
+    @abstractmethod
     def has_dynamic_partition(self, partitions_def_name: str, partition_key: str) -> bool:
-        return self.has_dynamic_partition(
-            partitions_def_name=partitions_def_name, partition_key=partition_key
-        )
+        ...
 
 
 class DagsterInstance(DynamicPartitionsStore):
     """Core abstraction for managing Dagster's access to storage and other resources.
 
     Use DagsterInstance.get() to grab the current DagsterInstance which will load based on
     the values in the ``dagster.yaml`` file in ``$DAGSTER_HOME``.
@@ -305,20 +306,20 @@
             pipeline runs. By default, this will be a
             :py:class:`dagster._core.storage.runs.SqliteRunStorage`. Configurable in ``dagster.yaml``
             using the :py:class:`~dagster.serdes.ConfigurableClass` machinery.
         event_storage (EventLogStorage): Used to store the structured event logs generated by
             pipeline runs. By default, this will be a
             :py:class:`dagster._core.storage.event_log.SqliteEventLogStorage`. Configurable in
             ``dagster.yaml`` using the :py:class:`~dagster.serdes.ConfigurableClass` machinery.
-        compute_log_manager (ComputeLogManager): The compute log manager handles stdout and stderr
-            logging for op compute functions. By default, this will be a
+        compute_log_manager (Optional[ComputeLogManager]): The compute log manager handles stdout
+            and stderr logging for op compute functions. By default, this will be a
             :py:class:`dagster._core.storage.local_compute_log_manager.LocalComputeLogManager`.
             Configurable in ``dagster.yaml`` using the
             :py:class:`~dagster.serdes.ConfigurableClass` machinery.
-        run_coordinator (RunCoordinator): A runs coordinator may be used to manage the execution
+        run_coordinator (Optional[RunCoordinator]): A runs coordinator may be used to manage the execution
             of pipeline runs.
         run_launcher (Optional[RunLauncher]): Optionally, a run launcher may be used to enable
             a Dagster instance to launch pipeline runs, e.g. on a remote Kubernetes cluster, in
             addition to running them locally.
         settings (Optional[Dict]): Specifies certain per-instance settings,
             such as feature flags. These are set in the ``dagster.yaml`` under a set of whitelisted
             keys.
@@ -334,16 +335,16 @@
 
     def __init__(
         self,
         instance_type: InstanceType,
         local_artifact_storage: "LocalArtifactStorage",
         run_storage: "RunStorage",
         event_storage: "EventLogStorage",
-        compute_log_manager: "ComputeLogManager",
-        run_coordinator: "RunCoordinator",
+        run_coordinator: Optional["RunCoordinator"],
+        compute_log_manager: Optional["ComputeLogManager"],
         run_launcher: Optional["RunLauncher"],
         scheduler: Optional["Scheduler"] = None,
         schedule_storage: Optional["ScheduleStorage"] = None,
         settings: Optional[Mapping[str, Any]] = None,
         secrets_loader: Optional["SecretsLoader"] = None,
         ref: Optional[InstanceRef] = None,
     ):
@@ -364,32 +365,47 @@
         )
         self._event_storage = check.inst_param(event_storage, "event_storage", EventLogStorage)
         self._event_storage.register_instance(self)
 
         self._run_storage = check.inst_param(run_storage, "run_storage", RunStorage)
         self._run_storage.register_instance(self)
 
-        self._compute_log_manager = check.inst_param(
-            compute_log_manager, "compute_log_manager", ComputeLogManager
-        )
-        if not isinstance(self._compute_log_manager, CapturedLogManager):
-            deprecation_warning(
-                "ComputeLogManager", "1.2.0", "Implement the CapturedLogManager interface instead."
+        if compute_log_manager:
+            self._compute_log_manager = check.inst_param(
+                compute_log_manager, "compute_log_manager", ComputeLogManager
+            )
+            if not isinstance(self._compute_log_manager, CapturedLogManager):
+                deprecation_warning(
+                    "ComputeLogManager",
+                    "1.2.0",
+                    "Implement the CapturedLogManager interface instead.",
+                )
+            self._compute_log_manager.register_instance(self)
+        else:
+            check.invariant(
+                ref, "Compute log manager must be provided if instance is not from a ref"
             )
-        self._compute_log_manager.register_instance(self)
+            self._compute_log_manager = None
+
         self._scheduler = check.opt_inst_param(scheduler, "scheduler", Scheduler)
 
         self._schedule_storage = check.opt_inst_param(
             schedule_storage, "schedule_storage", ScheduleStorage
         )
         if self._schedule_storage:
             self._schedule_storage.register_instance(self)
 
-        self._run_coordinator = check.inst_param(run_coordinator, "run_coordinator", RunCoordinator)
-        self._run_coordinator.register_instance(self)
+        if run_coordinator:
+            self._run_coordinator = check.inst_param(
+                run_coordinator, "run_coordinator", RunCoordinator
+            )
+            self._run_coordinator.register_instance(self)
+        else:
+            check.invariant(ref, "Run coordinator must be provided if instance is not from a ref")
+            self._run_coordinator = None
 
         if run_launcher:
             self._run_launcher: Optional[RunLauncher] = check.inst_param(
                 run_launcher, "run_launcher", RunLauncher
             )
             run_launcher.register_instance(self)
         else:
@@ -544,17 +560,17 @@
 
         return klass(
             instance_type=InstanceType.PERSISTENT,
             local_artifact_storage=instance_ref.local_artifact_storage,
             run_storage=run_storage,  # type: ignore  # (possible none)
             event_storage=event_storage,  # type: ignore  # (possible none)
             schedule_storage=schedule_storage,
-            compute_log_manager=instance_ref.compute_log_manager,
+            compute_log_manager=None,  # lazy load
             scheduler=instance_ref.scheduler,
-            run_coordinator=instance_ref.run_coordinator,  # type: ignore  # (possible none)
+            run_coordinator=None,  # lazy load
             run_launcher=None,  # lazy load
             settings=instance_ref.settings,
             secrets_loader=instance_ref.secrets_loader,
             ref=instance_ref,
             **kwargs,
         )
 
@@ -677,14 +693,26 @@
     def scheduler_class(self) -> Optional[str]:
         return self.scheduler.__class__.__name__ if self.scheduler else None
 
     # run coordinator
 
     @property
     def run_coordinator(self) -> "RunCoordinator":
+        from dagster._core.run_coordinator import RunCoordinator
+
+        # Lazily load in case the run coordinator requires dependencies that are not available
+        # everywhere that loads the instance
+        if not self._run_coordinator:
+            check.invariant(
+                self._ref, "Run coordinator not provided, and no instance ref available"
+            )
+            run_coordinator = cast(InstanceRef, self._ref).run_coordinator
+            check.invariant(run_coordinator, "Run coordinator not configured in instance ref")
+            self._run_coordinator = cast(RunCoordinator, run_coordinator)
+            self._run_coordinator.register_instance(self)
         return self._run_coordinator
 
     # run launcher
 
     @property
     def run_launcher(self) -> "RunLauncher":
         from dagster._core.launcher import RunLauncher
@@ -699,14 +727,26 @@
             self._run_launcher.register_instance(self)
         return self._run_launcher
 
     # compute logs
 
     @property
     def compute_log_manager(self) -> "ComputeLogManager":
+        from dagster._core.storage.compute_log_manager import ComputeLogManager
+
+        if not self._compute_log_manager:
+            check.invariant(
+                self._ref, "Compute log manager not provided, and no instance ref available"
+            )
+            compute_log_manager = cast(InstanceRef, self._ref).compute_log_manager
+            check.invariant(
+                compute_log_manager, "Compute log manager not configured in instance ref"
+            )
+            self._compute_log_manager = cast(ComputeLogManager, compute_log_manager)
+            self._compute_log_manager.register_instance(self)
         return self._compute_log_manager
 
     def get_settings(self, settings_key: str) -> Any:
         check.str_param(settings_key, "settings_key")
         if self._settings and settings_key in self._settings:
             return self._settings.get(settings_key)
         return {}
@@ -755,14 +795,18 @@
         return self.get_settings("run_monitoring")
 
     @property
     def run_monitoring_start_timeout_seconds(self) -> int:
         return self.run_monitoring_settings.get("start_timeout_seconds", 180)
 
     @property
+    def run_monitoring_cancel_timeout_seconds(self) -> int:
+        return self.run_monitoring_settings.get("cancel_timeout_seconds", 180)
+
+    @property
     def code_server_settings(self) -> Any:
         return self.get_settings("code_servers")
 
     @property
     def code_server_process_startup_timeout(self) -> int:
         return self.code_server_settings.get(
             "local_startup_timeout", DEFAULT_LOCAL_CODE_SERVER_STARTUP_TIMEOUT
@@ -856,19 +900,21 @@
         self._run_storage.optimize(print_fn)
         self._schedule_storage.optimize(print_fn)  # type: ignore  # (possible none)
         print_fn("Done.")
 
     def dispose(self) -> None:
         self._local_artifact_storage.dispose()
         self._run_storage.dispose()
-        self.run_coordinator.dispose()
+        if self._run_coordinator:
+            self._run_coordinator.dispose()
         if self._run_launcher:
             self._run_launcher.dispose()
         self._event_storage.dispose()
-        self._compute_log_manager.dispose()
+        if self._compute_log_manager:
+            self._compute_log_manager.dispose()
         if self._secrets_loader:
             self._secrets_loader.dispose()
 
         if self in DagsterInstance._TEMP_DIRS:
             DagsterInstance._TEMP_DIRS[self].cleanup()
             del DagsterInstance._TEMP_DIRS[self]
 
@@ -982,15 +1028,15 @@
         check.opt_set_param(solids_to_execute, "solids_to_execute", of_type=str)
         check.opt_list_param(solid_selection, "solid_selection", of_type=str)
         check.opt_set_param(asset_selection, "asset_selection", of_type=AssetKey)
 
         # solids_to_execute never provided
         if asset_selection or solid_selection:
             # for cases when `create_run_for_pipeline` is directly called
-            job_def = job_def.get_job_def_for_subset_selection(
+            job_def = job_def.get_subset(
                 asset_selection=asset_selection,
                 op_selection=solid_selection,
             )
         step_keys_to_execute = None
 
         if execution_plan:
             step_keys_to_execute = execution_plan.step_keys_to_execute
@@ -1642,16 +1688,17 @@
     @traced
     def get_records_for_run(
         self,
         run_id: str,
         cursor: Optional[str] = None,
         of_type: Optional[Union["DagsterEventType", Set["DagsterEventType"]]] = None,
         limit: Optional[int] = None,
+        ascending: bool = True,
     ) -> "EventLogConnection":
-        return self._event_storage.get_records_for_run(run_id, cursor, of_type, limit)
+        return self._event_storage.get_records_for_run(run_id, cursor, of_type, limit, ascending)
 
     def watch_event_logs(self, run_id: str, cursor: Optional[str], cb: "EventHandlerFn") -> None:
         return self._event_storage.watch(run_id, cursor, cb)
 
     def end_watch_event_logs(self, run_id: str, cb: "EventHandlerFn") -> None:
         return self._event_storage.end_watch(run_id, cb)
 
@@ -2047,15 +2094,15 @@
         check.inst(
             run.job_code_origin,
             JobPythonOrigin,
             "Python origin must be set for submitted runs",
         )
 
         try:
-            submitted_run = self._run_coordinator.submit_run(
+            submitted_run = self.run_coordinator.submit_run(
                 SubmitRunContext(run, workspace=workspace)
             )
         except:
             from dagster._core.events import EngineEventData
 
             error = serializable_error_info_from_exc_info(sys.exc_info())
             self.report_engine_event(
```

### Comparing `dagster-1.3.3/dagster/_core/instance/config.py` & `dagster-1.3.4/dagster/_core/instance/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,14 +299,15 @@
         ),
         "instance_class": config_field_for_configurable_class(),
         "python_logs": python_logs_config_schema(),
         "run_monitoring": Field(
             {
                 "enabled": Field(Bool, is_required=False),
                 "start_timeout_seconds": Field(int, is_required=False),
+                "cancel_timeout_seconds": Field(int, is_required=False),
                 "max_resume_run_attempts": Field(int, is_required=False),
                 "poll_interval_seconds": Field(int, is_required=False),
                 "cancellation_thread_poll_interval_seconds": Field(int, is_required=False),
             },
         ),
         "run_retries": Field(
             {
```

### Comparing `dagster-1.3.3/dagster/_core/instance/ref.py` & `dagster-1.3.4/dagster/_core/instance/ref.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/instance_for_test.py` & `dagster-1.3.4/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/launcher/base.py` & `dagster-1.3.4/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.3.4/dagster/_core/launcher/default_run_launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,25 +159,26 @@
         if not self.has_instance:
             return False
 
         run = self._instance.get_run_by_id(run_id)
         if not run:
             return False
 
+        self._instance.report_run_canceling(run)
+
         client = self._get_grpc_client_for_termination(run_id)
 
         if not client:
             self._instance.report_engine_event(
                 message="Unable to get grpc client to send termination request to.",
                 dagster_run=run,
                 cls=self.__class__,
             )
             return False
 
-        self._instance.report_run_canceling(run)
         res = deserialize_value(
             client.cancel_execution(CancelExecutionRequest(run_id=run_id)), CancelExecutionResult
         )
         return res.success
 
     def join(self, timeout=30):
         # If this hasn't been initialized at all, we can just do a noop
```

### Comparing `dagster-1.3.3/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.3.4/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/log_manager.py` & `dagster-1.3.4/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/nux.py` & `dagster-1.3.4/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/origin.py` & `dagster-1.3.4/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/run_coordinator/base.py` & `dagster-1.3.4/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.3.4/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.3.4/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/scheduler/__init__.py` & `dagster-1.3.4/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/scheduler/execution.py` & `dagster-1.3.4/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/scheduler/instigation.py` & `dagster-1.3.4/dagster/_core/scheduler/instigation.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 )
 from dagster._core.definitions.selector import InstigatorSelector, RepositorySelector
 from dagster._core.host_representation.origin import ExternalInstigatorOrigin
 from dagster._serdes import create_snapshot_id
 from dagster._serdes.serdes import (
     whitelist_for_serdes,
 )
+from dagster._utils import xor
 from dagster._utils.error import SerializableErrorInfo
 from dagster._utils.merger import merge_dicts
 
 InstigatorData: TypeAlias = Union["ScheduleInstigatorData", "SensorInstigatorData"]
 
 
 @whitelist_for_serdes(old_storage_names={"JobStatus"})
@@ -29,14 +30,49 @@
 
     # The run instigator is running, but only because of its default setting
     AUTOMATICALLY_RUNNING = "AUTOMATICALLY_RUNNING"
 
     STOPPED = "STOPPED"
 
 
+@whitelist_for_serdes
+class DynamicPartitionsRequestResult(
+    NamedTuple(
+        "_DynamicPartitionsRequestResult",
+        [
+            ("partitions_def_name", str),
+            ("added_partitions", Optional[Sequence[str]]),
+            ("deleted_partitions", Optional[Sequence[str]]),
+            ("skipped_partitions", Sequence[str]),
+        ],
+    )
+):
+    def __new__(
+        cls,
+        partitions_def_name: str,
+        added_partitions: Optional[Sequence[str]],
+        deleted_partitions: Optional[Sequence[str]],
+        skipped_partitions: Sequence[str],
+    ):
+        check.opt_sequence_param(added_partitions, "added_partitions")
+        check.opt_sequence_param(deleted_partitions, "deleted_partitions")
+
+        # One of added_partitions or deleted_partitions must be a sequence, and the other must be None
+        if not xor(added_partitions is None, deleted_partitions is None):
+            check.failed("Exactly one of added_partitions and deleted_partitions must be provided")
+
+        return super(DynamicPartitionsRequestResult, cls).__new__(
+            cls,
+            check.str_param(partitions_def_name, "partitions_def_name"),
+            added_partitions,
+            deleted_partitions,
+            check.sequence_param(skipped_partitions, "skipped_partitions"),
+        )
+
+
 @whitelist_for_serdes(old_storage_names={"SensorJobData"})
 class SensorInstigatorData(
     NamedTuple(
         "_SensorInstigatorData",
         [
             # the last completed tick timestamp, exposed to the context as a deprecated field
             ("last_tick_timestamp", Optional[float]),
@@ -237,14 +273,24 @@
 
     def with_origin_run(self, origin_run_id: str) -> "InstigatorTick":
         return self._replace(tick_data=self.tick_data.with_origin_run(origin_run_id))
 
     def with_log_key(self, log_key: Sequence[str]) -> "InstigatorTick":
         return self._replace(tick_data=self.tick_data.with_log_key(log_key))
 
+    def with_dynamic_partitions_request_result(
+        self,
+        dynamic_partitions_request_result: DynamicPartitionsRequestResult,
+    ) -> "InstigatorTick":
+        return self._replace(
+            tick_data=self.tick_data.with_dynamic_partitions_request_result(
+                dynamic_partitions_request_result
+            )
+        )
+
     @property
     def instigator_origin_id(self) -> str:
         return self.tick_data.instigator_origin_id
 
     @property
     def selector_id(self) -> Optional[str]:
         return self.tick_data.selector_id
@@ -309,14 +355,20 @@
     def is_failure(self) -> bool:
         return self.tick_data.status == TickStatus.FAILURE
 
     @property
     def is_success(self) -> bool:
         return self.tick_data.status == TickStatus.SUCCESS
 
+    @property
+    def dynamic_partitions_request_results(
+        self,
+    ) -> Sequence[DynamicPartitionsRequestResult]:
+        return self.tick_data.dynamic_partitions_request_results
+
 
 @whitelist_for_serdes(
     old_storage_names={"JobTickData"},
     storage_field_names={
         "instigator_origin_id": "job_origin_id",
         "instigator_name": "job_name",
         "instigator_type": "job_type",
@@ -336,14 +388,18 @@
             ("error", Optional[SerializableErrorInfo]),
             ("skip_reason", Optional[str]),
             ("cursor", Optional[str]),
             ("origin_run_ids", Sequence[str]),
             ("failure_count", int),
             ("selector_id", Optional[str]),
             ("log_key", Optional[List[str]]),
+            (
+                "dynamic_partitions_request_results",
+                Sequence[DynamicPartitionsRequestResult],
+            ),
         ],
     )
 ):
     """This class defines the data that is serialized and stored for each schedule/sensor tick. We
     depend on the storage implementation to provide tick ids, and therefore separate all other
     data into this serializable class that can be stored independently of the id.
 
@@ -356,14 +412,17 @@
         run_id (str): The run created by the tick.
         error (SerializableErrorInfo): The error caught during execution. This is set only when
             the status is ``TickStatus.Failure``
         skip_reason (str): message for why the tick was skipped
         origin_run_ids (List[str]): The runs originated from the schedule/sensor.
         failure_count (int): The number of times this tick has failed. If the status is not
             FAILED, this is the number of previous failures before it reached the current state.
+        dynamic_partitions_request_results (Sequence[DynamicPartitionsRequestResult]): The results
+            of the dynamic partitions requests evaluated within the tick.
+
     """
 
     def __new__(
         cls,
         instigator_origin_id: str,
         instigator_name: str,
         instigator_type: InstigatorType,
@@ -374,14 +433,17 @@
         error: Optional[SerializableErrorInfo] = None,
         skip_reason: Optional[str] = None,
         cursor: Optional[str] = None,
         origin_run_ids: Optional[Sequence[str]] = None,
         failure_count: Optional[int] = None,
         selector_id: Optional[str] = None,
         log_key: Optional[List[str]] = None,
+        dynamic_partitions_request_results: Optional[
+            Sequence[DynamicPartitionsRequestResult]
+        ] = None,
     ):
         _validate_tick_args(instigator_type, status, run_ids, error, skip_reason)
         check.opt_list_param(log_key, "log_key", of_type=str)
         return super(TickData, cls).__new__(
             cls,
             check.str_param(instigator_origin_id, "instigator_origin_id"),
             check.str_param(instigator_name, "instigator_name"),
@@ -393,14 +455,19 @@
             error,  # validated in _validate_tick_args
             skip_reason,  # validated in _validate_tick_args
             cursor=check.opt_str_param(cursor, "cursor"),
             origin_run_ids=check.opt_sequence_param(origin_run_ids, "origin_run_ids", of_type=str),
             failure_count=check.opt_int_param(failure_count, "failure_count", 0),
             selector_id=check.opt_str_param(selector_id, "selector_id"),
             log_key=log_key,
+            dynamic_partitions_request_results=check.opt_sequence_param(
+                dynamic_partitions_request_results,
+                "dynamic_partitions_request_results",
+                of_type=DynamicPartitionsRequestResult,
+            ),
         )
 
     def with_status(
         self,
         status: TickStatus,
         error: Optional[SerializableErrorInfo] = None,
         timestamp: Optional[float] = None,
@@ -478,14 +545,29 @@
         return TickData(
             **merge_dicts(
                 self._asdict(),
                 {"log_key": check.list_param(log_key, "log_key", of_type=str)},
             )
         )
 
+    def with_dynamic_partitions_request_result(
+        self, dynamic_partitions_request_result: DynamicPartitionsRequestResult
+    ):
+        return TickData(
+            **merge_dicts(
+                self._asdict(),
+                {
+                    "dynamic_partitions_request_results": [
+                        *self.dynamic_partitions_request_results,
+                        dynamic_partitions_request_result,
+                    ]
+                },
+            )
+        )
+
 
 def _validate_tick_args(
     instigator_type: InstigatorType,
     status: TickStatus,
     run_ids: Optional[Sequence[str]] = None,
     error: Optional[SerializableErrorInfo] = None,
     skip_reason: Optional[str] = None,
```

### Comparing `dagster-1.3.3/dagster/_core/scheduler/scheduler.py` & `dagster-1.3.4/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/secrets/env_file.py` & `dagster-1.3.4/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/selector/subset_selector.py` & `dagster-1.3.4/dagster/_core/selector/subset_selector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import re
 import sys
 from collections import defaultdict, deque
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
-    Any,
     Callable,
     Dict,
     FrozenSet,
     Generic,
     Hashable,
     Iterable,
     List,
@@ -16,26 +15,26 @@
     MutableSet,
     NamedTuple,
     Optional,
     Sequence,
     Set,
     Tuple,
     TypeVar,
-    Union,
 )
 
-from typing_extensions import Final, Literal, TypeAlias
+from typing_extensions import Literal, TypeAlias
 
 from dagster._core.definitions.dependency import DependencyStructure
 from dagster._core.definitions.events import AssetKey
 from dagster._core.errors import DagsterExecutionStepNotFoundError, DagsterInvalidSubsetError
 from dagster._utils import check
 
 if TYPE_CHECKING:
     from dagster._core.definitions.assets import AssetsDefinition
+    from dagster._core.definitions.graph_definition import GraphDefinition
     from dagster._core.definitions.job_definition import JobDefinition
     from dagster._core.definitions.source_asset import SourceAsset
 
 MAX_NUM = sys.maxsize
 
 T = TypeVar("T")
 T_Hashable = TypeVar("T_Hashable", bound=Hashable)
@@ -126,15 +125,15 @@
             )
             for upstream_key in upstream_asset_keys:
                 upstream[asset_key].add(upstream_key)
                 downstream[upstream_key] = downstream.get(upstream_key, set()) | {asset_key}
     return {"upstream": upstream, "downstream": downstream}
 
 
-def generate_dep_graph(job_def: "JobDefinition") -> DependencyGraph[str]:
+def generate_dep_graph(job_def: "GraphDefinition") -> DependencyGraph[str]:
     """Pipeline to dependency graph. It currently only supports top-level solids.
 
     Args:
         pipeline (JobDefinition): The pipeline to execute.
 
     Returns:
         graph (Dict[str, Dict[str, Set[str]]]): the input and output dependency graph. e.g.
@@ -348,73 +347,18 @@
     # traverse graph to get up/downsteam items
     subset_list += traverser.fetch_upstream(item, up_depth)
     subset_list += traverser.fetch_downstream(item, down_depth)
 
     return subset_list
 
 
-class SelectionTreeLeaf:
-    """Marker for no further nesting selection needed."""
-
-
-SelectionTreeBranch: TypeAlias = Dict[str, "SelectionTree"]
-SelectionTree: TypeAlias = Union[SelectionTreeBranch, SelectionTreeLeaf]
-
-SELECTION_TREE_LEAF_NODE: Final = SelectionTreeLeaf()
-
-
-def convert_dot_separated_string_to_selection_tree(
-    tree: SelectionTreeBranch, splits: Sequence[str]
-) -> SelectionTreeBranch:
-    # For example:
-    # "subgraph.subsubgraph.return_one" => {"subgraph": {"subsubgraph": {"return_one":
-    # SELECTION_TREE_LEAF_NODE}}}
-    key = splits[0]
-    if len(splits) == 1:
-        tree[key] = SELECTION_TREE_LEAF_NODE
-    else:
-        curr_node = tree.get(key, {})
-        assert not isinstance(curr_node, SelectionTreeLeaf), "Invalid selection tree"
-        tree[key] = convert_dot_separated_string_to_selection_tree(curr_node, splits[1:])
-    return tree
-
-
-def parse_op_selection(
-    job_def: "JobDefinition", op_selection: Sequence[str]
-) -> SelectionTreeBranch:
-    """Parse  an op selection into a nested dictionary.
-
-    Examples:
-        ["subgraph.return_one", "subgraph.adder", "subgraph.add_one", "add_one"]
-        => {"subgraph": {{"return_one": LeafNodeSelection}, {"adder": LeafNodeSelection}, {"add_one": LeafNodeSelection}}, "add_one": LeafNodeSelection}
-
-        ["subgraph.subsubgraph.return_one"]
-        => {"subgraph": {"subsubgraph": {"return_one": LeafNodeSelection}}}
-
-        ["top_level_op_1+"]
-        => {"top_level_op_1": LeafNodeSelection, "top_level_op_2": LeafNodeSelection}
-    """
-    if any(["." in item for item in op_selection]):
-        resolved_op_selection_dict: Dict[str, Any] = {}
-        for item in op_selection:
-            convert_dot_separated_string_to_selection_tree(
-                resolved_op_selection_dict, splits=item.split(".")
-            )
-        return resolved_op_selection_dict
-
-    return {
-        top_level_op: SELECTION_TREE_LEAF_NODE
-        for top_level_op in parse_solid_selection(job_def, op_selection)
-    }
-
-
-def parse_solid_selection(
-    job_def: "JobDefinition",
-    solid_selection: Sequence[str],
-) -> FrozenSet[str]:
+def parse_op_queries(
+    graph_def: "GraphDefinition",
+    op_queries: Sequence[str],
+) -> AbstractSet[str]:
     """Take pipeline definition and a list of solid selection queries (inlcuding names of solid
         invocations. See syntax examples below) and return a set of the qualified solid names.
 
     It currently only supports top-level solids.
 
     Query syntax examples:
     - "some_solid": select "some_solid" itself
@@ -433,33 +377,33 @@
         solid_selection (List[str]): a list of the solid selection queries (including single solid
             names) to execute.
 
     Returns:
         FrozenSet[str]: a frozenset of qualified deduplicated solid names, empty if no qualified
             subset selected.
     """
-    check.sequence_param(solid_selection, "solid_selection", of_type=str)
+    check.sequence_param(op_queries, "solid_selection", of_type=str)
 
     # special case: select all
-    if len(solid_selection) == 1 and solid_selection[0] == "*":
-        return frozenset(job_def.graph.node_names())
+    if len(op_queries) == 1 and op_queries[0] == "*":
+        return frozenset(graph_def.node_names())
 
-    graph = generate_dep_graph(job_def)
-    solids_set: Set[str] = set()
+    graph = generate_dep_graph(graph_def)
+    node_names: Set[str] = set()
 
     # loop over clauses
-    for clause in solid_selection:
+    for clause in op_queries:
         subset = clause_to_subset(graph, clause, lambda x: x)
         if len(subset) == 0:
             raise DagsterInvalidSubsetError(
-                f"No qualified ops to execute found for op_selection={solid_selection}"
+                f"No qualified ops to execute found for op_selection={op_queries}"
             )
-        solids_set.update(subset)
+        node_names.update(subset)
 
-    return frozenset(solids_set)
+    return node_names
 
 
 def parse_step_selection(
     step_deps: Mapping[str, AbstractSet[str]], step_selection: Sequence[str]
 ) -> FrozenSet[str]:
     """Take the dependency dictionary generated while building execution plan and a list of step key
      selection queries and return a set of the qualified step keys.
```

### Comparing `dagster-1.3.3/dagster/_core/snap/__init__.py` & `dagster-1.3.4/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/snap/dagster_types.py` & `dagster-1.3.4/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/snap/dep_snapshot.py` & `dagster-1.3.4/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.3.4/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/snap/job_snapshot.py` & `dagster-1.3.4/dagster/_core/snap/job_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/snap/mode.py` & `dagster-1.3.4/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/snap/node.py` & `dagster-1.3.4/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/DEVELOPING.md` & `dagster-1.3.4/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/README.md` & `dagster-1.3.4/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/env.py` & `dagster-1.3.4/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.3.4/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/asset_value_loader.py` & `dagster-1.3.4/dagster/_core/storage/asset_value_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             partition_key (Optional[str]): The partition of the asset to load.
             resource_config (Optional[Any]): A dictionary of resource configurations to be passed
                 to the :py:class:`IOManager`.
 
         Returns:
             The contents of an asset as a Python object.
         """
-        asset_key = AssetKey.from_coerceable(asset_key)
+        asset_key = AssetKey.from_coercible(asset_key)
         resource_config = resource_config or {}
 
         if asset_key in self._assets_defs_by_key:
             assets_def = self._assets_defs_by_key[asset_key]
 
             resource_defs = merge_dicts(
                 {DEFAULT_IO_MANAGER_KEY: default_job_io_manager_with_fs_io_manager_schema},
```

### Comparing `dagster-1.3.3/dagster/_core/storage/base_storage.py` & `dagster-1.3.4/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.3.4/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/captured_log_manager.py` & `dagster-1.3.4/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.3.4/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/compute_log_manager.py` & `dagster-1.3.4/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/config.py` & `dagster-1.3.4/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/dagster_run.py` & `dagster-1.3.4/dagster/_core/storage/dagster_run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/db_io_manager.py` & `dagster-1.3.4/dagster/_core/storage/db_io_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,17 @@
                                 partition_expr=cast(str, partition_expr_str), partitions=partitions
                             )
                         )
                 elif isinstance(context.asset_partitions_def, TimeWindowPartitionsDefinition):
                     partition_dimensions.append(
                         TablePartitionDimension(
                             partition_expr=cast(str, partition_expr),
-                            partitions=context.asset_partitions_time_window,
+                            partitions=context.asset_partitions_time_window
+                            if context.asset_partition_keys
+                            else [],
                         )
                     )
                 else:
                     partition_dimensions.append(
                         TablePartitionDimension(
                             partition_expr=cast(str, partition_expr),
                             partitions=context.asset_partition_keys,
```

### Comparing `dagster-1.3.3/dagster/_core/storage/event_log/__init__.py` & `dagster-1.3.4/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/event_log/base.py` & `dagster-1.3.4/dagster/_core/storage/event_log/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,36 +151,40 @@
 
     def get_logs_for_run(
         self,
         run_id: str,
         cursor: Optional[Union[str, int]] = None,
         of_type: Optional[Union[DagsterEventType, Set[DagsterEventType]]] = None,
         limit: Optional[int] = None,
+        ascending: bool = True,
     ) -> Sequence["EventLogEntry"]:
         """Get all of the logs corresponding to a run.
 
         Args:
             run_id (str): The id of the run for which to fetch logs.
             cursor (Optional[Union[str, int]]): Cursor value to track paginated queries.  Legacy
                 support for integer offset cursors.
             of_type (Optional[DagsterEventType]): the dagster event type to filter the logs.
             limit (Optional[int]): Max number of records to return.
         """
         if isinstance(cursor, int):
             cursor = EventLogCursor.from_offset(cursor + 1).to_string()
-        records = self.get_records_for_run(run_id, cursor, of_type, limit).records
+        records = self.get_records_for_run(
+            run_id, cursor, of_type, limit, ascending=ascending
+        ).records
         return [record.event_log_entry for record in records]
 
     @abstractmethod
     def get_records_for_run(
         self,
         run_id: str,
         cursor: Optional[str] = None,
         of_type: Optional[Union[DagsterEventType, Set[DagsterEventType]]] = None,
         limit: Optional[int] = None,
+        ascending: bool = True,
     ) -> EventLogConnection:
         """Get all of the event log records corresponding to a run.
 
         Args:
             run_id (str): The id of the run for which to fetch logs.
             cursor (Optional[str]): Cursor value to track paginated queries.
             of_type (Optional[DagsterEventType]): the dagster event type to filter the logs.
```

### Comparing `dagster-1.3.3/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.3.4/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/event_log/migration.py` & `dagster-1.3.4/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.3.4/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import threading
 from typing import Callable, List, MutableMapping, NamedTuple, Optional
 
 import dagster._check as check
 from dagster._core.events.log import EventLogEntry
 from dagster._core.storage.event_log.base import EventLogCursor, EventLogStorage
 
-POLLING_CADENCE = 0.1  # 100 ms
+INIT_POLL_PERIOD = 0.250  # 250ms
+MAX_POLL_PERIOD = 16.0  # 16s
 
 
 class CallbackAfterCursor(NamedTuple):
     """Callback passed from Observer class in event polling.
 
     cursor (str): Only process EventLogEntrys after the given cursor
     callback (Callable[[EventLogEntry], None]): callback passed from Observer
@@ -78,15 +79,15 @@
             self._disposed = True
             with self._dict_lock:
                 for watcher_thread in self._run_id_to_watcher_dict.values():
                     if not watcher_thread.should_thread_exit.is_set():
                         watcher_thread.should_thread_exit.set()
                 for run_id in self._run_id_to_watcher_dict:
                     self._run_id_to_watcher_dict[run_id].join()
-                del self._run_id_to_watcher_dict
+                self._run_id_to_watcher_dict = {}
 
 
 class SqlPollingRunIdEventWatcherThread(threading.Thread):
     """subclass of Thread that watches a given run_id for new Events by polling every POLLING_CADENCE.
 
     Holds a list of callbacks (_callback_fn_list) each passed in by an `Observer`. Note that
         the callbacks have a cursor associated; this means that the callbacks should be
@@ -149,22 +150,24 @@
         """Polling function to update Observers with EventLogEntrys from Event Log DB.
         Wakes every POLLING_CADENCE &
             1. executes a SELECT query to get new EventLogEntrys
             2. fires each callback (taking into account the callback.cursor) on the new EventLogEntrys
         Uses max_index_so_far as a cursor in the DB to make sure that only new records are retrieved.
         """
         cursor = None
-        while not self._should_thread_exit.wait(POLLING_CADENCE):
+        wait_time = INIT_POLL_PERIOD
+        while not self._should_thread_exit.wait(wait_time):
             conn = self._event_log_storage.get_records_for_run(self._run_id, cursor=cursor)
-            cursor = conn.cursor if conn.cursor else cursor
+            cursor = conn.cursor
             for event_record in conn.records:
                 with self._callback_fn_list_lock:
                     for callback_with_cursor in self._callback_fn_list:
                         if (
                             callback_with_cursor.cursor is None
                             or EventLogCursor.parse(callback_with_cursor.cursor).storage_id()
                             < event_record.storage_id
                         ):
                             callback_with_cursor.callback(
                                 event_record.event_log_entry,
                                 str(EventLogCursor.from_storage_id(event_record.storage_id)),
                             )
+            wait_time = INIT_POLL_PERIOD if conn.records else min(wait_time * 2, MAX_POLL_PERIOD)
```

### Comparing `dagster-1.3.3/dagster/_core/storage/event_log/schema.py` & `dagster-1.3.4/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.3.4/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,14 +391,15 @@
 
     def get_records_for_run(
         self,
         run_id,
         cursor: Optional[str] = None,
         of_type: Optional[Union[DagsterEventType, Set[DagsterEventType]]] = None,
         limit: Optional[int] = None,
+        ascending: bool = True,
     ) -> EventLogConnection:
         """Get all of the logs corresponding to a run.
 
         Args:
             run_id (str): The id of the run for which to fetch logs.
             cursor (Optional[int]): Zero-indexed logs will be returned starting from cursor + 1,
                 i.e., if cursor is -1, all logs will be returned. (default: -1)
@@ -415,30 +416,37 @@
             if isinstance(of_type, DagsterEventType)
             else check.opt_set_param(of_type, "dagster_event_type", of_type=DagsterEventType)
         )
 
         query = (
             db.select([SqlEventLogStorageTable.c.id, SqlEventLogStorageTable.c.event])
             .where(SqlEventLogStorageTable.c.run_id == run_id)
-            .order_by(SqlEventLogStorageTable.c.id.asc())
+            .order_by(
+                SqlEventLogStorageTable.c.id.asc()
+                if ascending
+                else SqlEventLogStorageTable.c.id.desc()
+            )
         )
         if dagster_event_types:
             query = query.where(
                 SqlEventLogStorageTable.c.dagster_event_type.in_(
                     [dagster_event_type.value for dagster_event_type in dagster_event_types]
                 )
             )
 
         # adjust 0 based index cursor to SQL offset
         if cursor is not None:
             cursor_obj = EventLogCursor.parse(cursor)
             if cursor_obj.is_offset_cursor():
                 query = query.offset(cursor_obj.offset())
             elif cursor_obj.is_id_cursor():
-                query = query.where(SqlEventLogStorageTable.c.id > cursor_obj.storage_id())
+                if ascending:
+                    query = query.where(SqlEventLogStorageTable.c.id > cursor_obj.storage_id())
+                else:
+                    query = query.where(SqlEventLogStorageTable.c.id < cursor_obj.storage_id())
 
         if limit:
             query = query.limit(limit)
 
         with self.run_connection(run_id) as conn:
             results = conn.execute(query).fetchall()
```

### Comparing `dagster-1.3.3/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.3.4/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.3.4/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.3.4/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/file_manager.py` & `dagster-1.3.4/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/fs_io_manager.py` & `dagster-1.3.4/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/input_manager.py` & `dagster-1.3.4/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/io_manager.py` & `dagster-1.3.4/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/legacy_storage.py` & `dagster-1.3.4/dagster/_core/storage/legacy_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,16 +378,19 @@
 
     def get_logs_for_run(
         self,
         run_id: str,
         cursor: Optional[Union[str, int]] = None,
         of_type: Optional[Union["DagsterEventType", Set["DagsterEventType"]]] = None,
         limit: Optional[int] = None,
+        ascending: bool = True,
     ) -> Iterable["EventLogEntry"]:
-        return self._storage.event_log_storage.get_logs_for_run(run_id, cursor, of_type, limit)
+        return self._storage.event_log_storage.get_logs_for_run(
+            run_id, cursor, of_type, limit, ascending
+        )
 
     def get_stats_for_run(self, run_id: str) -> "DagsterRunStatsSnapshot":
         return self._storage.event_log_storage.get_stats_for_run(run_id)
 
     def get_step_stats_for_run(
         self, run_id: str, step_keys: Optional[Sequence[str]] = None
     ) -> Sequence["RunStepKeyStatsSnapshot"]:
@@ -528,16 +531,19 @@
 
     def get_records_for_run(
         self,
         run_id: str,
         cursor: Optional[str] = None,
         of_type: Optional[Union["DagsterEventType", Set["DagsterEventType"]]] = None,
         limit: Optional[int] = None,
+        ascending: bool = True,
     ) -> EventLogConnection:
-        return self._storage.event_log_storage.get_records_for_run(run_id, cursor, of_type, limit)
+        return self._storage.event_log_storage.get_records_for_run(
+            run_id, cursor, of_type, limit, ascending
+        )
 
 
 class LegacyScheduleStorage(ScheduleStorage, ConfigurableClass):
     def __init__(self, storage: DagsterStorage, inst_data: Optional[ConfigurableClassData] = None):
         self._storage = check.inst_param(storage, "storage", DagsterStorage)
         self._inst_data = check.opt_inst_param(inst_data, "inst_data", ConfigurableClassData)
         super().__init__()
```

### Comparing `dagster-1.3.3/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.3.4/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/mem_io_manager.py` & `dagster-1.3.4/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.3.4/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/migration/utils.py` & `dagster-1.3.4/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.3.4/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/output_manager.py` & `dagster-1.3.4/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/partition_status_cache.py` & `dagster-1.3.4/dagster/_core/storage/partition_status_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/root.py` & `dagster-1.3.4/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/root_input_manager.py` & `dagster-1.3.4/dagster/_core/storage/root_input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/runs/base.py` & `dagster-1.3.4/dagster/_core/storage/runs/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/runs/in_memory.py` & `dagster-1.3.4/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/runs/migration.py` & `dagster-1.3.4/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/runs/schema.py` & `dagster-1.3.4/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.3.4/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.3.4/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.3.4/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/schedules/base.py` & `dagster-1.3.4/dagster/_core/storage/schedules/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/schedules/migration.py` & `dagster-1.3.4/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/schedules/schema.py` & `dagster-1.3.4/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.3.4/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.3.4/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.3.4/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/sql.py` & `dagster-1.3.4/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/sqlite.py` & `dagster-1.3.4/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/sqlite_storage.py` & `dagster-1.3.4/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/tags.py` & `dagster-1.3.4/dagster/_core/storage/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/temp_file_manager.py` & `dagster-1.3.4/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/storage/upath_io_manager.py` & `dagster-1.3.4/dagster/_core/storage/upath_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/system_config/composite_descent.py` & `dagster-1.3.4/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/system_config/objects.py` & `dagster-1.3.4/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/telemetry.py` & `dagster-1.3.4/dagster/_core/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/telemetry_upload.py` & `dagster-1.3.4/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/test_utils.py` & `dagster-1.3.4/dagster/_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.3.4/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/types/config_schema.py` & `dagster-1.3.4/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/types/dagster_type.py` & `dagster-1.3.4/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/types/decorator.py` & `dagster-1.3.4/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/types/loadable_target_origin.py` & `dagster-1.3.4/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/types/primitive_mapping.py` & `dagster-1.3.4/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/types/python_dict.py` & `dagster-1.3.4/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/types/python_set.py` & `dagster-1.3.4/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/types/python_tuple.py` & `dagster-1.3.4/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/types/transform_typing.py` & `dagster-1.3.4/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/utility_ops.py` & `dagster-1.3.4/dagster/_core/utility_ops.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/utils.py` & `dagster-1.3.4/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/workspace/autodiscovery.py` & `dagster-1.3.4/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/workspace/config_schema.py` & `dagster-1.3.4/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/workspace/context.py` & `dagster-1.3.4/dagster/_core/workspace/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/workspace/load.py` & `dagster-1.3.4/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/workspace/load_target.py` & `dagster-1.3.4/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/workspace/permissions.py` & `dagster-1.3.4/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_core/workspace/workspace.py` & `dagster-1.3.4/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_daemon/__init__.py` & `dagster-1.3.4/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_daemon/asset_daemon.py` & `dagster-1.3.4/dagster/_daemon/asset_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.3.4/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.3.4/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_daemon/backfill.py` & `dagster-1.3.4/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_daemon/cli/__init__.py` & `dagster-1.3.4/dagster/_daemon/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,15 @@
     help="Run any daemons configured on the DagsterInstance.",
 )
 @click.option(
     "--code-server-log-level",
     help="Set the log level for any code servers spun up by the daemon.",
     show_default=True,
     default="warning",
-    type=click.Choice(
-        ["critical", "error", "warning", "info", "debug", "trace"], case_sensitive=False
-    ),
+    type=click.Choice(["critical", "error", "warning", "info", "debug"], case_sensitive=False),
 )
 @click.option(
     "--instance-ref",
     type=click.STRING,
     required=False,
     hidden=True,
 )
```

### Comparing `dagster-1.3.3/dagster/_daemon/controller.py` & `dagster-1.3.4/dagster/_daemon/controller.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_daemon/daemon.py` & `dagster-1.3.4/dagster/_daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_daemon/monitoring/monitoring_daemon.py` & `dagster-1.3.4/dagster/_daemon/monitoring/monitoring_daemon.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     IN_PROGRESS_RUN_STATUSES,
     DagsterRunStatus,
     RunRecord,
     RunsFilter,
 )
 from dagster._core.storage.tags import MAX_RUNTIME_SECONDS_TAG
 from dagster._core.workspace.context import IWorkspace, IWorkspaceProcessContext
-from dagster._utils import DebugCrashFlags
+from dagster._utils import DebugCrashFlags, datetime_as_float
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 
 RESUME_RUN_LOG_MESSAGE = "Launching a new run worker to resume run"
 
 
 def monitor_starting_run(
     instance: DagsterInstance, run_record: RunRecord, logger: logging.Logger
@@ -51,14 +51,58 @@
             msg = msg + f"\n{debug_info}"
 
         logger.info(msg)
 
         instance.report_run_failed(run, msg)
 
 
+def monitor_canceling_run(
+    instance: DagsterInstance, run_record: RunRecord, logger: logging.Logger
+) -> None:
+    run = run_record.dagster_run
+    check.invariant(run.status == DagsterRunStatus.CANCELING)
+
+    canceling_events = instance.event_log_storage.get_logs_for_run(
+        run.run_id,
+        of_type={DagsterEventType.RUN_CANCELING},
+        limit=1,
+        ascending=False,  # Event will likely be at the end, so start from the back
+    )
+
+    if not canceling_events:
+        raise Exception("Run in status CANCELING doesn't have a RUN_CANCELING event")
+
+    event = canceling_events[0]
+
+    event_timestamp = (
+        event.timestamp
+        if isinstance(event.timestamp, float)
+        else datetime_as_float(event.timestamp)
+    )
+
+    if time.time() - event_timestamp >= instance.run_monitoring_cancel_timeout_seconds:
+        msg = (
+            "Run timed out due to taking longer than"
+            f" {instance.run_monitoring_cancel_timeout_seconds} seconds to cancel."
+        )
+
+        debug_info = None
+        try:
+            debug_info = instance.run_launcher.get_run_worker_debug_info(run)
+        except Exception:
+            logger.exception("Failure fetching debug info for failed run worker")
+
+        if debug_info:
+            msg = msg + f"\n{debug_info}"
+
+        logger.info(msg)
+
+        instance.report_run_canceled(run, msg)
+
+
 def count_resume_run_attempts(instance: DagsterInstance, run_id: str) -> int:
     events = instance.all_logs(run_id, of_type=DagsterEventType.ENGINE_EVENT)
     return len([event for event in events if event.message == RESUME_RUN_LOG_MESSAGE])
 
 
 def monitor_started_run(
     instance: DagsterInstance,
@@ -121,32 +165,40 @@
     logger: logging.Logger,
     _debug_crash_flags: Optional[DebugCrashFlags] = None,
 ) -> Iterator[Optional[SerializableErrorInfo]]:
     instance = workspace_process_context.instance
 
     # TODO: consider limiting number of runs to fetch
     run_records = list(
-        instance.get_run_records(filters=RunsFilter(statuses=IN_PROGRESS_RUN_STATUSES))
+        instance.get_run_records(
+            filters=RunsFilter(statuses=IN_PROGRESS_RUN_STATUSES + [DagsterRunStatus.CANCELING])
+        )
     )
 
     if not run_records:
         return
 
     logger.info(f"Collected {len(run_records)} runs for monitoring")
     workspace = workspace_process_context.create_request_context()
     for run_record in run_records:
         try:
             logger.info(f"Checking run {run_record.dagster_run.run_id}")
 
-            if run_record.dagster_run.status == DagsterRunStatus.STARTING:
+            if (
+                instance.run_monitoring_start_timeout_seconds > 0
+                and run_record.dagster_run.status == DagsterRunStatus.STARTING
+            ):
                 monitor_starting_run(instance, run_record, logger)
             elif run_record.dagster_run.status == DagsterRunStatus.STARTED:
                 monitor_started_run(instance, workspace, run_record, logger)
-            elif run_record.dagster_run.status == DagsterRunStatus.CANCELING:
-                # TODO: implement canceling timeouts
+            elif (
+                instance.run_monitoring_cancel_timeout_seconds > 0
+                and run_record.dagster_run.status == DagsterRunStatus.CANCELING
+            ):
+                monitor_canceling_run(instance, run_record, logger)
                 pass
             else:
                 check.invariant(False, f"Unexpected run status: {run_record.dagster_run.status}")
         except Exception:
             error_info = serializable_error_info_from_exc_info(sys.exc_info())
             logger.error(
                 f"Hit error while monitoring run {run_record.dagster_run.run_id}: {str(error_info)}"
```

### Comparing `dagster-1.3.3/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.3.4/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_daemon/sensor.py` & `dagster-1.3.4/dagster/_daemon/sensor.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from dagster._core.definitions.utils import validate_tags
 from dagster._core.errors import DagsterError
 from dagster._core.host_representation.code_location import CodeLocation
 from dagster._core.host_representation.external import ExternalJob, ExternalSensor
 from dagster._core.host_representation.external_data import ExternalTargetData
 from dagster._core.instance import DagsterInstance
 from dagster._core.scheduler.instigation import (
+    DynamicPartitionsRequestResult,
     InstigatorState,
     InstigatorStatus,
     InstigatorTick,
     SensorInstigatorData,
     TickData,
     TickStatus,
 )
@@ -139,14 +140,21 @@
 
     def add_run_info(self, run_id: Optional[str] = None, run_key: Optional[str] = None) -> None:
         self._tick = self._tick.with_run_info(run_id, run_key)
 
     def add_log_info(self, log_key: Sequence[str]) -> None:
         self._tick = self._tick.with_log_key(log_key)
 
+    def add_dynamic_partitions_request_result(
+        self, dynamic_partitions_request_result: DynamicPartitionsRequestResult
+    ) -> None:
+        self._tick = self._tick.with_dynamic_partitions_request_result(
+            dynamic_partitions_request_result
+        )
+
     def set_should_update_cursor_on_failure(self, should_update_cursor_on_failure: bool) -> None:
         self._should_update_cursor_on_failure = should_update_cursor_on_failure
 
     def _write(self) -> None:
         self._instance.update_tick(self._tick)
 
         if self._tick.status not in FINISHED_TICK_STATES:
@@ -611,14 +619,23 @@
 
                 if existent_partitions:
                     context.logger.info(
                         "Skipping addition of partition keys for dynamic partitions definition"
                         f" '{request.partitions_def_name}' that already exist:"
                         f" {existent_partitions}"
                     )
+
+                context.add_dynamic_partitions_request_result(
+                    DynamicPartitionsRequestResult(
+                        request.partitions_def_name,
+                        added_partitions=nonexistent_partitions,
+                        deleted_partitions=None,
+                        skipped_partitions=existent_partitions,
+                    )
+                )
             elif isinstance(request, DeleteDynamicPartitionsRequest):
                 if existent_partitions:
                     # TODO add a bulk delete method to the instance
                     for partition in existent_partitions:
                         instance.delete_dynamic_partition(request.partitions_def_name, partition)
 
                     context.logger.info(
@@ -628,14 +645,23 @@
 
                 if nonexistent_partitions:
                     context.logger.info(
                         "Skipping deletion of partition keys for dynamic partitions definition"
                         f" '{request.partitions_def_name}' that do not exist:"
                         f" {nonexistent_partitions}"
                     )
+
+                context.add_dynamic_partitions_request_result(
+                    DynamicPartitionsRequestResult(
+                        request.partitions_def_name,
+                        added_partitions=None,
+                        deleted_partitions=existent_partitions,
+                        skipped_partitions=nonexistent_partitions,
+                    )
+                )
             else:
                 check.failed(f"Unexpected action {request.action} for dynamic partition request")
     if not sensor_runtime_data.run_requests:
         if sensor_runtime_data.dagster_run_reactions:
             for run_reaction in sensor_runtime_data.dagster_run_reactions:
                 origin_run_id = check.not_none(run_reaction.dagster_run).run_id
                 if run_reaction.error:
```

### Comparing `dagster-1.3.3/dagster/_daemon/types.py` & `dagster-1.3.4/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_daemon/workspace.py` & `dagster-1.3.4/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_generate/download.py` & `dagster-1.3.4/dagster/_generate/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "tutorial_notebook_assets",
     "deploy_docker",
     "deploy_ecs",
     "deploy_k8s",
     "development_to_production",
     "feature_graph_backed_assets",
     "project_fully_featured",
+    "project_pypi_github",
     "with_airflow",
     "with_great_expectations",
     "with_pyspark",
     "with_pyspark_emr",
     "with_wandb",
 ]
```

### Comparing `dagster-1.3.3/dagster/_generate/generate.py` & `dagster-1.3.4/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.3.4/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.3.4/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # @generated
 
 # This file was generated by running `python -m dagster._grpc.compile`
 # Do not edit this file directly, and do not attempt to recompile it using
 # grpc_tools.protoc directly, as several changes must be made to the raw output
 
-
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from . import api_pb2 as api__pb2
```

### Comparing `dagster-1.3.3/dagster/_grpc/__init__.py` & `dagster-1.3.4/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_grpc/client.py` & `dagster-1.3.4/dagster/_grpc/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,48 +183,48 @@
         except Exception as e:
             self._raise_grpc_exception(
                 e, timeout=timeout, custom_timeout_message=custom_timeout_message
             )
 
     def ping(self, echo: str):
         check.str_param(echo, "echo")
-        res = self._query("Ping", api_pb2.PingRequest, echo=echo)  # type: ignore
+        res = self._query("Ping", api_pb2.PingRequest, echo=echo)
         return res.echo
 
     def heartbeat(self, echo: str = ""):
         check.str_param(echo, "echo")
-        res = self._query("Heartbeat", api_pb2.PingRequest, echo=echo)  # type: ignore
+        res = self._query("Heartbeat", api_pb2.PingRequest, echo=echo)
         return res.echo
 
     def streaming_ping(self, sequence_length: int, echo: str):
         check.int_param(sequence_length, "sequence_length")
         check.str_param(echo, "echo")
 
         for res in self._streaming_query(
             "StreamingPing",
-            api_pb2.StreamingPingRequest,  # type: ignore
+            api_pb2.StreamingPingRequest,
             sequence_length=sequence_length,
             echo=echo,
         ):
             yield {
                 "sequence_number": res.sequence_number,
                 "echo": res.echo,
             }
 
     def get_server_id(self, timeout: int = DEFAULT_GRPC_TIMEOUT) -> str:
-        res = self._query("GetServerId", api_pb2.Empty, timeout=timeout)  # type: ignore
+        res = self._query("GetServerId", api_pb2.Empty, timeout=timeout)
         return res.server_id
 
     def execution_plan_snapshot(self, execution_plan_snapshot_args: ExecutionPlanSnapshotArgs):
         check.inst_param(
             execution_plan_snapshot_args, "execution_plan_snapshot_args", ExecutionPlanSnapshotArgs
         )
         res = self._query(
             "ExecutionPlanSnapshot",
-            api_pb2.ExecutionPlanSnapshotRequest,  # type: ignore
+            api_pb2.ExecutionPlanSnapshotRequest,
             serialized_execution_plan_snapshot_args=serialize_value(execution_plan_snapshot_args),
         )
         return res.serialized_execution_plan_snapshot
 
     def list_repositories(self):
         res = self._query("ListRepositories", api_pb2.ListRepositoriesRequest)
         return res.serialized_list_repositories_response_or_error
@@ -305,15 +305,15 @@
             external_repository_origin,
             "external_repository_origin",
             ExternalRepositoryOrigin,
         )
 
         res = self._query(
             "ExternalRepository",
-            api_pb2.ExternalRepositoryRequest,  # type: ignore
+            api_pb2.ExternalRepositoryRequest,
             # rename this param name
             serialized_repository_python_origin=serialize_value(external_repository_origin),
             defer_snapshots=defer_snapshots,
         )
 
         return res.serialized_external_repository_data
 
@@ -326,27 +326,27 @@
             external_repository_origin,
             "external_repository_origin",
             ExternalRepositoryOrigin,
         )
 
         return self._query(
             "ExternalJob",
-            api_pb2.ExternalJobRequest,  # type: ignore
+            api_pb2.ExternalJobRequest,
             serialized_repository_origin=serialize_value(external_repository_origin),
             job_name=job_name,
         )
 
     def streaming_external_repository(
         self,
         external_repository_origin: ExternalRepositoryOrigin,
         defer_snapshots: bool = False,
     ):
         for res in self._streaming_query(
             "StreamingExternalRepository",
-            api_pb2.ExternalRepositoryRequest,  # type: ignore
+            api_pb2.ExternalRepositoryRequest,
             # Rename parameter
             serialized_repository_python_origin=serialize_value(external_repository_origin),
             defer_snapshots=defer_snapshots,
         ):
             yield {
                 "sequence_number": res.sequence_number,
                 "serialized_external_repository_chunk": res.serialized_external_repository_chunk,
@@ -397,15 +397,15 @@
 
         return "".join([chunk.serialized_chunk for chunk in chunks])
 
     def external_notebook_data(self, notebook_path: str):
         check.str_param(notebook_path, "notebook_path")
         res = self._query(
             "ExternalNotebookData",
-            api_pb2.ExternalNotebookDataRequest,  # type: ignore
+            api_pb2.ExternalNotebookDataRequest,
             notebook_path=notebook_path,
         )
         return res.content
 
     def shutdown_server(self, timeout=15):
         res = self._query("ShutdownServer", api_pb2.Empty, timeout=timeout)
         return res.serialized_shutdown_server_result
@@ -434,29 +434,29 @@
             can_cancel_execution_request,
             "can_cancel_execution_request",
             CanCancelExecutionRequest,
         )
 
         res = self._query(
             "CanCancelExecution",
-            api_pb2.CanCancelExecutionRequest,  # type: ignore
+            api_pb2.CanCancelExecutionRequest,
             timeout=timeout,
             serialized_can_cancel_execution_request=serialize_value(can_cancel_execution_request),
         )
 
         return res.serialized_can_cancel_execution_result
 
     def start_run(self, execute_run_args: ExecuteExternalJobArgs):
         check.inst_param(execute_run_args, "execute_run_args", ExecuteExternalJobArgs)
 
-        with DagsterInstance.from_ref(execute_run_args.instance_ref) as instance:  # type: ignore  # (possible none)
+        with DagsterInstance.from_ref(execute_run_args.instance_ref) as instance:  # type: ignore # (possible none)
             try:
                 res = self._query(
                     "StartRun",
-                    api_pb2.StartRunRequest,  # type: ignore
+                    api_pb2.StartRunRequest,
                     serialized_execute_run_args=serialize_value(execute_run_args),
                 )
                 return res.serialized_start_run_result
 
             except Exception:
                 dagster_run = instance.get_run_by_id(execute_run_args.run_id)
                 instance.report_engine_event(
```

### Comparing `dagster-1.3.3/dagster/_grpc/compile.py` & `dagster-1.3.4/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_grpc/impl.py` & `dagster-1.3.4/dagster/_grpc/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_grpc/protos/api.proto` & `dagster-1.3.4/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_grpc/server.py` & `dagster-1.3.4/dagster/_grpc/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -362,31 +362,31 @@
         loaded_repos = check.not_none(self._loaded_repositories)
         if external_repo_origin.repository_name not in loaded_repos.definitions_by_name:
             raise Exception(
                 f'Could not find a repository called "{external_repo_origin.repository_name}"'
             )
         return loaded_repos.definitions_by_name[external_repo_origin.repository_name]
 
-    def Ping(self, request, _context) -> api_pb2.PingReply:  # type: ignore
+    def Ping(self, request, _context) -> api_pb2.PingReply:
         echo = request.echo
-        return api_pb2.PingReply(echo=echo)  # type: ignore
+        return api_pb2.PingReply(echo=echo)
 
-    def StreamingPing(self, request, _context) -> Iterator[api_pb2.StreamingPingEvent]:  # type: ignore
+    def StreamingPing(self, request, _context) -> Iterator[api_pb2.StreamingPingEvent]:
         sequence_length = request.sequence_length
         echo = request.echo
         for sequence_number in range(sequence_length):
-            yield api_pb2.StreamingPingEvent(sequence_number=sequence_number, echo=echo)  # type: ignore
+            yield api_pb2.StreamingPingEvent(sequence_number=sequence_number, echo=echo)
 
-    def Heartbeat(self, request, _context) -> api_pb2.PingReply:  # type: ignore
+    def Heartbeat(self, request, _context) -> api_pb2.PingReply:
         self.__last_heartbeat_time = time.time()
         echo = request.echo
-        return api_pb2.PingReply(echo=echo)  # type: ignore
+        return api_pb2.PingReply(echo=echo)
 
-    def GetServerId(self, _request, _context) -> api_pb2.GetServerIdReply:  # type:ignore
-        return api_pb2.GetServerIdReply(server_id=self._server_id)  # type: ignore
+    def GetServerId(self, _request, _context) -> api_pb2.GetServerIdReply:
+        return api_pb2.GetServerIdReply(server_id=self._server_id)
 
     def ExecutionPlanSnapshot(self, request, _context):
         execution_plan_args = deserialize_value(
             request.serialized_execution_plan_snapshot_args,
             ExecutionPlanSnapshotArgs,
         )
 
@@ -395,17 +395,17 @@
             execution_plan_args.job_origin.job_name,
             execution_plan_args,
         )
         return api_pb2.ExecutionPlanSnapshotReply(
             serialized_execution_plan_snapshot=serialize_value(execution_plan_snapshot_or_error)
         )
 
-    def ListRepositories(self, request, _context) -> api_pb2.ListRepositoriesReply:  # type: ignore
+    def ListRepositories(self, request, _context) -> api_pb2.ListRepositoriesReply:
         if self._serializable_load_error:
-            return api_pb2.ListRepositoriesReply(  # type: ignore
+            return api_pb2.ListRepositoriesReply(
                 serialized_list_repositories_response_or_error=serialize_value(
                     self._serializable_load_error
                 )
             )
         try:
             loaded_repositories = check.not_none(self._loaded_repositories)
             serialized_response = serialize_value(
@@ -422,19 +422,19 @@
                 )
             )
         except Exception:
             serialized_response = serialize_value(
                 serializable_error_info_from_exc_info(sys.exc_info())
             )
 
-        return api_pb2.ListRepositoriesReply(  # type: ignore
+        return api_pb2.ListRepositoriesReply(
             serialized_list_repositories_response_or_error=serialized_response
         )
 
-    def ExternalPartitionNames(self, request, _context) -> api_pb2.ExternalPartitionNamesReply:  # type: ignore
+    def ExternalPartitionNames(self, request, _context) -> api_pb2.ExternalPartitionNamesReply:
         try:
             partition_names_args = deserialize_value(
                 request.serialized_partition_names_args,
                 PartitionNamesArgs,
             )
             serialized_response = serialize_value(
                 get_partition_names(
@@ -445,22 +445,22 @@
         except Exception:
             serialized_response = serialize_value(
                 ExternalPartitionExecutionErrorData(
                     serializable_error_info_from_exc_info(sys.exc_info())
                 )
             )
 
-        return api_pb2.ExternalPartitionNamesReply(  # type: ignore
+        return api_pb2.ExternalPartitionNamesReply(
             serialized_external_partition_names_or_external_partition_execution_error=serialized_response
         )
 
-    def ExternalNotebookData(self, request, _context) -> api_pb2.ExternalNotebookDataReply:  # type: ignore
+    def ExternalNotebookData(self, request, _context) -> api_pb2.ExternalNotebookDataReply:
         notebook_path = request.notebook_path
         check.str_param(notebook_path, "notebook_path")
-        return api_pb2.ExternalNotebookDataReply(content=get_notebook_data(notebook_path))  # type: ignore
+        return api_pb2.ExternalNotebookDataReply(content=get_notebook_data(notebook_path))
 
     def ExternalPartitionSetExecutionParams(self, request, _context):
         try:
             args = deserialize_value(
                 request.serialized_partition_set_execution_param_args,
                 PartitionSetExecutionParamArgs,
             )
@@ -505,15 +505,15 @@
                 )
             )
 
         return api_pb2.ExternalPartitionConfigReply(
             serialized_external_partition_config_or_external_partition_execution_error=serialized_data
         )
 
-    def ExternalPartitionTags(self, request, _context) -> api_pb2.ExternalPartitionTagsReply:  # type: ignore
+    def ExternalPartitionTags(self, request, _context) -> api_pb2.ExternalPartitionTagsReply:
         try:
             partition_args = deserialize_value(request.serialized_partition_args, PartitionArgs)
 
             instance_ref = (
                 partition_args.instance_ref if partition_args.instance_ref else self._instance_ref
             )
 
@@ -528,21 +528,21 @@
         except Exception:
             serialized_data = serialize_value(
                 ExternalPartitionExecutionErrorData(
                     serializable_error_info_from_exc_info(sys.exc_info())
                 )
             )
 
-        return api_pb2.ExternalPartitionTagsReply(  # type: ignore
+        return api_pb2.ExternalPartitionTagsReply(
             serialized_external_partition_tags_or_external_partition_execution_error=serialized_data
         )
 
     def ExternalPipelineSubsetSnapshot(
         self, request: Any, _context
-    ) -> api_pb2.ExternalPipelineSubsetSnapshotReply:  # type: ignore
+    ) -> api_pb2.ExternalPipelineSubsetSnapshotReply:
         try:
             job_subset_snapshot_args = deserialize_value(
                 request.serialized_pipeline_subset_snapshot_args,
                 JobSubsetSnapshotArgs,
             )
             serialized_external_pipeline_subset_result = serialize_value(
                 get_external_pipeline_subset_result(
@@ -557,15 +557,15 @@
         except Exception:
             serialized_external_pipeline_subset_result = serialize_value(
                 ExternalJobSubsetResult(
                     success=False, error=serializable_error_info_from_exc_info(sys.exc_info())
                 )
             )
 
-        return api_pb2.ExternalPipelineSubsetSnapshotReply(  # type: ignore
+        return api_pb2.ExternalPipelineSubsetSnapshotReply(
             serialized_external_pipeline_subset_result=serialized_external_pipeline_subset_result
         )
 
     def _get_serialized_external_repository_data(self, request):
         try:
             repository_origin = deserialize_value(
                 request.serialized_repository_python_origin,
@@ -585,26 +585,26 @@
 
     def ExternalRepository(self, request, _context):
         serialized_external_repository_data = self._get_serialized_external_repository_data(request)
         return api_pb2.ExternalRepositoryReply(
             serialized_external_repository_data=serialized_external_repository_data,
         )
 
-    def ExternalJob(self, request, _context) -> api_pb2.ExternalJobReply:  # type: ignore
+    def ExternalJob(self, request, _context) -> api_pb2.ExternalJobReply:
         try:
             repository_origin = deserialize_value(
                 request.serialized_repository_origin,
                 ExternalRepositoryOrigin,
             )
 
             job_def = self._get_repo_for_origin(repository_origin).get_job(request.job_name)
             ser_job_data = serialize_value(external_job_data_from_def(job_def))
-            return api_pb2.ExternalJobReply(serialized_job_data=ser_job_data)  # type: ignore
+            return api_pb2.ExternalJobReply(serialized_job_data=ser_job_data)
         except Exception:
-            return api_pb2.ExternalJobReply(  # type: ignore
+            return api_pb2.ExternalJobReply(
                 serialized_error=serialize_value(
                     serializable_error_info_from_exc_info(sys.exc_info())
                 )
             )
 
     def StreamingExternalRepository(self, request, _context):
         serialized_external_repository_data = self._get_serialized_external_repository_data(request)
@@ -687,24 +687,24 @@
                 ExternalSensorExecutionErrorData(
                     serializable_error_info_from_exc_info(sys.exc_info())
                 )
             )
 
         yield from self._split_serialized_data_into_chunk_events(serialized_sensor_data)
 
-    def ShutdownServer(self, request, _context) -> api_pb2.ShutdownServerReply:  # type: ignore
+    def ShutdownServer(self, request, _context) -> api_pb2.ShutdownServerReply:
         try:
             self._shutdown_once_executions_finish_event.set()
-            return api_pb2.ShutdownServerReply(  # type: ignore
+            return api_pb2.ShutdownServerReply(
                 serialized_shutdown_server_result=serialize_value(
                     ShutdownServerResult(success=True, serializable_error_info=None)
                 )
             )
         except:
-            return api_pb2.ShutdownServerReply(  # type: ignore
+            return api_pb2.ShutdownServerReply(
                 serialized_shutdown_server_result=serialize_value(
                     ShutdownServerResult(
                         success=False,
                         serializable_error_info=serializable_error_info_from_exc_info(
                             sys.exc_info()
                         ),
                     )
@@ -735,34 +735,34 @@
                     success=success,
                     message=message,
                     serializable_error_info=serializable_error_info,
                 )
             )
         )
 
-    def CanCancelExecution(self, request, _context) -> api_pb2.CanCancelExecutionReply:  # type: ignore
+    def CanCancelExecution(self, request, _context) -> api_pb2.CanCancelExecutionReply:
         can_cancel_execution_request = deserialize_value(
             request.serialized_can_cancel_execution_request,
             CanCancelExecutionRequest,
         )
         with self._execution_lock:
             run_id = can_cancel_execution_request.run_id
             can_cancel = (
                 run_id in self._executions and not self._termination_events[run_id].is_set()
             )
 
-        return api_pb2.CanCancelExecutionReply(  # type: ignore
+        return api_pb2.CanCancelExecutionReply(
             serialized_can_cancel_execution_result=serialize_value(
                 CanCancelExecutionResult(can_cancel=can_cancel)
             )
         )
 
-    def StartRun(self, request, _context) -> api_pb2.StartRunReply:  # type: ignore
+    def StartRun(self, request, _context) -> api_pb2.StartRunReply:
         if self._shutdown_once_executions_finish_event.is_set():
-            return api_pb2.StartRunReply(  # type: ignore
+            return api_pb2.StartRunReply(
                 serialized_start_run_result=serialize_value(
                     StartRunResult(
                         success=False,
                         message="Tried to start a run on a server after telling it to shut down",
                         serializable_error_info=None,
                     )
                 )
@@ -780,15 +780,15 @@
                 execute_external_job_args.job_origin.external_repository_origin.repository_name
             ]
             recon_job = recon_repo.get_reconstructable_job(
                 execute_external_job_args.job_origin.job_name
             )
 
         except:
-            return api_pb2.StartRunReply(  # type: ignore
+            return api_pb2.StartRunReply(
                 serialized_start_run_result=serialize_value(
                     StartRunResult(
                         success=False,
                         message=None,
                         serializable_error_info=serializable_error_info_from_exc_info(
                             sys.exc_info()
                         ),
@@ -858,15 +858,15 @@
 
         # Ensure that if the run failed, we remove it from the executions map before
         # returning so that CanCancel will never return True
         if not success:
             with self._execution_lock:
                 self._clear_run(run_id)
 
-        return api_pb2.StartRunReply(  # type: ignore
+        return api_pb2.StartRunReply(
             serialized_start_run_result=serialize_value(
                 StartRunResult(
                     success=success,
                     message=message,
                     serializable_error_info=serializable_error_info,
                 )
             )
@@ -877,17 +877,17 @@
             serialized_current_image=serialize_value(
                 GetCurrentImageResult(
                     current_image=self._container_image, serializable_error_info=None
                 )
             )
         )
 
-    def GetCurrentRuns(self, request, context) -> api_pb2.GetCurrentRunsReply:  # type: ignore
+    def GetCurrentRuns(self, request, context) -> api_pb2.GetCurrentRunsReply:
         with self._execution_lock:
-            return api_pb2.GetCurrentRunsReply(  # type: ignore
+            return api_pb2.GetCurrentRunsReply(
                 serialized_current_runs=serialize_value(
                     GetCurrentRunsResult(
                         current_runs=list(self._executions.keys()), serializable_error_info=None
                     )
                 )
             )
```

### Comparing `dagster-1.3.3/dagster/_grpc/server_watcher.py` & `dagster-1.3.4/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_grpc/types.py` & `dagster-1.3.4/dagster/_grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_grpc/utils.py` & `dagster-1.3.4/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_loggers/__init__.py` & `dagster-1.3.4/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_module_alias_map.py` & `dagster-1.3.4/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_scheduler/scheduler.py` & `dagster-1.3.4/dagster/_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_scheduler/stale.py` & `dagster-1.3.4/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_serdes/__init__.py` & `dagster-1.3.4/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_serdes/config_class.py` & `dagster-1.3.4/dagster/_serdes/config_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_serdes/ipc.py` & `dagster-1.3.4/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_serdes/serdes.py` & `dagster-1.3.4/dagster/_serdes/serdes.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_serdes/utils.py` & `dagster-1.3.4/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_seven/__init__.py` & `dagster-1.3.4/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_seven/abc.py` & `dagster-1.3.4/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_seven/compat/pendulum.py` & `dagster-1.3.4/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/__init__.py` & `dagster-1.3.4/dagster/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/alert.py` & `dagster-1.3.4/dagster/_utils/alert.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/backcompat.py` & `dagster-1.3.4/dagster/_utils/backcompat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/backoff.py` & `dagster-1.3.4/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/cached_method.py` & `dagster-1.3.4/dagster/_utils/cached_method.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/caching_instance_queryer.py` & `dagster-1.3.4/dagster/_utils/caching_instance_queryer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from collections import defaultdict
+from datetime import datetime
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Dict,
     Iterable,
     Mapping,
     Optional,
     Sequence,
     Union,
     cast,
 )
 
+import pendulum
+
 from dagster._core.definitions.asset_graph import AssetGraph
 from dagster._core.definitions.data_version import (
     DataVersion,
     extract_data_version_from_entry,
 )
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
 from dagster._core.events import DagsterEventType
@@ -36,28 +39,30 @@
     instance which will attempt to limit redundant expensive calls. Intended for use within the
     scope of a single "request" (e.g. GQL request, sensor tick).
 
     Args:
         instance (DagsterInstance): The instance to query.
     """
 
-    def __init__(self, instance: DagsterInstance):
+    def __init__(self, instance: DagsterInstance, evaluation_time: Optional[datetime] = None):
         self._instance = instance
 
         self._asset_record_cache: Dict[AssetKey, Optional[AssetRecord]] = {}
         self._latest_materialization_record_cache: Dict[
             AssetKeyPartitionKey, Optional[EventLogRecord]
         ] = {}
 
         self._asset_partition_count_cache: Dict[
             Optional[int], Dict[AssetKey, Mapping[str, int]]
         ] = defaultdict(dict)
 
         self._dynamic_partitions_cache: Dict[str, Sequence[str]] = {}
 
+        self._evaluation_time = evaluation_time if evaluation_time else pendulum.now("UTC")
+
     @property
     def instance(self) -> DagsterInstance:
         return self._instance
 
     ####################
     # QUERY BATCHING
     ####################
@@ -568,14 +573,15 @@
             return True
 
         if not self.materialization_exists(asset_partition):
             return False
 
         for parent in asset_graph.get_parents_partitions(
             self,
+            self._evaluation_time,
             asset_partition.asset_key,
             asset_partition.partition_key,
         ):
             if asset_graph.is_source(parent.asset_key):
                 if asset_graph.is_observable(
                     parent.asset_key
                 ) and self._new_version_of_source_exists_after_asset_partition(
@@ -587,7 +593,11 @@
                     continue
             elif self._materialization_of_a_exists_after_b(a=parent, b=asset_partition):
                 return False
             elif not self.is_reconciled(asset_partition=parent, asset_graph=asset_graph):
                 return False
 
         return True
+
+    @property
+    def evaluation_time(self) -> datetime:
+        return self._evaluation_time
```

### Comparing `dagster-1.3.3/dagster/_utils/dagster_type.py` & `dagster-1.3.4/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/error.py` & `dagster-1.3.4/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/external.py` & `dagster-1.3.4/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/forked_pdb.py` & `dagster-1.3.4/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/hosted_user_process.py` & `dagster-1.3.4/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/indenting_printer.py` & `dagster-1.3.4/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/interrupts.py` & `dagster-1.3.4/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/log.py` & `dagster-1.3.4/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/merger.py` & `dagster-1.3.4/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/net.py` & `dagster-1.3.4/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/schedules.py` & `dagster-1.3.4/dagster/_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/tags.py` & `dagster-1.3.4/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/temp_file.py` & `dagster-1.3.4/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/test/__init__.py` & `dagster-1.3.4/dagster/_utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/test/mysql_instance.py` & `dagster-1.3.4/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/test/postgres_instance.py` & `dagster-1.3.4/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/test/schedule_storage.py` & `dagster-1.3.4/dagster/_utils/test/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/timing.py` & `dagster-1.3.4/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/typing_api.py` & `dagster-1.3.4/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster/_utils/yaml_utils.py` & `dagster-1.3.4/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/dagster.egg-info/PKG-INFO` & `dagster-1.3.4/dagster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.3.3
+Version: 1.3.4
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.3.3/dagster.egg-info/SOURCES.txt` & `dagster-1.3.4/dagster.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 dagster/_core/definitions/multi_dimensional_partitions.py
 dagster/_core/definitions/no_step_launcher.py
 dagster/_core/definitions/node_container.py
 dagster/_core/definitions/node_definition.py
 dagster/_core/definitions/observe.py
 dagster/_core/definitions/op_definition.py
 dagster/_core/definitions/op_invocation.py
+dagster/_core/definitions/op_selection.py
 dagster/_core/definitions/output.py
 dagster/_core/definitions/partition.py
 dagster/_core/definitions/partition_key_range.py
 dagster/_core/definitions/partition_mapping.py
 dagster/_core/definitions/partitioned_schedule.py
 dagster/_core/definitions/policy.py
 dagster/_core/definitions/reconstruct.py
@@ -186,23 +187,22 @@
 dagster/_core/execution/backfill.py
 dagster/_core/execution/build_resources.py
 dagster/_core/execution/bulk_actions.py
 dagster/_core/execution/compute_logs.py
 dagster/_core/execution/context_creation_job.py
 dagster/_core/execution/execute_in_process.py
 dagster/_core/execution/execute_in_process_result.py
-dagster/_core/execution/execute_job_result.py
 dagster/_core/execution/execution_result.py
 dagster/_core/execution/host_mode.py
 dagster/_core/execution/job_backfill.py
+dagster/_core/execution/job_execution_result.py
 dagster/_core/execution/memoization.py
 dagster/_core/execution/poll_compute_logs.py
 dagster/_core/execution/resolve_versions.py
 dagster/_core/execution/resources_init.py
-dagster/_core/execution/results.py
 dagster/_core/execution/retries.py
 dagster/_core/execution/run_cancellation_thread.py
 dagster/_core/execution/stats.py
 dagster/_core/execution/tags.py
 dagster/_core/execution/validate_run_config.py
 dagster/_core/execution/watch_orphans.py
 dagster/_core/execution/with_resources.py
@@ -277,14 +277,15 @@
 dagster/_core/snap/config_types.py
 dagster/_core/snap/dagster_types.py
 dagster/_core/snap/dep_snapshot.py
 dagster/_core/snap/execution_plan_snapshot.py
 dagster/_core/snap/job_snapshot.py
 dagster/_core/snap/mode.py
 dagster/_core/snap/node.py
+dagster/_core/snap/snap_to_yaml.py
 dagster/_core/storage/DEVELOPING.md
 dagster/_core/storage/__init__.py
 dagster/_core/storage/asset_value_loader.py
 dagster/_core/storage/base_storage.py
 dagster/_core/storage/captured_log_manager.py
 dagster/_core/storage/cloud_storage_compute_log_manager.py
 dagster/_core/storage/compute_log_manager.py
@@ -385,14 +386,15 @@
 dagster/_core/storage/alembic/versions/031_add_kvs_table.py
 dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
 dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
 dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
 dagster/_core/storage/alembic/versions/035_add_run_job_index.py
 dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
 dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
 dagster/_core/storage/alembic/versions/__init__.py
 dagster/_core/storage/branching/__init__.py
 dagster/_core/storage/branching/branching_io_manager.py
 dagster/_core/storage/event_log/__init__.py
 dagster/_core/storage/event_log/base.py
 dagster/_core/storage/event_log/in_memory.py
 dagster/_core/storage/event_log/migration.py
```

### Comparing `dagster-1.3.3/dagster.egg-info/requires.txt` & `dagster-1.3.4/dagster.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dagster-1.3.3/setup.py` & `dagster-1.3.4/setup.py`

 * *Files identical despite different names*

