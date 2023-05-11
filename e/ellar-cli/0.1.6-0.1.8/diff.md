# Comparing `tmp/ellar-cli-0.1.6.tar.gz` & `tmp/ellar-cli-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellar-cli-0.1.6.tar", last modified: Sun Mar 26 09:18:08 2023, max compression
+gzip compressed data, was "ellar-cli-0.1.8.tar", last modified: Thu May 11 21:33:41 2023, max compression
```

## Comparing `ellar-cli-0.1.6.tar` & `ellar-cli-0.1.8.tar`

### file list

```diff
@@ -1,85 +1,86 @@
--rw-r--r--   0        0        0       65 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/.dockerignore
--rw-r--r--   0        0        0      140 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/.flake8
--rw-r--r--   0        0        0      205 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/.github/dependabot.yml
--rw-r--r--   0        0        0      571 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0      545 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/.github/workflows/test.yml
--rw-r--r--   0        0        0     1138 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/.github/workflows/test_full.yml
--rw-r--r--   0        0        0     1891 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/.gitignore
--rw-r--r--   0        0        0       53 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/.isort.cfg
--rw-r--r--   0        0        0     1073 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1083 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/LICENSE
--rw-r--r--   0        0        0     1050 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/Makefile
--rw-r--r--   0        0        0     2136 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/README.md
--rwxr-xr-x   0        0        0    36744 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/docs/img/EllarLogoIconOnly.png
--rw-r--r--   0        0        0      116 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/ellar_cli/__init__.py
--rw-r--r--   0        0        0       74 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/ellar_cli/__main__.py
--rw-r--r--   0        0        0      609 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/ellar_cli/cli.py
--rw-r--r--   0        0        0       26 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/ellar_cli/constants.py
--rw-r--r--   0        0        0     3679 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/ellar_cli/file_scaffolding.py
--rw-r--r--   0        0        0     2446 2023-03-26 09:17:50.696267 ellar-cli-0.1.6/ellar_cli/main.py
--rw-r--r--   0        0        0      221 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/manage_commands/__init__.py
--rw-r--r--   0        0        0     3048 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/manage_commands/create_module.py
--rw-r--r--   0        0        0     3149 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/manage_commands/create_project.py
--rw-r--r--   0        0        0     3575 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/manage_commands/new.py
--rw-r--r--   0        0        0    10718 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/manage_commands/runserver.py
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/py.typed
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/module_template/module_name/__init__.ellar
--rw-r--r--   0        0        0      525 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/module_template/module_name/controllers.ellar
--rw-r--r--   0        0        0     1052 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/module_template/module_name/module.ellar
--rw-r--r--   0        0        0      296 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/module_template/module_name/routers.ellar
--rw-r--r--   0        0        0      328 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/module_template/module_name/schemas.ellar
--rw-r--r--   0        0        0      180 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/module_template/module_name/services.ellar
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/module_template/module_name/tests/test_controllers.ellar
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/module_template/module_name/tests/test_routers.ellar
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/module_template/module_name/tests/test_services.ellar
--rw-r--r--   0        0        0      816 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/module_template/setup.json
--rw-r--r--   0        0        0      204 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/new_template/folder_name/README.md
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/new_template/folder_name/pyproject.toml
--rw-r--r--   0        0        0       54 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/new_template/folder_name/tests/conftest.ellar
--rw-r--r--   0        0        0      451 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/new_template/setup.json
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/project_template/project_name/__init__.ellar
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/project_template/project_name/apps/__init__.ellar
--rw-r--r--   0        0        0     2589 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/project_template/project_name/config.ellar
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/project_template/project_name/core/__init__.ellar
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/project_template/project_name/domain/__init__.ellar
--rw-r--r--   0        0        0      484 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/project_template/project_name/root_module.ellar
--rw-r--r--   0        0        0     1059 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/project_template/project_name/server.ellar
--rw-r--r--   0        0        0      930 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/project_template/setup.json
--rw-r--r--   0        0        0     2032 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/scaffolding/scaffolding_json_validator.py
--rw-r--r--   0        0        0     1233 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/schema.py
--rw-r--r--   0        0        0     7516 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/service.py
--rw-r--r--   0        0        0     1444 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/ellar_cli/testing.py
--rw-r--r--   0        0        0      660 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/mypy.ini
--rw-r--r--   0        0        0     2084 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      207 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/pytest.ini
--rw-r--r--   0        0        0     2033 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/tests/sample_app/example_project/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/tests/sample_app/example_project/apps/__init__.py
--rw-r--r--   0        0        0      319 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/tests/sample_app/example_project/commands.py
--rw-r--r--   0        0        0     2430 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/tests/sample_app/example_project/config.py
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/tests/sample_app/example_project/core/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/tests/sample_app/example_project/domain/__init__.py
--rw-r--r--   0        0        0      482 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/tests/sample_app/example_project/root_module.py
--rw-r--r--   0        0        0      927 2023-03-26 09:17:50.700268 ellar-cli-0.1.6/tests/sample_app/example_project/server.py
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/sample_app/example_project/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/sample_app/example_project_2/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/sample_app/example_project_2/apps/__init__.py
--rw-r--r--   0        0        0      499 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/sample_app/example_project_2/commands.py
--rw-r--r--   0        0        0     2432 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/sample_app/example_project_2/config.py
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/sample_app/example_project_2/core/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/sample_app/example_project_2/domain/__init__.py
--rw-r--r--   0        0        0      520 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/sample_app/example_project_2/root_module.py
--rw-r--r--   0        0        0      931 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/sample_app/example_project_2/server.py
--rw-r--r--   0        0        0        0 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/sample_app/example_project_2/tests/conftest.py
--rw-r--r--   0        0        0      602 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/sample_app/pyproject.toml
--rw-r--r--   0        0        0     5180 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/test_build_typers.py
--rw-r--r--   0        0        0     7323 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/test_ellar_cli_service.py
--rw-r--r--   0        0        0     4181 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/test_ellar_commands/test_create_module_command.py
--rw-r--r--   0        0        0     3171 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/test_ellar_commands/test_create_project_command.py
--rw-r--r--   0        0        0     2802 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/test_ellar_commands/test_new_command.py
--rw-r--r--   0        0        0     5268 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/test_ellar_commands/test_runserver_command.py
--rw-r--r--   0        0        0     2172 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/test_ellar_py_project.py
--rw-r--r--   0        0        0     2729 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/test_file_scaffolding.py
--rw-r--r--   0        0        0      363 2023-03-26 09:17:50.704268 ellar-cli-0.1.6/tests/test_scaffolding_templates_json.py
--rw-r--r--   0        0        0     4319 1970-01-01 00:00:00.000000 ellar-cli-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       65 2023-05-11 21:33:25.968736 ellar-cli-0.1.8/.dockerignore
+-rw-r--r--   0        0        0      140 2023-05-11 21:33:25.968736 ellar-cli-0.1.8/.flake8
+-rw-r--r--   0        0        0      205 2023-05-11 21:33:25.968736 ellar-cli-0.1.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      571 2023-05-11 21:33:25.968736 ellar-cli-0.1.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      545 2023-05-11 21:33:25.968736 ellar-cli-0.1.8/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1138 2023-05-11 21:33:25.968736 ellar-cli-0.1.8/.github/workflows/test_full.yml
+-rw-r--r--   0        0        0     1891 2023-05-11 21:33:25.968736 ellar-cli-0.1.8/.gitignore
+-rw-r--r--   0        0        0       53 2023-05-11 21:33:25.968736 ellar-cli-0.1.8/.isort.cfg
+-rw-r--r--   0        0        0     1073 2023-05-11 21:33:25.968736 ellar-cli-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1083 2023-05-11 21:33:25.968736 ellar-cli-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1050 2023-05-11 21:33:25.968736 ellar-cli-0.1.8/Makefile
+-rw-r--r--   0        0        0     2136 2023-05-11 21:33:25.968736 ellar-cli-0.1.8/README.md
+-rwxr-xr-x   0        0        0    36744 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/docs/img/EllarLogoIconOnly.png
+-rw-r--r--   0        0        0      116 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/__init__.py
+-rw-r--r--   0        0        0       74 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/__main__.py
+-rw-r--r--   0        0        0      609 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/cli.py
+-rw-r--r--   0        0        0       53 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/constants.py
+-rw-r--r--   0        0        0     3679 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/file_scaffolding.py
+-rw-r--r--   0        0        0     2464 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/main.py
+-rw-r--r--   0        0        0      221 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/manage_commands/__init__.py
+-rw-r--r--   0        0        0     3055 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/manage_commands/create_module.py
+-rw-r--r--   0        0        0     3156 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/manage_commands/create_project.py
+-rw-r--r--   0        0        0     3582 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/manage_commands/new.py
+-rw-r--r--   0        0        0    10945 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/manage_commands/runserver.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/py.typed
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/module_template/module_name/__init__.ellar
+-rw-r--r--   0        0        0      503 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/module_template/module_name/controllers.ellar
+-rw-r--r--   0        0        0     1052 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/module_template/module_name/module.ellar
+-rw-r--r--   0        0        0      296 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/module_template/module_name/routers.ellar
+-rw-r--r--   0        0        0      323 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/module_template/module_name/schemas.ellar
+-rw-r--r--   0        0        0      180 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/module_template/module_name/services.ellar
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/module_template/module_name/tests/__init__.ellar
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/module_template/module_name/tests/test_controllers.ellar
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/module_template/module_name/tests/test_routers.ellar
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/module_template/module_name/tests/test_services.ellar
+-rw-r--r--   0        0        0      884 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/module_template/setup.json
+-rw-r--r--   0        0        0      204 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/new_template/folder_name/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/new_template/folder_name/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/new_template/folder_name/tests/conftest.ellar
+-rw-r--r--   0        0        0      451 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/new_template/setup.json
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/project_template/project_name/__init__.ellar
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/project_template/project_name/apps/__init__.ellar
+-rw-r--r--   0        0        0     2579 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/project_template/project_name/config.ellar
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/project_template/project_name/core/__init__.ellar
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/project_template/project_name/domain/__init__.ellar
+-rw-r--r--   0        0        0      422 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/project_template/project_name/root_module.ellar
+-rw-r--r--   0        0        0     1066 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/project_template/project_name/server.ellar
+-rw-r--r--   0        0        0      930 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/project_template/setup.json
+-rw-r--r--   0        0        0     2032 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/scaffolding/scaffolding_json_validator.py
+-rw-r--r--   0        0        0     1240 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/schema.py
+-rw-r--r--   0        0        0     7568 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/service.py
+-rw-r--r--   0        0        0     1444 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/ellar_cli/testing.py
+-rw-r--r--   0        0        0      660 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/mypy.ini
+-rw-r--r--   0        0        0     2084 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/pytest.ini
+-rw-r--r--   0        0        0     2033 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/tests/sample_app/example_project/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/tests/sample_app/example_project/apps/__init__.py
+-rw-r--r--   0        0        0      293 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/tests/sample_app/example_project/commands.py
+-rw-r--r--   0        0        0     2454 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/tests/sample_app/example_project/config.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/tests/sample_app/example_project/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.972736 ellar-cli-0.1.8/tests/sample_app/example_project/domain/__init__.py
+-rw-r--r--   0        0        0      451 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/sample_app/example_project/root_module.py
+-rw-r--r--   0        0        0      934 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/sample_app/example_project/server.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/sample_app/example_project/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/sample_app/example_project_2/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/sample_app/example_project_2/apps/__init__.py
+-rw-r--r--   0        0        0      473 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/sample_app/example_project_2/commands.py
+-rw-r--r--   0        0        0     2456 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/sample_app/example_project_2/config.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/sample_app/example_project_2/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/sample_app/example_project_2/domain/__init__.py
+-rw-r--r--   0        0        0      489 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/sample_app/example_project_2/root_module.py
+-rw-r--r--   0        0        0      938 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/sample_app/example_project_2/server.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/sample_app/example_project_2/tests/conftest.py
+-rw-r--r--   0        0        0      602 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/sample_app/pyproject.toml
+-rw-r--r--   0        0        0     5180 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/test_build_typers.py
+-rw-r--r--   0        0        0     7323 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/test_ellar_cli_service.py
+-rw-r--r--   0        0        0     4181 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/test_ellar_commands/test_create_module_command.py
+-rw-r--r--   0        0        0     3171 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/test_ellar_commands/test_create_project_command.py
+-rw-r--r--   0        0        0     2802 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/test_ellar_commands/test_new_command.py
+-rw-r--r--   0        0        0     5268 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/test_ellar_commands/test_runserver_command.py
+-rw-r--r--   0        0        0     2176 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/test_ellar_py_project.py
+-rw-r--r--   0        0        0     2729 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/test_file_scaffolding.py
+-rw-r--r--   0        0        0      363 2023-05-11 21:33:25.976737 ellar-cli-0.1.8/tests/test_scaffolding_templates_json.py
+-rw-r--r--   0        0        0     4319 1970-01-01 00:00:00.000000 ellar-cli-0.1.8/PKG-INFO
```

### Comparing `ellar-cli-0.1.6/.github/workflows/publish.yml` & `ellar-cli-0.1.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/.github/workflows/test.yml` & `ellar-cli-0.1.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/.github/workflows/test_full.yml` & `ellar-cli-0.1.8/.github/workflows/test_full.yml`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/.gitignore` & `ellar-cli-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/.pre-commit-config.yaml` & `ellar-cli-0.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/LICENSE` & `ellar-cli-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/Makefile` & `ellar-cli-0.1.8/Makefile`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/README.md` & `ellar-cli-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/docs/img/EllarLogoIconOnly.png` & `ellar-cli-0.1.8/docs/img/EllarLogoIconOnly.png`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/ellar_cli/cli.py` & `ellar-cli-0.1.8/ellar_cli/cli.py`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/ellar_cli/file_scaffolding.py` & `ellar-cli-0.1.8/ellar_cli/file_scaffolding.py`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/ellar_cli/main.py` & `ellar-cli-0.1.8/ellar_cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import getopt
 import sys
 import typing as t
 
 import typer
-from ellar.commands import EllarTyper
-from ellar.constants import CALLABLE_COMMAND_INFO, MODULE_METADATA
+from ellar.common.commands import EllarTyper
+from ellar.common.constants import CALLABLE_COMMAND_INFO, MODULE_METADATA
 from ellar.core.factory import AppFactory
 from ellar.core.modules import ModuleSetup
-from ellar.services import Reflector
+from ellar.core.services import Reflector
 from typer import Typer
 from typer.models import CommandInfo
 
 from ellar_cli.constants import ELLAR_META
 
 from .manage_commands import create_module, create_project, new_command, runserver
 from .service import EllarCLIService
@@ -57,15 +57,15 @@
         typer.Abort()
         return 1
 
     meta_: t.Optional[EllarCLIService] = EllarCLIService.import_project_meta(app_name)
 
     if meta_ and meta_.has_meta:
         module_configs = AppFactory.get_all_modules(
-            ModuleSetup(meta_.import_root_module())  # type: ignore
+            ModuleSetup(meta_.import_root_module())  # type:ignore
         )
         reflector = Reflector()
 
         for module_config in module_configs:
             typers_commands = (
                 reflector.get(MODULE_METADATA.COMMANDS, module_config.module) or []
             )
```

