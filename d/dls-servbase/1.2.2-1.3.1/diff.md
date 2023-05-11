# Comparing `tmp/dls-servbase-1.2.2.tar.gz` & `tmp/dls-servbase-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-servbase-1.2.2.tar", last modified: Wed May 10 05:54:22 2023, max compression
+gzip compressed data, was "dls-servbase-1.3.1.tar", last modified: Thu May 11 05:14:00 2023, max compression
```

## Comparing `dls-servbase-1.2.2.tar` & `dls-servbase-1.3.1.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.668508 dls-servbase-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.656508 dls-servbase-1.2.2/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.660508 dls-servbase-1.2.2/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.660508 dls-servbase-1.2.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.660508 dls-servbase-1.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.652508 dls-servbase-1.2.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.660508 dls-servbase-1.2.2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.660508 dls-servbase-1.2.2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.660508 dls-servbase-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.660508 dls-servbase-1.2.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-10 05:54:22.668508 dls-servbase-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.660508 dls-servbase-1.2.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.656508 dls-servbase-1.2.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.660508 dls-servbase-1.2.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.660508 dls-servbase-1.2.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/docs/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/docs/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.660508 dls-servbase-1.2.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/good_config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 05:54:22.668508 dls-servbase-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.656508 dls-servbase-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.660508 dls-servbase-1.2.2/src/dls_servbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-10 05:54:22.000000 dls-servbase-1.2.2/src/dls_servbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-10 05:54:22.000000 dls-servbase-1.2.2/src/dls_servbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 05:54:22.000000 dls-servbase-1.2.2/src/dls_servbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 05:54:22.000000 dls-servbase-1.2.2/src/dls_servbase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-10 05:54:22.000000 dls-servbase-1.2.2/src/dls_servbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 05:54:22.000000 dls-servbase-1.2.2/src/dls_servbase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.664508 dls-servbase-1.2.2/src/dls_servbase_api/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12480 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_api/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.664508 dls-servbase-1.2.2/src/dls_servbase_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_api/databases/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.664508 dls-servbase-1.2.2/src/dls_servbase_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.664508 dls-servbase-1.2.2/src/dls_servbase_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.664508 dls-servbase-1.2.2/src/dls_servbase_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_cli/subcommands/start_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.664508 dls-servbase-1.2.2/src/dls_servbase_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 05:54:22.000000 dls-servbase-1.2.2/src/dls_servbase_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    29692 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.664508 dls-servbase-1.2.2/src/dls_servbase_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/contexts/classic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/contexts/contexts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.664508 dls-servbase-1.2.2/src/dls_servbase_lib/cookies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/cookies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/cookies/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/cookies/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/cookies/dataface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.668508 dls-servbase-1.2.2/src/dls_servbase_lib/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/databases/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/databases/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.668508 dls-servbase-1.2.2/src/dls_servbase_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/datafaces/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.668508 dls-servbase-1.2.2/src/dls_servbase_lib/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.668508 dls-servbase-1.2.2/src/dls_servbase_lib/guis/html/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/guis/html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.668508 dls-servbase-1.2.2/src/dls_servbase_lib/guis/html/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/guis/html/javascript/version.js
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/src/dls_servbase_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.668508 dls-servbase-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/tests/base_context_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/tests/base_specification_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/tests/base_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:54:22.668508 dls-servbase-1.2.2/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/tests/configurations/servbase.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/tests/test_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/tests/test_dataface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/tests/test_dataface_takeover.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-05-10 05:54:11.000000 dls-servbase-1.2.2/tests/test_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.647594 dls-servbase-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.635593 dls-servbase-1.3.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.639593 dls-servbase-1.3.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.639593 dls-servbase-1.3.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.639593 dls-servbase-1.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.635593 dls-servbase-1.3.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.639593 dls-servbase-1.3.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.639593 dls-servbase-1.3.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.639593 dls-servbase-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.639593 dls-servbase-1.3.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-11 05:14:00.647594 dls-servbase-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.639593 dls-servbase-1.3.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.635593 dls-servbase-1.3.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.639593 dls-servbase-1.3.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.639593 dls-servbase-1.3.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/docs/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/docs/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.639593 dls-servbase-1.3.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/good_config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 05:14:00.647594 dls-servbase-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.635593 dls-servbase-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.643594 dls-servbase-1.3.1/src/dls_servbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-11 05:14:00.000000 dls-servbase-1.3.1/src/dls_servbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-11 05:14:00.000000 dls-servbase-1.3.1/src/dls_servbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 05:14:00.000000 dls-servbase-1.3.1/src/dls_servbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-11 05:14:00.000000 dls-servbase-1.3.1/src/dls_servbase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-11 05:14:00.000000 dls-servbase-1.3.1/src/dls_servbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 05:14:00.000000 dls-servbase-1.3.1/src/dls_servbase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.643594 dls-servbase-1.3.1/src/dls_servbase_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_api/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.643594 dls-servbase-1.3.1/src/dls_servbase_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_api/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_api/databases/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.643594 dls-servbase-1.3.1/src/dls_servbase_api/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_api/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_api/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_api/datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_api/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_api/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.643594 dls-servbase-1.3.1/src/dls_servbase_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.643594 dls-servbase-1.3.1/src/dls_servbase_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_cli/subcommands/start_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.643594 dls-servbase-1.3.1/src/dls_servbase_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 05:14:00.000000 dls-servbase-1.3.1/src/dls_servbase_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29692 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.643594 dls-servbase-1.3.1/src/dls_servbase_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/contexts/classic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/contexts/contexts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.643594 dls-servbase-1.3.1/src/dls_servbase_lib/cookies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/cookies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/cookies/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/cookies/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/cookies/dataface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.647594 dls-servbase-1.3.1/src/dls_servbase_lib/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/databases/aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/databases/database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/databases/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/databases/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.647594 dls-servbase-1.3.1/src/dls_servbase_lib/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/datafaces/aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.647594 dls-servbase-1.3.1/src/dls_servbase_lib/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.647594 dls-servbase-1.3.1/src/dls_servbase_lib/guis/html/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/guis/html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.647594 dls-servbase-1.3.1/src/dls_servbase_lib/guis/html/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/guis/html/javascript/version.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/src/dls_servbase_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.647594 dls-servbase-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/tests/base_context_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/tests/base_specification_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/tests/base_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:14:00.647594 dls-servbase-1.3.1/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/tests/configurations/servbase.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/tests/test_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/tests/test_dataface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/tests/test_dataface_takeover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-05-11 05:13:50.000000 dls-servbase-1.3.1/tests/test_gui.py
```

### Comparing `dls-servbase-1.2.2/.dae-devops/Makefile` & `dls-servbase-1.3.1/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.dae-devops/docs/conventions.rst` & `dls-servbase-1.3.1/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.dae-devops/docs/developing.rst` & `dls-servbase-1.3.1/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.dae-devops/docs/devops.rst` & `dls-servbase-1.3.1/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.dae-devops/docs/docs_structure.rst` & `dls-servbase-1.3.1/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.dae-devops/docs/installing.rst` & `dls-servbase-1.3.1/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.dae-devops/docs/testing.rst` & `dls-servbase-1.3.1/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.dae-devops/project.yaml` & `dls-servbase-1.3.1/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.devcontainer/Dockerfile` & `dls-servbase-1.3.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.devcontainer/devcontainer.json` & `dls-servbase-1.3.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.github/CONTRIBUTING.rst` & `dls-servbase-1.3.1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.github/actions/install_requirements/action.yml` & `dls-servbase-1.3.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.github/dependabot.yml` & `dls-servbase-1.3.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.github/pages/make_switcher.py` & `dls-servbase-1.3.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.github/workflows/code.yml` & `dls-servbase-1.3.1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.github/workflows/docs.yml` & `dls-servbase-1.3.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.github/workflows/docs_clean.yml` & `dls-servbase-1.3.1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.github/workflows/linkcheck.yml` & `dls-servbase-1.3.1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.gitignore` & `dls-servbase-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.gitlab-ci.yml` & `dls-servbase-1.3.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/.vscode/launch.json` & `dls-servbase-1.3.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/LICENSE` & `dls-servbase-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/PKG-INFO` & `dls-servbase-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-servbase
-Version: 1.2.2
+Version: 1.3.1
 Summary: Simple HTTP service for database operations.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-servbase-1.2.2/README.rst` & `dls-servbase-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/docs/conf.py` & `dls-servbase-1.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/docs/images/dls-favicon.ico` & `dls-servbase-1.3.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/docs/images/dls-logo.svg` & `dls-servbase-1.3.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/pyproject.toml` & `dls-servbase-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase.egg-info/PKG-INFO` & `dls-servbase-1.3.1/src/dls_servbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-servbase
