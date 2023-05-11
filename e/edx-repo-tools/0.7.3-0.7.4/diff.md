# Comparing `tmp/edx-repo-tools-0.7.3.tar.gz` & `tmp/edx-repo-tools-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-repo-tools-0.7.3.tar", last modified: Fri Apr  7 10:02:59 2023, max compression
+gzip compressed data, was "edx-repo-tools-0.7.4.tar", last modified: Thu May 11 15:28:29 2023, max compression
```

## Comparing `edx-repo-tools-0.7.3.tar` & `edx-repo-tools-0.7.4.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.979294 edx-repo-tools-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      187 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-04-07 10:02:59.979294 edx-repo-tools-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.975294 edx-repo-tools-0.7.3/edx_repo_tools/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3022 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/add_common_constraint.py
--rw-r--r--   0 runner    (1001) docker     (122)     7051 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.975294 edx-repo-tools-0.7.3/edx_repo_tools/codemods/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.975294 edx-repo-tools-0.7.3/edx_repo_tools/codemods/django2/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/django2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/django2/auth_anonymous_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     1718 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/django2/foreignkey_on_delete_mod.py
--rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/django2/widget_add_renderer_mod.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.975294 edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3125 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/add_new_django32_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     2001 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/github_actions_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3830 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/github_actions_modernizer_django.py
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/remove_python2_unicode_compatible.py
--rw-r--r--   0 runner    (1001) docker     (122)     1372 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/replace_render_to_response.py
--rw-r--r--   0 runner    (1001) docker     (122)      500 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/replace_static.py
--rw-r--r--   0 runner    (1001) docker     (122)      814 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/replace_unicode_with_str.py
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/setup_file_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4132 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/tox_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4613 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/travis_modernizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.975294 edx-repo-tools-0.7.3/edx_repo_tools/codemods/node16/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/node16/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2913 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/node16/gha_ci_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/codemods/node16/gha_release_workflow_modernizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.975294 edx-repo-tools-0.7.3/edx_repo_tools/conventional_commits/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/conventional_commits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6830 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/conventional_commits/commitstats.py
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/dependabot_yml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.975294 edx-repo-tools-0.7.3/edx_repo_tools/dev/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/dev/clone_org.py
--rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/dev/get_org_repo_urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1167 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/dev/show_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.975294 edx-repo-tools-0.7.3/edx_repo_tools/find_dependencies/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/find_dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10833 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/find_dependencies/find_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.979294 edx-repo-tools-0.7.3/edx_repo_tools/gitgraft/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/gitgraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22365 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/gitgraft/gitgraft.py
--rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      977 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/modernize_openedx_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.979294 edx-repo-tools-0.7.3/edx_repo_tools/oep2/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/oep2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.979294 edx-repo-tools-0.7.3/edx_repo_tools/oep2/checks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/oep2/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/oep2/checks/check_explicit.py
--rw-r--r--   0 runner    (1001) docker     (122)     6240 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/oep2/checks/check_oep10.py
--rw-r--r--   0 runner    (1001) docker     (122)     1510 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/oep2/checks/check_oep2.py
--rw-r--r--   0 runner    (1001) docker     (122)      915 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/oep2/explode_repos_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.979294 edx-repo-tools-0.7.3/edx_repo_tools/oep2/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/oep2/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/oep2/report/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/oep2/report/oep2-report.ini
--rw-r--r--   0 runner    (1001) docker     (122)    10463 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/oep2/report/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.979294 edx-repo-tools-0.7.3/edx_repo_tools/ospr/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/ospr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/ospr/no_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.979294 edx-repo-tools-0.7.3/edx_repo_tools/release/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28778 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/release/tag_release.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.979294 edx-repo-tools-0.7.3/edx_repo_tools/repo_access_scraper/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/repo_access_scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6613 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/repo_access_scraper/repo_access_scraper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2479 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/edx_repo_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.975294 edx-repo-tools-0.7.3/edx_repo_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-04-07 10:02:59.000000 edx-repo-tools-0.7.3/edx_repo_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-04-07 10:02:59.000000 edx-repo-tools-0.7.3/edx_repo_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 10:02:59.000000 edx-repo-tools-0.7.3/edx_repo_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1782 2023-04-07 10:02:59.000000 edx-repo-tools-0.7.3/edx_repo_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-04-07 10:02:59.000000 edx-repo-tools-0.7.3/edx_repo_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-07 10:02:59.000000 edx-repo-tools-0.7.3/edx_repo_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.979294 edx-repo-tools-0.7.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-07 10:02:59.979294 edx-repo-tools-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4674 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:59.979294 edx-repo-tools-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/tests/test_actions_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/tests/test_actions_modernizer_django.py
--rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/tests/test_add_new_django32_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/tests/test_gha_release_workflow_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/tests/test_modernize_openedx_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)     2153 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/tests/test_node_ci_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/tests/test_remove_python2_unicode_compatible.py
--rw-r--r--   0 runner    (1001) docker     (122)     2073 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/tests/test_replace_render_to_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/tests/test_setup_file_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)    16510 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/tests/test_tag_release.py
--rw-r--r--   0 runner    (1001) docker     (122)     4131 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/tests/test_tox_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3517 2023-04-07 10:02:54.000000 edx-repo-tools-0.7.3/tests/test_travis_modernizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.454867 edx-repo-tools-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3131 2023-05-11 15:28:29.454867 edx-repo-tools-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.446867 edx-repo-tools-0.7.4/edx_repo_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3022 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/add_common_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7051 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.450867 edx-repo-tools-0.7.4/edx_repo_tools/codemods/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.450867 edx-repo-tools-0.7.4/edx_repo_tools/codemods/django2/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/django2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/django2/auth_anonymous_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1718 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/django2/foreignkey_on_delete_mod.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/django2/widget_add_renderer_mod.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.450867 edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3125 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/add_new_django32_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2001 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/github_actions_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3830 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/github_actions_modernizer_django.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/remove_python2_unicode_compatible.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1372 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/replace_render_to_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)      500 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/replace_static.py
+-rw-r--r--   0 runner    (1001) docker     (122)      814 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/replace_unicode_with_str.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/setup_file_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4132 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/tox_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4613 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/travis_modernizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.450867 edx-repo-tools-0.7.4/edx_repo_tools/codemods/node16/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/node16/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2913 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/node16/gha_ci_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/codemods/node16/gha_release_workflow_modernizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.450867 edx-repo-tools-0.7.4/edx_repo_tools/conventional_commits/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/conventional_commits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6830 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/conventional_commits/commitstats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/dependabot_yml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.450867 edx-repo-tools-0.7.4/edx_repo_tools/dev/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2390 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/dev/clone_org.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/dev/get_org_repo_urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1167 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/dev/show_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.450867 edx-repo-tools-0.7.4/edx_repo_tools/find_dependencies/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/find_dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10833 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/find_dependencies/find_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.450867 edx-repo-tools-0.7.4/edx_repo_tools/gitgraft/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/gitgraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22365 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/gitgraft/gitgraft.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      977 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/modernize_openedx_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.450867 edx-repo-tools-0.7.4/edx_repo_tools/oep2/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/oep2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.454867 edx-repo-tools-0.7.4/edx_repo_tools/oep2/checks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/oep2/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/oep2/checks/check_explicit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6240 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/oep2/checks/check_oep10.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1510 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/oep2/checks/check_oep2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/oep2/explode_repos_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.454867 edx-repo-tools-0.7.4/edx_repo_tools/oep2/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/oep2/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/oep2/report/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/oep2/report/oep2-report.ini
+-rw-r--r--   0 runner    (1001) docker     (122)    10463 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/oep2/report/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.454867 edx-repo-tools-0.7.4/edx_repo_tools/ospr/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/ospr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/ospr/no_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.454867 edx-repo-tools-0.7.4/edx_repo_tools/release/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28778 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/release/tag_release.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.454867 edx-repo-tools-0.7.4/edx_repo_tools/repo_access_scraper/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/repo_access_scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6613 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/repo_access_scraper/repo_access_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2479 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/edx_repo_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.450867 edx-repo-tools-0.7.4/edx_repo_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3131 2023-05-11 15:28:29.000000 edx-repo-tools-0.7.4/edx_repo_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-05-11 15:28:29.000000 edx-repo-tools-0.7.4/edx_repo_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 15:28:29.000000 edx-repo-tools-0.7.4/edx_repo_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-05-11 15:28:29.000000 edx-repo-tools-0.7.4/edx_repo_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-05-11 15:28:29.000000 edx-repo-tools-0.7.4/edx_repo_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-11 15:28:29.000000 edx-repo-tools-0.7.4/edx_repo_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.454867 edx-repo-tools-0.7.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 15:28:29.454867 edx-repo-tools-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4674 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:29.454867 edx-repo-tools-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/tests/test_actions_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/tests/test_actions_modernizer_django.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/tests/test_add_new_django32_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/tests/test_gha_release_workflow_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/tests/test_modernize_openedx_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2153 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/tests/test_node_ci_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/tests/test_remove_python2_unicode_compatible.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2073 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/tests/test_replace_render_to_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/tests/test_setup_file_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16510 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/tests/test_tag_release.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4131 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/tests/test_tox_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3517 2023-05-11 15:28:20.000000 edx-repo-tools-0.7.4/tests/test_travis_modernizer.py
```

### Comparing `edx-repo-tools-0.7.3/LICENSE.txt` & `edx-repo-tools-0.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/NOTICE.txt` & `edx-repo-tools-0.7.4/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/PKG-INFO` & `edx-repo-tools-0.7.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: edx-repo-tools
-Version: 0.7.3
+Version: 0.7.4
 Summary: This repo contains a number of tools Open edX uses for working with GitHub repositories.
 Home-page: https://github.com/openedx/repo-tools
 Author: edX
 Author-email: oscm@edx.org
 License: Apache
 Keywords: edx repo tools
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Provides-Extra: repo_access_scraper
 Provides-Extra: find_dependencies
