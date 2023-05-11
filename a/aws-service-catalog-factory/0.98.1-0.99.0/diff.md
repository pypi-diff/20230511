# Comparing `tmp/aws_service_catalog_factory-0.98.1.tar.gz` & `tmp/aws_service_catalog_factory-0.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_service_catalog_factory-0.98.1.tar", max compression
+gzip compressed data, was "aws_service_catalog_factory-0.99.0.tar", max compression
```

## Comparing `aws_service_catalog_factory-0.98.1.tar` & `aws_service_catalog_factory-0.99.0.tar`

### file list

```diff
@@ -1,119 +1,120 @@
--rw-r--r--   0        0        0    10142 2023-03-03 15:02:58.351145 aws_service_catalog_factory-0.98.1/LICENSE
--rw-r--r--   0        0        0     1395 2023-03-03 15:02:58.355145 aws_service_catalog_factory-0.98.1/README.md
--rw-r--r--   0        0        0     1969 2023-03-03 15:05:22.031267 aws_service_catalog_factory-0.98.1/pyproject.toml
--rw-r--r--   0        0        0      114 2023-03-03 15:02:58.395145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/__init__.py
--rw-r--r--   0        0        0     2471 2023-03-03 15:02:58.399145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/aws.py
--rwxr-xr-x   0        0        0    21375 2023-03-03 15:02:58.399145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/cli.py
--rw-r--r--   0        0        0     6793 2023-03-03 15:02:58.399145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/cloudformation_servicecatalog_deploy_action.py
--rw-r--r--   0        0        0      114 2023-03-03 15:02:58.399145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/__init__.py
--rw-r--r--   0        0        0     9353 2023-03-03 15:02:58.403145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/bootstrap.py
--rw-r--r--   0        0        0     2018 2023-03-03 15:02:58.403145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/bootstrap_test.py
--rw-r--r--   0        0        0     1981 2023-03-03 15:02:58.403145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/configuration_management.py
--rw-r--r--   0        0        0     3256 2023-03-03 15:02:58.403145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/extract_from_ssm.py
--rw-r--r--   0        0        0     3715 2023-03-03 15:02:58.403145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/generate.py
--rw-r--r--   0        0        0     1904 2023-03-03 15:02:58.403145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/list_resources.py
--rw-r--r--   0        0        0     1137 2023-03-03 15:02:58.403145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/management.py
--rw-r--r--   0        0        0    25820 2023-03-03 15:02:58.407145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/portfolios.py
--rw-r--r--   0        0        0      557 2023-03-03 15:02:58.407145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/seed.py
--rw-r--r--   0        0        0     9177 2023-03-03 15:02:58.407145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/show_pipelines.py
--rw-r--r--   0        0        0     1551 2023-03-03 15:02:58.407145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/stacks.py
--rw-r--r--   0        0        0    33941 2023-03-03 15:03:49.139187 aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/task_reference.py
--rw-r--r--   0        0        0     1613 2023-03-03 15:02:58.407145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/validate.py
--rw-r--r--   0        0        0      877 2023-03-03 15:02:58.407145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/version.py
--rw-r--r--   0        0        0     1604 2023-03-03 15:02:58.407145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/common/serialisation_utils.py
--rw-r--r--   0        0        0      719 2023-03-03 15:02:58.407145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/common/utils.py
--rw-r--r--   0        0        0     3140 2023-03-03 15:02:58.411145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/config.py
--rw-r--r--   0        0        0     3542 2023-03-03 15:02:58.411145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/constants.py
--rw-r--r--   0        0        0     3711 2023-03-03 15:02:58.411145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/constants_test.py
--rw-r--r--   0        0        0      285 2023-03-03 15:02:58.411145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/empty.template.yaml
--rw-r--r--   0        0        0      195 2023-03-03 15:02:58.411145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/environmental_variables.py
--rw-r--r--   0        0        0       57 2023-03-03 15:02:58.411145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/example-config-small.yaml
--rw-r--r--   0        0        0      265 2023-03-03 15:02:58.411145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/example-config.yaml
--rw-r--r--   0        0        0     3424 2023-03-03 15:02:58.415145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/portfolios/ccoe.yaml
--rw-r--r--   0        0        0     4983 2023-03-03 15:02:58.415145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/portfolios/example-quickstart.yaml
--rw-r--r--   0        0        0     1186 2023-03-03 15:02:58.415145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/portfolios/example-simple-github.yaml
--rw-r--r--   0        0        0     1192 2023-03-03 15:02:58.415145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/portfolios/example-simple.yaml
--rw-r--r--   0        0        0     2938 2023-03-03 15:02:58.415145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/schema/schema-apps.yaml
--rw-r--r--   0        0        0     5735 2023-03-03 15:02:58.415145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/schema/schema-portfolios.yaml
--rw-r--r--   0        0        0     4498 2023-03-03 15:02:58.415145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/schema/schema-stacks.yaml
--rw-r--r--   0        0        0     3608 2023-03-03 15:02:58.415145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/schema/schema-workspaces.yaml
--rwxr-xr-x   0        0        0     4416 2023-03-03 15:02:58.415145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/sdk.py
--rw-r--r--   0        0        0    13343 2023-03-03 15:02:58.415145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/servicecatalog-factory-initialiser.template.yaml
--rw-r--r--   0        0        0     1874 2023-03-03 15:02:58.415145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/servicecatalog-factory-regional.template.yaml
--rw-r--r--   0        0        0     8509 2023-03-03 15:02:58.419145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/servicecatalog-factory-secondary.template.yaml
--rw-r--r--   0        0        0    17682 2023-03-03 15:02:58.419145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/servicecatalog-factory.template.yaml
--rw-r--r--   0        0        0     3336 2023-03-03 15:02:58.419145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/tasks_unit_tests_helper.py
--rw-r--r--   0        0        0      114 2023-03-03 15:02:58.419145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/__init__.py
--rw-r--r--   0        0        0      662 2023-03-03 15:02:58.419145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/base_template.py
--rw-r--r--   0        0        0      114 2023-03-03 15:02:58.439145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/cdk/__init__.py
--rw-r--r--   0        0        0    20607 2023-03-03 15:02:58.439145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/cdk/product_pipeline.py
--rw-r--r--   0        0        0    13553 2023-03-03 15:02:58.439145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/cdk/product_template.py
--rw-r--r--   0        0        0     6776 2023-03-03 15:02:58.439145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/cdk/shared_resources.py
--rw-r--r--   0        0        0      114 2023-03-03 15:02:58.451145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/pipeline/__init__.py
--rw-r--r--   0        0        0     5329 2023-03-03 15:02:58.451145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/pipeline/build.py
--rw-r--r--   0        0        0    17176 2023-03-03 15:02:58.451145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/pipeline/deploy.py
--rw-r--r--   0        0        0    19523 2023-03-03 15:02:58.451145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/pipeline/package.py
--rw-r--r--   0        0        0     6083 2023-03-03 15:02:58.451145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/pipeline/pipeline_template_builder.py
--rw-r--r--   0        0        0     4624 2023-03-03 15:02:58.451145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/pipeline/source.py
--rw-r--r--   0        0        0    18241 2023-03-03 15:02:58.455145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/pipeline/test.py
--rw-r--r--   0        0        0      270 2023-03-03 15:02:58.455145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/pipeline/utils.py
--rw-r--r--   0        0        0      378 2023-03-03 15:02:58.455145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/product_template_factory.py
--rw-r--r--   0        0        0      620 2023-03-03 15:02:58.455145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/product_templates.py
--rw-r--r--   0        0        0    21359 2023-03-03 15:02:58.455145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/shared_resources.py
--rw-r--r--   0        0        0        0 2023-03-03 15:02:58.455145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/troposphere_contstants/__init__.py
--rw-r--r--   0        0        0      510 2023-03-03 15:02:58.455145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/troposphere_contstants/codebuild.py
--rw-r--r--   0        0        0      626 2023-03-03 15:02:58.455145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/templates/associations.j2
--rw-r--r--   0        0        0      661 2023-03-03 15:02:58.459145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/templates/constraint-launch-role-nested.template.yaml
--rw-r--r--   0        0        0      565 2023-03-03 15:02:58.459145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/templates/constraint-launch-role-parent.template.yaml
--rw-r--r--   0        0        0     8752 2023-03-03 15:02:58.459145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/templates/product-terraform.j2
--rw-r--r--   0        0        0      882 2023-03-03 15:02:58.459145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/templates/static-html-page.html
--rw-r--r--   0        0        0     8903 2023-03-03 15:02:58.459145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/templates/terraform.template.yaml.j2
--rw-r--r--   0        0        0      983 2023-03-03 15:02:58.459145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/templates/test-action.j2
--rw-r--r--   0        0        0      114 2023-03-03 15:02:58.459145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/utilities/__init__.py
--rw-r--r--   0        0        0      384 2023-03-03 15:02:58.463145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/utilities/assets.py
--rw-r--r--   0        0        0     1094 2023-03-03 15:02:58.463145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/utilities/assets_test.py
--rw-r--r--   0        0        0     1212 2023-03-03 15:02:58.463145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/utils.py
--rw-r--r--   0        0        0      114 2023-03-03 15:02:58.463145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/waluigi/__init__.py
--rw-r--r--   0        0        0    16791 2023-03-03 15:02:58.463145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/waluigi/scheduler.py
--rw-r--r--   0        0        0     5861 2023-03-03 15:02:58.463145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/waluigi/tasks.py
--rw-r--r--   0        0        0      114 2023-03-03 15:02:58.463145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/__init__.py
--rw-r--r--   0        0        0      114 2023-03-03 15:02:58.467145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/codecommit/__init__.py
--rw-r--r--   0        0        0     2901 2023-03-03 15:02:58.467145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/codecommit/create_code_repo_task.py
--rw-r--r--   0        0        0     1414 2023-03-03 15:02:58.467145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/codecommit/create_code_repo_task_test.py
--rw-r--r--   0        0        0      114 2023-03-03 15:02:58.467145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/dependencies/__init__.py
--rw-r--r--   0        0        0     8239 2023-03-03 15:02:58.467145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/dependencies/reservable_resources.py
--rw-r--r--   0        0        0     4266 2023-03-03 15:02:58.467145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/dependencies/resources_factory.py
--rw-r--r--   0        0        0      776 2023-03-03 15:02:58.467145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/dependencies/section_names.py
--rw-r--r--   0        0        0    10181 2023-03-03 15:02:58.471145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/dependencies/task_factory.py
--rw-r--r--   0        0        0      114 2023-03-03 15:02:58.471145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/generic/__init__.py
--rw-r--r--   0        0        0     2158 2023-03-03 15:02:58.471145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/generic/create_generic_version_pipeline_task.py
--rw-r--r--   0        0        0      490 2023-03-03 15:02:58.471145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/generic/delete_stack_task.py
--rw-r--r--   0        0        0      114 2023-03-03 15:02:58.471145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/__init__.py
--rw-r--r--   0        0        0     1609 2023-03-03 15:02:58.471145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/associate_product_with_portfolio_task.py
--rw-r--r--   0        0        0     1751 2023-03-03 15:02:58.471145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/associate_product_with_portfolio_task_test.py
--rw-r--r--   0        0        0     1893 2023-03-03 15:02:58.471145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/associate_tag_option_task.py
--rw-r--r--   0        0        0     1774 2023-03-03 15:02:58.475145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_combined_product_pipeline_task.py
--rw-r--r--   0        0        0     1613 2023-03-03 15:02:58.475145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_combined_product_pipeline_task_test.py
--rw-r--r--   0        0        0     2089 2023-03-03 15:02:58.475145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_launch_role_name_constraints_task.py
--rw-r--r--   0        0        0     1877 2023-03-03 15:02:58.475145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_portfolio_association_task.py
--rw-r--r--   0        0        0     1870 2023-03-03 15:02:58.475145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_portfolio_association_task_test.py
--rw-r--r--   0        0        0     1588 2023-03-03 15:02:58.475145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_portfolio_task.py
--rw-r--r--   0        0        0     1479 2023-03-03 15:02:58.479145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_portfolio_task_test.py
--rw-r--r--   0        0        0     6085 2023-03-03 15:02:58.479145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_product_task.py
--rw-r--r--   0        0        0     1994 2023-03-03 15:02:58.479145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_product_task_test.py
--rw-r--r--   0        0        0     1315 2023-03-03 15:02:58.479145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_tag_option_task.py
--rw-r--r--   0        0        0     2544 2023-03-03 15:02:58.479145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_version_pipeline_task.py
--rw-r--r--   0        0        0     1893 2023-03-03 15:02:58.479145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_version_pipeline_task_test.py
--rw-r--r--   0        0        0     2436 2023-03-03 15:02:58.479145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/delete_a_version_task.py
--rw-r--r--   0        0        0     1490 2023-03-03 15:02:58.479145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/delete_a_version_task_test.py
--rw-r--r--   0        0        0     2374 2023-03-03 15:02:58.479145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/delete_product_from_service_catalog_task.py
--rw-r--r--   0        0        0     3706 2023-03-03 15:02:58.479145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/delete_product_task.py
--rw-r--r--   0        0        0     1364 2023-03-03 15:02:58.479145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/delete_product_task_test.py
--rw-r--r--   0        0        0     2057 2023-03-03 15:02:58.483145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/ensure_product_version_details_correct_task.py
--rw-r--r--   0        0        0     1604 2023-03-03 15:02:58.483145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/ensure_product_version_details_correct_task_test.py
--rw-r--r--   0        0        0     1175 2023-03-03 15:02:58.483145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/get_bucket_task.py
--rw-r--r--   0        0        0     1056 2023-03-03 15:02:58.483145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/get_bucket_task_test.py
--rw-r--r--   0        0        0     4199 2023-03-03 15:02:58.483145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/tasks.py
--rw-r--r--   0        0        0     3747 2023-03-03 15:02:58.483145 aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/tasks_unit_tests_helper.py
--rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 aws_service_catalog_factory-0.98.1/setup.py
--rw-r--r--   0        0        0     3614 1970-01-01 00:00:00.000000 aws_service_catalog_factory-0.98.1/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-03-13 17:31:58.410717 aws_service_catalog_factory-0.99.0/LICENSE
+-rw-r--r--   0        0        0     1395 2023-03-13 17:31:58.410717 aws_service_catalog_factory-0.99.0/README.md
+-rw-r--r--   0        0        0     1969 2023-03-13 17:34:18.550927 aws_service_catalog_factory-0.99.0/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-03-13 17:31:58.446717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/__init__.py
+-rw-r--r--   0        0        0     2471 2023-03-13 17:31:58.450717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/aws.py
+-rwxr-xr-x   0        0        0    21375 2023-03-13 17:31:58.450717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/cli.py
+-rw-r--r--   0        0        0     6793 2023-03-13 17:31:58.450717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/cloudformation_servicecatalog_deploy_action.py
+-rw-r--r--   0        0        0      114 2023-03-13 17:31:58.450717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/__init__.py
+-rw-r--r--   0        0        0     9353 2023-03-13 17:31:58.450717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/bootstrap.py
+-rw-r--r--   0        0        0     2018 2023-03-13 17:31:58.450717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/bootstrap_test.py
+-rw-r--r--   0        0        0     1981 2023-03-13 17:31:58.450717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/configuration_management.py
+-rw-r--r--   0        0        0     3256 2023-03-13 17:31:58.450717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/extract_from_ssm.py
+-rw-r--r--   0        0        0     3715 2023-03-13 17:31:58.450717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/generate.py
+-rw-r--r--   0        0        0     1904 2023-03-13 17:31:58.450717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/list_resources.py
+-rw-r--r--   0        0        0     1137 2023-03-13 17:31:58.450717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/management.py
+-rw-r--r--   0        0        0    25820 2023-03-13 17:31:58.450717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/portfolios.py
+-rw-r--r--   0        0        0      557 2023-03-13 17:31:58.450717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/seed.py
+-rw-r--r--   0        0        0     9177 2023-03-13 17:31:58.450717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/show_pipelines.py
+-rw-r--r--   0        0        0     1551 2023-03-13 17:31:58.450717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/stacks.py
+-rw-r--r--   0        0        0    36064 2023-03-13 17:31:58.450717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/task_reference.py
+-rw-r--r--   0        0        0     1613 2023-03-13 17:31:58.450717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/validate.py
+-rw-r--r--   0        0        0      877 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/version.py
+-rw-r--r--   0        0        0     1604 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/common/serialisation_utils.py
+-rw-r--r--   0        0        0      719 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/common/utils.py
+-rw-r--r--   0        0        0     3140 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/config.py
+-rw-r--r--   0        0        0     3509 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/constants.py
+-rw-r--r--   0        0        0     3662 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/constants_test.py
+-rw-r--r--   0        0        0      285 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/empty.template.yaml
+-rw-r--r--   0        0        0      195 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/environmental_variables.py
+-rw-r--r--   0        0        0       57 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/example-config-small.yaml
+-rw-r--r--   0        0        0      265 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/example-config.yaml
+-rw-r--r--   0        0        0     3424 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/portfolios/ccoe.yaml
+-rw-r--r--   0        0        0     4983 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/portfolios/example-quickstart.yaml
+-rw-r--r--   0        0        0     1186 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/portfolios/example-simple-github.yaml
+-rw-r--r--   0        0        0     1192 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/portfolios/example-simple.yaml
+-rw-r--r--   0        0        0     2938 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/schema/schema-apps.yaml
+-rw-r--r--   0        0        0     5735 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/schema/schema-portfolios.yaml
+-rw-r--r--   0        0        0     4498 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/schema/schema-stacks.yaml
+-rw-r--r--   0        0        0     3608 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/schema/schema-workspaces.yaml
+-rwxr-xr-x   0        0        0     4416 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/sdk.py
+-rw-r--r--   0        0        0    13343 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/servicecatalog-factory-initialiser.template.yaml
+-rw-r--r--   0        0        0     1874 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/servicecatalog-factory-regional.template.yaml
+-rw-r--r--   0        0        0     8509 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/servicecatalog-factory-secondary.template.yaml
+-rw-r--r--   0        0        0    17682 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/servicecatalog-factory.template.yaml
+-rw-r--r--   0        0        0     3336 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/tasks_unit_tests_helper.py
+-rw-r--r--   0        0        0      114 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/__init__.py
+-rw-r--r--   0        0        0      662 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/base_template.py
+-rw-r--r--   0        0        0      114 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/cdk/__init__.py
+-rw-r--r--   0        0        0    20607 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/cdk/product_pipeline.py
+-rw-r--r--   0        0        0    13553 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/cdk/product_template.py
+-rw-r--r--   0        0        0     6776 2023-03-13 17:31:58.454717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/cdk/shared_resources.py
+-rw-r--r--   0        0        0      114 2023-03-13 17:31:58.482717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/pipeline/__init__.py
+-rw-r--r--   0        0        0     5329 2023-03-13 17:31:58.482717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/pipeline/build.py
+-rw-r--r--   0        0        0    17176 2023-03-13 17:31:58.482717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/pipeline/deploy.py
+-rw-r--r--   0        0        0    19523 2023-03-13 17:31:58.482717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/pipeline/package.py
+-rw-r--r--   0        0        0     6083 2023-03-13 17:31:58.482717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/pipeline/pipeline_template_builder.py
+-rw-r--r--   0        0        0     4624 2023-03-13 17:31:58.482717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/pipeline/source.py
+-rw-r--r--   0        0        0    18241 2023-03-13 17:31:58.482717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/pipeline/test.py
+-rw-r--r--   0        0        0      270 2023-03-13 17:31:58.482717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/pipeline/utils.py
+-rw-r--r--   0        0        0      378 2023-03-13 17:31:58.482717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/product_template_factory.py
+-rw-r--r--   0        0        0      620 2023-03-13 17:31:58.482717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/product_templates.py
+-rw-r--r--   0        0        0    21359 2023-03-13 17:31:58.482717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/shared_resources.py
+-rw-r--r--   0        0        0        0 2023-03-13 17:31:58.482717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/troposphere_contstants/__init__.py
+-rw-r--r--   0        0        0      510 2023-03-13 17:31:58.482717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/troposphere_contstants/codebuild.py
+-rw-r--r--   0        0        0      661 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/templates/constraint-launch-role-nested.template.yaml
+-rw-r--r--   0        0        0      565 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/templates/constraint-launch-role-parent.template.yaml
+-rw-r--r--   0        0        0     8752 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/templates/product-terraform.j2
+-rw-r--r--   0        0        0      882 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/templates/static-html-page.html
+-rw-r--r--   0        0        0     8903 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/templates/terraform.template.yaml.j2
+-rw-r--r--   0        0        0      983 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/templates/test-action.j2
+-rw-r--r--   0        0        0      114 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/utilities/__init__.py
+-rw-r--r--   0        0        0      384 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/utilities/assets.py
+-rw-r--r--   0        0        0     1094 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/utilities/assets_test.py
+-rw-r--r--   0        0        0     1482 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/utils.py
+-rw-r--r--   0        0        0      114 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/waluigi/__init__.py
+-rw-r--r--   0        0        0    16791 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/waluigi/scheduler.py
+-rw-r--r--   0        0        0     5861 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/waluigi/tasks.py
+-rw-r--r--   0        0        0      114 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/__init__.py
+-rw-r--r--   0        0        0      114 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/codecommit/__init__.py
+-rw-r--r--   0        0        0     2901 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/codecommit/create_code_repo_task.py
+-rw-r--r--   0        0        0     1414 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/codecommit/create_code_repo_task_test.py
+-rw-r--r--   0        0        0      114 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/dependencies/__init__.py
+-rw-r--r--   0        0        0     8239 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/dependencies/reservable_resources.py
+-rw-r--r--   0        0        0     4612 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/dependencies/resources_factory.py
+-rw-r--r--   0        0        0      902 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/dependencies/section_names.py
+-rw-r--r--   0        0        0    11360 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/dependencies/task_factory.py
+-rw-r--r--   0        0        0      114 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/generic/__init__.py
+-rw-r--r--   0        0        0     2158 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/generic/create_generic_version_pipeline_task.py
+-rw-r--r--   0        0        0      490 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/generic/delete_stack_task.py
+-rw-r--r--   0        0        0      114 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/__init__.py
+-rw-r--r--   0        0        0     1609 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/associate_product_with_portfolio_task.py
+-rw-r--r--   0        0        0     1751 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/associate_product_with_portfolio_task_test.py
+-rw-r--r--   0        0        0      279 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/associate_products_tasks.py
+-rw-r--r--   0        0        0     1893 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/associate_tag_option_task.py
+-rw-r--r--   0        0        0     1774 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_combined_product_pipeline_task.py
+-rw-r--r--   0        0        0     1613 2023-03-13 17:31:58.510717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_combined_product_pipeline_task_test.py
+-rw-r--r--   0        0        0     2089 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_launch_role_name_constraints_task.py
+-rw-r--r--   0        0        0     3241 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_portfolio_association_task.py
+-rw-r--r--   0        0        0     1870 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_portfolio_association_task_test.py
+-rw-r--r--   0        0        0     5973 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_portfolio_constraints_task.py
+-rw-r--r--   0        0        0     1588 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_portfolio_task.py
+-rw-r--r--   0        0        0     1479 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_portfolio_task_test.py
+-rw-r--r--   0        0        0     6085 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_product_task.py
+-rw-r--r--   0        0        0     1994 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_product_task_test.py
+-rw-r--r--   0        0        0     1315 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_tag_option_task.py
+-rw-r--r--   0        0        0     2544 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_version_pipeline_task.py
+-rw-r--r--   0        0        0     1893 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_version_pipeline_task_test.py
+-rw-r--r--   0        0        0     2436 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/delete_a_version_task.py
+-rw-r--r--   0        0        0     1490 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/delete_a_version_task_test.py
+-rw-r--r--   0        0        0     2374 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/delete_product_from_service_catalog_task.py
+-rw-r--r--   0        0        0     3706 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/delete_product_task.py
+-rw-r--r--   0        0        0     1364 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/delete_product_task_test.py
+-rw-r--r--   0        0        0     2057 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/ensure_product_version_details_correct_task.py
+-rw-r--r--   0        0        0     1604 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/ensure_product_version_details_correct_task_test.py
+-rw-r--r--   0        0        0     1175 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/get_bucket_task.py
+-rw-r--r--   0        0        0     1056 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/get_bucket_task_test.py
+-rw-r--r--   0        0        0     4630 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/tasks.py
+-rw-r--r--   0        0        0     3747 2023-03-13 17:31:58.514717 aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/tasks_unit_tests_helper.py
+-rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 aws_service_catalog_factory-0.99.0/setup.py
+-rw-r--r--   0        0        0     3614 1970-01-01 00:00:00.000000 aws_service_catalog_factory-0.99.0/PKG-INFO
```

### Comparing `aws_service_catalog_factory-0.98.1/LICENSE` & `aws_service_catalog_factory-0.99.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/README.md` & `aws_service_catalog_factory-0.99.0/README.md`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/pyproject.toml` & `aws_service_catalog_factory-0.99.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2019 Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 [tool.poetry]
 name = "aws-service-catalog-factory"
-version = "0.98.1"
+version = "0.99.0"
 description = "Making it easier to build ServiceCatalog products"
 classifiers = ["Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent", "Natural Language :: English"]
 homepage = "https://service-catalog-tools-workshop.com/"
 readme = "README.md"
 repository = "https://github.com/awslabs/aws-service-catalog-factory"
 authors = ["Eamonn Faherty <aws-service-catalog-tools@amazon.com>"]
 packages = [
```

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/aws.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/aws.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/cli.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/cli.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/cloudformation_servicecatalog_deploy_action.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/cloudformation_servicecatalog_deploy_action.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/bootstrap.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/bootstrap.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/bootstrap_test.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/bootstrap_test.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/configuration_management.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/configuration_management.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/extract_from_ssm.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/extract_from_ssm.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/generate.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/generate.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/list_resources.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/list_resources.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/management.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/management.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/portfolios.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/portfolios.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/seed.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/seed.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/show_pipelines.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/show_pipelines.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/stacks.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/stacks.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/task_reference.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/task_reference.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from servicecatalog_factory import constants
 from deepmerge import always_merger
 
 from servicecatalog_factory.workflow.dependencies import resources_factory
 
 
 GET_BUCKET_TASK_REFERENCE = "get-bucket"
