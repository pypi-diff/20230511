# Comparing `tmp/cookie_composer-0.9.1.tar.gz` & `tmp/cookie_composer-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookie_composer-0.9.1.tar", last modified: Wed Feb  8 13:07:11 2023, max compression
+gzip compressed data, was "cookie_composer-0.9.2.tar", last modified: Mon Feb 13 14:54:47 2023, max compression
```

## Comparing `cookie_composer-0.9.1.tar` & `cookie_composer-0.9.2.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 13:07:11.837652 cookie_composer-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-02-08 13:07:11.837652 cookie_composer-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 13:07:11.817650 cookie_composer-0.9.1/cookie_composer/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/cc_overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 13:07:11.821651 cookie_composer-0.9.1/cookie_composer/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/commands/authn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/commands/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/data_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/git_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 13:07:11.821651 cookie_composer-0.9.1/cookie_composer/merge_files/
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/merge_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/merge_files/ini_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/merge_files/json_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/merge_files/toml_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/merge_files/yaml_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/cookie_composer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 13:07:11.817650 cookie_composer-0.9.1/cookie_composer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-02-08 13:07:11.000000 cookie_composer-0.9.1/cookie_composer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-02-08 13:07:11.000000 cookie_composer-0.9.1/cookie_composer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 13:07:11.000000 cookie_composer-0.9.1/cookie_composer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-08 13:07:11.000000 cookie_composer-0.9.1/cookie_composer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 13:07:11.000000 cookie_composer-0.9.1/cookie_composer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-02-08 13:07:11.000000 cookie_composer-0.9.1/cookie_composer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-08 13:07:11.000000 cookie_composer-0.9.1/cookie_composer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 13:07:11.825651 cookie_composer-0.9.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/requirements/prod.in
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/requirements/prod.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-02-08 13:07:11.841652 cookie_composer-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 13:07:11.829651 cookie_composer-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 13:07:11.833652 cookie_composer-0.9.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/empty.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/existing.ini
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/existing.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/existing.toml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/existing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/gibberish.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/multi-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/new.ini
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/new.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/new.toml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/new.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 13:07:11.833652 cookie_composer-0.9.1/tests/fixtures/rendered1/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/rendered1/context.json
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/rendered1/rendered-composition.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 13:07:11.833652 cookie_composer-0.9.1/tests/fixtures/rendered1/testproject/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/rendered1/testproject/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/rendered1/testproject/dontmerge.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/rendered1/testproject/merge.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/rendered1/testproject/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 13:07:11.833652 cookie_composer-0.9.1/tests/fixtures/rendered2/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/rendered2/context.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 13:07:11.833652 cookie_composer-0.9.1/tests/fixtures/rendered2/testproject/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/rendered2/testproject/ABOUT.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/rendered2/testproject/dontmerge.json
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/rendered2/testproject/merge.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/rendered2/testproject/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/rendered_composition.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/single-template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 13:07:11.833652 cookie_composer-0.9.1/tests/fixtures/template1/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/template1/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 13:07:11.837652 cookie_composer-0.9.1/tests/fixtures/template1/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/template1/{{cookiecutter.repo_name}}/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/template1/{{cookiecutter.repo_name}}/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 13:07:11.837652 cookie_composer-0.9.1/tests/fixtures/template2/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/template2/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 13:07:11.837652 cookie_composer-0.9.1/tests/fixtures/template2/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/template2/{{cookiecutter.repo_name}}/ABOUT.md
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/fixtures/template2/{{cookiecutter.repo_name}}/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/test_cc_overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 13:07:11.837652 cookie_composer-0.9.1/tests/test_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/test_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/test_commands/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/test_commands/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/test_commands/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/test_commands/test_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/test_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/test_git_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/test_merge_files_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/test_merge_files_ini_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/test_merge_files_json_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/test_merge_files_toml_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/test_merge_files_yaml_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-02-08 13:06:50.000000 cookie_composer-0.9.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:47.317570 cookie_composer-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18005 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-02-13 14:54:47.317570 cookie_composer-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:47.305570 cookie_composer-0.9.2/cookie_composer/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/cc_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:47.309569 cookie_composer-0.9.2/cookie_composer/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/commands/authn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/commands/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/data_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/git_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:47.309569 cookie_composer-0.9.2/cookie_composer/merge_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/merge_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/merge_files/ini_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/merge_files/json_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/merge_files/toml_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/merge_files/yaml_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/cookie_composer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:47.305570 cookie_composer-0.9.2/cookie_composer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-02-13 14:54:47.000000 cookie_composer-0.9.2/cookie_composer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-02-13 14:54:47.000000 cookie_composer-0.9.2/cookie_composer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 14:54:47.000000 cookie_composer-0.9.2/cookie_composer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-13 14:54:47.000000 cookie_composer-0.9.2/cookie_composer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 14:54:47.000000 cookie_composer-0.9.2/cookie_composer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-02-13 14:54:47.000000 cookie_composer-0.9.2/cookie_composer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-13 14:54:47.000000 cookie_composer-0.9.2/cookie_composer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:47.309569 cookie_composer-0.9.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/requirements/prod.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/requirements/prod.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-02-13 14:54:47.317570 cookie_composer-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:47.313570 cookie_composer-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:47.313570 cookie_composer-0.9.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/empty.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/existing.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/existing.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/existing.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/existing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/gibberish.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/multi-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/new.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/new.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/new.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/new.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:47.313570 cookie_composer-0.9.2/tests/fixtures/rendered1/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/rendered1/context.json
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/rendered1/rendered-composition.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:47.313570 cookie_composer-0.9.2/tests/fixtures/rendered1/testproject/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/rendered1/testproject/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/rendered1/testproject/dontmerge.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/rendered1/testproject/merge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/rendered1/testproject/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:47.313570 cookie_composer-0.9.2/tests/fixtures/rendered2/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/rendered2/context.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:47.313570 cookie_composer-0.9.2/tests/fixtures/rendered2/testproject/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/rendered2/testproject/ABOUT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/rendered2/testproject/dontmerge.json
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/rendered2/testproject/merge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/rendered2/testproject/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/rendered_composition.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/single-template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:47.313570 cookie_composer-0.9.2/tests/fixtures/template1/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/template1/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:47.317570 cookie_composer-0.9.2/tests/fixtures/template1/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/template1/{{cookiecutter.repo_name}}/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/template1/{{cookiecutter.repo_name}}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:47.317570 cookie_composer-0.9.2/tests/fixtures/template2/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/template2/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:47.317570 cookie_composer-0.9.2/tests/fixtures/template2/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/template2/{{cookiecutter.repo_name}}/ABOUT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/fixtures/template2/{{cookiecutter.repo_name}}/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/test_cc_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:47.317570 cookie_composer-0.9.2/tests/test_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/test_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/test_commands/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/test_commands/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/test_commands/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/test_commands/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/test_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/test_git_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/test_merge_files_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/test_merge_files_ini_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/test_merge_files_json_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/test_merge_files_toml_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/test_merge_files_yaml_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-02-13 14:54:35.000000 cookie_composer-0.9.2/tests/test_utils.py
```

### Comparing `cookie_composer-0.9.1/CHANGELOG.md` & `cookie_composer-0.9.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,29 @@
 # Changelog
 