-Version: 1.2.2
+Version: 1.3.1
 Summary: Simple HTTP service for database operations.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-servbase-1.2.2/src/dls_servbase.egg-info/SOURCES.txt` & `dls-servbase-1.3.1/src/dls_servbase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_api/aiohttp_client.py` & `dls-servbase-1.3.1/src/dls_servbase_api/aiohttp_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import aiohttp
 
 # Utilities.
 from dls_utilpack.callsign import callsign
 from dls_utilpack.describe import describe
 from dls_utilpack.explain import explain, explain2
+from dls_utilpack.import_class import import_classname_from_modulename
 
 # Exceptions.
 from dls_servbase_api.exceptions import (
     ClientConnectorError as DlsServbaseClientConnectorError,
 )
 
 logger = logging.getLogger(__name__)
@@ -124,16 +125,23 @@
                         response_dict = json.loads(text)
 
                         if "exception" in response_dict:
                             qualname = response_dict["exception"].get("qualname")
                             exception_message = response_dict["exception"].get(
                                 "message", "no message"
                             )
-                            exception_class = RuntimeError
-                            exception_message = f"{qualname}: {exception_message}"
+                            try:
+                                modulename = ".".join(qualname.split(".")[:-1])
+                                classname = qualname.split(".")[-1]
+                                exception_class = import_classname_from_modulename(
+                                    classname, modulename
+                                )
+                            except Exception:
+                                exception_class = RuntimeError
+                                exception_message = f"{qualname}: {exception_message}"
                     except Exception:
                         pass
 
                     raise exception_class(exception_message)
         except aiohttp.ClientConnectorError as exception:
             raise DlsServbaseClientConnectorError(
                 explain(exception, f"connecting to {callsign(self)}")
```

### Comparing `dls-servbase-1.2.2/src/dls_servbase_api/datafaces/aiohttp.py` & `dls-servbase-1.3.1/src/dls_servbase_api/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_api/datafaces/context.py` & `dls-servbase-1.3.1/src/dls_servbase_api/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_api/datafaces/datafaces.py` & `dls-servbase-1.3.1/src/dls_servbase_api/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_cli/main.py` & `dls-servbase-1.3.1/src/dls_servbase_cli/main.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_cli/subcommands/base.py` & `dls-servbase-1.3.1/src/dls_servbase_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_cli/subcommands/start_services.py` & `dls-servbase-1.3.1/src/dls_servbase_cli/subcommands/start_services.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_cli/version.py` & `dls-servbase-1.3.1/src/dls_servbase_cli/version.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/__main__.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/base_aiohttp.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/base_aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/contexts/base.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/contexts/classic.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/contexts/classic.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/contexts/contexts.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/contexts/contexts.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/cookies/base.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/cookies/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/cookies/cookies.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/cookies/cookies.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/cookies/dataface.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/cookies/dataface.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/databases/aiosqlite.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/databases/aiosqlite.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/databases/database_definition.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/databases/database_definition.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/databases/databases.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/databases/databases.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/databases/table_definitions.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/databases/table_definitions.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/datafaces/aiohttp.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/datafaces/aiosqlite.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/datafaces/aiosqlite.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/datafaces/context.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/datafaces/datafaces.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/envvar.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/guis/aiohttp.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/guis/context.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/guis/context.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/guis/guis.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/guis/guis.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/src/dls_servbase_lib/version.py` & `dls-servbase-1.3.1/src/dls_servbase_lib/version.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/tests/base.py` & `dls-servbase-1.3.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/tests/base_context_tester.py` & `dls-servbase-1.3.1/tests/base_context_tester.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/tests/base_specification_tester.py` & `dls-servbase-1.3.1/tests/base_specification_tester.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/tests/base_tester.py` & `dls-servbase-1.3.1/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/tests/configurations/servbase.yaml` & `dls-servbase-1.3.1/tests/configurations/servbase.yaml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/tests/conftest.py` & `dls-servbase-1.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/tests/test_aiohttp.py` & `dls-servbase-1.3.1/tests/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/tests/test_database.py` & `dls-servbase-1.3.1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/tests/test_dataface.py` & `dls-servbase-1.3.1/tests/test_dataface.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/tests/test_dataface_takeover.py` & `dls-servbase-1.3.1/tests/test_dataface_takeover.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.2.2/tests/test_gui.py` & `dls-servbase-1.3.1/tests/test_gui.py`

 * *Files identical despite different names*

