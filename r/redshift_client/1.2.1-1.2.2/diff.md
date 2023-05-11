# Comparing `tmp/redshift_client-1.2.1.tar.gz` & `tmp/redshift_client-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redshift_client-1.2.1.tar", last modified: Tue Jan  1 00:00:00 1980, max compression
+gzip compressed data, was "redshift_client-1.2.2.tar", last modified: Tue Jan  1 00:00:00 1980, max compression
```

## Comparing `redshift_client-1.2.1.tar` & `redshift_client-1.2.2.tar`

### file list

```diff
@@ -1,49 +1,55 @@
--rw-r--r--   0        0        0       81 1980-01-01 00:00:00.000000 redshift_client-1.2.1/.envrc
--rw-r--r--   0        0        0       47 1980-01-01 00:00:00.000000 redshift_client-1.2.1/.gitignore
--rw-r--r--   0        0        0     2105 1980-01-01 00:00:00.000000 redshift_client-1.2.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      593 1980-01-01 00:00:00.000000 redshift_client-1.2.1/arch.cfg
--rw-r--r--   0        0        0      218 1980-01-01 00:00:00.000000 redshift_client-1.2.1/build/deps/default.nix
--rw-r--r--   0        0        0      579 1980-01-01 00:00:00.000000 redshift_client-1.2.1/build/deps/import-linter/default.nix
--rw-r--r--   0        0        0      202 1980-01-01 00:00:00.000000 redshift_client-1.2.1/build/deps/psycopg2/stubs.nix
--rw-r--r--   0        0        0      569 1980-01-01 00:00:00.000000 redshift_client-1.2.1/build/pkg/build.nix
--rwxr-xr-x   0        0        0      155 1980-01-01 00:00:00.000000 redshift_client-1.2.1/build/pkg/check/arch.sh
--rwxr-xr-x   0        0        0      127 1980-01-01 00:00:00.000000 redshift_client-1.2.1/build/pkg/check/tests.sh
--rwxr-xr-x   0        0        0      135 1980-01-01 00:00:00.000000 redshift_client-1.2.1/build/pkg/check/types.sh
--rw-r--r--   0        0        0      850 1980-01-01 00:00:00.000000 redshift_client-1.2.1/build/pkg/default.nix
--rwxr-xr-x   0        0        0      131 1980-01-01 00:00:00.000000 redshift_client-1.2.1/build/pkg/dev_env_hook.sh
--rw-r--r--   0        0        0     1482 1980-01-01 00:00:00.000000 redshift_client-1.2.1/build/pkg/vs_settings.py
--rw-r--r--   0        0        0      100 1980-01-01 00:00:00.000000 redshift_client-1.2.1/build/publish/default.nix
--rw-r--r--   0        0        0      262 1980-01-01 00:00:00.000000 redshift_client-1.2.1/ci/check.nix
--rw-r--r--   0        0        0      191 1980-01-01 00:00:00.000000 redshift_client-1.2.1/ci/utils.sh
--rw-r--r--   0        0        0     1437 1980-01-01 00:00:00.000000 redshift_client-1.2.1/default.nix
--rw-r--r--   0        0        0     1995 1980-01-01 00:00:00.000000 redshift_client-1.2.1/flake.lock
--rw-r--r--   0        0        0      915 1980-01-01 00:00:00.000000 redshift_client-1.2.1/flake.nix
--rw-r--r--   0        0        0      122 1980-01-01 00:00:00.000000 redshift_client-1.2.1/makes.lock.nix
--rw-r--r--   0        0        0      524 1980-01-01 00:00:00.000000 redshift_client-1.2.1/makes.nix
--rw-r--r--   0        0        0      740 1980-01-01 00:00:00.000000 redshift_client-1.2.1/mypy.ini
--rw-r--r--   0        0        0      260 1980-01-01 00:00:00.000000 redshift_client-1.2.1/nix.conf
--rw-r--r--   0        0        0      514 1980-01-01 00:00:00.000000 redshift_client-1.2.1/pyproject.toml
--rw-r--r--   0        0        0       22 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/__init__.py
--rw-r--r--   0        0        0      413 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/column.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/data_type/__init__.py
--rw-r--r--   0        0        0     1584 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/data_type/alias.py
--rw-r--r--   0        0        0     1108 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/data_type/core.py
--rw-r--r--   0        0        0     1555 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/data_type/decode.py
--rw-r--r--   0        0        0      175 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/id_objs.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/py.typed
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/schema/__init__.py
--rw-r--r--   0        0        0     6728 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/schema/client.py
--rw-r--r--   0        0        0      604 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/schema/core.py
--rw-r--r--   0        0        0     4410 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/sql_client/__init__.py
--rw-r--r--   0        0        0     1046 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/sql_client/_assert.py
--rw-r--r--   0        0        0     2381 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/sql_client/connection.py
--rw-r--r--   0        0        0     1534 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/sql_client/primitive.py
--rw-r--r--   0        0        0     1236 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/sql_client/query.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/table/__init__.py
--rw-r--r--   0        0        0     1274 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/table/_assert.py
--rw-r--r--   0        0        0    12339 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/table/client.py
--rw-r--r--   0        0        0     1219 1980-01-01 00:00:00.000000 redshift_client-1.2.1/redshift_client/table/core.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.1/tests/__init__.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.1/tests/py.typed
--rw-r--r--   0        0        0       45 1980-01-01 00:00:00.000000 redshift_client-1.2.1/tests/test_placeholder.py
--rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 redshift_client-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0       83 1980-01-01 00:00:00.000000 redshift_client-1.2.2/.envrc
+-rw-r--r--   0        0        0       47 1980-01-01 00:00:00.000000 redshift_client-1.2.2/.gitignore
+-rw-r--r--   0        0        0     2088 1980-01-01 00:00:00.000000 redshift_client-1.2.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      262 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/ci/check.nix
+-rw-r--r--   0        0        0      191 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/ci/utils.sh
+-rw-r--r--   0        0        0      780 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/default.nix
+-rw-r--r--   0        0        0      984 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/deps/default.nix
+-rw-r--r--   0        0        0      217 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/deps/deprecated/stubs.nix
+-rw-r--r--   0        0        0      251 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/deps/networkx.nix
+-rw-r--r--   0        0        0     1368 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/deps/override_utils.nix
+-rw-r--r--   0        0        0      202 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/deps/psycopg2/stubs.nix
+-rw-r--r--   0        0        0      182 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/dev_env/default.nix
+-rwxr-xr-x   0        0        0      131 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/dev_env/hook.sh
+-rw-r--r--   0        0        0     1482 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/dev_env/vs_settings.py
+-rw-r--r--   0        0        0      210 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/generic_builder/check.nix
+-rw-r--r--   0        0        0      341 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/generic_builder/default.nix
+-rw-r--r--   0        0        0      245 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/generic_builder/env.nix
+-rw-r--r--   0        0        0      310 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/generic_builder/metadata.nix
+-rwxr-xr-x   0        0        0      127 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/generic_builder/pkg/check/tests.sh
+-rwxr-xr-x   0        0        0      160 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/generic_builder/pkg/check/types.sh
+-rw-r--r--   0        0        0      625 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/generic_builder/pkg/default.nix
+-rw-r--r--   0        0        0     3085 1980-01-01 00:00:00.000000 redshift_client-1.2.2/flake.lock
+-rw-r--r--   0        0        0     1687 1980-01-01 00:00:00.000000 redshift_client-1.2.2/flake.nix
+-rw-r--r--   0        0        0      122 1980-01-01 00:00:00.000000 redshift_client-1.2.2/makes.lock.nix
+-rw-r--r--   0        0        0      524 1980-01-01 00:00:00.000000 redshift_client-1.2.2/makes.nix
+-rw-r--r--   0        0        0      714 1980-01-01 00:00:00.000000 redshift_client-1.2.2/mypy.ini
+-rw-r--r--   0        0        0      260 1980-01-01 00:00:00.000000 redshift_client-1.2.2/nix.conf
+-rw-r--r--   0        0        0      514 1980-01-01 00:00:00.000000 redshift_client-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0       22 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/__init__.py
+-rw-r--r--   0        0        0      423 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/column.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/data_type/__init__.py
+-rw-r--r--   0        0        0     1584 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/data_type/alias.py
+-rw-r--r--   0        0        0     1108 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/data_type/core.py
+-rw-r--r--   0        0        0     1555 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/data_type/decode.py
+-rw-r--r--   0        0        0      175 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/id_objs.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/py.typed
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/schema/__init__.py
+-rw-r--r--   0        0        0     6728 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/schema/client.py
+-rw-r--r--   0        0        0      604 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/schema/core.py
+-rw-r--r--   0        0        0     4410 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/sql_client/__init__.py
+-rw-r--r--   0        0        0     1046 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/sql_client/_assert.py
+-rw-r--r--   0        0        0     2381 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/sql_client/connection.py
+-rw-r--r--   0        0        0     1534 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/sql_client/primitive.py
+-rw-r--r--   0        0        0     1236 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/sql_client/query.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/table/__init__.py
+-rw-r--r--   0        0        0     1284 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/table/_assert.py
+-rw-r--r--   0        0        0    12339 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/table/client.py
+-rw-r--r--   0        0        0     1219 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/table/core.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.2/tests/arch/__init__.py
+-rw-r--r--   0        0        0     1559 1980-01-01 00:00:00.000000 redshift_client-1.2.2/tests/arch/arch.py
+-rw-r--r--   0        0        0     1055 1980-01-01 00:00:00.000000 redshift_client-1.2.2/tests/arch/test_arch.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.2/tests/py.typed
+-rw-r--r--   0        0        0       45 1980-01-01 00:00:00.000000 redshift_client-1.2.2/tests/test_placeholder.py
+-rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 redshift_client-1.2.2/PKG-INFO
```

### Comparing `redshift_client-1.2.1/.gitlab-ci.yml` & `redshift_client-1.2.2/.gitlab-ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 .with_nix: &with_nix
   image: nixos/nix:2.6.0
   before_script:
     - cp ./nix.conf /etc/nix/nix.conf
     - nix-env -iA nixpkgs.jq
     - nix-env -iA cachix -f https://cachix.org/api/v1/install
