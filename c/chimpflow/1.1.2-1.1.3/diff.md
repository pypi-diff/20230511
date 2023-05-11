# Comparing `tmp/chimpflow-1.1.2.tar.gz` & `tmp/chimpflow-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chimpflow-1.1.2.tar", last modified: Wed May  3 05:06:27 2023, max compression
+gzip compressed data, was "chimpflow-1.1.3.tar", last modified: Thu May 11 09:28:44 2023, max compression
```

## Comparing `chimpflow-1.1.2.tar` & `chimpflow-1.1.3.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.839121 chimpflow-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.827121 chimpflow-1.1.2/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.827121 chimpflow-1.1.2/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.827121 chimpflow-1.1.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.827121 chimpflow-1.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.823121 chimpflow-1.1.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.827121 chimpflow-1.1.2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.827121 chimpflow-1.1.2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.827121 chimpflow-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.827121 chimpflow-1.1.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-03 05:06:15.000000 chimpflow-1.1.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 05:06:15.000000 chimpflow-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-05-03 05:06:27.835121 chimpflow-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-03 05:06:15.000000 chimpflow-1.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.827121 chimpflow-1.1.2/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-03 05:06:15.000000 chimpflow-1.1.2/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.827121 chimpflow-1.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.823121 chimpflow-1.1.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.827121 chimpflow-1.1.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-03 05:06:15.000000 chimpflow-1.1.2/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-05-03 05:06:15.000000 chimpflow-1.1.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.827121 chimpflow-1.1.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-03 05:06:15.000000 chimpflow-1.1.2/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-03 05:06:15.000000 chimpflow-1.1.2/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-03 05:06:15.000000 chimpflow-1.1.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.827121 chimpflow-1.1.2/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.831121 chimpflow-1.1.2/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 05:06:15.000000 chimpflow-1.1.2/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-03 05:06:15.000000 chimpflow-1.1.2/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-03 05:06:15.000000 chimpflow-1.1.2/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-03 05:06:15.000000 chimpflow-1.1.2/docs/user/explanations/25-docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-03 05:06:15.000000 chimpflow-1.1.2/docs/user/explanations/51-todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.831121 chimpflow-1.1.2/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 05:06:15.000000 chimpflow-1.1.2/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-03 05:06:15.000000 chimpflow-1.1.2/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.831121 chimpflow-1.1.2/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.831121 chimpflow-1.1.2/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-03 05:06:15.000000 chimpflow-1.1.2/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 05:06:15.000000 chimpflow-1.1.2/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-03 05:06:15.000000 chimpflow-1.1.2/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 05:06:15.000000 chimpflow-1.1.2/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.831121 chimpflow-1.1.2/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 05:06:15.000000 chimpflow-1.1.2/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-03 05:06:15.000000 chimpflow-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 05:06:27.839121 chimpflow-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.823121 chimpflow-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.831121 chimpflow-1.1.2/src/chimpflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-05-03 05:06:27.000000 chimpflow-1.1.2/src/chimpflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-03 05:06:27.000000 chimpflow-1.1.2/src/chimpflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 05:06:27.000000 chimpflow-1.1.2/src/chimpflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-03 05:06:27.000000 chimpflow-1.1.2/src/chimpflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-03 05:06:27.000000 chimpflow-1.1.2/src/chimpflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 05:06:27.000000 chimpflow-1.1.2/src/chimpflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.831121 chimpflow-1.1.2/src/chimpflow_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_api/context_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.831121 chimpflow-1.1.2/src/chimpflow_api/miners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_api/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_api/miners/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_api/miners/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_api/miners/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_api/miners/miners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.831121 chimpflow-1.1.2/src/chimpflow_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.831121 chimpflow-1.1.2/src/chimpflow_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.835121 chimpflow-1.1.2/src/chimpflow_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 05:06:27.000000 chimpflow-1.1.2/src/chimpflow_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_lib/base_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_lib/chimp_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.835121 chimpflow-1.1.2/src/chimpflow_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.835121 chimpflow-1.1.2/src/chimpflow_lib/miners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_lib/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_lib/miners/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_lib/miners/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_lib/miners/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_lib/miners/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_lib/miners/direct_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_lib/miners/miners.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-03 05:06:15.000000 chimpflow-1.1.2/src/chimpflow_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.835121 chimpflow-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:15.000000 chimpflow-1.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-03 05:06:15.000000 chimpflow-1.1.2/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.835121 chimpflow-1.1.2/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-03 05:06:15.000000 chimpflow-1.1.2/tests/configurations/direct_poll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-03 05:06:15.000000 chimpflow-1.1.2/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-03 05:06:15.000000 chimpflow-1.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:06:27.835121 chimpflow-1.1.2/tests/echo_test_imgs/
--rw-r--r--   0 runner    (1001) docker     (123)   156218 2023-05-03 05:06:15.000000 chimpflow-1.1.2/tests/echo_test_imgs/97wo_01A_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   146361 2023-05-03 05:06:15.000000 chimpflow-1.1.2/tests/echo_test_imgs/97wo_01A_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   142418 2023-05-03 05:06:15.000000 chimpflow-1.1.2/tests/echo_test_imgs/97wo_01A_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-05-03 05:06:15.000000 chimpflow-1.1.2/tests/test_chimp_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-03 05:06:15.000000 chimpflow-1.1.2/tests/test_miner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.823770 chimpflow-1.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.811770 chimpflow-1.1.3/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.811770 chimpflow-1.1.3/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.811770 chimpflow-1.1.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.811770 chimpflow-1.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.807770 chimpflow-1.1.3/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.811770 chimpflow-1.1.3/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.811770 chimpflow-1.1.3/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.811770 chimpflow-1.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.811770 chimpflow-1.1.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-11 09:28:34.000000 chimpflow-1.1.3/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-11 09:28:34.000000 chimpflow-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-05-11 09:28:44.823770 chimpflow-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-11 09:28:34.000000 chimpflow-1.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.815770 chimpflow-1.1.3/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-11 09:28:34.000000 chimpflow-1.1.3/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.815770 chimpflow-1.1.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.807770 chimpflow-1.1.3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.815770 chimpflow-1.1.3/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-11 09:28:34.000000 chimpflow-1.1.3/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-05-11 09:28:34.000000 chimpflow-1.1.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.815770 chimpflow-1.1.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-11 09:28:34.000000 chimpflow-1.1.3/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-11 09:28:34.000000 chimpflow-1.1.3/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-11 09:28:34.000000 chimpflow-1.1.3/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.815770 chimpflow-1.1.3/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.815770 chimpflow-1.1.3/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-11 09:28:34.000000 chimpflow-1.1.3/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-11 09:28:34.000000 chimpflow-1.1.3/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-11 09:28:34.000000 chimpflow-1.1.3/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-11 09:28:34.000000 chimpflow-1.1.3/docs/user/explanations/25-docs-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 09:28:34.000000 chimpflow-1.1.3/docs/user/explanations/51-todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.815770 chimpflow-1.1.3/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-11 09:28:34.000000 chimpflow-1.1.3/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-11 09:28:34.000000 chimpflow-1.1.3/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.815770 chimpflow-1.1.3/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.815770 chimpflow-1.1.3/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-11 09:28:34.000000 chimpflow-1.1.3/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-11 09:28:34.000000 chimpflow-1.1.3/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-11 09:28:34.000000 chimpflow-1.1.3/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-11 09:28:34.000000 chimpflow-1.1.3/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.815770 chimpflow-1.1.3/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-11 09:28:34.000000 chimpflow-1.1.3/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-11 09:28:34.000000 chimpflow-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 09:28:44.823770 chimpflow-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.811770 chimpflow-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.815770 chimpflow-1.1.3/src/chimpflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-05-11 09:28:44.000000 chimpflow-1.1.3/src/chimpflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-11 09:28:44.000000 chimpflow-1.1.3/src/chimpflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:28:44.000000 chimpflow-1.1.3/src/chimpflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-11 09:28:44.000000 chimpflow-1.1.3/src/chimpflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-11 09:28:44.000000 chimpflow-1.1.3/src/chimpflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-11 09:28:44.000000 chimpflow-1.1.3/src/chimpflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.815770 chimpflow-1.1.3/src/chimpflow_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_api/context_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.819770 chimpflow-1.1.3/src/chimpflow_api/miners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_api/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_api/miners/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_api/miners/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_api/miners/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_api/miners/miners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_api/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_api/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.819770 chimpflow-1.1.3/src/chimpflow_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.819770 chimpflow-1.1.3/src/chimpflow_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.819770 chimpflow-1.1.3/src/chimpflow_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 09:28:44.000000 chimpflow-1.1.3/src/chimpflow_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_lib/base_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_lib/chimp_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.819770 chimpflow-1.1.3/src/chimpflow_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.819770 chimpflow-1.1.3/src/chimpflow_lib/miners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_lib/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_lib/miners/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_lib/miners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_lib/miners/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_lib/miners/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_lib/miners/direct_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_lib/miners/miners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-11 09:28:34.000000 chimpflow-1.1.3/src/chimpflow_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.823770 chimpflow-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:34.000000 chimpflow-1.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-11 09:28:34.000000 chimpflow-1.1.3/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.823770 chimpflow-1.1.3/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-11 09:28:34.000000 chimpflow-1.1.3/tests/configurations/direct_poll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-11 09:28:34.000000 chimpflow-1.1.3/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-11 09:28:34.000000 chimpflow-1.1.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:28:44.823770 chimpflow-1.1.3/tests/echo_test_imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)   156218 2023-05-11 09:28:34.000000 chimpflow-1.1.3/tests/echo_test_imgs/97wo_01A_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   146361 2023-05-11 09:28:34.000000 chimpflow-1.1.3/tests/echo_test_imgs/97wo_01A_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   142418 2023-05-11 09:28:34.000000 chimpflow-1.1.3/tests/echo_test_imgs/97wo_01A_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-11 09:28:34.000000 chimpflow-1.1.3/tests/test_chimp_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-11 09:28:34.000000 chimpflow-1.1.3/tests/test_miner.py
```

### Comparing `chimpflow-1.1.2/.dae-devops/Makefile` & `chimpflow-1.1.3/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.dae-devops/docs/conventions.rst` & `chimpflow-1.1.3/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.dae-devops/docs/developing.rst` & `chimpflow-1.1.3/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.dae-devops/docs/devops.rst` & `chimpflow-1.1.3/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.dae-devops/docs/docs_structure.rst` & `chimpflow-1.1.3/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.dae-devops/docs/installing.rst` & `chimpflow-1.1.3/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.dae-devops/docs/testing.rst` & `chimpflow-1.1.3/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.dae-devops/project.yaml` & `chimpflow-1.1.3/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.devcontainer/Dockerfile` & `chimpflow-1.1.3/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.devcontainer/devcontainer.json` & `chimpflow-1.1.3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.github/CONTRIBUTING.rst` & `chimpflow-1.1.3/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.github/actions/install_requirements/action.yml` & `chimpflow-1.1.3/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.github/dependabot.yml` & `chimpflow-1.1.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.github/pages/make_switcher.py` & `chimpflow-1.1.3/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.github/workflows/code.yml` & `chimpflow-1.1.3/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.github/workflows/docs.yml` & `chimpflow-1.1.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.github/workflows/docs_clean.yml` & `chimpflow-1.1.3/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.github/workflows/linkcheck.yml` & `chimpflow-1.1.3/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.gitignore` & `chimpflow-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.gitlab-ci.yml` & `chimpflow-1.1.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/.vscode/launch.json` & `chimpflow-1.1.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/LICENSE` & `chimpflow-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/PKG-INFO` & `chimpflow-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chimpflow
-Version: 1.1.2
+Version: 1.1.3
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `chimpflow-1.1.2/README.rst` & `chimpflow-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/configurations/development.yaml` & `chimpflow-1.1.3/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/docs/conf.py` & `chimpflow-1.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/docs/images/dls-favicon.ico` & `chimpflow-1.1.3/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/docs/images/dls-logo.svg` & `chimpflow-1.1.3/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/docs/index.rst` & `chimpflow-1.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/docs/user/explanations/25-docs-structure.rst` & `chimpflow-1.1.3/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/docs/user/index.rst` & `chimpflow-1.1.3/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/pyproject.toml` & `chimpflow-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow.egg-info/PKG-INFO` & `chimpflow-1.1.3/src/chimpflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chimpflow
-Version: 1.1.2
+Version: 1.1.3
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `chimpflow-1.1.2/src/chimpflow.egg-info/SOURCES.txt` & `chimpflow-1.1.3/src/chimpflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_api/context_base.py` & `chimpflow-1.1.3/src/chimpflow_api/context_base.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_api/exceptions.py` & `chimpflow-1.1.3/src/chimpflow_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_api/miners/aiohttp.py` & `chimpflow-1.1.3/src/chimpflow_api/miners/aiohttp.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_api/miners/context.py` & `chimpflow-1.1.3/src/chimpflow_api/miners/context.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_api/miners/miners.py` & `chimpflow-1.1.3/src/chimpflow_api/miners/miners.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_api/thing.py` & `chimpflow-1.1.3/src/chimpflow_api/thing.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_api/things.py` & `chimpflow-1.1.3/src/chimpflow_api/things.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_cli/main.py` & `chimpflow-1.1.3/src/chimpflow_cli/main.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_cli/subcommands/base.py` & `chimpflow-1.1.3/src/chimpflow_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_cli/subcommands/service.py` & `chimpflow-1.1.3/src/chimpflow_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_cli/version.py` & `chimpflow-1.1.3/src/chimpflow_cli/version.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_lib/__main__.py` & `chimpflow-1.1.3/src/chimpflow_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_lib/chimp_adapter.py` & `chimpflow-1.1.3/src/chimpflow_lib/chimp_adapter.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_lib/contexts/base.py` & `chimpflow-1.1.3/src/chimpflow_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_lib/exceptions.py` & `chimpflow-1.1.3/src/chimpflow_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_lib/miners/aiohttp.py` & `chimpflow-1.1.3/src/chimpflow_lib/miners/aiohttp.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             multiprocessing.current_process().name = "miner.chimpflow"
 
             self.activate_process_base()
 
         except Exception as exception:
             logger.exception("exception in miner process", exc_info=exception)
 