+ASSOCIATE_PRODUCTS_TASK_REFERENCE = "associate-products-task-reference"
 
 
 def create_task_for_combined_pipeline(
     task_reference,
     category,
     item,
     name,
@@ -152,14 +153,23 @@
     task_reference[GET_BUCKET_TASK_REFERENCE] = dict(
         task_reference=GET_BUCKET_TASK_REFERENCE,
         section_name=section_names.GET_BUCKET,
         dependencies_by_reference=[],
         region=constants.HOME_REGION,
     )
 
+    if not task_reference.get(ASSOCIATE_PRODUCTS_TASK_REFERENCE):
+        task_reference[ASSOCIATE_PRODUCTS_TASK_REFERENCE] = dict(
+            task_reference=ASSOCIATE_PRODUCTS_TASK_REFERENCE,
+            section_name=section_names.ASSOCIATE_PRODUCTS_TASKS,
+            dependencies_by_reference=[],
+            region=constants.HOME_REGION,
+        )
+    associate_products_task = task_reference[ASSOCIATE_PRODUCTS_TASK_REFERENCE]
+
     for file_name in glob.glob(f"{path}/*.yaml"):
         file = yaml.safe_load(open(file_name, "r").read())
         # Add external defined products and versions
         p_name = os.path.basename(file_name)[0:-5]
         for portfolio_file in glob.glob(f"{path}/{p_name}/Portfolios/*"):
             if os.path.isdir(portfolio_file):
                 portfolio_name = os.path.basename(portfolio_file)
@@ -271,14 +281,31 @@
                         dependencies_by_reference=[create_portfolio_task_ref],
                         region=region,
                         portfolio_name=portfolio_name,
                         associations=item.get("Associations"),
                         tags=item.get("Tags", []),
                     )
 
