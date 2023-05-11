# Comparing `tmp/wanna-ml-0.2.8.tar.gz` & `tmp/wanna-ml-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wanna-ml-0.2.8.tar", max compression
+gzip compressed data, was "wanna-ml-0.2.9.tar", max compression
```

## Comparing `wanna-ml-0.2.8.tar` & `wanna-ml-0.2.9.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0      275 2022-09-06 10:11:15.239657 wanna-ml-0.2.8/CHANGELOG.md
--rw-r--r--   0        0        0     3390 2022-09-06 10:11:15.239657 wanna-ml-0.2.8/README.md
--rw-r--r--   0        0        0     3916 2022-09-06 10:11:25.387727 wanna-ml-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      302 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/__init__.py
--rw-r--r--   0        0        0      302 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/cli/__init__.py
--rw-r--r--   0        0        0     1884 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/cli/__main__.py
--rw-r--r--   0        0        0        0 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/cli/plugins/__init__.py
--rw-r--r--   0        0        0      413 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/cli/plugins/base_plugin.py
--rw-r--r--   0        0        0     1042 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/cli/plugins/common_options.py
--rw-r--r--   0        0        0      803 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/cli/plugins/components_plugin.py
--rw-r--r--   0        0        0     4985 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/cli/plugins/job_plugin.py
--rw-r--r--   0        0        0     5744 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/cli/plugins/managed_notebook_plugin.py
--rw-r--r--   0        0        0     7549 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/cli/plugins/notebook_plugin.py
--rw-r--r--   0        0        0     5563 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/cli/plugins/pipeline_plugin.py
--rw-r--r--   0        0        0      984 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/cli/plugins/runner.py
--rw-r--r--   0        0        0     3616 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/cli/plugins/tensorboard_plugin.py
--rw-r--r--   0        0        0     1335 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/cli/version.py
--rw-r--r--   0        0        0        0 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/components/__init__.py
--rw-r--r--   0        0        0     2166 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/components/kubeflow/get_or_create_endpoint.py
--rw-r--r--   0        0        0      284 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/components/loader.py
--rw-r--r--   0        0        0      527 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/components/template.py
--rw-r--r--   0        0        0        0 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/components/templates/__init__.py
--rw-r--r--   0        0        0      700 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/components/templates/base/cookiecutter.json
--rw-r--r--   0        0        0       31 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/.dockerignore
--rw-r--r--   0        0        0      997 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/Dockerfile
--rw-r--r--   0        0        0       36 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/README.md
--rw-r--r--   0        0        0      839 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/component.yaml
--rw-r--r--   0        0        0      697 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/setup.py
--rw-r--r--   0        0        0        0 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/src/{{ cookiecutter.component_slug }}/__init__.py
--rw-r--r--   0        0        0      482 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/src/{{ cookiecutter.component_slug }}/{{cookiecutter.component_slug}}.py
--rw-r--r--   0        0        0      119 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/tests/test_{{cookiecutter.component_slug}}.py
--rw-r--r--   0        0        0        0 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/__init__.py
--rw-r--r--   0        0        0        0 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/deployment/__init__.py
--rw-r--r--   0        0        0     1716 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/deployment/artifacts_push.py
--rw-r--r--   0        0        0      122 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/deployment/credentials.py
--rw-r--r--   0        0        0     1071 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/deployment/io.py
--rw-r--r--   0        0        0     3584 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/deployment/models.py
--rw-r--r--   0        0        0     4659 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/deployment/monitoring.py
--rw-r--r--   0        0        0      370 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/deployment/vertex_connector.py
--rw-r--r--   0        0        0     9152 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/deployment/vertex_jobs.py
--rw-r--r--   0        0        0    10880 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/deployment/vertex_pipelines.py
--rw-r--r--   0        0        0     7874 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/deployment/vertex_scheduling.py
--rw-r--r--   0        0        0     2080 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/loggers/wanna_logger.py
--rw-r--r--   0        0        0        0 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/models/__init__.py
--rw-r--r--   0        0        0      879 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/models/base_instance.py
--rw-r--r--   0        0        0      318 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/models/cloud_scheduler.py
--rw-r--r--   0        0        0     1987 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/models/docker.py
--rw-r--r--   0        0        0      834 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/models/gcp_components.py
--rw-r--r--   0        0        0     1288 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/models/gcp_profile.py
--rw-r--r--   0        0        0     1955 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/models/notebook.py
--rw-r--r--   0        0        0      329 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/models/notification_channel.py
--rw-r--r--   0        0        0      726 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/models/pipeline.py
--rw-r--r--   0        0        0      203 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/models/tensorboard.py
--rw-r--r--   0        0        0     4917 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/models/training_custom_job.py
--rw-r--r--   0        0        0     2647 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/models/wanna_config.py
--rw-r--r--   0        0        0      265 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/models/wanna_project.py
--rw-r--r--   0        0        0        0 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/services/__init__.py
--rw-r--r--   0        0        0     8519 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/services/base.py
--rw-r--r--   0        0        0    16015 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/services/docker.py
--rw-r--r--   0        0        0    19391 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/services/jobs.py
--rw-r--r--   0        0        0    15034 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/services/managed_notebook.py
--rw-r--r--   0        0        0    19378 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/services/notebook.py
--rw-r--r--   0        0        0     4454 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/services/path_utils.py
--rw-r--r--   0        0        0    13732 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/services/pipeline.py
--rw-r--r--   0        0        0     8655 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/services/tensorboard.py
--rw-r--r--   0        0        0        0 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/templates/__init__.py
--rw-r--r--   0        0        0      655 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/templates/notebook_startup_script.sh.j2
--rw-r--r--   0        0        0      239 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/templates/notebook_template.Dockerfile
--rw-r--r--   0        0        0     1885 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/templates/scheduler_cloud_function.py
--rw-r--r--   0        0        0      152 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/templates/scheduler_cloud_function_requirements.txt
--rw-r--r--   0        0        0     1372 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/templates/sla_cloud_function.py
--rw-r--r--   0        0        0      104 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/templates/sla_cloud_function_requirements.txt
--rw-r--r--   0        0        0        0 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/utils/__init__.py
--rw-r--r--   0        0        0     3694 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/utils/config_enricher.py
--rw-r--r--   0        0        0     3021 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/utils/config_loader.py
--rw-r--r--   0        0        0     1248 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/utils/credentials.py
--rw-r--r--   0        0        0    12354 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/utils/gcp.py
--rw-r--r--   0        0        0      545 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/utils/json.py
--rw-r--r--   0        0        0     1344 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/utils/loaders.py
--rw-r--r--   0        0        0      396 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/utils/templates.py
--rw-r--r--   0        0        0      104 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/utils/time.py
--rw-r--r--   0        0        0     5615 2022-09-06 10:11:15.243657 wanna-ml-0.2.8/src/wanna/core/utils/validators.py
--rw-r--r--   0        0        0     6079 1970-01-01 00:00:00.000000 wanna-ml-0.2.8/setup.py
--rw-r--r--   0        0        0     6551 1970-01-01 00:00:00.000000 wanna-ml-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      275 2022-09-07 07:15:16.462216 wanna-ml-0.2.9/CHANGELOG.md
+-rw-r--r--   0        0        0     3390 2022-09-07 07:15:16.462216 wanna-ml-0.2.9/README.md
+-rw-r--r--   0        0        0     3916 2022-09-07 07:15:25.146238 wanna-ml-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      302 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/__init__.py
+-rw-r--r--   0        0        0      302 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/cli/__init__.py
+-rw-r--r--   0        0        0     1884 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/cli/__main__.py
+-rw-r--r--   0        0        0        0 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/cli/plugins/__init__.py
+-rw-r--r--   0        0        0      413 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/cli/plugins/base_plugin.py
+-rw-r--r--   0        0        0     1042 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/cli/plugins/common_options.py
+-rw-r--r--   0        0        0      803 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/cli/plugins/components_plugin.py
+-rw-r--r--   0        0        0     4985 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/cli/plugins/job_plugin.py
+-rw-r--r--   0        0        0     5744 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/cli/plugins/managed_notebook_plugin.py
+-rw-r--r--   0        0        0     7549 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/cli/plugins/notebook_plugin.py
+-rw-r--r--   0        0        0     5563 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/cli/plugins/pipeline_plugin.py
+-rw-r--r--   0        0        0      984 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/cli/plugins/runner.py
+-rw-r--r--   0        0        0     3616 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/cli/plugins/tensorboard_plugin.py
+-rw-r--r--   0        0        0     1335 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/cli/version.py
+-rw-r--r--   0        0        0        0 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/components/__init__.py
+-rw-r--r--   0        0        0     2166 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/components/kubeflow/get_or_create_endpoint.py
+-rw-r--r--   0        0        0      284 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/components/loader.py
+-rw-r--r--   0        0        0      527 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/components/template.py
+-rw-r--r--   0        0        0        0 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/components/templates/__init__.py
+-rw-r--r--   0        0        0      700 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/components/templates/base/cookiecutter.json
+-rw-r--r--   0        0        0       31 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/.dockerignore
+-rw-r--r--   0        0        0      997 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/Dockerfile
+-rw-r--r--   0        0        0       36 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/README.md
+-rw-r--r--   0        0        0      839 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/component.yaml
+-rw-r--r--   0        0        0      697 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/setup.py
+-rw-r--r--   0        0        0        0 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/src/{{ cookiecutter.component_slug }}/__init__.py
+-rw-r--r--   0        0        0      482 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/src/{{ cookiecutter.component_slug }}/{{cookiecutter.component_slug}}.py
+-rw-r--r--   0        0        0      119 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/tests/test_{{cookiecutter.component_slug}}.py
+-rw-r--r--   0        0        0        0 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/deployment/__init__.py
+-rw-r--r--   0        0        0     1716 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/deployment/artifacts_push.py
+-rw-r--r--   0        0        0      122 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/deployment/credentials.py
+-rw-r--r--   0        0        0     1071 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/deployment/io.py
+-rw-r--r--   0        0        0     3584 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/deployment/models.py
+-rw-r--r--   0        0        0     4659 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/deployment/monitoring.py
+-rw-r--r--   0        0        0      370 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/deployment/vertex_connector.py
+-rw-r--r--   0        0        0     9152 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/deployment/vertex_jobs.py
+-rw-r--r--   0        0        0    10880 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/deployment/vertex_pipelines.py
+-rw-r--r--   0        0        0     7874 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/deployment/vertex_scheduling.py
+-rw-r--r--   0        0        0     2080 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/loggers/wanna_logger.py
+-rw-r--r--   0        0        0        0 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/models/__init__.py
+-rw-r--r--   0        0        0      879 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/models/base_instance.py
+-rw-r--r--   0        0        0      318 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/models/cloud_scheduler.py
+-rw-r--r--   0        0        0     1987 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/models/docker.py
+-rw-r--r--   0        0        0      834 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/models/gcp_components.py
+-rw-r--r--   0        0        0     1288 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/models/gcp_profile.py
+-rw-r--r--   0        0        0     1955 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/models/notebook.py
+-rw-r--r--   0        0        0      329 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/models/notification_channel.py
+-rw-r--r--   0        0        0      726 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/models/pipeline.py
+-rw-r--r--   0        0        0      203 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/models/tensorboard.py
+-rw-r--r--   0        0        0     4917 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/models/training_custom_job.py
+-rw-r--r--   0        0        0     2647 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/models/wanna_config.py
+-rw-r--r--   0        0        0      265 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/models/wanna_project.py
+-rw-r--r--   0        0        0        0 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/services/__init__.py
+-rw-r--r--   0        0        0     8519 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/services/base.py
+-rw-r--r--   0        0        0    16271 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/services/docker.py
+-rw-r--r--   0        0        0    19391 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/services/jobs.py
+-rw-r--r--   0        0        0    15064 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/services/managed_notebook.py
+-rw-r--r--   0        0        0    19408 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/services/notebook.py
+-rw-r--r--   0        0        0     4454 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/services/path_utils.py
+-rw-r--r--   0        0        0    13732 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/services/pipeline.py
+-rw-r--r--   0        0        0     8655 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/services/tensorboard.py
+-rw-r--r--   0        0        0        0 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/templates/__init__.py
+-rw-r--r--   0        0        0      655 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/templates/notebook_startup_script.sh.j2
+-rw-r--r--   0        0        0      239 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/templates/notebook_template.Dockerfile
+-rw-r--r--   0        0        0     1885 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/templates/scheduler_cloud_function.py
+-rw-r--r--   0        0        0      152 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/templates/scheduler_cloud_function_requirements.txt
+-rw-r--r--   0        0        0     1372 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/templates/sla_cloud_function.py
+-rw-r--r--   0        0        0      104 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/templates/sla_cloud_function_requirements.txt
+-rw-r--r--   0        0        0        0 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/utils/__init__.py
+-rw-r--r--   0        0        0     3694 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/utils/config_enricher.py
+-rw-r--r--   0        0        0     3021 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/utils/config_loader.py
+-rw-r--r--   0        0        0     1248 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/utils/credentials.py
+-rw-r--r--   0        0        0    12354 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/utils/gcp.py
+-rw-r--r--   0        0        0      545 2022-09-07 07:15:16.466216 wanna-ml-0.2.9/src/wanna/core/utils/json.py
+-rw-r--r--   0        0        0     1344 2022-09-07 07:15:16.470216 wanna-ml-0.2.9/src/wanna/core/utils/loaders.py
+-rw-r--r--   0        0        0      396 2022-09-07 07:15:16.470216 wanna-ml-0.2.9/src/wanna/core/utils/templates.py
+-rw-r--r--   0        0        0      104 2022-09-07 07:15:16.470216 wanna-ml-0.2.9/src/wanna/core/utils/time.py
+-rw-r--r--   0        0        0     5615 2022-09-07 07:15:16.470216 wanna-ml-0.2.9/src/wanna/core/utils/validators.py
+-rw-r--r--   0        0        0     6079 1970-01-01 00:00:00.000000 wanna-ml-0.2.9/setup.py
+-rw-r--r--   0        0        0     6551 1970-01-01 00:00:00.000000 wanna-ml-0.2.9/PKG-INFO
```

### Comparing `wanna-ml-0.2.8/README.md` & `wanna-ml-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/pyproject.toml` & `wanna-ml-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 authors = ["Joao Da Silva <joao.silva1@avast.com>", "Michal Mrazek <michal.mrazek@avast.com>"]
 description = "CLI tool for managing ML projects on Vertex AI"
 name = "wanna-ml"