+Provides-Extra: repo_access_scraper
 Provides-Extra: conventional_commits
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
 ###################
 Open edX Repo Tools
 ###################
@@ -94,9 +93,7 @@
 .. _older README.md: https://github.com/openedx/repo-tools/blob/7aa8bda466d1925c56d4ad6e3b2bdd87b1f83148/README.md
 
 
 Feedback
 ========
 
 Please send any feedback to oscm@edx.org.
-
-
```

### Comparing `edx-repo-tools-0.7.3/README.rst` & `edx-repo-tools-0.7.4/README.rst`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/add_common_constraint.py` & `edx-repo-tools-0.7.4/edx_repo_tools/add_common_constraint.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/auth.py` & `edx-repo-tools-0.7.4/edx_repo_tools/auth.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/codemods/django2/auth_anonymous_update.py` & `edx-repo-tools-0.7.4/edx_repo_tools/codemods/django2/auth_anonymous_update.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/codemods/django2/foreignkey_on_delete_mod.py` & `edx-repo-tools-0.7.4/edx_repo_tools/codemods/django2/foreignkey_on_delete_mod.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/codemods/django2/widget_add_renderer_mod.py` & `edx-repo-tools-0.7.4/edx_repo_tools/codemods/django2/widget_add_renderer_mod.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/add_new_django32_settings.py` & `edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/add_new_django32_settings.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/github_actions_modernizer.py` & `edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/github_actions_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/github_actions_modernizer_django.py` & `edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/github_actions_modernizer_django.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/remove_python2_unicode_compatible.py` & `edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/remove_python2_unicode_compatible.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/replace_render_to_response.py` & `edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/replace_render_to_response.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/replace_unicode_with_str.py` & `edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/replace_unicode_with_str.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/setup_file_modernizer.py` & `edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/setup_file_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/tox_modernizer.py` & `edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/tox_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/codemods/django3/travis_modernizer.py` & `edx-repo-tools-0.7.4/edx_repo_tools/codemods/django3/travis_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/codemods/node16/gha_ci_modernizer.py` & `edx-repo-tools-0.7.4/edx_repo_tools/codemods/node16/gha_ci_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/codemods/node16/gha_release_workflow_modernizer.py` & `edx-repo-tools-0.7.4/edx_repo_tools/codemods/node16/gha_release_workflow_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/conventional_commits/commitstats.py` & `edx-repo-tools-0.7.4/edx_repo_tools/conventional_commits/commitstats.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/data.py` & `edx-repo-tools-0.7.4/edx_repo_tools/data.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/dependabot_yml.py` & `edx-repo-tools-0.7.4/edx_repo_tools/dependabot_yml.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/dev/clone_org.py` & `edx-repo-tools-0.7.4/edx_repo_tools/dev/clone_org.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Clone an entire GitHub organization into current directory."""
 
+import fnmatch
 import os.path
 import shutil
 
 import click
 from git.repo.base import Repo
 
 from edx_repo_tools.auth import pass_github
@@ -27,22 +28,26 @@
     help="Should only forks be cloned?"
 )
 @click.option(
     '--depth', type=int, default=0,
     help="Depth argument for git clone",
 )
 @click.option(
+    '--ignore',
+    help="Glob pattern for repos to ignore",
+)
+@click.option(
     '--prune', is_flag=True, default=False,
     help="Remove repos that we wouldn't have cloned",
 )
 @click.argument(
     'org'
 )
 @pass_github
-def main(hub, archived, archived_only, forks, forks_only, depth, prune, org):
+def main(hub, archived, archived_only, forks, forks_only, depth, ignore, prune, org):
     """
     Clone an entire GitHub organization into the current directory.
     Each repo becomes a subdirectory.
     """
     if archived_only:
         archived = True
     if forks_only:
@@ -53,14 +58,17 @@
             continue
         if not repo.fork and forks_only:
             continue
         if repo.archived and not archived:
             continue
         if not repo.archived and archived_only:
             continue
+        if ignore and fnmatch.fnmatch(repo.name, ignore):
+            print(f"Ignoring {repo.full_name}")
+            continue
         dir_name = repo.name
         dir_name = dir_name.lstrip("-")     # avoid dirname/option confusion
         dir_names.add(dir_name)
         if os.path.exists(dir_name):
             continue
 
         print("Cloning {}".format(repo.full_name))
```

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/dev/get_org_repo_urls.py` & `edx-repo-tools-0.7.4/edx_repo_tools/dev/get_org_repo_urls.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/dev/show_hooks.py` & `edx-repo-tools-0.7.4/edx_repo_tools/dev/show_hooks.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/find_dependencies/find_dependencies.py` & `edx-repo-tools-0.7.4/edx_repo_tools/find_dependencies/find_dependencies.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/gitgraft/gitgraft.py` & `edx-repo-tools-0.7.4/edx_repo_tools/gitgraft/gitgraft.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/helpers.py` & `edx-repo-tools-0.7.4/edx_repo_tools/helpers.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/modernize_openedx_yaml.py` & `edx-repo-tools-0.7.4/edx_repo_tools/modernize_openedx_yaml.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/oep2/checks/check_explicit.py` & `edx-repo-tools-0.7.4/edx_repo_tools/oep2/checks/check_explicit.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/oep2/checks/check_oep10.py` & `edx-repo-tools-0.7.4/edx_repo_tools/oep2/checks/check_oep10.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/oep2/checks/check_oep2.py` & `edx-repo-tools-0.7.4/edx_repo_tools/oep2/checks/check_oep2.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/oep2/explode_repos_yaml.py` & `edx-repo-tools-0.7.4/edx_repo_tools/oep2/explode_repos_yaml.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/oep2/report/cli.py` & `edx-repo-tools-0.7.4/edx_repo_tools/oep2/report/cli.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/oep2/report/plugin.py` & `edx-repo-tools-0.7.4/edx_repo_tools/oep2/report/plugin.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/ospr/no_yaml.py` & `edx-repo-tools-0.7.4/edx_repo_tools/ospr/no_yaml.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/release/tag_release.py` & `edx-repo-tools-0.7.4/edx_repo_tools/release/tag_release.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/repo_access_scraper/repo_access_scraper.py` & `edx-repo-tools-0.7.4/edx_repo_tools/repo_access_scraper/repo_access_scraper.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools/utils.py` & `edx-repo-tools-0.7.4/edx_repo_tools/utils.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools.egg-info/PKG-INFO` & `edx-repo-tools-0.7.4/edx_repo_tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: edx-repo-tools
-Version: 0.7.3
+Version: 0.7.4
 Summary: This repo contains a number of tools Open edX uses for working with GitHub repositories.
 Home-page: https://github.com/openedx/repo-tools
 Author: edX
 Author-email: oscm@edx.org
 License: Apache
 Keywords: edx repo tools
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Provides-Extra: repo_access_scraper
 Provides-Extra: find_dependencies