+                if item.get("Constraints"):
+                    task_reference[
+                        f"create-portfolio-{portfolio_name}-{region}-constraints"
+                    ] = dict(
+                        task_reference=f"create-portfolio-{portfolio_name}-{region}-constraints",
+                        section_name=section_names.CREATE_PORTFOLIO_CONSTRAINTS_TASK,
+                        create_portfolio_task_ref=create_portfolio_task_ref,
+                        dependencies_by_reference=[
+                            create_portfolio_task_ref,
+                            ASSOCIATE_PRODUCTS_TASK_REFERENCE,
+                        ],
+                        region=region,
+                        portfolio_name=portfolio_name,
+                        constraints=item.get("Constraints"),
+                        tags=item.get("Tags", []),
+                    )
+
                 # ADD PRODUCTS FOR THE PORTFOLIO
                 for product in item.get("Components", []) + item.get("Products", []):
                     create_product_task_ref = (
                         f"create-product-{product.get('Name')}-{region}"
                     )
                     if task_reference.get(create_product_task_ref):
                         raise Exception(
@@ -339,14 +366,17 @@
                         create_portfolio_task_ref=create_portfolio_task_ref,
                         dependencies_by_reference=[
                             create_product_task_ref,
                             create_portfolio_task_ref,
                         ],
                         region=region,
                     )