### Comparing `ellar-cli-0.1.6/ellar_cli/manage_commands/create_module.py` & `ellar-cli-0.1.8/ellar_cli/manage_commands/create_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 import typing as t
 from importlib import import_module
 
 import typer
-from ellar.helper.module_loading import module_dir
+from ellar.common.helper.module_loading import module_dir
 
 from ellar_cli import scaffolding
 from ellar_cli.constants import ELLAR_META
 from ellar_cli.schema import EllarScaffoldSchema
 
 from ..file_scaffolding import FileTemplateScaffold
 from ..service import EllarCLIException, EllarCLIService
```

### Comparing `ellar-cli-0.1.6/ellar_cli/manage_commands/create_project.py` & `ellar-cli-0.1.8/ellar_cli/manage_commands/create_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import typing as t
 import uuid
 from importlib import import_module
 
 import typer
-from ellar.helper.module_loading import module_dir
+from ellar.common.helper.module_loading import module_dir
 
 from ellar_cli import scaffolding
 from ellar_cli.constants import ELLAR_META
 from ellar_cli.schema import EllarScaffoldSchema
 
 from ..file_scaffolding import FileTemplateScaffold
 from ..service import EllarCLIException, EllarCLIService
```

### Comparing `ellar-cli-0.1.6/ellar_cli/manage_commands/new.py` & `ellar-cli-0.1.8/ellar_cli/manage_commands/new.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 import subprocess
 import typing as t
 
 import typer