+Provides-Extra: repo_access_scraper
 Provides-Extra: conventional_commits
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
 ###################
 Open edX Repo Tools
 ###################
@@ -94,9 +93,7 @@
 .. _older README.md: https://github.com/openedx/repo-tools/blob/7aa8bda466d1925c56d4ad6e3b2bdd87b1f83148/README.md
 
 
 Feedback
 ========
 
 Please send any feedback to oscm@edx.org.
-
-
```

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools.egg-info/SOURCES.txt` & `edx-repo-tools-0.7.4/edx_repo_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools.egg-info/entry_points.txt` & `edx-repo-tools-0.7.4/edx_repo_tools.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,7 @@
 remove_python2_unicode_compatible = edx_repo_tools.codemods.django3.remove_python2_unicode_compatible:main
 replace_render_to_response = edx_repo_tools.codemods.django3.replace_render_to_response:main
 replace_static = edx_repo_tools.codemods.django3.replace_static:main
 replace_unicode_with_str = edx_repo_tools.codemods.django3.replace_unicode_with_str:main
 repo_access_scraper = edx_repo_tools.repo_access_scraper.repo_access_scraper:main
 show_hooks = edx_repo_tools.dev.show_hooks:main
 tag_release = edx_repo_tools.release.tag_release:main
-
```