-    - source ./ci/utils.sh
+    - source ./build/ci/utils.sh
 
 
 .in_dev_branch: &in_dev_branch
   rules:
     - if: '$CI_COMMIT_TAG != null'
       when: never
     - if: '$CI_COMMIT_BRANCH =~ /^v\d+$/'
@@ -25,14 +25,22 @@
       when: never
     - if: '$CI_PIPELINE_SOURCE == "schedule"'
       when: never
     - if: '$CI_PIPELINE_SOURCE == "trigger"'
       when: never
     - when: on_success
 
+.in_prod_branch: &in_prod_branch
+  rules:
+    - if: '$CI_COMMIT_BRANCH == "main"'
+      when: on_success
+    - if: '$CI_COMMIT_BRANCH =~ /^v\d+$/'
+      when: on_success
+    - when: never
+
 .new_version: &new_version
   rules:
     - if: '$CI_COMMIT_TAG =~ /^v\d+\.\d+\.\d+$/'
       when: on_success
 
 format-code:
   image: ghcr.io/fluidattacks/makes:21.11
@@ -49,60 +57,46 @@
 
 lint-bash:
   image: ghcr.io/fluidattacks/makes:21.11
   stage: lint
   <<: *in_dev_branch
   script: m . /formatBash && m . /lintBash
 