+                    associate_products_task["dependencies_by_reference"].append(
+                        create_product_association_ref
+                    )
 
                     # CREATE LAUNCH ROLE NAME CONSTRAINTS
                     if (
                         product.get("Constraints", {})
                         .get("Launch", {})
                         .get("LocalRoleName")
                     ):
@@ -463,14 +493,23 @@
 
     return task_reference
 
 
 def generate_tasks_for_product(
     enabled_regions, file_name, product_details, p_name, task_reference
 ):
+    if not task_reference.get(ASSOCIATE_PRODUCTS_TASK_REFERENCE):
+        task_reference[ASSOCIATE_PRODUCTS_TASK_REFERENCE] = dict(
+            task_reference=ASSOCIATE_PRODUCTS_TASK_REFERENCE,
+            section_name=section_names.ASSOCIATE_PRODUCTS_TASKS,
+            dependencies_by_reference=[],
+            region=constants.HOME_REGION,
+        )
+    associate_products_task = task_reference[ASSOCIATE_PRODUCTS_TASK_REFERENCE]
+
     for region in enabled_regions:
         create_product_task_ref = (
             f"create-product-{product_details.get('Name')}-{region}"
         )
 
         if task_reference.get(create_product_task_ref):
             raise Exception(
@@ -619,14 +658,17 @@
                     create_portfolio_task_ref=get_portfolio_task_ref,
                     dependencies_by_reference=[
                         create_product_task_ref,
                         get_portfolio_task_ref,
                     ],
                     region=region,
                 )