### Comparing `edx-repo-tools-0.7.3/edx_repo_tools.egg-info/requires.txt` & `edx-repo-tools-0.7.4/edx_repo_tools.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,128 +1,129 @@
-pluggy==1.0.0
-backports-csv==1.0.7
+tqdm==4.65.0
+numpy==1.24.3
+service-identity==21.1.0
+fissix==21.11.13
+iniconfig==2.0.0
+ruamel-yaml-clib==0.2.7
+oauthlib==3.2.2
+py==1.11.0
+path-py==12.5.0
+lxml==4.9.2
+itemloaders==1.1.0
+cryptography==40.0.2
+platformdirs==3.5.0
+scrapy==2.8.0
+volatile==2.1.0
 tomli==2.0.1
-msgpack==1.0.5
-requests-oauthlib==1.3.1
-appdirs==1.4.4
-jira==1.0.3
-pycparser==2.21
-certifi==2022.12.7
-distlib==0.3.6
-typing-extensions==4.5.0
 tox==3.28.0
-itemloaders==1.0.6
-protego==0.2.1
-urllib3==1.26.15
-smmap==5.0.0
-ruamel-yaml==0.17.21
-pyasn1-modules==0.2.8
-python-dotenv==1.0.0
+click==8.1.3
+certifi==2022.12.7
+automat==22.10.0
+zope-interface==6.0
 queuelib==1.6.2
