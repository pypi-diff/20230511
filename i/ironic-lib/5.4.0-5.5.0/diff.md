# Comparing `tmp/ironic-lib-5.4.0.tar.gz` & `tmp/ironic-lib-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ironic-lib-5.4.0.tar", last modified: Fri Feb 10 16:04:11 2023, max compression
+gzip compressed data, was "ironic-lib-5.5.0.tar", last modified: Thu May 11 09:06:11 2023, max compression
```

## Comparing `ironic-lib-5.4.0.tar` & `ironic-lib-5.5.0.tar`

### file list

```diff
@@ -1,96 +1,98 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:04:11.164322 ironic-lib-5.4.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9780 2023-02-10 16:04:10.000000 ironic-lib-5.4.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    82460 2023-02-10 16:04:10.000000 ironic-lib-5.4.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11325 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2023-02-10 16:04:11.164322 ironic-lib-5.4.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2601 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/TESTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:04:11.152321 ironic-lib-5.4.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:04:11.152321 ironic-lib-5.4.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2362 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:04:11.152321 ironic-lib-5.4.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2860 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:04:11.152321 ironic-lib-5.4.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:04:11.148321 ironic-lib-5.4.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:04:11.148321 ironic-lib-5.4.0/etc/ironic/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:04:11.152321 ironic-lib-5.4.0/etc/ironic/rootwrap.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/etc/ironic/rootwrap.d/ironic-lib.filters
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/extra-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:04:11.156321 ironic-lib-5.4.0/ironic_lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7090 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/auth_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4960 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/capabilities.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:04:11.156321 ironic-lib-5.4.0/ironic_lib/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/common/i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5705 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/disk_partitioner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30540 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/disk_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6914 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/exception.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:04:11.156321 ironic-lib-5.4.0/ironic_lib/json_rpc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2927 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/json_rpc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8147 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/json_rpc/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11064 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/json_rpc/server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7751 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12150 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/mdns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9649 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/metrics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4513 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/metrics_collector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3717 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/metrics_statsd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4186 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/metrics_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:04:11.160322 ironic-lib-5.4.0/ironic_lib/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3093 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3523 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/tests/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8545 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/tests/test_basic_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3339 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/tests/test_capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9498 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/tests/test_disk_partitioner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47232 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/tests/test_disk_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2621 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/tests/test_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28993 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/tests/test_json_rpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5432 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/tests/test_keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15484 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/tests/test_mdns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7029 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/tests/test_metrics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2546 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/tests/test_metrics_collector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3807 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/tests/test_metrics_statsd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4476 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/tests/test_metrics_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35416 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/tests/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26544 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/ironic_lib/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:04:11.156321 ironic-lib-5.4.0/ironic_lib.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2023-02-10 16:04:10.000000 ironic-lib-5.4.0/ironic_lib.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2582 2023-02-10 16:04:11.000000 ironic-lib-5.4.0/ironic_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 16:04:10.000000 ironic-lib-5.4.0/ironic_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2023-02-10 16:04:10.000000 ironic-lib-5.4.0/ironic_lib.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 16:04:10.000000 ironic-lib-5.4.0/ironic_lib.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-10 16:04:10.000000 ironic-lib-5.4.0/ironic_lib.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-02-10 16:04:10.000000 ironic-lib-5.4.0/ironic_lib.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-02-10 16:04:10.000000 ironic-lib-5.4.0/ironic_lib.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/lower-constraints.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:04:11.148321 ironic-lib-5.4.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:04:11.164322 ironic-lib-5.4.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      568 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/releasenotes/notes/add-additional-disk-conversion-retry-dfff93cbdf779f81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/releasenotes/notes/add-metrics-collection-b9549ec62ce4feda.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      738 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/releasenotes/notes/basic-auth-middleware-e5af29651b2d7979.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/releasenotes/notes/conver-str-to-bytes-11a665d0fa8828ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/releasenotes/notes/drop-py-2-7-3c01e37309077c06.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/releasenotes/notes/erase-tiny-partitions-c408a3a4afe60d44.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/releasenotes/notes/extend-list-partitions-b71f81c77f6ecfdb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/releasenotes/notes/fix-metadisk-partitioning-32d3fca274290dd6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/releasenotes/notes/json_rpc-allowed_roles-3bee50b5936c2be3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/releasenotes/notes/remove-iscsi-verify-attempts-ff9eb5b7a28e6143.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/releasenotes/notes/rescan-for-partition-write-out-3fbb92ae5c2a33c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/releasenotes/notes/restore-centos7-compatibility-bfbe2bcf1d1fb7f0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/releasenotes/notes/wipe-gpt-on-metadata-wipe-ac0a93b16e00893f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1639 2023-02-10 16:04:11.164322 ironic-lib-5.4.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      441 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2233 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:04:11.164322 ironic-lib-5.4.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/zuul.d/ironic-lib-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-02-10 16:03:44.000000 ironic-lib-5.4.0/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:06:11.044878 ironic-lib-5.5.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9780 2023-05-11 09:06:10.000000 ironic-lib-5.5.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    82639 2023-05-11 09:06:10.000000 ironic-lib-5.5.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11325 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2023-05-11 09:06:11.044878 ironic-lib-5.5.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2601 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/TESTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:06:11.028869 ironic-lib-5.5.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:06:11.028869 ironic-lib-5.5.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2362 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:06:11.032872 ironic-lib-5.5.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2860 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:06:11.032872 ironic-lib-5.5.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:06:11.024867 ironic-lib-5.5.0/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:06:11.024867 ironic-lib-5.5.0/etc/ironic/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:06:11.032872 ironic-lib-5.5.0/etc/ironic/rootwrap.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/etc/ironic/rootwrap.d/ironic-lib.filters
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/extra-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:06:11.032872 ironic-lib-5.5.0/ironic_lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7090 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/auth_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4960 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/capabilities.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:06:11.036874 ironic-lib-5.5.0/ironic_lib/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/common/i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5705 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/disk_partitioner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30595 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/disk_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6914 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/exception.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:06:11.036874 ironic-lib-5.5.0/ironic_lib/json_rpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2927 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/json_rpc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8767 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/json_rpc/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11064 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/json_rpc/server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7751 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12150 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/mdns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9649 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/metrics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4513 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/metrics_collector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3717 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/metrics_statsd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4186 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/metrics_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:06:11.040876 ironic-lib-5.5.0/ironic_lib/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3093 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3523 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/tests/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8545 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/tests/test_basic_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3339 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/tests/test_capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9498 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/tests/test_disk_partitioner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    47344 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/tests/test_disk_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2621 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/tests/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29790 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/tests/test_json_rpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5432 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/tests/test_keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15484 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/tests/test_mdns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7029 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/tests/test_metrics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2546 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/tests/test_metrics_collector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3807 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/tests/test_metrics_statsd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4476 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/tests/test_metrics_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35416 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/tests/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26544 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/ironic_lib/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:06:11.036874 ironic-lib-5.5.0/ironic_lib.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2023-05-11 09:06:10.000000 ironic-lib-5.5.0/ironic_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2023-05-11 09:06:11.000000 ironic-lib-5.5.0/ironic_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-11 09:06:10.000000 ironic-lib-5.5.0/ironic_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2023-05-11 09:06:10.000000 ironic-lib-5.5.0/ironic_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-11 09:06:10.000000 ironic-lib-5.5.0/ironic_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-11 09:06:10.000000 ironic-lib-5.5.0/ironic_lib.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-05-11 09:06:10.000000 ironic-lib-5.5.0/ironic_lib.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-05-11 09:06:10.000000 ironic-lib-5.5.0/ironic_lib.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:06:11.024867 ironic-lib-5.5.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:06:11.044878 ironic-lib-5.5.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      568 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/releasenotes/notes/add-additional-disk-conversion-retry-dfff93cbdf779f81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/releasenotes/notes/add-metrics-collection-b9549ec62ce4feda.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/releasenotes/notes/add-port-to-rpc-client-2f2f0cd60547843f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      738 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/releasenotes/notes/basic-auth-middleware-e5af29651b2d7979.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/releasenotes/notes/conver-str-to-bytes-11a665d0fa8828ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/releasenotes/notes/drop-py-2-7-3c01e37309077c06.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/releasenotes/notes/erase-tiny-partitions-c408a3a4afe60d44.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/releasenotes/notes/extend-list-partitions-b71f81c77f6ecfdb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/releasenotes/notes/fix-dd-async-gpt-erasure-bbc6b084b0344d30.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/releasenotes/notes/fix-metadisk-partitioning-32d3fca274290dd6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/releasenotes/notes/json_rpc-allowed_roles-3bee50b5936c2be3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/releasenotes/notes/remove-iscsi-verify-attempts-ff9eb5b7a28e6143.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/releasenotes/notes/rescan-for-partition-write-out-3fbb92ae5c2a33c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/releasenotes/notes/restore-centos7-compatibility-bfbe2bcf1d1fb7f0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/releasenotes/notes/wipe-gpt-on-metadata-wipe-ac0a93b16e00893f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1639 2023-05-11 09:06:11.044878 ironic-lib-5.5.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      441 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2221 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:06:11.044878 ironic-lib-5.5.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/zuul.d/ironic-lib-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-05-11 09:05:48.000000 ironic-lib-5.5.0/zuul.d/project.yaml
```

### Comparing `ironic-lib-5.4.0/AUTHORS` & `ironic-lib-5.5.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ChangeLog` & `ironic-lib-5.5.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+5.5.0
+-----
+
+* Upgrade to latest hacking - v6
+* Add jsonrpc client port capability
+* Exclude all files starting with . from flake8 tests
+* Use direct writes when erasing the GPT
+
 5.4.0
 -----
 
 * Provide an interface to store metrics
 * Fix tox4 error
 * No longer override install\_command in tox.ini
 * Add Python3 antelope unit tests
