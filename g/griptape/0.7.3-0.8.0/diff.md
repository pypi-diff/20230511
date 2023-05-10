# Comparing `tmp/griptape-0.7.3.tar.gz` & `tmp/griptape-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape-0.7.3.tar", max compression
+gzip compressed data, was "griptape-0.8.0.tar", max compression
```

## Comparing `griptape-0.7.3.tar` & `griptape-0.8.0.tar`

### file list

```diff
@@ -1,120 +1,111 @@
--rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape-0.7.3/LICENSE
--rw-r--r--   0        0        0     4585 2023-05-02 23:30:51.255832 griptape-0.7.3/README.md
--rw-r--r--   0        0        0       65 2023-04-24 19:02:26.305879 griptape-0.7.3/griptape/__init__.py
--rw-r--r--   0        0        0      252 2023-04-30 17:35:29.017295 griptape-0.7.3/griptape/artifacts/__init__.py
--rw-r--r--   0        0        0      790 2023-05-01 15:10:00.633569 griptape-0.7.3/griptape/artifacts/base_artifact.py
--rw-r--r--   0        0        0      614 2023-04-30 17:35:28.969088 griptape-0.7.3/griptape/artifacts/error_artifact.py
--rw-r--r--   0        0        0      595 2023-04-30 17:35:28.959962 griptape-0.7.3/griptape/artifacts/text_artifact.py
--rw-r--r--   0        0        0      259 2023-04-28 14:34:39.021439 griptape-0.7.3/griptape/converters/__init__.py
--rw-r--r--   0        0        0      220 2023-04-28 14:34:39.020206 griptape-0.7.3/griptape/converters/base_converter.py
--rw-r--r--   0        0        0     2710 2023-04-30 17:35:29.011420 griptape-0.7.3/griptape/converters/chatgpt_plugin_converter.py
--rw-r--r--   0        0        0     1075 2023-04-30 17:35:28.978469 griptape-0.7.3/griptape/converters/langchain_tool_converter.py
--rw-r--r--   0        0        0      180 2023-04-28 15:15:41.999422 griptape-0.7.3/griptape/core/__init__.py
--rw-r--r--   0        0        0     2035 2023-04-27 23:20:01.169051 griptape-0.7.3/griptape/core/activity_mixin.py
--rw-r--r--   0        0        0     4110 2023-05-01 15:24:09.937386 griptape-0.7.3/griptape/core/base_tool.py
--rw-r--r--   0        0        0      533 2023-04-28 15:15:42.001353 griptape-0.7.3/griptape/core/decorators.py
--rw-r--r--   0        0        0      819 2023-04-27 20:13:16.211614 griptape-0.7.3/griptape/core/tool_loader.py
--rw-r--r--   0        0        0     1084 2023-04-30 19:54:49.004253 griptape-0.7.3/griptape/drivers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 griptape-0.7.3/griptape/drivers/memory/__init__.py
--rw-r--r--   0        0        0      555 2023-04-24 18:12:25.623896 griptape-0.7.3/griptape/drivers/memory/disk_memory_driver.py
--rw-r--r--   0        0        0      238 2023-04-23 22:46:42.644482 griptape-0.7.3/griptape/drivers/memory/memory_driver.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 griptape-0.7.3/griptape/drivers/prompt/__init__.py
--rw-r--r--   0        0        0     1192 2023-04-30 17:35:28.980331 griptape-0.7.3/griptape/drivers/prompt/base_prompt_driver.py
--rw-r--r--   0        0        0     1279 2023-04-30 17:35:29.003157 griptape-0.7.3/griptape/drivers/prompt/cohere_prompt_driver.py
--rw-r--r--   0        0        0     1956 2023-04-30 17:35:29.016094 griptape-0.7.3/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py
--rw-r--r--   0        0        0     1733 2023-04-30 17:35:29.013147 griptape-0.7.3/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py
--rw-r--r--   0        0        0     2711 2023-04-30 17:35:28.955013 griptape-0.7.3/griptape/drivers/prompt/openai_prompt_driver.py
--rw-r--r--   0        0        0        0 2023-04-27 20:13:16.212093 griptape-0.7.3/griptape/drivers/storage/__init__.py
--rw-r--r--   0        0        0      320 2023-04-27 20:13:16.212485 griptape-0.7.3/griptape/drivers/storage/base_storage_driver.py
--rw-r--r--   0        0        0     1365 2023-04-30 19:56:37.363730 griptape-0.7.3/griptape/drivers/storage/dynamodb_storage_driver.py
--rw-r--r--   0        0        0      557 2023-04-27 20:13:16.212694 griptape-0.7.3/griptape/drivers/storage/memory_storage_driver.py
--rw-r--r--   0        0        0      203 2023-04-23 17:45:35.150209 griptape-0.7.3/griptape/executors/__init__.py
--rw-r--r--   0        0        0     1916 2023-05-01 15:10:15.434624 griptape-0.7.3/griptape/executors/base_executor.py
--rw-r--r--   0        0        0     3326 2023-04-30 17:35:28.975177 griptape-0.7.3/griptape/executors/docker_executor.py
--rw-r--r--   0        0        0     2203 2023-04-30 17:35:28.958452 griptape-0.7.3/griptape/executors/local_executor.py
--rw-r--r--   0        0        0      271 2023-04-24 16:31:58.604436 griptape-0.7.3/griptape/memory/__init__.py
--rw-r--r--   0        0        0      701 2023-04-24 16:31:37.147209 griptape-0.7.3/griptape/memory/buffer_memory.py
--rw-r--r--   0        0        0     1758 2023-04-24 18:12:25.647629 griptape-0.7.3/griptape/memory/memory.py
--rw-r--r--   0        0        0      360 2023-04-23 22:49:52.124272 griptape-0.7.3/griptape/memory/run.py
--rw-r--r--   0        0        0     2024 2023-04-30 17:51:16.198545 griptape-0.7.3/griptape/memory/summary_memory.py
--rw-r--r--   0        0        0      120 2023-04-30 19:23:55.559304 griptape-0.7.3/griptape/ramps/__init__.py
--rw-r--r--   0        0        0      526 2023-04-30 19:23:55.545401 griptape-0.7.3/griptape/ramps/base_ramp.py
--rw-r--r--   0        0        0     2722 2023-05-03 17:48:46.260929 griptape-0.7.3/griptape/ramps/storage_ramp.py
--rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape-0.7.3/griptape/resources/docker_executor/Dockerfile
--rw-r--r--   0        0        0      126 2023-04-23 17:06:19.949373 griptape-0.7.3/griptape/rules/__init__.py
--rw-r--r--   0        0        0      461 2023-04-23 17:06:19.967138 griptape-0.7.3/griptape/rules/json.py
--rw-r--r--   0        0        0      495 2023-04-23 17:06:19.964844 griptape-0.7.3/griptape/rules/meta.py
--rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 griptape-0.7.3/griptape/rules/rule.py
--rw-r--r--   0        0        0     2183 2023-04-30 17:35:28.976419 griptape-0.7.3/griptape/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape-0.7.3/griptape/schemas/artifacts/__init__.py
--rw-r--r--   0        0        0      313 2023-04-30 16:38:23.177438 griptape-0.7.3/griptape/schemas/artifacts/artifact_schema.py
--rw-r--r--   0        0        0      269 2023-04-30 17:35:28.962971 griptape-0.7.3/griptape/schemas/artifacts/error_artifact_schema.py
--rw-r--r--   0        0        0      266 2023-04-30 17:35:28.966009 griptape-0.7.3/griptape/schemas/artifacts/text_artifact_schema.py
--rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 griptape-0.7.3/griptape/schemas/base_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape-0.7.3/griptape/schemas/drivers/__init__.py
--rw-r--r--   0        0        0      572 2023-04-24 18:12:25.664870 griptape-0.7.3/griptape/schemas/drivers/openai_prompt_driver_schema.py
--rw-r--r--   0        0        0      414 2023-04-23 17:06:19.959444 griptape-0.7.3/griptape/schemas/drivers/prompt_driver_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069641 griptape-0.7.3/griptape/schemas/memory/__init__.py
--rw-r--r--   0        0        0      307 2023-04-24 16:31:58.605715 griptape-0.7.3/griptape/schemas/memory/buffer_memory_schema.py
--rw-r--r--   0        0        0      385 2023-04-23 22:46:42.639391 griptape-0.7.3/griptape/schemas/memory/memory_schema.py
--rw-r--r--   0        0        0      350 2023-04-23 22:46:42.623642 griptape-0.7.3/griptape/schemas/memory/run_schema.py
--rw-r--r--   0        0        0      436 2023-04-24 16:31:58.600703 griptape-0.7.3/griptape/schemas/memory/summary_memory_schema.py
--rw-r--r--   0        0        0     5937 2023-04-23 17:06:19.960660 griptape-0.7.3/griptape/schemas/polymorphic_schema.py
--rw-r--r--   0        0        0      264 2023-04-23 17:06:19.956178 griptape-0.7.3/griptape/schemas/rule_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.7.3/griptape/schemas/structures/__init__.py
--rw-r--r--   0        0        0      359 2023-04-24 15:58:13.306117 griptape-0.7.3/griptape/schemas/structures/agent_schema.py
--rw-r--r--   0        0        0      303 2023-04-23 17:06:19.926957 griptape-0.7.3/griptape/schemas/structures/pipeline_schema.py
--rw-r--r--   0        0        0      510 2023-04-23 21:55:48.267318 griptape-0.7.3/griptape/schemas/structures/structure_schema.py
--rw-r--r--   0        0        0      257 2023-04-23 17:06:20.071895 griptape-0.7.3/griptape/schemas/structures/workflow_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.7.3/griptape/schemas/summarizers/__init__.py
--rw-r--r--   0        0        0      352 2023-04-24 18:12:25.646263 griptape-0.7.3/griptape/schemas/summarizers/prompt_driver_summarizer_schema.py
--rw-r--r--   0        0        0      290 2023-04-23 17:06:19.918871 griptape-0.7.3/griptape/schemas/summarizers/summarizer_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070339 griptape-0.7.3/griptape/schemas/tasks/__init__.py
--rw-r--r--   0        0        0      455 2023-04-23 21:55:48.293447 griptape-0.7.3/griptape/schemas/tasks/prompt_task_schema.py
--rw-r--r--   0        0        0      467 2023-04-23 21:55:48.265710 griptape-0.7.3/griptape/schemas/tasks/task_schema.py
--rw-r--r--   0        0        0      563 2023-04-23 22:36:52.428763 griptape-0.7.3/griptape/schemas/tasks/toolkit_task_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape-0.7.3/griptape/schemas/tokenizers/__init__.py
--rw-r--r--   0        0        0      341 2023-04-24 18:12:25.660055 griptape-0.7.3/griptape/schemas/tokenizers/tiktoken_tokenizer_schema.py
--rw-r--r--   0        0        0      374 2023-04-23 23:11:51.760187 griptape-0.7.3/griptape/structures/__init__.py
--rw-r--r--   0        0        0     2000 2023-04-24 16:10:53.941335 griptape-0.7.3/griptape/structures/agent.py
--rw-r--r--   0        0        0     2890 2023-04-30 17:35:28.986270 griptape-0.7.3/griptape/structures/pipeline.py
--rw-r--r--   0        0        0     4369 2023-04-30 19:31:02.389059 griptape-0.7.3/griptape/structures/structure.py
--rw-r--r--   0        0        0     1397 2023-04-23 23:24:38.546649 griptape-0.7.3/griptape/structures/structure_with_memory.py
--rw-r--r--   0        0        0     3052 2023-04-30 17:35:29.008055 griptape-0.7.3/griptape/structures/workflow.py
--rw-r--r--   0        0        0      210 2023-04-30 17:43:48.623726 griptape-0.7.3/griptape/summarizers/__init__.py
--rw-r--r--   0        0        0      535 2023-04-30 17:51:16.195968 griptape-0.7.3/griptape/summarizers/base_summarizer.py
--rw-r--r--   0        0        0     1397 2023-05-03 17:48:19.079278 griptape-0.7.3/griptape/summarizers/prompt_driver_summarizer.py
--rw-r--r--   0        0        0      292 2023-04-27 20:37:15.607423 griptape-0.7.3/griptape/tasks/__init__.py
--rw-r--r--   0        0        0     8697 2023-04-30 19:34:32.449147 griptape-0.7.3/griptape/tasks/action_subtask.py
--rw-r--r--   0        0        0     3751 2023-04-30 17:35:28.970533 griptape-0.7.3/griptape/tasks/base_task.py
--rw-r--r--   0        0        0     1677 2023-04-30 17:35:29.009441 griptape-0.7.3/griptape/tasks/prompt_task.py
--rw-r--r--   0        0        0     3705 2023-04-30 19:31:02.377122 griptape-0.7.3/griptape/tasks/toolkit_task.py
--rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape-0.7.3/griptape/templates/converters/chatgpt_plugin/ai-plugin.json.j2
--rw-r--r--   0        0        0       76 2023-04-24 15:53:53.079453 griptape-0.7.3/griptape/templates/prompts/agent.j2
--rw-r--r--   0        0        0     2165 2023-05-03 17:16:51.696175 griptape-0.7.3/griptape/templates/prompts/base.j2
--rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 griptape-0.7.3/griptape/templates/prompts/memory.j2
--rw-r--r--   0        0        0      150 2023-04-23 21:55:48.282971 griptape-0.7.3/griptape/templates/prompts/pipeline.j2
--rw-r--r--   0        0        0      351 2023-04-30 19:31:02.380912 griptape-0.7.3/griptape/templates/prompts/ramp.j2
--rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 griptape-0.7.3/griptape/templates/prompts/run.j2
--rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 griptape-0.7.3/griptape/templates/prompts/summarize.j2
--rw-r--r--   0        0        0      114 2023-04-24 16:10:53.946250 griptape-0.7.3/griptape/templates/prompts/tasks/prompt.j2
--rw-r--r--   0        0        0      175 2023-04-23 22:36:52.418559 griptape-0.7.3/griptape/templates/prompts/tasks/tool/subtask.j2
--rw-r--r--   0        0        0       64 2023-04-23 22:36:52.419627 griptape-0.7.3/griptape/templates/prompts/tasks/tool/subtasks.j2
--rw-r--r--   0        0        0      179 2023-04-24 16:10:53.954014 griptape-0.7.3/griptape/templates/prompts/tasks/tool/tool.j2
--rw-r--r--   0        0        0      351 2023-04-28 16:20:57.373167 griptape-0.7.3/griptape/templates/prompts/tool.j2
--rw-r--r--   0        0        0       40 2023-04-23 22:01:47.862316 griptape-0.7.3/griptape/templates/prompts/workflow.j2
--rw-r--r--   0        0        0      111 2023-04-30 19:36:10.118646 griptape-0.7.3/griptape/templates/ramps/storage.j2
--rw-r--r--   0        0        0      383 2023-04-24 18:12:25.639754 griptape-0.7.3/griptape/tokenizers/__init__.py
--rw-r--r--   0        0        0      730 2023-04-20 15:52:25.871234 griptape-0.7.3/griptape/tokenizers/base_tokenizer.py
--rw-r--r--   0        0        0      683 2023-04-24 18:12:25.672520 griptape-0.7.3/griptape/tokenizers/cohere_tokenizer.py
--rw-r--r--   0        0        0      674 2023-04-24 18:12:25.648974 griptape-0.7.3/griptape/tokenizers/hugging_face_tokenizer.py
--rw-r--r--   0        0        0     1448 2023-04-24 18:12:25.673513 griptape-0.7.3/griptape/tokenizers/tiktoken_tokenizer.py
--rw-r--r--   0        0        0      463 2023-04-27 20:13:16.215797 griptape-0.7.3/griptape/utils/__init__.py
--rw-r--r--   0        0        0      567 2023-04-30 20:59:42.640287 griptape-0.7.3/griptape/utils/command_runner.py
--rw-r--r--   0        0        0      509 2023-04-23 22:46:42.637126 griptape-0.7.3/griptape/utils/conversation.py
--rw-r--r--   0        0        0      857 2023-04-23 21:18:54.936489 griptape-0.7.3/griptape/utils/j2.py
--rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape-0.7.3/griptape/utils/manifest_validator.py
--rw-r--r--   0        0        0      206 2023-04-23 21:20:43.200189 griptape-0.7.3/griptape/utils/paths.py
--rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape-0.7.3/griptape/utils/python_runner.py
--rw-r--r--   0        0        0     1142 2023-05-03 17:50:11.229029 griptape-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     5999 1970-01-01 00:00:00.000000 griptape-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4512 2023-05-10 20:52:11.444133 griptape-0.8.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-24 19:02:26.305879 griptape-0.8.0/griptape/__init__.py
+-rw-r--r--   0        0        0      486 2023-05-10 16:01:15.657261 griptape-0.8.0/griptape/artifacts/__init__.py
+-rw-r--r--   0        0        0     1385 2023-05-10 16:17:57.768622 griptape-0.8.0/griptape/artifacts/base_artifact.py
+-rw-r--r--   0        0        0      799 2023-05-10 17:33:20.087370 griptape-0.8.0/griptape/artifacts/blob_artifact.py
+-rw-r--r--   0        0        0      359 2023-05-09 18:59:20.776163 griptape-0.8.0/griptape/artifacts/error_artifact.py
+-rw-r--r--   0        0        0      356 2023-05-10 16:01:15.661516 griptape-0.8.0/griptape/artifacts/info_artifact.py
+-rw-r--r--   0        0        0      615 2023-05-10 16:15:07.936323 griptape-0.8.0/griptape/artifacts/list_artifact.py
+-rw-r--r--   0        0        0      512 2023-05-09 18:59:20.786810 griptape-0.8.0/griptape/artifacts/text_artifact.py
+-rw-r--r--   0        0        0      126 2023-05-03 20:08:48.695610 griptape-0.8.0/griptape/core/__init__.py
+-rw-r--r--   0        0        0     3903 2023-05-10 19:30:09.375192 griptape-0.8.0/griptape/core/activity_mixin.py
+-rw-r--r--   0        0        0     4423 2023-05-10 20:24:20.848612 griptape-0.8.0/griptape/core/base_tool.py
+-rw-r--r--   0        0        0     1031 2023-05-10 16:50:18.389653 griptape-0.8.0/griptape/core/decorators.py
+-rw-r--r--   0        0        0     1376 2023-05-09 17:14:35.965124 griptape-0.8.0/griptape/drivers/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 griptape-0.8.0/griptape/drivers/memory/__init__.py
+-rw-r--r--   0        0        0      555 2023-04-24 18:12:25.623896 griptape-0.8.0/griptape/drivers/memory/disk_memory_driver.py
+-rw-r--r--   0        0        0      238 2023-04-23 22:46:42.644482 griptape-0.8.0/griptape/drivers/memory/memory_driver.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 griptape-0.8.0/griptape/drivers/prompt/__init__.py
+-rw-r--r--   0        0        0     1084 2023-05-03 19:38:21.133715 griptape-0.8.0/griptape/drivers/prompt/base_prompt_driver.py
+-rw-r--r--   0        0        0     1279 2023-04-30 17:35:29.003157 griptape-0.8.0/griptape/drivers/prompt/cohere_prompt_driver.py
+-rw-r--r--   0        0        0     1956 2023-04-30 17:35:29.016094 griptape-0.8.0/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py
+-rw-r--r--   0        0        0     1733 2023-04-30 17:35:29.013147 griptape-0.8.0/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py
+-rw-r--r--   0        0        0     2711 2023-04-30 17:35:28.955013 griptape-0.8.0/griptape/drivers/prompt/openai_prompt_driver.py
+-rw-r--r--   0        0        0        0 2023-04-27 20:13:16.212093 griptape-0.8.0/griptape/drivers/storage/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:43:06.908509 griptape-0.8.0/griptape/drivers/storage/blob/__init__.py
+-rw-r--r--   0        0        0      417 2023-05-09 17:07:04.025663 griptape-0.8.0/griptape/drivers/storage/blob/base_blob_storage_driver.py
+-rw-r--r--   0        0        0      762 2023-05-09 17:07:04.028021 griptape-0.8.0/griptape/drivers/storage/blob/memory_blob_storage_driver.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:04:11.435219 griptape-0.8.0/griptape/drivers/storage/text/__init__.py
+-rw-r--r--   0        0        0      434 2023-05-10 20:05:06.365336 griptape-0.8.0/griptape/drivers/storage/text/base_text_storage_driver.py
+-rw-r--r--   0        0        0     1373 2023-05-09 16:05:38.013785 griptape-0.8.0/griptape/drivers/storage/text/dynamodb_text_storage_driver.py
+-rw-r--r--   0        0        0      569 2023-05-09 17:14:35.966970 griptape-0.8.0/griptape/drivers/storage/text/memory_text_storage_driver.py
+-rw-r--r--   0        0        0      203 2023-04-23 17:45:35.150209 griptape-0.8.0/griptape/executors/__init__.py
+-rw-r--r--   0        0        0     1941 2023-05-09 21:53:42.521962 griptape-0.8.0/griptape/executors/base_executor.py
+-rw-r--r--   0        0        0     3304 2023-05-08 20:16:06.614331 griptape-0.8.0/griptape/executors/docker_executor.py
+-rw-r--r--   0        0        0     2205 2023-05-08 17:11:25.159107 griptape-0.8.0/griptape/executors/local_executor.py
+-rw-r--r--   0        0        0      271 2023-04-24 16:31:58.604436 griptape-0.8.0/griptape/memory/__init__.py
+-rw-r--r--   0        0        0      779 2023-05-09 18:59:20.783209 griptape-0.8.0/griptape/memory/buffer_memory.py
+-rw-r--r--   0        0        0     1764 2023-05-09 18:59:20.785081 griptape-0.8.0/griptape/memory/memory.py
+-rw-r--r--   0        0        0      360 2023-04-23 22:49:52.124272 griptape-0.8.0/griptape/memory/run.py
+-rw-r--r--   0        0        0     2105 2023-05-09 18:59:20.779182 griptape-0.8.0/griptape/memory/summary_memory.py
+-rw-r--r--   0        0        0      203 2023-05-09 21:24:07.655284 griptape-0.8.0/griptape/ramps/__init__.py
+-rw-r--r--   0        0        0     1541 2023-05-09 19:44:03.721738 griptape-0.8.0/griptape/ramps/base_ramp.py
+-rw-r--r--   0        0        0     1333 2023-05-10 18:51:24.674178 griptape-0.8.0/griptape/ramps/blob_storage_ramp.py
+-rw-r--r--   0        0        0     1505 2023-05-10 19:56:50.754286 griptape-0.8.0/griptape/ramps/text_storage_ramp.py
+-rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape-0.8.0/griptape/resources/docker_executor/Dockerfile
+-rw-r--r--   0        0        0       64 2023-05-05 15:39:50.489813 griptape-0.8.0/griptape/rules/__init__.py
+-rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 griptape-0.8.0/griptape/rules/rule.py
+-rw-r--r--   0        0        0      144 2023-05-05 15:39:50.487681 griptape-0.8.0/griptape/rules/ruleset.py
+-rw-r--r--   0        0        0     1165 2023-05-10 16:03:43.577569 griptape-0.8.0/griptape/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape-0.8.0/griptape/schemas/artifacts/__init__.py
+-rw-r--r--   0        0        0      275 2023-05-10 16:34:41.421057 griptape-0.8.0/griptape/schemas/artifacts/artifact_schema.py
+-rw-r--r--   0        0        0      409 2023-05-07 16:29:29.348073 griptape-0.8.0/griptape/schemas/artifacts/blob_artifact_schema.py
+-rw-r--r--   0        0        0      303 2023-05-06 19:49:43.542366 griptape-0.8.0/griptape/schemas/artifacts/error_artifact_schema.py
+-rw-r--r--   0        0        0      300 2023-05-09 21:33:24.929758 griptape-0.8.0/griptape/schemas/artifacts/info_artifact_schema.py
+-rw-r--r--   0        0        0      354 2023-05-10 16:16:15.649988 griptape-0.8.0/griptape/schemas/artifacts/list_artifact_schema.py
+-rw-r--r--   0        0        0      300 2023-05-06 19:49:43.546323 griptape-0.8.0/griptape/schemas/artifacts/text_artifact_schema.py
+-rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 griptape-0.8.0/griptape/schemas/base_schema.py
+-rw-r--r--   0        0        0        0 2023-05-03 19:15:12.616328 griptape-0.8.0/griptape/schemas/memory/__init__.py
+-rw-r--r--   0        0        0      299 2023-05-03 19:35:36.457310 griptape-0.8.0/griptape/schemas/memory/buffer_memory_schema.py
+-rw-r--r--   0        0        0      372 2023-05-10 16:35:39.384699 griptape-0.8.0/griptape/schemas/memory/memory_schema.py
+-rw-r--r--   0        0        0      350 2023-05-03 19:15:12.616696 griptape-0.8.0/griptape/schemas/memory/run_schema.py
+-rw-r--r--   0        0        0      372 2023-05-03 19:44:56.927223 griptape-0.8.0/griptape/schemas/memory/summary_memory_schema.py
+-rw-r--r--   0        0        0     5937 2023-04-23 17:06:19.960660 griptape-0.8.0/griptape/schemas/polymorphic_schema.py
+-rw-r--r--   0        0        0      374 2023-04-23 23:11:51.760187 griptape-0.8.0/griptape/structures/__init__.py
+-rw-r--r--   0        0        0     1586 2023-05-06 17:03:28.908015 griptape-0.8.0/griptape/structures/agent.py
+-rw-r--r--   0        0        0     2608 2023-05-06 20:59:22.417687 griptape-0.8.0/griptape/structures/pipeline.py
+-rw-r--r--   0        0        0     3843 2023-05-05 19:11:47.106450 griptape-0.8.0/griptape/structures/structure.py
+-rw-r--r--   0        0        0     1397 2023-04-23 23:24:38.546649 griptape-0.8.0/griptape/structures/structure_with_memory.py
+-rw-r--r--   0        0        0     2762 2023-05-06 20:59:22.418183 griptape-0.8.0/griptape/structures/workflow.py
+-rw-r--r--   0        0        0      210 2023-04-30 17:43:48.623726 griptape-0.8.0/griptape/summarizers/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-03 19:38:21.128646 griptape-0.8.0/griptape/summarizers/base_summarizer.py
+-rw-r--r--   0        0        0     1401 2023-05-06 17:03:28.895388 griptape-0.8.0/griptape/summarizers/prompt_driver_summarizer.py
+-rw-r--r--   0        0        0      292 2023-04-27 20:37:15.607423 griptape-0.8.0/griptape/tasks/__init__.py
+-rw-r--r--   0        0        0     8844 2023-05-10 19:30:09.377690 griptape-0.8.0/griptape/tasks/action_subtask.py
+-rw-r--r--   0        0        0     3806 2023-05-06 20:59:22.418476 griptape-0.8.0/griptape/tasks/base_task.py
+-rw-r--r--   0        0        0     1768 2023-05-07 22:44:27.768175 griptape-0.8.0/griptape/tasks/prompt_task.py
+-rw-r--r--   0        0        0     3642 2023-05-06 22:13:05.957939 griptape-0.8.0/griptape/tasks/toolkit_task.py
+-rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape-0.8.0/griptape/templates/converters/chatgpt_plugin/ai-plugin.json.j2
+-rw-r--r--   0        0        0       76 2023-04-24 15:53:53.079453 griptape-0.8.0/griptape/templates/prompts/agent.j2
+-rw-r--r--   0        0        0     2318 2023-05-09 19:10:52.013387 griptape-0.8.0/griptape/templates/prompts/base.j2
+-rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 griptape-0.8.0/griptape/templates/prompts/memory.j2
+-rw-r--r--   0        0        0      150 2023-04-23 21:55:48.282971 griptape-0.8.0/griptape/templates/prompts/pipeline.j2
+-rw-r--r--   0        0        0      482 2023-05-05 19:11:47.103721 griptape-0.8.0/griptape/templates/prompts/ramp.j2
+-rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 griptape-0.8.0/griptape/templates/prompts/run.j2
+-rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 griptape-0.8.0/griptape/templates/prompts/summarize.j2
+-rw-r--r--   0        0        0      122 2023-05-06 17:03:28.894137 griptape-0.8.0/griptape/templates/prompts/tasks/prompt.j2
+-rw-r--r--   0        0        0      179 2023-05-06 17:03:28.912824 griptape-0.8.0/griptape/templates/prompts/tasks/tool/subtask.j2
+-rw-r--r--   0        0        0       64 2023-04-23 22:36:52.419627 griptape-0.8.0/griptape/templates/prompts/tasks/tool/subtasks.j2
+-rw-r--r--   0        0        0      187 2023-05-06 17:03:28.888976 griptape-0.8.0/griptape/templates/prompts/tasks/tool/tool.j2
+-rw-r--r--   0        0        0      482 2023-05-05 19:11:47.105201 griptape-0.8.0/griptape/templates/prompts/tool.j2
+-rw-r--r--   0        0        0       40 2023-04-23 22:01:47.862316 griptape-0.8.0/griptape/templates/prompts/workflow.j2
+-rw-r--r--   0        0        0      131 2023-05-10 18:51:24.681023 griptape-0.8.0/griptape/templates/ramps/blob_storage.j2
+-rw-r--r--   0        0        0      131 2023-05-10 18:51:24.678788 griptape-0.8.0/griptape/templates/ramps/text_storage.j2
+-rw-r--r--   0        0        0      383 2023-04-24 18:12:25.639754 griptape-0.8.0/griptape/tokenizers/__init__.py
+-rw-r--r--   0        0        0      730 2023-04-20 15:52:25.871234 griptape-0.8.0/griptape/tokenizers/base_tokenizer.py
+-rw-r--r--   0        0        0      683 2023-04-24 18:12:25.672520 griptape-0.8.0/griptape/tokenizers/cohere_tokenizer.py
+-rw-r--r--   0        0        0      674 2023-04-24 18:12:25.648974 griptape-0.8.0/griptape/tokenizers/hugging_face_tokenizer.py
+-rw-r--r--   0        0        0     1448 2023-04-24 18:12:25.673513 griptape-0.8.0/griptape/tokenizers/tiktoken_tokenizer.py
+-rw-r--r--   0        0        0      463 2023-04-27 20:13:16.215797 griptape-0.8.0/griptape/utils/__init__.py
+-rw-r--r--   0        0        0      567 2023-04-30 20:59:42.640287 griptape-0.8.0/griptape/utils/command_runner.py
+-rw-r--r--   0        0        0      509 2023-04-23 22:46:42.637126 griptape-0.8.0/griptape/utils/conversation.py
+-rw-r--r--   0        0        0      857 2023-04-23 21:18:54.936489 griptape-0.8.0/griptape/utils/j2.py
+-rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape-0.8.0/griptape/utils/manifest_validator.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:56:24.051141 griptape-0.8.0/griptape/utils/marshmallow/__init__.py
+-rw-r--r--   0        0        0       52 2023-05-06 19:58:37.405568 griptape-0.8.0/griptape/utils/marshmallow/fields/__init__.py
+-rw-r--r--   0        0        0      422 2023-05-06 20:47:07.097992 griptape-0.8.0/griptape/utils/marshmallow/fields/bytes.py
+-rw-r--r--   0        0        0      206 2023-04-23 21:20:43.200189 griptape-0.8.0/griptape/utils/paths.py
+-rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape-0.8.0/griptape/utils/python_runner.py
+-rw-r--r--   0        0        0     1118 2023-05-10 20:52:58.474188 griptape-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5889 1970-01-01 00:00:00.000000 griptape-0.8.0/PKG-INFO
```

### Comparing `griptape-0.7.3/LICENSE` & `griptape-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape-0.7.3/README.md` & `griptape-0.8.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io/)
 [![Griptape Discord](https://dcbadge.vercel.app/api/server/gnWRz88eym?compact=true&style=flat)](https://discord.gg/gnWRz88eym)
 
 **griptape** is a modular Python framework for LLM workflows, tools, memory, and data that enables developers to:
 
 1. 🤖 Build **AI agents**, sequential **LLM pipelines** and sprawling **DAG workflows** for complex use cases.
 2. ⛓️ Augment LLMs with **chain of thought** capabilities.
-3. 🧰️ Integrate other services and functionality into LLMs as [tools](https://github.com/griptape-ai/griptape-tools) (e.g., calculators, web scrapers, spreadsheet editors, and API connectors); run tools in any environment (local, containerized, cloud, etc.); use tools directly in **griptape** or convert them into ramps abstractions, such as ChatGPT Plugins, LangChain tools, or Fixie.ai agents.
+3. 🧰️ Integrate other services and functionality into LLMs as [tools](https://github.com/griptape-ai/griptape-tools) (e.g., calculators, web scrapers, spreadsheet editors, and API connectors); run tools in any environment (local, containerized, cloud, etc.); and wrap tools with off prompt data storage that prevents LLMs from accessing your data directly.
 4. 💾 Add **memory** to AI pipelines for context preservation and summarization.
 
 ## Documentation
 
 Please refer to [Griptape Docs](https://griptape.readthedocs.io) for:
 
 - Getting started guides. 
@@ -27,72 +27,77 @@
 
 ```
 pip install griptape griptape-tools -U
 ```
 
 Second, configure an OpenAI client by [getting an API key](https://beta.openai.com/account/api-keys) and adding it to your environment as `OPENAI_API_KEY`. griptape uses [OpenAI Completions API](https://platform.openai.com/docs/guides/completion) to execute LLM prompts and to work with [LlamaIndex](https://gpt-index.readthedocs.io/en/latest/index.html) data structures.
 
-With **griptape**, you can create *structures*, such as `Agents`, `Pipelines`, and `Workflows`, that are composed of different types of tasks. You can also define structures as JSON objects and load them into **griptape** dynamically. Let's define a simple two-task pipeline that uses tools:
+With **griptape**, you can create *structures*, such as `Agents`, `Pipelines`, and `Workflows`, that are composed of different types of tasks. You can also define structures as JSON objects and load them into **griptape** dynamically. Let's define a simple two-task pipeline that uses tools and ramps:
 
 ```python
-from decouple import config
-from griptape.core import ToolLoader
-from griptape.drivers import OpenAiPromptDriver, MemoryStorageDriver
-from griptape.executors import LocalExecutor
 from griptape.memory import Memory
-from griptape.ramps import StorageRamp
+from griptape.ramps import TextStorageRamp, BlobStorageRamp
 from griptape.structures import Pipeline
 from griptape.tasks import ToolkitTask, PromptTask
-from griptape.tools import WebScraper
+from griptape.tools import WebScraper, TextProcessor, FileManager
 
-storage = StorageRamp(
-    driver=MemoryStorageDriver()
+# Ramps enable LLMs to store and manipulate data without ever looking at it directly.
+text_storage = TextStorageRamp()
+blob_storage = BlobStorageRamp()
+
+# Connect a web scraper to load web pages.
+web_scraper = WebScraper(
+    ramps={
+        "get_content": [text_storage]
+    }
+)
+
+# TextProcessor enables LLMs to summarize and query text.
+text_processor = TextProcessor(
+    ramps={
+        "summarize": [text_storage],
+        "query": [text_storage]
+    }
 )
 
-scraper = WebScraper(
+# File manager can load and store files locally.
+file_manager = FileManager(
     ramps={
-        "get_content": [storage]
+        "load": [blob_storage],
+        "save": [text_storage, blob_storage]
     }
 )
 
+# Pipelines represent sequences of tasks.
 pipeline = Pipeline(
-    memory=Memory(),
-    tool_loader=ToolLoader(
-        tools=[scraper],
-        executor=LocalExecutor()
-    )
+    memory=Memory()
 )
 
 pipeline.add_tasks(
+    # Load up the first argument from `pipeline.run`.
     ToolkitTask(
-        tool_names=[scraper.name]
+        "{{ args[0] }}",
+        tools=[web_scraper, text_processor, file_manager]
     ),
+    # Augment `input` from the previous task.
     PromptTask(
         "Say the following in spanish: {{ input }}"
     )
 )
 
-result = pipeline.run("Give me a summary of https://en.wikipedia.org/wiki/Large_language_model")
-
-print(result.output.value)
-
+result = pipeline.run("Load https://griptape.readthedocs.io, summarize it, and store it in griptape.txt")
 
+print(result.output.to_text())
 ```
 
 Boom! Our first LLM pipeline with two sequential tasks generated the following exchange:
 
 ```
-Q: Give me a summary of https://en.wikipedia.org/wiki/Large_language_model
-[chain of thought output... will vary depending on the model driver you're using]
-A: Los modelos de lenguaje de gran tamaño son herramientas utilizadas para tareas de 
-procesamiento del lenguaje natural, como detectar falsedades, completar oraciones y comprender 
-el lenguaje. Algunos modelos notables incluyen BERT, GPT-2, GPT-3, GPT-Neo y GLaM. The Pile es 
-un conjunto de datos extenso utilizado para el modelado del lenguaje. Estos modelos han sido 
-desarrollados e investigados en trabajos como TruthfulQA, HellaSwag y BERT: Pre-entrenamiento 
-de transformadores bidireccionales profundos para la comprensión del lenguaje.
+Q: Load https://griptape.readthedocs.io, summarize it, and store it in griptape.txt
+A: El contenido de https://griptape.readthedocs.io ha sido resumido y almacenado en griptape.txt.
 ```
 
 ## Versioning
 
 **griptape** is in early development and its APIs and documentation are subject to change. Until we stabilize the API and release version 1.0.0, we will use minor versions (i.e., x.Y.z) to introduce features and breaking features, and patch versions (i.e., x.y.Z) for bug fixes.
 
 ## Contributing
```

### Comparing `griptape-0.7.3/griptape/core/base_tool.py` & `griptape-0.8.0/griptape/core/base_tool.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,44 +5,50 @@
 import os
 from abc import ABC
 from typing import Optional
 import yaml
 from attr import define, fields, Attribute, field, Factory
 import attrs
 from decouple import config
+from griptape.artifacts import BaseArtifact
 from griptape.core import ActivityMixin
 
 if TYPE_CHECKING:
     from griptape.ramps import BaseRamp
 
 
 @define
 class BaseTool(ActivityMixin, ABC):
     MANIFEST_FILE = "manifest.yml"
     DOCKERFILE_FILE = "Dockerfile"
     REQUIREMENTS_FILE = "requirements.txt"
 
     name: str = field(default=Factory(lambda self: self.class_name, takes_self=True), kw_only=True)
     ramps: dict[str, list[BaseRamp]] = field(factory=dict, kw_only=True)
+    artifacts: list[BaseArtifact] = field(factory=list, kw_only=True)
 
     # Disable logging, unless it's an error, so that executors don't capture it as subprocess output.
     logging.basicConfig(level=logging.ERROR)
 
     def __attrs_post_init__(self):
         from griptape.ramps import BaseRamp
 
         # https://www.attrs.org/en/stable/api.html#attrs.resolve_types
         attrs.resolve_types(self.__class__, globals(), locals())
 
     @ramps.validator
     def validate_ramps(self, _, ramps: dict[str, list[BaseRamp]]) -> None:
-        ramp_names = [item.name for sublist in ramps.values() for item in sublist]
+        for activity_name, ramp_list in ramps.items():
+            ramp_names = [ramp.name for ramp in ramp_list]
 
-        if len(ramp_names) > len(set(ramp_names)):
-            raise ValueError("ramp names have to be unique")
+            if not self.find_activity(activity_name):
+                raise ValueError(f"activity {activity_name} doesn't exist")
+
+            if len(ramp_names) > len(set(ramp_names)):
+                raise ValueError(f"ramp names have to be unique in activity {activity_name}")
 
     @property
     def class_name(self):
         return self.__class__.__name__
 
     @property
     def env_fields(self) -> list[Attribute]:
```

### Comparing `griptape-0.7.3/griptape/drivers/__init__.py` & `griptape-0.8.0/griptape/drivers/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 from griptape.drivers.prompt.base_prompt_driver import BasePromptDriver
 from griptape.drivers.prompt.openai_prompt_driver import OpenAiPromptDriver
 from griptape.drivers.prompt.cohere_prompt_driver import CoherePromptDriver
 from griptape.drivers.prompt.hugging_face_pipeline_prompt_driver import HuggingFacePipelinePromptDriver
 from griptape.drivers.prompt.hugging_face_hub_prompt_driver import HuggingFaceHubPromptDriver
+
 from griptape.drivers.memory.memory_driver import MemoryDriver
 from griptape.drivers.memory.disk_memory_driver import DiskMemoryDriver
-from griptape.drivers.storage.base_storage_driver import BaseStorageDriver
-from griptape.drivers.storage.memory_storage_driver import MemoryStorageDriver
-from griptape.drivers.storage.dynamodb_storage_driver import DynamoDbStorageDriver
+
+from griptape.drivers.storage.text.base_text_storage_driver import BaseTextStorageDriver
+from griptape.drivers.storage.text.memory_text_storage_driver import MemoryTextStorageDriver
+from griptape.drivers.storage.text.dynamodb_text_storage_driver import DynamoDbStorageDriver
+
+from griptape.drivers.storage.blob.base_blob_storage_driver import BaseBlobStorageDriver
+from griptape.drivers.storage.blob.memory_blob_storage_driver import MemoryBlobStorageDriver
 
 __all__ = [
     "BasePromptDriver",
     "OpenAiPromptDriver",
     "CoherePromptDriver",
     "HuggingFacePipelinePromptDriver",
     "HuggingFaceHubPromptDriver",
 
     "MemoryDriver",
     "DiskMemoryDriver",
 
-    "BaseStorageDriver",
-    "MemoryStorageDriver",
-    "DynamoDbStorageDriver"
+    "BaseTextStorageDriver",
+    "MemoryTextStorageDriver",
+    "DynamoDbStorageDriver",
+
+    "BaseBlobStorageDriver",
+    "MemoryBlobStorageDriver"
 ]
```

### Comparing `griptape-0.7.3/griptape/drivers/memory/disk_memory_driver.py` & `griptape-0.8.0/griptape/drivers/memory/disk_memory_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.3/griptape/drivers/prompt/base_prompt_driver.py` & `griptape-0.8.0/griptape/drivers/prompt/base_prompt_driver.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     from griptape.artifacts import TextArtifact
 
 
 @define
 class BasePromptDriver(ABC):
     max_retries: int = field(default=8, kw_only=True)
     retry_delay: float = field(default=1, kw_only=True)
-    type: str = field(default=Factory(lambda self: self.__class__.__name__, takes_self=True), kw_only=True)
     temperature: float = field(default=0.5, kw_only=True)
     model: str
     tokenizer: BaseTokenizer
 
     def run(self, **kwargs) -> TextArtifact:
         for attempt in range(0, self.max_retries + 1):
             try:
```

### Comparing `griptape-0.7.3/griptape/drivers/prompt/cohere_prompt_driver.py` & `griptape-0.8.0/griptape/drivers/prompt/cohere_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.3/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py` & `griptape-0.8.0/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.3/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py` & `griptape-0.8.0/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.3/griptape/drivers/prompt/openai_prompt_driver.py` & `griptape-0.8.0/griptape/drivers/prompt/openai_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.3/griptape/drivers/storage/dynamodb_storage_driver.py` & `griptape-0.8.0/griptape/drivers/storage/text/dynamodb_text_storage_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from uuid import uuid4
 from typing import Optional
 from boto3 import resource
 from attr import define, field
-from griptape.drivers import BaseStorageDriver
+from griptape.drivers import BaseTextStorageDriver
 
 
 @define
-class DynamoDbStorageDriver(BaseStorageDriver):
+class DynamoDbStorageDriver(BaseTextStorageDriver):
     aws_region: str = field(default=None, kw_only=True)
     table_name: str = field(default=None, kw_only=True)
     partition_key: str = field(default=None, kw_only=True)
     value_attribute_key: str = field(default=None, kw_only=True)
     extra_attributes: any = field(default={}, kw_only=True)
 
     table: any = field(init=False)
```

### Comparing `griptape-0.7.3/griptape/drivers/storage/memory_storage_driver.py` & `griptape-0.8.0/griptape/drivers/storage/text/memory_text_storage_driver.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import uuid
 from typing import Optional
-from griptape.drivers import BaseStorageDriver
+from griptape.drivers import BaseTextStorageDriver
 from attr import define, field
 
 
 @define
-class MemoryStorageDriver(BaseStorageDriver):
+class MemoryTextStorageDriver(BaseTextStorageDriver):
     memory: dict[str, any] = field(factory=dict, kw_only=True)
 
     def save(self, value: any) -> str:
         key = uuid.uuid4().hex
 
         self.memory[key] = value
```

### Comparing `griptape-0.7.3/griptape/executors/base_executor.py` & `griptape-0.8.0/griptape/executors/base_executor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from __future__ import annotations
 import json
 import logging
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Union, Optional
 import inspect
 import os
 from abc import ABC, abstractmethod
-from griptape.artifacts import BaseArtifact, TextArtifact
+from griptape.artifacts import BaseArtifact, InfoArtifact
 
 if TYPE_CHECKING:
     from griptape.core import BaseTool
 
 
 class BaseExecutor(ABC):
-    def execute(self, tool_activity: callable, value: BaseArtifact) -> BaseArtifact:
-        result = self.before_execute(tool_activity, value)
-        result = self.executor_result_to_artifact(
-            self.try_execute(tool_activity, result)
+    def execute(self, tool_activity: callable, value: Optional[dict]) -> BaseArtifact:
+        preprocessed_value = self.before_execute(tool_activity, value)
+
+        artifact = self.executor_result_to_artifact(
+            self.try_execute(tool_activity, preprocessed_value)
         )
-        result = self.after_execute(tool_activity, result)
 
-        return result
+        return self.after_execute(tool_activity, artifact)
 
-    def before_execute(self, tool_activity: callable, value: BaseArtifact) -> BaseArtifact:
-        for ramps in tool_activity.__self__.ramps.get(tool_activity.config["name"], []):
-            value = ramps.process_input(tool_activity, value)
+    def before_execute(self, tool_activity: callable, value: Optional[dict]) -> Optional[dict]:
+        for ramp in tool_activity.__self__.ramps.get(tool_activity.config["name"], []):
+            value = ramp.process_input(tool_activity, value)
 
         return value
 
-    def after_execute(self, tool_activity: callable, value: BaseArtifact) -> BaseArtifact:
-        for ramps in tool_activity.__self__.ramps.get(tool_activity.config["name"], []):
-            value = ramps.process_output(tool_activity, value)
+    def after_execute(self, tool_activity: callable, value: Optional[BaseArtifact]) -> BaseArtifact:
+        for ramp in tool_activity.__self__.ramps.get(tool_activity.config["name"], []):
+            value = ramp.process_output(tool_activity, value)
 
         return value
 
+    @abstractmethod
+    def try_execute(self, tool_activity: callable, value: Optional[dict]) -> Union[BaseArtifact, str]:
+        ...
+
     def executor_result_to_artifact(self, result: Union[BaseArtifact, str]) -> BaseArtifact:
         if isinstance(result, BaseArtifact):
             return result
         else:
             try:
                 return BaseArtifact.from_dict(json.loads(result))
             except Exception:
-                logging.exception("Error converting executor result to an artifact; defaulting to TextArtifact")
+                logging.error("Error converting executor result to an artifact; defaulting to InfoArtifact")
 
-                return TextArtifact(result)
-
-    @abstractmethod
-    def try_execute(self, tool_activity: callable, value: BaseArtifact) -> Union[BaseArtifact, str]:
-        ...
+                return InfoArtifact(result)
 
     def tool_dir(self, tool: BaseTool):
         class_file = inspect.getfile(tool.__class__)
 
         return os.path.dirname(os.path.abspath(class_file))
```

### Comparing `griptape-0.7.3/griptape/executors/docker_executor.py` & `griptape-0.8.0/griptape/executors/docker_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Union
 import logging
 from typing import Optional
 from attr import define, field, Factory
 import docker
 from docker.errors import NotFound
-from griptape.artifacts import BaseArtifact, TextArtifact
+from griptape.artifacts import BaseArtifact
 from griptape.utils.paths import abs_path
 from griptape.executors import BaseExecutor
 import stringcase
 import tempfile
 import shutil
 import os
 
@@ -29,31 +29,31 @@
         try:
             return docker.from_env()
         except Exception as e:
             logging.error(e)
 
             return None
 
-    def try_execute(self, tool_activity: callable, value: BaseArtifact) -> Union[BaseArtifact, str]:
+    def try_execute(self, tool_activity: callable, value: Optional[dict]) -> Union[BaseArtifact, str]:
         tool = tool_activity.__self__
 
         self.build_image(tool)
         self.remove_existing_container(self.container_name(tool))
 
-        return self.run_container(tool_activity, value.value)
+        return self.run_container(tool_activity, value)
 
-    def run_container(self, tool_activity: callable, value: any) -> str:
+    def run_container(self, tool_activity: callable, value: Optional[dict]) -> str:
         tool = tool_activity.__self__
         workdir = "/tool"
         tool_name = tool.class_name
-        value = f'"{value}"' if isinstance(value, str) else value
+        input_value = value if value else ""
         command = [
             "python",
             "-c",
-            f'from tool import {tool_name}; print({tool_name}().{tool_activity.__name__}({value}))'
+            f'from tool import {tool_name}; print({tool_name}().{tool_activity.__name__}({input_value}))'
         ]
         binds = {
             self.tool_dir(tool): {
                 "bind": workdir,
                 "mode": "rw"
             }
         }
```

### Comparing `griptape-0.7.3/griptape/executors/local_executor.py` & `griptape-0.8.0/griptape/executors/local_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from __future__ import annotations
 import logging
 import os
 import subprocess
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Union, Optional
 from attr import define, field
 from griptape.artifacts import BaseArtifact, ErrorArtifact, TextArtifact
 from griptape.executors import BaseExecutor
 
 if TYPE_CHECKING:
     from griptape.core import BaseTool
 
 
 @define
 class LocalExecutor(BaseExecutor):
     verbose: int = field(default=False, kw_only=True)
 
-    def try_execute(self, tool_activity: callable, value: BaseArtifact) -> Union[BaseArtifact, str]:
+    def try_execute(self, tool_activity: callable, value: Optional[dict]) -> Union[BaseArtifact, str]:
         tool = tool_activity.__self__
 
         logging.warning(f"You are executing the {tool.name} tool in the local environment. Make sure to "
                         f"switch to a more secure ToolExecutor in production.")
 
         env = os.environ.copy()
 
         env.update(tool.env)
 
         self.install_dependencies(env, tool)
 
-        output = self.run_subprocess(env, tool_activity, value.value)
+        output = self.run_subprocess(env, tool_activity, value)
 
         if output.stderr and not output.stdout:
             return ErrorArtifact(output.stderr.strip())
         else:
             return output.stdout.strip()
 
     def install_dependencies(self, env: dict[str, str], tool: BaseTool) -> None:
@@ -48,22 +48,22 @@
             command,
             env=env,
             cwd=self.tool_dir(tool),
             stdout=None if self.verbose else subprocess.DEVNULL,
             stderr=None if self.verbose else subprocess.DEVNULL
         )
 
-    def run_subprocess(self, env: dict[str, str], tool_activity: callable, value: any) -> subprocess.CompletedProcess:
+    def run_subprocess(self, env: dict[str, str], tool_activity: callable, value: Optional[dict]) -> subprocess.CompletedProcess:
         tool = tool_activity.__self__
         tool_name = tool.class_name
-        value = f'"{value}"' if isinstance(value, str) else value
+        input_value = value if value else ""
         command = [
             "python",
             "-c",
-            f'from tool import {tool_name}; print({tool_name}().{tool_activity.__name__}({value}))'
+            f'from tool import {tool_name}; print({tool_name}().{tool_activity.__name__}({input_value}))'
         ]
 
         return subprocess.run(
             command,
             env=env,
             cwd=self.tool_dir(tool),
             capture_output=True,
```

### Comparing `griptape-0.7.3/griptape/memory/memory.py` & `griptape-0.8.0/griptape/memory/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     def to_json(self) -> str:
         return json.dumps(self.to_dict(), indent=2)
 
     def to_dict(self) -> dict:
         from griptape.schemas import MemorySchema
 
-        return MemorySchema().dump(self)
+        return dict(MemorySchema().dump(self))
 
     @classmethod
     def from_dict(cls, memory_dict: dict) -> Memory:
         from griptape.schemas import MemorySchema
 
         return MemorySchema().load(memory_dict)
```

### Comparing `griptape-0.7.3/griptape/memory/summary_memory.py` & `griptape-0.8.0/griptape/memory/summary_memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 import json
 from typing import TYPE_CHECKING
 from typing import Optional
 from attr import define, field
+from griptape.schemas import SummaryMemorySchema
 from griptape.utils import J2
 from griptape.memory import Memory
 
 if TYPE_CHECKING:
     from griptape.summarizers import BaseSummarizer
     from griptape.memory import Run
 
@@ -45,16 +46,16 @@
     def to_prompt_string(self, last_n: Optional[int] = None):
         return J2("prompts/memory.j2").render(
             summary=self.summary,
             runs=self.unsummarized_runs(last_n)
         )
 
     def to_dict(self) -> dict:
-        return SummaryMemory().dump(self)
+        return dict(SummaryMemorySchema().dump(self))
 
     @classmethod
-    def from_dict(cls, memory_dict: dict) -> Memory:
-        return SummaryMemory().load(memory_dict)
+    def from_dict(cls, memory_dict: dict) -> SummaryMemory:
+        return SummaryMemorySchema().load(memory_dict)
 
     @classmethod
-    def from_json(cls, memory_json: str) -> Memory:
+    def from_json(cls, memory_json: str) -> SummaryMemory:
         return SummaryMemory.from_dict(json.loads(memory_json))
```

### Comparing `griptape-0.7.3/griptape/schemas/polymorphic_schema.py` & `griptape-0.8.0/griptape/schemas/polymorphic_schema.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.3/griptape/structures/agent.py` & `griptape-0.8.0/griptape/structures/agent.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from __future__ import annotations
-import json
 from typing import TYPE_CHECKING
 from attr import define, field
 from griptape.memory import Run
 from griptape.structures import StructureWithMemory
 from griptape.tasks import PromptTask
 from griptape.utils import J2
 
@@ -49,31 +48,16 @@
 
         self.task.reset()
 
         self.task.execute()
 
         if self.memory:
             run = Run(
-                input=self.task.input.value,
-                output=self.task.output.value
+                input=self.task.input.to_text(),
+                output=self.task.output.to_text()
             )
 
             self.memory.add_run(run)
 
         self._execution_args = ()
 
         return self.task
-
-    def to_dict(self) -> dict:
-        from griptape.schemas import AgentSchema
-
-        return AgentSchema().dump(self)
-
-    @classmethod
-    def from_dict(cls, agent_dict: dict) -> Agent:
-        from griptape.schemas import AgentSchema
-
-        return AgentSchema().load(agent_dict)
-
-    @classmethod
-    def from_json(cls, agent_json: str) -> Agent:
-        return Agent.from_dict(json.loads(agent_json))
```

### Comparing `griptape-0.7.3/griptape/structures/pipeline.py` & `griptape-0.8.0/griptape/structures/pipeline.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 
     def last_task(self) -> Optional[BaseTask]:
         return self.tasks[-1] if self.tasks else None
 
     def finished_tasks(self) -> list[BaseTask]:
         return [s for s in self.tasks if s.is_finished()]
 
+    def __add__(self, other: BaseTask) -> BaseTask:
+        return [self.add_task(o) for o in other] if isinstance(other, list) else self + [other]
+
     def add_task(self, task: BaseTask) -> BaseTask:
         if self.last_task():
             self.last_task().add_child(task)
         else:
             task.structure = self
 
             self.tasks.append(task)
@@ -47,52 +50,37 @@
 
         [task.reset() for task in self.tasks]
 
         self.__run_from_task(self.first_task())
 
         if self.memory:
             run = Run(
-                input=self.first_task().input.value,
-                output=self.last_task().output.value
+                input=self.first_task().input.to_text(),
+                output=self.last_task().output.to_text()
             )
 
             self.memory.add_run(run)
 
         self._execution_args = ()
 
         return self.last_task()
 
     def context(self, task: BaseTask) -> dict[str, any]:
         context = super().context(task)
 
         context.update(
             {
-                "input": task.parents[0].output.value if task.parents and task.parents[0].output else None,
+                "input": task.parents[0].output.to_text() if task.parents and task.parents[0].output else None,
                 "parent": task.parents[0] if task.parents else None,
                 "child": task.children[0] if task.children else None
             }
         )
 
         return context
 
-    def to_dict(self) -> dict:
-        from griptape.schemas import PipelineSchema
-
-        return PipelineSchema().dump(self)
-
-    @classmethod
-    def from_dict(cls, pipeline_dict: dict) -> Pipeline:
-        from griptape.schemas import PipelineSchema
-
-        return PipelineSchema().load(pipeline_dict)
-
-    @classmethod
-    def from_json(cls, pipeline_json: str) -> Pipeline:
-        return Pipeline.from_dict(json.loads(pipeline_json))
-
     def __run_from_task(self, task: Optional[BaseTask]) -> None:
         if task is None:
             return
         else:
             if isinstance(task.execute(), ErrorArtifact):
                 return
             else:
```

### Comparing `griptape-0.7.3/griptape/structures/structure.py` & `griptape-0.8.0/griptape/structures/structure.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,37 +3,35 @@
 import logging
 import uuid
 from abc import ABC, abstractmethod
 from logging import Logger
 from typing import Optional, Union, TYPE_CHECKING
 from attr import define, field, Factory
 from rich.logging import RichHandler
-from griptape.tasks import ActionSubtask
 from griptape import utils
 from griptape.drivers import BasePromptDriver, OpenAiPromptDriver
+from griptape.rules.ruleset import Ruleset
+from griptape.tasks import ActionSubtask
 from griptape.utils import J2
-from griptape.core import ToolLoader
 
 if TYPE_CHECKING:
     from griptape.rules import Rule
     from griptape.tasks import BaseTask
 
 
 @define
 class Structure(ABC):
     LOGGER_NAME = "griptape-flow"
 
     id: str = field(default=Factory(lambda: uuid.uuid4().hex), kw_only=True)
-    type: str = field(default=Factory(lambda self: self.__class__.__name__, takes_self=True), kw_only=True)
     prompt_driver: BasePromptDriver = field(default=OpenAiPromptDriver(), kw_only=True)
-    rules: list[Rule] = field(factory=list, kw_only=True)
+    rulesets: list[Ruleset] = field(factory=list, kw_only=True)
     tasks: list[BaseTask] = field(factory=list, kw_only=True)
     custom_logger: Optional[Logger] = field(default=None, kw_only=True)
     logger_level: int = field(default=logging.INFO, kw_only=True)
-    tool_loader: ToolLoader = field(default=ToolLoader(), kw_only=True)
     _execution_args: tuple = ()
     _logger: Optional[Logger] = None
 
     def __attrs_post_init__(self):
         for task in self.tasks:
             task.structure = self
 
@@ -82,15 +80,15 @@
             json.dumps(
                 ActionSubtask.ACTION_SCHEMA.json_schema("ActionSchema")
             )
         )
 
         stack = [
             J2("prompts/base.j2").render(
-                rules=self.rules,
+                rulesets=self.rulesets,
                 action_schema=action_schema,
                 ramp_names=str.join(", ", [ramp.name for ramp in ramps]),
                 ramps=[J2("prompts/ramp.j2").render(ramp=ramp) for ramp in ramps],
                 tool_names=str.join(", ", [tool.name for tool in tools]),
                 tools=[J2("prompts/tool.j2").render(tool=tool) for tool in tools]
             )
         ]
@@ -99,37 +97,20 @@
 
     def to_prompt_string(self, task: BaseTask) -> str:
         return self.stack_to_prompt_string(self.prompt_stack(task))
 
     def stack_to_prompt_string(self, stack: list[str]) -> str:
         return str.join("\n", stack)
 
-    def to_json(self) -> str:
-        return json.dumps(self.to_dict(), indent=2)
-
     def context(self, task: BaseTask) -> dict[str, any]:
         return {
             "args": self.execution_args,
             "structure": self,
         }
 
     @abstractmethod
     def add_task(self, task: BaseTask) -> BaseTask:
         ...
 
     @abstractmethod
     def run(self, *args) -> Union[BaseTask, list[BaseTask]]:
         ...
-
-    @abstractmethod
-    def to_dict(self) -> dict:
-        ...
-
-    @classmethod
-    @abstractmethod
-    def from_dict(cls, structure_dict: dict) -> Structure:
-        ...
-
-    @classmethod
-    @abstractmethod
-    def from_json(cls, structure_json: str) -> Structure:
-        ...
```

### Comparing `griptape-0.7.3/griptape/structures/structure_with_memory.py` & `griptape-0.8.0/griptape/structures/structure_with_memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.3/griptape/structures/workflow.py` & `griptape-0.8.0/griptape/structures/workflow.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 from griptape.utils import J2
 
 
 @define
 class Workflow(Structure):
     executor: futures.Executor = field(default=futures.ThreadPoolExecutor(), kw_only=True)
 
+    def __add__(self, other: BaseTask) -> BaseTask:
+        return [self.add_task(o) for o in other] if isinstance(other, list) else self + [other]
+
     def add_task(self, task: BaseTask) -> BaseTask:
         task.structure = self
 
         self.tasks.append(task)
 
         return task
 
@@ -56,15 +59,15 @@
         return self.output_tasks()
 
     def context(self, task: BaseTask) -> dict[str, any]:
         context = super().context(task)
 
         context.update(
             {
-                "inputs": {parent.id: parent.output.value if parent.output else "" for parent in task.parents},
+                "inputs": {parent.id: parent.output.to_text() if parent.output else "" for parent in task.parents},
                 "parents": {parent.id: parent for parent in task.parents},
                 "children": {child.id: child for child in task.children}
             }
         )
 
         return context
 
@@ -81,22 +84,7 @@
                 if key_task.id in value_task.child_ids:
                     graph[key_task.id].add(value_task.id)
 
         return graph
 
     def order_tasks(self) -> list[BaseTask]:
         return [self.find_task(task_id) for task_id in TopologicalSorter(self.to_graph()).static_order()]
-
-    def to_dict(self) -> dict:
-        from griptape.schemas import WorkflowSchema
-
-        return WorkflowSchema().dump(self)
-
-    @classmethod
-    def from_dict(cls, workflow_dict: dict) -> Workflow:
-        from griptape.schemas import WorkflowSchema
-
-        return WorkflowSchema().load(workflow_dict)
-
-    @classmethod
-    def from_json(cls, workflow_json: str) -> Workflow:
-        return Workflow.from_dict(json.loads(workflow_json))
```

### Comparing `griptape-0.7.3/griptape/summarizers/prompt_driver_summarizer.py` & `griptape-0.8.0/griptape/summarizers/prompt_driver_summarizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         try:
             if len(runs) > 0:
                 return self.driver.run(
                     value=J2("prompts/summarize.j2").render(
                         summary=previous_summary,
                         runs=runs
                     )
-                ).value
+                ).to_text()
             else:
                 return previous_summary
         except Exception as e:
             logging.error(f"Error summarizing memory: {type(e).__name__}({e})")
 
             return previous_summary
```

### Comparing `griptape-0.7.3/griptape/tasks/action_subtask.py` & `griptape-0.8.0/griptape/tasks/action_subtask.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,119 +1,121 @@
 from __future__ import annotations
 import ast
 import json
 import re
-from typing import TYPE_CHECKING, Optional, Tuple
+from typing import TYPE_CHECKING, Optional
 import schema
 from attr import define, field
 from jsonschema.exceptions import ValidationError
 from jsonschema.validators import validate
-from schema import Schema, And, Literal
+from schema import Schema, Literal
 from griptape.artifacts import ErrorArtifact, TextArtifact
+from griptape.core import BaseTool, ActivityMixin
 from griptape.ramps import BaseRamp
 from griptape.tasks import PromptTask
-from griptape.core import BaseTool, ActivityMixin
 from griptape.utils import J2
 
 if TYPE_CHECKING:
     from griptape.artifacts import BaseArtifact
     from griptape.tasks import ToolkitTask
 
 
 @define
 class ActionSubtask(PromptTask):
     THOUGHT_PATTERN = r"^Thought:\s*(.*)$"
     ACTION_PATTERN = r"^Action:\s*({.*})$"
     OUTPUT_PATTERN = r"^Output:\s?([\s\S]*)$"
     INVALID_ACTION_ERROR_MSG = f"invalid action input, try again"
     ACTION_SCHEMA = Schema(
-        description="Actions have type, name, method, and optional input value.",
+        description="Actions have type, name, activity, and input value.",
         schema={
             Literal(
                 "type",
                 description="Action type"
-            ): And(str, lambda s: s in ("tool", "ramp")),
+            ): schema.Or("tool", "ramp"),
             Literal(
                 "name",
                 description="Action name"
             ): str,
             Literal(
                 "activity",
                 description="Action activity"
             ): str,
             schema.Optional(
                 Literal(
                     "input",
-                    description="Action method input value"
+                    description="Optional action activity input object with optional values and optional artifacts"
                 )
-            ): schema.Or(str, list, {object: object})
+            ): dict
         }
     )
 
     parent_task_id: Optional[str] = field(default=None, kw_only=True)
     thought: Optional[str] = field(default=None, kw_only=True)
     action_type: Optional[str] = field(default=None, kw_only=True)
     action_name: Optional[str] = field(default=None, kw_only=True)
     action_activity: Optional[str] = field(default=None, kw_only=True)
-    action_input: Optional[Tuple[str, list, dict]] = field(default=None, kw_only=True)
+    action_input: dict = field(default=None, kw_only=True)
 
     _tool: Optional[BaseTool] = None
-    _ramps: Optional[BaseRamp] = None
+    _ramp: Optional[BaseRamp] = None
 
     def attach(self, parent_task: ToolkitTask):
         self.parent_task_id = parent_task.id
         self.structure = parent_task.structure
-        self.__init_from_prompt(self.input.value)
+        self.__init_from_prompt(self.input.to_text())
 
     @property
     def task(self) -> Optional[ToolkitTask]:
         return self.structure.find_task(self.parent_task_id)
 
     @property
     def parents(self) -> list[ActionSubtask]:
         return [self.task.find_subtask(parent_id) for parent_id in self.parent_ids]
 
     @property
     def children(self) -> list[ActionSubtask]:
         return [self.task.find_subtask(child_id) for child_id in self.child_ids]
 
     def before_run(self) -> None:
-        self.structure.logger.info(f"Subtask {self.id}\n{self.input.value}")
+        self.structure.logger.info(f"Subtask {self.id}\n{self.input.to_text()}")
 
     def run(self) -> BaseArtifact:
         try:
             if self.action_name == "error":
-                self.output = ErrorArtifact(self.action_input, task=self.task)
+                self.output = ErrorArtifact(str(self.action_input))
             else:
                 if self.action_type == "tool":
                     if self._tool:
-                        observation = self.structure.tool_loader.executor.execute(
+                        observation = self.task.executor.execute(
                             getattr(self._tool, self.action_activity),
-                            TextArtifact(self.action_input)
+                            self.action_input if self.action_input else None
                         )
                     else:
                         observation = ErrorArtifact("tool not found")
                 elif self.action_type == "ramp":
-                    if self._ramps:
-                        observation = getattr(self._ramps, self.action_activity)(self.action_input)
+                    if self._ramp:
+                        observation = getattr(self._ramp, self.action_activity)(
+                            self.action_input if self.action_input else None
+                        )
                     else:
-                        observation = ErrorArtifact("ramps not found")
+                        observation = ErrorArtifact("ramp not found")
                 else:
                     observation = ErrorArtifact("invalid action type")
 
                 self.output = observation
         except Exception as e:
             self.structure.logger.error(f"Subtask {self.id}\n{e}", exc_info=True)
 
-            self.output = ErrorArtifact(str(e), exception=e, task=self.task)
+            self.output = ErrorArtifact(str(e))
         finally:
             return self.output
 
     def after_run(self) -> None:
-        self.structure.logger.info(f"Subtask {self.id}\nObservation: {self.output.value}")
+        self.structure.logger.info(f"Subtask {self.id}\nObservation: {self.output.to_text()}")
 
     def render(self) -> str:
         return J2("prompts/tasks/tool/subtask.j2").render(
             subtask=self
         )
 
     def to_json(self) -> str:
@@ -189,40 +191,43 @@
                     if self.action_name:
                         self._tool = self.task.find_tool(self.action_name)
 
                     if self._tool:
                         self.__validate_activity_mixin(self._tool)
                 elif self.action_type == "ramp":
                     if self.action_name:
-                        self._ramps = self.task.find_ramps(self.action_name)
+                        self._ramp = self.task.find_ramp(self.action_name)
 
-                    if self._ramps:
-                        self.__validate_activity_mixin(self._ramps)
+                    if self._ramp:
+                        self.__validate_activity_mixin(self._ramp)
             except SyntaxError as e:
                 self.structure.logger.error(f"Subtask {self.task.id}\nSyntax error: {e}")
 
                 self.action_name = "error"
-                self.action_input = f"syntax error: {e}"
+                self.action_input = {"error": f"syntax error: {e}"}
             except ValidationError as e:
                 self.structure.logger.error(f"Subtask {self.task.id}\nInvalid action JSON: {e}")
 
                 self.action_name = "error"
-                self.action_input = f"Action JSON validation error: {e}"
+                self.action_input = {"error": f"Action JSON validation error: {e}"}
             except Exception as e:
                 self.structure.logger.error(f"Subtask {self.task.id}\nError parsing tool action: {e}")
 
                 self.action_name = "error"
-                self.action_input = f"error: {self.INVALID_ACTION_ERROR_MSG}"
+                self.action_input = {"error": f"error: {self.INVALID_ACTION_ERROR_MSG}"}
         elif self.output is None and len(output_matches) > 0:
             self.output = TextArtifact(output_matches[-1])
 
     def __validate_activity_mixin(self, mixin: ActivityMixin) -> None:
         try:
-            validate(
-                instance=self.action_input,
-                schema=mixin.activity_schema(getattr(mixin, self.action_activity))
-            )
+            activity_schema = mixin.activity_schema(getattr(mixin, self.action_activity))
+
+            if activity_schema:
+                validate(
+                    instance=self.action_input,
+                    schema=activity_schema
+                )
         except ValidationError as e:
             self.structure.logger.error(f"Subtask {self.task.id}\nInvalid activity input JSON: {e}")
 
             self.action_name = "error"
-            self.action_input = f"Activity input JSON validation error: {e}"
+            self.action_input = {"error": f"Activity input JSON validation error: {e}"}
```

### Comparing `griptape-0.7.3/griptape/tasks/base_task.py` & `griptape-0.8.0/griptape/tasks/base_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     class State(Enum):
         PENDING = 1
         EXECUTING = 2
         FINISHED = 3
 
     id: str = field(default=Factory(lambda: uuid.uuid4().hex), kw_only=True)
     state: State = field(default=State.PENDING, kw_only=True)
-    type: str = field(default=Factory(lambda self: self.__class__.__name__, takes_self=True), kw_only=True)
     parent_ids: list[str] = field(factory=list, kw_only=True)
     child_ids: list[str] = field(factory=list, kw_only=True)
 
     output: Optional[BaseArtifact] = field(default=None, init=False)
     structure: Optional[Structure] = field(default=None, init=False)
 
     @property
@@ -37,14 +36,20 @@
     def parents(self) -> list[BaseTask]:
         return [self.structure.find_task(parent_id) for parent_id in self.parent_ids]
 
     @property
     def children(self) -> list[BaseTask]:
         return [self.structure.find_task(child_id) for child_id in self.child_ids]
 
+    def __rshift__(self, child: BaseTask) -> BaseTask:
+        return self.add_child(child)
+
+    def __lshift__(self, child: BaseTask) -> BaseTask:
+        return self.add_parent(child)
+
     def add_child(self, child: BaseTask) -> BaseTask:
         if self.structure:
             child.structure = self.structure
         elif child.structure:
             self.structure = child.structure
 
         if child not in self.structure.tasks:
@@ -104,15 +109,15 @@
 
             self.output = self.run()
 
             self.after_run()
         except Exception as e:
             self.structure.logger.error(f"Task {self.id}\n{e}", exc_info=True)
 
-            self.output = ErrorArtifact(str(e), exception=e, task=self)
+            self.output = ErrorArtifact(str(e))
         finally:
             self.state = BaseTask.State.FINISHED
 
             return self.output
 
     def can_execute(self) -> bool:
         return self.state == BaseTask.State.PENDING and all(parent.is_finished() for parent in self.parents)
```

### Comparing `griptape-0.7.3/griptape/tasks/prompt_task.py` & `griptape-0.8.0/griptape/tasks/prompt_task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional
 from attr import define, field
 from griptape.utils import J2
 from griptape.tasks import BaseTask
-from griptape.artifacts import TextArtifact
+from griptape.artifacts import TextArtifact, BaseArtifact
 
 if TYPE_CHECKING:
     from griptape.drivers import BasePromptDriver
 
 
 @define
 class PromptTask(BaseTask):
     prompt_template: str = field(default="{{ args[0] }}")
     context: dict[str, any] = field(factory=dict, kw_only=True)
     driver: Optional[BasePromptDriver] = field(default=None, kw_only=True)
+    output: Optional[BaseArtifact] = field(default=None, init=False)
 
     @property
     def input(self) -> TextArtifact:
         return TextArtifact(
             J2().render_from_string(
                 self.prompt_template,
                 **self.full_context
             )
         )
 
     def before_run(self) -> None:
         super().before_run()
 
-        self.structure.logger.info(f"Task {self.id}\nInput: {self.input.value}")
+        self.structure.logger.info(f"Task {self.id}\nInput: {self.input.to_text()}")
 
     def run(self) -> TextArtifact:
         self.output = self.active_driver().run(value=self.structure.to_prompt_string(self))
 
         return self.output
 
     def after_run(self) -> None:
         super().after_run()
 
-        self.structure.logger.info(f"Task {self.id}\nOutput: {self.output.value}")
+        self.structure.logger.info(f"Task {self.id}\nOutput: {self.output.to_text()}")
 
     def active_driver(self) -> BasePromptDriver:
         if self.driver is None:
             return self.structure.prompt_driver
         else:
             return self.driver
```

### Comparing `griptape-0.7.3/griptape/tasks/toolkit_task.py` & `griptape-0.8.0/griptape/tasks/toolkit_task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 from __future__ import annotations
-from abc import ABC
 from typing import TYPE_CHECKING, Optional
 from attr import define, field
 from griptape.core import BaseTool
+from griptape.executors import BaseExecutor, LocalExecutor
 from griptape.utils import J2
 from griptape.tasks import PromptTask
 from griptape.artifacts import TextArtifact, ErrorArtifact
 
 if TYPE_CHECKING:
     from griptape.tasks import ActionSubtask
     from griptape.ramps import BaseRamp
 
 
 @define
-class ToolkitTask(PromptTask, ABC):
+class ToolkitTask(PromptTask):
     DEFAULT_MAX_STEPS = 20
 
-    tool_names: list[str] = field(kw_only=True)
+    tools: list[BaseTool] = field(factory=list, kw_only=True)
+    executor: BaseExecutor = field(default=LocalExecutor(), kw_only=True)
     max_subtasks: int = field(default=DEFAULT_MAX_STEPS, kw_only=True)
     _subtasks: list[ActionSubtask] = field(factory=list)
 
-    @tool_names.validator
-    def validate_tool_names(self, _, tool_names: list[str]) -> None:
-        if len(tool_names) > len(set(tool_names)):
-            raise ValueError("tool names have to be unique")
+    @tools.validator
+    def validate_tools(self, _, tools: list[BaseTool]) -> None:
+        tool_names = [t.name for t in tools]
 
-    @property
-    def tools(self) -> list[BaseTool]:
-        return [
-            t for t in [self.structure.tool_loader.load_tool(t) for t in self.tool_names] if t is not None
-        ]
+        if len(tool_names) > len(set(tool_names)):
+            raise ValueError("tools have to be unique")
 
     @property
     def ramps(self) -> list[BaseRamp]:
         unique_ramps_dict = {}
 
         for ramps_dict in [tool.ramps for tool in self.tools]:
             for ramps_list in ramps_dict.values():
@@ -46,36 +43,35 @@
     def run(self) -> TextArtifact:
         from griptape.tasks import ActionSubtask
 
         self._subtasks.clear()
 
         subtask = self.add_subtask(
             ActionSubtask(
-                self.active_driver().run(value=self.structure.to_prompt_string(self)).value
+                self.active_driver().run(value=self.structure.to_prompt_string(self)).to_text()
             )
         )
 
         while True:
             if subtask.output is None:
                 if len(self._subtasks) >= self.max_subtasks:
                     subtask.output = ErrorArtifact(
-                        f"Exceeded tool limit of {self.max_subtasks} subtasks per task",
-                        task=self
+                        f"Exceeded tool limit of {self.max_subtasks} subtasks per task"
                     )
                 elif subtask.action_name is None:
                     # handle case when the LLM failed to follow the ReAct prompt and didn't return a proper action
                     subtask.output = TextArtifact(subtask.prompt_template)
                 else:
                     subtask.before_run()
                     subtask.run()
                     subtask.after_run()
 
                     subtask = self.add_subtask(
                         ActionSubtask(
-                            self.active_driver().run(value=self.structure.to_prompt_string(self)).value
+                            self.active_driver().run(value=self.structure.to_prompt_string(self)).to_text()
                         )
                     )
             else:
                 break
 
         self.output = subtask.output
 
@@ -102,12 +98,12 @@
 
     def find_tool(self, tool_name: str) -> Optional[BaseTool]:
         return next(
             (t for t in self.tools if t.name == tool_name),
             None
         )
 
-    def find_ramps(self, ramp_name: str) -> Optional[BaseRamp]:
+    def find_ramp(self, ramp_name: str) -> Optional[BaseRamp]:
         return next(
             (r for r in self.ramps if r.name == ramp_name),
             None
         )
```

### Comparing `griptape-0.7.3/griptape/templates/prompts/base.j2` & `griptape-0.8.0/griptape/templates/prompts/base.j2`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 You are an assistant that follows rules, acts truthfully, and doesn't make things up. You can perform actions to answer questions and complete tasks step-by-step. If an action fails you can be creative and try to fix it or try other options. To perform an action use this conversation format:
 
 Input: <original request>
 Thought: <your step-by-step thought process about how you can complete the request>
-Action: minified JSON object with the following JSON Schema: {{ action_schema }}
+Action: minified JSON object with the following JSON schema: {{ action_schema }}
 Observation: <action result>
 ...repeat Thought/Action/Observation until you can respond to the original request
-Thought: I have enough information to respond to the original request
 Output: <your final response>
 
 "Input:", "Thought:", "Action:", "Observation:", and "Output:" must ALWAYS start on a new line.
 
-Action must ALWAYS be a minified JSON object on a single line.
+Action must ALWAYS be a minified JSON object starting on the same line as "Action:"
 
-If you don't need to perform an action or if you don't know which action to perform, ignore Thought/Action/Observation and go straight to Output.
+If you don't need to perform an action or if you don't know which action to perform, ignore Thought/Action/Observation and go straight to Output. NEVER make up action types.
 
 Actions of type "tool"
 {% if tool_names|length > 0 %}
-You can use tool activities to complete tasks. You have access to the following tools: [{{ tool_names }}]. NEVER make up tool names. If you encounter an error from a tool you should try to fix it. Don't request extra information from the user.
+You can use tool activities to complete tasks. You have access to only the following tools: [{{ tool_names }}]. NEVER make up tools. If you encounter an error from a tool you should try to fix it. Don't request extra information from the user.
 
 {% for tool in tools %}
 {{ tool }}
 {% endfor %}
 {% else %}
 You don't have access to any actions of type "tool"
 {% endif %}
 
 Actions of type "ramp"
 {% if ramp_names|length > 0 %}
-Ramp is used as an intermediary between tools. Some tools might use ramps for outputs. You can use ramp activities to complete tasks. You have access to the following ramps: [{{ ramp_names }}]. NEVER make up ramp names. If you encounter an error from a ramp you should try to fix it. Don't request extra information from the user.
+Ramp is used to pass data between tools. Some tools might use ramps for outputs. You can use ramp activities to complete tasks. You have access to only the following ramps: [{{ ramp_names }}]. NEVER make up ramps. If you encounter an error from a ramp you should try to fix it. Don't request extra information from the user.
 
 {% for ramp in ramps %}
 {{ ramp }}
 {% endfor %}
 {% else %}
 You don't have access to any actions of type "ramp"
 {% endif %}
 
-{% if rules|length > 0 %}
-When responding, always use the following rules but don't allow those rules to override your conversation format:
-{% for rule in rules %}
+{% if rulesets|length > 0 %}
+When responding, always use rules from the following rulesets but don't allow those rules to override your conversation format. Rulesets can override and complement each other:
+
+{% for ruleset in rulesets %}
+Ruleset name: {{ ruleset.name }}
+"{{ ruleset.name }}" rules:
+{% for rule in ruleset.rules %}
 Rule #{{loop.index}}
 {{ rule.value }}
 {% endfor %}
+
+{% endfor %}
 {% endif %}
```

### Comparing `griptape-0.7.3/griptape/tokenizers/base_tokenizer.py` & `griptape-0.8.0/griptape/tokenizers/base_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.3/griptape/tokenizers/cohere_tokenizer.py` & `griptape-0.8.0/griptape/tokenizers/cohere_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.3/griptape/tokenizers/hugging_face_tokenizer.py` & `griptape-0.8.0/griptape/tokenizers/hugging_face_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.3/griptape/tokenizers/tiktoken_tokenizer.py` & `griptape-0.8.0/griptape/tokenizers/tiktoken_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.3/griptape/utils/command_runner.py` & `griptape-0.8.0/griptape/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.3/griptape/utils/j2.py` & `griptape-0.8.0/griptape/utils/j2.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.3/griptape/utils/python_runner.py` & `griptape-0.8.0/griptape/utils/python_runner.py`

 * *Files identical despite different names*

### Comparing `griptape-0.7.3/pyproject.toml` & `griptape-0.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape"
-version = "0.7.3"
+version = "0.8.0"
 description = "Modular Python framework for LLM workflows, tools, memory, and data."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape"
 
 packages = [
@@ -27,15 +27,14 @@
 stopit = "*"
 transformers = ">=4"
 huggingface-hub = ">=0.13"
 docker = ">=6"
 stringcase = ">=1"
 schema = ">=0.7"
 pyyaml = ">=6"
-langchain = ">=0.0.120"
 fastapi = ">=0.80"
 uvicorn = ">= 0.20"
 python-decouple=">=3"
 llama_index = "~0.6.0"
 boto3 = "^1.26.123"
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `griptape-0.7.3/PKG-INFO` & `griptape-0.8.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griptape
-Version: 0.7.3
+Version: 0.8.0
 Summary: Modular Python framework for LLM workflows, tools, memory, and data.
 Home-page: https://github.com/griptape-ai/griptape
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -17,15 +17,14 @@
 Requires-Dist: cohere (>=4)
 Requires-Dist: docker (>=6)
 Requires-Dist: fastapi (>=0.80)
 Requires-Dist: graphlib
 Requires-Dist: huggingface-hub (>=0.13)
 Requires-Dist: jinja2 (>=3.1)
 Requires-Dist: jsonschema (>=4)
-Requires-Dist: langchain (>=0.0.120)
 Requires-Dist: llama_index (>=0.6.0,<0.7.0)
 Requires-Dist: marshmallow (>=3)
 Requires-Dist: marshmallow-enum (>=1.5)
 Requires-Dist: openai (>=0.27)
 Requires-Dist: python-decouple (>=3)
 Requires-Dist: python-dotenv (>=0.21)
 Requires-Dist: pyyaml (>=6)
@@ -46,15 +45,15 @@
 [![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io/)
 [![Griptape Discord](https://dcbadge.vercel.app/api/server/gnWRz88eym?compact=true&style=flat)](https://discord.gg/gnWRz88eym)
 
 **griptape** is a modular Python framework for LLM workflows, tools, memory, and data that enables developers to:
 
 1. 🤖 Build **AI agents**, sequential **LLM pipelines** and sprawling **DAG workflows** for complex use cases.
 2. ⛓️ Augment LLMs with **chain of thought** capabilities.
-3. 🧰️ Integrate other services and functionality into LLMs as [tools](https://github.com/griptape-ai/griptape-tools) (e.g., calculators, web scrapers, spreadsheet editors, and API connectors); run tools in any environment (local, containerized, cloud, etc.); use tools directly in **griptape** or convert them into ramps abstractions, such as ChatGPT Plugins, LangChain tools, or Fixie.ai agents.
+3. 🧰️ Integrate other services and functionality into LLMs as [tools](https://github.com/griptape-ai/griptape-tools) (e.g., calculators, web scrapers, spreadsheet editors, and API connectors); run tools in any environment (local, containerized, cloud, etc.); and wrap tools with off prompt data storage that prevents LLMs from accessing your data directly.
 4. 💾 Add **memory** to AI pipelines for context preservation and summarization.
 
 ## Documentation
 
 Please refer to [Griptape Docs](https://griptape.readthedocs.io) for:
 
 - Getting started guides. 
@@ -68,72 +67,77 @@
 
 ```
 pip install griptape griptape-tools -U
 ```
 
 Second, configure an OpenAI client by [getting an API key](https://beta.openai.com/account/api-keys) and adding it to your environment as `OPENAI_API_KEY`. griptape uses [OpenAI Completions API](https://platform.openai.com/docs/guides/completion) to execute LLM prompts and to work with [LlamaIndex](https://gpt-index.readthedocs.io/en/latest/index.html) data structures.
 
-With **griptape**, you can create *structures*, such as `Agents`, `Pipelines`, and `Workflows`, that are composed of different types of tasks. You can also define structures as JSON objects and load them into **griptape** dynamically. Let's define a simple two-task pipeline that uses tools:
+With **griptape**, you can create *structures*, such as `Agents`, `Pipelines`, and `Workflows`, that are composed of different types of tasks. You can also define structures as JSON objects and load them into **griptape** dynamically. Let's define a simple two-task pipeline that uses tools and ramps:
 
 ```python
-from decouple import config
-from griptape.core import ToolLoader
-from griptape.drivers import OpenAiPromptDriver, MemoryStorageDriver
-from griptape.executors import LocalExecutor
 from griptape.memory import Memory
-from griptape.ramps import StorageRamp
+from griptape.ramps import TextStorageRamp, BlobStorageRamp
 from griptape.structures import Pipeline
 from griptape.tasks import ToolkitTask, PromptTask
-from griptape.tools import WebScraper
+from griptape.tools import WebScraper, TextProcessor, FileManager
 
-storage = StorageRamp(
-    driver=MemoryStorageDriver()
+# Ramps enable LLMs to store and manipulate data without ever looking at it directly.
+text_storage = TextStorageRamp()
+blob_storage = BlobStorageRamp()
+
+# Connect a web scraper to load web pages.
+web_scraper = WebScraper(
+    ramps={
+        "get_content": [text_storage]
+    }
+)
+
+# TextProcessor enables LLMs to summarize and query text.
+text_processor = TextProcessor(
+    ramps={
+        "summarize": [text_storage],
+        "query": [text_storage]
+    }
 )
 
-scraper = WebScraper(
+# File manager can load and store files locally.
+file_manager = FileManager(
     ramps={
-        "get_content": [storage]
+        "load": [blob_storage],
+        "save": [text_storage, blob_storage]
     }
 )
 
+# Pipelines represent sequences of tasks.
 pipeline = Pipeline(
-    memory=Memory(),
-    tool_loader=ToolLoader(
-        tools=[scraper],
-        executor=LocalExecutor()
-    )
+    memory=Memory()
 )
 
 pipeline.add_tasks(
+    # Load up the first argument from `pipeline.run`.
     ToolkitTask(
-        tool_names=[scraper.name]
+        "{{ args[0] }}",
+        tools=[web_scraper, text_processor, file_manager]
     ),
+    # Augment `input` from the previous task.
     PromptTask(
         "Say the following in spanish: {{ input }}"
     )
 )
 
-result = pipeline.run("Give me a summary of https://en.wikipedia.org/wiki/Large_language_model")
-
-print(result.output.value)
-
+result = pipeline.run("Load https://griptape.readthedocs.io, summarize it, and store it in griptape.txt")
 
+print(result.output.to_text())
 ```
 
 Boom! Our first LLM pipeline with two sequential tasks generated the following exchange:
 
 ```
-Q: Give me a summary of https://en.wikipedia.org/wiki/Large_language_model
-[chain of thought output... will vary depending on the model driver you're using]
-A: Los modelos de lenguaje de gran tamaño son herramientas utilizadas para tareas de 
-procesamiento del lenguaje natural, como detectar falsedades, completar oraciones y comprender 
-el lenguaje. Algunos modelos notables incluyen BERT, GPT-2, GPT-3, GPT-Neo y GLaM. The Pile es 
-un conjunto de datos extenso utilizado para el modelado del lenguaje. Estos modelos han sido 
-desarrollados e investigados en trabajos como TruthfulQA, HellaSwag y BERT: Pre-entrenamiento 
-de transformadores bidireccionales profundos para la comprensión del lenguaje.
+Q: Load https://griptape.readthedocs.io, summarize it, and store it in griptape.txt
+A: El contenido de https://griptape.readthedocs.io ha sido resumido y almacenado en griptape.txt.
 ```
 
 ## Versioning
 
 **griptape** is in early development and its APIs and documentation are subject to change. Until we stabilize the API and release version 1.0.0, we will use minor versions (i.e., x.Y.z) to introduce features and breaking features, and patch versions (i.e., x.y.Z) for bug fixes.
 
 ## Contributing
```