+                associate_products_task["dependencies_by_reference"].append(
+                    create_product_association_ref
+                )
 
                 # CREATE LAUNCH ROLE NAME CONSTRAINTS
                 if (
                     product_details.get("Constraints", {})
                     .get("Launch", {})
                     .get("LocalRoleName")
                 ):
```

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/validate.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/validate.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/commands/version.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/commands/version.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/common/serialisation_utils.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/common/serialisation_utils.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/common/utils.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/common/utils.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/config.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/config.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/constants.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     "UPDATE_ROLLBACK_IN_PROGRESS",
     "UPDATE_ROLLBACK_COMPLETE_CLEANUP_IN_PROGRESS",
     "REVIEW_IN_PROGRESS",
 ]
 PRODUCT = "product.j2"
 PRODUCT_TERRAFORM = "product-terraform.j2"
 TERRAFORM_TEMPLATE = "terraform.template.yaml.j2"
-ASSOCIATIONS = "associations.j2"
 HOME_REGION = os.environ.get(
     "AWS_REGION", os.environ.get("AWS_DEFAULT_REGION", "eu-west-1")
 )
 
 RESULTS_DIRECTORY = "results"
 
 PIPELINE_MODE_COMBINED = "combined"
```

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/constants_test.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/constants_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,14 @@
         "UPDATE_ROLLBACK_IN_PROGRESS",
         "UPDATE_ROLLBACK_COMPLETE_CLEANUP_IN_PROGRESS",
         "REVIEW_IN_PROGRESS",
     ]
     assert sut.PRODUCT == "product.j2"
     assert sut.PRODUCT_TERRAFORM == "product-terraform.j2"
     assert sut.TERRAFORM_TEMPLATE == "terraform.template.yaml.j2"