-from ellar.helper.module_loading import module_dir
+from ellar.common.helper.module_loading import module_dir
 
 from ellar_cli import scaffolding
 from ellar_cli.schema import EllarScaffoldSchema
 
 from ..file_scaffolding import FileTemplateScaffold
 from ..service import EllarCLIException
```

### Comparing `ellar-cli-0.1.6/ellar_cli/manage_commands/runserver.py` & `ellar-cli-0.1.8/ellar_cli/manage_commands/runserver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import ssl
 import sys
 import typing as t
 from pathlib import Path
 
 import typer
-from ellar.constants import LOG_LEVELS
-from ellar.helper.enums import create_enums_from_list
+from ellar.common.constants import LOG_LEVELS
+from ellar.common.helper.enums import create_enums_from_list
 from h11._connection import DEFAULT_MAX_INCOMPLETE_EVENT_SIZE
 from uvicorn.config import (
     HTTP_PROTOCOLS,
     INTERFACES,
     LIFESPAN,
+    LOG_LEVELS,
     LOGGING_CONFIG,
     LOOP_SETUPS,
     SSL_PROTOCOL_VERSION,
     WS_PROTOCOLS,
 )
 from uvicorn.main import run as uvicorn_run
 
@@ -28,14 +29,16 @@
 HTTP_CHOICES = create_enums_from_list("HTTP_CHOICES", *list(HTTP_PROTOCOLS.keys()))
 WS_CHOICES = create_enums_from_list("WS_CHOICES", *list(WS_PROTOCOLS.keys()))
 LIFESPAN_CHOICES = create_enums_from_list("LIFESPAN_CHOICES", *list(LIFESPAN.keys()))
 LOOP_CHOICES = create_enums_from_list(
     "LOOP_CHOICES", *[key for key in LOOP_SETUPS.keys() if key != "none"]
 )
 INTERFACE_CHOICES = create_enums_from_list("INTERFACES", *INTERFACES)
