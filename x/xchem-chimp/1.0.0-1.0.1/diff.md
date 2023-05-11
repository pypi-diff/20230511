# Comparing `tmp/xchem-chimp-1.0.0.tar.gz` & `tmp/xchem-chimp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchem-chimp-1.0.0.tar", last modified: Sun Apr  9 04:05:28 2023, max compression
+gzip compressed data, was "xchem-chimp-1.0.1.tar", last modified: Fri May  5 11:32:38 2023, max compression
```

## Comparing `xchem-chimp-1.0.0.tar` & `xchem-chimp-1.0.1.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.657743 xchem-chimp-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.645742 xchem-chimp-1.0.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.645742 xchem-chimp-1.0.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.645742 xchem-chimp-1.0.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.645742 xchem-chimp-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.641741 xchem-chimp-1.0.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.645742 xchem-chimp-1.0.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.645742 xchem-chimp-1.0.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.645742 xchem-chimp-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.645742 xchem-chimp-1.0.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-04-09 04:05:28.653742 xchem-chimp-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.645742 xchem-chimp-1.0.0/config/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/config/echolocator_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/detect_folder_chimp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/detect_list_file_chimp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/detect_list_file_to_ispyb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.649742 xchem-chimp-1.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.641741 xchem-chimp-1.0.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.649742 xchem-chimp-1.0.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.649742 xchem-chimp-1.0.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.649742 xchem-chimp-1.0.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.649742 xchem-chimp-1.0.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/docs/user/explanations/25-docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/docs/user/explanations/51-todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.649742 xchem-chimp-1.0.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.649742 xchem-chimp-1.0.0/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.649742 xchem-chimp-1.0.0/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.649742 xchem-chimp-1.0.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 04:05:28.657743 xchem-chimp-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.641741 xchem-chimp-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.649742 xchem-chimp-1.0.0/src/xchem_chimp/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/src/xchem_chimp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/src/xchem_chimp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 04:05:28.000000 xchem-chimp-1.0.0/src/xchem_chimp/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.649742 xchem-chimp-1.0.0/src/xchem_chimp/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/src/xchem_chimp/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/src/xchem_chimp/base/chimp_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/src/xchem_chimp/base/chimp_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/src/xchem_chimp/base/chimp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.649742 xchem-chimp-1.0.0/src/xchem_chimp/detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/src/xchem_chimp/detector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.653742 xchem-chimp-1.0.0/src/xchem_chimp/detector/background_images/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/src/xchem_chimp/detector/background_images/d1_background.png
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/src/xchem_chimp/detector/background_images/d2_background.png
--rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/src/xchem_chimp/detector/background_images/d3_background.png
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/src/xchem_chimp/detector/chimp_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    14293 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/src/xchem_chimp/detector/coord_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/src/xchem_chimp/detector/detector_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/src/xchem_chimp/detector/detector_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/src/xchem_chimp/detector/detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/src/xchem_chimp/detector/mask_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/src/xchem_chimp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.649742 xchem-chimp-1.0.0/src/xchem_chimp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-04-09 04:05:28.000000 xchem-chimp-1.0.0/src/xchem_chimp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-09 04:05:28.000000 xchem-chimp-1.0.0/src/xchem_chimp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 04:05:28.000000 xchem-chimp-1.0.0/src/xchem_chimp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-09 04:05:28.000000 xchem-chimp-1.0.0/src/xchem_chimp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-09 04:05:28.000000 xchem-chimp-1.0.0/src/xchem_chimp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 04:05:28.000000 xchem-chimp-1.0.0/src/xchem_chimp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.653742 xchem-chimp-1.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.641741 xchem-chimp-1.0.0/tests/SubwellImages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.653742 xchem-chimp-1.0.0/tests/SubwellImages/97wo_2021-09-14_RI1000-0276-3drop/
--rw-r--r--   0 runner    (1001) docker     (123)   156218 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/tests/SubwellImages/97wo_2021-09-14_RI1000-0276-3drop/97wo_01A_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.653742 xchem-chimp-1.0.0/tests/echo_test_imgs/
--rw-r--r--   0 runner    (1001) docker     (123)   146361 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/tests/echo_test_imgs/echo_test_im_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   142418 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/tests/echo_test_imgs/echo_test_im_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/tests/test_chimp_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/tests/test_chimp_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/tests/test_chimp_detector_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/tests/test_chimp_detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/tests/test_coord_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.653742 xchem-chimp-1.0.0/tests/test_imgs/
--rw-r--r--   0 runner    (1001) docker     (123)   485068 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/tests/test_imgs/big_crystals_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   402247 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/tests/test_imgs/small_crystals_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/tests/test_mask_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/xchem_conda_minimal.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.645742 xchem-chimp-1.0.0/zocalo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.653742 xchem-chimp-1.0.0/zocalo/recipes/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/zocalo/recipes/run_vmxi_processing.json
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/zocalo/recipes/run_vmxi_processing_test.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:05:28.653742 xchem-chimp-1.0.0/zocalo/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/zocalo/scripts/run_CHiMP_classify.sh
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/zocalo/scripts/run_CHiMP_classify_test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/zocalo/scripts/run_CHiMP_detect.sh
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/zocalo/scripts/run_CHiMP_detect_test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/zocalo/scripts/run_formulatrix_EF.sh
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/zocalo/scripts/run_formulatrix_EF_test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/zocalo/scripts/run_formulatrix_Z.sh
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-09 04:05:20.000000 xchem-chimp-1.0.0/zocalo/scripts/run_formulatrix_Z_test.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.105874 xchem-chimp-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.097874 xchem-chimp-1.0.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.097874 xchem-chimp-1.0.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.097874 xchem-chimp-1.0.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.097874 xchem-chimp-1.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.093874 xchem-chimp-1.0.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.097874 xchem-chimp-1.0.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.097874 xchem-chimp-1.0.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.097874 xchem-chimp-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.097874 xchem-chimp-1.0.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17364 2023-05-05 11:32:38.105874 xchem-chimp-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.097874 xchem-chimp-1.0.1/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/config/echolocator_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/detect_folder_chimp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/detect_list_file_chimp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/detect_list_file_to_ispyb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.097874 xchem-chimp-1.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.093874 xchem-chimp-1.0.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.097874 xchem-chimp-1.0.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.097874 xchem-chimp-1.0.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.097874 xchem-chimp-1.0.1/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.097874 xchem-chimp-1.0.1/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/docs/user/explanations/25-docs-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/docs/user/explanations/51-todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.101874 xchem-chimp-1.0.1/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.101874 xchem-chimp-1.0.1/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.101874 xchem-chimp-1.0.1/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.101874 xchem-chimp-1.0.1/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:32:38.105874 xchem-chimp-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.093874 xchem-chimp-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.101874 xchem-chimp-1.0.1/src/xchem_chimp/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/src/xchem_chimp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/src/xchem_chimp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 11:32:37.000000 xchem-chimp-1.0.1/src/xchem_chimp/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.101874 xchem-chimp-1.0.1/src/xchem_chimp/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/src/xchem_chimp/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/src/xchem_chimp/base/chimp_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/src/xchem_chimp/base/chimp_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/src/xchem_chimp/base/chimp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.101874 xchem-chimp-1.0.1/src/xchem_chimp/detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/src/xchem_chimp/detector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.101874 xchem-chimp-1.0.1/src/xchem_chimp/detector/background_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/src/xchem_chimp/detector/background_images/d1_background.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/src/xchem_chimp/detector/background_images/d2_background.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/src/xchem_chimp/detector/background_images/d3_background.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/src/xchem_chimp/detector/chimp_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/src/xchem_chimp/detector/coord_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/src/xchem_chimp/detector/detector_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/src/xchem_chimp/detector/detector_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/src/xchem_chimp/detector/detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/src/xchem_chimp/detector/mask_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/src/xchem_chimp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.101874 xchem-chimp-1.0.1/src/xchem_chimp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17364 2023-05-05 11:32:38.000000 xchem-chimp-1.0.1/src/xchem_chimp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-05 11:32:38.000000 xchem-chimp-1.0.1/src/xchem_chimp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:32:38.000000 xchem-chimp-1.0.1/src/xchem_chimp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-05 11:32:38.000000 xchem-chimp-1.0.1/src/xchem_chimp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-05 11:32:38.000000 xchem-chimp-1.0.1/src/xchem_chimp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 11:32:38.000000 xchem-chimp-1.0.1/src/xchem_chimp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.105874 xchem-chimp-1.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.093874 xchem-chimp-1.0.1/tests/SubwellImages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.105874 xchem-chimp-1.0.1/tests/SubwellImages/97wo_2021-09-14_RI1000-0276-3drop/
+-rw-r--r--   0 runner    (1001) docker     (123)   156218 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/tests/SubwellImages/97wo_2021-09-14_RI1000-0276-3drop/97wo_01A_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.105874 xchem-chimp-1.0.1/tests/echo_test_imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)   146361 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/tests/echo_test_imgs/echo_test_im_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   142418 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/tests/echo_test_imgs/echo_test_im_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/tests/test_chimp_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/tests/test_chimp_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/tests/test_chimp_detector_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/tests/test_chimp_detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/tests/test_coord_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.105874 xchem-chimp-1.0.1/tests/test_imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)   485068 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/tests/test_imgs/big_crystals_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   402247 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/tests/test_imgs/small_crystals_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/tests/test_mask_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/xchem_conda_minimal.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.093874 xchem-chimp-1.0.1/zocalo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.105874 xchem-chimp-1.0.1/zocalo/recipes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/zocalo/recipes/run_vmxi_processing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/zocalo/recipes/run_vmxi_processing_test.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:32:38.105874 xchem-chimp-1.0.1/zocalo/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/zocalo/scripts/run_CHiMP_classify.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/zocalo/scripts/run_CHiMP_classify_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/zocalo/scripts/run_CHiMP_detect.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/zocalo/scripts/run_CHiMP_detect_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/zocalo/scripts/run_formulatrix_EF.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/zocalo/scripts/run_formulatrix_EF_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/zocalo/scripts/run_formulatrix_Z.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 11:32:29.000000 xchem-chimp-1.0.1/zocalo/scripts/run_formulatrix_Z_test.sh
```

### Comparing `xchem-chimp-1.0.0/.dae-devops/Makefile` & `xchem-chimp-1.0.1/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.dae-devops/docs/conventions.rst` & `xchem-chimp-1.0.1/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.dae-devops/docs/developing.rst` & `xchem-chimp-1.0.1/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.dae-devops/docs/devops.rst` & `xchem-chimp-1.0.1/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.dae-devops/docs/docs_structure.rst` & `xchem-chimp-1.0.1/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.dae-devops/docs/installing.rst` & `xchem-chimp-1.0.1/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.dae-devops/docs/testing.rst` & `xchem-chimp-1.0.1/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.dae-devops/project.yaml` & `xchem-chimp-1.0.1/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.devcontainer/Dockerfile` & `xchem-chimp-1.0.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.devcontainer/devcontainer.json` & `xchem-chimp-1.0.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.github/CONTRIBUTING.rst` & `xchem-chimp-1.0.1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.github/actions/install_requirements/action.yml` & `xchem-chimp-1.0.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.github/dependabot.yml` & `xchem-chimp-1.0.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.github/pages/make_switcher.py` & `xchem-chimp-1.0.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.github/workflows/code.yml` & `xchem-chimp-1.0.1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.github/workflows/docs.yml` & `xchem-chimp-1.0.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.github/workflows/docs_clean.yml` & `xchem-chimp-1.0.1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.github/workflows/linkcheck.yml` & `xchem-chimp-1.0.1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.gitignore` & `xchem-chimp-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.gitlab-ci.yml` & `xchem-chimp-1.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/.vscode/launch.json` & `xchem-chimp-1.0.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/LICENSE` & `xchem-chimp-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/PKG-INFO` & `xchem-chimp-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchem-chimp
-Version: 1.0.0
+Version: 1.0.1
 Summary: XChem CHIMP
 Author-email: Olly King <olly.king@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -232,20 +232,29 @@
 ::
 
     pip install chimpflow
 
     chimpflow --version
 
 