-    assert sut.ASSOCIATIONS == "associations.j2"
 
     assert sut.RESULTS_DIRECTORY == "results"
 
     assert sut.PIPELINE_MODE_COMBINED == "combined"
     assert sut.PIPELINE_MODE_SPILT == "split"
     assert sut.PIPELINE_MODE_DEFAULT == sut.PIPELINE_MODE_SPILT
```

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/portfolios/ccoe.yaml` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/portfolios/ccoe.yaml`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/portfolios/example-quickstart.yaml` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/portfolios/example-quickstart.yaml`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/portfolios/example-simple-github.yaml` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/portfolios/example-simple-github.yaml`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/portfolios/example-simple.yaml` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/portfolios/example-simple.yaml`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/schema/schema-apps.yaml` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/schema/schema-apps.yaml`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/schema/schema-portfolios.yaml` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/schema/schema-portfolios.yaml`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/schema/schema-stacks.yaml` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/schema/schema-stacks.yaml`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/schema/schema-workspaces.yaml` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/schema/schema-workspaces.yaml`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/sdk.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/sdk.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/servicecatalog-factory-initialiser.template.yaml` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/servicecatalog-factory-initialiser.template.yaml`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/servicecatalog-factory-regional.template.yaml` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/servicecatalog-factory-regional.template.yaml`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/servicecatalog-factory-secondary.template.yaml` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/servicecatalog-factory-secondary.template.yaml`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/servicecatalog-factory.template.yaml` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/servicecatalog-factory.template.yaml`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/tasks_unit_tests_helper.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/tasks_unit_tests_helper.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/base_template.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/base_template.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/cdk/product_pipeline.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/cdk/product_pipeline.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/cdk/product_template.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/cdk/product_template.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/cdk/shared_resources.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/cdk/shared_resources.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/pipeline/build.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/pipeline/build.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/pipeline/deploy.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/pipeline/deploy.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/pipeline/package.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/pipeline/package.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/pipeline/pipeline_template_builder.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/pipeline/pipeline_template_builder.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/pipeline/source.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/pipeline/source.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/pipeline/test.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/pipeline/test.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/product_templates.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/product_templates.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/template_builder/shared_resources.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/template_builder/shared_resources.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/templates/constraint-launch-role-nested.template.yaml` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/templates/constraint-launch-role-nested.template.yaml`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/templates/constraint-launch-role-parent.template.yaml` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/templates/constraint-launch-role-parent.template.yaml`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/templates/product-terraform.j2` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/templates/product-terraform.j2`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/templates/static-html-page.html` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/templates/static-html-page.html`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/templates/terraform.template.yaml.j2` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/templates/terraform.template.yaml.j2`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/templates/test-action.j2` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/templates/test-action.j2`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/utilities/assets_test.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/utilities/assets_test.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/utils.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -32,18 +32,30 @@
         if isinstance(value, collections.Mapping):
             result[key] = merge(result.get(key, {}), value)
         else:
             result[key] = deepcopy(dict2[key])
     return result
 
 
-def unwrap(input):
-    if hasattr(input, "get_wrapped"):
-        result = input.get_wrapped()
-    else:
-        result = input
-
-    if isinstance(result, dict):
-        for k in result.keys():
-            result[k] = unwrap(result.get(k))
+def unwrap(what):
+    if hasattr(what, "get_wrapped"):
+        return unwrap(what.get_wrapped())
 
-    return result
+    if isinstance(what, dict):
+        thing = dict()
+        for k, v in what.items():
+            thing[k] = unwrap(v)
+        return thing
+
+    if isinstance(what, tuple):
+        thing = list()
+        for v in what:
+            thing.append(unwrap(v))
+        return thing
+
+    if isinstance(what, list):
+        thing = list()
+        for v in what:
+            thing.append(unwrap(v))
+        return thing
+
+    return what
```

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/waluigi/scheduler.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/waluigi/scheduler.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/waluigi/tasks.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/waluigi/tasks.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/codecommit/create_code_repo_task.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/codecommit/create_code_repo_task.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/codecommit/create_code_repo_task_test.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/codecommit/create_code_repo_task_test.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/dependencies/reservable_resources.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/dependencies/reservable_resources.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/dependencies/resources_factory.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/dependencies/resources_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,23 @@
         if status == "terminated":
             resources = []
         else:
             resources = [
                 r.SERVICE_CATALOG_ASSOCIATE_TAG_OPTION_PER_REGION_OF_ACCOUNT,
             ]
 