```

### Comparing `ironic-lib-5.4.0/LICENSE` & `ironic-lib-5.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/PKG-INFO` & `ironic-lib-5.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ironic-lib
-Version: 5.4.0
+Version: 5.5.0
 Summary: Ironic common library
 Home-page: https://docs.openstack.org/ironic-lib/
 Author: OpenStack Ironic
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==========
         ironic-lib
```

### Comparing `ironic-lib-5.4.0/README.rst` & `ironic-lib-5.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/TESTING.rst` & `ironic-lib-5.5.0/TESTING.rst`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/doc/source/conf.py` & `ironic-lib-5.5.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/doc/source/contributor/index.rst` & `ironic-lib-5.5.0/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/etc/ironic/rootwrap.d/ironic-lib.filters` & `ironic-lib-5.5.0/etc/ironic/rootwrap.d/ironic-lib.filters`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/__init__.py` & `ironic-lib-5.5.0/ironic_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/auth_basic.py` & `ironic-lib-5.5.0/ironic_lib/auth_basic.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/capabilities.py` & `ironic-lib-5.5.0/ironic_lib/capabilities.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/common/i18n.py` & `ironic-lib-5.5.0/ironic_lib/common/i18n.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/disk_partitioner.py` & `ironic-lib-5.5.0/ironic_lib/disk_partitioner.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/disk_utils.py` & `ironic-lib-5.5.0/ironic_lib/disk_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         raise ValueError('The device %s does not have a valid MBR '
                          'partition table' % device)
     # Sample output: /dev/vdb: msdos partitions 1 2 3 <5 6 7>
     # The partitions with number > 4 (and inside <>) are logical partitions
     output = output.replace('<', '').replace('>', '')
     partitions = [int(s) for s in output.split() if s.isdigit()]
 
