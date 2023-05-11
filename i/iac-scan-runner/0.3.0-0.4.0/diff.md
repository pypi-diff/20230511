# Comparing `tmp/iac-scan-runner-0.3.0.tar.gz` & `tmp/iac-scan-runner-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac-scan-runner-0.3.0.tar", last modified: Tue Mar 28 08:18:32 2023, max compression
+gzip compressed data, was "iac-scan-runner-0.4.0.tar", last modified: Thu May 11 06:18:40 2023, max compression
```

## Comparing `iac-scan-runner-0.3.0.tar` & `iac-scan-runner-0.4.0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:18:32.807153 iac-scan-runner-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2185 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:18:32.787153 iac-scan-runner-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:18:32.795153 iac-scan-runner-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2820 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    11462 2023-03-28 08:18:32.807153 iac-scan-runner-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9481 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:18:32.799153 iac-scan-runner-0.3.0/config/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/config/ansiblelint.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     8327 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/config/bandit.conf
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/config/dockerlint.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3678 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/config/git-leaks.toml
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/config/git-secrets.txt
--rw-r--r--   0 runner    (1001) docker     (122)      642 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/config/htmllint.json
--rw-r--r--   0 runner    (1001) docker     (122)     6690 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/config/javalint.xml
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/config/jslint.json
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/config/mdlint.rb
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/config/mdlint.rc
--rw-r--r--   0 runner    (1001) docker     (122)    16852 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/config/pylint.rc
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/config/scsslint.json
--rw-r--r--   0 runner    (1001) docker     (122)      201 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/config/sonar-project.properties
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/config/tslint.json
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/config/yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      384 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/docker-compose.yaml
--rwxr-xr-x   0 runner    (1001) docker     (122)     6191 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/install-checks.sh
--rw-r--r--   0 runner    (1001) docker     (122)    26774 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/open-api.json
--rw-r--r--   0 runner    (1001) docker     (122)   271405 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (122)      659 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/package.json
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-03-28 08:18:32.807153 iac-scan-runner-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:18:32.799153 iac-scan-runner-0.3.0/src/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:18:32.799153 iac-scan-runner-0.3.0/src/iac_scan_runner/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:18:32.803153 iac-scan-runner-0.3.0/src/iac_scan_runner/asset/
--rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/asset/response.html
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/asset/table_basic.html
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/asset/table_info.html
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/asset/table_problem.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:18:32.807153 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/ansible_lint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/bandit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1711 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/checkstyle.py
--rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/cloc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/es_lint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/git_leaks.py
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/git_secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/gixy.py
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/hadolint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1206 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/htmlhint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/markdown_lint.py
--rw-r--r--   0 runner    (1001) docker     (122)      644 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/opera_tosca_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/pylint.py
--rw-r--r--   0 runner    (1001) docker     (122)      900 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/pyup_safety.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/shellcheck.py
--rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/snyk.py
--rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/sonar_scanner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/steampunk_scanner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/stylelint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/terrascan.py
--rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/tflint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1203 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/tfsec.py
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/ts_lint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1348 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/checks/yamllint.py
--rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:18:32.807153 iac-scan-runner-0.3.0/src/iac_scan_runner/enums/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/enums/check_target_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/enums/scan_response_type.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:18:32.807153 iac-scan-runner-0.3.0/src/iac_scan_runner/functionality/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/functionality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      733 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/functionality/check_output.py
--rw-r--r--   0 runner    (1001) docker     (122)      506 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/functionality/cleanup_old_scans.py
--rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/functionality/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (122)     4316 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/functionality/project_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5009 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/functionality/results_persistence.py
--rw-r--r--   0 runner    (1001) docker     (122)    13500 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/functionality/results_summary.py
--rw-r--r--   0 runner    (1001) docker     (122)     7055 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/functionality/scan_project.py
--rw-r--r--   0 runner    (1001) docker     (122)    20113 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/functionality/scan_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:18:32.807153 iac-scan-runner-0.3.0/src/iac_scan_runner/interface/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1549 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/interface/check.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:18:32.807153 iac-scan-runner-0.3.0/src/iac_scan_runner/model/
--rw-r--r--   0 runner    (1001) docker     (122)      994 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/model/ConfigureCheck.py
--rw-r--r--   0 runner    (1001) docker     (122)      927 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/model/Scan.py
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/object_store.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:18:32.807153 iac-scan-runner-0.3.0/src/iac_scan_runner/routers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5701 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/routers/checks.py
--rw-r--r--   0 runner    (1001) docker     (122)      946 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/routers/openapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     9147 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/routers/project.py
--rw-r--r--   0 runner    (1001) docker     (122)     4274 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-03-28 08:15:16.000000 iac-scan-runner-0.3.0/src/iac_scan_runner/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:18:32.803153 iac-scan-runner-0.3.0/src/iac_scan_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11462 2023-03-28 08:18:32.000000 iac-scan-runner-0.3.0/src/iac_scan_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-03-28 08:18:32.000000 iac-scan-runner-0.3.0/src/iac_scan_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-28 08:18:32.000000 iac-scan-runner-0.3.0/src/iac_scan_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-03-28 08:18:32.000000 iac-scan-runner-0.3.0/src/iac_scan_runner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-03-28 08:18:32.000000 iac-scan-runner-0.3.0/src/iac_scan_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-03-28 08:18:32.000000 iac-scan-runner-0.3.0/src/iac_scan_runner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-28 08:18:32.000000 iac-scan-runner-0.3.0/src/iac_scan_runner.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.821981 iac-scan-runner-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     2185 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.801981 iac-scan-runner-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.801981 iac-scan-runner-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2820 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    11438 2023-05-11 06:18:40.821981 iac-scan-runner-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9458 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.801981 iac-scan-runner-0.4.0/config/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/ansiblelint.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     8327 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/bandit.conf
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/dockerlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3678 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/git-leaks.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/git-secrets.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      642 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/htmllint.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6690 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/javalint.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/jslint.json
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/mdlint.rb
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/mdlint.rc
+-rw-r--r--   0 runner    (1001) docker     (122)    16852 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/pylint.rc
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/scsslint.json
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/sonar-project.properties
+-rw-r--r--   0 runner    (1001) docker     (122)     1239 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/tslint.json
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      384 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/docker-compose.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6191 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/install-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (122)    26774 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/open-api.json
+-rw-r--r--   0 runner    (1001) docker     (122)   271405 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (122)      659 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-05-11 06:18:40.821981 iac-scan-runner-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.801981 iac-scan-runner-0.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.805981 iac-scan-runner-0.4.0/src/iac_scan_runner/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.805981 iac-scan-runner-0.4.0/src/iac_scan_runner/asset/
+-rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/asset/response.html
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/asset/table_basic.html
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/asset/table_info.html
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/asset/table_problem.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.813981 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/ansible_lint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/bandit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1711 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/checkstyle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/cloc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/es_lint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/git_leaks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/git_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/gixy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/hadolint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1206 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/htmlhint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/markdown_lint.py
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/opera_tosca_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/pyup_safety.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/shellcheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/snyk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/sonar_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/steampunk_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/stylelint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/terrascan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/tflint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1203 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/tfsec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/ts_lint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1348 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/yamllint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.817981 iac-scan-runner-0.4.0/src/iac_scan_runner/enums/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/enums/check_target_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/enums/scan_response_type.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.817981 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      733 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/check_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/cleanup_old_scans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4316 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/project_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5031 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/results_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13500 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/results_summary.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7265 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/scan_project.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20230 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/scan_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.817981 iac-scan-runner-0.4.0/src/iac_scan_runner/interface/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1549 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/interface/check.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.821981 iac-scan-runner-0.4.0/src/iac_scan_runner/model/
+-rw-r--r--   0 runner    (1001) docker     (122)      994 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/model/ConfigureCheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/model/Scan.py
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/object_store.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.821981 iac-scan-runner-0.4.0/src/iac_scan_runner/routers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5701 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/routers/checks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/routers/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/routers/project.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4274 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.805981 iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11438 2023-05-11 06:18:40.000000 iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-05-11 06:18:40.000000 iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 06:18:40.000000 iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-11 06:18:40.000000 iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-11 06:18:40.000000 iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-11 06:18:40.000000 iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 06:18:40.000000 iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/zip-safe
```

### Comparing `iac-scan-runner-0.3.0/.dockerignore` & `iac-scan-runner-0.4.0/.dockerignore`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/.github/workflows/ci_cd.yml` & `iac-scan-runner-0.4.0/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/.gitignore` & `iac-scan-runner-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/Dockerfile` & `iac-scan-runner-0.4.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/LICENSE` & `iac-scan-runner-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/PKG-INFO` & `iac-scan-runner-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-scan-runner
-Version: 0.3.0
+Version: 0.4.0
 Summary: IaC Scan Runner CLI
 Home-page: https://github.com/xlab-si/iac-scan-runner
 Author: XLAB d.o.o.
 Author-email: pypi@xlab.si
 Maintainer: xOpera team
 Maintainer-email: xopera@xlab.si
 Project-URL: Source Code, https://github.com/xlab-si/iac-scan-runner
@@ -39,15 +39,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IaC Scan Runner
 
 Service that scans your Infrastructure as Code for common vulnerabilities.
 
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/xlab-si/iac-scan-runner/Build%20and%20publish?label=ci%2Fcd)](https://github.com/xlab-si/iac-scan-runner/actions)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/xlab-si/iac-scan-runner/ci_cd.yml?branch=main)](https://github.com/xlab-si/iac-scan-runner/actions)
 [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/xscanner/runner?color=blue&label=docker)](https://hub.docker.com/r/xscanner/runner)
 [![PyPI](https://img.shields.io/pypi/v/iac-scan-runner)](https://pypi.org/project/iac-scan-runner/)
 [![Test PyPI](https://img.shields.io/badge/test%20pypi-dev%20version-blueviolet)](https://test.pypi.org/project/iac-scan-runner/)
 
 | Aspect        |     Information     |
 |---------------|:-------------------:|
 | Tool name     | **IaC Scan Runner** |
@@ -114,20 +114,29 @@
 ```
 
 ### Run from source
 
 To run locally from source:
 
 ```console
+# Export env variables 
+export MONGODB_CONNECTION_STRING=mongodb://localhost:27017
+export SCAN_PERSISTENCE=enabled
+export USER_MANAGEMENT=enabled
+
+# Setup MongoDB
+$ docker run --name mongodb -p 27017:27017 mongo
+
 # install prerequisites
 $ python3 -m venv .venv && . .venv/bin/activate
 (.venv) $ pip install -r requirements.txt
 (.venv) $ ./install-checks.sh
 # run IaC Scan Runner REST API (add --reload flag to apply code changes on the way)
-(.venv) $ uvicorn src.iac_scan_runner.api:app
+(.venv) $ cd src
+(.venv) $ uvicorn iac_scan_runner.api:app
 ```
 
 ## Usage and examples
 
 This part will show one of the possible deployments and short examples on how to use API calls.
 
 Firstly we will clone the [iac scan runner] repository and run the API.