-Model dataset
+Model file for xchem-chimp
 -----------------------------------------------------------------------
-::
 
-    wget https://zenodo.org/record/7810708/files/2022-12-07_CHiMP_Mask_R_CNN_XChem_50eph_VMXi_finetune_DICT_NZ.pytorch?download=1
+The model file is saved in::
+
+    https://gitlab.diamond.ac.uk/xchem/xchem-chimp-models
+
+
+This file is too large for github.
+
+For GitHub pytest to find the file in its CI/CD Actions, this file has been uploaded to zenodo::
+
+    https://zenodo.org/record/7810708/2022-12-07_CHiMP_Mask_R_CNN_XChem_50eph_VMXi_finetune_DICT_NZ.pytorch
 
+The tests/conftest.py fetches this file automatically.
 
 Running
 -----------------------------------------------------------------------
 ::
 
     rm -rf detector_output
     python -m detect_folder_chimp \
```

### Comparing `xchem-chimp-1.0.0/README.rst` & `xchem-chimp-1.0.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,29 @@
 ::
 
     pip install chimpflow
 
     chimpflow --version
 
 
-Model dataset
+Model file for xchem-chimp
 -----------------------------------------------------------------------
-::
 
-    wget https://zenodo.org/record/7810708/files/2022-12-07_CHiMP_Mask_R_CNN_XChem_50eph_VMXi_finetune_DICT_NZ.pytorch?download=1
+The model file is saved in::
+
+    https://gitlab.diamond.ac.uk/xchem/xchem-chimp-models
+
+
+This file is too large for github.
+
+For GitHub pytest to find the file in its CI/CD Actions, this file has been uploaded to zenodo::
+
+    https://zenodo.org/record/7810708/2022-12-07_CHiMP_Mask_R_CNN_XChem_50eph_VMXi_finetune_DICT_NZ.pytorch
 
