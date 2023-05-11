# Comparing `tmp/qwak_sdk-0.2.29rc0.tar.gz` & `tmp/qwak_sdk-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_sdk-0.2.29rc0.tar", max compression
+gzip compressed data, was "qwak_sdk-0.5.3.tar", max compression
```

## Comparing `qwak_sdk-0.2.29rc0.tar` & `qwak_sdk-0.5.3.tar`

### file list

```diff
@@ -1,302 +1,302 @@
--rw-r--r--   0        0        0      183 2023-04-27 07:15:38.098821 qwak_sdk-0.2.29rc0/README.md
--rw-r--r--   0        0        0     2617 2023-04-27 07:16:24.091230 qwak_sdk-0.2.29rc0/pyproject.toml
--rw-r--r--   0        0        0      139 2023-04-27 07:16:24.087230 qwak_sdk-0.2.29rc0/qwak_sdk/__init__.py
--rw-r--r--   0        0        0     2039 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/cli.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/admin/__init__.py
--rw-r--r--   0        0        0      327 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/admin/admin_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/admin/apikeys/__init__.py
--rw-r--r--   0        0        0      477 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/admin/apikeys/api_keys_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/admin/apikeys/generate/__init__.py
--rw-r--r--   0        0        0      677 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/admin/apikeys/generate/_logic.py
--rw-r--r--   0        0        0     1403 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/admin/apikeys/generate/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/admin/apikeys/revoke/__init__.py
--rw-r--r--   0        0        0      796 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/admin/apikeys/revoke/_logic.py
--rw-r--r--   0        0        0      952 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/admin/apikeys/revoke/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/audience/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/audience/_logic/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/audience/_logic/config/__init__.py
--rw-r--r--   0        0        0      367 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/audience/_logic/config/config_base.py
--rw-r--r--   0        0        0      885 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/audience/_logic/config/parser.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/audience/_logic/config/v1/__init__.py
--rw-r--r--   0        0        0      886 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py
--rw-r--r--   0        0        0     1626 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py
--rw-r--r--   0        0        0      817 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py
--rw-r--r--   0        0        0      340 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/audience/_logic/config/v1/route_config.py
--rw-r--r--   0        0        0      277 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/audience/_logic/config/v1/spec.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/auto_scalling/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/auto_scalling/_logic/__init__.py
--rw-r--r--   0        0        0       49 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/auto_scalling/_logic/config/__init__.py
--rw-r--r--   0        0        0     3098 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/auto_scalling/_logic/config/config.py
--rw-r--r--   0        0        0      646 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/auto_scalling/_logic/config/parser.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/auto_scalling/attach/__init__.py
--rw-r--r--   0        0        0     1359 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/auto_scalling/attach/_logic.py
--rw-r--r--   0        0        0      949 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/auto_scalling/attach/ui.py
--rw-r--r--   0        0        0      277 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/auto_scalling/autoscaling_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/__init__.py
--rw-r--r--   0        0        0      857 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/automations_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/delete/__init__.py
--rw-r--r--   0        0        0      235 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/delete/_logic.py
--rw-r--r--   0        0        0      604 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/delete/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/executions/__init__.py
--rw-r--r--   0        0        0      346 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/executions/executions_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/executions/list/__init__.py
--rw-r--r--   0        0        0      330 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/executions/list/_logic.py
--rw-r--r--   0        0        0      669 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/executions/list/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/list/__init__.py
--rw-r--r--   0        0        0      252 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/list/_logic.py
--rw-r--r--   0        0        0      546 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/list/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/register/__init__.py
--rw-r--r--   0        0        0     1624 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/register/_logic.py
--rw-r--r--   0        0        0     1331 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/register/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/delete/__init__.py
--rw-r--r--   0        0        0     1716 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/delete/_logic.py
--rw-r--r--   0        0        0     1039 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/delete/ui.py
--rw-r--r--   0        0        0     1002 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/feature_store_command_group.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/list/__init__.py
--rw-r--r--   0        0        0     4145 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/list/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/pause/__init__.py
--rw-r--r--   0        0        0      695 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/pause/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/register/__init__.py
--rw-r--r--   0        0        0    10893 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/register/_logic.py
--rw-r--r--   0        0        0     2822 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/register/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/resume/__init__.py
--rw-r--r--   0        0        0      700 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/resume/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/trigger/__init__.py
--rw-r--r--   0        0        0     1015 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/trigger/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/_logic/__init__.py
--rw-r--r--   0        0        0     2050 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/_logic/variations.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/__init__.py
--rw-r--r--   0        0        0     2005 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/build_steps.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/client_logs/__init__.py
--rw-r--r--   0        0        0     6129 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py
--rw-r--r--   0        0        0     4383 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py
--rw-r--r--   0        0        0     2908 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/client_logs/logger.py
--rw-r--r--   0        0        0     1369 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/client_logs/messages.py
--rw-r--r--   0        0        0     1435 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py
--rw-r--r--   0        0        0      359 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/client_logs/spinner.py
--rw-r--r--   0        0        0      975 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py
--rw-r--r--   0        0        0      311 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/client_logs/utils.py
--rw-r--r--   0        0        0     9876 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/config/config_v1.py
--rw-r--r--   0        0        0      131 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/constant/host_resource.py
--rw-r--r--   0        0        0      881 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/constant/step_description.py
--rw-r--r--   0        0        0       73 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/constant/temp_dir.py
--rw-r--r--   0        0        0      189 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/constant/upload_tag.py
--rw-r--r--   0        0        0     1872 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/context.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/interface/__init__.py
--rw-r--r--   0        0        0      568 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py
--rw-r--r--   0        0        0      745 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/__init__.py
--rw-r--r--   0        0        0      421 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/__init__.py
--rw-r--r--   0        0        0     1929 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/__init__.py
--rw-r--r--   0        0        0      957 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py
--rw-r--r--   0        0        0     1917 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/__init__.py
--rw-r--r--   0        0        0     2589 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/__init__.py
--rw-r--r--   0        0        0     4731 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py
--rw-r--r--   0        0        0     2025 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/__init__.py
--rw-r--r--   0        0        0     2232 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py
--rw-r--r--   0        0        0     4459 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py
--rw-r--r--   0        0        0     5385 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py
--rw-r--r--   0        0        0      274 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/__init__.py
--rw-r--r--   0        0        0      611 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py
--rw-r--r--   0        0        0     1605 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py
--rw-r--r--   0        0        0    11882 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py
--rw-r--r--   0        0        0      183 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/c_deploy/__init__.py
--rw-r--r--   0        0        0     2169 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py
--rw-r--r--   0        0        0     1644 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/util/__init__.py
--rw-r--r--   0        0        0     1686 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py
--rw-r--r--   0        0        0     1181 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/util/step_decorator.py
--rw-r--r--   0        0        0      188 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/util/text.py
--rw-r--r--   0        0        0     7125 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/builds/__init__.py
--rw-r--r--   0        0        0      491 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/builds/builds_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/builds/cancel/__init__.py
--rw-r--r--   0        0        0      181 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/builds/cancel/_logic.py
--rw-r--r--   0        0        0      528 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/builds/cancel/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/builds/logs/__init__.py
--rw-r--r--   0        0        0     1054 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/builds/logs/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/builds/status/__init__.py
--rw-r--r--   0        0        0      256 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/builds/status/_logic.py
--rw-r--r--   0        0        0      983 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/builds/status/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/create/__init__.py
--rw-r--r--   0        0        0     1335 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/create/_logic.py
--rw-r--r--   0        0        0     1016 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/create/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/delete/__init__.py
--rw-r--r--   0        0        0      186 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/delete/_logic.py
--rw-r--r--   0        0        0      638 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/delete/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/__init__.py
--rw-r--r--   0        0        0     1251 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py
--rw-r--r--   0        0        0     2494 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py
--rw-r--r--   0        0        0     8227 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py
--rw-r--r--   0        0        0    13221 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py
--rw-r--r--   0        0        0     3900 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py
--rw-r--r--   0        0        0     5809 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py
--rw-r--r--   0        0        0      770 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py
--rw-r--r--   0        0        0     1067 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py
--rw-r--r--   0        0        0     3166 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/batch/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/batch/_logic/__init__.py
--rw-r--r--   0        0        0      495 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/batch/_logic/advanced_deployment_mapper.py
--rw-r--r--   0        0        0      903 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py
--rw-r--r--   0        0        0     3025 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/batch/ui.py
--rw-r--r--   0        0        0      500 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/deploy_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/realtime/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/__init__.py
--rw-r--r--   0        0        0      902 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py
--rw-r--r--   0        0        0      907 2023-04-27 07:15:38.102821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py
--rw-r--r--   0        0        0     3621 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py
--rw-r--r--   0        0        0     4926 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/streaming/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/__init__.py
--rw-r--r--   0        0        0      905 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py
--rw-r--r--   0        0        0     1500 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py
--rw-r--r--   0        0        0     5391 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/undeploy/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/undeploy/_logic/__init__.py
--rw-r--r--   0        0        0     5783 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py
--rw-r--r--   0        0        0     3036 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py
--rw-r--r--   0        0        0     2093 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/undeploy/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/cancel/__init__.py
--rw-r--r--   0        0        0      409 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/cancel/_logic.py
--rw-r--r--   0        0        0      838 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/cancel/ui.py
--rw-r--r--   0        0        0      799 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/execution_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/report/__init__.py
--rw-r--r--   0        0        0      533 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/report/_logic.py
--rw-r--r--   0        0        0     1445 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/report/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/start/__init__.py
--rw-r--r--   0        0        0      605 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/start/_logic.py
--rw-r--r--   0        0        0     5168 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/start/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/status/__init__.py
--rw-r--r--   0        0        0      480 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/status/_logic.py
--rw-r--r--   0        0        0      830 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/status/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/__init__.py
--rw-r--r--   0        0        0     1375 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/churn/__init__.py
--rw-r--r--   0        0        0       35 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/churn/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0       84 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0      164 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/conda.yml
--rw-r--r--   0        0        0   129370 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv
--rw-r--r--   0        0        0     3610 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/__init__.py
--rw-r--r--   0        0        0     1030 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/__init__.py
--rw-r--r--   0        0        0       41 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0       74 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0      161 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/conda.yml
--rw-r--r--   0        0        0    53393 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv
--rw-r--r--   0        0        0     3967 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/general/__init__.py
--rw-r--r--   0        0        0      139 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/general/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0      120 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/__init__.py
--rw-r--r--   0        0        0      140 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/conda.yml
--rw-r--r--   0        0        0     2169 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/__init__.py
--rw-r--r--   0        0        0      117 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/test_qwak_model.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic/__init__.py
--rw-r--r--   0        0        0       61 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0      104 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0      182 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/conda.yml
--rw-r--r--   0        0        0     3353 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/__init__.py
--rw-r--r--   0        0        0      751 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/__init__.py
--rw-r--r--   0        0        0       68 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0      104 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0     3353 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0      448 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/__init__.py
--rw-r--r--   0        0        0      752 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
--rw-r--r--   0        0        0     1916 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/list/__init__.py
--rw-r--r--   0        0        0      166 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/list/_logic.py
--rw-r--r--   0        0        0     1135 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/list/ui.py
--rw-r--r--   0        0        0     1241 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/models_command_group.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/feedback/__init__.py
--rw-r--r--   0        0        0     2678 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/feedback/_logic.py
--rw-r--r--   0        0        0     1378 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/feedback/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/logs/__init__.py
--rw-r--r--   0        0        0     1577 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/logs/ui.py
--rw-r--r--   0        0        0      693 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/runtime_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/traffic_update/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/traffic_update/_logic/__init__.py
--rw-r--r--   0        0        0     1821 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py
--rw-r--r--   0        0        0     3160 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py
--rw-r--r--   0        0        0     1222 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/traffic_update/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/update/__init__.py
--rw-r--r--   0        0        0      393 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/update/_logic.py
--rw-r--r--   0        0        0      622 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/update/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/projects/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/projects/create/__init__.py
--rw-r--r--   0        0        0      259 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/projects/create/_logic.py
--rw-r--r--   0        0        0      691 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/projects/create/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/projects/delete/__init__.py
--rw-r--r--   0        0        0      203 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/projects/delete/_logic.py
--rw-r--r--   0        0        0      557 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/projects/delete/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/projects/list/__init__.py
--rw-r--r--   0        0        0      182 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/projects/list/_logic.py
--rw-r--r--   0        0        0     1124 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/projects/list/ui.py
--rw-r--r--   0        0        0      589 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/projects/projects_command_group.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/secrets/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/secrets/delete/__init__.py
--rw-r--r--   0        0        0      141 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/secrets/delete/_logic.py
--rw-r--r--   0        0        0      741 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/secrets/delete/ui.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/secrets/get/__init__.py
--rw-r--r--   0        0        0      142 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/secrets/get/_logic.py
--rw-r--r--   0        0        0      574 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/secrets/get/ui.py
--rw-r--r--   0        0        0      502 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/secrets/secrets_commands_group.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/secrets/set/__init__.py
--rw-r--r--   0        0        0      149 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/secrets/set/_logic.py
--rw-r--r--   0        0        0      615 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/secrets/set/ui.py
--rw-r--r--   0        0        0      430 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/commands/ui_tools.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/common/__init__.py
--rw-r--r--   0        0        0      437 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/common/run_config/__init__.py
--rw-r--r--   0        0        0     3166 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/common/run_config/base.py
--rw-r--r--   0        0        0     6087 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/common/run_config/utils.py
--rw-r--r--   0        0        0      381 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0       48 2023-04-27 07:15:38.106821 qwak_sdk-0.2.29rc0/qwak_sdk/exceptions/qwak_command_exception.py
--rw-r--r--   0        0        0      133 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/exceptions/qwak_deploy_new_build_failed.py
--rw-r--r--   0        0        0      424 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/exceptions/qwak_general_build_exception.py
--rw-r--r--   0        0        0      130 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/exceptions/qwak_remote_build_failed.py
--rw-r--r--   0        0        0       48 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/exceptions/qwak_resource_not_found.py
--rw-r--r--   0        0        0      746 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/exceptions/qwak_suggestion_exception.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/inner/__init__.py
--rw-r--r--   0        0        0     3164 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/inner/file_registry.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/inner/tools/__init__.py
--rw-r--r--   0        0        0     4541 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/inner/tools/cli_tools.py
--rw-r--r--   0        0        0      488 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/inner/tools/config_handler.py
--rw-r--r--   0        0        0       71 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/inner/tools/logger/__init__.py
--rw-r--r--   0        0        0     8869 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/inner/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/inner/tools/logger/logging.yml
--rw-r--r--   0        0        0     1013 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/inner/tools/tracking.py
--rw-r--r--   0        0        0      136 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/main.py
--rw-r--r--   0        0        0        0 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/tools/__init__.py
--rw-r--r--   0        0        0      287 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/tools/colors.py
--rw-r--r--   0        0        0      174 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/tools/files.py
--rw-r--r--   0        0        0     5616 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/tools/log_handling.py
--rw-r--r--   0        0        0     1192 2023-04-27 07:15:38.110821 qwak_sdk-0.2.29rc0/qwak_sdk/tools/utils.py
--rw-r--r--   0        0        0     8334 1970-01-01 00:00:00.000000 qwak_sdk-0.2.29rc0/setup.py
--rw-r--r--   0        0        0     1919 1970-01-01 00:00:00.000000 qwak_sdk-0.2.29rc0/PKG-INFO
+-rw-r--r--   0        0        0      183 2023-05-11 08:46:37.673262 qwak_sdk-0.5.3/README.md
+-rw-r--r--   0        0        0     2607 2023-05-11 08:47:24.125490 qwak_sdk-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-05-11 08:47:24.125490 qwak_sdk-0.5.3/qwak_sdk/__init__.py
+-rw-r--r--   0        0        0     2039 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/cli.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/__init__.py
+-rw-r--r--   0        0        0      327 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/admin_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/__init__.py
+-rw-r--r--   0        0        0      467 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/api_keys_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/generate/__init__.py
+-rw-r--r--   0        0        0      677 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/generate/_logic.py
+-rw-r--r--   0        0        0     1393 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/generate/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/revoke/__init__.py
+-rw-r--r--   0        0        0      796 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/revoke/_logic.py
+-rw-r--r--   0        0        0      942 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/revoke/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/__init__.py
+-rw-r--r--   0        0        0      367 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/config_base.py
+-rw-r--r--   0        0        0      885 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/parser.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/__init__.py
+-rw-r--r--   0        0        0      886 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py
+-rw-r--r--   0        0        0     1626 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py
+-rw-r--r--   0        0        0      817 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py
+-rw-r--r--   0        0        0      340 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/route_config.py
+-rw-r--r--   0        0        0      277 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/spec.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/_logic/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/_logic/config/__init__.py
+-rw-r--r--   0        0        0     3098 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/_logic/config/config.py
+-rw-r--r--   0        0        0      646 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/_logic/config/parser.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/attach/__init__.py
+-rw-r--r--   0        0        0     1359 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/attach/_logic.py
+-rw-r--r--   0        0        0      949 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/attach/ui.py
+-rw-r--r--   0        0        0      277 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/autoscaling_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/__init__.py
+-rw-r--r--   0        0        0      857 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/automations_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/delete/__init__.py
+-rw-r--r--   0        0        0      235 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/delete/_logic.py
+-rw-r--r--   0        0        0      604 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/executions/__init__.py
+-rw-r--r--   0        0        0      346 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/executions/executions_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/executions/list/__init__.py
+-rw-r--r--   0        0        0      330 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/executions/list/_logic.py
+-rw-r--r--   0        0        0      669 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/executions/list/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/list/__init__.py
+-rw-r--r--   0        0        0      252 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/list/_logic.py
+-rw-r--r--   0        0        0      546 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/list/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/register/__init__.py
+-rw-r--r--   0        0        0     1624 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/register/_logic.py
+-rw-r--r--   0        0        0     1331 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/register/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/delete/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/delete/_logic.py
+-rw-r--r--   0        0        0     1039 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/delete/ui.py
+-rw-r--r--   0        0        0     1002 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/feature_store_command_group.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/list/__init__.py
+-rw-r--r--   0        0        0     4145 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/list/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/pause/__init__.py
+-rw-r--r--   0        0        0      695 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/pause/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/register/__init__.py
+-rw-r--r--   0        0        0    10893 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/register/_logic.py
+-rw-r--r--   0        0        0     2822 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/register/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/resume/__init__.py
+-rw-r--r--   0        0        0      700 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/resume/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/trigger/__init__.py
+-rw-r--r--   0        0        0     1015 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/trigger/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/_logic/__init__.py
+-rw-r--r--   0        0        0     2050 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/_logic/variations.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/__init__.py
+-rw-r--r--   0        0        0     2005 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/build_steps.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/__init__.py
+-rw-r--r--   0        0        0     6185 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py
+-rw-r--r--   0        0        0     4383 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py
+-rw-r--r--   0        0        0     2908 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/logger.py
+-rw-r--r--   0        0        0     1369 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/messages.py
+-rw-r--r--   0        0        0     1435 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py
+-rw-r--r--   0        0        0      359 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/spinner.py
+-rw-r--r--   0        0        0      975 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py
+-rw-r--r--   0        0        0      311 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/utils.py
+-rw-r--r--   0        0        0     9876 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/config/config_v1.py
+-rw-r--r--   0        0        0      131 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/constant/host_resource.py
+-rw-r--r--   0        0        0      881 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/constant/step_description.py
+-rw-r--r--   0        0        0       73 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/constant/temp_dir.py
+-rw-r--r--   0        0        0      189 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/constant/upload_tag.py
+-rw-r--r--   0        0        0     1872 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/context.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/interface/__init__.py
+-rw-r--r--   0        0        0      568 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py
+-rw-r--r--   0        0        0      745 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/__init__.py
+-rw-r--r--   0        0        0      421 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/__init__.py
+-rw-r--r--   0        0        0     1929 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/__init__.py
+-rw-r--r--   0        0        0      957 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py
+-rw-r--r--   0        0        0     1917 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/__init__.py
+-rw-r--r--   0        0        0     2589 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py
+-rw-r--r--   0        0        0     2025 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/__init__.py
+-rw-r--r--   0        0        0     2232 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py
+-rw-r--r--   0        0        0     4459 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py
+-rw-r--r--   0        0        0     5385 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py
+-rw-r--r--   0        0        0      274 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/__init__.py
+-rw-r--r--   0        0        0      611 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py
+-rw-r--r--   0        0        0     1605 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py
+-rw-r--r--   0        0        0    11882 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py
+-rw-r--r--   0        0        0      183 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/c_deploy/__init__.py
+-rw-r--r--   0        0        0     2169 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py
+-rw-r--r--   0        0        0     1644 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/util/__init__.py
+-rw-r--r--   0        0        0     1686 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py
+-rw-r--r--   0        0        0     1181 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/util/step_decorator.py
+-rw-r--r--   0        0        0      188 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/util/text.py
+-rw-r--r--   0        0        0     7125 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/__init__.py
+-rw-r--r--   0        0        0      491 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/builds_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/cancel/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/cancel/_logic.py
+-rw-r--r--   0        0        0      518 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/cancel/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/logs/__init__.py
+-rw-r--r--   0        0        0     1054 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/logs/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/status/__init__.py
+-rw-r--r--   0        0        0      256 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/status/_logic.py
+-rw-r--r--   0        0        0      973 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/status/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/create/__init__.py
+-rw-r--r--   0        0        0     1335 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/create/_logic.py
+-rw-r--r--   0        0        0     1016 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/create/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/delete/__init__.py
+-rw-r--r--   0        0        0      186 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/delete/_logic.py
+-rw-r--r--   0        0        0      638 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/__init__.py
+-rw-r--r--   0        0        0     1251 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py
+-rw-r--r--   0        0        0     2494 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py
+-rw-r--r--   0        0        0     8227 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py
+-rw-r--r--   0        0        0    13221 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py
+-rw-r--r--   0        0        0     3900 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py
+-rw-r--r--   0        0        0     5799 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py
+-rw-r--r--   0        0        0      770 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py
+-rw-r--r--   0        0        0     1067 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py
+-rw-r--r--   0        0        0     3166 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/batch/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/batch/_logic/__init__.py
+-rw-r--r--   0        0        0      495 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/batch/_logic/advanced_deployment_mapper.py
+-rw-r--r--   0        0        0      903 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py
+-rw-r--r--   0        0        0     3015 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/batch/ui.py
+-rw-r--r--   0        0        0      500 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/deploy_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/__init__.py
+-rw-r--r--   0        0        0      902 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py
+-rw-r--r--   0        0        0      907 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py
+-rw-r--r--   0        0        0     3621 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py
+-rw-r--r--   0        0        0     4917 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/streaming/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/__init__.py
+-rw-r--r--   0        0        0      905 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py
+-rw-r--r--   0        0        0     1500 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py
+-rw-r--r--   0        0        0     5381 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/undeploy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/undeploy/_logic/__init__.py
+-rw-r--r--   0        0        0     5773 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py
+-rw-r--r--   0        0        0     3036 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py
+-rw-r--r--   0        0        0     2083 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/undeploy/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/cancel/__init__.py
+-rw-r--r--   0        0        0      409 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/cancel/_logic.py
+-rw-r--r--   0        0        0      828 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/cancel/ui.py
+-rw-r--r--   0        0        0      789 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/execution_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/report/__init__.py
+-rw-r--r--   0        0        0      533 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/report/_logic.py
+-rw-r--r--   0        0        0     1435 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/report/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/start/__init__.py
+-rw-r--r--   0        0        0      605 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/start/_logic.py
+-rw-r--r--   0        0        0     5158 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/start/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/status/__init__.py
+-rw-r--r--   0        0        0      480 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/status/_logic.py
+-rw-r--r--   0        0        0      820 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/status/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/__init__.py
+-rw-r--r--   0        0        0     1375 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/__init__.py
+-rw-r--r--   0        0        0       35 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0      164 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/conda.yml
+-rw-r--r--   0        0        0   129370 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv
+-rw-r--r--   0        0        0     3610 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/__init__.py
+-rw-r--r--   0        0        0     1030 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0       74 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0      161 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/conda.yml
+-rw-r--r--   0        0        0    53393 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv
+-rw-r--r--   0        0        0     3967 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0      120 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/conda.yml
+-rw-r--r--   0        0        0     2169 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/__init__.py
+-rw-r--r--   0        0        0      117 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/test_qwak_model.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0      104 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/conda.yml
+-rw-r--r--   0        0        0     3353 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/__init__.py
+-rw-r--r--   0        0        0      751 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0      104 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0     3353 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0      448 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/__init__.py
+-rw-r--r--   0        0        0      752 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
+-rw-r--r--   0        0        0     1906 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/list/__init__.py
+-rw-r--r--   0        0        0      166 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/list/_logic.py
+-rw-r--r--   0        0        0     1135 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/list/ui.py
+-rw-r--r--   0        0        0     1241 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/models_command_group.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/feedback/__init__.py
+-rw-r--r--   0        0        0     2678 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/feedback/_logic.py
+-rw-r--r--   0        0        0     1378 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/feedback/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/logs/__init__.py
+-rw-r--r--   0        0        0     1577 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/logs/ui.py
+-rw-r--r--   0        0        0      693 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/runtime_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/traffic_update/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/traffic_update/_logic/__init__.py
+-rw-r--r--   0        0        0     1811 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py
+-rw-r--r--   0        0        0     3160 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py
+-rw-r--r--   0        0        0     1212 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/traffic_update/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/update/__init__.py
+-rw-r--r--   0        0        0      393 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/update/_logic.py
+-rw-r--r--   0        0        0      622 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/update/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/create/__init__.py
+-rw-r--r--   0        0        0      259 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/create/_logic.py
+-rw-r--r--   0        0        0      691 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/create/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/delete/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/delete/_logic.py
+-rw-r--r--   0        0        0      557 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/list/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/list/_logic.py
+-rw-r--r--   0        0        0     1124 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/list/ui.py
+-rw-r--r--   0        0        0      589 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/projects_command_group.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/delete/__init__.py
+-rw-r--r--   0        0        0      141 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/delete/_logic.py
+-rw-r--r--   0        0        0      741 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/get/__init__.py
+-rw-r--r--   0        0        0      142 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/get/_logic.py
+-rw-r--r--   0        0        0      574 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/get/ui.py
+-rw-r--r--   0        0        0      502 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/secrets_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/set/__init__.py
+-rw-r--r--   0        0        0      149 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/set/_logic.py
+-rw-r--r--   0        0        0      615 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/set/ui.py
+-rw-r--r--   0        0        0      430 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/ui_tools.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/common/__init__.py
+-rw-r--r--   0        0        0      437 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/common/run_config/__init__.py
+-rw-r--r--   0        0        0     3166 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/common/run_config/base.py
+-rw-r--r--   0        0        0     6087 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/common/run_config/utils.py
+-rw-r--r--   0        0        0      381 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/exceptions/qwak_command_exception.py
+-rw-r--r--   0        0        0      133 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/exceptions/qwak_deploy_new_build_failed.py
+-rw-r--r--   0        0        0      424 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/exceptions/qwak_general_build_exception.py
+-rw-r--r--   0        0        0      130 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/exceptions/qwak_remote_build_failed.py
+-rw-r--r--   0        0        0       48 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/exceptions/qwak_resource_not_found.py
+-rw-r--r--   0        0        0      746 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/exceptions/qwak_suggestion_exception.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/__init__.py
+-rw-r--r--   0        0        0     3164 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/file_registry.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/tools/__init__.py
+-rw-r--r--   0        0        0     4541 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/tools/cli_tools.py
+-rw-r--r--   0        0        0      488 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/tools/config_handler.py
+-rw-r--r--   0        0        0       71 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/tools/logger/__init__.py
+-rw-r--r--   0        0        0     8869 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/tools/logger/logging.yml
+-rw-r--r--   0        0        0     1013 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/tools/tracking.py
+-rw-r--r--   0        0        0      136 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/main.py
+-rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/tools/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/tools/colors.py
+-rw-r--r--   0        0        0     2257 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/tools/files.py
+-rw-r--r--   0        0        0     5616 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/tools/log_handling.py
+-rw-r--r--   0        0        0     1168 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/tools/utils.py
+-rw-r--r--   0        0        0     8325 1970-01-01 00:00:00.000000 qwak_sdk-0.5.3/setup.py
+-rw-r--r--   0        0        0     1910 1970-01-01 00:00:00.000000 qwak_sdk-0.5.3/PKG-INFO
```

### Comparing `qwak_sdk-0.2.29rc0/pyproject.toml` & `qwak_sdk-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-sdk"
-version = "0.2.29.rc0"
+version = "0.5.3"
 description = "Qwak SDK and CLI for qwak models"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     {include = "qwak_sdk"},
 ]
