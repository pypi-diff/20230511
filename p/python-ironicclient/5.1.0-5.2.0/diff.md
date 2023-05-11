# Comparing `tmp/python-ironicclient-5.1.0.tar.gz` & `tmp/python-ironicclient-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ironicclient-5.1.0.tar", last modified: Fri Feb 17 10:38:39 2023, max compression
+gzip compressed data, was "python-ironicclient-5.2.0.tar", last modified: Thu May 11 09:01:50 2023, max compression
```

## Comparing `python-ironicclient-5.1.0.tar` & `python-ironicclient-5.2.0.tar`

### file list

```diff
@@ -1,357 +1,360 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.215122 python-ironicclient-5.1.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7126 2023-02-17 10:38:39.000000 python-ironicclient-5.1.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    39936 2023-02-17 10:38:38.000000 python-ironicclient-5.1.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4232 2023-02-17 10:38:39.215122 python-ironicclient-5.1.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2592 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.175091 python-ironicclient-5.1.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.175091 python-ironicclient-5.1.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3380 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/doc/source/api_v1.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.175091 python-ironicclient-5.1.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/doc/source/cli/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.171088 python-ironicclient-5.1.0/doc/source/cli/osc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.175091 python-ironicclient-5.1.0/doc/source/cli/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1096 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/doc/source/cli/osc/v1/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2602 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/doc/source/cli/osc_plugin_cli.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2923 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/doc/source/cli/standalone.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2719 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.175091 python-ironicclient-5.1.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1519 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1956 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/doc/source/contributor/testing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.179094 python-ironicclient-5.1.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.179094 python-ironicclient-5.1.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5817 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/doc/source/user/create_command.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.179094 python-ironicclient-5.1.0/ironicclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6037 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.179094 python-ironicclient-5.1.0/ironicclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.179094 python-ironicclient-5.1.0/ironicclient/common/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/common/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16928 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/common/apiclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13414 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/common/apiclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13786 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/common/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3324 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/common/filecache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19500 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/common/http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      890 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/common/i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15715 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2695 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/exc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.179094 python-ironicclient-5.1.0/ironicclient/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5009 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/osc/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.179094 python-ironicclient-5.1.0/ironicclient/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14167 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_allocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11134 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_chassis.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5486 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12397 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_deploy_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9423 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_driver.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    78358 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19378 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17413 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_portgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13536 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_volume_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15268 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_volume_target.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8613 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.179094 python-ironicclient-5.1.0/ironicclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.183097 python-ironicclient-5.1.0/ironicclient/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17958 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.183097 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.183097 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18361 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8146 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_allocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3308 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_chassis_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_conductor_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7239 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_deploy_template_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1364 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_driver_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9457 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1994 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_create_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4970 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3438 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_power_states.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3877 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_provision_states.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4800 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2963 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5116 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_portgroup_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1115 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/functional/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.183097 python-ironicclient-5.1.0/ironicclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.183097 python-ironicclient-5.1.0/ironicclient/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.183097 python-ironicclient-5.1.0/ironicclient/tests/unit/common/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/common/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7181 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/common/apiclient/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5355 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/common/apiclient/test_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9677 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/common/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8411 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/common/test_filecache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24336 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/common/test_http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17264 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/common/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.187101 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1841 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7293 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/test_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.187101 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10097 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23761 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_allocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17983 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_chassis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9451 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1739 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16550 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_deploy_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20048 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   137839 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29204 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28663 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_portgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31976 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38280 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_target.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11630 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2627 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/test_exc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/test_import.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5060 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.191104 python-ironicclient-5.1.0/ironicclient/tests/unit/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11950 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_allocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14520 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_chassis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6113 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6549 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22786 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_create_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9684 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_deploy_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8960 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1964 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_events.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    70854 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11355 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13737 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_portgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3923 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_resource_fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11601 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_volume_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10998 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_volume_target.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.191104 python-ironicclient-5.1.0/ironicclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8839 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/v1/allocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8245 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/v1/chassis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5710 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/v1/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3713 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/v1/conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13649 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/v1/create_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4538 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/v1/deploy_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7352 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/v1/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/v1/events.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49609 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/v1/node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5979 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/v1/port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10726 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/v1/portgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17139 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/v1/resource_fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2370 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/v1/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4938 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/v1/volume_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4928 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/ironicclient/v1/volume_target.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.175091 python-ironicclient-5.1.0/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.191104 python-ironicclient-5.1.0/playbooks/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/playbooks/functional/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.191104 python-ironicclient-5.1.0/python_ironicclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4232 2023-02-17 10:38:39.000000 python-ironicclient-5.1.0/python_ironicclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16437 2023-02-17 10:38:39.000000 python-ironicclient-5.1.0/python_ironicclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-17 10:38:39.000000 python-ironicclient-5.1.0/python_ironicclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8739 2023-02-17 10:38:39.000000 python-ironicclient-5.1.0/python_ironicclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-17 10:38:39.000000 python-ironicclient-5.1.0/python_ironicclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-17 10:38:39.000000 python-ironicclient-5.1.0/python_ironicclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2023-02-17 10:38:39.000000 python-ironicclient-5.1.0/python_ironicclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-02-17 10:38:39.000000 python-ironicclient-5.1.0/python_ironicclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.175091 python-ironicclient-5.1.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.211119 python-ironicclient-5.1.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/SHA1-hash-auth-token-f8dce46f854c002c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/accept-valid_interfaces-3b8f5e3e362e04cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-allocation-owner-0c6daad4ebfea5e6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-bios-registry-in-list-21974873f146aff7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-chassis_uuid-removal-possibility-5bc0bc3a7953eaa5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-conductor-cli-233249ebc9d5a5f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-create-command-3df5efbbecc33276.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-deploy-steps-arg-0b127e29c8cf976d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-driver-cli-fields-selector-b0f527eb5f6fb2a9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-environment-variable-to-specify-version-cache-timeout-dfa5f6d4af0ea1d3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-events-support-53c461d28abf010b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-is-smartnic-port-attr-ed46d887aec276ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-json-option-0cf29be2a97e0212.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-network-data-node-attr-81dec9cecb7491b9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-neutron-integration-fields-cee7596c49722de6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-no-retired-opt-403bb5e466e4facb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-node-boot-mode-08ac768649a2fc93.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-node-boot-mode-set-9746b45aa3f80fe8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-node-description-support-6efd0882eaa0c788.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-node-history-b9b9beeb0200f185.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-node-lessee-c36409eb0415f75d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-node-owner-c2dce5a6075ce2b7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-node-resource-class-6040d1d6c734522c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-pecan-exc-construction-a776408f7ae110dc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-port-internal-info-74a03ebd8b0a3dfc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-portgroup-mode-properties-0a3023cf905adaef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-portgroups-support-c3cf3826093ee815.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-portgroups-to-create-command-6d685277f7af79df.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-rescue-interface-to-node-and-driver-e3ff9b5df2628e5a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-rescue-unrescue-support-f78266514ca59346.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-vif-attach-detach-support-e680d64e4add0fa4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-volume-connector-api-873090474d5e41b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-volume-connector-cli-873090474d5e41b9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-volume-target-api-e062303f4b3b40ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add-volume-target-cli-e062303f4b3b40f0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add_api_versions-a59e5b6899833c33.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add_automated_clean_field-d2a0c824a4e90bf4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/add_retired_field-6ec9f97c7c2f86ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/address-cross-distro-iso-tools-006711c9f150037a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/allocation-api-5f13082a8b36d788.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/allocation-backfill-4d4e51af2f787a72.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/allow-allocation-update-b4fb715045ab40a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/allow-api-user-to-use-latest-6b80e9f584eaaa4e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/allow-client-to-request-list-of-versions-88f019cad76e6464.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/bug-1524745-adds-node-create-args-a7ace744515e5943.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/bug-1524745-extend-driver-list-and-driver-show-800d96393aa17342.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/bug-1524745-update-baremetal-node-set-c1ac57de0d481efe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/bug-1712935-allow-os_baremetal_api_version_env_var_to_be_latest-28c8eed24f389673.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/bug-1724974-add-wanboot-to-supported-boot-devices.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/bug-1745099-allow-integer-portgroup-mode-6be4d3b35e216486.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/client-session-09e6ced1fbc6a9b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/conductor-group-9cfab3756aa108e4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/configdrive-7bd2b67830691b2e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/continue-del-next-node-8827e67e1c41a0a5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/debug-e9dd680d783fa4b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/deploy-templates-df354ce825b00430.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2705 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/deprecate-http-client-8d664e5ec50ec403.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/deprecate-ironic-cli-686b7a238ddf3e25.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/display-empty-string-for-chassis-uuid-if-it-is-empty-a5471c3aa740a27d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/driver-properties-for-osc-07a99d2d4e166436.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/drop-py-2-7-b0b950c0c2b6a667.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/endpoint-plus-version-4248f4f229dbc7dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/endpoint-strip-dea59ccb05628a35.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/extend-vif-attach-commands-ef3a931413ddcee7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/feature-parity-osc-cli-7606eed15f1c124f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/fix-negotiate-version-503-c3cb8d1d4901541a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/fix-owner-feature-2f3f0163ff307727.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/fix-python3-compatibility-993ace45fefcba34.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/fix-token-with-vhosts-5d0a6d53e807fa5e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/implicit-version-warning-d34b99727b50d519.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/implicit-version-warning-old-cli-fe34d423ae63544a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/index-error-no-endpoint-eb281187f80a9aa4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/instance-crash-dump-d845a31e72b5a9f7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1165 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/ironic-cli-version-a5cdec73d585444d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/ironic-create-files-fix-c31e40e566ff86b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/json-bytes-2f0085202d5e5796.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/keystone-token-auth-661a0c0d53c1b4de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/latest-baremetal-api-version-a20e3099e3b97a1b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1270 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/latest-default-41fdcc49701c4d70.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/latest-renegotiation-55daa01b3fc261be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/list-nodes-by-driver-b1e1e1018077089b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/logging-9c452e4869d80de9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      592 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/manual-clean-09f6b49df7d2513f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/missing-session-cc11e62dc966b4e0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/negative-wrap-fix-4197e91b2ecfb722.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/network_data-c48b3878a5b04df5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/no-automated-clean-0e437581ded44eb3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/no-osc-requirement-411f25fd10f18caa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      415 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/no-resource-attributeerror-d0cb327abab7dcc0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/node-deploy-step-061e8925dfee3918.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/node-driver-support-storage-interface-e93fc8d4de5d24d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/node-fault-adbe74fd600063ee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/not-ignore-delete-failtures-0783d33a606ed6f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-baremetal-driver-raid-properties-159bd57058c0fc0e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-baremetal-node-bios-setting-list-b062b31d0d4de337.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1170 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-commands-1-7-d531960472a11ac2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-default-microver-172d6e69316e70c1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-instance-crash-dump-22634a57104561a5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-max-microver-22-dc0d91a62f03a2e6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-node-list-chassis-091d080684cdccf8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-node-list-no-maintenance-ff1cef7cfbe60fb9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-node-list-option-driver-a2901ba6b4e1d3b5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-node-list-provisionstate-cd98dbddaad93e96.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-node-list-unassociated-60e46958a0abc3e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-node-power-on-off-c269980e3b9c79ca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-node-rebuild-configdrive-8979d5b1373e8d5f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-node-set-chassis-aae3413489b66b9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-plugin-9b5344aceb886cc1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-plugin-chassis-create-show-fix-ee276d707c5a5bdf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-plugin-f87e0fbb472261dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1181 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-plugin-ff0d897d8441a9e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-plugin-node-create-show-fix-283148c86fbccce2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-plugin-node-set-target-raid-config-5d538d6253902ecb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-plugin-set-unset-target-raid-config-9a1cecb5620eafda.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-port-create-uuid-5da551b154540ef7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-port-set-llc-pxeenabled-21fd8ea1982af17e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-soft-reboot-poweroff-121b8043567f54a9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-versioned-endpoint-fix-08f6b7af2f47a5d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/osc-wait-option-for-provisioning-commands-b6f5b875d573c9c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/oslo-i18n-optional-ff28821441a0807c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/oslo.config-f67bf37ea35dd7fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/pass-interface-argument-deb92e3feb0bf051.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/port-physical-network-6ea8860d773e473c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/prelude-2-0-release-ee44150902d3d399.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/protected-72d7419245a4f6c3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/provision-state-adopt-d07b838813cecfb1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/provision-state-wait-e7ff919ce8e13703.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/raid_CLI_support-7e816ccd0fb31d2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/remove-deprecated-endpoint-argument-fc0bd8099067e4ca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/remove-deprecated-http-client-c969f583573251e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/remove-deprecated-keystone-args-925ac5f3607a89a3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/remove-deprecated-osc-cmd-6dc980299d2fbde4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/remove-ironic-command-5c9f7bc4946996e0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/remove-llc-short-arg-89c7443acc6c54a4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/remove-states-field-0242960d121a09a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/reset-interface-bbd7a612242db399.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/reset-interfaces-bec227bf933fea59.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/retry-on-keystone-auth-retriable-failures-91c08b9f8bdab7f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/session-client-endpoint-override-20f1d822b4430afa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/session-create-092172964afdb71b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/show-required-arguments-in-help-commands-of-node-create-port-create-b213bb28bcc94743.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/soft-reboot-poweroff-e33d078a05db3894.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/standalone-cli-f07834585909334a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/start-using-reno-ccd220efa2c7022a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/strip-prefix-when-paginating-6140465b1488828e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/support-passing-global-request-id-4b96beb31ec906cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/switch-requests-8304d4465a8976b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/traits-support-8864f6816abecdb2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/typerror-132801fe4541fdb4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/version-overrides-4e9ba1266a238c6a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/vif-attach-port-29a421b245e19f2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/wait-for-prov-last-error-5f49b1c488879775.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/notes/yaml-files-79cd8367d7a4c2f2.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.211119 python-ironicclient-5.1.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.211119 python-ironicclient-5.1.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.211119 python-ironicclient-5.1.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9019 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9750 2023-02-17 10:38:39.215122 python-ironicclient-5.1.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.215122 python-ironicclient-5.1.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/tools/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6953 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/tools/install_venv_common.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/tools/with_venv.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2744 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:38:39.215122 python-ironicclient-5.1.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/zuul.d/ironicclient-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2023-02-17 10:37:51.000000 python-ironicclient-5.1.0/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7126 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40110 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4232 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2592 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.066241 python-ironicclient-5.2.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3380 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/api_v1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/cli/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.066241 python-ironicclient-5.2.0/doc/source/cli/osc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/doc/source/cli/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1096 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/cli/osc/v1/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2602 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/cli/osc_plugin_cli.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2923 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/cli/standalone.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2719 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1519 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1956 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/contributor/testing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5817 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/user/create_command.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/ironicclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6037 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/ironicclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/ironicclient/common/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16928 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/apiclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13414 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/apiclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13786 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3324 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/filecache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19500 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      890 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16410 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2695 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/exc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/ironicclient/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5009 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/ironicclient/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14167 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_allocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11134 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_chassis.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5486 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12397 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_deploy_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9423 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_driver.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    79576 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19378 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17413 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_portgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13536 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_volume_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15268 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_volume_target.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8613 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/ironicclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.074241 python-ironicclient-5.2.0/ironicclient/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17958 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.074241 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.074241 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18361 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8146 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_allocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3308 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_chassis_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_conductor_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7239 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_deploy_template_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1364 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_driver_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9457 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1994 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_create_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4970 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3438 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_power_states.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3877 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_provision_states.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4800 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2963 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5116 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_portgroup_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1115 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.074241 python-ironicclient-5.2.0/ironicclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.074241 python-ironicclient-5.2.0/ironicclient/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.074241 python-ironicclient-5.2.0/ironicclient/tests/unit/common/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/common/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7181 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/common/apiclient/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5355 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/common/apiclient/test_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9677 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/common/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8411 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/common/test_filecache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24336 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/common/test_http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17668 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/common/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.074241 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1841 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7293 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/test_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.078241 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10097 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23761 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_allocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17983 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_chassis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9451 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1739 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16550 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_deploy_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20048 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   140580 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29204 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28663 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_portgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31976 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38280 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_target.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11630 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2627 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/test_exc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/test_import.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5060 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.078241 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11950 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_allocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14520 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_chassis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6113 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6549 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22786 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_create_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9684 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_deploy_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8960 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1964 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_events.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    74840 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11355 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13737 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_portgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3923 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_resource_fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11601 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_volume_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10998 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_volume_target.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.082241 python-ironicclient-5.2.0/ironicclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8839 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/allocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8245 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/chassis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5710 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3713 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13649 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/create_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4538 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/deploy_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7352 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/events.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50734 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5979 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10726 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/portgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17139 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/resource_fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2370 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4938 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/volume_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4928 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/volume_target.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.066241 python-ironicclient-5.2.0/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.082241 python-ironicclient-5.2.0/playbooks/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/playbooks/functional/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.082241 python-ironicclient-5.2.0/python_ironicclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4232 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/python_ironicclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16585 2023-05-11 09:01:50.000000 python-ironicclient-5.2.0/python_ironicclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/python_ironicclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8739 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/python_ironicclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/python_ironicclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/python_ironicclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/python_ironicclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/python_ironicclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.066241 python-ironicclient-5.2.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/SHA1-hash-auth-token-f8dce46f854c002c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/accept-valid_interfaces-3b8f5e3e362e04cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-allocation-owner-0c6daad4ebfea5e6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-bios-registry-in-list-21974873f146aff7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-chassis_uuid-removal-possibility-5bc0bc3a7953eaa5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-conductor-cli-233249ebc9d5a5f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-create-command-3df5efbbecc33276.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-deploy-steps-arg-0b127e29c8cf976d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-driver-cli-fields-selector-b0f527eb5f6fb2a9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-environment-variable-to-specify-version-cache-timeout-dfa5f6d4af0ea1d3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-events-support-53c461d28abf010b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-is-smartnic-port-attr-ed46d887aec276ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-json-option-0cf29be2a97e0212.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-network-data-node-attr-81dec9cecb7491b9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-neutron-integration-fields-cee7596c49722de6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-no-retired-opt-403bb5e466e4facb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-node-boot-mode-08ac768649a2fc93.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-node-boot-mode-set-9746b45aa3f80fe8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-node-description-support-6efd0882eaa0c788.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-node-history-b9b9beeb0200f185.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-node-lessee-c36409eb0415f75d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-node-owner-c2dce5a6075ce2b7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-node-resource-class-6040d1d6c734522c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-pecan-exc-construction-a776408f7ae110dc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-port-internal-info-74a03ebd8b0a3dfc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-portgroup-mode-properties-0a3023cf905adaef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-portgroups-support-c3cf3826093ee815.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-portgroups-to-create-command-6d685277f7af79df.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-rescue-interface-to-node-and-driver-e3ff9b5df2628e5a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-rescue-unrescue-support-f78266514ca59346.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-vif-attach-detach-support-e680d64e4add0fa4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-volume-connector-api-873090474d5e41b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-volume-connector-cli-873090474d5e41b9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-volume-target-api-e062303f4b3b40ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-volume-target-cli-e062303f4b3b40f0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add_api_versions-a59e5b6899833c33.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add_automated_clean_field-d2a0c824a4e90bf4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add_retired_field-6ec9f97c7c2f86ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/address-cross-distro-iso-tools-006711c9f150037a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/allocation-api-5f13082a8b36d788.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/allocation-backfill-4d4e51af2f787a72.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/allow-allocation-update-b4fb715045ab40a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/allow-api-user-to-use-latest-6b80e9f584eaaa4e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/allow-client-to-request-list-of-versions-88f019cad76e6464.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/bug-1524745-adds-node-create-args-a7ace744515e5943.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/bug-1524745-extend-driver-list-and-driver-show-800d96393aa17342.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/bug-1524745-update-baremetal-node-set-c1ac57de0d481efe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/bug-1712935-allow-os_baremetal_api_version_env_var_to_be_latest-28c8eed24f389673.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/bug-1724974-add-wanboot-to-supported-boot-devices.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/bug-1745099-allow-integer-portgroup-mode-6be4d3b35e216486.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/client-session-09e6ced1fbc6a9b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/conductor-group-9cfab3756aa108e4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/configdrive-7bd2b67830691b2e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/configdrive-json-b9d173dde111cf22.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/continue-del-next-node-8827e67e1c41a0a5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/debug-e9dd680d783fa4b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/deploy-templates-df354ce825b00430.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2705 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/deprecate-http-client-8d664e5ec50ec403.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/deprecate-ironic-cli-686b7a238ddf3e25.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/display-empty-string-for-chassis-uuid-if-it-is-empty-a5471c3aa740a27d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/driver-properties-for-osc-07a99d2d4e166436.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/drop-py-2-7-b0b950c0c2b6a667.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/endpoint-plus-version-4248f4f229dbc7dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/endpoint-strip-dea59ccb05628a35.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/extend-vif-attach-commands-ef3a931413ddcee7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/feature-parity-osc-cli-7606eed15f1c124f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/fix-negotiate-version-503-c3cb8d1d4901541a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/fix-owner-feature-2f3f0163ff307727.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/fix-python3-compatibility-993ace45fefcba34.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/fix-token-with-vhosts-5d0a6d53e807fa5e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/implicit-version-warning-d34b99727b50d519.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/implicit-version-warning-old-cli-fe34d423ae63544a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/index-error-no-endpoint-eb281187f80a9aa4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/instance-crash-dump-d845a31e72b5a9f7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1165 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/ironic-cli-version-a5cdec73d585444d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/ironic-create-files-fix-c31e40e566ff86b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/json-bytes-2f0085202d5e5796.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/keystone-token-auth-661a0c0d53c1b4de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/latest-baremetal-api-version-a20e3099e3b97a1b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1270 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/latest-default-41fdcc49701c4d70.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/latest-renegotiation-55daa01b3fc261be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/list-nodes-by-driver-b1e1e1018077089b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/logging-9c452e4869d80de9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      592 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/manual-clean-09f6b49df7d2513f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/missing-session-cc11e62dc966b4e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/multinode-actions-9f682ad5172f032f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/negative-wrap-fix-4197e91b2ecfb722.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/network_data-c48b3878a5b04df5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/no-automated-clean-0e437581ded44eb3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/no-osc-requirement-411f25fd10f18caa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      415 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/no-resource-attributeerror-d0cb327abab7dcc0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/node-deploy-step-061e8925dfee3918.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/node-driver-support-storage-interface-e93fc8d4de5d24d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/node-fault-adbe74fd600063ee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/not-ignore-delete-failtures-0783d33a606ed6f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-baremetal-driver-raid-properties-159bd57058c0fc0e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-baremetal-node-bios-setting-list-b062b31d0d4de337.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1170 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-commands-1-7-d531960472a11ac2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-default-microver-172d6e69316e70c1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-instance-crash-dump-22634a57104561a5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-max-microver-22-dc0d91a62f03a2e6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-node-list-chassis-091d080684cdccf8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-node-list-no-maintenance-ff1cef7cfbe60fb9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-node-list-option-driver-a2901ba6b4e1d3b5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-node-list-provisionstate-cd98dbddaad93e96.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-node-list-unassociated-60e46958a0abc3e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-node-power-on-off-c269980e3b9c79ca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-node-rebuild-configdrive-8979d5b1373e8d5f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-node-set-chassis-aae3413489b66b9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-9b5344aceb886cc1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-chassis-create-show-fix-ee276d707c5a5bdf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-f87e0fbb472261dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1181 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-ff0d897d8441a9e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-node-create-show-fix-283148c86fbccce2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-node-set-target-raid-config-5d538d6253902ecb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-set-unset-target-raid-config-9a1cecb5620eafda.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-port-create-uuid-5da551b154540ef7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-port-set-llc-pxeenabled-21fd8ea1982af17e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-soft-reboot-poweroff-121b8043567f54a9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-versioned-endpoint-fix-08f6b7af2f47a5d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-wait-option-for-provisioning-commands-b6f5b875d573c9c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/oslo-i18n-optional-ff28821441a0807c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/oslo.config-f67bf37ea35dd7fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/pass-interface-argument-deb92e3feb0bf051.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/port-physical-network-6ea8860d773e473c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/prelude-2-0-release-ee44150902d3d399.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/protected-72d7419245a4f6c3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/provision-state-adopt-d07b838813cecfb1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/provision-state-wait-e7ff919ce8e13703.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/raid_CLI_support-7e816ccd0fb31d2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/remove-deprecated-endpoint-argument-fc0bd8099067e4ca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/remove-deprecated-http-client-c969f583573251e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/remove-deprecated-keystone-args-925ac5f3607a89a3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/remove-deprecated-osc-cmd-6dc980299d2fbde4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/remove-ironic-command-5c9f7bc4946996e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/remove-llc-short-arg-89c7443acc6c54a4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/remove-states-field-0242960d121a09a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/reset-interface-bbd7a612242db399.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/reset-interfaces-bec227bf933fea59.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/retry-on-keystone-auth-retriable-failures-91c08b9f8bdab7f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/session-client-endpoint-override-20f1d822b4430afa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/session-create-092172964afdb71b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/show-required-arguments-in-help-commands-of-node-create-port-create-b213bb28bcc94743.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/soft-reboot-poweroff-e33d078a05db3894.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/standalone-cli-f07834585909334a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/start-using-reno-ccd220efa2c7022a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/strip-prefix-when-paginating-6140465b1488828e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/support-passing-global-request-id-4b96beb31ec906cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/switch-requests-8304d4465a8976b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/traits-support-8864f6816abecdb2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/typerror-132801fe4541fdb4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/version-overrides-4e9ba1266a238c6a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/vif-attach-port-29a421b245e19f2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/wait-for-prov-last-error-5f49b1c488879775.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/yaml-files-79cd8367d7a4c2f2.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9019 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9750 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/tools/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6953 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/tools/install_venv_common.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/tools/with_venv.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2737 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/zuul.d/ironicclient-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/zuul.d/project.yaml
```

### Comparing `python-ironicclient-5.1.0/AUTHORS` & `python-ironicclient-5.2.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ChangeLog` & `python-ironicclient-5.2.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+5.2.0
+-----
+
+* Update dependencies for pep8: to hacking v6
+* Accept configdrive as a JSON file
+* Update master for stable/2023.1
+* Allow several nodes for most node actions
+
 5.1.0
 -----
 
 * Fix tox4 error
 * No longer override install\_command in tox.ini
 * Fix wrong assertion methods
 * Add Python3 antelope unit tests
