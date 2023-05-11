# Comparing `tmp/echolocator-1.2.0.tar.gz` & `tmp/echolocator-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echolocator-1.2.0.tar", last modified: Fri May  5 11:50:45 2023, max compression
+gzip compressed data, was "echolocator-1.3.0.tar", last modified: Thu May 11 06:45:48 2023, max compression
```

## Comparing `echolocator-1.2.0.tar` & `echolocator-1.3.0.tar`

### file list

```diff
@@ -1,214 +1,217 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.773450 echolocator-1.2.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.773450 echolocator-1.2.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-05 11:50:37.000000 echolocator-1.2.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.773450 echolocator-1.2.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-05 11:50:37.000000 echolocator-1.2.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-05 11:50:37.000000 echolocator-1.2.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.773450 echolocator-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.769450 echolocator-1.2.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-05 11:50:37.000000 echolocator-1.2.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-05 11:50:37.000000 echolocator-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-05 11:50:37.000000 echolocator-1.2.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-05 11:50:37.000000 echolocator-1.2.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-05 11:50:37.000000 echolocator-1.2.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-05 11:50:37.000000 echolocator-1.2.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-05 11:50:37.000000 echolocator-1.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-05 11:50:37.000000 echolocator-1.2.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 11:50:37.000000 echolocator-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-05-05 11:50:37.000000 echolocator-1.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-05-05 11:50:45.789451 echolocator-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-05 11:50:37.000000 echolocator-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-05 11:50:37.000000 echolocator-1.2.0/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/docs/1_tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/1_tutorials/101_run_conda.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/1_tutorials/102_update_image.rst
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/1_tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/docs/2_how-to/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/2_how-to/201_add_fields.rst
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/2_how-to.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/docs/3_explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/3_explanations/301_naming_conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/3_explanations/302_process.rst
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/3_explanations.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/docs/4_reference/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/4_reference/402_building_conda.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/4_reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.777450 echolocator-1.2.0/docs/diagrams/
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/diagrams/3drop_texrank_coordinates.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/images/excalidraw-example.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/images/git_merge.png
--rw-r--r--   0 runner    (1001) docker     (123)   703604 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/images/image_details.png
--rw-r--r--   0 runner    (1001) docker     (123)   135258 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/images/image_list.png
--rw-r--r--   0 runner    (1001) docker     (123)   142461 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/images/swiss3.png
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 11:50:37.000000 echolocator-1.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/modulefiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-05 11:50:37.000000 echolocator-1.2.0/modulefiles/conda
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-05 11:50:37.000000 echolocator-1.2.0/modulefiles/paths
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-05 11:50:37.000000 echolocator-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:50:45.789451 echolocator-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.769450 echolocator-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-05-05 11:50:45.000000 echolocator-1.2.0/src/echolocator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-05-05 11:50:45.000000 echolocator-1.2.0/src/echolocator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:50:45.000000 echolocator-1.2.0/src/echolocator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-05 11:50:45.000000 echolocator-1.2.0/src/echolocator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-05 11:50:45.000000 echolocator-1.2.0/src/echolocator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-05 11:50:45.000000 echolocator-1.2.0/src/echolocator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator_api/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_api/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 11:50:45.000000 echolocator-1.2.0/src/echolocator_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator_lib/composers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/composers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/composers/composers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/composers/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/composers/prettyhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/composers/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.781450 echolocator-1.2.0/src/echolocator_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23452 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/css/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/css/image_edit_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/css/image_list_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/css/pixel_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/css/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/css/system_health_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/images/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/images/green_dot_crosshair.png
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/images/radial1.666.png
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/common/base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/events.js
--rw-r--r--   0 runner    (1001) docker     (123)    19504 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/page.js
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.773450 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.773450 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.773450 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.785451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.773450 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/raphael/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/runtime.js
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/version.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/hair/
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/spreader.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/ring.js
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/transformer.js
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-05 11:50:37.000000 echolocator-1.2.0/src/echolocator_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/tests/example_images/
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/example_images/1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/example_images/2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/example_images/3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/example_images/4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:45.789451 echolocator-1.2.0/tests/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/images/1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/images/2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/images/3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/test_droplocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/test_export_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/test_export_to_soakdb3.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/test_fetch_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-05 11:50:37.000000 echolocator-1.2.0/tests/test_fetch_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.592593 echolocator-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.556593 echolocator-1.3.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-11 06:45:29.000000 echolocator-1.3.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.560593 echolocator-1.3.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-11 06:45:29.000000 echolocator-1.3.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-11 06:45:29.000000 echolocator-1.3.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-11 06:45:29.000000 echolocator-1.3.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-11 06:45:29.000000 echolocator-1.3.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-11 06:45:29.000000 echolocator-1.3.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-11 06:45:29.000000 echolocator-1.3.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-11 06:45:29.000000 echolocator-1.3.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-11 06:45:29.000000 echolocator-1.3.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.560593 echolocator-1.3.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-11 06:45:29.000000 echolocator-1.3.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-11 06:45:29.000000 echolocator-1.3.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.560593 echolocator-1.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-11 06:45:29.000000 echolocator-1.3.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.548593 echolocator-1.3.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.560593 echolocator-1.3.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-11 06:45:29.000000 echolocator-1.3.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-11 06:45:29.000000 echolocator-1.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.560593 echolocator-1.3.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-11 06:45:29.000000 echolocator-1.3.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-11 06:45:29.000000 echolocator-1.3.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.560593 echolocator-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-11 06:45:29.000000 echolocator-1.3.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-11 06:45:29.000000 echolocator-1.3.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-11 06:45:29.000000 echolocator-1.3.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-11 06:45:29.000000 echolocator-1.3.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-11 06:45:29.000000 echolocator-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-11 06:45:29.000000 echolocator-1.3.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-11 06:45:29.000000 echolocator-1.3.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.560593 echolocator-1.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-11 06:45:29.000000 echolocator-1.3.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-11 06:45:29.000000 echolocator-1.3.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-11 06:45:29.000000 echolocator-1.3.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-11 06:45:29.000000 echolocator-1.3.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-11 06:45:29.000000 echolocator-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-05-11 06:45:29.000000 echolocator-1.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-05-11 06:45:48.588593 echolocator-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-11 06:45:29.000000 echolocator-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.564593 echolocator-1.3.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-11 06:45:29.000000 echolocator-1.3.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.564593 echolocator-1.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.564593 echolocator-1.3.0/docs/1_tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/1_tutorials/101_run_conda.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/1_tutorials/102_update_image.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/1_tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.564593 echolocator-1.3.0/docs/2_how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/2_how-to/201_add_fields.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/2_how-to.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.564593 echolocator-1.3.0/docs/3_explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/3_explanations/301_naming_conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/3_explanations/302_process.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/3_explanations.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.564593 echolocator-1.3.0/docs/4_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/4_reference/402_building_conda.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/4_reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.564593 echolocator-1.3.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.564593 echolocator-1.3.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.564593 echolocator-1.3.0/docs/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/diagrams/3drop_texrank_coordinates.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.568593 echolocator-1.3.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/images/excalidraw-example.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/images/git_merge.png
+-rw-r--r--   0 runner    (1001) docker     (123)   703604 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/images/image_details.png
+-rw-r--r--   0 runner    (1001) docker     (123)   135258 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/images/image_list.png
+-rw-r--r--   0 runner    (1001) docker     (123)   142461 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/images/swiss3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-11 06:45:29.000000 echolocator-1.3.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.568593 echolocator-1.3.0/modulefiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-11 06:45:29.000000 echolocator-1.3.0/modulefiles/conda
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-11 06:45:29.000000 echolocator-1.3.0/modulefiles/paths
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-11 06:45:29.000000 echolocator-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 06:45:48.592593 echolocator-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.552593 echolocator-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.568593 echolocator-1.3.0/src/echolocator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-05-11 06:45:48.000000 echolocator-1.3.0/src/echolocator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-05-11 06:45:48.000000 echolocator-1.3.0/src/echolocator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 06:45:48.000000 echolocator-1.3.0/src/echolocator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-11 06:45:48.000000 echolocator-1.3.0/src/echolocator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-11 06:45:48.000000 echolocator-1.3.0/src/echolocator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 06:45:48.000000 echolocator-1.3.0/src/echolocator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.568593 echolocator-1.3.0/src/echolocator_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_api/context_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.568593 echolocator-1.3.0/src/echolocator_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_api/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.572593 echolocator-1.3.0/src/echolocator_api/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_api/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_api/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_api/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_api/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_api/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.572593 echolocator-1.3.0/src/echolocator_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.572593 echolocator-1.3.0/src/echolocator_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.572593 echolocator-1.3.0/src/echolocator_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 06:45:48.000000 echolocator-1.3.0/src/echolocator_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.572593 echolocator-1.3.0/src/echolocator_lib/composers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/composers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/composers/composers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/composers/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/composers/prettyhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/composers/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.572593 echolocator-1.3.0/src/echolocator_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.576593 echolocator-1.3.0/src/echolocator_lib/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29336 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.576593 echolocator-1.3.0/src/echolocator_lib/guis/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.576593 echolocator-1.3.0/src/echolocator_lib/guis/html/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/css/image_edit_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/css/image_list_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.576593 echolocator-1.3.0/src/echolocator_lib/guis/html/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/css/pixel_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/css/plate_list_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/css/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/css/system_health_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.576593 echolocator-1.3.0/src/echolocator_lib/guis/html/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/images/green_dot_crosshair.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/images/radial1.666.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.576593 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.580593 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/common/base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.580593 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/events.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/page.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/plate_list_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.556593 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.580593 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.556593 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.580593 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.556593 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.584593 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.584593 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.556593 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/raphael/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.584593 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/runtime.js
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/version.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.584593 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/webviz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.588593 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/webviz/hair/
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/webviz/spreader.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.588593 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/ring.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/webviz/transformer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-11 06:45:29.000000 echolocator-1.3.0/src/echolocator_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.588593 echolocator-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:29.000000 echolocator-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-05-11 06:45:29.000000 echolocator-1.3.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.588593 echolocator-1.3.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-11 06:45:29.000000 echolocator-1.3.0/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-11 06:45:29.000000 echolocator-1.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.588593 echolocator-1.3.0/tests/example_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-11 06:45:29.000000 echolocator-1.3.0/tests/example_images/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-05-11 06:45:29.000000 echolocator-1.3.0/tests/example_images/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-05-11 06:45:29.000000 echolocator-1.3.0/tests/example_images/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-05-11 06:45:29.000000 echolocator-1.3.0/tests/example_images/4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:45:48.588593 echolocator-1.3.0/tests/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-11 06:45:29.000000 echolocator-1.3.0/tests/images/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-05-11 06:45:29.000000 echolocator-1.3.0/tests/images/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-05-11 06:45:29.000000 echolocator-1.3.0/tests/images/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-05-11 06:45:29.000000 echolocator-1.3.0/tests/test_droplocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-05-11 06:45:29.000000 echolocator-1.3.0/tests/test_export_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-05-11 06:45:29.000000 echolocator-1.3.0/tests/test_export_to_soakdb3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-05-11 06:45:29.000000 echolocator-1.3.0/tests/test_fetch_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-05-11 06:45:29.000000 echolocator-1.3.0/tests/test_fetch_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-05-11 06:45:29.000000 echolocator-1.3.0/tests/test_report_plates.py
```

### Comparing `echolocator-1.2.0/.dae-devops/Makefile` & `echolocator-1.3.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.dae-devops/docs/conventions.rst` & `echolocator-1.3.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.dae-devops/docs/developing.rst` & `echolocator-1.3.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.dae-devops/docs/devops.rst` & `echolocator-1.3.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.dae-devops/docs/docs_structure.rst` & `echolocator-1.3.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.dae-devops/docs/installing.rst` & `echolocator-1.3.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.dae-devops/docs/testing.rst` & `echolocator-1.3.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.dae-devops/project.yaml` & `echolocator-1.3.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.devcontainer/Dockerfile` & `echolocator-1.3.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.devcontainer/devcontainer.json` & `echolocator-1.3.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.github/CONTRIBUTING.rst` & `echolocator-1.3.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.github/actions/install_requirements/action.yml` & `echolocator-1.3.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.github/dependabot.yml` & `echolocator-1.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.github/pages/make_switcher.py` & `echolocator-1.3.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.github/workflows/code.yml` & `echolocator-1.3.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.github/workflows/docs.yml` & `echolocator-1.3.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.github/workflows/docs_clean.yml` & `echolocator-1.3.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.github/workflows/linkcheck.yml` & `echolocator-1.3.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.gitignore` & `echolocator-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.gitlab-ci.yml` & `echolocator-1.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/.vscode/launch.json` & `echolocator-1.3.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/LICENSE` & `echolocator-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/Makefile` & `echolocator-1.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/PKG-INFO` & `echolocator-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echolocator
-Version: 1.2.0
+Version: 1.3.0
 Summary: XChem GUI for manually targeting drop points for the Echo dispenser.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `echolocator-1.2.0/README.rst` & `echolocator-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/configurations/development.yaml` & `echolocator-1.3.0/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/docs/1_tutorials/101_run_conda.rst` & `echolocator-1.3.0/docs/1_tutorials/101_run_conda.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/docs/1_tutorials/102_update_image.rst` & `echolocator-1.3.0/docs/1_tutorials/102_update_image.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/docs/2_how-to/201_add_fields.rst` & `echolocator-1.3.0/docs/2_how-to/201_add_fields.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/docs/3_explanations/301_naming_conventions.rst` & `echolocator-1.3.0/docs/3_explanations/301_naming_conventions.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/docs/3_explanations/302_process.rst` & `echolocator-1.3.0/docs/3_explanations/302_process.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/docs/4_reference/402_building_conda.rst` & `echolocator-1.3.0/docs/4_reference/402_building_conda.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/docs/_static/theme_overrides.css` & `echolocator-1.3.0/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/docs/conf.py` & `echolocator-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/docs/diagrams/3drop_texrank_coordinates.drawio` & `echolocator-1.3.0/docs/diagrams/3drop_texrank_coordinates.drawio`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/docs/images/dls-favicon.ico` & `echolocator-1.3.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/docs/images/dls-logo.svg` & `echolocator-1.3.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/docs/images/excalidraw-example.svg` & `echolocator-1.3.0/docs/images/excalidraw-example.svg`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/docs/images/git_merge.png` & `echolocator-1.3.0/docs/images/git_merge.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/docs/images/image_details.png` & `echolocator-1.3.0/docs/images/image_details.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/docs/images/image_list.png` & `echolocator-1.3.0/docs/images/image_list.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/docs/images/swiss3.png` & `echolocator-1.3.0/docs/images/swiss3.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/modulefiles/conda` & `echolocator-1.3.0/modulefiles/conda`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/pyproject.toml` & `echolocator-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator.egg-info/PKG-INFO` & `echolocator-1.3.0/src/echolocator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echolocator