+    elif section_name == section_names.ASSOCIATE_PRODUCTS_TASKS:
+        resources = []
+
+    elif section_name == section_names.CREATE_PORTFOLIO_CONSTRAINTS_TASK:
+        resources = [
+            r.SERVICE_CATALOG_LIST_PROVISIONING_ARTIFACTS_PER_REGION_OF_ACCOUNT,
+            r.CLOUDFORMATION_CREATE_OR_UPDATE_PER_REGION_OF_ACCOUNT,
+        ]
+
     else:
         raise Exception(f"Unknown section_name: {section_name}")
 
     result = list()
     for resource in resources:
         try:
             result.append(resource.format(**parameters_to_use))
```

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/dependencies/section_names.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/dependencies/section_names.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,7 +11,9 @@
 CREATE_PORTFOLIO_ASSOCIATIONS_TASK = "create-portfolio-associations-task"
 CREATE_PRODUCT_ASSOCIATION_TASK = "create-product-association-task"
 CREATE_LAUNCH_ROLE_NAME_CONSTRAINTS_TASK = "create-launch-role-name-constraints-task"
 ENSURE_PRODUCT_VERSION_DETAILS_CORRECT_TASK = (
     "ensure-product-version-details-correct-task"
 )
 CREATE_CODE_REPO_TASK = "create-code-repo-task"
+ASSOCIATE_PRODUCTS_TASKS = "associate-products-tasks"
+CREATE_PORTFOLIO_CONSTRAINTS_TASK = "create-portfolio-constraints-task"
```

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/dependencies/task_factory.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/dependencies/task_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         if status == "terminated":
             raise Exception("NOT BUILT YET")
         else:
             from servicecatalog_factory.workflow.portfolios import (
                 create_portfolio_association_task,
             )
 