-        logger.debug(f"[PIDAL] {callsign(self)} is returning from activate_process")
+        logger.debug(f"[DISSHU] {callsign(self)} is returning from activate_process")
 
     # ----------------------------------------------------------------------------------------
     def activate_thread(self, loop) -> None:
         """
         Activate the direct miner and web server in a new thread.
 
         Meant to be called from inside a newly created thread.
```

### Comparing `chimpflow-1.1.2/src/chimpflow_lib/miners/base.py` & `chimpflow-1.1.3/src/chimpflow_lib/miners/base.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_lib/miners/context.py` & `chimpflow-1.1.3/src/chimpflow_lib/miners/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,20 +71,18 @@
 
         Stop service if one was started and releases any client resources.
         """
 
         if self.server is not None:
             if self.context_specification.get("start_as") == "process":
                 logger.info(
-                    "[NEWSHUT] in context exit, sending shutdown to client process"
+                    "[DISSHU] in context exit, sending shutdown to client process"
                 )
                 # Put in request to shutdown the server.
                 await self.server.client_shutdown()
-                logger.info(
-                    "[NEWSHUT] in context exit, sent shutdown to client process"
-                )
+                logger.info("[DISSHU] in context exit, sent shutdown to client process")
 
             if self.context_specification.get("start_as") == "coro":
                 await self.server.direct_shutdown()
 
             if self.context_specification.get("start_as") == "direct":
                 await self.server.deactivate()