-Version: 1.2.0
+Version: 1.3.0
 Summary: XChem GUI for manually targeting drop points for the Echo dispenser.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `echolocator-1.2.0/src/echolocator.egg-info/SOURCES.txt` & `echolocator-1.3.0/src/echolocator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -96,28 +96,30 @@
 src/echolocator_lib/guis/context.py
 src/echolocator_lib/guis/guis.py
 src/echolocator_lib/guis/html/index.html
 src/echolocator_lib/guis/html/index.js
 src/echolocator_lib/guis/html/css/image_edit_ux.css
 src/echolocator_lib/guis/html/css/image_list_ux.css
 src/echolocator_lib/guis/html/css/pixel_ux.css
+src/echolocator_lib/guis/html/css/plate_list_ux.css
 src/echolocator_lib/guis/html/css/styles.css
 src/echolocator_lib/guis/html/css/system_health_ux.css
 src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png
 src/echolocator_lib/guis/html/images/green_dot_crosshair.png
 src/echolocator_lib/guis/html/images/radial1.666.png
 src/echolocator_lib/guis/html/javascript/runtime.js
 src/echolocator_lib/guis/html/javascript/version.js
 src/echolocator_lib/guis/html/javascript/common/base.js
 src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js
 src/echolocator_lib/guis/html/javascript/echolocator/events.js
 src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js
 src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js
 src/echolocator_lib/guis/html/javascript/echolocator/page.js
 src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js
+src/echolocator_lib/guis/html/javascript/echolocator/plate_list_ux.js
 src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js
 src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js
 src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js
 src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js
 src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js
 src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
 src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
@@ -143,14 +145,15 @@
 tests/base.py
 tests/conftest.py
 tests/test_droplocation.py
 tests/test_export_to_csv.py
 tests/test_export_to_soakdb3.py
 tests/test_fetch_image.py
 tests/test_fetch_images.py
+tests/test_report_plates.py
 tests/configurations/service.yaml
 tests/example_images/1.jpg
 tests/example_images/2.jpg
 tests/example_images/3.jpg
 tests/example_images/4.png
 tests/images/1.jpg
 tests/images/2.jpg
```

### Comparing `echolocator-1.2.0/src/echolocator_api/context_base.py` & `echolocator-1.3.0/src/echolocator_api/context_base.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_api/databases/constants.py` & `echolocator-1.3.0/src/echolocator_api/databases/constants.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_api/exceptions.py` & `echolocator-1.3.0/src/echolocator_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_api/guis/aiohttp.py` & `echolocator-1.3.0/src/echolocator_api/guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_api/guis/context.py` & `echolocator-1.3.0/src/echolocator_api/guis/context.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_api/guis/guis.py` & `echolocator-1.3.0/src/echolocator_api/guis/guis.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_cli/main.py` & `echolocator-1.3.0/src/echolocator_cli/main.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_cli/subcommands/base.py` & `echolocator-1.3.0/src/echolocator_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_cli/subcommands/service.py` & `echolocator-1.3.0/src/echolocator_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_cli/version.py` & `echolocator-1.3.0/src/echolocator_cli/version.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/__main__.py` & `echolocator-1.3.0/src/echolocator_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/composers/composers.py` & `echolocator-1.3.0/src/echolocator_lib/composers/composers.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/composers/prettyhelper.py` & `echolocator-1.3.0/src/echolocator_lib/composers/prettyhelper.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/composers/text.py` & `echolocator-1.3.0/src/echolocator_lib/composers/text.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/contexts/base.py` & `echolocator-1.3.0/src/echolocator_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/envvar.py` & `echolocator-1.3.0/src/echolocator_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/aiohttp.py` & `echolocator-1.3.0/src/echolocator_lib/guis/aiohttp.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 from typing import List
 
 from dls_servbase_api.constants import Keywords as ProtocoljKeywords
 
 # Utilities.
 from dls_utilpack.callsign import callsign
+from dls_utilpack.exceptions import EndOfList, ProgrammingFault
 from dls_utilpack.require import require
 
 # Basic things.
 from dls_utilpack.thing import Thing
 from dls_utilpack.visit import get_xchem_directory
 
 # The model which describes the crystal wells to be injected into soakdb3.
@@ -161,30 +162,25 @@
 
         except Exception:
             raise RuntimeError(f"unable to start {callsign(self)} server coro")
 
     # ----------------------------------------------------------------------------------------
     async def direct_shutdown(self):
         """"""
-        logger.debug(f"[ECHDON] {callsign(self)} in direct_shutdown")
 
         # Forget we have an xchembku client reference.
         self.__xchembku = None
 
         if self.__xchembku_client_context is not None:
-            logger.debug(f"[ECHDON] {callsign(self)} exiting __xchembku_client_context")
             await self.__xchembku_client_context.aexit()
-            logger.debug(f"[ECHDON] {callsign(self)} exited __xchembku_client_context")
             self.__xchembku_client_context = None
 
         # Let the base class stop the server event looping.
         await self.base_direct_shutdown()
 
-        logger.debug(f"[ECHDON] {callsign(self)} called base_direct_shutdown")
-
     # ----------------------------------------------------------------------------------------
     async def dispatch(self, request_dict, opaque):
         """"""
 
         command = require("request json", request_dict, Keywords.COMMAND)
 
         # Having no xchembku client reference means we must be shutting down.
@@ -196,20 +192,23 @@
 
         if command == Commands.LOAD_TABS:
             return await self.__load_tabs(opaque, request_dict)
 
         if command == Commands.SELECT_TAB:
             return await self.__select_tab(opaque, request_dict)
 
-        if command == Commands.FETCH_IMAGE:
-            return await self.__fetch_image(opaque, request_dict)
+        elif command == Commands.REPORT_PLATES:
+            return await self.__report_plates(opaque, request_dict)
 
         elif command == Commands.FETCH_IMAGE_LIST:
             return await self.__fetch_image_list(opaque, request_dict)
 
+        if command == Commands.FETCH_IMAGE:
+            return await self.__fetch_image(opaque, request_dict)
+
         elif command == Commands.EXPORT_TO_SOAKDB3:
             return await self.__export_to_soakdb3(opaque, request_dict)
 
         elif command == Commands.EXPORT_TO_CSV:
             return await self.__export_to_csv(opaque, request_dict)
 
         elif command == Commands.UPDATE:
@@ -241,77 +240,69 @@
         self.set_cookie_content(opaque, Cookies.TABS_MANAGER, Keywords.TAB_ID, tab_id)
 
         response = {}
 
         return response
 
     # ----------------------------------------------------------------------------------------
-    async def __fetch_image(self, opaque, request_dict):
+    async def __report_plates(self, opaque, request_dict):
 