@@ -23,16 +23,16 @@
 "Home page" = "https://www.qwak.com/"
 
 [tool.poetry.scripts]
 qwak = "qwak_sdk.main:qwak_cli"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.10"
-qwak-core = "==0.0.35"
-qwak-inference = "==0.0.11.rc0"
+qwak-core = "==0.0.53"
+qwak-inference = "==0.1.1"
 tabulate = ">=0.8.0"
 python-json-logger = ">=2.0.2"
 pydantic = "*"
 yaspin = ">=2.0.0"
 assertpy = "^1.1"
 cookiecutter = "*"
 gitpython = ">=2.1.0"
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/cli.py` & `qwak_sdk-0.5.3/qwak_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/admin/apikeys/generate/_logic.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/generate/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/admin/apikeys/generate/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/generate/ui.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 from qwak.clients.administration.self_service.client import APIKEY_ALREADY_EXISTS
+from qwak.tools.logger.logger import get_qwak_logger
 
 from qwak_sdk.commands.admin.apikeys.generate._logic import execute_generate_apikey
 from qwak_sdk.inner.tools.cli_tools import QwakCommand
-from qwak_sdk.inner.tools.logger.logger import get_qwak_logger
 
 logger = get_qwak_logger()
 
 
 @click.command("generate", help="api keys", cls=QwakCommand)
 @click.option(
     "--environment-name",
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/admin/apikeys/revoke/_logic.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/revoke/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/admin/apikeys/revoke/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/revoke/ui.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import click
+from qwak.tools.logger.logger import get_qwak_logger
 
 from qwak_sdk.commands.admin.apikeys.revoke._logic import execute_revoke_apikey
 from qwak_sdk.inner.tools.cli_tools import QwakCommand
-from qwak_sdk.inner.tools.logger.logger import get_qwak_logger
 
 logger = get_qwak_logger()
 
 
 @click.command("revoke", help="api keys", cls=QwakCommand)
 @click.option(
     "--environment-name",
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/audience/_logic/config/parser.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/parser.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/auto_scalling/_logic/config/config.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/_logic/config/config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/auto_scalling/_logic/config/parser.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/_logic/config/parser.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/auto_scalling/attach/_logic.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/attach/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/auto_scalling/attach/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/attach/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/automations_commands_group.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/automations/automations_commands_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/delete/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/automations/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/executions/list/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/automations/executions/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/list/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/automations/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/register/_logic.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/automations/register/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/automations/register/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/automations/register/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/delete/_logic.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/delete/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/delete/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/feature_store_command_group.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/feature_store_command_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/list/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/pause/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/pause/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/register/_logic.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/register/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/register/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/register/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/resume/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/resume/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/feature_store/trigger/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/trigger/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/_logic/variations.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/build_steps.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/build_steps.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,17 @@
         exit(1)
 
     def handle_pipeline_quiet_exception(
         self, build_id: str, phase_id: str, ex: BaseException, duration_in_seconds: int
     ):
         if self.sp:
             self.sp.ok("‼️")
+            print(f"\n{Color.RED}{ex}")
         self.__report_failure(phase_id, duration_in_seconds)
+        exit(1)
 
 
 class ProgrammaticBuildRunner(BuildRunHandler):
     def handle_phase_in_progress(self, phase_id: str):
         logging.debug(
             f"Build phase in progress: {self.build_phase_to_human_readable_string(phase_id)}"
         )
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/client_logs/logger.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/client_logs/messages.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/messages.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/config/config_v1.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/config/config_v1.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/constant/step_description.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/constant/step_description.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/context.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/context.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/_logic/util/step_decorator.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/util/step_decorator.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/build/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/builds/cancel/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/cancel/ui.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import click
+from qwak.tools.logger.logger import get_qwak_logger
 
 from qwak_sdk.commands.models.builds.cancel._logic import execute_cancel_build
 from qwak_sdk.inner.tools.cli_tools import QwakCommand
-from qwak_sdk.inner.tools.logger.logger import get_qwak_logger
 
 logger = get_qwak_logger()
 
 
 @click.command("cancel", cls=QwakCommand)
 @click.argument("build_id")
 def cancel_build(build_id, **kwargs):
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/builds/logs/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/logs/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/builds/status/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/status/ui.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 
 import click
 from _qwak_proto.qwak.builds.builds_pb2 import BuildStatus
+from qwak.tools.logger.logger import get_qwak_logger
 
 from qwak_sdk.commands.models.builds.status._logic import execute_get_build_status
 from qwak_sdk.inner.tools.cli_tools import QwakCommand
-from qwak_sdk.inner.tools.logger.logger import get_qwak_logger
 
 logger = get_qwak_logger()
 
 
 @click.command("status", cls=QwakCommand)
 @click.argument("build_id")
 def get_build_status(build_id, **kwargs):
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/create/_logic.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/create/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/create/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/create/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/delete/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Dict
 
 from _qwak_proto.qwak.deployment.deployment_pb2 import ModelDeploymentStatus
 from _qwak_proto.qwak.deployment.deployment_service_pb2 import DeployModelResponse
 from _qwak_proto.qwak.ecosystem.v0.ecosystem_pb2 import UserContextEnvironmentDetails
 from qwak.clients.administration.eco_system.client import EcosystemClient
 from qwak.exceptions import QwakException
+from qwak.tools.logger.logger import get_qwak_logger
 from tabulate import tabulate
 
 from qwak_sdk.commands.models.deployments.deploy._logic.base_deploy_executor import (
     FAILED_STATUS,
     BaseDeployExecutor,
 )
-from qwak_sdk.inner.tools.logger.logger import get_qwak_logger
 from qwak_sdk.tools.utils import qwak_spinner
 
 logger = get_qwak_logger()
 
 
 def __client_deployment_remote(
     deploy: BaseDeployExecutor, sync: bool, output_multiple: bool = False
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/batch/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/batch/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import click
 from qwak.inner.const import QwakConstants
+from qwak.tools.logger.logger import set_qwak_logger_stdout_verbosity_level
 
 from qwak_sdk.commands.models.deployments.deploy._logic.deploy_config import (
     DeployConfig,
     PurchaseOption,
 )
 from qwak_sdk.commands.models.deployments.deploy._logic.deployment_response_handler import (
     client_deployment,
 )
 from qwak_sdk.commands.models.deployments.deploy.batch._logic.deploy_executor import (
     BatchDeployExecutor,
 )
 from qwak_sdk.inner.tools.cli_tools import QwakCommand
 from qwak_sdk.inner.tools.config_handler import config_handler
-from qwak_sdk.inner.tools.logger.logger import set_qwak_logger_stdout_verbosity_level
 
 
 @click.command("batch", help="Deploy batch model.", cls=QwakCommand)
 @click.option(
     "--build-id",
     help="Build ID, If not specified latest successful build will deployed.",
     type=str,
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Optional
 
 import click
 from qwak.inner.const import QwakConstants
+from qwak.tools.logger.logger import (
+    get_qwak_logger,
+    set_qwak_logger_stdout_verbosity_level,
+)
 
 from qwak_sdk.commands.models.deployments.deploy._logic.deploy_config import (
     DeployConfig,
     PurchaseOption,
 )
 from qwak_sdk.commands.models.deployments.deploy._logic.deployment_response_handler import (
     client_deployment,
 )
 from qwak_sdk.commands.models.deployments.deploy.realtime._logic.deploy_executor import (
     RealtimeDeployExecutor,
 )
 from qwak_sdk.inner.tools.cli_tools import QwakCommand
 from qwak_sdk.inner.tools.config_handler import config_handler
-from qwak_sdk.inner.tools.logger.logger import (
-    get_qwak_logger,
-    set_qwak_logger_stdout_verbosity_level,
-)
 
 logger = get_qwak_logger()
 PENDING_STATUSES = [
     "INITIATING_DEPLOYMENT",
     "PENDING_DEPLOYMENT",
     "INITIATING_UNDEPLOYMENT",
     "PENDING_UNDEPLOYMENT",
@@ -145,15 +145,15 @@
     help="Indicate the instance deployments type, whether it is spot/ondemand. Default is spot",
 )
 @click.option(
     "--deployments-timeout",
     type=int,
     help="The number of seconds the deployments can be in progress before it is considered as failed. This is useful "
     "in cases where a deployments has a high number of pods to replace, scarce resources (gpu), or large build "
-    "size. Default is 600 seconds (10 minutes).",
+    "size. Default is 1800 seconds (30 minutes).",
 )
 @click.option(
     "-E",
     "--env-vars",
     required=False,
     metavar="NAME=VALUE",
     multiple=True,
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 import click
+from qwak.tools.logger.logger import (
+    get_qwak_logger,
+    set_qwak_logger_stdout_verbosity_level,
+)
 
 from qwak_sdk.commands.models.deployments.deploy._logic.deploy_config import (
     AutoOffsetReset,
     CompressionTypes,
     DeployConfig,
     PurchaseOption,
 )
@@ -10,18 +14,14 @@
     client_deployment,
 )
 from qwak_sdk.commands.models.deployments.deploy.streaming._logic.deploy_executor import (
     StreamDeployExecutor,
 )
 from qwak_sdk.inner.tools.cli_tools import QwakCommand
 from qwak_sdk.inner.tools.config_handler import config_handler
-from qwak_sdk.inner.tools.logger.logger import (
-    get_qwak_logger,
-    set_qwak_logger_stdout_verbosity_level,
-)
 
 logger = get_qwak_logger()
 PENDING_STATUSES = [
     "INITIATING_DEPLOYMENT",
     "PENDING_DEPLOYMENT",
     "INITIATING_UNDEPLOYMENT",
     "PENDING_UNDEPLOYMENT",
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,25 +9,25 @@
     TrafficConfig,
     Variation,
 )
 from _qwak_proto.qwak.ecosystem.v0.ecosystem_pb2 import EnvironmentDetails
 from qwak.clients.administration.eco_system.client import EcosystemClient
 from qwak.clients.deployment.client import DeploymentManagementClient
 from qwak.exceptions import QwakException
+from qwak.tools.logger.logger import get_qwak_logger
 
 from qwak_sdk.commands.models._logic.variations import (
     create_variation_from_variation_config,
 )
 from qwak_sdk.commands.models.deployments.deploy._logic.deploy_config import (
     DeployConfig,
 )
 from qwak_sdk.commands.models.deployments.undeploy._logic.variations import (
     validate_variations_for_undeploy,
 )
-from qwak_sdk.inner.tools.logger.logger import get_qwak_logger
 
 NO_DEPLOYED_VARIATIONS_ERROR_MSG = (
     "There are currently no deployed variations for model {model_id} in {env_name}"
 )
 
 logger = get_qwak_logger()
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/deployments/undeploy/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/undeploy/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import List
 
 import click
 from qwak.clients.model_management import ModelsManagementClient
+from qwak.tools.logger.logger import get_qwak_logger
 
 from qwak_sdk.commands.models.deployments.deploy._logic.deploy_config import (
     DeployConfig,
 )
 from qwak_sdk.commands.models.deployments.undeploy._logic.request_undeploy import (
     undeploy,
 )
 from qwak_sdk.inner.tools.cli_tools import QwakCommand
 from qwak_sdk.inner.tools.config_handler import config_handler
-from qwak_sdk.inner.tools.logger.logger import get_qwak_logger
 
 logger = get_qwak_logger()
 
 
 @click.command(
     name="undeploy",
     help="Model undeploy operation",
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/cancel/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/cancel/ui.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 from qwak.exceptions import QwakException
+from qwak.tools.logger.logger import get_qwak_logger
 
 from qwak_sdk.commands.models.executions.cancel._logic import execute_execution_cancel
 from qwak_sdk.inner.tools.cli_tools import QwakCommand
-from qwak_sdk.inner.tools.logger.logger import get_qwak_logger
 
 logger = get_qwak_logger()
 
 
 @click.command(name="cancel", help="Cancel a running execution.", cls=QwakCommand)
 @click.option(
     "--execution-id",
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/execution_commands_group.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/execution_commands_group.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import click
+from qwak.tools.logger.logger import get_qwak_logger
 
 from qwak_sdk.commands.models.executions.cancel.ui import execution_cancel
 from qwak_sdk.commands.models.executions.report.ui import execution_report
 from qwak_sdk.commands.models.executions.start.ui import execution_start
 from qwak_sdk.commands.models.executions.status.ui import execution_status
-from qwak_sdk.inner.tools.logger.logger import get_qwak_logger
 
 logger = get_qwak_logger()
 
 
 @click.group(
     name="execution",
     help="Executions of a batch job on deployed model.",
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/report/_logic.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/report/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/report/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/report/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 from qwak.exceptions import QwakException
+from qwak.tools.logger.logger import get_qwak_logger
 
 from qwak_sdk.commands.models.executions.report._logic import execute_execution_report
 from qwak_sdk.inner.tools.cli_tools import QwakCommand
-from qwak_sdk.inner.tools.logger.logger import get_qwak_logger
 from qwak_sdk.tools.colors import Color
 
 logger = get_qwak_logger()
 
 
 @click.command(name="report", help="Get the report of an execution.", cls=QwakCommand)
 @click.option(
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/start/_logic.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/start/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/start/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/start/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
     GPU_TYPE_MAP,
     INPUT_FORMATTERS_MAP,
     OUTPUT_FORMATTERS_MAP,
     ExecutionConfig,
 )
 from qwak.exceptions import QwakException
 from qwak.inner.const import QwakConstants
+from qwak.tools.logger.logger import get_qwak_logger
 from tabulate import tabulate
 
 from qwak_sdk.commands.models.executions.start._logic import execute_start_execution
 from qwak_sdk.inner.tools.cli_tools import QwakCommand
 from qwak_sdk.inner.tools.config_handler import config_handler
-from qwak_sdk.inner.tools.logger.logger import get_qwak_logger
 
 logger = get_qwak_logger()
 
 
 @click.command(
     name="start", help="Start an execution job on a deployed model.", cls=QwakCommand
 )
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/executions/status/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/status/ui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 from qwak.exceptions import QwakException
+from qwak.tools.logger.logger import get_qwak_logger
 
 from qwak_sdk.commands.models.executions.status._logic import execute_execution_status
 from qwak_sdk.inner.tools.cli_tools import QwakCommand
-from qwak_sdk.inner.tools.logger.logger import get_qwak_logger
 
 logger = get_qwak_logger()
 
 
 @click.command(name="status", help="Get the status of an execution.", cls=QwakCommand)
 @click.option(
     "--execution-id",
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/init/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/ui.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import click
+from qwak.tools.logger.logger import get_qwak_logger
 
 from qwak_sdk.commands.models.init._logic.initialize_model_structure import (
     initialize_model_structure,
 )
 from qwak_sdk.inner.tools.cli_tools import QwakCommand
-from qwak_sdk.inner.tools.logger.logger import get_qwak_logger
 
 logger = get_qwak_logger()
 
 
 @click.command("init", cls=QwakCommand)
 @click.option(
     "--model-directory", metavar="NAME", required=False, help="folder for model content"
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/list/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/models_command_group.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/models_command_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/feedback/_logic.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/feedback/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/feedback/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/feedback/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/logs/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/logs/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/runtime_commands_group.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/runtime_commands_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Tuple
 
 from qwak.clients.administration.eco_system.client import EcosystemClient
 from qwak.clients.deployment.client import DeploymentManagementClient
+from qwak.tools.logger.logger import get_qwak_logger
 
 from qwak_sdk.commands.models._logic.variations import (
     create_variation_from_variation_config,
 )
 from qwak_sdk.commands.models.deployments.deploy._logic.deploy_config import (
     DeployConfig,
 )
 from qwak_sdk.commands.models.runtime.traffic_update._logic.variations import (
     validate_requested_variations_against_existing_in_apply,
 )
 from qwak_sdk.inner.tools.config_handler import config_handler
-from qwak_sdk.inner.tools.logger.logger import get_qwak_logger
 
 logger = get_qwak_logger()
 
 
 def execute_runtime_traffic_update(
     model_id: str, from_file: str, environment_name: Tuple[str]
 ):
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/traffic_update/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/traffic_update/ui.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Tuple
 
 import click
 from qwak.exceptions import QwakException
+from qwak.tools.logger.logger import get_qwak_logger
 
 from qwak_sdk.commands.models.runtime.traffic_update._logic.execute_runtime_update_traffic import (
     execute_runtime_traffic_update,
 )
 from qwak_sdk.inner.tools.cli_tools import QwakCommand
-from qwak_sdk.inner.tools.logger.logger import get_qwak_logger
 
 logger = get_qwak_logger()
 
 
 @click.command("traffic_update", cls=QwakCommand)
 @click.option("-m", "--model-id", required=True, help="Model named ID")
 @click.option(
```

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/models/runtime/update/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/update/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/projects/create/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/projects/create/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/projects/delete/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/projects/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/projects/list/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/projects/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/projects/projects_command_group.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/projects/projects_command_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/secrets/delete/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/secrets/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/secrets/get/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/secrets/get/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/commands/secrets/set/ui.py` & `qwak_sdk-0.5.3/qwak_sdk/commands/secrets/set/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/common/run_config/base.py` & `qwak_sdk-0.5.3/qwak_sdk/common/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/common/run_config/utils.py` & `qwak_sdk-0.5.3/qwak_sdk/common/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/exceptions/qwak_suggestion_exception.py` & `qwak_sdk-0.5.3/qwak_sdk/exceptions/qwak_suggestion_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/inner/file_registry.py` & `qwak_sdk-0.5.3/qwak_sdk/inner/file_registry.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/inner/tools/cli_tools.py` & `qwak_sdk-0.5.3/qwak_sdk/inner/tools/cli_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/inner/tools/logger/logger.py` & `qwak_sdk-0.5.3/qwak_sdk/inner/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/inner/tools/logger/logging.yml` & `qwak_sdk-0.5.3/qwak_sdk/inner/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/inner/tools/tracking.py` & `qwak_sdk-0.5.3/qwak_sdk/inner/tools/tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/tools/log_handling.py` & `qwak_sdk-0.5.3/qwak_sdk/tools/log_handling.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.2.29rc0/qwak_sdk/tools/utils.py` & `qwak_sdk-0.5.3/qwak_sdk/tools/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import logging
 import sys
 from contextlib import contextmanager
 from typing import Callable, Optional
 
+from qwak.tools.logger.logger import get_qwak_logger, get_qwak_logger_verbosity_level
 from yaspin import yaspin
 
-from qwak_sdk.inner.tools.logger.logger import (
-    get_qwak_logger,
-    get_qwak_logger_verbosity_level,
-)
-
 logger = get_qwak_logger()
 
 
 @contextmanager
 def qwak_spinner(
     begin_text: Optional[str],
     end_text: Optional[str] = "",
```

### Comparing `qwak_sdk-0.2.29rc0/setup.py` & `qwak_sdk-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,16 +123,16 @@
 
 install_requires = \
 ['assertpy>=1.1,<2.0',
  'cookiecutter',
  'gitpython>=2.1.0',
  'pydantic',
  'python-json-logger>=2.0.2',
- 'qwak-core==0.0.35',
- 'qwak-inference==0.0.11.rc0',
+ 'qwak-core==0.0.53',
+ 'qwak-inference==0.1.1',
  'tabulate>=0.8.0',
  'yaspin>=2.0.0']
 
 extras_require = \
 {'batch': ['boto3>=1.24.89,<2.0.0',
            'joblib>=1.1.0,<2.0.0',
            'pyarrow>=6.0.0,<11.0.0'],
@@ -147,15 +147,15 @@
                                                                   'pandas>=1.4.3,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['qwak = qwak_sdk.main:qwak_cli']}
 
 setup_kwargs = {
     'name': 'qwak-sdk',
-    'version': '0.2.29rc0',
+    'version': '0.5.3',
     'description': 'Qwak SDK and CLI for qwak models',
     'long_description': '# Qwak SDK\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_sdk-0.2.29rc0/PKG-INFO` & `qwak_sdk-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-sdk
-Version: 0.2.29rc0
+Version: 0.5.3
 Summary: Qwak SDK and CLI for qwak models
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -25,16 +25,16 @@
 Requires-Dist: gitpython (>=2.1.0)
 Requires-Dist: joblib (>=1.1.0,<2.0.0) ; extra == "batch" or extra == "feedback"
 Requires-Dist: pandas (<1.4) ; (python_full_version >= "3.7.1" and python_version < "3.8") and (extra == "batch" or extra == "feedback")
 Requires-Dist: pandas (>=1.4.3,<2.0.0) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "batch" or extra == "feedback")
 Requires-Dist: pyarrow (>=6.0.0,<11.0.0) ; extra == "batch"
 Requires-Dist: pydantic
 Requires-Dist: python-json-logger (>=2.0.2)
-Requires-Dist: qwak-core (==0.0.35)
-Requires-Dist: qwak-inference (==0.0.11.rc0)
+Requires-Dist: qwak-core (==0.0.53)
+Requires-Dist: qwak-inference (==0.1.1)
 Requires-Dist: tabulate (>=0.8.0)
 Requires-Dist: yaspin (>=2.0.0)
 Project-URL: Home page, https://www.qwak.com/
 Description-Content-Type: text/markdown
 
 # Qwak SDK
```