-    return(sum(i < 5 for i in partitions), sum(i > 4 for i in partitions))
+    return (sum(i < 5 for i in partitions), sum(i > 4 for i in partitions))
 
 
 def get_disk_identifier(dev):
     """Get the disk identifier from the disk being exposed by the ramdisk.
 
     This disk identifier is appended to the pxe config which will then be
     used by chain.c32 to detect the correct disk to chainload. This is helpful
@@ -623,23 +623,24 @@
     # Overwrite the Primary GPT, catch very small partitions (like EBRs)
     dd_device = 'of=%s' % dev
     dd_count = 'count=%s' % GPT_SIZE_SECTORS
     dev_size = get_dev_block_size(dev)
     if dev_size < GPT_SIZE_SECTORS:
         dd_count = 'count=%s' % dev_size
     utils.execute('dd', 'bs=512', 'if=/dev/zero', dd_device, dd_count,
-                  run_as_root=True, use_standard_locale=True)
+                  'oflag=direct', run_as_root=True, use_standard_locale=True)
 
     # Overwrite the Secondary GPT, do this only if there could be one
     if dev_size > GPT_SIZE_SECTORS:
         gpt_backup = dev_size - GPT_SIZE_SECTORS
         dd_seek = 'seek=%i' % gpt_backup
         dd_count = 'count=%s' % GPT_SIZE_SECTORS
         utils.execute('dd', 'bs=512', 'if=/dev/zero', dd_device, dd_count,
-                      dd_seek, run_as_root=True, use_standard_locale=True)
+                      'oflag=direct', dd_seek, run_as_root=True,
+                      use_standard_locale=True)
 
     # Go ahead and let sgdisk run as well.
     utils.execute('sgdisk', '-Z', dev, run_as_root=True,
                   use_standard_locale=True)
 
     try:
         utils.wait_for_disk_to_become_available(dev)
```

### Comparing `ironic-lib-5.4.0/ironic_lib/exception.py` & `ironic-lib-5.5.0/ironic_lib/exception.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/json_rpc/__init__.py` & `ironic-lib-5.5.0/ironic_lib/json_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/json_rpc/client.py` & `ironic-lib-5.5.0/ironic_lib/json_rpc/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,26 +78,42 @@
         self.serializer = serializer
         self.version_cap = version_cap
 
     def can_send_version(self, version):
         return _can_send_version(version, self.version_cap)
 
     def prepare(self, topic, version=None):
+        """Prepare the client to transmit a request.
+
+        :param topic: Topic which is being addressed. Typically this
+                      is the hostname of the remote json-rpc service.
+        :param version: The RPC API version to utilize.
+        """
+
         host = topic.split('.', 1)[1]
+        # NOTE(TheJulia): Originally, I was worried about ip addresses being
+        # used, but looking at the topic split, it would have never really
+        # worked.
+        host, port = netutils.parse_host_port(host)
         return _CallContext(
             host, self.serializer, version=version,
             version_cap=self.version_cap,
-            allowed_exception_namespaces=self.allowed_exception_namespaces)
+            allowed_exception_namespaces=self.allowed_exception_namespaces,
+            port=port)
 
 
 class _CallContext(object):
     """Wrapper object for compatibility with oslo.messaging API."""
 
     def __init__(self, host, serializer, version=None, version_cap=None,
-                 allowed_exception_namespaces=()):
+                 allowed_exception_namespaces=(), port=None):
+        if not port:
+            self.port = CONF.json_rpc.port
+        else:
+            self.port = int(port)
         self.host = host
         self.serializer = serializer
         self.version = version
         self.version_cap = version_cap
         self.allowed_exception_namespaces = allowed_exception_namespaces
 
     def _is_known_exception(self, class_name):
@@ -186,25 +202,24 @@
                           or uuidutils.generate_uuid())
 
         scheme = 'http'
         if CONF.json_rpc.use_ssl:
             scheme = 'https'
         url = '%s://%s:%d' % (scheme,
                               netutils.escape_ipv6(self.host),
-                              CONF.json_rpc.port)
+                              self.port)
         LOG.debug("RPC %s to %s with %s", method, url,
                   strutils.mask_dict_password(body))
         try:
             result = _get_session().post(url, json=body)
         except Exception as exc:
             LOG.debug('RPC %s to %s failed with %s', method, url, exc)
             raise
         LOG.debug('RPC %s to %s returned %s', method, url,
                   strutils.mask_password(result.text or '<None>'))
-
         if not cast:
             result = result.json()
             self._handle_error(result.get('error'))
             result = self.serializer.deserialize_entity(context,
                                                         result['result'])
             return result
```

### Comparing `ironic-lib-5.4.0/ironic_lib/json_rpc/server.py` & `ironic-lib-5.5.0/ironic_lib/json_rpc/server.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/keystone.py` & `ironic-lib-5.5.0/ironic_lib/keystone.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/mdns.py` & `ironic-lib-5.5.0/ironic_lib/mdns.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/metrics.py` & `ironic-lib-5.5.0/ironic_lib/metrics.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/metrics_collector.py` & `ironic-lib-5.5.0/ironic_lib/metrics_collector.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/metrics_statsd.py` & `ironic-lib-5.5.0/ironic_lib/metrics_statsd.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/metrics_utils.py` & `ironic-lib-5.5.0/ironic_lib/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/tests/base.py` & `ironic-lib-5.5.0/ironic_lib/tests/base.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/tests/test_base.py` & `ironic-lib-5.5.0/ironic_lib/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/tests/test_basic_auth.py` & `ironic-lib-5.5.0/ironic_lib/tests/test_basic_auth.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/tests/test_capabilities.py` & `ironic-lib-5.5.0/ironic_lib/tests/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/tests/test_disk_partitioner.py` & `ironic-lib-5.5.0/ironic_lib/tests/test_disk_partitioner.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/tests/test_disk_utils.py` & `ironic-lib-5.5.0/ironic_lib/tests/test_disk_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,20 +397,20 @@
 
         expected_calls = [mock.call('wipefs', '--force', '--all', 'fake-dev',
                                     run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('blockdev', '--getsz', 'fake-dev',
                                     run_as_root=True),
                           mock.call('dd', 'bs=512', 'if=/dev/zero',
-                                    'of=fake-dev', 'count=33',
+                                    'of=fake-dev', 'count=33', 'oflag=direct',
                                     run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('dd', 'bs=512', 'if=/dev/zero',
-                                    'of=fake-dev', 'count=33', 'seek=991',
-                                    run_as_root=True,
+                                    'of=fake-dev', 'count=33', 'oflag=direct',
+                                    'seek=991', run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('sgdisk', '-Z', 'fake-dev',
                                     run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('fuser', self.dev,
                                     check_exit_code=[0, 1],
                                     run_as_root=True)]
@@ -432,20 +432,20 @@
     def test_destroy_disk_metadata_sgdisk_fail(self, mock_exec):
         expected_calls = [mock.call('wipefs', '--force', '--all', 'fake-dev',
                                     run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('blockdev', '--getsz', 'fake-dev',
                                     run_as_root=True),
                           mock.call('dd', 'bs=512', 'if=/dev/zero',
-                                    'of=fake-dev', 'count=33',
+                                    'of=fake-dev', 'count=33', 'oflag=direct',
                                     run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('dd', 'bs=512', 'if=/dev/zero',
-                                    'of=fake-dev', 'count=33', 'seek=991',
-                                    run_as_root=True,
+                                    'of=fake-dev', 'count=33', 'oflag=direct',
+                                    'seek=991', run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('sgdisk', '-Z', 'fake-dev',
                                     run_as_root=True,
                                     use_standard_locale=True)]
         mock_exec.side_effect = iter([
             (None, None),
             ('1024\n', None),
@@ -480,15 +480,15 @@
     def test_destroy_disk_metadata_ebr(self, mock_exec):
         expected_calls = [mock.call('wipefs', '--force', '--all', 'fake-dev',
                                     run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('blockdev', '--getsz', 'fake-dev',
                                     run_as_root=True),
                           mock.call('dd', 'bs=512', 'if=/dev/zero',
-                                    'of=fake-dev', 'count=2',
+                                    'of=fake-dev', 'count=2', 'oflag=direct',
                                     run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('sgdisk', '-Z', 'fake-dev',
                                     run_as_root=True,
                                     use_standard_locale=True)]
         mock_exec.side_effect = iter([
             (None, None),
@@ -503,20 +503,20 @@
     def test_destroy_disk_metadata_tiny_partition(self, mock_exec):
         expected_calls = [mock.call('wipefs', '--force', '--all', 'fake-dev',
                                     run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('blockdev', '--getsz', 'fake-dev',
                                     run_as_root=True),
                           mock.call('dd', 'bs=512', 'if=/dev/zero',
-                                    'of=fake-dev', 'count=33',
+                                    'of=fake-dev', 'count=33', 'oflag=direct',
                                     run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('dd', 'bs=512', 'if=/dev/zero',
-                                    'of=fake-dev', 'count=33', 'seek=9',
-                                    run_as_root=True,
+                                    'of=fake-dev', 'count=33', 'oflag=direct',
+                                    'seek=9', run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('sgdisk', '-Z', 'fake-dev',
                                     run_as_root=True,
                                     use_standard_locale=True)]
         mock_exec.side_effect = iter([
             (None, None),
             ('42\n', None),
```

### Comparing `ironic-lib-5.4.0/ironic_lib/tests/test_exception.py` & `ironic-lib-5.5.0/ironic_lib/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/tests/test_json_rpc.py` & `ironic-lib-5.5.0/ironic_lib/tests/test_json_rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,35 +391,53 @@
         response = mock_session.return_value.post.return_value
         response.json.return_value = {
             'jsonrpc': '2.0',
             'result': 42
         }
         cctx = self.client.prepare('foo.2001:db8::1')
         self.assertEqual('2001:db8::1', cctx.host)
+        self.assertEqual(8089, cctx.port)
         result = cctx.call(self.context, 'do_something', answer=42)
         self.assertEqual(42, result)
         mock_session.return_value.post.assert_called_once_with(
             'http://[2001:db8::1]:8089',
             json={'jsonrpc': '2.0',
                   'method': 'do_something',
                   'params': {'answer': 42, 'context': self.ctx_json},
                   'id': self.context.request_id})
 
+    def test_call_ipv6_success_rfc2732(self, mock_session):
+        response = mock_session.return_value.post.return_value
+        response.json.return_value = {
+            'jsonrpc': '2.0',
+            'result': 42
+        }
+        cctx = self.client.prepare('foo.[2001:db8::1]:8192')
+        self.assertEqual('2001:db8::1', cctx.host)
+        result = cctx.call(self.context, 'do_something', answer=42)
+        self.assertEqual(42, result)
+        mock_session.return_value.post.assert_called_once_with(
+            'http://[2001:db8::1]:8192',
+            json={'jsonrpc': '2.0',
+                  'method': 'do_something',
+                  'params': {'answer': 42, 'context': self.ctx_json},
+                  'id': self.context.request_id})
+
     def test_call_success_with_version(self, mock_session):
         response = mock_session.return_value.post.return_value
         response.json.return_value = {
             'jsonrpc': '2.0',
             'result': 42
         }
-        cctx = self.client.prepare('foo.example.com', version='1.42')
+        cctx = self.client.prepare('foo.example.com:8192', version='1.42')
         self.assertEqual('example.com', cctx.host)
         result = cctx.call(self.context, 'do_something', answer=42)
         self.assertEqual(42, result)
         mock_session.return_value.post.assert_called_once_with(
-            'http://example.com:8089',
+            'http://example.com:8192',
             json={'jsonrpc': '2.0',
                   'method': 'do_something',
                   'params': {'answer': 42, 'context': self.ctx_json,
                              'rpc.version': '1.42'},
                   'id': self.context.request_id})
 
     def test_call_success_with_version_and_cap(self, mock_session):
```

### Comparing `ironic-lib-5.4.0/ironic_lib/tests/test_keystone.py` & `ironic-lib-5.5.0/ironic_lib/tests/test_keystone.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/tests/test_mdns.py` & `ironic-lib-5.5.0/ironic_lib/tests/test_mdns.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/tests/test_metrics.py` & `ironic-lib-5.5.0/ironic_lib/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/tests/test_metrics_collector.py` & `ironic-lib-5.5.0/ironic_lib/tests/test_metrics_collector.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/tests/test_metrics_statsd.py` & `ironic-lib-5.5.0/ironic_lib/tests/test_metrics_statsd.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/tests/test_metrics_utils.py` & `ironic-lib-5.5.0/ironic_lib/tests/test_metrics_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/tests/test_utils.py` & `ironic-lib-5.5.0/ironic_lib/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib/utils.py` & `ironic-lib-5.5.0/ironic_lib/utils.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/ironic_lib.egg-info/PKG-INFO` & `ironic-lib-5.5.0/ironic_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ironic-lib
-Version: 5.4.0
+Version: 5.5.0
 Summary: Ironic common library
 Home-page: https://docs.openstack.org/ironic-lib/
 Author: OpenStack Ironic
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==========
         ironic-lib
```

### Comparing `ironic-lib-5.4.0/ironic_lib.egg-info/SOURCES.txt` & `ironic-lib-5.5.0/ironic_lib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -60,19 +60,21 @@
 ironic_lib/tests/test_metrics.py
 ironic_lib/tests/test_metrics_collector.py
 ironic_lib/tests/test_metrics_statsd.py
 ironic_lib/tests/test_metrics_utils.py
 ironic_lib/tests/test_utils.py
 releasenotes/notes/add-additional-disk-conversion-retry-dfff93cbdf779f81.yaml
 releasenotes/notes/add-metrics-collection-b9549ec62ce4feda.yaml
+releasenotes/notes/add-port-to-rpc-client-2f2f0cd60547843f.yaml
 releasenotes/notes/basic-auth-middleware-e5af29651b2d7979.yaml
 releasenotes/notes/conver-str-to-bytes-11a665d0fa8828ec.yaml
 releasenotes/notes/drop-py-2-7-3c01e37309077c06.yaml
 releasenotes/notes/erase-tiny-partitions-c408a3a4afe60d44.yaml
 releasenotes/notes/extend-list-partitions-b71f81c77f6ecfdb.yaml
+releasenotes/notes/fix-dd-async-gpt-erasure-bbc6b084b0344d30.yaml
 releasenotes/notes/fix-metadisk-partitioning-32d3fca274290dd6.yaml
 releasenotes/notes/json_rpc-allowed_roles-3bee50b5936c2be3.yaml
 releasenotes/notes/remove-iscsi-verify-attempts-ff9eb5b7a28e6143.yaml
 releasenotes/notes/rescan-for-partition-write-out-3fbb92ae5c2a33c6.yaml
 releasenotes/notes/restore-centos7-compatibility-bfbe2bcf1d1fb7f0.yaml
 releasenotes/notes/wipe-gpt-on-metadata-wipe-ac0a93b16e00893f.yaml
 zuul.d/ironic-lib-jobs.yaml
```

### Comparing `ironic-lib-5.4.0/releasenotes/notes/add-additional-disk-conversion-retry-dfff93cbdf779f81.yaml` & `ironic-lib-5.5.0/releasenotes/notes/add-additional-disk-conversion-retry-dfff93cbdf779f81.yaml`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/releasenotes/notes/basic-auth-middleware-e5af29651b2d7979.yaml` & `ironic-lib-5.5.0/releasenotes/notes/basic-auth-middleware-e5af29651b2d7979.yaml`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/setup.cfg` & `ironic-lib-5.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/setup.py` & `ironic-lib-5.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-5.4.0/tox.ini` & `ironic-lib-5.5.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -18,29 +18,29 @@
 commands = stestr run {posargs}
 
 [flake8]
 show-source = True
 # [E129] Visually indented line with same indent as next logical line.
 # [W503] Line break occurred before a binary operator. Conflicts with W504.
 ignore = E129,W503
-exclude = .venv,.tox,dist,doc,*.egg,.update-venv
+exclude=.*,dist,doc,*lib/python*,*egg,build
 import-order-style = pep8
 application-import-names = ironic_lib
 # [H106] Don't put vim configuration in source files.
 # [H203] Use assertIs(Not)None to check for None.
 # [H204] Use assert(Not)Equal to check for equality.
 # [H205] Use assert(Greater|Less)(Equal) for comparison.
 # [H210] Require 'autospec', 'spec', or 'spec_set' in mock.patch/mock.patch.object calls
 # [H904] Delay string interpolations at logging calls.
 enable-extensions=H106,H203,H204,H205,H210,H904
 
 [testenv:pep8]
 deps =
     flake8-import-order>=0.17.1 # LGPLv3
-    hacking>=4.1.0,<5.0.0 # Apache-2.0
+    hacking~=6.0.0 # Apache-2.0
     pycodestyle>=2.0.0,<3.0.0 # MIT
     Pygments>=2.2.0 # BSD
     doc8>=0.6.0 # Apache 2.0
 commands =
     flake8 {posargs}
     doc8 README.rst doc/source --ignore D001
```

### Comparing `ironic-lib-5.4.0/zuul.d/ironic-lib-jobs.yaml` & `ironic-lib-5.5.0/zuul.d/ironic-lib-jobs.yaml`

 * *Files identical despite different names*