@@ -148,40 +157,32 @@
   'http://0.0.0.0/project?creator_id=test' \
   -H 'accept: application/json' \
   -d ''
 ```
 
 project id will be returned to us. For this example project id is 1e7b2a91-2896-40fd-8d53-83db56088026.
 
-2. Now check if project is created by listing all existing projects.
-
-```console
-curl -X 'GET' \
-  'http://0.0.0.0/project/checks?project_id=1e7b2a91-2896-40fd-8d53-83db56088026' \
-  -H 'accept: application/json'
-```
 
-3. For example, let say we want to initiate all check expect ansible-lint. Let's disable it.
+2. For example, let say we want to initiate all check expect ansible-lint. Let's disable it.
 
 ```console
 curl -X 'PUT' \
-  'http://0.0.0.0/project/checks/ansible-lint/disable?project_id=1e7b2a91-2896-40fd-8d53-83db56088026' \
+  'http://0.0.0.0:8000/projects/1e7b2a91-2896-40fd-8d53-83db56088026/checks/ansible-lint/disable' \
   -H 'accept: application/json'
 ```
 
-4. Now when project is configured, we can simply choose files that we want to scan and zip them. For IaC-Scan-Runner to
+3. Now when project is configured, we can simply choose files that we want to scan and zip them. For IaC-Scan-Runner to
    work files are expected to be a compressed archives (usually zip files). In this case response type will be json
    , but it is possible to change it to html.Please change YOUR.zip to path of your file.
 
 ```console
 curl -X 'POST' \