+## 0.9.2 (2023-02-13)
+[Compare the full difference.](https://github.com/coordt/cookie-composer/compare/0.9.1...0.9.2)
+
+### New
+
+- Added test for validate_context_params. [a52d28d](https://github.com/coordt/cookie-composer/commit/a52d28d97445c426f02cb8399883ad8a9052928c)
+    
+- Added ability to pass initial contexts. [9e3cdf3](https://github.com/coordt/cookie-composer/commit/9e3cdf34480f9bfafd5f4750d48b78cc6ac294e1)
+    
+### Updates
+
+- Modified CLI options and arguments. [02a4bf3](https://github.com/coordt/cookie-composer/commit/02a4bf3a9378f2788be53cfa769bbc5a9bb3eae3)
+    
+  - The `output_dir` argument was moved to the `--destination` option.
+  - Added `CONTEXT_PARAMS` argument for initial context
+- Removed checkout from first commit when linking. [f2725ef](https://github.com/coordt/cookie-composer/commit/f2725ef3464f932914e3393e5883792a8f93d0ca)
+    
+  - The first commit was causing confusing issues and now a normal checkout is performed.
+
+
 ## 0.9.1 (2023-02-08)
 [Compare the full difference.](https://github.com/coordt/cookie-composer/compare/0.9.0...0.9.1)
 
 ### New
 
 - Added `--version` option. [4b1b9e1](https://github.com/coordt/cookie-composer/commit/4b1b9e1fd84f976f590dcc1ad803dea4808fe643)
```

### Comparing `cookie_composer-0.9.1/CODE_OF_CONDUCT.md` & `cookie_composer-0.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/CONTRIBUTING.md` & `cookie_composer-0.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/LICENSE` & `cookie_composer-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/PKG-INFO` & `cookie_composer-0.9.2/cookie_composer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cookie_composer
-Version: 0.9.1
+Name: cookie-composer
+Version: 0.9.2
 Summary: Create new projects from a composition of several templates
 Home-page: https://github.com/coordt/cookie-composer
 Author: Corey Oordt
 Author-email: coreyoordt@gmail.com
 Keywords: cookie_composer cookiecutter
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `cookie_composer-0.9.1/README.md` & `cookie_composer-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer/authentication.py` & `cookie_composer-0.9.2/cookie_composer/authentication.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer/cc_overrides.py` & `cookie_composer-0.9.2/cookie_composer/cc_overrides.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer/commands/add.py` & `cookie_composer-0.9.2/cookie_composer/commands/add.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """The implementation of the add command."""
-from typing import Optional
+from typing import Any, Dict, Optional
 
 import logging
 from pathlib import Path
 
 from cookie_composer.composition import (
     get_composition_from_path_or_url,
     read_rendered_composition,
@@ -27,27 +27,29 @@
     destination_dir: Optional[Path] = None,
     no_input: bool = False,
     checkout: Optional[str] = None,
     directory: Optional[str] = None,
     overwrite_if_exists: bool = False,
     skip_if_file_exists: bool = False,
     default_config: bool = False,
+    initial_context: Optional[Dict[str, Any]] = None,
 ):
     """
     Add a template or configuration to an existing project.
 
     Args:
         path_or_url: A URL or string to add the template or configuration
         destination_dir: The project directory to add the layer to
         no_input: If ``True`` force each layer's ``no_input`` attribute to ``True``
         checkout: The branch, tag or commit to check out after git clone
         directory: Directory within repo that holds cookiecutter.json file
         overwrite_if_exists: Overwrite the contents of the output directory if it already exists
         skip_if_file_exists: Skip the files in the corresponding directories if they already exist
         default_config: Do not load a config file. Use the defaults instead
+        initial_context: The initial context for the composition layer
 
     Raises:
         GitError: If the destination_dir is not a git repository
         ValueError: If there is not a .composition.yaml file in the destination directory
     """
     destination_dir = Path(destination_dir).resolve() or Path().cwd().resolve()
     output_dir = destination_dir.parent
@@ -65,14 +67,15 @@
         checkout,
         default_config,
         directory,
         no_input,
         output_dir,
         overwrite_if_exists,
         skip_if_file_exists,
+        initial_context=initial_context or {},
     )
 
     # Get the merged context for all layers
     initial_context = get_context_for_layer(proj_composition)
 
     # Make sure the destination directory is a git repository
     repo = get_repo(destination_dir)
```

### Comparing `cookie_composer-0.9.1/cookie_composer/commands/authn.py` & `cookie_composer-0.9.2/cookie_composer/commands/authn.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer/commands/create.py` & `cookie_composer-0.9.2/cookie_composer/commands/create.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Methods for generating projects."""
 
-from typing import Optional
+from typing import Any, Dict, Optional
 
 import logging
 from pathlib import Path
 
 from cookie_composer.composition import (
     RenderedComposition,
     get_composition_from_path_or_url,
@@ -20,43 +20,46 @@
     output_dir: Optional[Path] = None,
     no_input: bool = False,
     checkout: Optional[str] = None,
     directory: Optional[str] = None,
     overwrite_if_exists: bool = False,
     skip_if_file_exists: bool = False,
     default_config: bool = False,
+    initial_context: Optional[Dict[str, Any]] = None,
 ) -> Path:
     """
     Generate a new project from a composition file, local template or remote template.
 
     Args:
         path_or_url: The path or url to the composition file or template
         output_dir: Where to generate the project
         no_input: If ``True`` force each layer's ``no_input`` attribute to ``True``
         checkout: The branch, tag or commit to check out after git clone
         directory: Directory within repo that holds cookiecutter.json file
         overwrite_if_exists: Overwrite the contents of the output directory if it already exists
         skip_if_file_exists: Skip the files in the corresponding directories if they already exist
         default_config: Do not load a config file. Use the defaults instead
+        initial_context: The initial context for the composition
 
     Returns:
         The path to the generated project.
     """
     output_dir = Path(output_dir).resolve() or Path().cwd().resolve()
     composition = get_composition_from_path_or_url(
         path_or_url,
         checkout,
         default_config,
         directory,
         no_input,
         output_dir,
         overwrite_if_exists,
         skip_if_file_exists,
+        initial_context or {},
     )
-    rendered_layers = render_layers(composition.layers, output_dir, no_input=no_input)
+    rendered_layers = render_layers(composition.layers, output_dir, no_input=no_input, accept_hooks=False)
     rendered_composition = RenderedComposition(
         layers=rendered_layers,
         render_dir=output_dir,
         rendered_name=rendered_layers[0].rendered_name,
     )
     write_rendered_composition(rendered_composition)
     return rendered_composition.render_dir / rendered_composition.rendered_name
```

### Comparing `cookie_composer-0.9.1/cookie_composer/commands/link.py` & `cookie_composer-0.9.2/cookie_composer/commands/link.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 """The implementation of the link command."""
-from typing import Optional
+from typing import Any, Dict, Optional
 
 from pathlib import Path
 
 from cookie_composer.commands.create import create_cmd
-from cookie_composer.git_commands import (
-    branch_exists,
-    branch_from_first_commit,
-    checkout_branch,
-    get_repo,
-    remote_branch_exists,
-)
+from cookie_composer.git_commands import checkout_branch, get_repo
 
 
 def link_cmd(
     path_or_url: str,
     destination_dir: Optional[Path] = None,
     no_input: bool = False,
     checkout: Optional[str] = None,
     directory: Optional[str] = None,
     overwrite_if_exists: bool = False,
     skip_if_file_exists: bool = False,
     default_config: bool = False,
+    initial_context: Optional[Dict[str, Any]] = None,
 ):
     """
     Link a template or configuration to an existing project.
 
     Args:
         path_or_url: A URL or string to add the template or configuration
         destination_dir: The project directory to add the layer to
         no_input: If ``True`` force each layer's ``no_input`` attribute to ``True``
         checkout: The branch, tag or commit to check out after git clone
         directory: Directory within repo that holds cookiecutter.json file
         overwrite_if_exists: Overwrite the contents of the output directory if it already exists
         skip_if_file_exists: Skip the files in the corresponding directories if they already exist
         default_config: Do not load a config file. Use the defaults instead
+        initial_context: The initial context for the composition
 
     Raises:
         GitError: If the destination_dir is not a git repository
         GitError: If the destination_dir git repository is dirty
         ValueError: If there is a .composition.yaml file in the destination directory
     """
     destination_dir = Path(destination_dir).resolve() or Path().cwd().resolve()
@@ -49,30 +45,28 @@
 
     # Check for the project composition file
     proj_composition_path = destination_dir / ".composition.yaml"
     if proj_composition_path.exists():
         raise ValueError(f"There is already a .composition.yaml file in {destination_dir}")
 
     branch_name = "link_composition"
-    if branch_exists(repo, branch_name) or remote_branch_exists(repo, branch_name):
-        checkout_branch(repo, branch_name)
-    else:
-        branch_from_first_commit(repo, branch_name)
+    checkout_branch(repo, branch_name)
 
     previously_untracked_files = set(repo.untracked_files)
 
     create_cmd(
         path_or_url,
         output_dir,
         no_input,
         checkout,
         directory,
         overwrite_if_exists,
         skip_if_file_exists,
         default_config,
+        initial_context=initial_context or {},
     )
 
     changed_files = [item.a_path for item in repo.index.diff(None)]
     untracked_files = set(repo.untracked_files)
     new_untracked_files = untracked_files - previously_untracked_files
     changed_files.extend(list(new_untracked_files))
```

### Comparing `cookie_composer-0.9.1/cookie_composer/commands/update.py` & `cookie_composer-0.9.2/cookie_composer/commands/update.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer/composition.py` & `cookie_composer-0.9.2/cookie_composer/composition.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     def layer_names(self) -> List[str]:
         """Return a list of the names of all the layers."""
         return [x.layer.layer_name for x in self.layers]
 
 
 def is_composition_file(path_or_url: Union[str, Path]) -> bool:
     """
-    Is the filename a composition file?
+    Return ``True`` if the filename a composition file.
 
     Args:
         path_or_url: The path or URL to check
 
     Returns:
         ``True`` if the path is a configuration file.
     """
@@ -325,27 +325,29 @@
     checkout: Optional[str] = None,
     default_config: bool = False,
     directory: Optional[str] = None,
     no_input: bool = False,
     output_dir: Optional[Path] = None,
     overwrite_if_exists: bool = False,
     skip_if_file_exists: bool = False,
+    initial_context: Optional[Dict[str, Any]] = None,
 ) -> Composition:
     """
     Generate a :class:`Composition` from a path or URL.
 
     Args:
         path_or_url: The path or url to the composition file or template
         checkout: The branch, tag or commit to check out after git clone
         default_config: Do not load a config file. Use the defaults instead
         directory: Directory within repo that holds cookiecutter.json file
         no_input: If ``True`` force each layer's ``no_input`` attribute to ``True``
         output_dir: Where to generate the project
         overwrite_if_exists: Overwrite the contents of the output directory if it already exists
         skip_if_file_exists: Skip the files in the corresponding directories if they already exist
+        initial_context: The initial context for the composition
 
     Returns:
         The composition object.
     """
     if is_composition_file(path_or_url):
         composition = read_composition(path_or_url)
         logger.info(f"Rendering composition {path_or_url} to {output_dir}.")
@@ -354,11 +356,12 @@
         tmpl = LayerConfig(
             template=path_or_url,
             directory=directory,
             checkout=checkout,
             no_input=no_input or default_config,
             skip_if_file_exists=skip_if_file_exists,
             overwrite=overwrite_rules,
+            context=initial_context or {},
         )
         composition = Composition(layers=[tmpl])
         logger.info(f"Rendering template {path_or_url} to {output_dir}.")
     return composition
```

### Comparing `cookie_composer-0.9.1/cookie_composer/data_merge.py` & `cookie_composer-0.9.2/cookie_composer/data_merge.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer/diff.py` & `cookie_composer-0.9.2/cookie_composer/diff.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer/exceptions.py` & `cookie_composer-0.9.2/cookie_composer/exceptions.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer/git_commands.py` & `cookie_composer-0.9.2/cookie_composer/git_commands.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer/layers.py` & `cookie_composer-0.9.2/cookie_composer/layers.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer/matching.py` & `cookie_composer-0.9.2/cookie_composer/matching.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer/merge_files/__init__.py` & `cookie_composer-0.9.2/cookie_composer/merge_files/__init__.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer/merge_files/ini_file.py` & `cookie_composer-0.9.2/cookie_composer/merge_files/ini_file.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer/merge_files/json_file.py` & `cookie_composer-0.9.2/cookie_composer/merge_files/json_file.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer/merge_files/toml_file.py` & `cookie_composer-0.9.2/cookie_composer/merge_files/toml_file.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer/merge_files/yaml_file.py` & `cookie_composer-0.9.2/cookie_composer/merge_files/yaml_file.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer/utils.py` & `cookie_composer-0.9.2/cookie_composer/utils.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer.egg-info/PKG-INFO` & `cookie_composer-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cookie-composer
-Version: 0.9.1
+Name: cookie_composer
+Version: 0.9.2
 Summary: Create new projects from a composition of several templates
 Home-page: https://github.com/coordt/cookie-composer
 Author: Corey Oordt
 Author-email: coreyoordt@gmail.com
 Keywords: cookie_composer cookiecutter
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `cookie_composer-0.9.1/cookie_composer.egg-info/SOURCES.txt` & `cookie_composer-0.9.2/cookie_composer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/cookie_composer.egg-info/requires.txt` & `cookie_composer-0.9.2/cookie_composer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/pyproject.toml` & `cookie_composer-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/requirements/dev.txt` & `cookie_composer-0.9.2/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/requirements/docs.txt` & `cookie_composer-0.9.2/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/requirements/prod.txt` & `cookie_composer-0.9.2/requirements/prod.txt`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/requirements/test.txt` & `cookie_composer-0.9.2/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/setup.cfg` & `cookie_composer-0.9.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.9.1
+current_version = 0.9.2
 commit = True
 commit_args = --no-verify
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\+\w+-(?P<dev>\d+))?
 serialize = 
 	{major}.{minor}.{patch}+{$BRANCH_NAME}-{dev}
```

### Comparing `cookie_composer-0.9.1/setup.py` & `cookie_composer-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/tests/conftest.py` & `cookie_composer-0.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/tests/fixtures/rendered_composition.yaml` & `cookie_composer-0.9.2/tests/fixtures/rendered_composition.yaml`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/tests/test_authentication.py` & `cookie_composer-0.9.2/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/tests/test_cc_overrides.py` & `cookie_composer-0.9.2/tests/test_cc_overrides.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/tests/test_commands/test_add.py` & `cookie_composer-0.9.2/tests/test_commands/test_add.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/tests/test_commands/test_create.py` & `cookie_composer-0.9.2/tests/test_commands/test_create.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/tests/test_commands/test_link.py` & `cookie_composer-0.9.2/tests/test_commands/test_link.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,39 +2,53 @@
 import shutil
 from pathlib import Path
 
 import pytest
 from git import Repo
 
 from cookie_composer.commands import link
-from cookie_composer.git_commands import get_repo
+from cookie_composer.git_commands import checkout_branch, get_repo
 
 
 @pytest.fixture
 def linkable_repo(fixtures_path, tmp_path) -> Path:
     """A default repo for testing."""
     rendered_layer = fixtures_path / "rendered1" / "testproject"
     dest_path = tmp_path / "fake-project-template"
     shutil.copytree(rendered_layer, dest_path)
     repo = Repo.init(dest_path)
-    repo.index.add(repo.untracked_files)
-    repo.index.commit(message="Initial commit")
+    for f in repo.untracked_files:
+        repo.index.add(f)
+        repo.index.commit(f"Added untracked file: {f}")
+
     assert not repo.is_dirty()
     return dest_path
 
 
 def test_link(linkable_repo: Path, fixtures_path: Path):
     """Linking an existing repo should create another branch."""
     template = fixtures_path / "template1"
 
     repo = get_repo(linkable_repo)
+    import subprocess
 
-    link.link_cmd(str(template), linkable_repo, no_input=True)
+    output = subprocess.run(
+        ["git", "log", "--graph", "--oneline", "--decorate"], text=True, cwd=linkable_repo, capture_output=True
+    )
+    print(output.stdout)
 
+    previous_master_sha = repo.heads.master.commit.hexsha
+
+    link.link_cmd(str(template), linkable_repo, no_input=True)
+    checkout_branch(repo, "link_composition")
     assert {head.name for head in repo.heads} == {"master", "link_composition"}
+    output = subprocess.run(
+        ["git", "log", "--graph", "--oneline", "--decorate"], text=True, cwd=linkable_repo, capture_output=True
+    )
+    assert repo.commit("link_composition~1").hexsha == previous_master_sha
 
 
 def test_link_cant_install_over_composition(linkable_repo: Path, fixtures_path: Path):
     """Can't link a repo with a .composition.yaml file."""
     repo = get_repo(linkable_repo)
     comp_file = linkable_repo / ".composition.yaml"
     comp_file.write_text("")
```

### Comparing `cookie_composer-0.9.1/tests/test_commands/test_update.py` & `cookie_composer-0.9.2/tests/test_commands/test_update.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/tests/test_composition.py` & `cookie_composer-0.9.2/tests/test_composition.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/tests/test_git_commands.py` & `cookie_composer-0.9.2/tests/test_git_commands.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/tests/test_layers.py` & `cookie_composer-0.9.2/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/tests/test_merge_files_helpers.py` & `cookie_composer-0.9.2/tests/test_merge_files_helpers.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/tests/test_merge_files_ini_file.py` & `cookie_composer-0.9.2/tests/test_merge_files_ini_file.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/tests/test_merge_files_json_file.py` & `cookie_composer-0.9.2/tests/test_merge_files_json_file.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/tests/test_merge_files_toml_file.py` & `cookie_composer-0.9.2/tests/test_merge_files_toml_file.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/tests/test_merge_files_yaml_file.py` & `cookie_composer-0.9.2/tests/test_merge_files_yaml_file.py`

 * *Files identical despite different names*

### Comparing `cookie_composer-0.9.1/tests/test_utils.py` & `cookie_composer-0.9.2/tests/test_utils.py`

 * *Files identical despite different names*