+The tests/conftest.py fetches this file automatically.
 
 Running
 -----------------------------------------------------------------------
 ::
 
     rm -rf detector_output
     python -m detect_folder_chimp \
```

### Comparing `xchem-chimp-1.0.0/detect_folder_chimp.py` & `xchem-chimp-1.0.1/detect_folder_chimp.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/detect_list_file_chimp.py` & `xchem-chimp-1.0.1/detect_list_file_chimp.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/detect_list_file_to_ispyb.py` & `xchem-chimp-1.0.1/detect_list_file_to_ispyb.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/docs/conf.py` & `xchem-chimp-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/docs/images/dls-favicon.ico` & `xchem-chimp-1.0.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/docs/images/dls-logo.svg` & `xchem-chimp-1.0.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/docs/index.rst` & `xchem-chimp-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/docs/user/explanations/25-docs-structure.rst` & `xchem-chimp-1.0.1/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/docs/user/index.rst` & `xchem-chimp-1.0.1/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/pyproject.toml` & `xchem-chimp-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/src/xchem_chimp/__main__.py` & `xchem-chimp-1.0.1/src/xchem_chimp/__main__.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/src/xchem_chimp/base/chimp_base.py` & `xchem-chimp-1.0.1/src/xchem_chimp/base/chimp_base.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/src/xchem_chimp/base/chimp_utils.py` & `xchem-chimp-1.0.1/src/xchem_chimp/base/chimp_utils.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/src/xchem_chimp/detector/background_images/d1_background.png` & `xchem-chimp-1.0.1/src/xchem_chimp/detector/background_images/d1_background.png`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/src/xchem_chimp/detector/background_images/d2_background.png` & `xchem-chimp-1.0.1/src/xchem_chimp/detector/background_images/d2_background.png`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/src/xchem_chimp/detector/background_images/d3_background.png` & `xchem-chimp-1.0.1/src/xchem_chimp/detector/background_images/d3_background.png`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/src/xchem_chimp/detector/chimp_detector.py` & `xchem-chimp-1.0.1/src/xchem_chimp/detector/chimp_detector.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/src/xchem_chimp/detector/coord_generator.py` & `xchem-chimp-1.0.1/src/xchem_chimp/detector/coord_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,37 +129,46 @@
                 fig_out_path = output_dir / f"{img_path.stem}_preview.png"
                 logging.debug(f"Saving figure out to {fig_out_path}")
                 plt.axis("off")
                 plt.savefig(fig_out_path, bbox_inches="tight")
                 plt.close()
 
     def calculate_well_centres(self) -> None:
-        logging.debug("Calculating well centroids...")
-        # Load in background images
-        logging.debug("Loading background images")
+        # Load in background images.
+        # TODO: Make static background images for other plate types besides swiss3.
         bg_image_pths = sorted(list(BG_IMAGE_DIR.glob("*.png")))
         bg_image_arrays = [img_as_float(skio.imread(pth)) for pth in bg_image_pths]
         for output_dict in self.combined_coords_list:
             im_path = output_dict["image_path"]
-            logging.debug(f"{im_path}")
             im_array = self.read_and_resize_image(im_path)
             if "_1.jpg" in im_path:
                 bg_image = bg_image_arrays[0]
             elif "_2.jpg" in im_path:
                 bg_image = bg_image_arrays[1]
             elif "_3.jpg" in im_path:
                 bg_image = bg_image_arrays[2]
             else:
-                logging.error("Could not parse filename.")
+                raise RuntimeError(
+                    f'image filename "{im_path}" does not end with _1, _2 or _3'
+                )
             corr = signal.correlate2d(im_array, bg_image, mode="same", boundary="fill")
             y, x = np.unravel_index(np.argmax(corr), corr.shape)
             y, x = np.rint(np.array([y, x]) * (1.0 / IM_SCALE_FACTOR)).astype(int)
-            logging.debug(f"Well centroid found at {y, x}")
+            # Apply a fixed fudge offset to compensate for some unknown systematic problem in the well centroid detection.
+            # TODO: Fix problem where well centroid calculation apparently is shifted from the true value.
+            # UPDATE crystal_well_autolocations SET well_centroid_x = well_centroid_x + 30, well_centroid_y = well_centroid_y - 10
+            fudge_x = 30
+            fudge_y = -10
+            x += fudge_x
+            y += fudge_y
+            logging.debug(
+                f"Well centroid found at {x, y} after applying fudge offset {fudge_x, fudge_y}"
+            )
             output_dict["well_centroid"] = [y, x]
-            # Calculate realspace offset and add to dictionary
+            # Calculate realspace offset and add to dictionary.
             if output_dict["echo_coordinate"]:
                 output_dict["real_space_offset"] = utils.calculate_realspace_offset(
                     output_dict["echo_coordinate"][0],
                     np.array([y, x]),
                     np.array([MICRONS_PER_PIXEL_Y, MICRONS_PER_PIXEL_X]),
                 )
```