-build-runtime-env:
+build-for-python38:
   <<: *with_nix
   <<: *in_dev_branch
   stage: build
   script:
-    - build ".#python38.env.runtime"
+    - build ".#python38.pkg"
 
-build-dev-env:
+build-for-python39:
   <<: *with_nix
   <<: *in_dev_branch
   stage: build
   script:
-    - build ".#python38.env.dev"
+    - build ".#python39.pkg"
 
-arch-check:
+build-for-python310:
   <<: *with_nix
   <<: *in_dev_branch
-  stage: test
-  script:
-    - build ".#python38.check.arch"
-
-test-check:
-  <<: *with_nix
-  <<: *in_dev_branch
-  stage: test
+  stage: build
   script:
-    - build ".#python38.check.tests"
+    - build ".#python310.pkg"
 
-type-check:
+build-for-python311:
   <<: *with_nix
   <<: *in_dev_branch
-  stage: test
-  script:
-    - build ".#python38.check.types"
-
-build-for-min-python:
-  <<: *with_nix
-  <<: *new_version
   stage: build
   script:
-    - build ".#python38.pkg"
+    - build ".#python311.pkg"
 
 deploy-to-pypi:
   <<: *with_nix
   <<: *new_version
   stage: deploy
   script:
     - src=$(pwd)
     - nix develop -i
       -k FLIT_USERNAME
       -k FLIT_PASSWORD
-      ".#publish" -c
+      ".#python311.publish" -c
         flit -f "${src}/pyproject.toml" publish