-            factory_version = "XXX"  # TODO implement or remove
+            factory_version = constants.VERSION
 
             return create_portfolio_association_task.CreatePortfolioAssociationTask(
                 **minimum_common_parameters,
                 region=parameters_to_use.get("region"),
                 portfolio_name=parameters_to_use.get("portfolio_name"),
                 create_portfolio_task_ref=parameters_to_use.get(
                     "create_portfolio_task_ref"
@@ -228,9 +228,38 @@
                 create_product_task_ref=parameters_to_use.get(
                     "create_product_task_ref"
                 ),
                 create_tag_option_task_ref=parameters_to_use.get(
                     "create_tag_option_task_ref"
                 ),
             )
+    elif section_name == section_names.ASSOCIATE_PRODUCTS_TASKS:
+        from servicecatalog_factory.workflow.portfolios import associate_products_tasks
+
+        return associate_products_tasks.AssociationProductsTasks(
+            **minimum_common_parameters
+        )
+
+    elif section_name == section_names.CREATE_PORTFOLIO_CONSTRAINTS_TASK:
+        if status == "terminated":
+            raise Exception("NOT BUILT YET")
+        else:
+            from servicecatalog_factory.workflow.portfolios import (
+                create_portfolio_constraints_task,
+            )
+
+            factory_version = constants.VERSION
+
+            return create_portfolio_constraints_task.CreatePortfolioConstraintsTask(
+                **minimum_common_parameters,
+                region=parameters_to_use.get("region"),
+                portfolio_name=parameters_to_use.get("portfolio_name"),
+                create_portfolio_task_ref=parameters_to_use.get(
+                    "create_portfolio_task_ref"
+                ),
+                constraints=parameters_to_use.get("constraints"),
+                tags=parameters_to_use.get("tags"),
+                factory_version=factory_version,
+            )
+
     else:
         raise Exception(f"Unknown section_name: {section_name}")
```

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/generic/create_generic_version_pipeline_task.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/generic/create_generic_version_pipeline_task.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/associate_product_with_portfolio_task.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/associate_product_with_portfolio_task.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/associate_product_with_portfolio_task_test.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/associate_product_with_portfolio_task_test.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/associate_tag_option_task.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/associate_tag_option_task.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_combined_product_pipeline_task.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_combined_product_pipeline_task.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_combined_product_pipeline_task_test.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_combined_product_pipeline_task_test.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_launch_role_name_constraints_task.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_launch_role_name_constraints_task.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_portfolio_association_task_test.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_portfolio_association_task_test.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_portfolio_task.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_portfolio_task.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_portfolio_task_test.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_portfolio_task_test.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_product_task.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_product_task.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_product_task_test.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_product_task_test.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_tag_option_task.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_tag_option_task.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_version_pipeline_task.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_version_pipeline_task.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/create_version_pipeline_task_test.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/create_version_pipeline_task_test.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/delete_a_version_task.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/delete_a_version_task.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/delete_a_version_task_test.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/delete_a_version_task_test.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/delete_product_from_service_catalog_task.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/delete_product_from_service_catalog_task.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/delete_product_task.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/delete_product_task.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/delete_product_task_test.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/delete_product_task_test.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/ensure_product_version_details_correct_task.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/ensure_product_version_details_correct_task.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/ensure_product_version_details_correct_task_test.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/ensure_product_version_details_correct_task_test.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/get_bucket_task.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/get_bucket_task.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/portfolios/get_bucket_task_test.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/portfolios/get_bucket_task_test.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/tasks.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/tasks.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from betterboto import client as betterboto_client
 
 from servicecatalog_factory import constants
 
 from servicecatalog_factory.waluigi import tasks as waluigi_tasks
 
 logger = logging.getLogger(__file__)
+from botocore.config import Config
 
 
 class FactoryTask(waluigi_tasks.WaluigiTaskMixin, luigi.Task):
     def params_for_results_display(self):
         return {"task_reference": self.task_reference}
 
     @property
@@ -49,19 +50,29 @@
     @property
     def factory_region(self):
         region = os.environ.get("REGION", None)
         if region is None:
             raise Exception("You must export REGION")
         return region
 
-    def client(self, service):
-        return betterboto_client.ClientContextManager(service,)
+    def client(self, service, retry_max_attempts=None):
+        kwargs = dict()
+        if retry_max_attempts is not None:
+            kwargs["config"] = Config(retries={"max_attempts": retry_max_attempts,})
+
+        return betterboto_client.ClientContextManager(service, **kwargs)
+
+    def regional_client(self, service, retry_max_attempts=None):
+        kwargs = dict()
+        if retry_max_attempts is not None:
+            kwargs["config"] = Config(retries={"max_attempts": retry_max_attempts,})
 
-    def regional_client(self, service):
-        return betterboto_client.ClientContextManager(service, region_name=self.region,)
+        return betterboto_client.ClientContextManager(
+            service, region_name=self.region, **kwargs
+        )
 
     def load_from_input(self, input_name):
         with self.input().get(input_name).open("r") as f:
             return json.loads(f.read())
 
     def info(self, message):
         logger.info(f"{self.uid}: {message}")
```

### Comparing `aws_service_catalog_factory-0.98.1/servicecatalog_factory/workflow/tasks_unit_tests_helper.py` & `aws_service_catalog_factory-0.99.0/servicecatalog_factory/workflow/tasks_unit_tests_helper.py`

 * *Files identical despite different names*

### Comparing `aws_service_catalog_factory-0.98.1/setup.py` & `aws_service_catalog_factory-0.99.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
  'yamale==3.0.8']
 
 entry_points = \
 {'console_scripts': ['servicecatalog-factory = servicecatalog_factory.cli:cli']}
 
 setup_kwargs = {
     'name': 'aws-service-catalog-factory',
-    'version': '0.98.1',
+    'version': '0.99.0',
     'description': 'Making it easier to build ServiceCatalog products',
     'long_description': '# aws-service-catalog-factory\n\n![logo](./docs/logo.png) \n\n## What is it?\nThis is a python3 framework that makes it easier to build multi region AWS Service Catalog portfolios.\n\nWith this framework you define a portfolio in YAML.  For each product version in your portfolio you specify which git \nrepository it is in and the framework will build out AWS CodePipelines for each product version.\n\nThese CodePipelines can run CFN_NAG and Cloudformation_rspec on your templates enabling you to check your templates are \ngood quality that they are functionally correct.\n\n## Getting started\n\nYou can read the [installation how to](https://service-catalog-tools-workshop.com/30-how-tos/10-installation/20-service-catalog-factory.html)\nor you can read through the [every day use](https://service-catalog-tools-workshop.com/30-how-tos/50-every-day-use.html)\nguides.\n\nYou can read the [documentation](https://aws-service-catalog-factory.readthedocs.io/en/latest/) to understand the inner \nworkings. \n\n\n## Going further\n\nThe framework is one of a pair.  The other is [aws-service-catalog-puppet](https://github.com/awslabs/aws-service-catalog-puppet).\nWith Service Catalog Puppet you can provision products into multiple regions of multiple accounts using YAML and you can \nshare portfolios across multiple regions of multiple accounts. \n\n## License\n\nThis library is licensed under the Apache 2.0 License. \n',
     'author': 'Eamonn Faherty',
     'author_email': 'aws-service-catalog-tools@amazon.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://service-catalog-tools-workshop.com/',
```

### Comparing `aws_service_catalog_factory-0.98.1/PKG-INFO` & `aws_service_catalog_factory-0.99.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-service-catalog-factory
-Version: 0.98.1
+Version: 0.99.0
 Summary: Making it easier to build ServiceCatalog products
 Home-page: https://service-catalog-tools-workshop.com/
 Author: Eamonn Faherty
 Author-email: aws-service-catalog-tools@amazon.com
 Requires-Python: >=3.7,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