```

### Comparing `python-ironicclient-5.1.0/LICENSE` & `python-ironicclient-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/PKG-INFO` & `python-ironicclient-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ironicclient
-Version: 5.1.0
+Version: 5.2.0
 Summary: OpenStack Bare Metal Provisioning API Client Library
 Home-page: https://docs.openstack.org/python-ironicclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==================================
         Python bindings for the Ironic API
```

### Comparing `python-ironicclient-5.1.0/README.rst` & `python-ironicclient-5.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/doc/source/api_v1.rst` & `python-ironicclient-5.2.0/doc/source/api_v1.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/doc/source/cli/osc/v1/index.rst` & `python-ironicclient-5.2.0/doc/source/cli/osc/v1/index.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/doc/source/cli/osc_plugin_cli.rst` & `python-ironicclient-5.2.0/doc/source/cli/osc_plugin_cli.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/doc/source/cli/standalone.rst` & `python-ironicclient-5.2.0/doc/source/cli/standalone.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/doc/source/conf.py` & `python-ironicclient-5.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/doc/source/contributor/contributing.rst` & `python-ironicclient-5.2.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/doc/source/contributor/testing.rst` & `python-ironicclient-5.2.0/doc/source/contributor/testing.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/doc/source/index.rst` & `python-ironicclient-5.2.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/doc/source/user/create_command.rst` & `python-ironicclient-5.2.0/doc/source/user/create_command.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/__init__.py` & `python-ironicclient-5.2.0/ironicclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/client.py` & `python-ironicclient-5.2.0/ironicclient/client.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/common/apiclient/base.py` & `python-ironicclient-5.2.0/ironicclient/common/apiclient/base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/common/apiclient/exceptions.py` & `python-ironicclient-5.2.0/ironicclient/common/apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/common/base.py` & `python-ironicclient-5.2.0/ironicclient/common/base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/common/filecache.py` & `python-ironicclient-5.2.0/ironicclient/common/filecache.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/common/http.py` & `python-ironicclient-5.2.0/ironicclient/common/http.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/common/i18n.py` & `python-ironicclient-5.2.0/ironicclient/common/i18n.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/common/utils.py` & `python-ironicclient-5.2.0/ironicclient/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -414,14 +414,16 @@
     count = 0
     while not timeout or time.time() < threshold:
         yield count
 
         poll_delay_function(poll_interval)
         count += 1
 