-  'http://0.0.0.0/project/scan?project_id=1e7b2a91-2896-40fd-8d53-83db56088026&scan_response_type=json' \
+  'http://0.0.0.0:8000/projects/1e7b2a91-2896-40fd-8d53-83db56088026/scan?scan_response_type=json' \
   -H 'accept: application/json' \
   -H 'Content-Type: multipart/form-data' \
-  -F 'checks=' \
   -F 'iac=@YOUR.zip;type=application/zip'
 ```
 
 That is it.
 
 ### Extending the scan workflow with new check tools
```

### Comparing `iac-scan-runner-0.3.0/README.md` & `iac-scan-runner-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # IaC Scan Runner
 
 Service that scans your Infrastructure as Code for common vulnerabilities.
 
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/xlab-si/iac-scan-runner/Build%20and%20publish?label=ci%2Fcd)](https://github.com/xlab-si/iac-scan-runner/actions)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/xlab-si/iac-scan-runner/ci_cd.yml?branch=main)](https://github.com/xlab-si/iac-scan-runner/actions)
 [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/xscanner/runner?color=blue&label=docker)](https://hub.docker.com/r/xscanner/runner)
 [![PyPI](https://img.shields.io/pypi/v/iac-scan-runner)](https://pypi.org/project/iac-scan-runner/)
 [![Test PyPI](https://img.shields.io/badge/test%20pypi-dev%20version-blueviolet)](https://test.pypi.org/project/iac-scan-runner/)
 
 | Aspect        |     Information     |
 |---------------|:-------------------:|
 | Tool name     | **IaC Scan Runner** |
@@ -73,20 +73,29 @@
 ```
 
 ### Run from source
 
 To run locally from source:
 
 ```console
+# Export env variables 
+export MONGODB_CONNECTION_STRING=mongodb://localhost:27017
+export SCAN_PERSISTENCE=enabled
+export USER_MANAGEMENT=enabled
+
+# Setup MongoDB
+$ docker run --name mongodb -p 27017:27017 mongo
+
 # install prerequisites
 $ python3 -m venv .venv && . .venv/bin/activate
 (.venv) $ pip install -r requirements.txt
 (.venv) $ ./install-checks.sh
 # run IaC Scan Runner REST API (add --reload flag to apply code changes on the way)
-(.venv) $ uvicorn src.iac_scan_runner.api:app
+(.venv) $ cd src
+(.venv) $ uvicorn iac_scan_runner.api:app
 ```
 
 ## Usage and examples
 
 This part will show one of the possible deployments and short examples on how to use API calls.
 
 Firstly we will clone the [iac scan runner] repository and run the API.
@@ -107,40 +116,32 @@
   'http://0.0.0.0/project?creator_id=test' \
   -H 'accept: application/json' \
   -d ''
 ```
 
 project id will be returned to us. For this example project id is 1e7b2a91-2896-40fd-8d53-83db56088026.
 
-2. Now check if project is created by listing all existing projects.
-
-```console
-curl -X 'GET' \
-  'http://0.0.0.0/project/checks?project_id=1e7b2a91-2896-40fd-8d53-83db56088026' \
-  -H 'accept: application/json'
-```
 
-3. For example, let say we want to initiate all check expect ansible-lint. Let's disable it.
+2. For example, let say we want to initiate all check expect ansible-lint. Let's disable it.
 
 ```console
 curl -X 'PUT' \
-  'http://0.0.0.0/project/checks/ansible-lint/disable?project_id=1e7b2a91-2896-40fd-8d53-83db56088026' \
+  'http://0.0.0.0:8000/projects/1e7b2a91-2896-40fd-8d53-83db56088026/checks/ansible-lint/disable' \
   -H 'accept: application/json'
 ```
 
-4. Now when project is configured, we can simply choose files that we want to scan and zip them. For IaC-Scan-Runner to
+3. Now when project is configured, we can simply choose files that we want to scan and zip them. For IaC-Scan-Runner to
    work files are expected to be a compressed archives (usually zip files). In this case response type will be json
    , but it is possible to change it to html.Please change YOUR.zip to path of your file.
 
 ```console
 curl -X 'POST' \
-  'http://0.0.0.0/project/scan?project_id=1e7b2a91-2896-40fd-8d53-83db56088026&scan_response_type=json' \
+  'http://0.0.0.0:8000/projects/1e7b2a91-2896-40fd-8d53-83db56088026/scan?scan_response_type=json' \
   -H 'accept: application/json' \
   -H 'Content-Type: multipart/form-data' \
-  -F 'checks=' \
   -F 'iac=@YOUR.zip;type=application/zip'
 ```
 
 That is it.
 
 ### Extending the scan workflow with new check tools
 
@@ -214,8 +215,8 @@
 
 [xopera@xlab.si]: mailto:xopera@xlab.si
 
 [Apache License 2.0]: https://www.apache.org/licenses/LICENSE-2.0
 
 [PIACERE]: https://www.piacere-project.eu/
 
-[iac scan runner]: https://github.com/xlab-si/iac-scan-runner
+[iac scan runner]: https://github.com/xlab-si/iac-scan-runner
```

### Comparing `iac-scan-runner-0.3.0/config/bandit.conf` & `iac-scan-runner-0.4.0/config/bandit.conf`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/config/git-leaks.toml` & `iac-scan-runner-0.4.0/config/git-leaks.toml`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/config/htmllint.json` & `iac-scan-runner-0.4.0/config/htmllint.json`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/config/javalint.xml` & `iac-scan-runner-0.4.0/config/javalint.xml`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/config/jslint.json` & `iac-scan-runner-0.4.0/config/jslint.json`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/config/pylint.rc` & `iac-scan-runner-0.4.0/config/pylint.rc`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/config/scsslint.json` & `iac-scan-runner-0.4.0/config/scsslint.json`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/config/tslint.json` & `iac-scan-runner-0.4.0/config/tslint.json`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/install-checks.sh` & `iac-scan-runner-0.4.0/install-checks.sh`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/open-api.json` & `iac-scan-runner-0.4.0/open-api.json`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/package-lock.json` & `iac-scan-runner-0.4.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/package.json` & `iac-scan-runner-0.4.0/package.json`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/setup.cfg` & `iac-scan-runner-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/api.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/api.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/asset/response.html` & `iac-scan-runner-0.4.0/src/iac_scan_runner/asset/response.html`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/ansible_lint.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/ansible_lint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/bandit.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/bandit.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/checkstyle.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/checkstyle.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/cloc.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/cloc.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/es_lint.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/es_lint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/git_leaks.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/git_leaks.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/git_secrets.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/git_secrets.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/gixy.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/gixy.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/hadolint.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/hadolint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/htmlhint.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/htmlhint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/markdown_lint.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/markdown_lint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/opera_tosca_parser.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/opera_tosca_parser.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/pylint.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/pylint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/pyup_safety.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/pyup_safety.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/shellcheck.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/shellcheck.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/snyk.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/snyk.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/sonar_scanner.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/sonar_scanner.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/steampunk_scanner.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/steampunk_scanner.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/stylelint.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/stylelint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/terrascan.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/terrascan.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/tflint.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/tflint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/tfsec.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/tfsec.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/ts_lint.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/ts_lint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/checks/yamllint.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/yamllint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/cli.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/cli.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/functionality/check_output.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/check_output.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/functionality/compatibility.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/compatibility.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/functionality/project_config.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/project_config.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/functionality/results_persistence.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/results_persistence.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,12 +137,12 @@
         :return: All scan results for given project identifier
         """
         if self.connection_problem:
             self.connect_db()
 
         if self.mycol is not None:
             myquery = {"project_id": project_id}
-            cursor = self.mycol.find(myquery)
-            output = ""
-            for doc in cursor:
-                output = output + str(doc)
-            return output
+            data = self.mycol.find_one(myquery)
+            if data is None:
+                raise Exception("Project id does not exist or there are no scan results")
+            return data
+
```

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/functionality/results_summary.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/results_summary.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/functionality/scan_project.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/scan_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,17 +79,18 @@
         :return: JSON object of project
         """
         if self.connection_problem:
             self.connect_db()
 
         if self.mycol is not None:
             myquery = {"project_id": project_id}
-            mydoc = self.mycol.find(myquery)
-            for x in mydoc:
-                return x
+            mydoc = self.mycol.find_one(myquery)
+            if mydoc is None:
+                raise Exception("Project id does not exist")
+            return mydoc
 
     def set_config(self, project_id: str, config_id: str):
 
         """Changes an active configuration of a given scan project
         :param project_id: Identifier of a scan project
         :param config_id: Identifier of currently active project configuration that we want to assign     
         :return: JSON object of user
@@ -187,22 +188,25 @@
         """
         if self.connection_problem:
             self.connect_db()
 
         if self.mycol is not None:
             current_project = self.load_project(project_id)
             current_list = current_project["checklist"]
-            current_list.remove(check)
+            current_list.remove(check) if check in current_list else None
             myquery = {"project_id": project_id}
             new_value = {"$set": {"checklist": current_list}}
             try:
                 self.mycol.find_one_and_update(myquery, new_value, upsert=True)
             except Exception as e:
                 print(str(e))
 
     def get_project_check_list(self, project_id):
         """Get project check list
 
         :param project_id: Identifier of a scan project
         """
         query = {"project_id": project_id}
-        return self.mycol.find_one(query, {"checklist": 1, "_id": 0})["checklist"]
+        result = self.mycol.find_one(query, {"checklist": 1, "_id": 0})
+        if result is None:
+            raise Exception("Project id does not exist")
+        return result["checklist"]
```

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/functionality/scan_runner.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/scan_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,14 +337,16 @@
     def disable_check(self, check_name: str, project_id: str) -> str:
         """
         Disables the specified check and makes it unavailable to be used
         :param check_name: Name of the check
         :param project_id: Project identification
         :return: String with result for disabling check
         """
+        if check_name not in self.iac_checks.keys():
+            raise Exception(f"Nonexistent check: {check_name}")
         if project_id and self.users_enabled:
             self.scan_project.remove_check(project_id, check_name)
             self.iac_checks[check_name].enabled = False
             active_project = self.scan_project.load_project(project_id)
             enabled_checks = active_project["checklist"]
         else:
             if check_name in self.iac_checks.keys():
```

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/interface/check.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/interface/check.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/model/ConfigureCheck.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/model/ConfigureCheck.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/model/Scan.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/model/Scan.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,32 @@
 
 
 class ScanModel(BaseModel):
     """
     Scan model
     """
     iac: UploadFile
+
+    @classmethod
+    def as_form(cls,
+                iac: UploadFile = File(default=None,
+                                       description='IaC file (zip or tar compressed) that will be scanned')):
+        """
+        Converts model to form_data structure for FastAPI
+
+        :param iac: zip file of documents to be scanned
+        """
+        return cls(iac=iac)
+
+
+class ScanModelDeprecated(BaseModel):
+    """
+    Deprecated Scan model
+    """
+    iac: UploadFile
     checks: Optional[List[str]]
 
     @classmethod
     def as_form(cls,
                 checks: Optional[List[str]] = Form(None,
                                                    description='List of selected checks (by their unique names) to '
                                                                'be executed on IaC'),
```

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/object_store.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/object_store.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 
 tags_metadata = [
     {
         "name": "Checks",
         "description": "***Depricated***",
     },
     {
-        "name": "Project",
+        "name": "Projects",
     },
 ]
 
 app = FastAPI(
     docs_url="/swagger",
     title="IaC Scan Runner REST API",
     description="Service that scans your Infrastructure as Code for common vulnerabilities",
-    version="0.3.0",
+    version="0.4.0",
     root_path=os.getenv('ROOT_PATH', "/"),
     openapi_tags=tags_metadata
 )
```

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/routers/checks.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/routers/checks.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/routers/openapi.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/routers/openapi.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/routers/project.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/routers/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from iac_scan_runner.enums.scan_response_type import ScanResponseType
 from iac_scan_runner.functionality.results_persistence import ResultsPersistence
 from iac_scan_runner.functionality.scan_project import ScanProject
 from iac_scan_runner.model.ConfigureCheck import CheckConfigurationModel
 from iac_scan_runner.model.Scan import ScanModel
 from iac_scan_runner.object_store import scan_runner
 
-router = APIRouter(tags=["Project"], prefix="/project")
+router = APIRouter(tags=["Projects"], prefix="/projects")
 
 
 @router.post("", summary="Generate new scan project for given user as creator",
              responses={200: {}, 400: {"model": str}})
 async def post_new_project(creator_id: str) -> JSONResponse:
     """
     Create a new project which might contain multiple scan runs
@@ -31,44 +31,35 @@
         pid = scan_project.new_project(creator_id, "", scan_runner.project_checklist)
 
         return JSONResponse(status_code=status.HTTP_200_OK, content=pid)
     except Exception as e:
         return JSONResponse(status_code=status.HTTP_400_BAD_REQUEST, content=str(e))
 
 
-@router.post("/scan", summary="Initiate IaC scan", responses={200: {}, 400: {"model": str}})
-async def post_scan(form_data: ScanModel = Depends(ScanModel.as_form),
-                    project_id: Optional[str] = None,
+@router.post("/{project_id}/scan", summary="Initiate IaC scan", responses={200: {}, 400: {"model": str}})
+async def post_scan(project_id: str, form_data: ScanModel = Depends(ScanModel.as_form),
                     scan_response_type: ScanResponseType = ScanResponseType.json) -> Union[JSONResponse, HTMLResponse]:
     """
     Run IaC scan
     \f
     :param form_data: Form data model
     :param project_id: Identifier of a project_id to which where scan run belongs
     :param scan_response_type: Scan response type (JSON or HTML)
     :return: JSONResponse or HTMLResponse object (with status code 200 or 400)
     """
     try:
-        if not form_data.checks or form_data.checks == ['']:
-            checks = []
-        else:
-            checks = list(set(form_data.checks[0].split(",")))
-
-        if not project_id:
-            project_id = ""
-
-        scan_output = scan_runner.scan_iac(form_data.iac, project_id, checks, scan_response_type)
+        scan_output = scan_runner.scan_iac(form_data.iac, project_id, [], scan_response_type)
         if scan_response_type == ScanResponseType.html:
             return HTMLResponse(status_code=status.HTTP_200_OK, content=scan_output)
         return JSONResponse(status_code=status.HTTP_200_OK, content=scan_output)
     except Exception as e:
         return JSONResponse(status_code=status.HTTP_400_BAD_REQUEST, content=str(e))
 
 
-@router.get("/results", summary="Retrieve particular scan result by given uuid",
+@router.get("/{project_id}/results", summary="Retrieve particular scan result by given uuid",
             responses={200: {}, 400: {"model": str}})
 async def get_scan_result(uuid: Optional[str], project_id: Optional[str]) -> JSONResponse:
     """
     Retrieve a particular scan result
     \f
     :param uuid: Identifier of a saved scan record
     :param project_id: Identifier of a project
@@ -94,31 +85,32 @@
     Delete a particular scan result
     \f
     :param uuid: Identifier of a saved scan record
     :return: JSONResponse object (with status code 200 or 400)
     """
     try:
         results_persistence = ResultsPersistence()
-
         result = results_persistence.show_result(uuid)
         if not result is None:
             results_persistence.delete_result(uuid)
             return JSONResponse(status_code=status.HTTP_200_OK, content=f"Deleted scan result {uuid}")
         else:
             return JSONResponse(status_code=status.HTTP_200_OK, content=f"No such scan result {uuid}")
     except Exception as e:
         return JSONResponse(status_code=status.HTTP_400_BAD_REQUEST, content=str(e))
 
 
-@router.get("/checks", summary="Retrieve and filter checks", responses={200: {}, 400: {"model": str}})
-async def get_checks(project_id:str, keyword: Optional[str] = None, enabled: Optional[bool] = None, configured: Optional[bool] = None,
+@router.get("/{project_id}/checks", summary="Retrieve and filter checks", responses={200: {}, 400: {"model": str}})
+async def get_checks(project_id: str, keyword: Optional[str] = None, enabled: Optional[bool] = None,
+                     configured: Optional[bool] = None,
                      target_entity_type: Optional[CheckTargetEntityType] = None) -> JSONResponse:
     """
     Retrieve and filter checks
     \f
+    :param project_id: Identifier of a project
     :param keyword: substring for filtering
     :param enabled: bool saying whether check is enabled or disabled
     :param configured: bool saying whether check is configured or not
     :param target_entity_type: CheckTargetEntityType object - IaC, component or both
     :return: JSONResponse object (with status code 200 or 400)
     """
     try:
@@ -139,15 +131,15 @@
                                     "configured": check.configured, "target_entity_type": check.target_entity_type},
                      filtered_checks)
         return JSONResponse(status_code=status.HTTP_200_OK, content=list(checks))
     except Exception as e:
         return JSONResponse(status_code=status.HTTP_400_BAD_REQUEST, content=str(e))
 
 
-@router.put("/checks/{check_name}/enable", summary="Enable execution of particular check for a specific project",
+@router.put("/{project_id}/checks/{check_name}/enable", summary="Enable execution of particular check for a specific project",
             responses={200: {}, 400: {"model": str}})
 async def put_enable_checks(check_name: str, project_id: Optional[str]) -> JSONResponse:
     """
     Enable execution of particular check for a specific project
     \f
     :param check_name: Unique name of check to be enabled
     :param project_id: Identifier of a project
@@ -155,38 +147,39 @@
     """
     try:
         return JSONResponse(status_code=status.HTTP_200_OK, content=scan_runner.enable_check(check_name, project_id))
     except Exception as e:
         return JSONResponse(status_code=status.HTTP_400_BAD_REQUEST, content=str(e))
 
 
-@router.put("/checks/{check_name}/disable", summary="Disable execution of particular check for a specific project",
+@router.put("/{project_id}/checks/{check_name}/disable", summary="Disable execution of particular check for a specific project",
             responses={200: {}, 400: {"model": str}})
-async def put_disable_checks(check_name: str, project_id: Optional[str]) -> JSONResponse:
+async def put_disable_checks(project_id: str, check_name: str) -> JSONResponse:
     """
     Disable execution of particular check for a specific project
     \f
     :param check_name: Unique name of check to be disabled
     :param project_id: Identifier of a project
     :return: JSONResponse object (with status code 200 or 400)
     """
     try:
         return JSONResponse(status_code=status.HTTP_200_OK, content=scan_runner.disable_check(check_name, project_id))
     except Exception as e:
         return JSONResponse(status_code=status.HTTP_400_BAD_REQUEST, content=str(e))
 
 
-@router.put("/checks/{check_name}/configure", summary="Configure execution of particular check for a specific project",
+@router.put("/{project_id}/checks/{check_name}/configure", summary="Configure execution of particular check for a specific project",
             responses={200: {}, 400: {"model": str}})
-async def put_configure_check(check_name: str,
+async def put_configure_check(project_id: str, check_name: str,
                               form_data: CheckConfigurationModel = Depends(
                                   CheckConfigurationModel.as_form)) -> JSONResponse:
     """
     Configure execution of particular check for a specific project
     \f
+    :param project_id: Identifier of a project
     :param check_name: Unique name of check to be configured
     :param form_data: Form data model
     :return: JSONResponse object (with status code 200 or 400)
     """
     try:
         return JSONResponse(status_code=status.HTTP_200_OK,
                             content=scan_runner.configure_check(check_name, form_data.config_file, form_data.secret))
```

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/utils.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/utils.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner/vars.py` & `iac-scan-runner-0.4.0/src/iac_scan_runner/vars.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner.egg-info/PKG-INFO` & `iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-scan-runner
-Version: 0.3.0
+Version: 0.4.0
 Summary: IaC Scan Runner CLI
 Home-page: https://github.com/xlab-si/iac-scan-runner
 Author: XLAB d.o.o.
 Author-email: pypi@xlab.si
 Maintainer: xOpera team
 Maintainer-email: xopera@xlab.si
 Project-URL: Source Code, https://github.com/xlab-si/iac-scan-runner
@@ -39,15 +39,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IaC Scan Runner
 
 Service that scans your Infrastructure as Code for common vulnerabilities.
 
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/xlab-si/iac-scan-runner/Build%20and%20publish?label=ci%2Fcd)](https://github.com/xlab-si/iac-scan-runner/actions)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/xlab-si/iac-scan-runner/ci_cd.yml?branch=main)](https://github.com/xlab-si/iac-scan-runner/actions)
 [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/xscanner/runner?color=blue&label=docker)](https://hub.docker.com/r/xscanner/runner)
 [![PyPI](https://img.shields.io/pypi/v/iac-scan-runner)](https://pypi.org/project/iac-scan-runner/)
 [![Test PyPI](https://img.shields.io/badge/test%20pypi-dev%20version-blueviolet)](https://test.pypi.org/project/iac-scan-runner/)
 
 | Aspect        |     Information     |
 |---------------|:-------------------:|
 | Tool name     | **IaC Scan Runner** |
@@ -114,20 +114,29 @@
 ```
 
 ### Run from source
 
 To run locally from source:
 
 ```console
+# Export env variables 
+export MONGODB_CONNECTION_STRING=mongodb://localhost:27017
+export SCAN_PERSISTENCE=enabled
+export USER_MANAGEMENT=enabled
+
+# Setup MongoDB
+$ docker run --name mongodb -p 27017:27017 mongo
+
 # install prerequisites
 $ python3 -m venv .venv && . .venv/bin/activate
 (.venv) $ pip install -r requirements.txt
 (.venv) $ ./install-checks.sh
 # run IaC Scan Runner REST API (add --reload flag to apply code changes on the way)
-(.venv) $ uvicorn src.iac_scan_runner.api:app
+(.venv) $ cd src
+(.venv) $ uvicorn iac_scan_runner.api:app
 ```
 
 ## Usage and examples
 
 This part will show one of the possible deployments and short examples on how to use API calls.
 
 Firstly we will clone the [iac scan runner] repository and run the API.
@@ -148,40 +157,32 @@
   'http://0.0.0.0/project?creator_id=test' \
   -H 'accept: application/json' \
   -d ''
 ```
 
 project id will be returned to us. For this example project id is 1e7b2a91-2896-40fd-8d53-83db56088026.
 
-2. Now check if project is created by listing all existing projects.
-
-```console
-curl -X 'GET' \
-  'http://0.0.0.0/project/checks?project_id=1e7b2a91-2896-40fd-8d53-83db56088026' \
-  -H 'accept: application/json'
-```
 
-3. For example, let say we want to initiate all check expect ansible-lint. Let's disable it.
+2. For example, let say we want to initiate all check expect ansible-lint. Let's disable it.
 
 ```console
 curl -X 'PUT' \
-  'http://0.0.0.0/project/checks/ansible-lint/disable?project_id=1e7b2a91-2896-40fd-8d53-83db56088026' \
+  'http://0.0.0.0:8000/projects/1e7b2a91-2896-40fd-8d53-83db56088026/checks/ansible-lint/disable' \
   -H 'accept: application/json'
 ```
 
-4. Now when project is configured, we can simply choose files that we want to scan and zip them. For IaC-Scan-Runner to
+3. Now when project is configured, we can simply choose files that we want to scan and zip them. For IaC-Scan-Runner to
    work files are expected to be a compressed archives (usually zip files). In this case response type will be json
    , but it is possible to change it to html.Please change YOUR.zip to path of your file.
 
 ```console
 curl -X 'POST' \
-  'http://0.0.0.0/project/scan?project_id=1e7b2a91-2896-40fd-8d53-83db56088026&scan_response_type=json' \
+  'http://0.0.0.0:8000/projects/1e7b2a91-2896-40fd-8d53-83db56088026/scan?scan_response_type=json' \
   -H 'accept: application/json' \
   -H 'Content-Type: multipart/form-data' \
-  -F 'checks=' \
   -F 'iac=@YOUR.zip;type=application/zip'
 ```
 
 That is it.
 
 ### Extending the scan workflow with new check tools
```

### Comparing `iac-scan-runner-0.3.0/src/iac_scan_runner.egg-info/SOURCES.txt` & `iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