```

### Comparing `redshift_client-1.2.1/build/pkg/vs_settings.py` & `redshift_client-1.2.2/build/dev_env/vs_settings.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.1/flake.lock` & `redshift_client-1.2.2/flake.lock`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.91171875%*

 * *Differences: {"'nodes'": "{'nixpkgs': {'locked': {'lastModified': 1679793451, 'narHash': "*

 * *            "'sha256-JafTtgMDATE8dZOImBhWMA9RCn9AP8FVOpN+9K/tTlg=', 'rev': "*

 * *            "'0cd51a933d91078775b300cf0f29aa3495231aa2'}, 'original': {'rev': "*

 * *            "'0cd51a933d91078775b300cf0f29aa3495231aa2'}}, 'root': {'inputs': {'nix_filter': "*

 * *            "'nix_filter_3', 'arch-lint': 'arch-lint', 'fa-purity': 'fa-purity', delete: "*

 * *            "['purity']}}, 'arch-lint': OrderedDict([('inputs', OrderedDict([('nix_filter', […]*

```diff
@@ -1,9 +1,53 @@
 {
     "nodes": {
+        "arch-lint": {
+            "inputs": {
+                "nix_filter": "nix_filter",
+                "nixpkgs": [
+                    "nixpkgs"
+                ]
+            },
+            "locked": {
+                "lastModified": 1683562176,
+                "narHash": "sha256-dlbR1p3lGlyJbr02EhOT11Mv0MfV7Rdqx81UYsd4I6M=",
+                "owner": "dmurciaatfluid",
+                "repo": "arch_lint",
+                "rev": "067d033fc82af3142b9faf6fb307c8812210873b",
+                "type": "gitlab"
+            },
+            "original": {
+                "owner": "dmurciaatfluid",
+                "ref": "v2.4.0",
+                "repo": "arch_lint",
+                "type": "gitlab"
+            }
+        },
+        "fa-purity": {
+            "inputs": {
+                "nix_filter": "nix_filter_2",
+                "nixpkgs": [
+                    "nixpkgs"
+                ]
+            },
+            "locked": {
+                "lastModified": 1683067095,
+                "narHash": "sha256-PXtAE7mLIlr6urKo+yH+Vwjf4cL+NwjNxa0YhjwQR/4=",
+                "owner": "dmurciaatfluid",
+                "repo": "purity",
+                "rev": "a89d23efd5ee2b2b49b951f187448a1afc6565a3",
+                "type": "gitlab"
+            },
+            "original": {
+                "owner": "dmurciaatfluid",
+                "ref": "v1.33.2",
+                "repo": "purity",
+                "type": "gitlab"
+            }
+        },
         "nix_filter": {
             "locked": {
                 "lastModified": 1645371475,
                 "narHash": "sha256-z2n0y5ME7yQTqzzGWnQTVd1MG5Bp1E+of7ZgA861/9E=",
                 "owner": "numtide",
                 "repo": "nix-filter",
                 "rev": "38bc843f1ce76958a9f6f0a1e4e3455221c8ecf6",
@@ -26,55 +70,50 @@
             },
             "original": {
                 "owner": "numtide",
                 "repo": "nix-filter",
                 "type": "github"
             }
         },
-        "nixpkgs": {
+        "nix_filter_3": {
             "locked": {
-                "lastModified": 1658172557,
-                "narHash": "sha256-oMwKOcpt9IsuW3g7ZcSZEnTJOMgw9jzVxJOF+15xjNs=",
-                "owner": "nixos",
-                "repo": "nixpkgs",
-                "rev": "02da3a122947e0ae1c024d276b03cb487f2266bd",
+                "lastModified": 1645371475,
+                "narHash": "sha256-z2n0y5ME7yQTqzzGWnQTVd1MG5Bp1E+of7ZgA861/9E=",
+                "owner": "numtide",
+                "repo": "nix-filter",
+                "rev": "38bc843f1ce76958a9f6f0a1e4e3455221c8ecf6",
                 "type": "github"
             },
             "original": {
-                "owner": "nixos",
-                "repo": "nixpkgs",
+                "owner": "numtide",
+                "repo": "nix-filter",
                 "type": "github"
             }
         },
-        "purity": {
-            "inputs": {
-                "nix_filter": "nix_filter_2",
-                "nixpkgs": [
-                    "nixpkgs"
-                ]
-            },
+        "nixpkgs": {
             "locked": {
-                "lastModified": 1668537152,
-                "narHash": "sha256-pj3QzQMuWPHSe+trWyfTXTZ3gZGA4+ME80Us/hLv0qM=",
-                "owner": "dmurciaatfluid",
-                "repo": "purity",
-                "rev": "c6802114d23a1793efb7a004b5e5add4ec599e90",
-                "type": "gitlab"
+                "lastModified": 1679793451,
+                "narHash": "sha256-JafTtgMDATE8dZOImBhWMA9RCn9AP8FVOpN+9K/tTlg=",
+                "owner": "nixos",
+                "repo": "nixpkgs",
+                "rev": "0cd51a933d91078775b300cf0f29aa3495231aa2",
+                "type": "github"
             },
             "original": {
-                "owner": "dmurciaatfluid",
-                "ref": "v1.26.0",
-                "repo": "purity",
-                "type": "gitlab"
+                "owner": "nixos",
+                "repo": "nixpkgs",
+                "rev": "0cd51a933d91078775b300cf0f29aa3495231aa2",
+                "type": "github"
             }
         },
         "root": {
             "inputs": {
-                "nix_filter": "nix_filter",
-                "nixpkgs": "nixpkgs",
-                "purity": "purity"
+                "arch-lint": "arch-lint",
+                "fa-purity": "fa-purity",
+                "nix_filter": "nix_filter_3",
+                "nixpkgs": "nixpkgs"
             }
         }
     },
     "root": "root",
     "version": 7
 }
```

### Comparing `redshift_client-1.2.1/makes.nix` & `redshift_client-1.2.2/makes.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.1/mypy.ini` & `redshift_client-1.2.2/mypy.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 [mypy]
-ignore_missing_imports = False
-
-disallow_any_unimported = True
-disallow_any_expr = True
 disallow_any_decorated = True
+disallow_any_expr = True
 disallow_any_explicit = True
 disallow_any_generics = True
+disallow_any_unimported = True
+disallow_incomplete_defs = True
 disallow_subclassing_any = True
-
 disallow_untyped_calls = True
-disallow_untyped_defs = True
-disallow_incomplete_defs = True
-check_untyped_defs = True
 disallow_untyped_decorators = True
+disallow_untyped_defs = True
 
+check_untyped_defs = True
 no_implicit_optional = True
+strict = True
+strict_equality = True
 strict_optional = True
 
 warn_redundant_casts = True
 warn_unused_ignores = True
 warn_no_return = True
 warn_return_any = True
 warn_unreachable = True
 
-show_none_errors = True
 ignore_errors = False
-
+ignore_missing_imports = False
 allow_untyped_globals = False
 allow_redefinition = False
 local_partial_types = False
-implicit_reexport = True
-strict_equality = True
-strict = True
+implicit_reexport = False
```

### Comparing `redshift_client-1.2.1/pyproject.toml` & `redshift_client-1.2.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 classifiers = [
     "License :: OSI Approved :: MIT License",
 ]
 requires-python = ">=3.8"
 dependencies = [
     "Deprecated >=1.2.12, <2.0.0",
     "psycopg2 >=2.8.6, <3.0.0",
-    "fa-purity >=1.26.0 , <2.0.0",
+    "fa-purity >=1.33.2 , <2.0.0",
     "types-Deprecated >=1.2.1, <2.0.0",
 ]
 description = "Redshift client-SDK"
 dynamic = ["version"]
 
 [build-system]
 requires = ["flit_core >=3.2,<4"]
```

### Comparing `redshift_client-1.2.1/redshift_client/data_type/alias.py` & `redshift_client-1.2.2/redshift_client/data_type/alias.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.1/redshift_client/data_type/core.py` & `redshift_client-1.2.2/redshift_client/data_type/core.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.1/redshift_client/data_type/decode.py` & `redshift_client-1.2.2/redshift_client/data_type/decode.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.1/redshift_client/schema/client.py` & `redshift_client-1.2.2/redshift_client/schema/client.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.1/redshift_client/schema/core.py` & `redshift_client-1.2.2/redshift_client/schema/core.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.1/redshift_client/sql_client/__init__.py` & `redshift_client-1.2.2/redshift_client/sql_client/__init__.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.1/redshift_client/sql_client/_assert.py` & `redshift_client-1.2.2/redshift_client/sql_client/_assert.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.1/redshift_client/sql_client/connection.py` & `redshift_client-1.2.2/redshift_client/sql_client/connection.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.1/redshift_client/sql_client/primitive.py` & `redshift_client-1.2.2/redshift_client/sql_client/primitive.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.1/redshift_client/sql_client/query.py` & `redshift_client-1.2.2/redshift_client/sql_client/query.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.1/redshift_client/table/_assert.py` & `redshift_client-1.2.2/redshift_client/table/_assert.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from redshift_client.column import (
     Column,
     ColumnId,
 )
 from redshift_client.data_type.decode import (
     decode_type,
 )
-from redshift_client.sql_client import (
+from redshift_client.sql_client.primitive import (
     PrimitiveVal,
 )
 from typing import (
     Optional,
     Tuple,
 )
```

### Comparing `redshift_client-1.2.1/redshift_client/table/client.py` & `redshift_client-1.2.2/redshift_client/table/client.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.1/redshift_client/table/core.py` & `redshift_client-1.2.2/redshift_client/table/core.py`

 * *Files identical despite different names*