### Comparing `xchem-chimp-1.0.0/src/xchem_chimp/detector/detector_dataset.py` & `xchem-chimp-1.0.1/src/xchem_chimp/detector/detector_dataset.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/src/xchem_chimp/detector/detector_utils.py` & `xchem-chimp-1.0.1/src/xchem_chimp/detector/detector_utils.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/src/xchem_chimp/detector/mask_saver.py` & `xchem-chimp-1.0.1/src/xchem_chimp/detector/mask_saver.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/src/xchem_chimp/version.py` & `xchem-chimp-1.0.1/src/xchem_chimp/version.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/src/xchem_chimp.egg-info/PKG-INFO` & `xchem-chimp-1.0.1/src/xchem_chimp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchem-chimp
-Version: 1.0.0
+Version: 1.0.1
 Summary: XChem CHIMP
 Author-email: Olly King <olly.king@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -232,20 +232,29 @@
 ::
 
     pip install chimpflow
 
     chimpflow --version
 
 
-Model dataset
+Model file for xchem-chimp
 -----------------------------------------------------------------------
-::
 
-    wget https://zenodo.org/record/7810708/files/2022-12-07_CHiMP_Mask_R_CNN_XChem_50eph_VMXi_finetune_DICT_NZ.pytorch?download=1
+The model file is saved in::
+
+    https://gitlab.diamond.ac.uk/xchem/xchem-chimp-models
+
+
+This file is too large for github.
+
+For GitHub pytest to find the file in its CI/CD Actions, this file has been uploaded to zenodo::
+
+    https://zenodo.org/record/7810708/2022-12-07_CHiMP_Mask_R_CNN_XChem_50eph_VMXi_finetune_DICT_NZ.pytorch
 