+    if callable(timeout_message):
+        timeout_message = timeout_message()
     raise exc.StateTransitionTimeout(timeout_message)
 
 
 def handle_json_arg(json_arg, info_desc):
     """Read a JSON argument from stdin, file or string.
 
     :param json_arg: May be a file name containing the JSON, a JSON string, or
@@ -431,7 +433,28 @@
     :raises: InvalidAttribute if the argument cannot be parsed.
     """
     if json_arg == '-':
         json_arg = get_from_stdin(info_desc)
     if json_arg:
         json_arg = handle_json_or_file_arg(json_arg)
     return json_arg
+
+
+def get_json_data(data):
+    """Check if the binary data is JSON and parse it if so.
+
+    Only supports dictionaries.
+    """
+    # We don't want to simply loads() a potentially large binary. Doing so,
+    # in my testing, is orders of magnitude (!!) slower than this process.
+    for idx in range(len(data)):
+        char = data[idx:idx + 1]
+        if char.isspace():
+            continue
+        if char != b'{' and char != 'b[':
+            return None  # not JSON, at least not JSON we care about
+        break  # maybe JSON
+
+    try:
+        return json.loads(data)
+    except ValueError:
+        return None
```

### Comparing `python-ironicclient-5.1.0/ironicclient/exc.py` & `python-ironicclient-5.2.0/ironicclient/exc.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/osc/plugin.py` & `python-ironicclient-5.2.0/ironicclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_allocation.py` & `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_allocation.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_chassis.py` & `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_chassis.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_conductor.py` & `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_conductor.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_create.py` & `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_create.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_deploy_template.py` & `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_deploy_template.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_driver.py` & `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_driver.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_node.py` & `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 from ironicclient.v1 import resource_fields as res_fields
 from ironicclient.v1 import utils as v1_utils
 
 CONFIG_DRIVE_ARG_HELP = _(
     "A gzipped, base64-encoded configuration drive string OR "
     "the path to the configuration drive file OR the path to a "
     "directory containing the config drive files OR a JSON object to build "
-    "config drive from. In case it's a directory, a config drive will be "
-    "generated from it. In case it's a JSON object with optional keys "
-    "`meta_data`, `user_data` and `network_data`, a config drive will "
-    "be generated on the server side (see the bare metal API reference for "
-    "more details).")
+    "config drive from OR the path to the JSON file. In case it's a "
+    "directory, a config drive will be generated from it. In case it's a JSON "
+    "object with optional keys `meta_data`, `user_data` and `network_data` "
+    "or a JSON file, a config drive will be generated on the server side "
+    "(see the bare metal API reference for more details).")
 
 
 NETWORK_DATA_ARG_HELP = _(
     "JSON string or a YAML file or '-' for stdin to read static network "
     "configuration for the baremetal node associated with this ironic node. "
     "Format of this file should comply with Nova network data metadata "
     "(network_data.json). Depending on ironic boot interface capabilities "
@@ -57,17 +57,18 @@
 
     log = logging.getLogger(__name__ + ".ProvisionStateBaremetalNode")
 
     def get_parser(self, prog_name):
         parser = super(ProvisionStateBaremetalNode, self).get_parser(prog_name)
 
         parser.add_argument(
-            'node',
+            'nodes',
             metavar='<node>',
-            help=_("Name or UUID of the node.")
+            nargs='+',
+            help=_("Names or UUID's of the nodes.")
         )
         parser.add_argument(
             '--provision-state',
             default=self.PROVISION_STATE,
             required=False,
             choices=[self.PROVISION_STATE],
             help=argparse.SUPPRESS)
@@ -92,21 +93,22 @@
                 pass
             else:
                 if isinstance(config_drive_dict, dict):
                     config_drive = config_drive_dict
 
         rescue_password = getattr(parsed_args, 'rescue_password', None)
 
-        baremetal_client.node.set_provision_state(
-            parsed_args.node,
-            parsed_args.provision_state,
-            configdrive=config_drive,
-            cleansteps=clean_steps,
-            deploysteps=deploy_steps,
-            rescue_password=rescue_password)
+        for node in parsed_args.nodes:
+            baremetal_client.node.set_provision_state(
+                node,
+                parsed_args.provision_state,
+                configdrive=config_drive,
+                cleansteps=clean_steps,
+                deploysteps=deploy_steps,
+                rescue_password=rescue_password)
 
 
 class ProvisionStateWithWait(ProvisionStateBaremetalNode):
     """Provision state class adding --wait flag."""
 
     log = logging.getLogger(__name__ + ".ProvisionStateWithWait")
 
@@ -141,19 +143,20 @@
             parsed_args.provision_state)
         if wait_args is None:
             # This should never happen in reality, but checking just in case
             raise exc.CommandError(
                 _("'--wait is not supported for provision state '%s'")
                 % parsed_args.provision_state)
 
-        print(_('Waiting for provision state %(state)s on node %(node)s') %
-              {'state': wait_args['expected_state'], 'node': parsed_args.node})
+        print(_('Waiting for provision state %(state)s on node(s) %(node)s') %
+              {'state': wait_args['expected_state'],
+               'node': ', '.join(parsed_args.nodes)})
 
         baremetal_client.node.wait_for_provision_state(
-            parsed_args.node,
+            parsed_args.nodes,
             timeout=parsed_args.wait_timeout,
             **wait_args)
 
 
 class AbortBaremetalNode(ProvisionStateBaremetalNode):
     """Set provision state of baremetal node to 'abort'"""
 
@@ -173,17 +176,18 @@
 
     log = logging.getLogger(__name__ + ".BootdeviceSetBaremetalNode")
 
     def get_parser(self, prog_name):
         parser = super(BootdeviceSetBaremetalNode, self).get_parser(prog_name)
 
         parser.add_argument(
-            'node',
+            'nodes',
             metavar='<node>',
-            help=_("Name or UUID of the node")
+            nargs='+',
+            help=_("Names or UUID's of the nodes")
         )
         parser.add_argument(
             'device',
             metavar='<device>',
             choices=v1_utils.BOOT_DEVICES,
             help=_("One of %s") % (oscutils.format_list(v1_utils.BOOT_DEVICES))
         )
@@ -196,18 +200,17 @@
         )
         return parser
 
     def take_action(self, parsed_args):
         self.log.debug("take_action(%s)", parsed_args)
 
         baremetal_client = self.app.client_manager.baremetal
-        baremetal_client.node.set_boot_device(
-            parsed_args.node,
-            parsed_args.device,
-            parsed_args.persistent)
+        for node in parsed_args.nodes:
+            baremetal_client.node.set_boot_device(
+                node, parsed_args.device, parsed_args.persistent)
 
 
 class BootdeviceShowBaremetalNode(command.ShowOne):
     """Show the boot device information for a node"""
 
     log = logging.getLogger(__name__ + ".BootdeviceShowBaremetalNode")
 
@@ -247,35 +250,34 @@
 
     log = logging.getLogger(__name__ + ".BootmodeSetBaremetalNode")
 
     def get_parser(self, prog_name):
         parser = super(BootmodeSetBaremetalNode, self).get_parser(prog_name)
 
         parser.add_argument(
-            'node',
+            'nodes',
             metavar='<node>',
-            help=_("Name or UUID of the node.")
+            nargs='+',
+            help=_("Names or UUID's of the nodes.")
         )
         parser.add_argument(
             'boot_mode',
             choices=['uefi', 'bios'],
             metavar='<boot_mode>',
             help=_('The boot mode to set for node (uefi/bios)')
         )
 
         return parser
 
     def take_action(self, parsed_args):
         self.log.debug("take_action(%s)", parsed_args)
 
         baremetal_client = self.app.client_manager.baremetal
-
-        baremetal_client.node.set_boot_mode(
-            parsed_args.node,
-            parsed_args.boot_mode)
+        for node in parsed_args.nodes:
+            baremetal_client.node.set_boot_mode(node, parsed_args.boot_mode)
 
 
 class CleanBaremetalNode(ProvisionStateWithWait):
     """Set provision state of baremetal node to 'clean'"""
 
     log = logging.getLogger(__name__ + ".CleanBaremetalNode")
     PROVISION_STATE = 'clean'
@@ -302,47 +304,51 @@
 
     log = logging.getLogger(__name__ + ".ConsoleDisableBaremetalNode")
 
     def get_parser(self, prog_name):
         parser = super(ConsoleDisableBaremetalNode, self).get_parser(prog_name)
 
         parser.add_argument(
-            'node',
+            'nodes',
             metavar='<node>',
-            help=_("Name or UUID of the node")
+            nargs='+',
+            help=_("Names or UUID's of the nodes")
         )
         return parser
 
     def take_action(self, parsed_args):
         self.log.debug("take_action(%s)", parsed_args)
 
         baremetal_client = self.app.client_manager.baremetal
-        baremetal_client.node.set_console_mode(parsed_args.node, False)
+        for node in parsed_args.nodes:
+            baremetal_client.node.set_console_mode(node, False)
 
 
 class ConsoleEnableBaremetalNode(command.Command):
     """Enable console access for a node"""
 
     log = logging.getLogger(__name__ + ".ConsoleEnableBaremetalNode")
 
     def get_parser(self, prog_name):
         parser = super(ConsoleEnableBaremetalNode, self).get_parser(prog_name)
 
         parser.add_argument(
-            'node',
+            'nodes',
             metavar='<node>',
-            help=_("Name or UUID of the node")
+            nargs='+',
+            help=_("Names or UUID's of the nodes")
         )
         return parser
 
     def take_action(self, parsed_args):
         self.log.debug("take_action(%s)", parsed_args)
 
         baremetal_client = self.app.client_manager.baremetal
-        baremetal_client.node.set_console_mode(parsed_args.node, True)
+        for node in parsed_args.nodes:
+            baremetal_client.node.set_console_mode(node, True)
 
 
 class ConsoleShowBaremetalNode(command.ShowOne):
     """Show console information for a node"""
 
     log = logging.getLogger(__name__ + ".ConsoleShowBaremetalNode")
 
@@ -813,61 +819,61 @@
 
     log = logging.getLogger(__name__ + ".MaintenanceSetBaremetalNode")
 
     def get_parser(self, prog_name):
         parser = super(MaintenanceSetBaremetalNode, self).get_parser(prog_name)
 
         parser.add_argument(
-            'node',
+            'nodes',
             metavar='<node>',
-            help=_("Name or UUID of the node.")
+            nargs='+',
+            help=_("Names or UUID's of the nodes.")
         )
         parser.add_argument(
             '--reason',
             metavar='<reason>',
             default=None,
             help=_("Reason for setting maintenance mode."))
 
         return parser
 
     def take_action(self, parsed_args):
         self.log.debug("take_action(%s)", parsed_args)
 
         baremetal_client = self.app.client_manager.baremetal
 
-        baremetal_client.node.set_maintenance(
-            parsed_args.node,
-            True,
-            maint_reason=parsed_args.reason)
+        for node in parsed_args.nodes:
+            baremetal_client.node.set_maintenance(
+                node, True, maint_reason=parsed_args.reason)
 
 
 class MaintenanceUnsetBaremetalNode(command.Command):
     """Unset baremetal node from maintenance mode"""
 
     log = logging.getLogger(__name__ + ".MaintenanceUnsetBaremetalNode")
 
     def get_parser(self, prog_name):
         parser = super(MaintenanceUnsetBaremetalNode,
                        self).get_parser(prog_name)
 
         parser.add_argument(
-            'node',
+            'nodes',
             metavar='<node>',
-            help=_("Name or UUID of the node.")
+            nargs='+',
+            help=_("Names or UUID's of the nodes.")
         )
         return parser
 
     def take_action(self, parsed_args):
         self.log.debug("take_action(%s)", parsed_args)
 
         baremetal_client = self.app.client_manager.baremetal
 
-        baremetal_client.node.set_maintenance(
-            parsed_args.node,
-            False)
+        for node in parsed_args.nodes:
+            baremetal_client.node.set_maintenance(node, False)
 
 
 class ManageBaremetalNode(ProvisionStateWithWait):
     """Set provision state of baremetal node to 'manage'"""
 
     log = logging.getLogger(__name__ + ".ManageBaremetalNode")
     PROVISION_STATE = 'manage'