-virtualenv==20.21.0
-gitdb==4.0.10
-py==1.11.0
-packaging==23.0
-pyjwt[crypto]==2.6.0
-ruamel-yaml-clib==0.2.7
-hyperlink==21.0.0
-twisted==22.10.0
-pytest==7.2.2
-path-py==12.5.0
-parsel==1.7.0
+filelock==3.12.0
 constantly==15.1.0
-pydispatcher==2.0.7
-itemadapter==0.7.0
-more-itertools==9.1.0
-oauthlib==3.2.2
-jmespath==1.0.1
-scrapy==2.8.0
-service-identity==21.1.0
-urlobject==2.4.3
-tlslite==0.4.9
-cachecontrol==0.12.11
-attrs==22.2.0
-tldextract==3.4.0
-lazy==1.5
-tqdm==4.65.0
+appdirs==1.4.4
 pytest-xdist==3.2.1
-pyasn1==0.4.8
+pyyaml==6.0
+github3-py==4.0.1
+urllib3==1.26.15
+requests-oauthlib==1.3.1
 uritemplate==4.1.1
-cffi==1.15.1
-iniconfig==2.0.0
-volatile==2.1.0
-bowler==0.9.0
-incremental==22.10.0
-path==16.6.0
-zope-interface==5.5.2
-pytest-logging==2015.11.4
+jira==1.0.3
 idna==3.4
-python-dateutil==2.8.2
-gitpython==3.1.31
-fissix==21.11.13
-w3lib==2.1.1
-statistics==1.0.3.5
-platformdirs==3.1.1
+packaging==23.1
+six==1.16.0
+jmespath==1.0.1
+exceptiongroup==1.1.1
+attrs==23.1.0
+docutils==0.19
+pyjwt[crypto]==2.6.0
+pytest==7.3.1
+tlslite==0.4.9
+protego==0.2.1
+more-itertools==9.1.0
+python-dotenv==1.0.0
+cffi==1.15.1
+parsel==1.8.1
 moreorless==0.4.0
+itemadapter==0.8.0
+urlobject==2.4.3
 cssselect==1.2.0
-pyyaml==6.0
-requests-toolbelt==0.10.1
-numpy==1.24.2
-docutils==0.19
-filelock==3.10.0
-requests==2.28.2
-requests-file==1.5.1
-github3-py==3.2.0
+ruamel-yaml==0.17.22
 lockfile==0.12.2
-charset-normalizer==3.1.0
-click==8.1.3
-automat==22.10.0
-pyopenssl==23.0.0
-cryptography==39.0.2
-exceptiongroup==1.1.1
+virtualenv==20.23.0
+python-dateutil==2.8.2
+requests-file==1.5.1
+bowler==0.9.0
+requests==2.29.0
+pluggy==1.0.0
+requests-toolbelt==1.0.0
 execnet==1.9.0