+The tests/conftest.py fetches this file automatically.
 
 Running
 -----------------------------------------------------------------------
 ::
 
     rm -rf detector_output
     python -m detect_folder_chimp \
```

### Comparing `xchem-chimp-1.0.0/src/xchem_chimp.egg-info/SOURCES.txt` & `xchem-chimp-1.0.1/src/xchem_chimp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/tests/SubwellImages/97wo_2021-09-14_RI1000-0276-3drop/97wo_01A_1.jpg` & `xchem-chimp-1.0.1/tests/SubwellImages/97wo_2021-09-14_RI1000-0276-3drop/97wo_01A_1.jpg`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/tests/conftest.py` & `xchem-chimp-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/tests/echo_test_imgs/echo_test_im_1.jpg` & `xchem-chimp-1.0.1/tests/echo_test_imgs/echo_test_im_1.jpg`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/tests/echo_test_imgs/echo_test_im_3.jpg` & `xchem-chimp-1.0.1/tests/echo_test_imgs/echo_test_im_3.jpg`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/tests/test_chimp_base.py` & `xchem-chimp-1.0.1/tests/test_chimp_base.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/tests/test_chimp_detector.py` & `xchem-chimp-1.0.1/tests/test_chimp_detector.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/tests/test_chimp_detector_dataset.py` & `xchem-chimp-1.0.1/tests/test_chimp_detector_dataset.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/tests/test_chimp_detector_utils.py` & `xchem-chimp-1.0.1/tests/test_chimp_detector_utils.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/tests/test_coord_generator.py` & `xchem-chimp-1.0.1/tests/test_coord_generator.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/tests/test_imgs/big_crystals_3.jpg` & `xchem-chimp-1.0.1/tests/test_imgs/big_crystals_3.jpg`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/tests/test_imgs/small_crystals_2.jpg` & `xchem-chimp-1.0.1/tests/test_imgs/small_crystals_2.jpg`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/tests/test_mask_saver.py` & `xchem-chimp-1.0.1/tests/test_mask_saver.py`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/zocalo/recipes/run_vmxi_processing.json` & `xchem-chimp-1.0.1/zocalo/recipes/run_vmxi_processing.json`

 * *Files identical despite different names*

### Comparing `xchem-chimp-1.0.0/zocalo/recipes/run_vmxi_processing_test.json` & `xchem-chimp-1.0.1/zocalo/recipes/run_vmxi_processing_test.json`

 * *Files identical despite different names*