```

### Comparing `chimpflow-1.1.2/src/chimpflow_lib/miners/direct_poll.py` & `chimpflow-1.1.3/src/chimpflow_lib/miners/direct_poll.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,17 +109,17 @@
             # Wait for the ticking to stop.
             await self.__tick_future
 
         # Forget we have an xchembku client reference.
         self.__xchembku = None
 
         if self.__xchembku_client_context is not None:
-            logger.debug(f"[ECHDON] {callsign(self)} exiting __xchembku_client_context")
+            logger.debug(f"[DISSHU] {callsign(self)} exiting __xchembku_client_context")
             await self.__xchembku_client_context.aexit()
-            logger.debug(f"[ECHDON] {callsign(self)} exited __xchembku_client_context")
+            logger.debug(f"[DISSHU] {callsign(self)} exited __xchembku_client_context")
             self.__xchembku_client_context = None
 
     # ----------------------------------------------------------------------------------------
     async def tick(self) -> None:
         """
         A coro task which does periodic checking for new eligible images from xchembku.
```

### Comparing `chimpflow-1.1.2/src/chimpflow_lib/miners/miners.py` & `chimpflow-1.1.3/src/chimpflow_lib/miners/miners.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/src/chimpflow_lib/version.py` & `chimpflow-1.1.3/src/chimpflow_lib/version.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/tests/base.py` & `chimpflow-1.1.3/tests/base.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/tests/configurations/direct_poll.yaml` & `chimpflow-1.1.3/tests/configurations/direct_poll.yaml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/tests/configurations/service.yaml` & `chimpflow-1.1.3/tests/configurations/service.yaml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/tests/conftest.py` & `chimpflow-1.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/tests/echo_test_imgs/97wo_01A_1.jpg` & `chimpflow-1.1.3/tests/echo_test_imgs/97wo_01A_1.jpg`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/tests/echo_test_imgs/97wo_01A_2.jpg` & `chimpflow-1.1.3/tests/echo_test_imgs/97wo_01A_2.jpg`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/tests/echo_test_imgs/97wo_01A_3.jpg` & `chimpflow-1.1.3/tests/echo_test_imgs/97wo_01A_3.jpg`

 * *Files identical despite different names*

### Comparing `chimpflow-1.1.2/tests/test_chimp_adapter.py` & `chimpflow-1.1.3/tests/test_chimp_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,22 +47,25 @@
         }
 
         # Do the work in a separate process.
         # TODO: Figure out how to release resources from torchvision in process.
         p = multiprocessing.Process(target=self.__process, args=[self.__run_97wo_01A_1])
         p.start()
         p.join()
+        assert p.exitcode == 0
 
         p = multiprocessing.Process(target=self.__process, args=[self.__run_97wo_01A_2])
         p.start()
         p.join()
+        assert p.exitcode == 0
 
         p = multiprocessing.Process(target=self.__process, args=[self.__run_97wo_01A_3])
         p.start()
         p.join()
+        assert p.exitcode == 0
 
     # ----------------------------------------------------------------------------------------
     def __process(self, run):
         chimp_adapter = ChimpAdapter(self.__specification)
 
         run(chimp_adapter)
 
@@ -84,16 +87,16 @@
         assert well_model_autolocation.drop_detected
 
         assert well_model_autolocation.number_of_crystals == pytest.approx(30, 1)
 
         assert well_model_autolocation.auto_target_x == pytest.approx(479, 3)
         assert well_model_autolocation.auto_target_y == pytest.approx(475, 3)
 
-        assert well_model_autolocation.well_centroid_x == 600
-        assert well_model_autolocation.well_centroid_y == 504
+        assert well_model_autolocation.well_centroid_x == 630
+        assert well_model_autolocation.well_centroid_y == 494
 
     # ----------------------------------------------------------------------------------------
     def __run_97wo_01A_2(self, chimp_adapter):
 
         # Make a well model to serve as the input to the chimp adapter process method.
         well_model = CrystalWellModel(
             position="01A_2",
@@ -109,16 +112,16 @@
         assert well_model_autolocation.drop_detected
 
         assert well_model_autolocation.number_of_crystals == pytest.approx(13, 1)
 
         assert well_model_autolocation.auto_target_x == pytest.approx(475, 3)
         assert well_model_autolocation.auto_target_y == pytest.approx(745, 3)
 
-        assert well_model_autolocation.well_centroid_x == 600
-        assert well_model_autolocation.well_centroid_y == 536
+        assert well_model_autolocation.well_centroid_x == 630
+        assert well_model_autolocation.well_centroid_y == 526
 
     # ----------------------------------------------------------------------------------------
     def __run_97wo_01A_3(self, chimp_adapter):
 
         # Make a well model to serve as the input to the chimp adapter process method.
         well_model = CrystalWellModel(
             position="01A_3",
@@ -134,9 +137,9 @@
         assert well_model_autolocation.drop_detected
 
         assert well_model_autolocation.number_of_crystals == pytest.approx(2, 1)
 
         assert well_model_autolocation.auto_target_x == pytest.approx(417, 3)
         assert well_model_autolocation.auto_target_y == pytest.approx(672, 3)
 
-        assert well_model_autolocation.well_centroid_x == 608
-        assert well_model_autolocation.well_centroid_y == 504
+        assert well_model_autolocation.well_centroid_x == 638
+        assert well_model_autolocation.well_centroid_y == 494
```

### Comparing `chimpflow-1.1.2/tests/test_miner.py` & `chimpflow-1.1.3/tests/test_miner.py`

 * *Files identical despite different names*