-six==1.16.0
-lxml==4.9.2
+pyopenssl==23.1.1
+hyperlink==21.0.0
+typing-extensions==4.5.0
+gitpython==3.1.31
+pytest-logging==2015.11.4
+path==16.6.0
+pyasn1-modules==0.3.0
+tldextract==3.4.1
+cachecontrol==0.12.11
+gitdb==4.0.10
+smmap==5.0.0
+pycparser==2.21
+incremental==22.10.0
+msgpack==1.0.5
+twisted==22.10.0
+lazy==1.5
+charset-normalizer==3.1.0
+distlib==0.3.6
+pydispatcher==2.0.7
+backports-csv==1.0.7
+pyasn1==0.5.0
+w3lib==2.1.1
+statistics==1.0.3.5
 
 [conventional_commits]
-pillow==9.4.0
-packaging==23.0
-fonttools==4.39.0
-kiwisolver==1.4.4
-matplotlib==3.7.1
-cycler==0.11.0
+packaging==23.1
+typing-extensions==4.5.0
 mako==1.2.4
-pytz==2022.7.1
 contourpy==1.0.7
-importlib-metadata==6.0.0
-alembic==1.10.2
+numpy==1.24.3
+six==1.16.0
+matplotlib==3.7.1
+pytz==2023.3
+alembic==1.10.4
+zipp==3.15.0
+fonttools==4.39.3
+cycler==0.11.0
+dataset==1.6.0
+banal==1.0.6
+tzdata==2023.3
+pillow==9.5.0
 importlib-resources==5.12.0
+kiwisolver==1.4.4
+sqlalchemy==1.4.48
 python-dateutil==2.8.2
-typing-extensions==4.5.0
-sqlalchemy==1.4.46
-banal==1.0.6
-markupsafe==2.1.2
-dataset==1.6.0
-zipp==3.15.0
 greenlet==2.0.2
-pandas==1.5.3
+importlib-metadata==6.6.0
 pyparsing==3.0.9
-six==1.16.0
-numpy==1.24.2
+pandas==2.0.1
+markupsafe==2.1.2
 
 [find_dependencies]
-requests==2.28.2
-markdown-it-py==2.2.0
-certifi==2022.12.7
-urllib3==1.26.15
 mdurl==0.1.2
 idna==3.4
-rich==13.3.2
+urllib3==1.26.15
 typing-extensions==4.5.0
-pygments==2.14.0
+rich==13.3.5
+requests==2.29.0
 charset-normalizer==3.1.0
+certifi==2022.12.7
+pygments==2.15.1
+markdown-it-py==2.2.0
 
 [repo_access_scraper]
 pyee==9.0.4
-typing-extensions==4.5.0
+playwright==1.33.0
 greenlet==2.0.1
-playwright==1.31.1
+typing-extensions==4.5.0
```

### Comparing `edx-repo-tools-0.7.3/setup.py` & `edx-repo-tools-0.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/tests/test_actions_modernizer.py` & `edx-repo-tools-0.7.4/tests/test_actions_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/tests/test_actions_modernizer_django.py` & `edx-repo-tools-0.7.4/tests/test_actions_modernizer_django.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/tests/test_add_new_django32_settings.py` & `edx-repo-tools-0.7.4/tests/test_add_new_django32_settings.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/tests/test_gha_release_workflow_modernizer.py` & `edx-repo-tools-0.7.4/tests/test_gha_release_workflow_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/tests/test_modernize_openedx_yaml.py` & `edx-repo-tools-0.7.4/tests/test_modernize_openedx_yaml.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/tests/test_node_ci_modernizer.py` & `edx-repo-tools-0.7.4/tests/test_node_ci_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/tests/test_remove_python2_unicode_compatible.py` & `edx-repo-tools-0.7.4/tests/test_remove_python2_unicode_compatible.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/tests/test_replace_render_to_response.py` & `edx-repo-tools-0.7.4/tests/test_replace_render_to_response.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/tests/test_setup_file_modernizer.py` & `edx-repo-tools-0.7.4/tests/test_setup_file_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/tests/test_tag_release.py` & `edx-repo-tools-0.7.4/tests/test_tag_release.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/tests/test_tox_modernizer.py` & `edx-repo-tools-0.7.4/tests/test_tox_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.3/tests/test_travis_modernizer.py` & `edx-repo-tools-0.7.4/tests/test_travis_modernizer.py`

 * *Files identical despite different names*