-        # Get uuid from the cookie if it's not being posted here.
-        crystal_well_uuid = await self.set_or_get_cookie_content(
+        # Remember last posted value for auto_update_enabled.
+        auto_update_enabled = await self._handle_auto_update(
+            opaque, request_dict, Cookies.PLATE_LIST_UX
+        )
+
+        visit_filter = await self.set_or_get_cookie_content(
             opaque,
-            Cookies.IMAGE_EDIT_UX,
-            "crystal_well_uuid",
-            request_dict.get("crystal_well_uuid"),
-            "",
+            Cookies.PLATE_LIST_UX,
+            "visit_filter",
+            request_dict.get("visit_filter"),
+            None,
         )
 
-        logger.info(
-            f"fetching image from crystal_well_uuid {crystal_well_uuid}"
-            f" direction {request_dict.get('direction')}"
+        should_show_only_needing_intervention = await self.set_or_get_cookie_content(
+            opaque,
+            Cookies.PLATE_LIST_UX,
+            "should_show_only_needing_intervention",
+            request_dict.get("should_show_only_needing_intervention"),
+            False,
         )
 
-        # Not able to get an image from posted value or cookie?
-        # Usually first time visiting Image Details tab when no image picked from list.
-        if crystal_well_uuid == "":
-            response = {"record": None}
-            return response
+        filters = {
+            "visit_filter": visit_filter,
+            "should_show_only_needing_intervention": should_show_only_needing_intervention,
+        }
 
-        # Start a filter where we anchor on the given well.
-        filter = CrystalWellFilterModel(
-            anchor=crystal_well_uuid,
-            limit=1,
-            sortby=CrystalWellFilterSortbyEnum.NUMBER_OF_CRYSTALS,
-        )
-
-        # Caller is providing visit?
-        visit = request_dict.get("visit")
-        if visit is not None:
-            filter.visit = visit
-
-        # Image previous or next?
-        direction = request_dict.get("direction", 0)
-        if direction != 0:
-            filter.direction = direction
+        # Start a filter where default is sorted on reverse.
+        filter = CrystalPlateFilterModel(direction=-1)
 
-        should_show_only_undecided = await self.set_or_get_cookie_content(
-            opaque,
-            Cookies.IMAGE_LIST_UX,
-            "should_show_only_undecided",
-            request_dict.get("should_show_only_undecided"),
-            False,
+        logger.debug(
+            f"fetching image records, visit_filter is '{visit_filter}' and "
+            f" should_show_only_needing_intervention is '{should_show_only_needing_intervention}'"
         )
-        if should_show_only_undecided:
-            filter.is_decided = False
 
-        crystal_well_models = (
-            await self.__xchembku.fetch_crystal_wells_needing_droplocation(filter)
+        if visit_filter is not None and visit_filter.strip() != "":
+            filter.visit = visit_filter
+        if should_show_only_needing_intervention:
+            filter.needing_intervention = True
+
+        # Fetch the list from the xchembku.
+        crystal_plate_report_models = await self.__xchembku.report_crystal_plates(
+            filter
         )
 
-        if len(crystal_well_models) == 0:
-            response = {"record": None}
-            if direction != 0:
-                response["confirmation"] = "there are no more images in this direction"
-            return response
+        html = echolocator_composers_get_default().compose_crystal_plate_report(
+            crystal_plate_report_models
+        )
 
-        # Presumably there is only one image of interest.
-        record = crystal_well_models[0].dict()
-        record["filename"] = "filestore" + record["filename"]
-        response = {"record": record}
+        response = {
+            "html": html,
+            "filters": filters,
+            "auto_update_enabled": auto_update_enabled,
+        }
 
         return response
 
     # ----------------------------------------------------------------------------------------
     async def __fetch_image_list(self, opaque, request_dict):
 
         # Remember last posted value for auto_update_enabled.
@@ -323,74 +314,188 @@
             opaque,
             Cookies.IMAGE_LIST_UX,
             "visit_filter",
             request_dict.get("visit_filter"),
             None,
         )
 
+        barcode_filter = await self.set_or_get_cookie_content(
+            opaque,
+            Cookies.IMAGE_LIST_UX,
+            "barcode_filter",
+            request_dict.get("barcode_filter"),
+            None,
+        )
+
         should_show_only_undecided = await self.set_or_get_cookie_content(
             opaque,
             Cookies.IMAGE_LIST_UX,
             "should_show_only_undecided",
             request_dict.get("should_show_only_undecided"),
             False,
         )
 
+        show_first_image = request_dict.get("show_first_image", False)
+
         if visit_filter is None:
             visit_filter = ""
         visit_filter = visit_filter.strip()
 
+        if barcode_filter is None:
+            barcode_filter = ""
+        barcode_filter = barcode_filter.strip()
+
         filters = {
             "visit_filter": visit_filter,
+            "barcode_filter": barcode_filter,
             "should_show_only_undecided": should_show_only_undecided,
         }
 
         if visit_filter == "":
             html = "please enter a visit"
+            crystal_well_index = None
+            crystal_well_count = None
 
         else:
             logger.debug(
                 f"fetching image records, visit_filter is '{visit_filter}' and "
-                f" should_show_only_undecided is '{should_show_only_undecided}'"
+                f" barcode_filter is '{barcode_filter}' and "
+                f" should_show_only_undecided is '{should_show_only_undecided}' and"
+                f" show_first_image is '{show_first_image}'"
             )
 
-            # Start a filter where we anchor on the given image.
+            # Start a filter for the list based on visit only.
             filter = CrystalWellFilterModel(
                 visit=visit_filter,
                 sortby=CrystalWellFilterSortbyEnum.NUMBER_OF_CRYSTALS,
             )
 
+            if barcode_filter != "":
+                filter.barcode = barcode_filter
+
             should_show_only_undecided = await self.set_or_get_cookie_content(
                 opaque,
                 Cookies.IMAGE_LIST_UX,
                 "should_show_only_undecided",
                 request_dict.get("should_show_only_undecided"),
                 False,
             )
             if should_show_only_undecided:
                 filter.is_decided = False
 
-            # Fetch the list from the xchembku.
+            # Fetch the properly ordered and filtered list from the xchembku.
             crystal_well_models = (
                 await self.__xchembku.fetch_crystal_wells_needing_droplocation(filter)
             )
 
-            html = echolocator_composers_get_default().compose_image_list(
-                crystal_well_models
+            crystal_well_count = len(crystal_well_models)
+
+            # Remember the crystal well uuids in the list in the cookie.
+            crystal_well_uuids = [m.uuid for m in crystal_well_models]
+            self.set_cookie_content(
+                opaque,
+                Cookies.IMAGE_LIST_UX,
+                "crystal_well_uuids",
+                crystal_well_uuids,
             )
 
+            # Asking for first image only, and there are any?
+            if show_first_image and crystal_well_count > 0:
+                # Give the first image index in the response.
+                crystal_well_index = 0
+                # Don't give html in the response.
+                html = None
+            # Asking for image list?
+            else:
+                # Give the html.
+                html = echolocator_composers_get_default().compose_image_list(
+                    crystal_well_models
+                )
+                crystal_well_index = None
+
         response = {
             "html": html,
+            Keywords.CRYSTAL_WELL_INDEX: crystal_well_index,
+            Keywords.CRYSTAL_WELL_COUNT: crystal_well_count,
             "filters": filters,
             "auto_update_enabled": auto_update_enabled,
         }
 
         return response
 
     # ----------------------------------------------------------------------------------------
+    async def __fetch_image(self, opaque, request_dict):
+
+        # Get uuid from the cookie if it's not being posted here.
+        crystal_well_index = await self.set_or_get_cookie_content(
+            opaque,
+            Cookies.IMAGE_EDIT_UX,
+            Keywords.CRYSTAL_WELL_INDEX,
+            request_dict.get(Keywords.CRYSTAL_WELL_INDEX),
+            None,
+        )
+
+        logger.info(f"fetching image from crystal_well_index {crystal_well_index}")
+
+        # Not able to get an image from posted value or cookie?
+        # Usually first time visiting Image Details tab when no image picked from list.
+        if crystal_well_index is None:
+            raise ProgrammingFault(
+                f"no value for {Keywords.CRYSTAL_WELL_INDEX} in post or cookie {Cookies.IMAGE_EDIT_UX}"
+            )
+
+        # Get uuids of the current list from the cookie.
+        crystal_well_uuids = await self.get_cookie_content(
+            opaque,
+            Cookies.IMAGE_LIST_UX,
+            "crystal_well_uuids",
+            None,
+        )
+
+        if crystal_well_uuids is None:
+            raise ProgrammingFault(
+                f"cookie {Cookies.IMAGE_LIST_UX} has no value for crystal_well_uuids"
+            )
+
+        crystal_well_count = len(crystal_well_uuids)
+        if crystal_well_index >= crystal_well_count:
+            raise EndOfList(
+                f"crystal_well_index {crystal_well_index} exceeds crystal_well_uuids length {crystal_well_count}"
+            )
+
+        # The uuid at the posted index.
+        crystal_well_uuid = crystal_well_uuids[crystal_well_index]
+
+        # Filter to get just the single well.
+        filter = CrystalWellFilterModel(anchor=crystal_well_uuid)
+
+        # Get the single record.
+        crystal_well_models = (
+            await self.__xchembku.fetch_crystal_wells_needing_droplocation(filter)
+        )
+
+        if len(crystal_well_models) == 0:
+            raise ProgrammingFault(
+                f"crystal_well_index {crystal_well_index} for uuid {crystal_well_uuid} doesn't exist in the database"
+            )
+
+        # Presumably there is only one image of interest.
+        record = crystal_well_models[0].dict()
+        # Filestore's full path to the image file.
+        record["filename"] = "filestore" + record["filename"]
+        response = {
+            "record": record,
+            # Give back current one and length of the list to help with the prev/next button composing.
+            Keywords.CRYSTAL_WELL_INDEX: crystal_well_index,
+            Keywords.CRYSTAL_WELL_COUNT: crystal_well_count,
+        }
+
+        return response
+
+    # ----------------------------------------------------------------------------------------
     async def __update(self, opaque, request_dict):
 
         t = require("ajax request", request_dict, "crystal_well_droplocation_model")
 
         # Wrap a model around the posted fields.
         crystal_well_droplocation_model = CrystalWellDroplocationModel(**t)
 
@@ -398,43 +503,37 @@
         await self.__xchembku.upsert_crystal_well_droplocations(
             [crystal_well_droplocation_model],
             only_fields=list(t.keys()),
         )
 
         # Caller wants to select the next image automatically?
         if request_dict.get(Keywords.SHOULD_ADVANCE, False):
+            # There is a next image in the sequence?
+            crystal_well_index = request_dict.get(Keywords.CRYSTAL_WELL_INDEX_NEXT)
 
-            # Caller must provide a visit in order to automatically advance.
-            visit = request_dict.get("visit")
-            if visit is None:
-                raise RuntimeError(
-                    "programming error: visit not submitted with request to advance after update"
-                )
-
-            # Advance by fetching the next image record after the update.
-            next_request_dict = {
-                ProtocoljKeywords.ENABLE_COOKIES: [
-                    Cookies.IMAGE_EDIT_UX,
-                    Cookies.IMAGE_LIST_UX,
-                ],
-                Keywords.COMMAND: Commands.FETCH_IMAGE,
-                "crystal_well_uuid": crystal_well_droplocation_model.crystal_well_uuid,
-                "direction": 1,
-                "visit": visit,
-            }
-            response = await self.__fetch_image(opaque, next_request_dict)
-
-            if response.get("record") is not None:
+            if crystal_well_index is not None:
+                # Advance by fetching the next image record after the update.
+                # Filters are provided in the IMAGE_LIST_UX cookie.
+                next_request_dict = {
+                    ProtocoljKeywords.ENABLE_COOKIES: [
+                        Cookies.IMAGE_EDIT_UX,
+                        Cookies.IMAGE_LIST_UX,
+                    ],
+                    Keywords.COMMAND: Commands.FETCH_IMAGE,
+                    Keywords.CRYSTAL_WELL_INDEX: crystal_well_index,
+                }
+                response = await self.__fetch_image(opaque, next_request_dict)
                 response[
                     "confirmation"
                 ] = "drop location has been updated and view advanced to next image"
             else:
-                response[
-                    "confirmation"
-                ] = "drop location has been updated and there are no more images in the list"
+                response = {
+                    "record": None,
+                    "confirmation": "drop location has been updated and have reached the end of the list",
+                }
         else:
             response = {"confirmation": "drop location has been updated"}
 
         return response
 
     # ----------------------------------------------------------------------------------------
     async def __export_to_soakdb3(self, opaque, request_dict):
@@ -446,34 +545,78 @@
 
         # Visit must not be blank.
         visit_filter = visit_filter.strip()
         if visit_filter == "":
             response = {"error": "blank visit was given"}
             return response
 
+        # Caller may provide a barcode.
+        barcode_filter = request_dict.get("barcode_filter", "")
+        barcode_filter = barcode_filter.strip()
+        if barcode_filter == "":
+            barcode_filter = None
+
         # Get a filter for wells we want to export.
         crystal_well_filter = CrystalWellFilterModel(
             visit=visit_filter,
+            barcode=barcode_filter,
             is_decided=True,
             is_usable=True,
             sortby=CrystalWellFilterSortbyEnum.POSITION,
         )
 
         # Fetch the list of wells according to the filter.
         crystal_well_models: List[
             CrystalWellNeedingDroplocationModel
         ] = await self.__xchembku.fetch_crystal_wells_needing_droplocation(
-            crystal_well_filter
+            crystal_well_filter, why="[EXPFIL] get list to be epxorted"
         )
 
+        logger.debug(f"[EXPFIL] found {len(crystal_well_models)} to be exported")
+
         # Export the crystal wells to the appropriate soakdb3 visit.
         await self.__export_to_soakdb3_visit(visit_filter, crystal_well_models)
 
+        # Make the list of droplocations to update with the exported flag.
+        crystal_well_droplocation_models: List[CrystalWellDroplocationModel] = list()
+        for crystal_well_model in crystal_well_models:
+            # We only need the crystal_well_uuid for upserting.
+            # This will have to be revisited if we ever want multiple droplocations on a single well.
+            crystal_well_droplocation_model = CrystalWellDroplocationModel(
+                crystal_well_uuid=crystal_well_model.uuid,
+                is_exported_to_soakdb3=True,
+            )
+            crystal_well_droplocation_models.append(crystal_well_droplocation_model)
+
+        # Update the database for those that just got exported.
+        # TODO: Use a bulk update when setting is_exported_to_soakdb3 field after export.
+        result_counts = await self.__xchembku.upsert_crystal_well_droplocations(
+            crystal_well_droplocation_models,
+            only_fields=["is_exported_to_soakdb3"],
+            why="setting is_exported_to_soakdb3 field after export",
+        )
+
+        logger.debug(f"[EXPFIL] result_counts {result_counts}")
+
+        # ----------------------------------------------------------------------
+        # Start a filter where we anchor on the given image.
+        filter = CrystalPlateFilterModel(direction=-1)
+
+        # Fetch the list from the xchembku.
+        crystal_plate_report_models = await self.__xchembku.report_crystal_plates(
+            filter
+        )
+
+        html = echolocator_composers_get_default().compose_crystal_plate_report(
+            crystal_plate_report_models
+        )
+
         response = {
-            "confirmation": f"exported {len(crystal_well_models)} rows to soakdb3 visit {visit_filter}"
+            "confirmation": f"exported {len(crystal_well_models)} rows to soakdb3 visit {visit_filter}",
+            "html": html,
         }
 
         return response
 
     # ----------------------------------------------------------------------------------------
     async def __export_to_soakdb3_visit(
         self,
```

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/context.py` & `echolocator-1.3.0/src/echolocator_lib/guis/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,17 @@
         elif self.context_specification.get("start_as") == "process":
             logger.debug("starting gui context")
             await self.server.start_process()
 
     # ----------------------------------------------------------------------------------------
     async def aexit(self):
         """ """
-        logger.debug(f"[ECHDON] {thing_type} aexit")
+        logger.debug(f"[DISSHU] {thing_type} aexit")
 
         if self.server is not None:
             if self.context_specification.get("start_as") == "process":
-                logger.debug(f"[ECHDON] {thing_type} calling client_shutdown")
+                logger.debug(f"[DISSHU] {thing_type} calling client_shutdown")
                 # Put in request to shutdown the server.
                 await self.server.client_shutdown()
 
             if self.context_specification.get("start_as") == "coro":
                 await self.server.direct_shutdown()
```

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/guis.py` & `echolocator-1.3.0/src/echolocator_lib/guis/guis.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/css/image_list_ux.css` & `echolocator-1.3.0/src/echolocator_lib/guis/html/css/image_list_ux.css`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     background-color: gray;
     color: white;
     font-weight: bold;
 }
 
 
 #image_list_ux_interaction_parent .T_barcode_filter {
-    width: 320px;
+    width: 64px;
 }
 
 #image_list_ux_interaction_parent .T_is_drop {
     display: none;
 }
 
 #image_list_ux_interaction_parent .T_real_space_target_x,
```

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png` & `echolocator-1.3.0/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/css/styles.css` & `echolocator-1.3.0/src/echolocator_lib/guis/html/css/styles.css`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 BUTTON,
 SELECT,
 INPUT {
   width: 172px;
 }
 
 INPUT[type=checkbox] {
-  width: 22px;
+  width: auto;
+  margin-left: 0px;
 }
 
 
 /* --------------------------------------------------------------------------- */
 .T_side_by_side {
   white-space: nowrap;
   width: 100%;
```

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/images/green_dot_crosshair.png` & `echolocator-1.3.0/src/echolocator_lib/guis/html/images/green_dot_crosshair.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/images/radial1.666.png` & `echolocator-1.3.0/src/echolocator_lib/guis/html/images/radial1.666.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/index.html` & `echolocator-1.3.0/src/echolocator_lib/guis/html/index.html`

 * *Files 24% similar despite different names*

```diff
@@ -29,68 +29,97 @@
     <script src="javascript/echolocator/page.js"></script>
 
     <!-- Logic for this page. -->
     <script src="javascript/echolocator/events.js"></script>
     <script src="javascript/echolocator/ux_base.js"></script>
     <script src="javascript/echolocator/ux_auto_update.js"></script>
     <script src="javascript/echolocator/tabs_manager.js"></script>
+    <script src="javascript/echolocator/plate_list_ux.js"></script>
     <script src="javascript/echolocator/image_list_ux.js"></script>
     <script src="javascript/echolocator/image_edit_ux.js"></script>
     <script src="javascript/echolocator/centroid_ux.js"></script>
     <script src="javascript/echolocator/pixel_ux.js"></script>
 
     <!-- javascript companion to html layout -->
     <script src="index.js"></script>
 
     <!-- Styles for this page. -->
     <link rel="stylesheet" href="css/styles.css">
+    <link rel="stylesheet" href="css/plate_list_ux.css">
     <link rel="stylesheet" href="css/image_list_ux.css">
     <link rel="stylesheet" href="css/image_edit_ux.css">
     <link rel="stylesheet" href="css/pixel_ux.css">
 
 </head>
 
 <body class="body">
     <div id="tabs_manager_interaction_parent">
         <div class="T_tabs" id="tabs">
 
             <ul>
+                <li><a href="#tab-plate-list">Plate List</a></li>
                 <li><a href="#tab-image-list">Image List</a></li>
                 <li><a href="#tab-image-edit">Image Details</a></li>
             </ul>
 
 
+            <div id="tab-plate-list">
+                <div id="plate_list_ux_interaction_parent">
+                    <div class="T_auto_update">
+                        <div class="T_toggle">AUTO</div>
+                        <div class="T_status">-</div>
+                    </div>
+                    <div class="T_inputs" style="margin-top: 8px; margin-bottom: 8px;">
+                        <div class="T_row">
+                            <div class="T_field">
+                                <div class="T_prompt">visit</div>
+                                <div class="T_input"><input type="text" id="visit_filter" class="T_visit_filter"></div>
+                                <div class="T_separator"></div>
+                                <div class="T_prompt">show only needing intervention</div>
+                                <div class="T_input"><input id="should_show_only_needing_intervention" type="checkbox"
+                                        class="T_should_show_only_needing_intervention"></div>
+                            </div>
+                        </div>
+                    </div>
+                    <div class="T_section">
+                        <div class="T_title" title="plate list">Plate List</div>
+                        <div class="T_composed T_plate_list" style="overflow:scroll; height: 100%;">-</div>
+                    </div>
+                </div>
+            </div><!-- tab-plate-list -->
+
+
             <div id="tab-image-list">
                 <div id="image_list_ux_interaction_parent">
                     <div class="T_auto_update">
                         <div class="T_toggle">AUTO</div>
                         <div class="T_status">-</div>
                     </div>
                     <div class="T_buttons" style="margin-top: 8px; margin-bottom: 8px;">
                         <div class="T_field">
                             <div class="T_prompt">visit</div>
-                            <div class="T_input"><input type="text" class="T_visit_filter"></div>
-                            <div class="T_separator"></div>
-                            <button class="T_export_to_soakdb3_button" title="export to soakdb3 database">Export to
-                                Soakdb3</button>
+                            <div class="T_input"><input type="text" id="visit_filter" class="T_visit_filter"></div>
                             <div class="T_separator"></div>
-                            <button class="T_export_to_csv_button" title="export to csv file">Export to CSV</button>
+
+                            <div class="T_prompt">barcode</div>
+                            <div class="T_input"><input type="text" id="barcode_filter" class="T_barcode_filter"></div>
+                            <div class="T_help">Leaving this blank will show wells in all plates of the visit.</div>
                         </div>
                     </div>
                     <div class="T_inputs" style="margin-top: 8px; margin-bottom: 8px;">
                         <div class="T_row">
                             <div class="T_field">
                                 <div class="T_prompt">show only undecided</div>
                                 <div class="T_input"><input type="checkbox" class="T_should_show_only_undecided"></div>
                             </div>
                         </div>
                     </div>
                     <div class="T_section">
                         <div class="T_title" title="image list">Image List</div>
-                        <div class="T_composed T_image_list" style="overflow:scroll;height: 100%;">-</div>
+                        <div class="T_composed T_image_list" style="overflow:scroll; height: 100%;">-</div>
                     </div>
                 </div>
             </div><!-- tab-image-list -->
 
             <div id="tab-image-edit">
                 <div id="image_edit_ux_interaction_parent" tabindex="0">
                     <div class="T_buttons T_hide_when_no_image" style="margin-top: 8px; margin-bottom: 8px;">
@@ -104,28 +133,38 @@
                             (-)</span></button>
                         <button class="T_next_button" title="next image">Next<span class="T_hint"> (right
                                 arrow)</span></button>
                     </div>
 
                     <div class="T_image_info T_hide_when_no_image" style="margin-top: 8px; margin-bottom: 8px;">
                         <div class="T_field">
-                            <div class="T_prompt">filename:</div>
-                            <div class="T_input">
-                                <div class="T_filename"></div>
-                            </div>
+                            <div class="T_prompt">Showing: <span class="T_crystal_well_index"></span> out of <span
+                                    class="T_crystal_well_count"></span></div>
+
                             <div class="T_separator"></div>
                             <div class="T_prompt">Num crystals:</div>
                             <div class="T_input">
                                 <div class="T_number_of_crystals"></div>
                             </div>
                             <div class="T_separator"></div>
                             <div class="T_prompt">is usable?</div>
                             <div class="T_input">
                                 <div class="T_is_usable"></div>
                             </div>
+                            <div class="T_separator"></div>
+                            <div class="T_prompt">is exported?</div>
+                            <div class="T_input">
+                                <div class="T_is_exported_to_soakdb3"></div>
+                            </div>
+                        </div>
+                        <div class="T_field">
+                            <div class="T_prompt">filename:</div>
+                            <div class="T_input">
+                                <div class="T_filename"></div>
+                            </div>
                         </div>
                     </div>
 
                     <div id="image1" class="dataframe T_hide_when_no_image" style="width: 100%;">
                         <div class="container view-container">
                             <div id="image1_viewport" class="viewport">
                                 <img id="detector1_image" src="images/radial1.666.png"
```

#### html2text {}

```diff
@@ -7,25 +7,38 @@
 
 
 
 
 
 
 
+
+    * Plate_List
     * Image_List
     * Image_Details
 AUTO
 -
 visit
 [                    ]
-Export to Soakdb3
-Export to CSV
+show only needing intervention
+⁰
+Plate List
+-
+AUTO
+-
+visit
+[                    ]
+barcode
+[                    ]
+Leaving this blank will show wells in all plates of the visit.
 show only undecided
 ⁰
 Image List
 -
 Previous (left arrow) Usable (space bar) Not Usable (right click or X)
 Undecided (-) Next (right arrow)
-filename:
+Showing:  out of
 Num crystals:
 is usable?
+is exported?
+filename:
 [images/radial1.666.png]
```

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/index.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/index.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,12 @@
 // $(window).resize(function (jquery_event_object) { console.log("WINDOW RESIZE"); });
 
 class Index extends echolocator__Page {
     #tabs_manager = null;
+    #plate_list_ux = null;
     #image_list_ux = null;
     #image_edit_ux = null;
 
     #tab_id_last_opened = null;
 
     constructor(runtime) {
         super(runtime);
@@ -53,14 +54,19 @@
         // -------------------------------------------------------------------
 
         this.#tabs_manager = new echolocator__TabsManager(
             self.runtime,
             "tabs_manager",
             $("#tabs_manager_interaction_parent"));
 
+        this.#plate_list_ux = new echolocator__PlateListUx(
+            self.runtime,
+            "plate_list",
+            $("#plate_list_ux_interaction_parent"));
+
         this.#image_list_ux = new echolocator__ImageListUx(
             self.runtime,
             "image_list",
             $("#image_list_ux_interaction_parent"));
 
         this.#image_edit_ux = new echolocator__ImageEditUx(
             self.runtime,
@@ -74,14 +80,21 @@
         // Tabs have created, which may need some tweaking inside the tab.
         this.#tabs_manager.addEventListener(
             echolocator__Events_TABS_CREATED_EVENT,
             function(event) {
                 that.handle_tabs_created(event);
             });
 
+        // User picks an plate from the plate list.
+        this.#plate_list_ux.addEventListener(
+            echolocator__Events_PLATE_PICKED_EVENT,
+            function(event) {
+                that.handle_plate_picked(event);
+            });
+
         // User picks an image from the image list.
         this.#image_list_ux.addEventListener(
             echolocator__Events_IMAGE_PICKED_EVENT,
             function(event) {
                 that.handle_image_picked(event);
             });
 
@@ -91,14 +104,15 @@
             function(event) {
                 that.handle_image_previous_or_next(event);
             });
 
         // -------------------------------------------------------------------
 
         this.#tabs_manager.activate()
+        this.#plate_list_ux.activate();
         this.#image_list_ux.activate();
         this.#image_edit_ux.activate();
 
         // Tab has been opened (made current).
         this.#tabs_manager.addEventListener(
             echolocator__Events_TAB_OPENED,
             function(event) {
@@ -143,31 +157,54 @@
 
         var $interaction_parent = $("#" + tab_id).children().first();
 
         var interaction_parent_id = $interaction_parent.attr("id");
 
         // console.log(F + ": $interaction_parent_id is \"" + interaction_parent_id + "\"");
 
-        if (interaction_parent_id == "image_list_ux_interaction_parent") {
+        if (interaction_parent_id == "plate_list_ux_interaction_parent") {
+            this.#plate_list_ux.request_update()
+        } else if (interaction_parent_id == "image_list_ux_interaction_parent") {
             this.#image_list_ux.request_update()
         } else if (interaction_parent_id == "image_edit_ux_interaction_parent") {
             this.#image_edit_ux.request_update()
         }
 
     } // end method
 
     // -----------------------------------------------------------------------
+    // Propagate event where user clicks a filename, such as in plate_list_ux.
+    handle_plate_picked(event) {
+        var F = "Index::handle_plate_picked";
+
+        // Get the visit and barcode provided by the plate row that was clicked.
+        var visit_filter = event.detail.visit;
+        var barcode_filter = event.detail.barcode;
+
+        console.log(F + ": [CWINDX] visit is \"" + visit_filter + "\", barcode is \"" + barcode_filter + "\"")
+
+        // Tell the image list to show the images from the new plate.
+        var should_show_only_undecided = true;
+        this.#image_list_ux.show_first_image(visit_filter, barcode_filter, should_show_only_undecided);
+
+        // this.#tabs_manager.switch_to_tab("tab-image-edit")
+
+    } // end method
+
+    // -----------------------------------------------------------------------
     // Propagate event where user clicks a filename, such as in image_list_ux.
     handle_image_picked(event) {
         var F = "Index::handle_image_picked";
 
-        var crystal_well_uuid = event.detail.crystal_well_uuid;
+        var crystal_well_index = event.detail.crystal_well_index;
+
+        console.log(F + ": [CWINDX] event.detail crystal_well_index is " + crystal_well_index)
 
         // Tell the image editor to show the new image.
-        this.#image_edit_ux.set_crystal_well_uuid(crystal_well_uuid);
+        this.#image_edit_ux.set_crystal_well_index(crystal_well_index);
 
         this.#tabs_manager.switch_to_tab("tab-image-edit")
 
         // Resize the displayed image according to the current screen size.
         // this.resize_image()
 
     } // end method
```

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/common/base.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/common/base.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,21 @@
 // Class backing the actions ux.
 
 class echolocator__ImageEditUx extends echolocator__UxAutoUpdate {
     COOKIE_NAME = "IMAGE_EDIT_UX";
     FETCH_IMAGE = "echolocator_guis::commands::fetch_image";
     UPDATE = "echolocator_guis::commands::update";
+    CRYSTAL_WELL_INDEX = "echolocator_guis::keywords::crystal_well_index";
+    CRYSTAL_WELL_INDEX_NEXT = "echolocator_guis::keywords::crystal_well_index_next";
+    CRYSTAL_WELL_COUNT = "echolocator_guis::keywords::crystal_well_count";
     SHOULD_ADVANCE = "echolocator_guis::keywords::should_advance";
 
     #jquery_objects = {};
-    #crystal_well_uuid = null;
+    #crystal_well_index = null;
+    #crystal_well_count = null;
     #record = null;
     #raphael = null;
     #is_dragging = null;
     #transformer = null;
     #confirmed_target_ux = null;
     #well_centroid_ux = null;
 
@@ -45,16 +49,20 @@
         // Pass this transformer to anyone who wants to use the raphael for drawing.
         this.#raphael.webviz_transformer = this.#transformer;
 
         this.#jquery_objects.$raphael1_paper = $("#raphael1_paper SVG", this.$interaction_parent);
         this.#jquery_objects.$image = $("IMG", this.$interaction_parent);
         this.#jquery_objects.$hide_when_no_image = $(".T_hide_when_no_image", this.$interaction_parent);
         this.#jquery_objects.$filename = $(".T_filename", this.$interaction_parent);
+        this.#jquery_objects.$crystal_well_index = $(".T_crystal_well_index", this.$interaction_parent);
+        this.#jquery_objects.$crystal_well_count = $(".T_crystal_well_count", this.$interaction_parent);
         this.#jquery_objects.$number_of_crystals = $(".T_number_of_crystals", this.$interaction_parent);
         this.#jquery_objects.$is_usable = $(".T_is_usable", this.$interaction_parent);
+        this.#jquery_objects.$is_exported_to_soakdb3 = $(".T_is_exported_to_soakdb3", this.$interaction_parent);
+
         this.#jquery_objects.previous_button = $(".T_previous_button", this.$interaction_parent);
         this.#jquery_objects.accept_button = $(".T_accept_button", this.$interaction_parent);
         this.#jquery_objects.reject_button = $(".T_reject_button", this.$interaction_parent);
         this.#jquery_objects.reset_button = $(".T_reset_button", this.$interaction_parent);
         this.#jquery_objects.next_button = $(".T_next_button", this.$interaction_parent);
 
         console.log(F + ": raphael1_paper is a " + this.selector_description(this.#jquery_objects.$raphael1_paper))
@@ -124,24 +132,27 @@
             function(jquery_event_object) {
                 console.log(F + ": clicked accept");
                 that._send_update(true);
             });
 
         this.#jquery_objects.reject_button.click(
             function(jquery_event_object) {
+                console.log(F + ": clicked reject");
                 that._send_update(false);
             });
 
         this.#jquery_objects.reset_button.click(
             function(jquery_event_object) {
+                console.log(F + ": clicked undecided");
                 that._send_update(null);
             });
 
         this.#jquery_objects.next_button.click(
             function(jquery_event_object) {
+                console.log(F + ": clicked next");
                 that._handle_previous_or_next(1);
             });
 
 
         // ----------------------------------------------------------
         // Make the draggable crosshair for the target location.
         this.#confirmed_target_ux = new echolocator__PixelUx(
@@ -180,56 +191,59 @@
         // Activate the spreader to react on window size changes.
         this.image1_spreader.activate($("#image1"), window);
 
         // Activate well_centroid first, so it lies "under" the confirmed target in case they overlap.
         this.#well_centroid_ux.activate(this.#raphael);
         this.#confirmed_target_ux.activate(this.#raphael);
 
-        this.request_update()
+        // this.request_update()
     } // end method
 
 
     // -------------------------------------------------------------
     // When the selected filename changes, we get notified.
     // We will load the image into the display.
 
-    set_crystal_well_uuid(crystal_well_uuid) {
-        var F = "echolocator__ImageEditUx::set_crystal_well_uuid";
+    set_crystal_well_index(crystal_well_index) {
+        var F = "echolocator__ImageEditUx::set_crystal_well_index";
+
+        console.log(F + ": [CWINDX] crystal_well_index is " + crystal_well_index)
 
         // Remember the image info.
-        this.#crystal_well_uuid = crystal_well_uuid;
+        this.#crystal_well_index = crystal_well_index;
 
-        if (this.#crystal_well_uuid === undefined) {
-            this.display_ajax_error("there are no more images to view");
-        } else {
-            this.display_ajax_error(null);
+        // if (this.#crystal_well_index === undefined) {
+        //     this.display_ajax_error("there are no more images to view");
+        // }
+        // else {
+        //     this.display_ajax_error(null);
 
-            // Request image info from the server.
-            this.request_update()
+        //     // Request image info from the server.
+        //     this.request_update()
 
-        }
+        // }
 
     } // end method
 
     // -------------------------------------------------------------
-    // Handle accept or reject button click.
+    // Send update to currently loaded image.
 
     _send_update(is_usable, confirmed_target) {
         var F = "echolocator__ImageEditUx::_handle_is_usable_change";
 
-        if (this.#crystal_well_uuid) {
+        if (this.#crystal_well_index !== null && this.#crystal_well_index !== undefined) {
             // Build json request.
             var json_object = {}
             // TODO: Remove hardcoded "IMAGE_LIST_UX" in image edit's cookie list.
             json_object[this.ENABLE_COOKIES] = [this.COOKIE_NAME, "IMAGE_LIST_UX"]
             json_object[this.COMMAND] = this.UPDATE;
 
             // We pass the fields of the database we want updated.
             var model = {
-                "crystal_well_uuid": this.#crystal_well_uuid,
+                "crystal_well_uuid": this.#record.uuid,
                 "is_usable": is_usable
             }
 
             if (confirmed_target !== undefined) {
                 model["confirmed_target_x"] = confirmed_target.x;
                 model["confirmed_target_y"] = confirmed_target.y;
             }
@@ -244,22 +258,21 @@
             }
 
             json_object["crystal_well_droplocation_model"] = model;
 
             // Tell server to add response["html"] for next image in series.
             json_object[this.SHOULD_ADVANCE] = true;
 
-            // Server needs to know the visit as its limiting window in the advancement logic.
-            json_object["visit"] = this.#record.visit;
+            if (this.#crystal_well_index < this.#crystal_well_count - 1) {
+                json_object[this.CRYSTAL_WELL_INDEX_NEXT] = this.#crystal_well_index + 1;
+                json_object[this.CRYSTAL_WELL_COUNT] = this.#crystal_well_count;
+            }
 
             // Send request to update database immediately.
             this.send(json_object);
-
-            // Move to next image.
-            this.request_update(1);
         }
 
     } // end method
 
     // -------------------------------------------------------------
     // Handle previous or next button click.
 
@@ -287,58 +300,85 @@
 
     // -------------------------------------------------------------
     // Handle left click on the raphael paper.
 
     _handle_canvas_left_click(jquery_event_object) {
         var F = "echolocator__ImageEditUx::_handle_canvas_left_click";
 
+        if (this.#record.is_exported_to_soakdb3) {
+            console.log(F + ": ignoring canvas left click because is_exported_to_soakdb3 is " + this.#record.is_exported_to_soakdb3);
+            return;
+        }
+
         console.log(F + ": seeing canvas left click");
 
         var view_position = {
             x: jquery_event_object.offsetX,
             y: jquery_event_object.offsetY
         }
 
         // Convert to target position before giving to pixel_ux.
         var confirmed_target = this.#transformer.view_to_data(view_position);
 
         // Notify pixel_ux of requested change in position.
-        this.#confirmed_target_ux.set_uuid(this.#crystal_well_uuid, confirmed_target);
+        this.#confirmed_target_ux.set_uuid(this.#crystal_well_index, confirmed_target);
 
         // Mark image usable and save target location.
         this._send_update(true, confirmed_target)
 
     } // end method
 
     // -------------------------------------------------------------
     // Handle right click on the raphael paper.
 
     _handle_canvas_right_click(jquery_event_object) {
         var F = "echolocator__ImageEditUx::_handle_canvas_right_click";
 
+        if (this.#record.is_exported_to_soakdb3)
+            return;
+
         // Mark image unusable.
         this._send_update(false)
 
     } // end method
 
     // -------------------------------------------------------------
     // Request update from database.
 
-    request_update(direction = 0) {
+    request_update(direction) {
+        var F = "echolocator__ImageEditUx::request_update";
+
+
+        if (direction === null || direction === undefined)
+            direction = 0;
+
+        var new_crystal_well_index = this.#crystal_well_index;
+        if (direction != 0) {
+            new_crystal_well_index += direction;
+
+            if (new_crystal_well_index >= this.#crystal_well_count)
+                new_crystal_well_index = null;
+
+            console.log(F + ": [CWINDX]" +
+                " this.#crystal_well_index is " + this.#crystal_well_index +
+                " moving to " + new_crystal_well_index +
+                " in crystal_well_count " + this.#crystal_well_count);
+        }
+
+        // if (new_crystal_well_index < 0 || new_crystal_well_index >= this.#crystal_well_count) {
+        //     return;
+        // }
+
 
         var json_object = {}
         // TODO: Remove hardcoded "IMAGE_LIST_UX" in image edit's cookie list.
         json_object[this.ENABLE_COOKIES] = [this.COOKIE_NAME, "IMAGE_LIST_UX"]
         json_object[this.COMMAND] = this.FETCH_IMAGE;
-        json_object["crystal_well_uuid"] = this.#crystal_well_uuid;
-
-        if (direction !== 0) {
-            json_object["direction"] = direction;
-            json_object["visit"] = this.#record.visit;
-        }
+        //json_object[this.SHOULD_ADVANCE] = true;
+        json_object[this.CRYSTAL_WELL_INDEX] = new_crystal_well_index;
 
         this.send(json_object);
 
     } // end method
 
     // -------------------------------------------------------------
     // Handle an error response.
@@ -377,40 +417,62 @@
             }
             this.#jquery_objects.$hide_when_no_image.hide();
             return;
         }
 
         this.#jquery_objects.$hide_when_no_image.show();
 
-        // Remember which crystal_well_uuid we are showing.
-        this.#crystal_well_uuid = record.uuid;
+        // Remember which set_crystal_well_index we are showing.
+        this.#crystal_well_index = response[this.CRYSTAL_WELL_INDEX];
+        this.#crystal_well_count = response[this.CRYSTAL_WELL_COUNT];
+
+        // Display the index (plus 1 to be less confusing to viewer) and length.
+        this.#jquery_objects.$crystal_well_index.text(this.#crystal_well_index + 1);
+        this.#jquery_objects.$crystal_well_count.text(this.#crystal_well_count);
+
+        this.#jquery_objects.previous_button.attr("disabled", this.#crystal_well_index == 0);
+        this.#jquery_objects.next_button.attr("disabled", this.#crystal_well_index >= this.#crystal_well_count - 1);
+
+        this.#jquery_objects.accept_button.attr("disabled", record.is_exported_to_soakdb3);
+        this.#jquery_objects.reject_button.attr("disabled", record.is_exported_to_soakdb3);
+        this.#jquery_objects.reset_button.attr("disabled", record.is_exported_to_soakdb3);
+
+        this.#confirmed_target_ux.enabled(!record.is_exported_to_soakdb3)
 
         // Update the display with the new file's contents.
         var src = record.filename;
         this.#jquery_objects.$image.prop("src", src)
 
-        // Render the crystal_well_uuid stuff.
+        // Render the set_crystal_well_index stuff.
         this.#jquery_objects.$filename.text(record.filename);
+
+        if (record.number_of_crystals === null)
+            record.number_of_crystals = "-";
+
         if (record.is_usable === null)
-            record.is_usable = "-";
+            record.is_usable = "undecided";
         if (record.is_usable === true)
             record.is_usable = "yes";
         if (record.is_usable === false)
             record.is_usable = "no";
 
-        if (record.number_of_crystals === null)
-            record.number_of_crystals = "-";
+        if (record.is_exported_to_soakdb3 === null)
+            this.#jquery_objects.$is_exported_to_soakdb3.text("no");
+        if (record.is_exported_to_soakdb3 === true)
+            this.#jquery_objects.$is_exported_to_soakdb3.text("yes");
+        if (record.is_exported_to_soakdb3 === false)
+            this.#jquery_objects.$is_exported_to_soakdb3.text("no");
 
         this.#jquery_objects.$number_of_crystals.text(record.number_of_crystals);
         this.#jquery_objects.$is_usable.text(record.is_usable);
 
         // Keep the last record loaded.
         this.#record = record;
 
-        // The the pixel ux about the crystal_well_uuid so it can be included in sending changes.
+        // The the pixel ux about the set_crystal_well_index so it can be included in sending changes.
         var x = record.confirmed_target_x;
         if (x === null)
             x = record.auto_target_x;
         if (x === null)
             x = 10;
 
         var y = record.confirmed_target_y;
@@ -420,17 +482,17 @@
             y = 10;
 
         var confirmed_target = {
             x: x,
             y: y
         };
 
-        this.#confirmed_target_ux.set_uuid(this.#crystal_well_uuid, confirmed_target);
+        this.#confirmed_target_ux.set_uuid(this.#crystal_well_index, confirmed_target);
 
-        // The the pixel ux about the crystal_well_uuid so it can be included in sending changes.
+        // The the pixel ux about the set_crystal_well_index so it can be included in sending changes.
         var x = record.well_centroid_x;
         if (x === null)
             x = 100;
 
         var y = record.well_centroid_y;
         if (y === null)
             y = 100;
@@ -470,15 +532,15 @@
 
     render() {
         var F = "echolocator__ImageEditUx::render";
 
         var w = $("#image1_viewport").width()
         var h = $("#image1_viewport").height()
 
-        console.log(F + " image1_viewport size is [" + w + ", " + h + "]");
+        // console.log(F + " image1_viewport size is [" + w + ", " + h + "]");
 
         // Resize the annotation overlay.
         $("#raphael1_viewport").width(w)
         $("#raphael1_viewport").height(h)
 
         // To transform coordinates.
         this.#transformer.set_view({
@@ -509,15 +571,15 @@
             return;
 
         var record = this.#record;
 
         var w = record.width;
         var h = record.height;
 
-        console.log(F + " image data size is [" + w + ", " + h + "]");
+        // console.log(F + " image data size is [" + w + ", " + h + "]");
 
         // To transform coordinates.
         this.#transformer.set_data({
             x1: 0,
             y1: 0,
             x2: w,
             y2: h
@@ -525,15 +587,15 @@
 
         // Transform data to view.
         var view_position = this.#transformer.data_to_view({
             x: w,
             y: h
         })
 
-        console.log(F + " data to view is [" + view_position.x + ", " + view_position.y + "]");
+        // console.log(F + " data to view is [" + view_position.x + ", " + view_position.y + "]");
 
         // TODO: Move detector1_image resize into image_edit_ux.
         var $img = $("#detector1_image")
         $img.prop("width", view_position.x)
         $img.prop("height", view_position.y)
 
     } // end method
```

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 // Class backing the actions ux.
 
 class echolocator__ImageListUx extends echolocator__UxAutoUpdate {
     COOKIE_NAME = "IMAGE_LIST_UX";
     FETCH_IMAGE_LIST = "echolocator_guis::commands::fetch_image_list";
-    EXPORT_TO_SOAKDB3 = "echolocator_guis::commands::export_to_soakdb3";
-    EXPORT_TO_CSV = "echolocator_guis::commands::export_to_csv";
+    CRYSTAL_WELL_INDEX = "echolocator_guis::keywords::crystal_well_index";
 
     #jquery_objects = {};
-    #visit_filter = "undefined";
-    #should_show_only_undecided = "undefined";
+    #visit_filter = null;
+    #barcode_filter = null;
+    #should_show_only_undecided = null;
 
     constructor(runtime, plugin_link_name, $interaction_parent) {
         super(runtime);
 
         this.plugin_link_name = plugin_link_name;
         this.$interaction_parent = $interaction_parent;
         this.filename_rows = undefined;
@@ -21,53 +21,78 @@
     // -------------------------------------------------------------
     // Activate things on the UX.
 
     activate() {
         super.activate()
 
         this.#jquery_objects.$div = $(".T_composed", this.$interaction_parent);
-        this.#jquery_objects.$visit_filter = $(".T_visit_filter", this.$interaction_parent);
+        this.#jquery_objects.$visit_filter = $("#visit_filter", this.$interaction_parent);
+        this.#jquery_objects.$barcode_filter = $("#barcode_filter", this.$interaction_parent);
         this.#jquery_objects.$should_show_only_undecided = $(".T_should_show_only_undecided", this.$interaction_parent);
-        this.#jquery_objects.$export_to_soakdb3_button = $(".T_export_to_soakdb3_button", this.$interaction_parent);
-        this.#jquery_objects.$export_to_csv_button = $(".T_export_to_csv_button", this.$interaction_parent);
 
         var that = this;
         this.#jquery_objects.$visit_filter.change(
             function(jquery_event_object) {
                 that._handle_filter_change(jquery_event_object);
             });
 
-        this.#jquery_objects.$should_show_only_undecided.change(
+        this.#jquery_objects.$barcode_filter.change(
             function(jquery_event_object) {
                 that._handle_filter_change(jquery_event_object);
             });
 
-        this.#jquery_objects.$export_to_soakdb3_button.click(
+        this.#jquery_objects.$should_show_only_undecided.change(
             function(jquery_event_object) {
-                that._handle_export_to_soakdb3_clicked(jquery_event_object);
+                that._handle_filter_change(jquery_event_object);
             });
 
-        this.#jquery_objects.$export_to_csv_button.click(
-            function(jquery_event_object) {
-                that._handle_export_to_csv_clicked(jquery_event_object);
-            });
+    } // end method
+
+    // -------------------------------------------------------------
+
+    show_list(visit_filter, barcode_filter, should_show_only_undecided) {
+        var F = "echolocator__ImageListUx::show_list"
+
+        this.#visit_filter = visit_filter;
+        this.#barcode_filter = barcode_filter;
+        this.#should_show_only_undecided = should_show_only_undecided;
+        this.request_update();
+
+    } // end method
+
+    // -------------------------------------------------------------
+
+    show_first_image(visit_filter, barcode_filter, should_show_only_undecided) {
+        var F = "echolocator__ImageListUx::show_first_image"
+
+        this.#visit_filter = visit_filter;
+        this.#barcode_filter = barcode_filter;
+        this.#should_show_only_undecided = should_show_only_undecided;
+        this.request_update(true);
 
     } // end method
 
     // -------------------------------------------------------------
     // Request update from database.
 
-    request_update() {
+    request_update(show_first_image) {
 
         var json_object = {}
         json_object[this.COMMAND] = this.FETCH_IMAGE_LIST;
         json_object[this.ENABLE_COOKIES] = [this.COOKIE_NAME];
 
-        json_object["visit_filter"] = this.#visit_filter;
-        json_object["should_show_only_undecided"] = this.#should_show_only_undecided;
+        // Don't post any value if none defined yet, this will allow them to come from cookie, if any.
+        if (this.#visit_filter !== undefined && this.#visit_filter !== null)
+            json_object["visit_filter"] = this.#visit_filter;
+        if (this.#barcode_filter !== undefined && this.#barcode_filter !== null)
+            json_object["barcode_filter"] = this.#barcode_filter;
+        if (this.#should_show_only_undecided !== undefined && this.#should_show_only_undecided !== null)
+            json_object["should_show_only_undecided"] = this.#should_show_only_undecided;
+        if (show_first_image !== undefined)
+            json_object["show_first_image"] = show_first_image;
 
         this.send(json_object);
 
     } // end method
 
     // -------------------------------------------------------------
     // Handle the response when it comes.
@@ -83,107 +108,92 @@
             var t;
 
             t = filters["visit_filter"];
             if (t === undefined)
                 t = "";
             this.#jquery_objects.$visit_filter.val(t);
 
+            t = filters["barcode_filter"];
+            if (t === undefined)
+                t = "";
+            this.#jquery_objects.$barcode_filter.val(t);
+
             t = filters["should_show_only_undecided"];
             if (t === undefined)
                 t = false;
             this.#jquery_objects.$should_show_only_undecided.prop("checked", t);
         }
 
         var html = response.html;
 
-        if (html !== undefined) {
+        if (html !== null && html !== undefined) {
             this.#jquery_objects.$div.html(html);
             // Attach events to all the individual job links in the "recent jobs" grid.
             this._attach_links();
         }
-    }
 
-    // -------------------------------------------------------------
+        // Response includes "first image"?
+        var crystal_well_index = response[this.CRYSTAL_WELL_INDEX];
 
-    _handle_filter_change(jquery_event_object) {
-        var F = "echolocator__ImageListUx::_handle_filter_change"
+        console.log(F + ": [CWINDX] response[" + this.CRYSTAL_WELL_INDEX + "] is " + crystal_well_index);
 
-        this.#visit_filter = this.#jquery_objects.$visit_filter.val()
-        this.#should_show_only_undecided = this.#jquery_objects.$should_show_only_undecided.prop("checked")
-        this.request_update()
-
-    } // end method
-
-    // -------------------------------------------------------------
-
-    _handle_export_to_soakdb3_clicked(jquery_event_object) {
-        var F = "echolocator__ImageListUx::_handle_export_to_soakdb3_clicked"
+        // Post this up to the page to switch tabs, similar to clicking on a row.
+        if (crystal_well_index !== null && crystal_well_index !== undefined) {
 
-        this.#visit_filter = this.#jquery_objects.$visit_filter.val()
-
-        // Enable no cookie for this request.
-        var json_object = {}
-        json_object[this.COMMAND] = this.EXPORT_TO_SOAKDB3;
-
-        json_object["visit_filter"] = this.#visit_filter;
-
-        this.send(json_object);
+            this._load_image(crystal_well_index);
 
-    } // end method
+            this.set_and_render_auto_update(false);
+        }
+    }
 
     // -------------------------------------------------------------
 
-    _handle_export_to_csv_clicked(jquery_event_object) {
-        var F = "echolocator__ImageListUx::_handle_export_to_csv_clicked"
+    _handle_filter_change(jquery_event_object) {
+        var F = "echolocator__ImageListUx::_handle_filter_change"
 
         this.#visit_filter = this.#jquery_objects.$visit_filter.val()
-
-        // Enable no cookie for this request.
-        var json_object = {}
-        json_object[this.COMMAND] = this.EXPORT_TO_CSV;
-
-        json_object["visit_filter"] = this.#visit_filter;
-
-        this.send(json_object);
+        this.#barcode_filter = this.#jquery_objects.$barcode_filter.val()
+        this.#should_show_only_undecided = this.#jquery_objects.$should_show_only_undecided.prop("checked")
+        this.request_update()
 
     } // end method
 
     // -------------------------------------------------------------
 
     _handle_filename_clicked(jquery_event_object) {
 
         var $filename_row = $(jquery_event_object.target);
 
         // User clicked on a cell within the row?
         if ($filename_row.get(0).tagName == "TD")
             $filename_row = $filename_row.parent();
 
         // The row has the attribute holding the crystal well of this row.
-        var crystal_well_uuid = $filename_row.attr("crystal_well_uuid");
+        var crystal_well_index = parseInt($filename_row.attr("crystal_well_index"));
 
-        this._load_image(crystal_well_uuid);
+        this._load_image(crystal_well_index);
 
         this.set_and_render_auto_update(false);
 
     } // end method
 
     // -------------------------------------------------------------
 
-    _load_image(crystal_well_uuid) {
+    _load_image(crystal_well_index) {
         var F = "echolocator__ImageListUx::_load_image";
 
-        console.log(F + ": loading image for crystal_well_uuid " + crystal_well_uuid)
+        console.log(F + ": [CWINDX] loading image for crystal_well_index " + crystal_well_index)
 
         //     this.$filename_rows.removeClass("T_picked");
         //     image_info.$filename_row.addClass("T_picked");
 
         // Trigger an event that the index.js will use to coordinate cross-widget changes.
         var custom_event = new CustomEvent(echolocator__Events_IMAGE_PICKED_EVENT, {
             detail: {
-                crystal_well_uuid: crystal_well_uuid
+                crystal_well_index: crystal_well_index
             }
         });
 
         this.dispatchEvent(custom_event);
 
     } // end method
```

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -63,14 +63,29 @@
     } // end method
 
     // -------------------------------------------------------------
     // When the selected image changes, we get notified.
     // We will move the guide to the image's target location.
     // We will update the x and y as the guid moves.
 
+    enabled(flag) {
+        var F = "echolocator__PixelUx[" + this.plugin_link_name + "]::enabled"
+
+        this.#is_draggable = flag;
+        this.#guide.set_box({
+            "enabled": flag
+        });
+
+    } // end method
+
+    // -------------------------------------------------------------
+    // When the selected image changes, we get notified.
+    // We will move the guide to the image's target location.
+    // We will update the x and y as the guid moves.
+
     set_uuid(uuid, target) {
         var F = "echolocator__PixelUx[" + this.plugin_link_name + "]::set_uuid"
 
         // Remember the image info.
         this.#uuid = uuid;
         this.#target = target;
```

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -11,15 +11,15 @@
         this.name = name;
         this.debug_identifier = name;
         this.precisionLine = precisionLine;
     } // end constructor
 
     // -------------------------------------------------------------
 
-    activate(raphael, color, is_draggable) {
+    activate(raphael, color, is_enabled) {
         var F = "webviz__hair__Guide2[" + this.name + "]::activate";
 
         this._raphael = raphael
 
         raphael.setStart();
 
         this._hline = this._raphael.path("M0,0:L1,0").attr({
@@ -58,29 +58,30 @@
 
         this._vline._group = this._group;
         this._vline._parent_object = this;
 
         this._ball._group = this._group;
         this._ball._parent_object = this;
 
-        if (is_draggable)
+        this.is_enabled = is_enabled;
+        if (is_enabled)
             this._group.drag(this._drag_move, this._drag_start, this._drag_stop);
 
         console.log(F + ": activated")
     } // end method
 
     // -------------------------------------------------------------
     set_box(settings) {
         var F = "webviz__hair__Guide2[" + this.name + "]::set_box";
 
         for (var k in settings) {
             var setting = settings[k];
 
             if (k == "position") {
-                console.log(F + ": setting position [" + setting.x + ", " + setting.y + "]")
+                // console.log(F + ": setting position [" + setting.x + ", " + setting.y + "]")
 
                 // Something wrong with settings?
                 if (!isNaN(setting.x) && !isNaN(setting.y)) {
                     this._group.transform("");
                     this._group.translate(setting.x, setting.y);
 
                     var hpath = "M" + 0 + "," + -10000 + ":L" + 0 + "," + 10000;
@@ -97,14 +98,18 @@
             // The setting is for visibility?
             else if (k == "visible") {
                 if (setting)
                     this._group.show();
                 else
                     this._group.hide();
             }
+            // The setting is for visibility?
+            else if (k == "enabled") {
+                this.is_enabled = setting;
+            }
 
         }
     } // end method
 
     // -------------------------------------------------------------
     // Returns the currents settings in a JSON-serializable structure.
 
@@ -123,26 +128,32 @@
         };
 
         return settings;
     } // end method
 
     // -------------------------------------------------------------
     _drag_move(dx, dy) {
+        if (!this._parent_object.is_enabled)
+            return;
+
         this._group.translate(dx - this.odx, dy - this.ody);
         this.odx = dx;
         this.ody = dy;
 
         this._parent_object._trigger_change_event(webviz__hair__Guide2__UserMotionEvent);
 
     } // end method
 
     // -------------------------------------------------------------
     _drag_start() {
         var F = "webviz__hair__Guide2[" + this._parent_object.name + "]::_drag_start";
 
+        if (!this._parent_object.is_enabled)
+            return;
+
         console.log(F + ": drag start")
 
         // var keys = new Array();
         // for (var k in this)
         // {
         //     keys.push(k);
         // }
@@ -153,14 +164,17 @@
         this.timeout = undefined;
     }
 
     // -------------------------------------------------------------
     _drag_stop() {
         var F = "webviz__hair__Guide2[" + this._parent_object.name + "]::_drag_stop";
 
+        if (!this._parent_object.is_enabled)
+            return;
+
         // Not yet started the timeout?
         if (this.timeout === undefined) {
             console.log(F + ": drag stop");
             var that = this;
             // Notify listeners in separate thread.
             this.timeout = setTimeout(function() {
                 that._parent_object._trigger_change_event(webviz__hair__Guide2__UserChangeEvent)
```

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/spreader.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/webviz/spreader.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -16,15 +16,15 @@
 
     activate(spreadable, container) {
         var F = "webviz__Spreader::activate";
 
         this.$spreadable = $(spreadable);
         this.$container = $(container);
 
-        console.log(F + " activating spreadable " + this.selector_description(this.$spreadable))
+        this.console_log(F + " activating spreadable " + this.selector_description(this.$spreadable))
 
         // Do the initial spread when activating.
         // this.spread();
 
         // Re-spread every time the container changes size, but not more often than 250ms.
         var that = this;
         this.$container.resize(function() {
@@ -35,48 +35,54 @@
         });
 
     } // end method
 
 
     // -------------------------------------------------------------
 
+    console_log(message) {
+        // console.log(message);
+    }
+
+    // -------------------------------------------------------------
+
     spread() {
         var F = "webviz__Spreader::spread";
 
-        console.log(F + " spreading " + this.selector_description(this.$spreadable) + " ------------------------ ")
+        this.console_log(F + " spreading " + this.selector_description(this.$spreadable) + " ------------------------ ")
 
         var container_outer_width = this.$container.outerWidth();
         var container_outer_height = this.$container.outerHeight();
-        console.log(F + " container outer size is " + container_outer_width + ", " + container_outer_height);
+        this.console_log(F + " container outer size is " + container_outer_width + ", " + container_outer_height);
 
         var container_inner_width = this.$container.innerWidth();
         var container_inner_height = this.$container.innerHeight();
-        console.log(F + " container inner size is " + container_inner_width + ", " + container_inner_height);
+        this.console_log(F + " container inner size is " + container_inner_width + ", " + container_inner_height);
 
         var spreadable_offset = this.$spreadable.offset();
         var spreadable_inner_width = this.$spreadable.innerWidth()
         var spreadable_inner_height = this.$spreadable.innerHeight()
         var spreadable_outer_width = this.$spreadable.outerWidth()
         var spreadable_outer_height = this.$spreadable.outerHeight()
 
-        console.log(F + " spreadable offset is " + spreadable_offset.left + ", " + spreadable_offset.top);
-        console.log(F + " spreadable inner size is " + spreadable_inner_width + ", " + spreadable_inner_height);
-        console.log(F + " spreadable outer size is " + spreadable_outer_width + ", " + spreadable_outer_height);
+        this.console_log(F + " spreadable offset is " + spreadable_offset.left + ", " + spreadable_offset.top);
+        this.console_log(F + " spreadable inner size is " + spreadable_inner_width + ", " + spreadable_inner_height);
+        this.console_log(F + " spreadable outer size is " + spreadable_outer_width + ", " + spreadable_outer_height);
 
         var spreadable_border_width = spreadable_outer_width - spreadable_inner_width;
         var spreadable_border_height = spreadable_outer_height - spreadable_inner_height;
 
         var remaining_w = container_outer_width - spreadable_offset.left
         var remaining_h = container_outer_height - spreadable_offset.top
 
         var padding = 8;
         this.$spreadable.innerWidth(remaining_w - spreadable_border_width - padding)
         this.$spreadable.innerHeight(remaining_h - spreadable_border_height - padding)
 
-        // console.log(F + " pulling triggger " + webviz__Spreader__SpreadEvent);
+        // this.console_log(F + " pulling triggger " + webviz__Spreader__SpreadEvent);
 
         // Trigger an event that the index.js will use to coordinate cross-widget changes.
         var custom_event = new CustomEvent(webviz__Spreader__SpreadEvent, {
             detail: undefined
         });
         this.dispatchEvent(custom_event);
```

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/ring.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/ring.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/guis/html/javascript/webviz/transformer.js` & `echolocator-1.3.0/src/echolocator_lib/guis/html/javascript/webviz/transformer.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/src/echolocator_lib/version.py` & `echolocator-1.3.0/src/echolocator_lib/version.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/tests/base.py` & `echolocator-1.3.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/tests/configurations/service.yaml` & `echolocator-1.3.0/tests/configurations/service.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 logging_settings:
     console:
         enabled: True
         verbose: True
         filters:
             markers:
+                - "[DISSHU]"
                 - "[RELCOOK]"
                 - "[COOKSEL]"
                 - "[COOKOFF]"
                 - "[GUITABS]"
                 - "[SETTINGVAL]"
     logfile:
         enabled: True
```

### Comparing `echolocator-1.2.0/tests/conftest.py` & `echolocator-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/tests/example_images/1.jpg` & `echolocator-1.3.0/tests/example_images/1.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/tests/example_images/2.jpg` & `echolocator-1.3.0/tests/example_images/2.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/tests/example_images/3.jpg` & `echolocator-1.3.0/tests/example_images/3.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/tests/example_images/4.png` & `echolocator-1.3.0/tests/example_images/4.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/tests/images/1.jpg` & `echolocator-1.3.0/tests/images/1.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/tests/images/2.jpg` & `echolocator-1.3.0/tests/images/2.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/tests/images/3.jpg` & `echolocator-1.3.0/tests/images/3.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/tests/test_droplocation.py` & `echolocator-1.3.0/tests/test_fetch_image.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import logging
 
+import pytest
+
 # API constants.
 from dls_servbase_api.constants import Keywords as ProtocoljKeywords
 from dls_servbase_lib.datafaces.context import Context as DlsServbaseDatafaceContext
 
 # Utilities.
-from dls_utilpack.describe import describe
+from dls_utilpack.exceptions import EndOfList, ProgrammingFault
 
 # Things xchembku provides.
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 from xchembku_api.datafaces.datafaces import xchembku_datafaces_get_default
-from xchembku_api.models.crystal_well_filter_model import CrystalWellFilterModel
 
 # Client context creator.
 from echolocator_api.guis.context import Context as GuiClientContext
 
 # GUI constants.
 from echolocator_lib.guis.constants import Commands, Cookies, Keywords
 
@@ -27,28 +28,28 @@
 # Base class for the tester.
 from tests.base import Base
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
-class TestDroplocation:
+class TestFetchImage:
     def test(self, constants, logging_setup, output_directory):
         """ """
 
         configuration_file = "tests/configurations/service.yaml"
-        DroplocationTester().main(
+        FetchImageTester().main(
             constants,
             configuration_file,
             output_directory,
         )
 
 
 # ----------------------------------------------------------------------------------------
-class DroplocationTester(Base):
+class FetchImageTester(Base):
     """
     Class to test the gui fetch_image endpoint.
     """
 
     async def _main_coroutine(self, constants, output_directory):
         """ """
 
@@ -83,136 +84,140 @@
         async with xchembku_client_context:
             # Start the dataface the gui uses for cookies.
             async with servbase_dataface_context:
                 # Start the gui client context.
                 async with gui_client_context:
                     # And the gui server context which starts the coro.
                     async with gui_server_context:
-                        await self.__run_part1(constants, output_directory)
-                        logger.debug(
-                            "[ECHDON] finished running __run_part1, so gui_server_context going out of scope"
-                        )
+                        await self.__run_the_test(constants, output_directory)
 
     # ----------------------------------------------------------------------------------------
 
-    async def __run_part1(self, constants, output_directory):
+    async def __run_the_test(self, constants, output_directory):
         """ """
         # Reference the xchembku object which the context has set up as the default.
         xchembku = xchembku_datafaces_get_default()
 
+        self.__cookies = {}
+
+        # Error when no index given in the request.
+        await self.__request_error_no_index()
+
+        # Query for a list, which will be zero length because there are no wells injected yet.
+        await self.__fetch_image_list()
+
+        # Error when requesting from empty list.
+        await self.__request_from_empty_list()
+
         crystal_wells = []
 
-        self.__cookies = {}
         # Inject some wells.
+        crystal_wells.append(await self.inject(xchembku, False, False))
+        crystal_wells.append(await self.inject(xchembku, True, True))
         crystal_wells.append(await self.inject(xchembku, True, False))
-        crystal_wells.append(await self.inject(xchembku, True, False))
+        crystal_wells.append(await self.inject(xchembku, True, True))
+        crystal_wells.append(await self.inject(xchembku, True, True))
         crystal_wells.append(await self.inject(xchembku, True, False))
 
-        # The crystal count increases with each one added, so they are sorted in reverse order of adding.
-        await self.__set_confirmed_target_and_advance(xchembku, crystal_wells, 2, 1)
-        await self.__set_confirmed_target_and_advance(xchembku, crystal_wells, 1, 0)
-        await self.__set_confirmed_target_and_advance(xchembku, crystal_wells, 0, None)
+        # Make a list which is no longer empty.
+        await self.__fetch_image_list()
 
-        await self.__set_is_usable_and_dont_advance(xchembku, crystal_wells, 0, False)
-        await self.__set_is_usable_and_dont_advance(xchembku, crystal_wells, 0, True)
+        await self.__request_anchor(crystal_wells)
 
     # ----------------------------------------------------------------------------------------
 
-    async def __set_confirmed_target_and_advance(
-        self, xchembku, crystal_well_models, index1, index2
-    ):
+    async def __fetch_image_list(self):
         """ """
 
-        x = 100 + index1
-        y = 200 + index1
         request = {
             ProtocoljKeywords.ENABLE_COOKIES: [
-                Cookies.IMAGE_EDIT_UX,
                 Cookies.IMAGE_LIST_UX,
             ],
-            Keywords.COMMAND: Commands.UPDATE,
-            Keywords.SHOULD_ADVANCE: True,
-            "visit": self.visit,
-            "crystal_well_droplocation_model": {
-                "crystal_well_uuid": crystal_well_models[index1].uuid,
-                "confirmed_target_x": x,
-                "confirmed_target_y": y,
-                "is_usable": True,
-            },
+            Keywords.COMMAND: Commands.FETCH_IMAGE_LIST,
+            "visit_filter": self.visit,
         }
 
         response = await echolocator_guis_get_default().client_protocolj(
             request, cookies=self.__cookies
         )
 
+        # Pick up the cookies established by the list query.
         self.__cookies = response["__cookies"]
 
-        note = f"advance from {index1} to {index2}"
-        logger.debug(describe(f"set_target response, {note}", response))
+    # ----------------------------------------------------------------------------------------
 
-        assert "record" in response, note
-        record = response["record"]
-        assert "confirmation" in response, note
-        assert "has been updated" in response["confirmation"], note
-        if index2 is not None:
-            assert record is not None, note
-            assert record["uuid"] == crystal_well_models[index2].uuid, note
-            assert "advanced" in response["confirmation"], note
-        else:
-            assert record is None, note
-            assert "no more images" in response["confirmation"], note
-
-        # Fetch the record which should have been updated.
-        fetched_models = await xchembku.fetch_crystal_wells_needing_droplocation(
-            CrystalWellFilterModel(anchor=crystal_well_models[index1].uuid)
-        )
-
-        assert fetched_models[0].confirmed_target_x == x, note
-        assert fetched_models[0].confirmed_target_y == y, note
-        assert fetched_models[0].is_usable is True, note
+    async def __request_error_no_index(self):
+        """ """
+
+        request = {
+            ProtocoljKeywords.ENABLE_COOKIES: [
+                Cookies.IMAGE_EDIT_UX,
+                Cookies.IMAGE_LIST_UX,
+            ],
+            Keywords.COMMAND: Commands.FETCH_IMAGE,
+        }
+
+        with pytest.raises(ProgrammingFault) as excinfo:
+            await echolocator_guis_get_default().client_protocolj(
+                request,
+                cookies=self.__cookies,
+            )
+
+        assert f"no value for {Keywords.CRYSTAL_WELL_INDEX}" in str(excinfo.value)
 
     # ----------------------------------------------------------------------------------------
 
-    async def __set_is_usable_and_dont_advance(
-        self,
-        xchembku,
-        crystal_well_models,
-        index1,
-        is_usable,
-    ):
+    async def __request_from_empty_list(self):
         """ """
 
-        # Build the request to change only the is_usable field.
         request = {
             ProtocoljKeywords.ENABLE_COOKIES: [
                 Cookies.IMAGE_EDIT_UX,
                 Cookies.IMAGE_LIST_UX,
             ],
-            Keywords.COMMAND: Commands.UPDATE,
-            Keywords.SHOULD_ADVANCE: False,
-            "crystal_well_droplocation_model": {
-                "crystal_well_uuid": crystal_well_models[index1].uuid,
-                "is_usable": is_usable,
-            },
+            Keywords.COMMAND: Commands.FETCH_IMAGE,
+            Keywords.CRYSTAL_WELL_INDEX: 1,
+        }
+
+        with pytest.raises(EndOfList):
+            await echolocator_guis_get_default().client_protocolj(
+                request,
+                cookies=self.__cookies,
+            )
+
+    # ----------------------------------------------------------------------------------------
+
+    async def __request_anchor(self, crystal_wells):
+        """ """
+
+        request = {
+            ProtocoljKeywords.ENABLE_COOKIES: [
+                Cookies.IMAGE_EDIT_UX,
+                Cookies.IMAGE_LIST_UX,
+            ],
+            Keywords.COMMAND: Commands.FETCH_IMAGE,
+            Keywords.CRYSTAL_WELL_INDEX: 2,  # 04A_1
         }
 
-        # Send the ajax request to the gui.
         response = await echolocator_guis_get_default().client_protocolj(
-            request, cookies=self.__cookies
+            request,
+            cookies=self.__cookies,
+        )
+
+        # Keep now we have both cookies.
+        self.__cookies = response["__cookies"]
+
+        record = response["record"]
+        assert record is not None
+        assert record["position"] == "04A_1"
+
+        # -------------------------------------------------------------------------------------
+        # Same query again, but rely on cookie for index.
+        request.pop(Keywords.CRYSTAL_WELL_INDEX)
+
+        response = await echolocator_guis_get_default().client_protocolj(
+            request,
+            cookies=self.__cookies,
         )
 
-        assert "record" not in response
-        assert "confirmation" in response
-        assert "has been updated" in response["confirmation"]
-
-        # Fetch the record which should have been updated.
-        fetched_models = await xchembku.fetch_crystal_wells_needing_droplocation(
-            CrystalWellFilterModel(anchor=crystal_well_models[index1].uuid)
-        )
-
-        # These should remain changed from when we set them previously in the test.
-        x = 100 + index1
-        y = 200 + index1
-
-        assert fetched_models[0].confirmed_target_x == x, f"index {index1}"
-        assert fetched_models[0].confirmed_target_y == y, f"index {index1}"
-        assert fetched_models[0].is_usable is is_usable, f"index {index1}"
+        record = response["record"]
+        assert record["position"] == "04A_1"
```

### Comparing `echolocator-1.2.0/tests/test_export_to_csv.py` & `echolocator-1.3.0/tests/test_export_to_csv.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.2.0/tests/test_export_to_soakdb3.py` & `echolocator-1.3.0/tests/test_export_to_soakdb3.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 from soakdb3_api.datafaces.context import Context as Soakdb3DatafaceClientContext
 from soakdb3_api.datafaces.datafaces import (
     datafaces_get_default as soakdb3_datafaces_get_default,
 )
 
 # The service process startup/teardown context.
 from soakdb3_lib.datafaces.context import Context as Soakdb3DatafaceServerContext
-
-# Things xchembku provides.
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 from xchembku_api.datafaces.datafaces import xchembku_datafaces_get_default
 
+# Things xchembku provides.
+from xchembku_api.models.crystal_well_filter_model import CrystalWellFilterModel
+
 # Client context creator.
 from echolocator_api.guis.context import Context as GuiClientContext
 
 # GUI constants.
 from echolocator_lib.guis.constants import Commands, Keywords
 
 # Server context creator.
@@ -111,19 +112,19 @@
                 async with xchembku_client_context:
                     # Start the dataface the gui uses for cookies.
                     async with servbase_dataface_context:
                         # Start the gui client context.
                         async with gui_client_context:
                             # And the gui server context which starts the coro.
                             async with gui_server_context:
-                                await self.__run_part1(constants, output_directory)
+                                await self.__run_the_test(constants, output_directory)
 
     # ----------------------------------------------------------------------------------------
 
-    async def __run_part1(self, constants, output_directory):
+    async def __run_the_test(self, constants, output_directory):
         """ """
 
         # Reference the soakdb3 dataface object which the context has set up as the default.
         soakdb3_dataface = soakdb3_datafaces_get_default()
 
         # Reference the xchembku object which the context has set up as the default.
         self.__xchembku = xchembku_datafaces_get_default()
@@ -206,7 +207,15 @@
         assert int(queried_models[0].EchoY) == -842
         assert queried_models[1].CrystalWell == "04A_1"
         assert int(queried_models[1].EchoX) == 6
         assert int(queried_models[1].EchoY) == -274
         assert queried_models[2].CrystalWell == "05A_1"
         assert int(queried_models[2].EchoX) == 289
         assert int(queried_models[2].EchoY) == 9
+
+        # Check the results stored in xchembku, the exported flag should be set.
+        crystal_well_models = (
+            await self.__xchembku.fetch_crystal_wells_needing_droplocation(
+                CrystalWellFilterModel(is_exported_to_soakdb3=True)
+            )
+        )
+        assert len(crystal_well_models) == 3
```

### Comparing `echolocator-1.2.0/tests/test_fetch_images.py` & `echolocator-1.3.0/tests/test_fetch_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,30 +155,29 @@
             "visit_filter": self.visit,
         }
 
         response = await echolocator_guis_get_default().client_protocolj(
             request, cookies={}
         )
 
-        logger.debug(describe("fetch_image response", response))
+        # logger.debug(describe("fetch_images cookies", response["__cookies"]))
 
         soup = BeautifulSoup(response["html"], "html.parser")
 
         # Find the table element.
         table = soup.find("table")
 
         # Count the number of rows in the table.
         rows = table.find_all("tr")
 
         # Assert that the row count is equal to the expected value.
         assert len(rows) == 1 + 5
 
         # Check the first row's filename.
-        # Remember fiels are injected with increasing crystal counts,
-        # so default sorting is in reverse order.
+        # Wells are injected with increasing crystal counts, so default sorting is in reverse order.
         row = rows[1]
         columns = row.find_all(class_="T_filename")
         assert len(columns) == 1
         assert columns[0].get_text() == Path(crystal_wells[5].filename).stem
 
         # Check the last row's filename.
         row = rows[5]
```