@@ -967,17 +973,18 @@
 
     log = logging.getLogger(__name__ + ".PowerBaremetalNode")
 
     def get_parser(self, prog_name):
         parser = super(PowerBaremetalNode, self).get_parser(prog_name)
 
         parser.add_argument(
-            'node',
+            'nodes',
             metavar='<node>',
-            help=_("Name or UUID of the node.")
+            nargs='+',
+            help=_("Names or UUID's of the nodes.")
         )
         parser.add_argument(
             '--power-timeout',
             metavar='<power-timeout>',
             default=None,
             type=int,
             help=_("Timeout (in seconds, positive integer) to wait for the "
@@ -988,17 +995,18 @@
     def take_action(self, parsed_args):
         self.log.debug("take_action(%s)", parsed_args)
 
         baremetal_client = self.app.client_manager.baremetal
 
         soft = getattr(parsed_args, 'soft', False)
 
-        baremetal_client.node.set_power_state(
-            parsed_args.node, self.POWER_STATE, soft,
-            timeout=parsed_args.power_timeout)
+        for node in parsed_args.nodes:
+            baremetal_client.node.set_power_state(
+                node, self.POWER_STATE, soft,
+                timeout=parsed_args.power_timeout)
 
 
 class PowerOffBaremetalNode(PowerBaremetalNode):
     """Power off a node"""
 
     log = logging.getLogger(__name__ + ".PowerOffBaremetalNode")
     POWER_STATE = 'off'
@@ -1034,17 +1042,18 @@
 
     log = logging.getLogger(__name__ + ".RebootBaremetalNode")
 
     def get_parser(self, prog_name):
         parser = super(RebootBaremetalNode, self).get_parser(prog_name)
 
         parser.add_argument(
-            'node',
+            'nodes',
             metavar='<node>',
-            help=_("Name or UUID of the node.")
+            nargs='+',
+            help=_("Names or UUID's of the nodes.")
         )
         parser.add_argument(
             '--soft',
             dest='soft',
             action='store_true',
             default=False,
             help=_("Request Graceful reboot.")
@@ -1061,17 +1070,18 @@
         return parser
 
     def take_action(self, parsed_args):
         self.log.debug("take_action(%s)", parsed_args)
 
         baremetal_client = self.app.client_manager.baremetal
 
-        baremetal_client.node.set_power_state(
-            parsed_args.node, 'reboot', parsed_args.soft,
-            timeout=parsed_args.power_timeout)
+        for node in parsed_args.nodes:
+            baremetal_client.node.set_power_state(
+                node, 'reboot', parsed_args.soft,
+                timeout=parsed_args.power_timeout)
 
 
 class RebuildBaremetalNode(ProvisionStateWithWait):
     """Set provision state of baremetal node to 'rebuild'"""
 
     log = logging.getLogger(__name__ + ".RebuildBaremetalNode")
     PROVISION_STATE = 'rebuild'
@@ -1123,47 +1133,51 @@
 
     log = logging.getLogger(__name__ + ".SecurebootOnBaremetalNode")
 
     def get_parser(self, prog_name):
         parser = super(SecurebootOnBaremetalNode, self).get_parser(prog_name)
 
         parser.add_argument(
-            'node',
+            'nodes',
             metavar='<node>',
+            nargs='+',
             help=_("Name or UUID of the node")
         )
         return parser
 
     def take_action(self, parsed_args):
         self.log.debug("take_action(%s)", parsed_args)
 
         baremetal_client = self.app.client_manager.baremetal
-        baremetal_client.node.set_secure_boot(parsed_args.node, 'on')
+        for node in parsed_args.nodes:
+            baremetal_client.node.set_secure_boot(node, 'on')
 
 
 class SecurebootOffBaremetalNode(command.Command):
     """Turn secure boot off"""
 
     log = logging.getLogger(__name__ + ".SecurebootOffBaremetalNode")
 
     def get_parser(self, prog_name):
         parser = super(SecurebootOffBaremetalNode, self).get_parser(prog_name)
 
         parser.add_argument(
-            'node',
+            'nodes',
             metavar='<node>',
+            nargs='+',
             help=_("Name or UUID of the node")
         )
         return parser
 
     def take_action(self, parsed_args):
         self.log.debug("take_action(%s)", parsed_args)
 
         baremetal_client = self.app.client_manager.baremetal
-        baremetal_client.node.set_secure_boot(parsed_args.node, 'off')
+        for node in parsed_args.nodes:
+            baremetal_client.node.set_secure_boot(node, 'off')
 
 
 class SetBaremetalNode(command.Command):
     """Set baremetal properties"""
 
     log = logging.getLogger(__name__ + ".SetBaremetalNode")
 
@@ -1180,17 +1194,18 @@
             help=reset_help
         )
 
     def get_parser(self, prog_name):
         parser = super(SetBaremetalNode, self).get_parser(prog_name)
 
         parser.add_argument(
-            'node',
+            'nodes',
             metavar='<node>',
-            help=_("Name or UUID of the node."),
+            nargs='+',
+            help=_("Names or UUID's of the nodes."),
         )
         parser.add_argument(
             "--instance-uuid",
             metavar="<uuid>",
             help=_("Set instance UUID of node to <uuid>"),
         )
         parser.add_argument(
@@ -1385,25 +1400,32 @@
         )
 
         return parser
 
     def take_action(self, parsed_args):
         self.log.debug("take_action(%s)", parsed_args)
 
+        if parsed_args.name and len(parsed_args.nodes) > 1:
+            raise exc.CommandError(
+                _("--name cannot be used with more than one node"))
+        if parsed_args.instance_uuid and len(parsed_args.nodes) > 1:
+            raise exc.CommandError(
+                _("--instance-uuid cannot be used with more than one node"))
+
         baremetal_client = self.app.client_manager.baremetal
 
         # NOTE(rloo): Do this before updating the rest. Otherwise, it won't
         #             work if parsed_args.node is the name and the name is
         #             also being modified.
         if parsed_args.target_raid_config:
             raid_config = parsed_args.target_raid_config
             raid_config = utils.handle_json_arg(raid_config,
                                                 'target_raid_config')
-            baremetal_client.node.set_target_raid_config(parsed_args.node,
-                                                         raid_config)
+            for node in parsed_args.nodes:
+                baremetal_client.node.set_target_raid_config(node, raid_config)
 
         properties = []
         for field in ['instance_uuid', 'name',
                       'chassis_uuid', 'driver', 'resource_class',
                       'conductor_group', 'protected', 'protected_reason',
                       'retired', 'retired_reason', 'owner', 'lessee',
                       'description']:
@@ -1447,17 +1469,18 @@
         if parsed_args.network_data:
             network_data = utils.handle_json_arg(
                 parsed_args.network_data, 'static network configuration')
             network_data = ["network_data=%s" % json.dumps(network_data)]
             properties.extend(utils.args_array_to_patch('add', network_data))
 
         if properties:
-            baremetal_client.node.update(
-                parsed_args.node, properties,
-                reset_interfaces=parsed_args.reset_interfaces)
+            for node in parsed_args.nodes:
+                baremetal_client.node.update(
+                    node, properties,
+                    reset_interfaces=parsed_args.reset_interfaces)
         elif not parsed_args.target_raid_config:
             self.log.warning("Please specify what to set.")
 
 
 class ShowBaremetalNode(command.ShowOne):
     """Show baremetal node details"""
 
@@ -1530,17 +1553,18 @@
     """Unset baremetal properties"""
     log = logging.getLogger(__name__ + ".UnsetBaremetalNode")
 
     def get_parser(self, prog_name):
         parser = super(UnsetBaremetalNode, self).get_parser(prog_name)
 
         parser.add_argument(
-            'node',
+            'nodes',
             metavar='<node>',
-            help=_("Name or UUID of the node.")
+            nargs='+',
+            help=_("Names or UUID's of the nodes.")
         )
         parser.add_argument(
             '--instance-uuid',
             action='store_true',
             default=False,
             help=_('Unset instance UUID on this baremetal node')
         )
@@ -1728,15 +1752,16 @@
 
         baremetal_client = self.app.client_manager.baremetal
 
         # NOTE(rloo): Do this before removing the rest. Otherwise, it won't
         #             work if parsed_args.node is the name and the name is
         #             also being removed.
         if parsed_args.target_raid_config:
-            baremetal_client.node.set_target_raid_config(parsed_args.node, {})
+            for node in parsed_args.nodes:
+                baremetal_client.node.set_target_raid_config(node, {})
 
         properties = []
         for field in ['instance_uuid', 'name', 'chassis_uuid',
                       'resource_class', 'conductor_group', 'automated_clean',
                       'bios_interface', 'boot_interface', 'console_interface',
                       'deploy_interface', 'inspect_interface',
                       'management_interface', 'network_interface',
@@ -1761,16 +1786,18 @@
         if parsed_args.instance_info:
             properties.extend(utils.args_array_to_patch('remove',
                               ['instance_info/' + x for x
                                in parsed_args.instance_info]))
         if parsed_args.network_data:
             properties.extend(utils.args_array_to_patch(
                 'remove', ["network_data"]))
+
         if properties:
-            baremetal_client.node.update(parsed_args.node, properties)
+            for node in parsed_args.nodes:
+                baremetal_client.node.update(node, properties)
         elif not parsed_args.target_raid_config:
             self.log.warning("Please specify what to unset.")
 
 
 class ValidateBaremetalNode(command.Lister):
     """Validate a node's driver interfaces"""
 
@@ -1908,27 +1935,28 @@
 
     log = logging.getLogger(__name__ + ".InjectNmiBaremetalNode")
 
     def get_parser(self, prog_name):
         parser = super(InjectNmiBaremetalNode, self).get_parser(prog_name)
 
         parser.add_argument(
-            'node',
+            'nodes',
             metavar='<node>',
-            help=_("Name or UUID of the node.")
+            nargs='+',
+            help=_("Names or UUID's of the nodes.")
         )
 
         return parser
 
     def take_action(self, parsed_args):
         self.log.debug("take_action(%s)", parsed_args)
 
         baremetal_client = self.app.client_manager.baremetal
-
-        baremetal_client.node.inject_nmi(parsed_args.node)
+        for node in parsed_args.nodes:
+            baremetal_client.node.inject_nmi(node)
 
 
 class ListTraitsBaremetalNode(command.Lister):
     """List a node's traits."""
 
     log = logging.getLogger(__name__ + ".ListTraitsBaremetalNode")
```

### Comparing `python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_port.py` & `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_port.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_portgroup.py` & `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_portgroup.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_volume_connector.py` & `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_volume_connector.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/osc/v1/baremetal_volume_target.py` & `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_volume_target.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/shell.py` & `python-ironicclient-5.2.0/ironicclient/shell.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/functional/base.py` & `python-ironicclient-5.2.0/ironicclient/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/base.py` & `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_allocation.py` & `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_allocation.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_chassis_basic.py` & `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_chassis_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_conductor_basic.py` & `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_conductor_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_deploy_template_basic.py` & `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_deploy_template_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_driver_basic.py` & `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_driver_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_basic.py` & `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_create_negative.py` & `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_create_negative.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_fields.py` & `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_fields.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_negative.py` & `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_negative.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_power_states.py` & `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_power_states.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_provision_states.py` & `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_provision_states.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_basic.py` & `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_create.py` & `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_create.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/functional/osc/v1/test_baremetal_portgroup_basic.py` & `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_portgroup_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/functional/utils.py` & `python-ironicclient-5.2.0/ironicclient/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/common/apiclient/test_base.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/common/apiclient/test_base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/common/apiclient/test_exceptions.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/common/apiclient/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/common/test_base.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/common/test_base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/common/test_filecache.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/common/test_filecache.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/common/test_http.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/common/test_http.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/common/test_utils.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/common/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,7 +409,20 @@
         mock_open.return_value.__enter__.side_effect = IOError
 
         with tempfile.NamedTemporaryFile(mode='w') as f:
             self.assertRaisesRegex(exc.InvalidAttribute,
                                    "from file",
                                    utils.handle_json_or_file_arg, f.name)
             mock_open.assert_called_once_with(f.name, 'r')
+
+
+class GetJsonDataTest(test_utils.BaseTestCase):
+
+    def test_success(self):
+        result = utils.get_json_data(b'\n{"answer": 42}')
+        self.assertEqual({"answer": 42}, result)
+
+    def test_definitely_not_json(self):
+        self.assertIsNone(utils.get_json_data(b'0x010x020x03'))
+
+    def test_could_be_json(self):
+        self.assertIsNone(utils.get_json_data(b'{"hahaha, just kidding\x00'))
```

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/osc/fakes.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/fakes.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/osc/test_plugin.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/test_plugin.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/fakes.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/fakes.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_allocation.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_allocation.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_chassis.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_chassis.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_conductor.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_conductor.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_create.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_create.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_deploy_template.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_deploy_template.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_driver.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_driver.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_node.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
         # Get the command object to test
         self.cmd = baremetal_node.AbortBaremetalNode(self.app, None)
 
     def test_abort(self):
         arglist = ['node_uuid']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'abort'),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -66,88 +66,84 @@
 
         # Get the command object to test
         self.cmd = baremetal_node.AdoptBaremetalNode(self.app, None)
 
     def test_adopt(self):
         arglist = ['node_uuid']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'adopt'),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_provision_state.assert_called_once_with(
             'node_uuid', 'adopt',
             cleansteps=None, deploysteps=None, configdrive=None,
             rescue_password=None)
-
-    def test_adopt_no_wait(self):
-        arglist = ['node_uuid']
-        verifylist = [
-            ('node', 'node_uuid'),
-            ('provision_state', 'adopt')
-        ]
-
-        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
-
-        self.cmd.take_action(parsed_args)
-
         self.baremetal_mock.node.wait_for_provision_state.assert_not_called()
 
     def test_adopt_baremetal_provision_state_active_and_wait(self):
         arglist = ['node_uuid',
                    '--wait', '15']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'adopt'),
             ('wait_timeout', 15)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
+        test_node.set_provision_state.assert_called_once_with(
+            'node_uuid', 'adopt',
+            cleansteps=None, deploysteps=None, configdrive=None,
+            rescue_password=None)
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='active',
+            ['node_uuid'], expected_state='active',
             poll_interval=2, timeout=15)
 
     def test_adopt_baremetal_provision_state_default_wait(self):
         arglist = ['node_uuid',
                    '--wait']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'adopt'),
             ('wait_timeout', 0)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
+        test_node.set_provision_state.assert_called_once_with(
+            'node_uuid', 'adopt',
+            cleansteps=None, deploysteps=None, configdrive=None,
+            rescue_password=None)
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='active',
+            ['node_uuid'], expected_state='active',
             poll_interval=2, timeout=0)
 
 
 class TestClean(TestBaremetal):
     def setUp(self):
         super(TestClean, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.CleanBaremetalNode(self.app, None)
 
     def test_clean_without_steps(self):
         arglist = ['node_uuid']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'clean'),
         ]
 
         self.assertRaises(oscutils.ParserException, self.check_parser,
                           self.cmd, arglist, verifylist)
 
     def test_clean_with_steps(self):
@@ -163,15 +159,15 @@
         }
         steps_json = json.dumps(steps_dict)
 
         arglist = ['--clean-steps', steps_json, 'node_uuid']
         verifylist = [
             ('clean_steps', steps_json),
             ('provision_state', 'clean'),
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_provision_state.assert_called_once_with(
@@ -185,15 +181,15 @@
 
         # Get the command object to test
         self.cmd = baremetal_node.InspectBaremetalNode(self.app, None)
 
     def test_inspect(self):
         arglist = ['node_uuid']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'inspect'),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -208,15 +204,15 @@
 
         # Get the command object to test
         self.cmd = baremetal_node.ManageBaremetalNode(self.app, None)
 
     def test_manage(self):
         arglist = ['node_uuid']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'manage'),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -231,15 +227,15 @@
 
         # Get the command object to test
         self.cmd = baremetal_node.ProvideBaremetalNode(self.app, None)
 
     def test_provide(self):
         arglist = ['node_uuid']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'provide'),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -254,15 +250,15 @@
 
         # Get the command object to test
         self.cmd = baremetal_node.RebuildBaremetalNode(self.app, None)
 
     def test_rebuild(self):
         arglist = ['node_uuid']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'rebuild'),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -277,15 +273,15 @@
 
         # Get the command object to test
         self.cmd = baremetal_node.UndeployBaremetalNode(self.app, None)
 
     def test_undeploy(self):
         arglist = ['node_uuid']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'deleted'),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -299,40 +295,40 @@
         super(TestBootdeviceSet, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.BootdeviceSetBaremetalNode(self.app, None)
 
     def test_bootdevice_set(self):
         arglist = ['node_uuid', 'bios']
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('device', 'bios')]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_boot_device.assert_called_once_with(
             'node_uuid', 'bios', False)
 
     def test_bootdevice_set_persistent(self):
         arglist = ['node_uuid', 'bios', '--persistent']
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('device', 'bios'),
                       ('persistent', True)]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_boot_device.assert_called_once_with(
             'node_uuid', 'bios', True)
 
     def test_bootdevice_set_invalid_device(self):
         arglist = ['node_uuid', 'foo']
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('device', 'foo')]
 
         self.assertRaises(oscutils.ParserException,
                           self.check_parser,
                           self.cmd, arglist, verifylist)
 
     def test_bootdevice_set_device_only(self):
@@ -385,15 +381,15 @@
         super(TestConsoleDisable, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.ConsoleDisableBaremetalNode(self.app, None)
 
     def test_console_disable(self):
         arglist = ['node_uuid']
-        verifylist = [('node', 'node_uuid')]
+        verifylist = [('nodes', ['node_uuid'])]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_console_mode.assert_called_once_with(
             'node_uuid', False)
@@ -404,15 +400,15 @@
         super(TestConsoleEnable, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.ConsoleEnableBaremetalNode(self.app, None)
 
     def test_console_enable(self):
         arglist = ['node_uuid']
-        verifylist = [('node', 'node_uuid')]
+        verifylist = [('nodes', ['node_uuid'])]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_console_mode.assert_called_once_with(
             'node_uuid', True)
@@ -445,15 +441,15 @@
         super(TestSecurebootOff, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.SecurebootOffBaremetalNode(self.app, None)
 
     def test_secure_boot_off(self):
         arglist = ['node_uuid']
-        verifylist = [('node', 'node_uuid')]
+        verifylist = [('nodes', ['node_uuid'])]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_secure_boot.assert_called_once_with(
             'node_uuid', 'off')
@@ -464,15 +460,15 @@
         super(TestSecurebootOn, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.SecurebootOnBaremetalNode(self.app, None)
 
     def test_console_enable(self):
         arglist = ['node_uuid']
-        verifylist = [('node', 'node_uuid')]
+        verifylist = [('nodes', ['node_uuid'])]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_secure_boot.assert_called_once_with(
             'node_uuid', 'on')
@@ -482,18 +478,17 @@
     def setUp(self):
         super(TestBootmodeSet, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.BootmodeSetBaremetalNode(self.app, None)
 
     def test_baremetal_boot_mode_bios(self):
-        arglist = ['node_uuid',
-                   'bios']
+        arglist = ['node_uuid', 'bios']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('boot_mode', 'bios'),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -1441,15 +1436,15 @@
         # Get the command object to test
         self.cmd = baremetal_node.MaintenanceSetBaremetalNode(self.app, None)
 
     def test_baremetal_maintenance_on(self):
         arglist = ['node_uuid',
                    '--reason', 'maintenance reason']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('reason', 'maintenance reason'),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -1458,47 +1453,73 @@
             True,
             maint_reason='maintenance reason'
         )
 
     def test_baremetal_maintenance_on_no_reason(self):
         arglist = ['node_uuid']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_maintenance.assert_called_once_with(
             'node_uuid',
             True,
             maint_reason=None
         )
 
+    def test_baremetal_maintenance_on_several_nodes(self):
+        arglist = ['node_uuid', 'node_name']
+        verifylist = [
+            ('nodes', ['node_uuid', 'node_name']),
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+
+        self.baremetal_mock.node.set_maintenance.assert_has_calls(
+            [mock.call(n, True, maint_reason=None) for n in arglist]
+        )
+
 
 class TestBaremetalMaintenanceUnset(TestBaremetal):
     def setUp(self):
         super(TestBaremetalMaintenanceUnset, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.MaintenanceUnsetBaremetalNode(self.app, None)
 
     def test_baremetal_maintenance_off(self):
         arglist = ['node_uuid']
-        verifylist = [('node', 'node_uuid')]
+        verifylist = [('nodes', ['node_uuid'])]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_maintenance.assert_called_once_with(
             'node_uuid',
             False)
 
+    def test_baremetal_maintenance_off_several_nodes(self):
+        arglist = ['node_uuid', 'node_name']
+        verifylist = [('nodes', ['node_uuid', 'node_name'])]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+
+        self.baremetal_mock.node.set_maintenance.assert_has_calls(
+            [mock.call(n, False) for n in arglist]
+        )
+
 
 class TestPassthruCall(TestBaremetal):
     def setUp(self):
         super(TestPassthruCall, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.PassthruCallBaremetalNode(self.app, None)
@@ -1568,15 +1589,15 @@
         super(TestPower, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.PowerBaremetalNode(self.app, None)
 
     def test_baremetal_power(self):
         arglist = ['node_uuid']
-        verifylist = [('node', 'node_uuid')]
+        verifylist = [('nodes', ['node_uuid'])]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.assertRaisesRegex(AttributeError,
                                ".*no attribute 'POWER_STATE'",
                                self.cmd.take_action, parsed_args)
 
@@ -1586,54 +1607,54 @@
         super(TestPowerOff, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.PowerOffBaremetalNode(self.app, None)
 
     def test_baremetal_power_off(self):
         arglist = ['node_uuid']
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('soft', False),
                       ('power_timeout', None)]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_power_state.assert_called_once_with(
             'node_uuid', 'off', False, timeout=None)
 
     def test_baremetal_power_off_timeout(self):
         arglist = ['node_uuid', '--power-timeout', '2']
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('soft', False),
                       ('power_timeout', 2)]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_power_state.assert_called_once_with(
             'node_uuid', 'off', False, timeout=2)
 
     def test_baremetal_soft_power_off(self):
         arglist = ['node_uuid', '--soft']
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('soft', True),
                       ('power_timeout', None)]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_power_state.assert_called_once_with(
             'node_uuid', 'off', True, timeout=None)
 
     def test_baremetal_soft_power_off_timeout(self):
         arglist = ['node_uuid', '--soft', '--power-timeout', '2']
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('soft', True),
                       ('power_timeout', 2)]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -1644,37 +1665,51 @@
         arglist = []
         verifylist = []
 
         self.assertRaises(oscutils.ParserException,
                           self.check_parser,
                           self.cmd, arglist, verifylist)
 
+    def test_baremetal_power_off_several_nodes(self):
+        arglist = ['node_uuid', 'node_name']
+        verifylist = [('nodes', ['node_uuid', 'node_name']),
+                      ('soft', False),
+                      ('power_timeout', None)]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+
+        self.baremetal_mock.node.set_power_state.assert_has_calls([
+            mock.call(n, 'off', False, timeout=None) for n in arglist
+        ])
+
 
 class TestPowerOn(TestBaremetal):
     def setUp(self):
         super(TestPowerOn, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.PowerOnBaremetalNode(self.app, None)
 
     def test_baremetal_power_on(self):
         arglist = ['node_uuid']
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('power_timeout', None)]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_power_state.assert_called_once_with(
             'node_uuid', 'on', False, timeout=None)
 
     def test_baremetal_power_on_timeout(self):
         arglist = ['node_uuid', '--power-timeout', '2']
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('power_timeout', 2)]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_power_state.assert_called_once_with(
@@ -1697,15 +1732,15 @@
         self.cmd = baremetal_node.DeployBaremetalNode(self.app, None)
 
     def test_deploy_baremetal_provision_state_active_and_configdrive(self):
         arglist = ['node_uuid',
                    '--config-drive', 'path/to/drive',
                    '--deploy-steps', '[{"interface":"deploy"}]']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'active'),
             ('config_drive', 'path/to/drive'),
             ('deploy_steps', '[{"interface":"deploy"}]')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
@@ -1717,15 +1752,15 @@
             configdrive='path/to/drive', rescue_password=None)
 
     def test_deploy_baremetal_provision_state_active_and_configdrive_dict(
             self):
         arglist = ['node_uuid',
                    '--config-drive', '{"meta_data": {}}']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'active'),
             ('config_drive', '{"meta_data": {}}'),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
@@ -1734,62 +1769,85 @@
             'node_uuid', 'active',
             cleansteps=None, deploysteps=None, configdrive={'meta_data': {}},
             rescue_password=None)
 
     def test_deploy_no_wait(self):
         arglist = ['node_uuid']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'active')
         ]
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
         self.cmd.take_action(parsed_args)
         self.baremetal_mock.node.wait_for_provision_state.assert_not_called()
 
     def test_deploy_baremetal_provision_state_active_and_wait(self):
         arglist = ['node_uuid',
                    '--wait', '15']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'active'),
             ('wait_timeout', 15)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='active',
+            ['node_uuid'], expected_state='active',
             poll_interval=10, timeout=15)
 
     def test_deploy_baremetal_provision_state_default_wait(self):
         arglist = ['node_uuid',
                    '--wait']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'active'),
             ('wait_timeout', 0)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='active',
+            ['node_uuid'], expected_state='active',
             poll_interval=10, timeout=0)
 
+    def test_deploy_baremetal_provision_state_several_nodes(self):
+        arglist = ['node_uuid', 'node_name',
+                   '--wait', '15']
+        verifylist = [
+            ('nodes', ['node_uuid', 'node_name']),
+            ('provision_state', 'active'),
+            ('wait_timeout', 15)
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+
+        test_node = self.baremetal_mock.node
+        test_node.set_provision_state.assert_has_calls([
+            mock.call(n, 'active', cleansteps=None, deploysteps=None,
+                      configdrive=None, rescue_password=None)
+            for n in ['node_uuid', 'node_name']
+        ])
+        test_node.wait_for_provision_state.assert_called_once_with(
+            ['node_uuid', 'node_name'], expected_state='active',
+            poll_interval=10, timeout=15)
+
     def test_deploy_baremetal_provision_state_mismatch(self):
         arglist = ['node_uuid',
                    '--provision-state', 'abort']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'active'),
         ]
 
         self.assertRaises(oscutils.ParserException,
                           self.check_parser,
                           self.cmd, arglist, verifylist)
 
@@ -1800,72 +1858,72 @@
 
         # Get the command object to test
         self.cmd = baremetal_node.ManageBaremetalNode(self.app, None)
 
     def test_manage_no_wait(self):
         arglist = ['node_uuid']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'manage')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.wait_for_provision_state.assert_not_called()
 
     def test_manage_baremetal_provision_state_manageable_and_wait(self):
         arglist = ['node_uuid',
                    '--wait', '15']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'manage'),
             ('wait_timeout', 15)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='manageable',
+            ['node_uuid'], expected_state='manageable',
             poll_interval=2, timeout=15)
 
     def test_manage_baremetal_provision_state_default_wait(self):
         arglist = ['node_uuid',
                    '--wait']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'manage'),
             ('wait_timeout', 0)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='manageable',
+            ['node_uuid'], expected_state='manageable',
             poll_interval=2, timeout=0)
 
 
 class TestCleanBaremetalProvisionState(TestBaremetal):
     def setUp(self):
         super(TestCleanBaremetalProvisionState, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.CleanBaremetalNode(self.app, None)
 
     def test_clean_no_wait(self):
         arglist = ['node_uuid', '--clean-steps', '-']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'clean'),
             ('clean_steps', '-')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
@@ -1873,62 +1931,62 @@
         self.baremetal_mock.node.wait_for_provision_state.assert_not_called()
 
     def test_clean_baremetal_provision_state_manageable_and_wait(self):
         arglist = ['node_uuid',
                    '--wait', '15',
                    '--clean-steps', '-']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'clean'),
             ('wait_timeout', 15),
             ('clean_steps', '-')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='manageable',
+            ['node_uuid'], expected_state='manageable',
             poll_interval=10, timeout=15)
 
     def test_clean_baremetal_provision_state_default_wait(self):
         arglist = ['node_uuid',
                    '--wait',
                    '--clean-steps', '-']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'clean'),
             ('wait_timeout', 0),
             ('clean_steps', '-')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='manageable',
+            ['node_uuid'], expected_state='manageable',
             poll_interval=10, timeout=0)
 
 
 class TestRescueBaremetalProvisionState(TestBaremetal):
     def setUp(self):
         super(TestRescueBaremetalProvisionState, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.RescueBaremetalNode(self.app, None)
 
     def test_rescue_baremetal_no_wait(self):
         arglist = ['node_uuid',
                    '--rescue-password', 'supersecret']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'rescue'),
             ('rescue_password', 'supersecret'),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
@@ -1938,47 +1996,47 @@
             configdrive=None, rescue_password='supersecret')
 
     def test_rescue_baremetal_provision_state_rescue_and_wait(self):
         arglist = ['node_uuid',
                    '--wait', '15',
                    '--rescue-password', 'supersecret']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'rescue'),
             ('rescue_password', 'supersecret'),
             ('wait_timeout', 15)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='rescue',
+            ['node_uuid'], expected_state='rescue',
             poll_interval=10, timeout=15)
 
     def test_rescue_baremetal_provision_state_default_wait(self):
         arglist = ['node_uuid',
                    '--wait',
                    '--rescue-password', 'supersecret']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'rescue'),
             ('rescue_password', 'supersecret'),
             ('wait_timeout', 0)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='rescue',
+            ['node_uuid'], expected_state='rescue',
             poll_interval=10, timeout=0)
 
     def test_rescue_baremetal_no_rescue_password(self):
         arglist = ['node_uuid']
         verifylist = [('node', 'node_uuid'),
                       ('provision_state', 'rescue')]
 
@@ -1993,115 +2051,115 @@
 
         # Get the command object to test
         self.cmd = baremetal_node.InspectBaremetalNode(self.app, None)
 
     def test_inspect_no_wait(self):
         arglist = ['node_uuid']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'inspect')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.wait_for_provision_state.assert_not_called()
 
     def test_inspect_baremetal_provision_state_managable_and_wait(self):
         arglist = ['node_uuid',
                    '--wait', '15']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'inspect'),
             ('wait_timeout', 15)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='manageable',
+            ['node_uuid'], expected_state='manageable',
             poll_interval=2, timeout=15)
 
     def test_inspect_baremetal_provision_state_default_wait(self):
         arglist = ['node_uuid',
                    '--wait']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'inspect'),
             ('wait_timeout', 0)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='manageable',
+            ['node_uuid'], expected_state='manageable',
             poll_interval=2, timeout=0)
 
 
 class TestProvideBaremetalProvisionState(TestBaremetal):
     def setUp(self):
         super(TestProvideBaremetalProvisionState, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.ProvideBaremetalNode(self.app, None)
 
     def test_provide_no_wait(self):
         arglist = ['node_uuid']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'provide')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.wait_for_provision_state.assert_not_called()
 
     def test_provide_baremetal_provision_state_available_and_wait(self):
         arglist = ['node_uuid',
                    '--wait', '15']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'provide'),
             ('wait_timeout', 15)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='available',
+            ['node_uuid'], expected_state='available',
             poll_interval=10, timeout=15)
 
     def test_provide_baremetal_provision_state_default_wait(self):
         arglist = ['node_uuid',
                    '--wait']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'provide'),
             ('wait_timeout', 0)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='available',
+            ['node_uuid'], expected_state='available',
             poll_interval=10, timeout=0)
 
 
 class TestRebuildBaremetalProvisionState(TestBaremetal):
     def setUp(self):
         super(TestRebuildBaremetalProvisionState, self).setUp()
 
@@ -2109,15 +2167,15 @@
         self.cmd = baremetal_node.RebuildBaremetalNode(self.app, None)
 
     def test_rebuild_baremetal_provision_state_active_and_configdrive(self):
         arglist = ['node_uuid',
                    '--config-drive', 'path/to/drive',
                    '--deploy-steps', '[{"interface":"deploy"}]']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'rebuild'),
             ('config_drive', 'path/to/drive'),
             ('deploy_steps', '[{"interface":"deploy"}]')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
@@ -2127,15 +2185,15 @@
             'node_uuid', 'rebuild',
             cleansteps=None, deploysteps=[{"interface": "deploy"}],
             configdrive='path/to/drive', rescue_password=None)
 
     def test_rebuild_no_wait(self):
         arglist = ['node_uuid']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'rebuild')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2146,115 +2204,115 @@
 
         self.baremetal_mock.node.wait_for_provision_state.assert_not_called()
 
     def test_rebuild_baremetal_provision_state_active_and_wait(self):
         arglist = ['node_uuid',
                    '--wait', '15']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'rebuild'),
             ('wait_timeout', 15)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='active',
+            ['node_uuid'], expected_state='active',
             poll_interval=10, timeout=15)
 
     def test_rebuild_baremetal_provision_state_default_wait(self):
         arglist = ['node_uuid',
                    '--wait']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'rebuild'),
             ('wait_timeout', 0)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='active',
+            ['node_uuid'], expected_state='active',
             poll_interval=10, timeout=0)
 
 
 class TestUndeployBaremetalProvisionState(TestBaremetal):
     def setUp(self):
         super(TestUndeployBaremetalProvisionState, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.UndeployBaremetalNode(self.app, None)
 
     def test_undeploy_no_wait(self):
         arglist = ['node_uuid']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'deleted')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.wait_for_provision_state.assert_not_called()
 
     def test_undeploy_baremetal_provision_state_available_and_wait(self):
         arglist = ['node_uuid',
                    '--wait', '15']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'deleted'),
             ('wait_timeout', 15)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='available',
+            ['node_uuid'], expected_state='available',
             poll_interval=10, timeout=15)
 
     def test_undeploy_baremetal_provision_state_default_wait(self):
         arglist = ['node_uuid',
                    '--wait']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'deleted'),
             ('wait_timeout', 0)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='available',
+            ['node_uuid'], expected_state='available',
             poll_interval=10, timeout=0)
 
 
 class TestUnrescueBaremetalProvisionState(TestBaremetal):
     def setUp(self):
         super(TestUnrescueBaremetalProvisionState, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.UnrescueBaremetalNode(self.app, None)
 
     def test_unrescue_no_wait(self):
         arglist = ['node_uuid']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'unrescue'),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2262,44 +2320,44 @@
             'node_uuid', 'unrescue', cleansteps=None, deploysteps=None,
             configdrive=None, rescue_password=None)
 
     def test_unrescue_baremetal_provision_state_active_and_wait(self):
         arglist = ['node_uuid',
                    '--wait', '15']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'unrescue'),
             ('wait_timeout', 15)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='active',
+            ['node_uuid'], expected_state='active',
             poll_interval=10, timeout=15)
 
     def test_unrescue_baremetal_provision_state_default_wait(self):
         arglist = ['node_uuid',
                    '--wait']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('provision_state', 'unrescue'),
             ('wait_timeout', 0)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
-            'node_uuid', expected_state='active',
+            ['node_uuid'], expected_state='active',
             poll_interval=10, timeout=0)
 
 
 class TestBaremetalReboot(TestBaremetal):
     def setUp(self):
         super(TestBaremetalReboot, self).setUp()
 
@@ -2312,54 +2370,54 @@
 
         self.assertRaises(oscutils.ParserException,
                           self.check_parser,
                           self.cmd, arglist, verifylist)
 
     def test_baremetal_reboot_uuid_only(self):
         arglist = ['node_uuid']
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('soft', False),
                       ('power_timeout', None)]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_power_state.assert_called_once_with(
             'node_uuid', 'reboot', False, timeout=None)
 
     def test_baremetal_reboot_timeout(self):
         arglist = ['node_uuid', '--power-timeout', '2']
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('soft', False),
                       ('power_timeout', 2)]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_power_state.assert_called_once_with(
             'node_uuid', 'reboot', False, timeout=2)
 
     def test_baremetal_soft_reboot(self):
         arglist = ['node_uuid', '--soft']
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('soft', True),
                       ('power_timeout', None)]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_power_state.assert_called_once_with(
             'node_uuid', 'reboot', True, timeout=None)
 
     def test_baremetal_soft_reboot_timeout(self):
         arglist = ['node_uuid', '--soft', '--power-timeout', '2']
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('soft', True),
                       ('power_timeout', 2)]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2388,25 +2446,25 @@
         self.assertRaises(oscutils.ParserException,
                           self.check_parser,
                           self.cmd, arglist, verifylist)
 
     def test_baremetal_set_no_property(self):
         arglist = ['node_uuid']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
         self.cmd.take_action(parsed_args)
         self.assertFalse(self.baremetal_mock.node.update.called)
 
     def test_baremetal_set_one_property(self):
         arglist = ['node_uuid', '--property', 'path/to/property=value']
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('property', ['path/to/property=value']),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2420,15 +2478,15 @@
     def test_baremetal_set_multiple_properties(self):
         arglist = [
             'node_uuid',
             '--property', 'path/to/property=value',
             '--property', 'other/path=value2'
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('property',
              [
                  'path/to/property=value',
                  'other/path=value2',
              ]),
         ]
 
@@ -2449,15 +2507,15 @@
 
     def test_baremetal_set_instance_uuid(self):
         arglist = [
             'node_uuid',
             '--instance-uuid', 'xxxxx',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('instance_uuid', 'xxxxx')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2469,15 +2527,15 @@
 
     def test_baremetal_set_name(self):
         arglist = [
             'node_uuid',
             '--name', 'xxxxx',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('name', 'xxxxx')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2490,15 +2548,15 @@
     def test_baremetal_set_chassis(self):
         chassis = '4f4135ea-7e58-4e3d-bcc4-b87ca16e980b'
         arglist = [
             'node_uuid',
             '--chassis-uuid', chassis,
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('chassis_uuid', chassis)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2510,15 +2568,15 @@
 
     def test_baremetal_set_driver(self):
         arglist = [
             'node_uuid',
             '--driver', 'xxxxx',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('driver', 'xxxxx')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2531,15 +2589,15 @@
     def test_baremetal_set_driver_reset_interfaces(self):
         arglist = [
             'node_uuid',
             '--driver', 'xxxxx',
             '--reset-interfaces',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('driver', 'xxxxx'),
             ('reset_interfaces', True),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
@@ -2552,15 +2610,15 @@
 
     def test_reset_interfaces_without_driver(self):
         arglist = [
             'node_uuid',
             '--reset-interfaces',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('reset_interfaces', True),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.assertRaises(exc.CommandError,
                           self.cmd.take_action, parsed_args)
@@ -2568,15 +2626,15 @@
 
     def _test_baremetal_set_hardware_interface(self, interface):
         arglist = [
             'node_uuid',
             '--%s-interface' % interface, 'xxxxx',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('%s_interface' % interface, 'xxxxx')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2625,15 +2683,15 @@
 
     def _test_baremetal_reset_hardware_interface(self, interface):
         arglist = [
             'node_uuid',
             '--reset-%s-interface' % interface,
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('reset_%s_interface' % interface, True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2681,15 +2739,15 @@
 
     def test_baremetal_set_resource_class(self):
         arglist = [
             'node_uuid',
             '--resource-class', 'foo',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('resource_class', 'foo')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2701,15 +2759,15 @@
 
     def test_baremetal_set_conductor_group(self):
         arglist = [
             'node_uuid',
             '--conductor-group', 'foo',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('conductor_group', 'foo')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2721,15 +2779,15 @@
 
     def test_baremetal_set_automated_clean(self):
         arglist = [
             'node_uuid',
             '--automated-clean'
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('automated_clean', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2741,15 +2799,15 @@
 
     def test_baremetal_set_no_automated_clean(self):
         arglist = [
             'node_uuid',
             '--no-automated-clean'
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('automated_clean', False)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2761,15 +2819,15 @@
 
     def test_baremetal_set_protected(self):
         arglist = [
             'node_uuid',
             '--protected'
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('protected', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2782,15 +2840,15 @@
     def test_baremetal_set_protected_with_reason(self):
         arglist = [
             'node_uuid',
             '--protected',
             '--protected-reason', 'reason!'
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('protected', True),
             ('protected_reason', 'reason!')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
@@ -2804,15 +2862,15 @@
 
     def test_baremetal_set_retired(self):
         arglist = [
             'node_uuid',
             '--retired'
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('retired', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2825,15 +2883,15 @@
     def test_baremetal_set_retired_with_reason(self):
         arglist = [
             'node_uuid',
             '--retired',
             '--retired-reason', 'out of warranty!'
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('retired', True),
             ('retired_reason', 'out of warranty!')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
@@ -2848,15 +2906,15 @@
 
     def test_baremetal_set_extra(self):
         arglist = [
             'node_uuid',
             '--extra', 'foo=bar',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('extra', ['foo=bar'])
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2868,15 +2926,15 @@
 
     def test_baremetal_set_driver_info(self):
         arglist = [
             'node_uuid',
             '--driver-info', 'foo=bar',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('driver_info', ['foo=bar'])
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2888,15 +2946,15 @@
 
     def test_baremetal_set_instance_info(self):
         arglist = [
             'node_uuid',
             '--instance-info', 'foo=bar',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('instance_info', ['foo=bar'])
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -2912,15 +2970,15 @@
         self.cmd.log = mock.Mock(autospec=True)
         target_raid_config_string = '{"raid": "config"}'
         expected_target_raid_config = {'raid': 'config'}
         mock_handle.return_value = expected_target_raid_config.copy()
 
         arglist = ['node_uuid',
                    '--target-raid-config', target_raid_config_string]
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('target_raid_config', target_raid_config_string)]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
         self.cmd.take_action(parsed_args)
 
         self.cmd.log.warning.assert_not_called()
         self.assertFalse(mock_stdin.called)
@@ -2937,15 +2995,15 @@
         target_raid_config_string = '{"raid": "config"}'
         expected_target_raid_config = {'raid': 'config'}
         mock_handle.return_value = expected_target_raid_config.copy()
 
         arglist = ['node_uuid',
                    '--name', 'xxxxx',
                    '--target-raid-config', target_raid_config_string]
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('name', 'xxxxx'),
                       ('target_raid_config', target_raid_config_string)]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
         self.cmd.take_action(parsed_args)
 
         self.cmd.log.warning.assert_not_called()
@@ -2967,15 +3025,15 @@
         target_raid_config_string = '{"raid": "config"}'
         expected_target_raid_config = {'raid': 'config'}
         mock_stdin.return_value = target_raid_config_string
         mock_handle.return_value = expected_target_raid_config.copy()
 
         arglist = ['node_uuid',
                    '--target-raid-config', target_value]
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('target_raid_config', target_value)]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
         self.cmd.take_action(parsed_args)
 
         self.cmd.log.warning.assert_not_called()
         mock_stdin.assert_called_once_with('target_raid_config')
@@ -2990,15 +3048,15 @@
             self, mock_handle, mock_stdin):
         self.cmd.log = mock.Mock(autospec=True)
         target_value = '-'
         mock_stdin.side_effect = exc.InvalidAttribute('bad')
 
         arglist = ['node_uuid',
                    '--target-raid-config', target_value]
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('target_raid_config', target_value)]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
         self.assertRaises(exc.InvalidAttribute,
                           self.cmd.take_action, parsed_args)
 
         self.cmd.log.warning.assert_not_called()
@@ -3010,15 +3068,15 @@
 
     def test_baremetal_set_owner(self):
         arglist = [
             'node_uuid',
             '--owner', 'owner 1',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('owner', 'owner 1')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3032,15 +3090,15 @@
 
     def test_baremetal_set_description(self):
         arglist = [
             'node_uuid',
             '--description', 'there is no spoon',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('description', 'there is no spoon')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3054,15 +3112,15 @@
 
     def test_baremetal_set_lessee(self):
         arglist = [
             'node_uuid',
             '--lessee', 'lessee 1',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('lessee', 'lessee 1')
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3079,15 +3137,15 @@
         self.cmd.log = mock.Mock(autospec=True)
         network_data_string = '{"a": ["b"]}'
         expected_network_data = {'a': ['b']}
         mock_handle.return_value = expected_network_data.copy()
 
         arglist = ['node_uuid',
                    '--network-data', network_data_string]
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('network_data', network_data_string)]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.update.assert_called_once_with(
@@ -3269,38 +3327,38 @@
 
         self.assertRaises(oscutils.ParserException,
                           self.check_parser,
                           self.cmd, arglist, verifylist)
 
     def test_baremetal_unset_no_property(self):
         arglist = ['node_uuid']
-        verifylist = [('node', 'node_uuid')]
+        verifylist = [('nodes', ['node_uuid'])]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
         self.cmd.take_action(parsed_args)
         self.assertFalse(self.baremetal_mock.node.update.called)
 
     def test_baremetal_unset_one_property(self):
         arglist = ['node_uuid', '--property', 'path/to/property']
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('property', ['path/to/property'])]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.update.assert_called_once_with(
             'node_uuid',
             [{'path': '/properties/path/to/property', 'op': 'remove'}])
 
     def test_baremetal_unset_multiple_properties(self):
         arglist = ['node_uuid',
                    '--property', 'path/to/property',
                    '--property', 'other/path']
-        verifylist = [('node', 'node_uuid'),
+        verifylist = [('nodes', ['node_uuid']),
                       ('property',
                        ['path/to/property',
                         'other/path'])]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
@@ -3313,15 +3371,15 @@
 
     def test_baremetal_unset_instance_uuid(self):
         arglist = [
             'node_uuid',
             '--instance-uuid',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('instance_uuid', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3332,15 +3390,15 @@
 
     def test_baremetal_unset_name(self):
         arglist = [
             'node_uuid',
             '--name',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('name', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3351,15 +3409,15 @@
 
     def test_baremetal_unset_resource_class(self):
         arglist = [
             'node_uuid',
             '--resource-class',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('resource_class', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3370,15 +3428,15 @@
 
     def test_baremetal_unset_conductor_group(self):
         arglist = [
             'node_uuid',
             '--conductor-group',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('conductor_group', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3389,15 +3447,15 @@
 
     def test_baremetal_unset_automated_clean(self):
         arglist = [
             'node_uuid',
             '--automated-clean',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('automated_clean', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3408,15 +3466,15 @@
 
     def test_baremetal_unset_protected(self):
         arglist = [
             'node_uuid',
             '--protected',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('protected', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3427,15 +3485,15 @@
 
     def test_baremetal_unset_protected_reason(self):
         arglist = [
             'node_uuid',
             '--protected-reason',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('protected_reason', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3446,15 +3504,15 @@
 
     def test_baremetal_unset_retired(self):
         arglist = [
             'node_uuid',
             '--retired',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('retired', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3465,15 +3523,15 @@
 
     def test_baremetal_unset_retired_reason(self):
         arglist = [
             'node_uuid',
             '--retired-reason',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('retired_reason', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3484,15 +3542,15 @@
 
     def test_baremetal_unset_extra(self):
         arglist = [
             'node_uuid',
             '--extra', 'foo',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('extra', ['foo'])
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3503,15 +3561,15 @@
 
     def test_baremetal_unset_driver_info(self):
         arglist = [
             'node_uuid',
             '--driver-info', 'foo',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('driver_info', ['foo'])
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3522,15 +3580,15 @@
 
     def test_baremetal_unset_instance_info(self):
         arglist = [
             'node_uuid',
             '--instance-info', 'foo',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('instance_info', ['foo'])
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3542,15 +3600,15 @@
     def test_baremetal_unset_target_raid_config(self):
         self.cmd.log = mock.Mock(autospec=True)
         arglist = [
             'node_uuid',
             '--target-raid-config',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('target_raid_config', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3563,15 +3621,15 @@
         self.cmd.log = mock.Mock(autospec=True)
         arglist = [
             'node_uuid',
             '--name',
             '--target-raid-config',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('name', True),
             ('target_raid_config', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
@@ -3586,15 +3644,15 @@
 
     def test_baremetal_unset_chassis_uuid(self):
         arglist = [
             'node_uuid',
             '--chassis-uuid',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('chassis_uuid', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3605,15 +3663,15 @@
 
     def _test_baremetal_unset_hw_interface(self, interface):
         arglist = [
             'node_uuid',
             '--%s-interface' % interface,
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('%s_interface' % interface, True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3660,15 +3718,15 @@
 
     def test_baremetal_unset_owner(self):
         arglist = [
             'node_uuid',
             '--owner',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('owner', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3679,15 +3737,15 @@
 
     def test_baremetal_unset_description(self):
         arglist = [
             'node_uuid',
             '--description',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('description', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3698,15 +3756,15 @@
 
     def test_baremetal_unset_lessee(self):
         arglist = [
             'node_uuid',
             '--lessee',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('lessee', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3717,15 +3775,15 @@
 
     def test_baremetal_unset_network_data(self):
         arglist = [
             'node_uuid',
             '--network-data',
         ]
         verifylist = [
-            ('node', 'node_uuid'),
+            ('nodes', ['node_uuid']),
             ('network_data', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
@@ -3879,15 +3937,15 @@
 
         self.assertRaises(oscutils.ParserException,
                           self.check_parser,
                           self.cmd, arglist, verifylist)
 
     def test_baremetal_inject_nmi_uuid(self):
         arglist = ['node_uuid']
-        verifylist = [('node', 'node_uuid')]
+        verifylist = [('nodes', ['node_uuid'])]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.inject_nmi.assert_called_once_with(
             'node_uuid')
```

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_port.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_port.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_portgroup.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_portgroup.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_connector.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_connector.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_target.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_target.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/test_client.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/test_exc.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/test_exc.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/test_import.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/test_import.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/utils.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_allocation.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_allocation.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_chassis.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_chassis.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_client.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_client.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_conductor.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_conductor.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_create_resources.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_create_resources.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_deploy_template.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_deploy_template.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_driver.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_driver.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_events.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_events.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_node.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -1595,14 +1595,31 @@
         body = {'target': target_state,
                 'configdrive': file_content.decode('utf-8')}
         expect = [
             ('PUT', '/v1/nodes/%s/states/provision' % NODE1['uuid'], {}, body),
         ]
         self.assertEqual(expect, self.api.calls)
 
+    def test_node_set_provision_state_with_configdrive_json_file(self):
+        target_state = 'active'
+        file_content = b'{"user_data": "foo bar"}'
+
+        with tempfile.NamedTemporaryFile() as f:
+            f.write(file_content)
+            f.flush()
+            self.mgr.set_provision_state(NODE1['uuid'], target_state,
+                                         configdrive=f.name)
+
+        body = {'target': target_state,
+                'configdrive': {"user_data": "foo bar"}}
+        expect = [
+            ('PUT', '/v1/nodes/%s/states/provision' % NODE1['uuid'], {}, body),
+        ]
+        self.assertEqual(expect, self.api.calls)
+
     @mock.patch.object(common_utils, 'make_configdrive', autospec=True)
     def test_node_set_provision_state_with_configdrive_dir(self,
                                                            mock_configdrive):
         mock_configdrive.return_value = 'fake-configdrive'
         target_state = 'active'
 
         with common_utils.tempdir() as dirname:
@@ -2010,14 +2027,86 @@
         mock_get.assert_called_with(
             self.mgr, 'node',
             os_ironic_api_version=None, global_request_id=None)
         self.assertEqual(4, mock_get.call_count)
         mock_sleep.assert_called_with(node._DEFAULT_POLL_INTERVAL)
         self.assertEqual(3, mock_sleep.call_count)
 
+    @mock.patch.object(time, 'sleep', autospec=True)
+    @mock.patch.object(node.NodeManager, 'get', autospec=True)
+    def test_wait_for_provision_state_several(self, mock_get, mock_sleep):
+        mock_get.side_effect = [
+            self._fake_node_for_wait('deploying', target='active'),
+            # Sometimes non-fatal errors can be recorded in last_error
+            self._fake_node_for_wait('deploying', target='active',
+                                     error='Node locked'),
+            self._fake_node_for_wait('deploying', target='active'),
+            self._fake_node_for_wait('deploying', target='active'),
+            self._fake_node_for_wait('active'),
+            self._fake_node_for_wait('active'),
+        ]
+
+        self.mgr.wait_for_provision_state(['node1', 'node2'], 'active')
+
+        mock_get.assert_has_calls([
+            mock.call(self.mgr, 'node1', os_ironic_api_version=None,
+                      global_request_id=None),
+            mock.call(self.mgr, 'node2', os_ironic_api_version=None,
+                      global_request_id=None),
+        ], any_order=True)
+        self.assertEqual(6, mock_get.call_count)
+        mock_sleep.assert_called_with(node._DEFAULT_POLL_INTERVAL)
+        self.assertEqual(2, mock_sleep.call_count)
+
+    @mock.patch.object(time, 'sleep', autospec=True)
+    @mock.patch.object(node.NodeManager, 'get', autospec=True)
+    def test_wait_for_provision_state_one_failed(self, mock_get, mock_sleep):
+        mock_get.side_effect = [
+            self._fake_node_for_wait('deploying', target='active'),
+            self._fake_node_for_wait('deploying', target='active'),
+            self._fake_node_for_wait('active'),
+            self._fake_node_for_wait('deploy failed', error='boom'),
+        ]
+
+        self.assertRaisesRegex(exc.StateTransitionFailed,
+                               'boom',
+                               self.mgr.wait_for_provision_state,
+                               ['node1', 'node2'], 'active')
+
+        mock_get.assert_has_calls([
+            mock.call(self.mgr, 'node1', os_ironic_api_version=None,
+                      global_request_id=None),
+            mock.call(self.mgr, 'node2', os_ironic_api_version=None,
+                      global_request_id=None),
+        ], any_order=True)
+        self.assertEqual(4, mock_get.call_count)
+        mock_sleep.assert_called_with(node._DEFAULT_POLL_INTERVAL)
+        self.assertEqual(1, mock_sleep.call_count)
+
+    @mock.patch.object(time, 'sleep', autospec=True)
+    @mock.patch.object(node.NodeManager, 'get', autospec=True)
+    def test_wait_for_provision_state_one_timeout(self, mock_get, mock_sleep):
+        fake_waiting_node = self._fake_node_for_wait(
+            'deploying', target='active')
+        fake_success_node = self._fake_node_for_wait('active')
+
+        def side_effect(node_manager, node_ident, *args, **kwargs):
+            if node_ident == 'node1':
+                return fake_success_node
+            else:
+                return fake_waiting_node
+
+        mock_get.side_effect = side_effect
+
+        self.assertRaisesRegex(exc.StateTransitionTimeout,
+                               r'Node\(s\) node2',
+                               self.mgr.wait_for_provision_state,
+                               ['node1', 'node2'], 'active',
+                               timeout=0.001)
+
     def test_node_get_traits(self):
         traits = self.mgr.get_traits(NODE1['uuid'])
         expect = [
             ('GET', '/v1/nodes/%s/traits' % NODE1['uuid'], {}, None),
         ]
         self.assertEqual(expect, self.api.calls)
         self.assertEqual(TRAITS['traits'], traits)
```

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_port.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_port.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_portgroup.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_portgroup.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_resource_fields.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_resource_fields.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_volume_connector.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_volume_connector.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/tests/unit/v1/test_volume_target.py` & `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_volume_target.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/v1/allocation.py` & `python-ironicclient-5.2.0/ironicclient/v1/allocation.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/v1/chassis.py` & `python-ironicclient-5.2.0/ironicclient/v1/chassis.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/v1/client.py` & `python-ironicclient-5.2.0/ironicclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/v1/conductor.py` & `python-ironicclient-5.2.0/ironicclient/v1/conductor.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/v1/create_resources.py` & `python-ironicclient-5.2.0/ironicclient/v1/create_resources.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/v1/deploy_template.py` & `python-ironicclient-5.2.0/ironicclient/v1/deploy_template.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/v1/driver.py` & `python-ironicclient-5.2.0/ironicclient/v1/driver.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/v1/events.py` & `python-ironicclient-5.2.0/ironicclient/v1/events.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/v1/node.py` & `python-ironicclient-5.2.0/ironicclient/v1/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -680,21 +680,26 @@
             global_request_id=None, deploysteps=None):
         """Set the provision state for the node.
 
         :param node_uuid: The UUID or name of the node.
         :param state: The desired provision state. One of 'active', 'deleted',
              'rebuild', 'inspect', 'provide', 'manage', 'clean', 'abort',
              'rescue', 'unrescue'.
-        :param configdrive: A gzipped, base64-encoded configuration drive
-            string OR the path to the configuration drive file OR the path to
-            a directory containing the config drive files OR a dictionary to
-            build config drive from. In case it's a directory, a config drive
-            will be generated from it. In case it's a dictionary, a config
-            drive will be generated on the server side (requires API version
-            1.56). This is only valid when setting state to 'active'.
+        :param configdrive: One of:
+
+            * a gzipped, base64-encoded configuration drive string
+            * a dictionary to build config drive from
+            * a path to the configuration drive file (ISO 9660 or VFAT)
+            * a path to a directory containing the config drive files
+            * a path to a JSON file to build config from
+
+            In case it's a directory, a config drive will be generated from
+            it. In case it's a dictionary or a JSON file, a config drive will
+            be generated on the server side (requires API version 1.56).
+            This is only valid when setting state to 'active'.
         :param cleansteps: The clean steps as a list of clean-step
             dictionaries; each dictionary should have keys 'interface' and
             'step', and optional key 'args'. This must be specified (and is
             only valid) when setting provision-state to 'clean'.
         :param rescue_password: A string to be used as the login password
             inside the rescue ramdisk once a node is rescued. This must be
             specified (and is only valid) when setting 'state' to 'rescue'.
@@ -714,14 +719,17 @@
         path = "%s/states/provision" % node_uuid
         body = {'target': state}
         if configdrive:
             if isinstance(configdrive, str):
                 if os.path.isfile(configdrive):
                     with open(configdrive, 'rb') as f:
                         configdrive = f.read()
+                    json_data = utils.get_json_data(configdrive)
+                    if json_data is not None:
+                        configdrive = json_data
                 elif os.path.isdir(configdrive):
                     configdrive = utils.make_configdrive(configdrive)
                 else:
                     raise ValueError('Config drive seems to refer to a file '
                                      'or directory but this file/directory '
                                      'does not exist: %s.' % configdrive)
 
@@ -936,32 +944,69 @@
             path += '?' + '&'.join(filters)
 
         return self._list_primitives(
             self._path(path), 'bios',
             os_ironic_api_version=os_ironic_api_version,
             global_request_id=global_request_id)
 
+    def _check_one_provision_state(self, node_ident, expected_state,
+                                   fail_on_unexpected_state=True,
+                                   os_ironic_api_version=None,
+                                   global_request_id=None):
+        # TODO(dtantsur): use version negotiation to request API 1.8 and use
+        # the "fields" argument to reduce amount of data sent.
+        node = self.get(
+            node_ident, os_ironic_api_version=os_ironic_api_version,
+            global_request_id=global_request_id)
+        if node.provision_state == expected_state:
+            LOG.debug('Node %(node)s reached provision state %(state)s',
+                      {'node': node_ident, 'state': expected_state})
+            return True
+
+        # Note that if expected_state == 'error' we still succeed
+        if (node.provision_state == 'error'
+                or node.provision_state.endswith(' failed')):
+            raise exc.StateTransitionFailed(
+                _('Node %(node)s failed to reach state %(state)s. '
+                    'It\'s in state %(actual)s, and has error: %(error)s') %
+                {'node': node_ident, 'state': expected_state,
+                    'actual': node.provision_state, 'error': node.last_error})
+
+        if fail_on_unexpected_state and not node.target_provision_state:
+            raise exc.StateTransitionFailed(
+                _('Node %(node)s failed to reach state %(state)s. '
+                    'It\'s in unexpected stable state %(actual)s') %
+                {'node': node_ident, 'state': expected_state,
+                 'actual': node.provision_state})
+
+        LOG.debug('Still waiting for node %(node)s to reach state '
+                  '%(state)s, the current state is %(actual)s',
+                  {'node': node_ident, 'state': expected_state,
+                   'actual': node.provision_state})
+
+        return False
+
     def wait_for_provision_state(self, node_ident, expected_state,
                                  timeout=0,
                                  poll_interval=_DEFAULT_POLL_INTERVAL,
                                  poll_delay_function=None,
                                  fail_on_unexpected_state=True,
                                  os_ironic_api_version=None,
                                  global_request_id=None):
-        """Helper function to wait for a node to reach a given state.
+        """Helper function to wait for nodes to reach a given state.
 
         Polls Ironic API in a loop until node gets to a requested state.
 
         Fails in the following cases:
         * Timeout (if provided) is reached
         * Node's last_error gets set to a non-empty value
         * Unexpected stable state is reached and fail_on_unexpected_state is on
         * Error state is reached (if it's not equal to expected_state)
 
-        :param node_ident: node UUID or name
+        :param node_ident: node UUID or name (one or a list)
         :param expected_state: expected final provision state
         :param timeout: timeout in seconds, no timeout if 0
         :param poll_interval: interval in seconds between 2 poll
         :param poll_delay_function: function to use to wait between polls
             (defaults to time.sleep). Should take one argument - delay time
             in seconds. Any exceptions raised inside it will abort the wait.
         :param fail_on_unexpected_state: whether to fail if the nodes
@@ -971,51 +1016,40 @@
         :param global_request_id: String containing global request ID header
             value (in form "req-<UUID>") to use for the request.
 
         :raises: StateTransitionFailed if node reached an error state
         :raises: StateTransitionTimeout on timeout
         """
         expected_state = expected_state.lower()
-        timeout_msg = _('Node %(node)s failed to reach state %(state)s in '
-                        '%(timeout)s seconds') % {'node': node_ident,
-                                                  'state': expected_state,
-                                                  'timeout': timeout}
+        if not isinstance(node_ident, list):
+            node_ident = [node_ident]
+        unfinished = node_ident
+
+        def _timeout():
+            return (
+                _('Node(s) %(node)s failed to reach state %(state)s in '
+                  '%(timeout)s seconds')
+                % {'node': ', '.join(unfinished),
+                   'state': expected_state,
+                   'timeout': timeout}
+            )
 
-        # TODO(dtantsur): use version negotiation to request API 1.8 and use
-        # the "fields" argument to reduce amount of data sent.
         for _count in utils.poll(timeout, poll_interval, poll_delay_function,
-                                 timeout_msg):
-            node = self.get(
-                node_ident, os_ironic_api_version=os_ironic_api_version,
-                global_request_id=global_request_id)
-            if node.provision_state == expected_state:
-                LOG.debug('Node %(node)s reached provision state %(state)s',
-                          {'node': node_ident, 'state': expected_state})
-                return
-
-            # Note that if expected_state == 'error' we still succeed
-            if (node.provision_state == 'error'
-                    or node.provision_state.endswith(' failed')):
-                raise exc.StateTransitionFailed(
-                    _('Node %(node)s failed to reach state %(state)s. '
-                      'It\'s in state %(actual)s, and has error: %(error)s') %
-                    {'node': node_ident, 'state': expected_state,
-                     'actual': node.provision_state, 'error': node.last_error})
-
-            if fail_on_unexpected_state and not node.target_provision_state:
-                raise exc.StateTransitionFailed(
-                    _('Node %(node)s failed to reach state %(state)s. '
-                      'It\'s in unexpected stable state %(actual)s') %
-                    {'node': node_ident, 'state': expected_state,
-                     'actual': node.provision_state})
-
-            LOG.debug('Still waiting for node %(node)s to reach state '
-                      '%(state)s, the current state is %(actual)s',
-                      {'node': node_ident, 'state': expected_state,
-                       'actual': node.provision_state})
+                                 _timeout):
+            current, unfinished = unfinished, []
+            for node in current:
+                if not self._check_one_provision_state(
+                        node,
+                        expected_state,
+                        fail_on_unexpected_state=fail_on_unexpected_state,
+                        os_ironic_api_version=os_ironic_api_version,
+                        global_request_id=global_request_id):
+                    unfinished.append(node)
+            if not unfinished:
+                break
 
     def get_history_list(self,
                          node_ident,
                          detail=False,
                          os_ironic_api_version=None,
                          global_request_id=None):
         """Get node history event list.
```

### Comparing `python-ironicclient-5.1.0/ironicclient/v1/port.py` & `python-ironicclient-5.2.0/ironicclient/v1/port.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/v1/portgroup.py` & `python-ironicclient-5.2.0/ironicclient/v1/portgroup.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/v1/resource_fields.py` & `python-ironicclient-5.2.0/ironicclient/v1/resource_fields.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/v1/utils.py` & `python-ironicclient-5.2.0/ironicclient/v1/utils.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/v1/volume_connector.py` & `python-ironicclient-5.2.0/ironicclient/v1/volume_connector.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/ironicclient/v1/volume_target.py` & `python-ironicclient-5.2.0/ironicclient/v1/volume_target.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/playbooks/functional/run.yaml` & `python-ironicclient-5.2.0/playbooks/functional/run.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/python_ironicclient.egg-info/PKG-INFO` & `python-ironicclient-5.2.0/python_ironicclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ironicclient
-Version: 5.1.0
+Version: 5.2.0
 Summary: OpenStack Bare Metal Provisioning API Client Library
 Home-page: https://docs.openstack.org/python-ironicclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==================================
         Python bindings for the Ironic API
```

### Comparing `python-ironicclient-5.1.0/python_ironicclient.egg-info/SOURCES.txt` & `python-ironicclient-5.2.0/python_ironicclient.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,15 @@
 releasenotes/notes/bug-1524745-update-baremetal-node-set-c1ac57de0d481efe.yaml
 releasenotes/notes/bug-1712935-allow-os_baremetal_api_version_env_var_to_be_latest-28c8eed24f389673.yaml
 releasenotes/notes/bug-1724974-add-wanboot-to-supported-boot-devices.yaml
 releasenotes/notes/bug-1745099-allow-integer-portgroup-mode-6be4d3b35e216486.yaml
 releasenotes/notes/client-session-09e6ced1fbc6a9b0.yaml
 releasenotes/notes/conductor-group-9cfab3756aa108e4.yaml
 releasenotes/notes/configdrive-7bd2b67830691b2e.yaml
+releasenotes/notes/configdrive-json-b9d173dde111cf22.yaml
 releasenotes/notes/continue-del-next-node-8827e67e1c41a0a5.yaml
 releasenotes/notes/debug-e9dd680d783fa4b6.yaml
 releasenotes/notes/deploy-templates-df354ce825b00430.yaml
 releasenotes/notes/deprecate-http-client-8d664e5ec50ec403.yaml
 releasenotes/notes/deprecate-ironic-cli-686b7a238ddf3e25.yaml
 releasenotes/notes/display-empty-string-for-chassis-uuid-if-it-is-empty-a5471c3aa740a27d.yaml
 releasenotes/notes/driver-properties-for-osc-07a99d2d4e166436.yaml
@@ -222,14 +223,15 @@
 releasenotes/notes/latest-baremetal-api-version-a20e3099e3b97a1b.yaml
 releasenotes/notes/latest-default-41fdcc49701c4d70.yaml
 releasenotes/notes/latest-renegotiation-55daa01b3fc261be.yaml
 releasenotes/notes/list-nodes-by-driver-b1e1e1018077089b.yaml
 releasenotes/notes/logging-9c452e4869d80de9.yaml
 releasenotes/notes/manual-clean-09f6b49df7d2513f.yaml
 releasenotes/notes/missing-session-cc11e62dc966b4e0.yaml
+releasenotes/notes/multinode-actions-9f682ad5172f032f.yaml
 releasenotes/notes/negative-wrap-fix-4197e91b2ecfb722.yaml
 releasenotes/notes/network_data-c48b3878a5b04df5.yaml
 releasenotes/notes/no-automated-clean-0e437581ded44eb3.yaml
 releasenotes/notes/no-osc-requirement-411f25fd10f18caa.yaml
 releasenotes/notes/no-resource-attributeerror-d0cb327abab7dcc0.yaml
 releasenotes/notes/node-deploy-step-061e8925dfee3918.yaml
 releasenotes/notes/node-driver-support-storage-interface-e93fc8d4de5d24d6.yaml
@@ -291,14 +293,15 @@
 releasenotes/notes/switch-requests-8304d4465a8976b1.yaml
 releasenotes/notes/traits-support-8864f6816abecdb2.yaml
 releasenotes/notes/typerror-132801fe4541fdb4.yaml
 releasenotes/notes/version-overrides-4e9ba1266a238c6a.yaml
 releasenotes/notes/vif-attach-port-29a421b245e19f2b.yaml
 releasenotes/notes/wait-for-prov-last-error-5f49b1c488879775.yaml
 releasenotes/notes/yaml-files-79cd8367d7a4c2f2.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/mitaka.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
```

### Comparing `python-ironicclient-5.1.0/python_ironicclient.egg-info/entry_points.txt` & `python-ironicclient-5.2.0/python_ironicclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/accept-valid_interfaces-3b8f5e3e362e04cd.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/accept-valid_interfaces-3b8f5e3e362e04cd.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/add-create-command-3df5efbbecc33276.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/add-create-command-3df5efbbecc33276.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/add-deploy-steps-arg-0b127e29c8cf976d.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/add-deploy-steps-arg-0b127e29c8cf976d.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/add-volume-connector-api-873090474d5e41b8.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/add-volume-connector-api-873090474d5e41b8.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/add-volume-connector-cli-873090474d5e41b9.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/add-volume-connector-cli-873090474d5e41b9.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/add-volume-target-api-e062303f4b3b40ef.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/add-volume-target-api-e062303f4b3b40ef.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/add-volume-target-cli-e062303f4b3b40f0.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/add-volume-target-cli-e062303f4b3b40f0.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/allow-api-user-to-use-latest-6b80e9f584eaaa4e.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/allow-api-user-to-use-latest-6b80e9f584eaaa4e.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/bug-1524745-extend-driver-list-and-driver-show-800d96393aa17342.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/bug-1524745-extend-driver-list-and-driver-show-800d96393aa17342.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/deprecate-http-client-8d664e5ec50ec403.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/deprecate-http-client-8d664e5ec50ec403.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/ironic-cli-version-a5cdec73d585444d.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/ironic-cli-version-a5cdec73d585444d.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/latest-default-41fdcc49701c4d70.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/latest-default-41fdcc49701c4d70.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/manual-clean-09f6b49df7d2513f.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/manual-clean-09f6b49df7d2513f.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/no-osc-requirement-411f25fd10f18caa.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/no-osc-requirement-411f25fd10f18caa.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/node-driver-support-storage-interface-e93fc8d4de5d24d6.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/node-driver-support-storage-interface-e93fc8d4de5d24d6.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/osc-baremetal-node-bios-setting-list-b062b31d0d4de337.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/osc-baremetal-node-bios-setting-list-b062b31d0d4de337.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/osc-commands-1-7-d531960472a11ac2.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/osc-commands-1-7-d531960472a11ac2.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/osc-plugin-f87e0fbb472261dd.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-f87e0fbb472261dd.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/osc-plugin-ff0d897d8441a9e1.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-ff0d897d8441a9e1.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/osc-port-set-llc-pxeenabled-21fd8ea1982af17e.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/osc-port-set-llc-pxeenabled-21fd8ea1982af17e.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/prelude-2-0-release-ee44150902d3d399.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/prelude-2-0-release-ee44150902d3d399.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/remove-deprecated-osc-cmd-6dc980299d2fbde4.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/remove-deprecated-osc-cmd-6dc980299d2fbde4.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/support-passing-global-request-id-4b96beb31ec906cb.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/support-passing-global-request-id-4b96beb31ec906cb.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/notes/traits-support-8864f6816abecdb2.yaml` & `python-ironicclient-5.2.0/releasenotes/notes/traits-support-8864f6816abecdb2.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/releasenotes/source/conf.py` & `python-ironicclient-5.2.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/requirements.txt` & `python-ironicclient-5.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/setup.cfg` & `python-ironicclient-5.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/setup.py` & `python-ironicclient-5.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/tools/install_venv_common.py` & `python-ironicclient-5.2.0/tools/install_venv_common.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.1.0/tox.ini` & `python-ironicclient-5.2.0/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 deps =
   -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
   -r{toxinidir}/doc/requirements.txt
 commands = sphinx-build -a -E -W -d releasenotes/build/doctrees -b html releasenotes/source releasenotes/build/html
 
 [testenv:pep8]
 deps =
-    hacking>=3.1.0,<4.0.0 # Apache-2.0
+    hacking~=6.0.0 # Apache-2.0
     doc8>=0.6.0 # Apache-2.0
     flake8-import-order>=0.17.1 # LGPLv3
-    pycodestyle>=2.0.0,<2.7.0 # MIT
+    pycodestyle>=2.0.0,<3.0.0 # MIT
     Pygments>=2.2.0 # BSD
 commands =
     flake8 {posargs}
     doc8 doc/source CONTRIBUTING.rst README.rst
 
 [testenv:cover]
 setenv = {[testenv]setenv}
```

### Comparing `python-ironicclient-5.1.0/zuul.d/ironicclient-jobs.yaml` & `python-ironicclient-5.2.0/zuul.d/ironicclient-jobs.yaml`

 * *Files identical despite different names*