-version = "v0.2.8"
+version = "v0.2.9"
 packages = [
     { include = "wanna", from = "src" },
 ]
 include = ["CHANGELOG.md"]
 readme = "README.md"
 license = "MIT"
 keywords = ["mlops", "vertex-ai", "GCP", "google-cloud-platform", "machine-learning"]
```

### Comparing `wanna-ml-0.2.8/src/wanna/cli/__main__.py` & `wanna-ml-0.2.9/src/wanna/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/cli/plugins/common_options.py` & `wanna-ml-0.2.9/src/wanna/cli/plugins/common_options.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/cli/plugins/components_plugin.py` & `wanna-ml-0.2.9/src/wanna/cli/plugins/components_plugin.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/cli/plugins/job_plugin.py` & `wanna-ml-0.2.9/src/wanna/cli/plugins/job_plugin.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/cli/plugins/managed_notebook_plugin.py` & `wanna-ml-0.2.9/src/wanna/cli/plugins/managed_notebook_plugin.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/cli/plugins/notebook_plugin.py` & `wanna-ml-0.2.9/src/wanna/cli/plugins/notebook_plugin.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/cli/plugins/pipeline_plugin.py` & `wanna-ml-0.2.9/src/wanna/cli/plugins/pipeline_plugin.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/cli/plugins/runner.py` & `wanna-ml-0.2.9/src/wanna/cli/plugins/runner.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/cli/plugins/tensorboard_plugin.py` & `wanna-ml-0.2.9/src/wanna/cli/plugins/tensorboard_plugin.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/cli/version.py` & `wanna-ml-0.2.9/src/wanna/cli/version.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/components/kubeflow/get_or_create_endpoint.py` & `wanna-ml-0.2.9/src/wanna/components/kubeflow/get_or_create_endpoint.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/components/template.py` & `wanna-ml-0.2.9/src/wanna/components/template.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/components/templates/base/cookiecutter.json` & `wanna-ml-0.2.9/src/wanna/components/templates/base/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/Dockerfile` & `wanna-ml-0.2.9/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/Dockerfile`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/component.yaml` & `wanna-ml-0.2.9/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/component.yaml`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/setup.py` & `wanna-ml-0.2.9/src/wanna/components/templates/base/{{ cookiecutter.component_slug }}/setup.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/deployment/artifacts_push.py` & `wanna-ml-0.2.9/src/wanna/core/deployment/artifacts_push.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/deployment/io.py` & `wanna-ml-0.2.9/src/wanna/core/deployment/io.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/deployment/models.py` & `wanna-ml-0.2.9/src/wanna/core/deployment/models.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/deployment/monitoring.py` & `wanna-ml-0.2.9/src/wanna/core/deployment/monitoring.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/deployment/vertex_jobs.py` & `wanna-ml-0.2.9/src/wanna/core/deployment/vertex_jobs.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/deployment/vertex_pipelines.py` & `wanna-ml-0.2.9/src/wanna/core/deployment/vertex_pipelines.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/deployment/vertex_scheduling.py` & `wanna-ml-0.2.9/src/wanna/core/deployment/vertex_scheduling.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/loggers/wanna_logger.py` & `wanna-ml-0.2.9/src/wanna/core/loggers/wanna_logger.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/models/base_instance.py` & `wanna-ml-0.2.9/src/wanna/core/models/base_instance.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/models/docker.py` & `wanna-ml-0.2.9/src/wanna/core/models/docker.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/models/gcp_components.py` & `wanna-ml-0.2.9/src/wanna/core/models/gcp_components.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/models/gcp_profile.py` & `wanna-ml-0.2.9/src/wanna/core/models/gcp_profile.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/models/notebook.py` & `wanna-ml-0.2.9/src/wanna/core/models/notebook.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/models/pipeline.py` & `wanna-ml-0.2.9/src/wanna/core/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/models/training_custom_job.py` & `wanna-ml-0.2.9/src/wanna/core/models/training_custom_job.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/models/wanna_config.py` & `wanna-ml-0.2.9/src/wanna/core/models/wanna_config.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/services/base.py` & `wanna-ml-0.2.9/src/wanna/core/services/base.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/services/docker.py` & `wanna-ml-0.2.9/src/wanna/core/services/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,18 +344,24 @@
             f"{self.docker_registry}/{self.docker_registry_suffix}{self.docker_project_id}/"
             f"{self.docker_repository}/{self.wanna_project_name}/{image_name}:{version}"
             for version in versions
         ]
 
     def build_container_and_get_image_url(self, docker_image_ref: str, push_mode: PushMode = PushMode.all) -> str:
         if push_mode == PushMode.quick:
+            # only get image tag
             docker_image_model = self.find_image_model_by_name(docker_image_ref)
             tags = self.construct_image_tag(image_name=docker_image_model.name)
             image_url = tags[0]
+        elif push_mode == PushMode.manifests:
+            # only build image
+            image_tag = self.get_image(docker_image_ref=docker_image_ref)
+            image_url = image_tag[2]
         else:
+            # build image and push
             image_tag = self.get_image(docker_image_ref=docker_image_ref)
             if len(image_tag) > 1 and image_tag[1]:
                 self.push_image(image_tag[1])
             image_url = image_tag[2]
         return image_url
 
     @staticmethod
```

### Comparing `wanna-ml-0.2.8/src/wanna/core/services/jobs.py` & `wanna-ml-0.2.9/src/wanna/core/services/jobs.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/services/managed_notebook.py` & `wanna-ml-0.2.9/src/wanna/core/services/managed_notebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,15 +340,15 @@
             ):
                 to_be_created.append(notebook)
 
         return to_be_deleted, to_be_created
 
     def build(self) -> int:
         for instance in self.instances:
-            self._create_runtime_request(instance=instance, deploy=False)
+            self._create_runtime_request(instance=instance, deploy=False, push_mode=PushMode.manifests)
         logger.user_success("Managed notebooks validation OK!")
         return 0
 
     def push(self, instance_name: str):
         instances = self._filter_instances_by_name(instance_name)
 
         docker_image_refs = set(
```

### Comparing `wanna-ml-0.2.8/src/wanna/core/services/notebook.py` & `wanna-ml-0.2.9/src/wanna/core/services/notebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,15 +399,15 @@
                 )
             else:
                 logger.user_error(f"No notebook {instance_name} found")
                 raise ValueError(f"Notebook {instance_name} does not exists in configuration")
 
     def build(self) -> int:
         for instance in self.instances:
-            self._create_instance_request(notebook_instance=instance, deploy=False)
+            self._create_instance_request(notebook_instance=instance, deploy=False, push_mode=PushMode.manifests)
         logger.user_success("Notebooks validation OK!")
         return 0
 
     def push(self, instance_name: str):
         instances = self._filter_instances_by_name(instance_name)
 
         docker_image_refs = set(
```

### Comparing `wanna-ml-0.2.8/src/wanna/core/services/path_utils.py` & `wanna-ml-0.2.9/src/wanna/core/services/path_utils.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/services/pipeline.py` & `wanna-ml-0.2.9/src/wanna/core/services/pipeline.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/services/tensorboard.py` & `wanna-ml-0.2.9/src/wanna/core/services/tensorboard.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/templates/notebook_startup_script.sh.j2` & `wanna-ml-0.2.9/src/wanna/core/templates/notebook_startup_script.sh.j2`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/templates/scheduler_cloud_function.py` & `wanna-ml-0.2.9/src/wanna/core/templates/scheduler_cloud_function.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/templates/sla_cloud_function.py` & `wanna-ml-0.2.9/src/wanna/core/templates/sla_cloud_function.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/utils/config_enricher.py` & `wanna-ml-0.2.9/src/wanna/core/utils/config_enricher.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/utils/config_loader.py` & `wanna-ml-0.2.9/src/wanna/core/utils/config_loader.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/utils/credentials.py` & `wanna-ml-0.2.9/src/wanna/core/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/utils/gcp.py` & `wanna-ml-0.2.9/src/wanna/core/utils/gcp.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/utils/json.py` & `wanna-ml-0.2.9/src/wanna/core/utils/json.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/utils/loaders.py` & `wanna-ml-0.2.9/src/wanna/core/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/src/wanna/core/utils/validators.py` & `wanna-ml-0.2.9/src/wanna/core/utils/validators.py`

 * *Files identical despite different names*

### Comparing `wanna-ml-0.2.8/setup.py` & `wanna-ml-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
  'waiting>=1.4.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['wanna = wanna.cli.__main__:wanna']}
 
 setup_kwargs = {
     'name': 'wanna-ml',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'CLI tool for managing ML projects on Vertex AI',
     'long_description': '# WANNA-ML\n\n---\n\n<p align="center" font-style="italic"> \n<em> Complete MLOps framework for Vertex-AI  </em>\n</p>\n\n---\n\n<p align="center">\n<a href="https://github.com/avast/wanna-ml/actions/workflows/build.yml" target="_blank">\n    <img src="https://github.com/avast/wanna-ml/actions/workflows/build.yml/badge.svg" alt="Build">\n</a>\n<a href="https://github.com/avast/wanna-ml/actions/workflows/release.yml" target="_blank">\n    <img src="https://github.com/avast/wanna-ml/actions/workflows/release.yml/badge.svg" alt="Release">\n</a>\n<a href="https://codecov.io/gh/avast/wanna-ml" target="_blank">\n    <img src="https://codecov.io/gh/avast/wanna-ml/branch/master/graph/badge.svg?token=TAFWK4GJPR" alt="Coverage">\n</a>\n<a href="https://pypi.org/project/wanna-ml/" target="_blank">\n    <img src="https://img.shields.io/pypi/v/wanna-ml?color=%2334D058&label=pypi%20package" alt="Package version">\n</a>\n</p>\n\n# About WANNA-ML\n\nWANNA-ML is a CLI tool that helps researchers, data scientists, and ML Engineers quickly adapt to Google Cloud Platform (GCP) and get started on the cloud in almost no time.\n\nIt makes it easy to start a Jupyter notebook, run training jobs and pipelines, build a Docker container, export logs to Tensorboards, and much more.\n\nWe build on top of Vertex-AI managed services and integrate with other GCP services like Cloud Build and Artifact Registry to provide you with a standardized structure for managing ML assets on GCP.\n\n\n## Help\n\nSee the [documentation](https://avast.github.io/wanna-ml/) for more details.\n\n\n## Get started\n\n### Installation\nInstall using `pip install -U wanna-ml`.\n\nFor more information on the installation process and requirements, visit out [installation page in documentation](https://avast.github.io/wanna-ml/installation)\n\n### Use Docker Image\nFor your convenience, we have prepared a Docker image with everything you need to get started.\n```bash\ndocker pull michalmrazek9/wanna-ml\n\ndocker run -it michalmrazek9/wanna-ml\n\n$ wanna version\n```\n\n### Authentication\nWANNA-ML relies on `gcloud` for user authentication. \n\n1. Install the `gcloud` CLI - follow [official guide](https://cloud.google.com/sdk/docs/install)\n2. Authenticate with the `gcloud init`\n3. Set you Google Application Credentials `gcloud auth application-default login`\n\n### Docker Build\nYou can use a local Docker daemon to build Docker images, but it is not required. \nYou are free to choose between local building on GCP Cloud Build. \nIf you prefer local Docker image building, install  [Docker Desktop](https://www.docker.com/products/docker-desktop/).\n\n### GCP IAM Roles and Permissions\nDifferent WANNA-ML calls require different GCP permissions to create given resources on GCP. Our [documentation page](https://avast.github.io/wanna-ml/)\nlists recommended GCP IAM roles for each `wanna` command.\n\n## Examples\nJump to [the samples](https://github.com/avast/wanna-ml/tree/master/samples) to see a complete solution \nfor various use cases.\n\n## Issues\nPlease report issues to [GitHub](https://github.com/avast/wanna-ml/issues).\n\n## Contributing\nYour contributions are always welcome, see [CONTRIBUTING.md](https://github.com/avast/wanna-ml/blob/master/CONTRIBUTING.md) for more information.\nIf you like WANNA-ML, don\'t forget to give our project a star! \n\n## Licence\nDistributed under the MIT License - see [LICENSE](https://github.com/avast/wanna-ml/blob/master/LICENCE).\n',
     'author': 'Joao Da Silva',
     'author_email': 'joao.silva1@avast.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://avast.github.io/wanna-ml',
```

#### html2text {}

```diff
@@ -23,15 +23,15 @@
 'mkdocstrings-python>=0.7.1,<0.8.0', 'mkdocstrings>=0.19.0,<0.20.0',
 'packaging>=21.3,<22.0', 'pathvalidate>=2.5.0,<3.0.0',
 'pydantic>=1.9.0,<2.0.0', 'python-on-whales>=0.43.0,<0.44.0', 'pyyaml-
 include>=1.3,<2.0', 'rich>=12.5.1,<13.0.0', 'smart-open[gcs]>=6.0,<7.0',
 'treelib>=1.6.1,<2.0.0', 'typer==0.6.1', 'types-setuptools>=63.2.3,<64.0.0',
 'waiting>=1.4.1,<2.0.0'] entry_points = \ {'console_scripts': ['wanna =
 wanna.cli.__main__:wanna']} setup_kwargs = { 'name': 'wanna-ml', 'version':
-'0.2.8', 'description': 'CLI tool for managing ML projects on Vertex AI',
+'0.2.9', 'description': 'CLI tool for managing ML projects on Vertex AI',
 'long_description': '# WANNA-ML\n\n---\n\n
                   \nComplete MLOps framework for Vertex-AI\n
 \n\n---\n\n
    \n\n_[Build]\n\n\n_[Release]\n\n\n_[Coverage]\n\n\n_[Package_version]\n\n
 \n\n# About WANNA-ML\n\nWANNA-ML is a CLI tool that helps researchers, data
 scientists, and ML Engineers quickly adapt to Google Cloud Platform (GCP) and
 get started on the cloud in almost no time.\n\nIt makes it easy to start a
```

### Comparing `wanna-ml-0.2.8/PKG-INFO` & `wanna-ml-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wanna-ml
-Version: 0.2.8
+Version: 0.2.9
 Summary: CLI tool for managing ML projects on Vertex AI
 Home-page: https://avast.github.io/wanna-ml
 License: MIT
 Keywords: mlops,vertex-ai,GCP,google-cloud-platform,machine-learning
 Author: Joao Da Silva
 Author-email: joao.silva1@avast.com
 Requires-Python: >=3.7,<3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wanna-ml Version: 0.2.8 Summary: CLI tool for
+Metadata-Version: 2.1 Name: wanna-ml Version: 0.2.9 Summary: CLI tool for
 managing ML projects on Vertex AI Home-page: https://avast.github.io/wanna-ml
 License: MIT Keywords: mlops,vertex-ai,GCP,google-cloud-platform,machine-
 learning Author: Joao Da Silva Author-email: joao.silva1@avast.com Requires-
 Python: >=3.7,<3.11 Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