+_LOG_LEVELS = dict(**LOG_LEVELS, NOT_SET=0)
+LOG_LEVELS_CHOICES = create_enums_from_list("LOG_LEVELS", *list(_LOG_LEVELS.keys()))
 
 
 def runserver(
     ctx: typer.Context,
     host: str = typer.Option(
         "127.0.0.1", help="Bind socket to this host.", show_default=True
     ),
@@ -108,16 +111,16 @@
         INTERFACE_CHOICES.auto.value,
         show_default=True,
         help="Select ASGI3, ASGI2, or WSGI as the application interface.",
     ),
     env_file: t.Optional[Path] = typer.Option(
         None, show_default=True, exists=True, help="Environment configuration file."
     ),
-    log_level: t.Optional[LOG_LEVELS] = typer.Option(
-        None,
+    log_level: LOG_LEVELS_CHOICES = typer.Option(
+        LOG_LEVELS_CHOICES.NOT_SET.value,
         show_default=True,
         help="Log level. [default: None]",
     ),
     access_log: bool = typer.Option(
         True,
         "--access-log/--no-access-log",
         is_flag=True,
@@ -262,15 +265,15 @@
         ws=ws.value,
         ws_max_size=ws_max_size,
         ws_ping_interval=ws_ping_interval,
         ws_ping_timeout=ws_ping_timeout,
         lifespan=lifespan.value,
         env_file=env_file,
         log_config=LOGGING_CONFIG if log_config is None else log_config,
-        log_level=_log_level.name,
+        log_level=_log_level.value if _log_level.value != "NOT_SET" else None,
         access_log=access_log,
         interface=interface.value,
         reload=reload,
         reload_dirs=reload_dirs or None,
         reload_includes=reload_includes or None,
         reload_excludes=reload_excludes or None,
         reload_delay=reload_delay,
```

### Comparing `ellar-cli-0.1.6/ellar_cli/scaffolding/module_template/module_name/module.ellar` & `ellar-cli-0.1.8/ellar_cli/scaffolding/module_template/module_name/module.ellar`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/ellar_cli/scaffolding/module_template/setup.json` & `ellar-cli-0.1.8/ellar_cli/scaffolding/module_template/setup.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997519841269841%*

 * *Differences: {"'files'": "{0: {'files': {6: {'files': {insert: [(0, OrderedDict([('name', "*

 * *            "'__init__.ellar')]))]}}}}}"}*

```diff
@@ -22,14 +22,17 @@
                 },
                 {
                     "name": "services.ellar"
                 },
                 {
                     "files": [
                         {
+                            "name": "__init__.ellar"
+                        },
+                        {
                             "name": "test_controllers.ellar"
                         },
                         {
                             "name": "test_routers.ellar"
                         },
                         {
                             "name": "test_services.ellar"
```

### Comparing `ellar-cli-0.1.6/ellar_cli/scaffolding/project_template/project_name/config.ellar` & `ellar-cli-0.1.8/ellar_cli/scaffolding/project_template/project_name/config.ellar`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 export ELLAR_CONFIG_MODULE={{project_name}}.config:DevelopmentConfig
 """
 
 import typing as t
 
 from pydantic.json import ENCODERS_BY_TYPE as encoders_by_type
 from starlette.middleware import Middleware
-from ellar.core.exceptions import IExceptionHandler
-from ellar.core import ConfigDefaultTypesMixin, JSONResponse
+from ellar.common import IExceptionHandler, JSONResponse
+from ellar.core import ConfigDefaultTypesMixin
 from ellar.core.versioning import BaseAPIVersioning, DefaultAPIVersioning
 
 
 class BaseConfig(ConfigDefaultTypesMixin):
     DEBUG: bool = False
 
     DEFAULT_JSON_CLASS: t.Type[JSONResponse] = JSONResponse
@@ -64,8 +64,7 @@
     SERIALIZER_CUSTOM_ENCODER: t.Dict[
         t.Any, t.Callable[[t.Any], t.Any]
     ] = encoders_by_type
 
 
 class DevelopmentConfig(BaseConfig):
     DEBUG: bool = True
-
```

### Comparing `ellar-cli-0.1.6/ellar_cli/scaffolding/project_template/project_name/server.ellar` & `ellar-cli-0.1.8/ellar_cli/scaffolding/project_template/project_name/server.ellar`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from ellar.constants import ELLAR_CONFIG_MODULE
+from ellar.common.constants import ELLAR_CONFIG_MODULE
 from ellar.core.factory import AppFactory
 # from ellar.openapi import OpenAPIDocumentModule, OpenAPIDocumentBuilder, SwaggerDocumentGenerator
 from .root_module import ApplicationModule
 
 application = AppFactory.create_from_app_module(
     ApplicationModule,
     config_module=os.environ.get(
```

### Comparing `ellar-cli-0.1.6/ellar_cli/scaffolding/project_template/setup.json` & `ellar-cli-0.1.8/ellar_cli/scaffolding/project_template/setup.json`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/ellar_cli/scaffolding/scaffolding_json_validator.py` & `ellar-cli-0.1.8/ellar_cli/scaffolding/scaffolding_json_validator.py`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/ellar_cli/schema.py` & `ellar-cli-0.1.8/ellar_cli/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing as t
 
-from ellar.serializer import Serializer
+from ellar.common.serializer import Serializer
 from pydantic import Field
 
 
 class EllarPyProjectSerializer(Serializer):
     project_name: str = Field(alias="project-name")
     application: str = Field(alias="application")
     config: str = Field(alias="config")
```

### Comparing `ellar-cli-0.1.6/ellar_cli/service.py` & `ellar-cli-0.1.8/ellar_cli/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 import typing as t
 
 from click import ClickException
-from ellar.constants import ELLAR_CONFIG_MODULE, ELLAR_PY_PROJECT
+from ellar.common.constants import ELLAR_CONFIG_MODULE
+from ellar.common.helper.importer import import_from_string, module_import
+from ellar.common.helper.module_loading import module_dir
 from ellar.core import App, Config, ModuleBase
-from ellar.helper.importer import import_from_string, module_import
-from ellar.helper.module_loading import module_dir
 from tomlkit import dumps as tomlkit_dumps, parse as tomlkit_parse, table
 from tomlkit.items import Table
 
+from ellar_cli.constants import ELLAR_PY_PROJECT
 from ellar_cli.schema import EllarPyProjectSerializer
 
 PY_PROJECT_TOML = "pyproject.toml"
 ELLAR_DEFAULT_KEY = "default"
 ELLAR_PROJECTS_KEY = "projects"
```

### Comparing `ellar-cli-0.1.6/ellar_cli/testing.py` & `ellar-cli-0.1.8/ellar_cli/testing.py`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/mypy.ini` & `ellar-cli-0.1.8/mypy.ini`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/pyproject.toml` & `ellar-cli-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 
 dependencies = [
     # exclude 0.11.2 and 0.11.3 due to https://github.com/sdispater/tomlkit/issues/225
     "tomlkit >=0.11.1,<1.0.0,!=0.11.2,!=0.11.3",
-    "uvicorn[standard] == 0.20.0",
-    "ellar >= 0.3.4"
+    "uvicorn[standard] == 0.22.0",
+    "ellar >= 0.3.8"
 ]
 
 [project.scripts]
 ellar = "ellar_cli.cli:main"
 
 [project.urls]
 Documentation = "https://github.com/eadwinCode/ellar-cli"
```

### Comparing `ellar-cli-0.1.6/tests/conftest.py` & `ellar-cli-0.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/tests/sample_app/example_project/config.py` & `ellar-cli-0.1.8/tests/sample_app/example_project/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 Make changes and define your own configurations specific to your application
 
 export ELLAR_CONFIG_MODULE=example_project.config:DevelopmentConfig
 """
 
 import typing as t
 
-from ellar.core import ConfigDefaultTypesMixin, JSONResponse
+from ellar.common import JSONResponse
+from ellar.core import ConfigDefaultTypesMixin
 from ellar.core.versioning import BaseAPIVersioning, DefaultAPIVersioning
 from pydantic.json import ENCODERS_BY_TYPE as encoders_by_type
 from starlette.middleware import Middleware
 
 
 class BaseConfig(ConfigDefaultTypesMixin):
     DEBUG: bool = False
```

### Comparing `ellar-cli-0.1.6/tests/sample_app/example_project/server.py` & `ellar-cli-0.1.8/tests/sample_app/example_project_2/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import os
 
-from ellar.constants import ELLAR_CONFIG_MODULE
+from ellar.common.constants import ELLAR_CONFIG_MODULE
 from ellar.core.factory import AppFactory
 
 # from ellar.openapi import OpenAPIDocumentModule, OpenAPIDocumentBuilder
 from .root_module import ApplicationModule
 
 application = AppFactory.create_from_app_module(
     ApplicationModule,
     config_module=os.environ.get(
-        ELLAR_CONFIG_MODULE, "example_project.config:DevelopmentConfig"
+        ELLAR_CONFIG_MODULE, "example_project_2.config:DevelopmentConfig"
     ),
 )
 
 # uncomment this section if you want API documentation
 
 # document_builder = OpenAPIDocumentBuilder()
-# document_builder.set_title('Example_project Title') \
+# document_builder.set_title('Example_project_2 Title') \
 #     .set_version('1.0.2') \
 #     .set_contact(name='Author Name', url='https://www.author-name.com', email='authorname@gmail.com') \
 #     .set_license('MIT Licence', url='https://www.google.com')
 #
 # document = document_builder.build_document(app)
 # module = application.install_module(OpenAPIDocumentModule, document=document)
 # module.setup_swagger_doc()
```

### Comparing `ellar-cli-0.1.6/tests/sample_app/example_project_2/config.py` & `ellar-cli-0.1.8/tests/sample_app/example_project_2/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 Make changes and define your own configurations specific to your application
 
 export ELLAR_CONFIG_MODULE=example_project_2.config:DevelopmentConfig
 """
 
 import typing as t
 
-from ellar.core import ConfigDefaultTypesMixin, JSONResponse
+from ellar.common import JSONResponse
+from ellar.core import ConfigDefaultTypesMixin
 from ellar.core.versioning import BaseAPIVersioning, DefaultAPIVersioning
 from pydantic.json import ENCODERS_BY_TYPE as encoders_by_type
 from starlette.middleware import Middleware
 
 
 class BaseConfig(ConfigDefaultTypesMixin):
     DEBUG: bool = False
```

### Comparing `ellar-cli-0.1.6/tests/sample_app/example_project_2/server.py` & `ellar-cli-0.1.8/tests/sample_app/example_project/server.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import os
 
-from ellar.constants import ELLAR_CONFIG_MODULE
+from ellar.common.constants import ELLAR_CONFIG_MODULE
 from ellar.core.factory import AppFactory
 
 # from ellar.openapi import OpenAPIDocumentModule, OpenAPIDocumentBuilder
 from .root_module import ApplicationModule
 
 application = AppFactory.create_from_app_module(
     ApplicationModule,
     config_module=os.environ.get(
-        ELLAR_CONFIG_MODULE, "example_project_2.config:DevelopmentConfig"
+        ELLAR_CONFIG_MODULE, "example_project.config:DevelopmentConfig"
     ),
 )
 
 # uncomment this section if you want API documentation
 
 # document_builder = OpenAPIDocumentBuilder()
-# document_builder.set_title('Example_project_2 Title') \
+# document_builder.set_title('Example_project Title') \
 #     .set_version('1.0.2') \
 #     .set_contact(name='Author Name', url='https://www.author-name.com', email='authorname@gmail.com') \
 #     .set_license('MIT Licence', url='https://www.google.com')
 #
 # document = document_builder.build_document(app)
 # module = application.install_module(OpenAPIDocumentModule, document=document)
 # module.setup_swagger_doc()
```

### Comparing `ellar-cli-0.1.6/tests/sample_app/pyproject.toml` & `ellar-cli-0.1.8/tests/sample_app/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/tests/test_build_typers.py` & `ellar-cli-0.1.8/tests/test_build_typers.py`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/tests/test_ellar_cli_service.py` & `ellar-cli-0.1.8/tests/test_ellar_cli_service.py`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/tests/test_ellar_commands/test_create_module_command.py` & `ellar-cli-0.1.8/tests/test_ellar_commands/test_create_module_command.py`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/tests/test_ellar_commands/test_create_project_command.py` & `ellar-cli-0.1.8/tests/test_ellar_commands/test_create_project_command.py`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/tests/test_ellar_commands/test_new_command.py` & `ellar-cli-0.1.8/tests/test_ellar_commands/test_new_command.py`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/tests/test_ellar_commands/test_runserver_command.py` & `ellar-cli-0.1.8/tests/test_ellar_commands/test_runserver_command.py`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/tests/test_ellar_py_project.py` & `ellar-cli-0.1.8/tests/test_ellar_py_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from ellar.constants import ELLAR_PY_PROJECT
 from tomlkit import table
 from tomlkit.items import Table
 
+from ellar_cli.constants import ELLAR_PY_PROJECT
 from ellar_cli.service import EllarPyProject
 
 
 def test_get_or_create_ellar_py_project(mock_py_project_table):
     assert ELLAR_PY_PROJECT not in mock_py_project_table
     EllarPyProject.get_or_create_ellar_py_project(mock_py_project_table)
     assert ELLAR_PY_PROJECT in mock_py_project_table
```

### Comparing `ellar-cli-0.1.6/tests/test_file_scaffolding.py` & `ellar-cli-0.1.8/tests/test_file_scaffolding.py`

 * *Files identical despite different names*

### Comparing `ellar-cli-0.1.6/PKG-INFO` & `ellar-cli-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellar-cli
-Version: 0.1.6
+Version: 0.1.8
 Summary: Ellar CLI Tool for Scaffolding Ellar Projects, Modules and also running Ellar Commands
 Author-email: Ezeudoh Tochukwu <tochukwu.ezeudoh@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -24,16 +24,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: AsyncIO
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: tomlkit >=0.11.1,<1.0.0,!=0.11.2,!=0.11.3
-Requires-Dist: uvicorn[standard] == 0.20.0
-Requires-Dist: ellar >= 0.3.4
+Requires-Dist: uvicorn[standard] == 0.22.0
+Requires-Dist: ellar >= 0.3.8
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pytest >=7.1.3,<8.0.0 ; extra == "test"
 Requires-Dist: pytest-cov >=2.12.0,<5.0.0 ; extra == "test"
 Requires-Dist: mypy ==0.971 ; extra == "test"
 Requires-Dist: flake8 >=3.8.3,<7.0.0 ; extra == "test"
 Requires-Dist: black ==22.8.0 ; extra == "test"
 Requires-Dist: isort >=5.0.6,<6.0.0 ; extra == "test"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ellar-cli Version: 0.1.6 Summary: Ellar CLI Tool
+Metadata-Version: 2.1 Name: ellar-cli Version: 0.1.8 Summary: Ellar CLI Tool
 for Scaffolding Ellar Projects, Modules and also running Ellar Commands Author-
 email: Ezeudoh Tochukwu
 ezeudoh@gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: Operating System :: OS
 Independent Classifier: Topic :: Internet Classifier: Topic :: Software
 Development :: Libraries :: Application Frameworks Classifier: Topic ::
@@ -13,16 +13,16 @@
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: AsyncIO Classifier: Topic :: Internet :: WWW/HTTP ::
 HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP Requires-Dist: tomlkit
->=0.11.1,<1.0.0,!=0.11.2,!=0.11.3 Requires-Dist: uvicorn[standard] == 0.20.0
-Requires-Dist: ellar >= 0.3.4 Requires-Dist: pre-commit ; extra == "dev"
+>=0.11.1,<1.0.0,!=0.11.2,!=0.11.3 Requires-Dist: uvicorn[standard] == 0.22.0
+Requires-Dist: ellar >= 0.3.8 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pytest >=7.1.3,<8.0.0 ; extra == "test" Requires-Dist: pytest-
 cov >=2.12.0,<5.0.0 ; extra == "test" Requires-Dist: mypy ==0.971 ; extra ==
 "test" Requires-Dist: flake8 >=3.8.3,<7.0.0 ; extra == "test" Requires-Dist:
 black ==22.8.0 ; extra == "test" Requires-Dist: isort >=5.0.6,<6.0.0 ; extra ==
 "test" Requires-Dist: pytest-asyncio ; extra == "test" Requires-Dist: autoflake
 ; extra == "test" Project-URL: Documentation, https://github.com/eadwinCode/
 ellar-cli Project-URL: Homepage, https://eadwincode.github.io/ellar-cli/
```

