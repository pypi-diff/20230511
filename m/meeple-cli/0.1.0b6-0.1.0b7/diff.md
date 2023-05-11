# Comparing `tmp/meeple-cli-0.1.0b6.tar.gz` & `tmp/meeple-cli-0.1.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meeple-cli-0.1.0b6.tar", last modified: Mon Apr 17 03:57:16 2023, max compression
+gzip compressed data, was "meeple-cli-0.1.0b7.tar", last modified: Thu May 11 01:15:57 2023, max compression
```

## Comparing `meeple-cli-0.1.0b6.tar` & `meeple-cli-0.1.0b7.tar`

### file list

```diff
@@ -1,54 +1,53 @@
--rw-r--r--   0        0        0       66 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/.flake8
--rw-r--r--   0        0        0     1090 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1290 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/.github/workflows/python-test.yml
--rw-r--r--   0        0        0      289 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/.gitignore
--rw-r--r--   0        0        0      168 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/.markdownlint.yaml
--rw-r--r--   0        0        0     1347 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/LICENSE
--rw-r--r--   0        0        0     4284 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/README.md
--rw-r--r--   0        0        0      249 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/codecov.yml
--rw-r--r--   0        0        0     5188 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/docs/changelog.md
--rw-r--r--   0        0        0      830 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/justfile
--rw-r--r--   0        0        0     1014 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/pyproject.toml
--rw-r--r--   0        0        0      112 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/__init__.py
--rw-r--r--   0        0        0      639 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/__init__.py
--rw-r--r--   0        0        0     1498 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/add.py
--rw-r--r--   0        0        0     2251 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/collections.py
--rw-r--r--   0        0        0      941 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/completions.py
--rw-r--r--   0        0        0     1385 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/delete.py
--rw-r--r--   0        0        0     1489 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/drop.py
--rw-r--r--   0        0        0     5333 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/find.py
--rw-r--r--   0        0        0      670 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/hot.py
--rw-r--r--   0        0        0     1490 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/info.py
--rw-r--r--   0        0        0     3644 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/list.py
--rw-r--r--   0        0        0     2394 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/move.py
--rw-r--r--   0        0        0      658 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/new.py
--rw-r--r--   0        0        0     1182 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/open.py
--rw-r--r--   0        0        0     1179 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/rename.py
--rw-r--r--   0        0        0      948 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/search.py
--rw-r--r--   0        0        0     3403 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/stats.py
--rw-r--r--   0        0        0     2640 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/update.py
--rw-r--r--   0        0        0     1153 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/root.py
--rw-r--r--   0        0        0        0 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/type/__init__.py
--rw-r--r--   0        0        0      278 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/type/collection.py
--rw-r--r--   0        0        0     4385 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/type/item.py
--rw-r--r--   0        0        0        0 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/__init__.py
--rw-r--r--   0        0        0     1450 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/api_util.py
--rw-r--r--   0        0        0      697 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/cmd_util.py
--rw-r--r--   0        0        0     2024 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/collection_util.py
--rw-r--r--   0        0        0      235 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/completion_util.py
--rw-r--r--   0        0        0     2596 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/data_util.py
--rw-r--r--   0        0        0      927 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/filter_util.py
--rw-r--r--   0        0        0      617 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/fs_util.py
--rw-r--r--   0        0        0      352 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/input_util.py
--rw-r--r--   0        0        0     3543 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/output_util.py
--rw-r--r--   0        0        0     2616 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/sort_util.py
--rw-r--r--   0        0        0        0 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/tests/__init__.py
--rw-r--r--   0        0        0      313 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/tests/test_root.py
--rw-r--r--   0        0        0        0 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/tests/util/__init__.py
--rw-r--r--   0        0        0     1879 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/tests/util/test_filter_util.py
--rw-r--r--   0        0        0     2188 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/tests/util/test_fs_util.py
--rw-r--r--   0        0        0      565 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/tests/util/test_input_util.py
--rw-r--r--   0        0        0     2274 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/tests/util/test_output_util.py
--rw-r--r--   0        0        0     2525 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/tests/util/test_sort_util.py
--rw-r--r--   0        0        0     5283 1970-01-01 00:00:00.000000 meeple-cli-0.1.0b6/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/.flake8
+-rw-r--r--   0        0        0     1090 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1279 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0      289 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/.gitignore
+-rw-r--r--   0        0        0      168 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/.markdownlint.yaml
+-rw-r--r--   0        0        0     1347 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/LICENSE
+-rw-r--r--   0        0        0     4265 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/README.md
+-rw-r--r--   0        0        0      249 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/codecov.yml
+-rw-r--r--   0        0        0     7025 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/docs/changelog.md
+-rw-r--r--   0        0        0      838 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/justfile
+-rw-r--r--   0        0        0     1014 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/src/meeple/__init__.py
+-rw-r--r--   0        0        0      639 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/src/meeple/command/__init__.py
+-rw-r--r--   0        0        0     2118 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/src/meeple/command/add.py
+-rw-r--r--   0        0        0     2676 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/src/meeple/command/collections.py
+-rw-r--r--   0        0        0      955 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/src/meeple/command/completions.py
+-rw-r--r--   0        0        0     1502 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/src/meeple/command/delete.py
+-rw-r--r--   0        0        0     2138 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/src/meeple/command/drop.py
+-rw-r--r--   0        0        0     5843 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/src/meeple/command/find.py
+-rw-r--r--   0        0        0      670 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/src/meeple/command/hot.py
+-rw-r--r--   0        0        0     1528 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/src/meeple/command/info.py
+-rw-r--r--   0        0        0     3973 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/src/meeple/command/list.py
+-rw-r--r--   0        0        0     3257 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/src/meeple/command/move.py
+-rw-r--r--   0        0        0      765 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/src/meeple/command/new.py
+-rw-r--r--   0        0        0     1271 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/src/meeple/command/open.py
+-rw-r--r--   0        0        0     1361 2023-05-11 01:15:51.812237 meeple-cli-0.1.0b7/src/meeple/command/rename.py
+-rw-r--r--   0        0        0     1250 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/command/search.py
+-rw-r--r--   0        0        0     3944 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/command/stats.py
+-rw-r--r--   0        0        0     3893 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/command/update.py
+-rw-r--r--   0        0        0     1153 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/root.py
+-rw-r--r--   0        0        0        0 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/type/__init__.py
+-rw-r--r--   0        0        0      278 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/type/collection.py
+-rw-r--r--   0        0        0     4385 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/type/item.py
+-rw-r--r--   0        0        0        0 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/util/__init__.py
+-rw-r--r--   0        0        0     1450 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/util/api_util.py
+-rw-r--r--   0        0        0      697 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/util/cmd_util.py
+-rw-r--r--   0        0        0     3229 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/util/collection_util.py
+-rw-r--r--   0        0        0      235 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/util/completion_util.py
+-rw-r--r--   0        0        0     2486 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/util/data_util.py
+-rw-r--r--   0        0        0      927 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/util/filter_util.py
+-rw-r--r--   0        0        0      617 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/util/fs_util.py
+-rw-r--r--   0        0        0      320 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/util/input_util.py
+-rw-r--r--   0        0        0     4025 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/util/output_util.py
+-rw-r--r--   0        0        0     2616 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/src/meeple/util/sort_util.py
+-rw-r--r--   0        0        0        0 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/tests/__init__.py
+-rw-r--r--   0        0        0      313 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/tests/test_root.py
+-rw-r--r--   0        0        0        0 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/tests/util/__init__.py
+-rw-r--r--   0        0        0     1879 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/tests/util/test_filter_util.py
+-rw-r--r--   0        0        0     2188 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/tests/util/test_fs_util.py
+-rw-r--r--   0        0        0     2274 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/tests/util/test_output_util.py
+-rw-r--r--   0        0        0     2525 2023-05-11 01:15:51.816237 meeple-cli-0.1.0b7/tests/util/test_sort_util.py
+-rw-r--r--   0        0        0     5264 1970-01-01 00:00:00.000000 meeple-cli-0.1.0b7/PKG-INFO
```

### Comparing `meeple-cli-0.1.0b6/.github/workflows/python-publish.yml` & `meeple-cli-0.1.0b7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b6/.github/workflows/python-test.yml` & `meeple-cli-0.1.0b7/.github/workflows/python-test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
 
 name: Test Python Package
 
 on:
   push:
   pull_request:
-    branches: ["main", "develop"]
+    branches: ["main"]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
```

### Comparing `meeple-cli-0.1.0b6/.pre-commit-config.yaml` & `meeple-cli-0.1.0b7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b6/LICENSE` & `meeple-cli-0.1.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b6/README.md` & `meeple-cli-0.1.0b7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,33 +12,33 @@
 [BoardGameGeek](https://boardgamegeek.com).**
 
 > Disclaimer: Neither `meeple-cli` nor its maintainers are affiliated with
 > [BoardGameGeek](https://boardgamegeek.com).
 
 ## Install
 
-Global isolated install via [pipx](https://pypa.github.io/pipx/) (recommended):
+Via [Homebrew](https://brew.sh) (Recommended on macOS/Linux)
+
+```zsh
+brew tap boldandbrad/tap
+brew install meeple-cli
+```
+
+Via [pipx](https://pypa.github.io/pipx/) (Recommended on Windows):
 
 ```sh
 pipx install meeple-cli
 ```
 
-Local python environment install:
+Via `pip`:
 
 ```sh
 pip install meeple-cli
 ```
 
-<!-- Homebrew install: -->
-
-<!-- ```zsh
-brew tap boldandbrad/homebrew-tap
-brew install meeple-cli
-```-->
-
 <!-- > For more details, read the **meeple-cli**
 > [install guide](https://boldandbrad.github.io/meeple-cli/#/install). -->
 
 ## Usage
 
 ```txt
 $ meeple --help
```

### Comparing `meeple-cli-0.1.0b6/docs/changelog.md` & `meeple-cli-0.1.0b7/docs/changelog.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,53 @@
 The format is based on
 [Keep a Changelog](https://keepachangelog.com/en/1.1.0/ "Keep a Changelog"),
 and this project adheres to
 [Semantic Versioning](https://semver.org/spec/v2.0.0.html "Semantic Versioning").
 
 ## [Unreleased]
 
+## [v0.1.0b7] - 2023-05-10
+
+### Added
+
+- `meeple add`
+  - Gracefully handle the re-addition of items slated to be dropped.
+  - Recommend `meeple update` in output.
+- `meeple collections` - Show pending changes indicators and warning message.
+- `meeple drop`
+  - Gracefully handle the re-removal of items slated to be added.
+  - Recommend `meeple update` in output.
+- `meeple find`/`meeple list`/`meeple search`/`meeple stats` - Show warning message when no items match provided filters.
+- `meeple move` - Recommend `meeple update` in output.
+- `meeple stats` - Show pending changes warning message.
+- `meeple update`: `-f/--force` - Force update regardless of collection state.
+- `INSTALL` - Install via [Homebrew](https://brew.sh). See project README for details.
+
+### Changed
+
+- `meeple completions` - Simplify output style.
+- `meeple delete`/`meeple open` - Confirmation input must now match `y/Y/n/N` or a re-prompt will occur.
+- `meeple update`
+  - By default, only update collections that are either outdated or have pending changes.
+  - Output is more readable.
+- `GENERAL`
+  - Item names now appear blue and italicized in output messages.
+  - Collection names now appear magenta and underlined in output messages.
+  - Commands now appear green in output messages.
+  - Item Ids and other values now appear yellow in error and warning messages.
+  - Output message ontainer borders now appear dimmer.
+- `DATA`
+  - Update collection yaml file format to accomodate pending changes. (NON-BREAKING - Collection modifying commands such `meeple add/drop/move/update` will automatically convert old files to the new format when possible.)
+
+### Fixed
+
+- `meeple find` - Exit with error when no collections exist to search.
+- `GENERAL` - Properly print out messages as Errors instead of Warnings when the
+  result is a process termination.
+
 ## [v0.1.0b6] - 2023-04-16
 
 ### Added
 
 - `GENERAL` - Sortedby column indicator in sorted output.
 - `meeple list` - _Type_ column included if output contains both boardgames and expansions.
 - `TESTS` - Increase test coverage.
```

### Comparing `meeple-cli-0.1.0b6/justfile` & `meeple-cli-0.1.0b7/justfile`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 # activate venv
 venv:
     . .venv/bin/activate
 
 # install meeple-cli from local
 install:
-    pip install -q .
+    pip install -q ."[test]"
 
 # install meeple-cli via flit
 flit-install:
     pip install flit
     flit install
 
 # install editable
```

### Comparing `meeple-cli-0.1.0b6/pyproject.toml` & `meeple-cli-0.1.0b7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b6/src/meeple/command/__init__.py` & `meeple-cli-0.1.0b7/src/meeple/command/__init__.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b6/src/meeple/command/add.py` & `meeple-cli-0.1.0b7/src/meeple/command/drop.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,34 +12,54 @@
 from meeple.util.output_util import print_error, print_info
 
 
 @click.command()
 @click.argument("collection", shell_complete=complete_collections)
 @click.argument("id", type=int)
 @click.help_option("-h", "--help")
-def add(collection: str, id: int) -> None:
-    """Add an item to a collection.
+def drop(collection: str, id: int) -> None:
+    """Remove an item from a collection.
 
-    - COLLECTION is the name of the intended destination collection.
+    - COLLECTION is the name of the collection to be modified.
 
-    - ID is the BoardGameGeek ID of the board game/expansion to be added.
+    - ID is the BoardGameGeek ID of the board game/expansion to be removed.
     """
     # check that the given id is a valid BoardGameGeek ID
     bgg_id = id
     bgg_item = get_bgg_item(bgg_id)
     if not bgg_item:
-        sys.exit(print_error(f"'{bgg_id}' is not a valid BoardGameGeek ID"))
+        sys.exit(
+            print_error(f"[yellow]{bgg_id}[/yellow] is not a valid BoardGameGeek ID.")
+        )
 
     # check that the given collection is a valid collection
     if not is_collection(collection):
-        sys.exit(print_error(f"'{collection}' is not a valid collection"))
-
-    bgg_ids = read_collection(collection)
-    # check that the given id does not already exist in the given collection
-    if bgg_ids and bgg_id in bgg_ids:
-        sys.exit(print_error(f"'{bgg_id}' already exists in '{collection}'"))
-
-    # add the id to the collection and save
-    bgg_ids.append(bgg_id)
-    bgg_ids.sort()
-    update_collection(collection, bgg_ids)
-    print_info(f"Added '{bgg_item.name}' to '{collection}'")
+        sys.exit(
+            print_error(f"[yellow]{collection}[/yellow] is not a valid collection.")
+        )
+
+    item_ids, to_add_ids, to_drop_ids = read_collection(collection)
+
+    # check if the given id already does not exist in the given collection
+    if (not item_ids or bgg_id not in item_ids) and (
+        not to_add_ids and bgg_id not in to_add_ids
+    ):
+        sys.exit(
+            print_error(
+                f"[i blue]{bgg_item.name}[/i blue] already doesn't exist in [u magenta]{collection}[/u magenta]."
+            )
+        )
+
+    if to_add_ids and bgg_id in to_add_ids:
+        # if the given id is slated to be added, simply undo that
+        to_add_ids.remove(bgg_id)
+    else:
+        # drop the id from the collection as normal
+        item_ids.remove(bgg_id)
+        to_drop_ids.append(bgg_id)
+        to_drop_ids.sort()
+
+    # persist changes
+    update_collection(collection, item_ids, to_add_ids, to_drop_ids)
+    print_info(
+        f"Dropped [i blue]{bgg_item.name}[/i blue] from [u magenta]{collection}[/u magenta]. To update, run: [green]meeple update[/green]"
+    )
```

### Comparing `meeple-cli-0.1.0b6/src/meeple/command/collections.py` & `meeple-cli-0.1.0b7/src/meeple/command/collections.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import sys
 
 import click
 
 from meeple.type.collection import Collection
-from meeple.util.collection_util import get_collections
+from meeple.util.collection_util import get_collections, is_pending_updates
 from meeple.util.data_util import get_collection_data, last_updated
 from meeple.util.output_util import (
     CollectionHeader,
+    fmt_collection_name,
     fmt_headers,
+    print_error,
     print_table,
     print_warning,
 )
 from meeple.util.sort_util import COLLECTION_SORT_KEYS, sort_collections
 
 
 @click.command()
@@ -28,25 +30,28 @@
     """List all collections."""
     # attempt to retrieve collections
     collections = get_collections()
 
     # check that local collections exist
     if not collections:
         sys.exit(
-            print_warning(
-                "No local collections yet exist. Create a new one with `meeple new`"
+            print_error(
+                "No local collections yet exist. To create one, run: [green]meeple new[/green]"
             )
         )
 
     collection_list = []
+    pending_changes = False
     for collection in collections:
         boardgames, expansions = get_collection_data(collection)
         collection_list.append(
             Collection(collection, boardgames, expansions, last_updated(collection))
         )
+        if is_pending_updates(collection):
+            pending_changes = True
 
     # sort output
     collection_list, sort_direction = sort_collections(collection_list, sort)
 
     # prepare table data
     headers = [CollectionHeader.NAME]
     if verbose:
@@ -59,21 +64,27 @@
         )
 
     # format headers
     headers = fmt_headers(headers, sort, sort_direction)
 
     rows = []
     for collection in collection_list:
-        cols = [collection.name]
+        cols = [fmt_collection_name(collection.name)]
         # include additional data if the user chose verbose output
         if verbose:
             cols.extend(
                 [
                     str(len(collection.boardgames)),
                     str(len(collection.expansions)),
                     collection.last_updated,
                 ]
             )
 
         rows.append(cols)
 
+    # print warning if some collections need to be updated
+    if pending_changes:
+        print_warning(
+            "Some collections ([red]*[/red]) are pending changes. To apply, run [green]meeple update[/green]"
+        )
+
     print_table(rows, headers)
```

### Comparing `meeple-cli-0.1.0b6/src/meeple/command/completions.py` & `meeple-cli-0.1.0b7/src/meeple/command/completions.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,19 +11,18 @@
 def completions(shell: str) -> None:
     """Setup meeple shell completions.
 
     - SHELL is the shell for which to setup completions.
     """
     match shell.lower():
         case "bash":
-            print_info("Add this to ~/.bashrc:")
-            print('\teval "$(_MEEPLE_COMPLETE=bash_source meeple)"')
+            print_info(
+                'To install completions, add this to ~/.bashrc: [green]eval "$(_MEEPLE_COMPLETE=bash_source meeple)"[/green]'
+            )
         case "zsh":
-            print_info("Add this to ~/.zshrc:")
-            print('\teval "$(_MEEPLE_COMPLETE=zsh_source meeple)"')
-        case "fish":
             print_info(
-                "Save the following script to ~/.config/fish/completions/meeple.fish:"
+                'To install completions, add this to ~/.zshrc: [green]eval "$(_MEEPLE_COMPLETE=zsh_source meeple)"[/green]'
             )
-            print(
-                "\t_MEEPLE_COMPLETE=fish_source meeple > ~/.config/fish/completions/meeple.fish"
+        case "fish":
+            print_info(
+                "To install completions, run: [green]_MEEPLE_COMPLETE=fish_source meeple > ~/.config/fish/completions/meeple.fish[/green]"
             )
```

### Comparing `meeple-cli-0.1.0b6/src/meeple/command/delete.py` & `meeple-cli-0.1.0b7/src/meeple/command/delete.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,26 @@
 def delete(collection: str, yes: bool) -> None:
     """Delete a collection.
 
     - COLLECTION is the name of the collection to be deleted.
     """
     # check that the given collection exists
     if not is_collection(collection):
-        sys.exit(print_error(f"'{collection}' already does not exist"))
+        sys.exit(
+            print_error(f"[yellow]{collection}[/yellow] is not a valid collection.")
+        )
 
     # ask for confirmation or not depending on presence of flag
     if not yes:
-        confirmation = bool_input(f"Are you sure you want to delete '{collection}'?")
+        confirmation = bool_input(
+            f"Are you sure you want to delete collection [u magenta]{collection}[/u magenta]?"
+        )
     else:
         confirmation = True
 
     # delete collection and its data if confirmation succeeded
     if confirmation:
         delete_collection(collection)
         boardgames, expansions = get_collection_data(collection)
         if boardgames or expansions:
             delete_collection_data(collection)
-        print_info(f"Deleted collection '{collection}'")
+        print_info(f"Deleted collection [u magenta]{collection}[/u magenta].")
```

### Comparing `meeple-cli-0.1.0b6/src/meeple/command/drop.py` & `meeple-cli-0.1.0b7/src/meeple/command/add.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,33 +12,53 @@
 from meeple.util.output_util import print_error, print_info
 
 
 @click.command()
 @click.argument("collection", shell_complete=complete_collections)
 @click.argument("id", type=int)
 @click.help_option("-h", "--help")
-def drop(collection: str, id: int) -> None:
-    """Remove an item from a collection.
+def add(collection: str, id: int) -> None:
+    """Add an item to a collection.
 
-    - COLLECTION is the name of the collection to be modified.
+    - COLLECTION is the name of the intended destination collection.
 
-    - ID is the BoardGameGeek ID of the board game/expansion to be removed.
+    - ID is the BoardGameGeek ID of the board game/expansion to be added.
     """
     # check that the given id is a valid BoardGameGeek ID
     bgg_id = id
     bgg_item = get_bgg_item(bgg_id)
     if not bgg_item:
-        sys.exit(print_error(f"'{bgg_id}' is not a valid BoardGameGeek ID"))
+        sys.exit(
+            print_error(f"[yellow]{bgg_id}[/yellow] is not a valid BoardGameGeek ID.")
+        )
 
     # check that the given collection is a valid collection
     if not is_collection(collection):
-        sys.exit(print_error(f"'{collection}' is not a valid collection"))
-
-    bgg_ids = read_collection(collection)
-    # check that the given id already does not exist in the given collection
-    if bgg_id not in bgg_ids:
-        sys.exit(print_error(f"'{bgg_id}' already doesn't exist in '{collection}'"))
-
-    # remove the id from the collection and save
-    bgg_ids.remove(bgg_id)
-    update_collection(collection, bgg_ids)
-    print_info(f"Dropped '{bgg_item.name}' from '{collection}'")
+        sys.exit(
+            print_error(f"[yellow]{collection}[/yellow] is not a valid collection.")
+        )
+
+    item_ids, to_add_ids, to_drop_ids = read_collection(collection)
+
+    # check if the given id already exists in the given collection
+    if (item_ids and bgg_id in item_ids) or (to_add_ids and bgg_id in to_add_ids):
+        sys.exit(
+            print_error(
+                f"[i blue]{bgg_item.name}[/i blue] already exists in collection [u magenta]{collection}[/u magenta]."
+            )
+        )
+
+    if to_drop_ids and bgg_id in to_drop_ids:
+        # if the given id is slated to be dropped, simply undo that
+        to_drop_ids.remove(bgg_id)
+        item_ids.append(bgg_id)
+        item_ids.sort()
+    else:
+        # otherwise, add the id to the collection as normal
+        to_add_ids.append(bgg_id)
+        to_add_ids.sort()
+
+    # persist changes
+    update_collection(collection, item_ids, to_add_ids, to_drop_ids)
+    print_info(
+        f"Added [i blue]{bgg_item.name}[/i blue]' to [u]{collection}[/u]. To update, run: [green]meeple update[/green]"
+    )
```

### Comparing `meeple-cli-0.1.0b6/src/meeple/command/find.py` & `meeple-cli-0.1.0b7/src/meeple/command/find.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     fmt_rank,
     fmt_rating,
     fmt_type,
     fmt_weight,
     fmt_year,
     print_error,
     print_table,
+    print_warning,
 )
 from meeple.util.sort_util import ITEM_SORT_KEYS, sort_items
 
 
 @click.command()
 @click.argument("collections", nargs=-1, shell_complete=complete_collections)
 @click.option(
@@ -82,14 +83,22 @@
     if not are_collections(collections):
         sys.exit(print_error("Not all provided collections are valid collections."))
 
     # if no collections provided, default to all local collections
     if not collections:
         collections = get_collections()
 
+    # check that local collections exist
+    if not collections:
+        sys.exit(
+            print_error(
+                "No local collections yet exist. To create one, run: [green]meeple new[/green]"
+            )
+        )
+
     # get collection items
     result_items = []
     collection_list = []
     for collection in collections:
         boardgames, expansions = get_collection_data(collection)
         collection_list.append(Collection(collection, boardgames, expansions, None))
 
@@ -108,14 +117,22 @@
     if players:
         result_items = filterby_players(result_items, players)
     if max_time:
         result_items = filterby_playtime(result_items, max_time)
     if weight:
         result_items = filterby_weight(result_items, weight)
 
+    # check that data exists after applied filters
+    if not result_items:
+        sys.exit(
+            print_warning(
+                f"No items found matching provided filters for collection(s) [u magenta]{collections}[/u magenta]."
+            )
+        )
+
     # sort output
     result_items, sort_direction = sort_items(result_items, sort)
 
     # prepare table headers
     headers = [ItemHeader.ID, ItemHeader.NAME]
     # include type column if neither type is ommitted
     if item_type not in ("bg", "ex"):
```

### Comparing `meeple-cli-0.1.0b6/src/meeple/command/hot.py` & `meeple-cli-0.1.0b7/src/meeple/command/hot.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b6/src/meeple/command/info.py` & `meeple-cli-0.1.0b7/src/meeple/command/info.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 
     - ID is the BoardGameGeek ID of the board game/expansion to be detailed.
     """
     # check that the given id is a valid one
     bgg_id = id
     bgg_item = get_bgg_item(bgg_id)
     if not bgg_item:
-        sys.exit(print_error(f"'{bgg_id}' is not a valid BoardGameGeek ID"))
+        sys.exit(
+            print_error(f"[yellow]{bgg_id}[/yellow] is not a valid BoardGameGeek ID.")
+        )
 
     info_rows = [
         [
             f"Rating: {fmt_rating(bgg_item.rating)}",
             f"Players: {fmt_players(bgg_item.minplayers, bgg_item.maxplayers)}",
             f"Min Age: {bgg_item.minage}",
         ],
```

### Comparing `meeple-cli-0.1.0b6/src/meeple/command/list.py` & `meeple-cli-0.1.0b7/src/meeple/command/list.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,34 +53,45 @@
 def list_collection(collection: str, item_type: str, sort: str, verbose: bool) -> None:
     """List contents of a collection.
 
     - COLLECTION is the name of the collection to be listed.
     """
     # check that the given collection is a valid collection
     if not is_collection(collection):
-        sys.exit(print_error(f"'{collection}' is not a valid collection"))
+        sys.exit(
+            print_error(f"[yellow]{collection}[/yellow] is not a valid collection.")
+        )
 
     boardgames, expansions = get_collection_data(collection)
+
     # check that local data exists for the given collection
-    # TODO: add error/better handling for when a collection has no data files and/or is empty?
+    # TODO: add better error handling for when a collection has no data files and/or is empty?
     if not boardgames and not expansions:
         sys.exit(
-            print_warning(
-                f"local data not found for '{collection}'. update with `meeple update {collection}`"
+            print_error(
+                f"Local data not found for [u magenta]{collection}[/u magenta]. To update, run: [green]meeple update {collection}[/green]"
             )
         )
 
     # determine what to include in results depending on given flags
     if item_type == "bg":
         out_list = boardgames
     elif item_type == "ex":
         out_list = expansions
     else:
         out_list = boardgames + expansions
 
+    # check that data exists after applied filters
+    if not out_list:
+        sys.exit(
+            print_warning(
+                f"No items found matching provided filters for collection [u magenta]{collection}[/u magenta]."
+            )
+        )
+
     # sort output
     out_list, sort_direction = sort_items(out_list, sort)
 
     # prepare table data
     headers = [ItemHeader.ID, ItemHeader.NAME]
     # include type column if neither type is ommitted
     if item_type not in ("bg", "ex"):
```

### Comparing `meeple-cli-0.1.0b6/src/meeple/command/move.py` & `meeple-cli-0.1.0b7/src/meeple/command/move.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,41 +26,64 @@
 
     - ID is the BoardGameGeek ID of the board game/expansion to be moved.
     """
     # check that the given id is a valid BoardGameGeek ID
     bgg_id = id
     bgg_item = get_bgg_item(bgg_id)
     if not bgg_item:
-        sys.exit(print_error(f"'{bgg_id}' is not a valid BoardGameGeek ID"))
+        sys.exit(
+            print_error(f"[yellow]{bgg_id}[/yellow] is not a valid BoardGameGeek ID.")
+        )
 
     # check that the given collection is a valid collection
     if not is_collection(from_collection):
-        sys.exit(print_error(f"'{from_collection}' is not a valid collection"))
+        sys.exit(
+            print_error(
+                f"[yellow]{from_collection}[/yellow] is not a valid collection."
+            )
+        )
+
+    from_item_ids, from_to_add_ids, from_to_drop_ids = read_collection(from_collection)
 
     # check that the given collection is a valid collection
     if not is_collection(to_collection):
         # TODO: offer to create the new collection
-        sys.exit(print_error(f"'{to_collection}' is not a valid collection"))
+        sys.exit(
+            print_error(f"[yellow]{to_collection}[/yellow] is not a valid collection.")
+        )
+
+    dest_item_ids, dest_to_add_ids, dest_to_drop_ids = read_collection(to_collection)
+
+    # check that the id exists in from collection
+    # TODO: check the from collection to_add list and to_drop list
+    if bgg_id not in from_item_ids:
+        # TODO: ask if they want to add it to the destination collection anyway
+        sys.exit(
+            print_error(
+                f"[i blue]{bgg_item.name}[/i blue] already doesn't exist in [u magenta]{from_collection}[/u magenta]."
+            )
+        )
 
-    # TODO: refactor to avoid the following duplicated code
-    # remove the id from the source collection
-    from_bgg_ids = read_collection(from_collection)
-    if bgg_id not in from_bgg_ids:
-        # TODO: ask if they want to add it to the to collection anyway
+    # check that the id doesn't exist in dest collection
+    # TODO: check the dest collection to_add list and to_drop list
+    if dest_item_ids and bgg_id in dest_item_ids:
         sys.exit(
-            print_error(f"'{bgg_id}' already doesn't exist in '{from_collection}'")
+            print_error(
+                f"[i blue]{bgg_item.name}[/i blue] already exists in collection [u magenta]{to_collection}[/u magenta]."
+            )
         )
 
-    from_bgg_ids.remove(bgg_id)
+    # drop the id from the from collection
+    from_item_ids.remove(bgg_id)
+    from_to_drop_ids.append(bgg_id)
+    from_to_drop_ids.sort()
 
     # add the id to the destination collection
-    to_bgg_ids = read_collection(to_collection)
-    if to_bgg_ids and bgg_id in to_bgg_ids:
-        sys.exit(print_error(f"'{bgg_id}' already exists in '{to_collection}'"))
-
-    to_bgg_ids.append(bgg_id)
-    to_bgg_ids.sort()
-
-    # save changes
-    update_collection(from_collection, from_bgg_ids)
-    update_collection(to_collection, to_bgg_ids)
-    print_info(f"Moved '{bgg_item.name}' from '{from_collection}' to '{to_collection}'")
+    dest_to_add_ids.append(bgg_id)
+    dest_to_add_ids.sort()
+
+    # persist changes
+    update_collection(from_collection, from_item_ids, from_to_add_ids, from_to_drop_ids)
+    update_collection(to_collection, dest_item_ids, dest_to_add_ids, dest_to_drop_ids)
+    print_info(
+        f"Moved [i blue]{bgg_item.name}[/i blue] from [u magenta]{from_collection}[/u magenta] to [u magenta]{to_collection}[/u magenta]. To update, run: [green]meeple update[/green]"
+    )
```

### Comparing `meeple-cli-0.1.0b6/src/meeple/command/new.py` & `meeple-cli-0.1.0b7/src/meeple/command/new.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,12 +12,16 @@
 def new(collection: str) -> None:
     """Create a new collection.
 
     - COLLECTION is the name of the collection to be created.
     """
     # check that the given collection doesn't already exist
     if is_collection(collection):
-        sys.exit(print_error(f"'{collection}' already exists"))
+        sys.exit(
+            print_error(
+                f"Collection [u magenta]{collection}[/u magenta] already exists."
+            )
+        )
 
     # create new collection
     create_collection(collection)
-    print_info(f"Created new collection '{collection}'")
+    print_info(f"Created new collection [u magenta]{collection}[/u magenta].")
```

### Comparing `meeple-cli-0.1.0b6/src/meeple/command/open.py` & `meeple-cli-0.1.0b7/src/meeple/command/open.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import webbrowser
 
 import click
 
 from meeple.util.api_util import BGG_DOMAIN, get_bgg_items
 from meeple.util.input_util import bool_input
-from meeple.util.output_util import print_error, print_info
+from meeple.util.output_util import print_error, print_info, printf
 
 
 @click.command(name="open")
 @click.argument("id", type=int)
 @click.option("-y", "--yes", is_flag=True, help="Bypass confirmation.")
 @click.help_option("-h", "--help")
 def open_on_bgg(id: int, yes: bool) -> None:
@@ -17,18 +17,20 @@
 
     - ID is the BoardGameGeek ID of the board game/expansion to be opened on boardgamegeek.com.
     """
     # check that the given id is a valid BoardGameGeek ID
     bgg_id = id
     api_result = get_bgg_items([bgg_id])
     if not api_result:
-        sys.exit(print_error(f"Provided '{bgg_id}' is not a valid BoardGameGeek ID"))
+        sys.exit(
+            print_error(f"[yellow]{bgg_id}[/yellow] is not a valid BoardGameGeek ID.")
+        )
 
     # confirm the user wants to open the board game/expansion on BoardGameGeek website
     item = api_result[0]
     url = f"https://{BGG_DOMAIN}/{item.type}/{bgg_id}"
     name = item.name
-    if yes or bool_input(f"Open '{name}' on {BGG_DOMAIN}?"):
-        print(f"\tOpening '{name}' on {BGG_DOMAIN} ...")
+    if yes or bool_input(f"Open [i blue]{name}[/i blue] on {BGG_DOMAIN}?"):
+        printf(f" ╰╴ Opening [i blue]{name}[/i blue] on {BGG_DOMAIN} ...")
         webbrowser.open(url)
     else:
-        print_info(f"View '{name}' at {url}")
+        print_info(f"View [i blue]{name}[/i blue] at {url}")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `meeple-cli-0.1.0b6/src/meeple/command/rename.py` & `meeple-cli-0.1.0b7/src/meeple/command/rename.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,17 +16,25 @@
     """Rename a local collection.
 
     - COLLECTION is the name of the collection to be renamed.
     - NEW_NAME is the new name to assign to the collection.
     """
     # check that the given collection is a valid collection
     if not is_collection(collection):
-        sys.exit(print_error(f"'{collection}' is not a valid collection"))
+        sys.exit(
+            print_error(f"[yellow]{collection}[/yellow] is not a valid collection.")
+        )
 
     # check that the given collection new name doesn't already exist
     if is_collection(new_name):
-        sys.exit(print_error(f"'{new_name}' already exists"))
+        sys.exit(
+            print_error(
+                f"Collection [u magenta]{collection}[/u magenta] already exists."
+            )
+        )
 
     # create new collection
     rename_collection(collection, new_name)
     rename_collection_data_dir(collection, new_name)
-    print_info(f"Renamed collection '{collection}' to '{new_name}'")
+    print_info(
+        f"Renamed collection [u magenta]{collection}[/u magenta] to [u magenta]{new_name}[/u magenta]."
+    )
```

### Comparing `meeple-cli-0.1.0b6/src/meeple/command/search.py` & `meeple-cli-0.1.0b7/src/meeple/command/search.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,48 @@
+import sys
+
 import click
 
 from meeple.util.api_util import search_bgg
-from meeple.util.output_util import ItemHeader, fmt_headers, fmt_year, print_table
+from meeple.util.output_util import (
+    ItemHeader,
+    fmt_headers,
+    fmt_year,
+    print_table,
+    print_warning,
+)
 
 
 @click.command()
 @click.argument("query")
 @click.help_option("-h", "--help")
 def search(query: str) -> None:
     """Search BoardGameGeek for items.
 
     - QUERY is the text to be searched for on BoardGameGeek. If searching multiple words, surround with quotes.
     """
     # search BoardGameGeek with user provided query
-    api_result = search_bgg(query)
-    api_result.sort(key=lambda x: x.id)
+    result_items = search_bgg(query)
+
+    # check that data exists after applied filters
+    if not result_items:
+        sys.exit(
+            print_warning(
+                f"No items found on BoardGameGeek matching search term [i blue]{query}[i blue]."
+            )
+        )
+
+    result_items.sort(key=lambda x: x.id)
 
     # prepare table data
     headers = [ItemHeader.ID, ItemHeader.NAME, ItemHeader.YEAR]
     headers = fmt_headers(headers, None, None)
 
     rows = []
-    for item in api_result:
+    for item in result_items:
         cols = []
         cols.extend(
             [
                 str(item.id),
                 item.name,
                 fmt_year(item.year),
             ]
```

### Comparing `meeple-cli-0.1.0b6/src/meeple/root.py` & `meeple-cli-0.1.0b7/src/meeple/root.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b6/src/meeple/type/item.py` & `meeple-cli-0.1.0b7/src/meeple/type/item.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b6/src/meeple/util/api_util.py` & `meeple-cli-0.1.0b7/src/meeple/util/api_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b6/src/meeple/util/cmd_util.py` & `meeple-cli-0.1.0b7/src/meeple/util/cmd_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b6/src/meeple/util/collection_util.py` & `meeple-cli-0.1.0b7/src/meeple/util/collection_util.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,72 +3,110 @@
 from pathlib import Path
 from typing import List
 
 import yaml
 
 from meeple.util.fs_util import get_collection_dir
 
-IN_PATH = get_collection_dir()
-ID_LIST_KEY = "bgg-ids"
+COLLECTION_DIR = get_collection_dir()
+
+_ITEM_LIST_KEY = "items"
+_OLD_ITEM_LIST_KEY = "bgg-ids"  # TODO: eventually remove
+_TO_ADD_LIST_KEY = "to_add"
+_TO_DROP_LIST_KEY = "to_drop"
 
 
 def _collection_file(collection_name: str) -> str:
-    return join(IN_PATH, f"{collection_name}.yml")
+    return join(COLLECTION_DIR, f"{collection_name}.yml")
+
+
+def _get_ids(data: dict, list_key: str) -> List[int]:
+    if list_key in data:
+        ids = data[list_key]
+        if not ids:
+            return []
+    # remove non int values from list
+    for bgg_id in ids:
+        if not isinstance(bgg_id, int):
+            ids.remove(bgg_id)
+    return ids
 
 
 def get_collections() -> List[str]:
     # create in_path dir and exit if it does not exist
-    if not Path(IN_PATH).exists():
-        Path(IN_PATH).mkdir(parents=True)
+    if not Path(COLLECTION_DIR).exists():
+        Path(COLLECTION_DIR).mkdir(parents=True)
 
     # retrieve collection source files from in_path
-    collection_files = next(walk(IN_PATH))[2]
+    collection_files = next(walk(COLLECTION_DIR))[2]
     collections = []
     for collection_file in collection_files:
         collection, ext = splitext(collection_file)
         if ext == ".yml":
             collections.append(collection)
     return collections
 
 
 def is_collection(name: str) -> bool:
     return name in get_collections()
 
 
+def is_pending_updates(name: str) -> bool:
+    _, to_add_ids, to_drop_ids = read_collection(name)
+    return len(to_add_ids) > 0 or len(to_drop_ids) > 0
+
+
 def are_collections(names: [str]) -> bool:
     return set(names) <= set(get_collections())
 
 
-def read_collection(name: str) -> List[int]:
+def read_collection(name: str) -> (List[int], List[int], List[int]):
     with open(_collection_file(name), "r") as f:
         data = yaml.load(f, Loader=yaml.FullLoader)
-        if data and ID_LIST_KEY in data:
-            bgg_ids = data[ID_LIST_KEY]
+
+        # check if data is in old format
+        # TODO: eventually remove
+        if data and _OLD_ITEM_LIST_KEY in data:
+            bgg_ids = data[_OLD_ITEM_LIST_KEY]
             if not bgg_ids:
-                return []
+                return [], [], []
 
             # remove non int values from list
             for bgg_id in bgg_ids:
                 if not isinstance(bgg_id, int):
                     bgg_ids.remove(bgg_id)
-            return bgg_ids
-        return []
+            return bgg_ids, [], []
+
+        if data:
+            return (
+                _get_ids(data, _ITEM_LIST_KEY),
+                _get_ids(data, _TO_ADD_LIST_KEY),
+                _get_ids(data, _TO_DROP_LIST_KEY),
+            )
+        return [], [], []
 
 
 def create_collection(name: str) -> None:
-    data = {ID_LIST_KEY: []}
+    # TODO: create a class for this Collection object
+    data = {_ITEM_LIST_KEY: [], _TO_ADD_LIST_KEY: [], _TO_DROP_LIST_KEY: []}
     with open(_collection_file(name), "w") as f:
         yaml.dump(data, f)
 
 
-def update_collection(name: str, ids: list) -> None:
-    data = {ID_LIST_KEY: ids}
+def update_collection(
+    name: str, item_ids: list, to_add_ids: list, to_drop_ids: list
+) -> None:
+    data = {
+        _ITEM_LIST_KEY: item_ids,
+        _TO_ADD_LIST_KEY: to_add_ids,
+        _TO_DROP_LIST_KEY: to_drop_ids,
+    }
     with open(_collection_file(name), "w") as f:
         yaml.dump(data, f)
 
 
 def rename_collection(current_name: str, new_name: str) -> None:
-    Path(_collection_file(current_name)).rename(join(IN_PATH, f"{new_name}.yml"))
+    Path(_collection_file(current_name)).rename(join(COLLECTION_DIR, f"{new_name}.yml"))
 
 
 def delete_collection(name: str) -> None:
     Path(_collection_file(name)).unlink()
```

### Comparing `meeple-cli-0.1.0b6/src/meeple/util/data_util.py` & `meeple-cli-0.1.0b7/src/meeple/util/data_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from os.path import basename, join, splitext
 from pathlib import Path
 from typing import List
 
 from meeple.type.item import Item
 from meeple.util.fs_util import get_data_dir
 
-OUT_PATH = get_data_dir()
+DATA_DIR = get_data_dir()
 
 
 def _collection_data_dir(collection_name: str) -> str:
-    return join(OUT_PATH, collection_name)
+    return join(DATA_DIR, collection_name)
 
 
 def _latest_data_file(collection_name: str) -> str:
     # find latest data dump file path for collection
     data_dir = _collection_data_dir(collection_name)
     if not Path(data_dir).exists():
         return None
@@ -27,15 +27,15 @@
     latest_data_files = next(walk(latest_month_dir))[2]
     latest_data_files.sort()
     return join(latest_month_dir, latest_data_files[-1])
 
 
 def rename_collection_data_dir(current_name: str, new_name: str) -> None:
     if Path(_collection_data_dir(current_name)).exists():
-        rename(_collection_data_dir(current_name), join(OUT_PATH, new_name))
+        rename(_collection_data_dir(current_name), join(DATA_DIR, new_name))
 
 
 def last_updated(collection_name: str) -> str:
     latest_data_file = _latest_data_file(collection_name)
     if not latest_data_file:
         return "NA"
     date = splitext(basename(latest_data_file))[0]
@@ -68,13 +68,11 @@
 
     # create out dirs if they do not exist
     if not Path(data_path).exists():
         Path(data_path).mkdir(parents=True)
 
     with open(join(data_path, filename), "w") as f:
         json.dump(result, f, indent=4, ensure_ascii=False)
-    # TODO: find a more elegant way to print this out
-    print(f"\tUpdated collection '{collection_name}'.")
 
 
 def delete_collection_data(collection_name: str) -> None:
     shutil.rmtree(_collection_data_dir(collection_name))
```

### Comparing `meeple-cli-0.1.0b6/src/meeple/util/filter_util.py` & `meeple-cli-0.1.0b7/src/meeple/util/filter_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b6/src/meeple/util/fs_util.py` & `meeple-cli-0.1.0b7/src/meeple/util/fs_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b6/src/meeple/util/output_util.py` & `meeple-cli-0.1.0b7/src/meeple/util/output_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from enum import Enum
 
 from rich import box
 from rich.console import Console
 from rich.table import Table
 
 from meeple.util.api_util import BOARDGAME_TYPE, EXPANSION_TYPE
+from meeple.util.collection_util import is_pending_updates
 
 NA_VALUE = "[bright_black]NA[/bright_black]"
 
 SORT_ASC_SYMBOL = "[blue]˄[/blue]"
 SORT_DESC_SYMBOL = "[blue]˅[/blue]"
 
 
@@ -30,14 +31,20 @@
 class CollectionHeader(Enum):
     NAME = ("Name", "name")
     BOARDGAMES = ("Boardgames", "boardgames")
     EXPANSIONS = ("Expansions", "expansions")
     UPDATED = ("Last Updated", "updated")
 
 
+def fmt_collection_name(name: str) -> str:
+    if is_pending_updates(name):
+        return f"{name} ([red]*[/red])"
+    return name
+
+
 def fmt_headers(headers: ItemHeader, sort_key: str, sort_direction: str):
     header_strs = []
     for header in headers:
         if sort_key and header.value[1] == sort_key:
             header_strs.append(f"{header.value[0]} {sort_direction}")
             continue
         header_strs.append(header.value[0])
@@ -106,37 +113,50 @@
 
 def fmt_year(year: str) -> str:
     if int(year) == 0:
         return NA_VALUE
     return year
 
 
+def printf(message: str) -> None:
+    console = Console()
+    console.print(message)
+
+
 def print_error(message: str) -> None:
-    print_table([["[red]Error[/red]", message]])
+    print_table([["[red]Error[/red]", message]], dim_border=True)
 
 
 def print_info(message: str) -> None:
-    print_table([[message]])
+    print_table([[message]], dim_border=True)
 
 
 def print_warning(message: str) -> None:
-    print_table([["[yellow]Warning[/yellow]", message]])
+    print_table([["[yellow]Warning[/yellow]", message]], dim_border=True)
 
 
 def print_table(
-    rows: list, headers: list = [], lines: bool = False, zebra: bool = False
+    rows: list,
+    headers: list = [],
+    lines: bool = False,
+    dim_border: bool = False,
+    zebra: bool = False,
 ) -> None:
     row_styles = []
+    border_styles = []
     if zebra:
         row_styles = ["", "dim"]
+    if dim_border:
+        border_styles = "dim"
     table = Table(
         box=box.ROUNDED,
         show_header=(len(headers) != 0),
         show_lines=lines,
         row_styles=row_styles,
+        border_style=border_styles,
     )
     for header in headers:
         table.add_column(header)
     for row in rows:
         table.add_row(*row)
     console = Console()
     console.print(table)
```

### Comparing `meeple-cli-0.1.0b6/src/meeple/util/sort_util.py` & `meeple-cli-0.1.0b7/src/meeple/util/sort_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b6/tests/util/test_filter_util.py` & `meeple-cli-0.1.0b7/tests/util/test_filter_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b6/tests/util/test_fs_util.py` & `meeple-cli-0.1.0b7/tests/util/test_fs_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b6/tests/util/test_output_util.py` & `meeple-cli-0.1.0b7/tests/util/test_output_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b6/tests/util/test_sort_util.py` & `meeple-cli-0.1.0b7/tests/util/test_sort_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b6/PKG-INFO` & `meeple-cli-0.1.0b7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meeple-cli
-Version: 0.1.0b6
+Version: 0.1.0b7
 Summary: Local board game collection manager. Powered by BoardGameGeek.
 Author-email: Bradley Wojcik <bradleycwojcik@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: click >=8
 Requires-Dist: rich >=13
@@ -40,33 +40,33 @@
 [BoardGameGeek](https://boardgamegeek.com).**
 
 > Disclaimer: Neither `meeple-cli` nor its maintainers are affiliated with
 > [BoardGameGeek](https://boardgamegeek.com).
 
 ## Install
 
-Global isolated install via [pipx](https://pypa.github.io/pipx/) (recommended):
+Via [Homebrew](https://brew.sh) (Recommended on macOS/Linux)
+
+```zsh
+brew tap boldandbrad/tap
+brew install meeple-cli
+```
+
+Via [pipx](https://pypa.github.io/pipx/) (Recommended on Windows):
 
 ```sh
 pipx install meeple-cli
 ```
 
-Local python environment install:
+Via `pip`:
 
 ```sh
 pip install meeple-cli
 ```
 
-<!-- Homebrew install: -->
-
-<!-- ```zsh
-brew tap boldandbrad/homebrew-tap
-brew install meeple-cli
-```-->
-
 <!-- > For more details, read the **meeple-cli**
 > [install guide](https://boldandbrad.github.io/meeple-cli/#/install). -->
 
 ## Usage
 
 ```txt
 $ meeple --help
```

